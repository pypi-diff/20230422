# Comparing `tmp/echohue-0.1.1.tar.gz` & `tmp/echohue-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echohue-0.1.1.tar", last modified: Sat Apr 22 14:41:23 2023, max compression
+gzip compressed data, was "echohue-0.1.2.tar", last modified: Sat Apr 22 15:03:18 2023, max compression
```

## Comparing `echohue-0.1.1.tar` & `echohue-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:41:23.732638 echohue-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 14:41:09.000000 echohue-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-22 14:41:23.732638 echohue-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-22 14:41:09.000000 echohue-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 14:41:09.000000 echohue-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-22 14:41:09.000000 echohue-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-22 14:41:23.732638 echohue-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:41:23.728638 echohue-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:41:23.732638 echohue-0.1.1/src/echohue/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-22 14:41:09.000000 echohue-0.1.1/src/echohue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 14:41:09.000000 echohue-0.1.1/src/echohue/all.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-22 14:41:09.000000 echohue-0.1.1/src/echohue/get-state.json
--rw-r--r--   0 runner    (1001) docker     (123)    45248 2023-04-22 14:41:09.000000 echohue-0.1.1/src/echohue/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:41:23.732638 echohue-0.1.1/src/echohue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-22 14:41:23.000000 echohue-0.1.1/src/echohue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-22 14:41:23.000000 echohue-0.1.1/src/echohue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 14:41:23.000000 echohue-0.1.1/src/echohue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-22 14:41:23.000000 echohue-0.1.1/src/echohue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-22 14:41:23.000000 echohue-0.1.1/src/echohue.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:41:23.732638 echohue-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-22 14:41:09.000000 echohue-0.1.1/test/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:03:18.043933 echohue-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 15:03:07.000000 echohue-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-22 15:03:18.043933 echohue-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-22 15:03:07.000000 echohue-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 15:03:07.000000 echohue-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 15:03:07.000000 echohue-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-22 15:03:18.043933 echohue-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:03:18.043933 echohue-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:03:18.043933 echohue-0.1.2/src/echohue/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-22 15:03:07.000000 echohue-0.1.2/src/echohue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-22 15:03:07.000000 echohue-0.1.2/src/echohue/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45156 2023-04-22 15:03:07.000000 echohue-0.1.2/src/echohue/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:03:18.043933 echohue-0.1.2/src/echohue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-22 15:03:18.000000 echohue-0.1.2/src/echohue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-22 15:03:18.000000 echohue-0.1.2/src/echohue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 15:03:18.000000 echohue-0.1.2/src/echohue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-22 15:03:18.000000 echohue-0.1.2/src/echohue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:03:18.043933 echohue-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-22 15:03:07.000000 echohue-0.1.2/test/test_server.py
```

### Comparing `echohue-0.1.1/LICENSE` & `echohue-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `echohue-0.1.1/PKG-INFO` & `echohue-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echohue
-Version: 0.1.1
+Version: 0.1.2
 Summary: Philips Hue lamp emulation for Amazon Echo
 Home-page: https://github.com/mightytry/alexa-echo-hue
 Author: mightytry
 Author-email: 
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mightytry/alexa-echo-hue/issues
 Project-URL: Docs, https://github.com/mightytry/alexa-echo-hue
```

### Comparing `echohue-0.1.1/README.md` & `echohue-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `echohue-0.1.1/setup.cfg` & `echohue-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `echohue-0.1.1/src/echohue/main.py` & `echohue-0.1.2/src/echohue/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import asyncio
 from contextlib import AbstractAsyncContextManager
+import copy
 import datetime
 import socket
 import struct
 import email.utils
 import uuid
-from aiofile import async_open
 import re
 import sys
 import logging
 import logging.handlers
 import json
+from .defaults import ALL, GETSTATE
 
 M_SEARCH_REQ_MATCH = "M-SEARCH"
 
 UPNP_BROADCAST = """NOTIFY * HTTP/1.1
 HOST: 239.255.255.250:1900
 CACHE-CONTROL: max-age=100
 LOCATION: http://{}:{}/description.xml
@@ -437,43 +438,42 @@
 
         self.logger.debug("-------------------------------")
         self.logger.debug("    ")
 
     async def get_onelight_json(self, device):
         # example template values: "on", "[0.0,0.0]", "Hue Lamp 1", "254", "201"
         # on, bri, xy, ct, name
-        data = await self.get_json_att(device, "./all.json")
+        data = await self.get_json_att(device, ALL)
         data["uniqueid"] = self.gen_unique_id()
         return json.dumps(data)
     
     def gen_unique_id(self):
         # gen "00:11:22:33:44:55:66:77-88" like id
         serial = uuid.uuid4().hex[:18]
         return ":".join([serial[i:i+2] for i in range(0, len(serial)-2, 2)]) + "-" + str(serial[-2:])
 
     async def get_onelight_state_json(self, device):
         # example template values: "on", "[0.0,0.0]", "Hue Lamp 1", "254", "201"
         # on, bri, xy, ct, name
-        return json.dumps(await self.get_json_att(device, "./get-state.json"))
+        return json.dumps(await self.get_json_att(device, GETSTATE))
 
-    async def get_json_att(self, device, path):
-        async with async_open(path, 'r') as f:
-            json_resp = json.loads(await f.read())
-
-            json_resp["state"]["on"] = device.on
-            json_resp["state"]["hue"] = device.hue
-            json_resp["state"]["sat"] = device.sat
-            json_resp["state"]["bri"] = device.bri
-            json_resp["state"]["ct"] = device.ct
-            json_resp["state"]["xy"] = device.xy
-            json_resp["state"]["colormode"] = device.colormode
-            json_resp["name"] = device.name
-            json_resp["swupdate"]["lastinstall"] = datetime.datetime.now().isoformat().split(".")[0]
+    async def get_json_att(self, device, template):
+        json_resp = copy.deepcopy(template)
 
-            return json_resp
+        json_resp["state"]["on"] = device.on
+        json_resp["state"]["hue"] = device.hue
+        json_resp["state"]["sat"] = device.sat
+        json_resp["state"]["bri"] = device.bri
+        json_resp["state"]["ct"] = device.ct
+        json_resp["state"]["xy"] = device.xy
+        json_resp["state"]["colormode"] = device.colormode
+        json_resp["name"] = device.name
+        json_resp["swupdate"]["lastinstall"] = datetime.datetime.now().isoformat().split(".")[0]
+
+        return json_resp
 
     async def send_json(self, client, resp):
         date_str = email.utils.formatdate(timeval=None, localtime=False, usegmt=True)
         full_resp = (JSON_HEADERS %(len(resp), date_str, resp)).replace("\n", "\r\n")
         await self.event_loop.sock_sendall(client, full_resp.encode())
 
     async def stop(self):
```

### Comparing `echohue-0.1.1/src/echohue.egg-info/PKG-INFO` & `echohue-0.1.2/src/echohue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echohue
-Version: 0.1.1
+Version: 0.1.2
 Summary: Philips Hue lamp emulation for Amazon Echo
 Home-page: https://github.com/mightytry/alexa-echo-hue
 Author: mightytry
 Author-email: 
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mightytry/alexa-echo-hue/issues
 Project-URL: Docs, https://github.com/mightytry/alexa-echo-hue
```

### Comparing `echohue-0.1.1/test/test_server.py` & `echohue-0.1.2/test/test_server.py`

 * *Files identical despite different names*

