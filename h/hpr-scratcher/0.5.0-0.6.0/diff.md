# Comparing `tmp/hpr_scratcher-0.5.0.tar.gz` & `tmp/hpr_scratcher-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpr_scratcher-0.5.0.tar", max compression
+gzip compressed data, was "hpr_scratcher-0.6.0.tar", max compression
```

## Comparing `hpr_scratcher-0.5.0.tar` & `hpr_scratcher-0.6.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2957 2023-04-19 15:25:07.637443 hpr_scratcher-0.5.0/README.md
--rwxr-xr-x   0        0        0    13721 2023-04-19 15:10:02.799997 hpr_scratcher-0.5.0/hpr_scratcher/__init__.py
--rw-r--r--   0        0        0      479 2023-04-19 15:24:57.870300 hpr_scratcher-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3451 1970-01-01 00:00:00.000000 hpr_scratcher-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3147 2023-04-22 13:17:50.013907 hpr_scratcher-0.6.0/README.md
+-rwxr-xr-x   0        0        0    15800 2023-04-21 19:41:03.866374 hpr_scratcher-0.6.0/hpr_scratcher/__init__.py
+-rw-r--r--   0        0        0      479 2023-04-22 13:16:59.162457 hpr_scratcher-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 hpr_scratcher-0.6.0/PKG-INFO
```

### Comparing `hpr_scratcher-0.5.0/README.md` & `hpr_scratcher-0.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ```
 
 Then in $HOME/.config/hypr/scratchpads.json add:
 
 ```json
 {
   "term": {
-    "command": "kitty",
+    "command": "kitty --class kitty-dropterm",
     "animation": "fromTop",
     "margin": 50,
     "unfocus": "hide"
   },
   "volume": {
     "command": "pavucontrol",
     "animation": "fromRight"
@@ -65,14 +65,19 @@
 - `show <scratchpad name>` : show the given scratchpad
 - `hide <scratchpad name>` : hide the given scratchpad
 
 Note: with no argument it runs the daemon (doesn't fork in the background)
 
 ## Scratchpad Options
 
+### command
+
+This is the command you wish to run in the scratchpad.
+For a nice startup you need to be able to identify this window in `hyprland.conf`, using `--class` is often a good idea.
+
 ### animation
 
 Type of animation to use
 
 - `null` / `""` / not defined
 - "fromTop"
 - "fromBottom"
@@ -89,14 +94,20 @@
 
 ### margin (optional)
 
 number of pixels for the margin
 
 # Changelog
 
+# 0.6.0
+
+- animation names are case-insensitive now
+- drop `hyprctl` dependency
+- auto-restarts applications when needed
+
 # 0.5.0
 
 - windows can slide from any direction now (values for "animation" property):
   - `fromTop`
   - `fromBottom`
   - `fromLeft`
   - `fromRight`
@@ -123,13 +134,7 @@
 
 - add a "reload" command re-reading the configuration
 - allow automatic hiding on focus
 
 # 0.1.0
 
 - first version, close to no options
-
-# TODO
-
-- Allow auto-restart of applications (if closed)
-  - Allow closing the app on unfocus
-- Move to socket instead of hyprctl when possible
```

### Comparing `hpr_scratcher-0.5.0/hpr_scratcher/__init__.py` & `hpr_scratcher-0.6.0/hpr_scratcher/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,86 +4,108 @@
 import time
 import json
 import sys
 import os
 
 DEBUG = os.environ.get("DEBUG", False)
 
-MARGIN = 60  # TODO take it from JSON config
+HYPRCTL = f'/tmp/hypr/{ os.environ["HYPRLAND_INSTANCE_SIGNATURE"] }/.socket.sock'
 EVENTS = f'/tmp/hypr/{ os.environ["HYPRLAND_INSTANCE_SIGNATURE"] }/.socket2.sock'
 CONTROL = f'/tmp/hypr/{ os.environ["HYPRLAND_INSTANCE_SIGNATURE"] }/.scratchpads.sock'
 
 CONFIG_FILE = "~/.config/hypr/scratchpads.json"
+DEFAULT_MARGIN = 60
 
 
-def hyprctlJSON(command):
+async def hyprctlJSON(command):
     if DEBUG:
         print("(JS)>>>", command)
-    return json.loads(subprocess.getoutput(f"hyprctl -j {command}"))
+    ctl_reader, ctl_writer = await asyncio.open_unix_connection(HYPRCTL)
+    ctl_writer.write(f"-j/{command}".encode())
+    await ctl_writer.drain()
+    resp = await ctl_reader.read()
+    ctl_writer.close()
+    await ctl_writer.wait_closed()
+    return json.loads(resp)
 
 
-def hyprctl(command):
+async def hyprctl(command):
     if DEBUG:
         print(">>>", command)
-    subprocess.call(
-        ["hyprctl", "dispatch", command],
-        stdout=subprocess.DEVNULL,
-        stderr=subprocess.DEVNULL,
-    )
+    ctl_reader, ctl_writer = await asyncio.open_unix_connection(HYPRCTL)
+    ctl_writer.write(f"/dispatch {command}".encode())
+    await ctl_writer.drain()
+    resp = await ctl_reader.read(100)
+    ctl_writer.close()
+    await ctl_writer.wait_closed()
+    if DEBUG:
+        print("<<<", resp)
+    return resp == b"ok"
 
 
-def get_focused_monitor_props():
-    for monitor in hyprctlJSON("monitors"):
+async def get_focused_monitor_props():
+    for monitor in await hyprctlJSON("monitors"):
         if monitor.get("focused") == True:
             return monitor
 
 
-def get_client_props_by_pid(pid: int):
-    for client in hyprctlJSON("clients"):
+async def get_client_props_by_pid(pid: int):
+    for client in await hyprctlJSON("clients"):
         if client.get("pid") == pid:
             return client
 
 
 class Scratch:
     def __init__(self, uid, opts):
         self.uid = uid
         self.pid = 0
         self.conf = opts
         self.visible = False
         self.just_created = True
         self.clientInfo = {}
-        self.scratches = {}
+
+    def isAlive(self):
+        path = f"/proc/{self.pid}"
+        if os.path.exists(path):
+            for line in open(os.path.join(path, "status"), "r").readlines():
+                if line.startswith("State"):
+                    state = line.split()[1]
+                    return state in "RSDTt"  # not "Z (zombie)"or "X (dead)"
+        return False
+
+    def reset(self, pid: int):
+        self.pid = pid
+        self.visible = False
+        self.just_created = True
+        self.clientInfo = {}
 
     @property
-    def address(self):
-        return self.clientInfo.get("address", "")[2:]
+    def address(self) -> str:
+        return str(self.clientInfo.get("address", ""))[2:]
 
-    def updateClientInfo(self, clientInfo=None):
+    async def updateClientInfo(self, clientInfo=None):
         if clientInfo is None:
-            clientInfo = get_client_props_by_pid(self.pid)
+            clientInfo = await get_client_props_by_pid(self.pid)
         assert clientInfo
         self.clientInfo.update(clientInfo)
 
 
 class ScratchpadManager:
     server: asyncio.Server
     event_reader: asyncio.StreamReader
     stopped = False
 
     def __init__(self):
         self.procs = {}
         self.scratches = {}
         self.transitioning_scratches = set()
         self.startedAt = time.time()
+        self._respawned_scratches = set()
         self.load_config()
 
-    @property
-    def is_starting(self):
-        return time.time() - self.startedAt < 10
-
     def load_config(self):
         config = json.loads(
             open(os.path.expanduser(CONFIG_FILE), encoding="utf-8").read()
         )
         scratches = {k: Scratch(k, v) for k, v in config.items()}
 
         is_updating = not bool(self.scratches)
@@ -99,28 +121,35 @@
                 if name not in scratches:
                     del self.scratches[name]
 
         # not known yet
         self.scratches_by_address = {}
         self.scratches_by_pid = {}
 
+    def start_scratch_command(self, name: str):
+        self._respawned_scratches.add(name)
+        scratch = self.scratches[name]
+        old_pid = self.procs[name].pid if name in self.procs else 0
+        self.procs[name] = subprocess.Popen(
+            scratch.conf["command"],
+            stdin=subprocess.DEVNULL,
+            stdout=subprocess.DEVNULL,
+            stderr=subprocess.DEVNULL,
+            shell=True,
+        )
+        pid = self.procs[name].pid
+        self.scratches[name].reset(pid)
+        self.scratches_by_pid[self.procs[name].pid] = scratch
+        if old_pid:
+            del self.scratches_by_pid[old_pid]
+
     def load_clients(self):
-        self.procs = {
-            name: subprocess.Popen(
-                scratch.conf["command"],
-                stdin=subprocess.DEVNULL,
-                stdout=subprocess.DEVNULL,
-                stderr=subprocess.DEVNULL,
-                shell=True,
-            )
-            for name, scratch in self.scratches.items()
-        }
-        for name, proc in self.procs.items():
-            self.scratches[name].pid = proc.pid
-            self.scratches_by_pid[proc.pid] = self.scratches[name]
+        self.procs = {}
+        for name in self.scratches:
+            self.start_scratch_command(name)
 
     # event handlers:
 
     async def event_moveworkspace(self, params):
         pass
 
     async def event_openlayer(self, params):
@@ -173,22 +202,23 @@
                     ):
                         await self.run_hide(uid)
 
     async def event_openwindow(self, params):
         addr, wrkspc, kls, title = params.split(",", 3)
         if wrkspc == "special":
             item = self.scratches_by_address.get(addr)
-            if not item and self.is_starting:
-                self.updateScratchInfo()
+            if not item and self._respawned_scratches:
+                await self.updateScratchInfo()
                 item = self.scratches_by_address.get(addr)
             if item and item.just_created:
+                self._respawned_scratches.discard(item.uid)
                 await self.run_hide(item.uid, force=True)
                 item.just_created = False
 
-    async def event_activewindow(self, params):
+    async def event_activewindow(self, params):  # XXX: do not use
         return
 
     # command handlers
 
     async def run_reload(self):
         self.load_config()
 
@@ -199,106 +229,106 @@
             print(f"{uid} is not configured")
             return
         if item.visible:
             await self.run_hide(uid)
         else:
             await self.run_show(uid)
 
-    def updateScratchInfo(self, scratch: Scratch | None = None):
+    async def updateScratchInfo(self, scratch: Scratch | None = None):
         if scratch is None:
-            for client in hyprctlJSON("clients"):
+            for client in await hyprctlJSON("clients"):
                 scratch = self.scratches_by_pid.get(client["pid"])
                 if scratch:
-                    scratch.updateClientInfo(client)
+                    await scratch.updateClientInfo(client)
                     self.scratches_by_address[
                         scratch.clientInfo["address"][2:]
                     ] = scratch
         else:
             add_to_address_book = ("address" not in scratch.clientInfo) or (
                 scratch.address not in self.scratches_by_address
             )
-            scratch.updateClientInfo()
+            await scratch.updateClientInfo()
             if add_to_address_book:
                 self.scratches_by_address[scratch.clientInfo["address"][2:]] = scratch
 
     async def run_hide(self, uid: str, force=False):
         uid = uid.strip()
         item = self.scratches.get(uid)
         if not item:
             print(f"{uid} is not configured")
             return
         if not item.visible and not force:
             print(f"{uid} is already hidden")
             return
         item.visible = False
         pid = "pid:%d" % item.pid
-        animation_type = item.conf.get("animation")
+        animation_type = item.conf.get("animation", "").lower()
         if animation_type:
             offset = item.conf.get("offset")
             if offset is None:
                 if "size" not in item.clientInfo:
-                    self.updateScratchInfo(item)
+                    await self.updateScratchInfo(item)
 
                 offset = int(1.3 * item.clientInfo["size"][1])
 
-            if animation_type == "fromTop":
-                hyprctl(f"movewindowpixel 0 -{offset},{pid}")
-            elif animation_type == "fromBottom":
-                hyprctl(f"movewindowpixel 0 {offset},{pid}")
-            elif animation_type == "fromLeft":
-                hyprctl(f"movewindowpixel -{offset} 0,{pid}")
-            elif animation_type == "fromRight":
-                hyprctl(f"movewindowpixel {offset} 0,{pid}")
+            if animation_type == "fromtop":
+                await hyprctl(f"movewindowpixel 0 -{offset},{pid}")
+            elif animation_type == "frombottom":
+                await hyprctl(f"movewindowpixel 0 {offset},{pid}")
+            elif animation_type == "fromleft":
+                await hyprctl(f"movewindowpixel -{offset} 0,{pid}")
+            elif animation_type == "fromright":
+                await hyprctl(f"movewindowpixel {offset} 0,{pid}")
 
             if uid in self.transitioning_scratches:
                 return  # abort sequence
-            await asyncio.sleep(0.2)
+            await asyncio.sleep(0.2)  # await for animation to finish
         if uid not in self.transitioning_scratches:
-            hyprctl(f"movetoworkspacesilent special,{pid}")
+            await hyprctl(f"movetoworkspacesilent special,{pid}")
 
-    def _animation_fromTop(self, monitor, client, client_uid, margin):
+    async def _animation_fromtop(self, monitor, client, client_uid, margin):
         mon_x = monitor["x"]
         mon_y = monitor["y"]
         mon_width = monitor["width"]
 
         client_width = client["size"][0]
         margin_x = int((mon_width - client_width) / 2) + mon_x
-        hyprctl(f"movewindowpixel exact {margin_x} {mon_y + margin},{client_uid}")
+        await hyprctl(f"movewindowpixel exact {margin_x} {mon_y + margin},{client_uid}")
 
-    def _animation_fromBottom(self, monitor, client, client_uid, margin):
+    async def _animation_frombottom(self, monitor, client, client_uid, margin):
         mon_x = monitor["x"]
         mon_y = monitor["y"]
         mon_width = monitor["width"]
         mon_height = monitor["height"]
 
         client_width = client["size"][0]
         client_height = client["size"][1]
         margin_x = int((mon_width - client_width) / 2) + mon_x
-        hyprctl(
+        await hyprctl(
             f"movewindowpixel exact {margin_x} {mon_y + mon_height - client_height - margin},{client_uid}"
         )
 
-    def _animation_fromLeft(self, monitor, client, client_uid, margin):
+    async def _animation_fromleft(self, monitor, client, client_uid, margin):
         mon_y = monitor["y"]
         mon_height = monitor["height"]
 
         client_height = client["size"][1]
         margin_y = int((mon_height - client_height) / 2) + mon_y
 
-        hyprctl(f"movewindowpixel exact {margin} {margin_y},{client_uid}")
+        await hyprctl(f"movewindowpixel exact {margin} {margin_y},{client_uid}")
 
-    def _animation_fromRight(self, monitor, client, client_uid, margin):
+    async def _animation_fromright(self, monitor, client, client_uid, margin):
         mon_y = monitor["y"]
         mon_width = monitor["width"]
         mon_height = monitor["height"]
 
         client_width = client["size"][0]
         client_height = client["size"][1]
         margin_y = int((mon_height - client_height) / 2) + mon_y
-        hyprctl(
+        await hyprctl(
             f"movewindowpixel exact {mon_width - client_width - margin} {margin_y},{client_uid}"
         )
 
     async def run_show(self, uid, force=False):
         uid = uid.strip()
         item = self.scratches.get(uid)
 
@@ -306,36 +336,43 @@
             print(f"{uid} is not configured")
             return
 
         if item.visible and not force:
             print(f"{uid} is already visible")
             return
 
+        if not item.isAlive():
+            print(f"{uid} is not running, restarting...")
+            self.procs[uid].kill()
+            self.start_scratch_command(uid)
+            while uid in self._respawned_scratches:
+                await asyncio.sleep(0.05)
+
         item.visible = True
-        monitor = get_focused_monitor_props()
+        monitor = await get_focused_monitor_props()
         assert monitor
 
-        self.updateScratchInfo(item)
+        await self.updateScratchInfo(item)
 
         pid = "pid:%d" % item.pid
 
-        animation_type = item.conf.get("animation")
+        animation_type = item.conf.get("animation", "").lower()
 
         wrkspc = monitor["activeWorkspace"]["id"]
         self.transitioning_scratches.add(uid)
-        hyprctl(f"movetoworkspacesilent {wrkspc},{pid}")
+        await hyprctl(f"movetoworkspacesilent {wrkspc},{pid}")
         if animation_type:
-            margin = item.conf.get("margin", MARGIN)
+            margin = item.conf.get("margin", DEFAULT_MARGIN)
             fn = getattr(self, "_animation_%s" % animation_type)
-            fn(monitor, item.clientInfo, pid, margin)
+            await fn(monitor, item.clientInfo, pid, margin)
 
         # FIXME: pin doesn't always work
-        # hyprctl(f"pin {pid}")
-        hyprctl(f"focuswindow {pid}")
-        await asyncio.sleep(0.2)
+        # await hyprctl(f"pin {pid}")
+        await hyprctl(f"focuswindow {pid}")
+        await asyncio.sleep(0.2)  # ensure some time for events to propagate
         self.transitioning_scratches.discard(uid)
 
     # Async loops & handlers (dispatchers):
 
     async def read_events_loop(self):
         while not self.stopped:
             data = (await self.event_reader.readline()).decode()
@@ -378,21 +415,30 @@
             print("Unknown command:", cmd)
 
     async def serve(self):
         try:
             async with self.server:
                 await self.server.serve_forever()
         finally:
-            for scratch in self.scratches:
-                proc = self.procs[scratch]
+
+            async def die_in_piece(scratch: Scratch):
+                proc = self.procs[scratch.uid]
                 proc.terminate()
-                await asyncio.sleep(0.1)
-                proc.kill()
+                for n in range(10):
+                    if not scratch.isAlive():
+                        break
+                    await asyncio.sleep(0.1)
+                if scratch.isAlive():
+                    proc.kill()
                 proc.wait()
 
+            await asyncio.gather(
+                *(die_in_piece(scratch) for scratch in self.scratches.values())
+            )
+
     async def run(self):
         await asyncio.gather(
             asyncio.create_task(self.serve()),
             asyncio.create_task(self.read_events_loop()),
         )
```

### Comparing `hpr_scratcher-0.5.0/PKG-INFO` & `hpr_scratcher-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpr-scratcher
-Version: 0.5.0
+Version: 0.6.0
 Summary: A scratchpad manager for hyprland
 Home-page: https://github.com/hyprland-community/hpr-scratcher
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -55,15 +55,15 @@
 ```
 
 Then in $HOME/.config/hypr/scratchpads.json add:
 
 ```json
 {
   "term": {
-    "command": "kitty",
+    "command": "kitty --class kitty-dropterm",
     "animation": "fromTop",
     "margin": 50,
     "unfocus": "hide"
   },
   "volume": {
     "command": "pavucontrol",
     "animation": "fromRight"
@@ -80,14 +80,19 @@
 - `show <scratchpad name>` : show the given scratchpad
 - `hide <scratchpad name>` : hide the given scratchpad
 
 Note: with no argument it runs the daemon (doesn't fork in the background)
 
 ## Scratchpad Options
 
+### command
+
+This is the command you wish to run in the scratchpad.
+For a nice startup you need to be able to identify this window in `hyprland.conf`, using `--class` is often a good idea.
+
 ### animation
 
 Type of animation to use
 
 - `null` / `""` / not defined
 - "fromTop"
 - "fromBottom"
@@ -104,14 +109,20 @@
 
 ### margin (optional)
 
 number of pixels for the margin
 
 # Changelog
 
+# 0.6.0
+
+- animation names are case-insensitive now
+- drop `hyprctl` dependency
+- auto-restarts applications when needed
+
 # 0.5.0
 
 - windows can slide from any direction now (values for "animation" property):
   - `fromTop`
   - `fromBottom`
   - `fromLeft`
   - `fromRight`
@@ -139,13 +150,7 @@
 - add a "reload" command re-reading the configuration
 - allow automatic hiding on focus
 
 # 0.1.0
 
 - first version, close to no options
 
-# TODO
-
-- Allow auto-restart of applications (if closed)
-  - Allow closing the app on unfocus
-- Move to socket instead of hyprctl when possible
-
```

