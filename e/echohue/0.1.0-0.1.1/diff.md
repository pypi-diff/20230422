# Comparing `tmp/echohue-0.1.0.tar.gz` & `tmp/echohue-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echohue-0.1.0.tar", last modified: Fri Apr 21 16:05:11 2023, max compression
+gzip compressed data, was "echohue-0.1.1.tar", last modified: Sat Apr 22 14:41:23 2023, max compression
```

## Comparing `echohue-0.1.0.tar` & `echohue-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:11.948641 echohue-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-21 16:05:00.000000 echohue-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-21 16:05:11.948641 echohue-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-21 16:05:00.000000 echohue-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 16:05:00.000000 echohue-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 16:05:00.000000 echohue-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-21 16:05:11.948641 echohue-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:11.944640 echohue-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:11.944640 echohue-0.1.0/src/echohue/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 16:05:00.000000 echohue-0.1.0/src/echohue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44759 2023-04-21 16:05:00.000000 echohue-0.1.0/src/echohue/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:11.948641 echohue-0.1.0/src/echohue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-21 16:05:11.000000 echohue-0.1.0/src/echohue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-21 16:05:11.000000 echohue-0.1.0/src/echohue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:05:11.000000 echohue-0.1.0/src/echohue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 16:05:11.000000 echohue-0.1.0/src/echohue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 16:05:11.000000 echohue-0.1.0/src/echohue.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:11.948641 echohue-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-21 16:05:00.000000 echohue-0.1.0/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:41:23.732638 echohue-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 14:41:09.000000 echohue-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-22 14:41:23.732638 echohue-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-22 14:41:09.000000 echohue-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 14:41:09.000000 echohue-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-22 14:41:09.000000 echohue-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-22 14:41:23.732638 echohue-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:41:23.728638 echohue-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:41:23.732638 echohue-0.1.1/src/echohue/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-22 14:41:09.000000 echohue-0.1.1/src/echohue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 14:41:09.000000 echohue-0.1.1/src/echohue/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-22 14:41:09.000000 echohue-0.1.1/src/echohue/get-state.json
+-rw-r--r--   0 runner    (1001) docker     (123)    45248 2023-04-22 14:41:09.000000 echohue-0.1.1/src/echohue/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:41:23.732638 echohue-0.1.1/src/echohue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-22 14:41:23.000000 echohue-0.1.1/src/echohue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-22 14:41:23.000000 echohue-0.1.1/src/echohue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 14:41:23.000000 echohue-0.1.1/src/echohue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-22 14:41:23.000000 echohue-0.1.1/src/echohue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-22 14:41:23.000000 echohue-0.1.1/src/echohue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:41:23.732638 echohue-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-22 14:41:09.000000 echohue-0.1.1/test/test_server.py
```

### Comparing `echohue-0.1.0/LICENSE` & `echohue-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `echohue-0.1.0/setup.cfg` & `echohue-0.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -25,11 +25,14 @@
 	= src
 packages = find:
 install_requires = file: requirements.txt
 
 [options.packages.find]
 where = src
 
+[options.package_data]
+* = *.json
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `echohue-0.1.0/src/echohue/main.py` & `echohue-0.1.1/src/echohue/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,17 +188,20 @@
             try:
                 self.logger.debug("Waiting for M-SEARCH")
                 data, addr = await self.event_loop.sock_recvfrom(self.sock, 1024)
                 data = data.decode() # type: ignore
             # if socket closed by stop() method
             except ConnectionResetError:
                 break
-            except socket.error:
-                self.logger.error("Socket error")
-                continue
+            except socket.error as e:
+                if e.winerror == 995:
+                    break
+                else:
+                    self.logger.error(e)
+                    continue
             else:
                 if M_SEARCH_REQ_MATCH in data:
                     self.logger.debug("Received M-SEARCH from {}".format(addr))
 
                     if "urn:schemas-upnp-org:device:basic:1" in data:
                         self.logger.debug("received urn:schemas-upnp-org:device:basic:1")
                         
@@ -267,17 +270,21 @@
 
     async def loop(self):
         while True:
             try:
                 client, addr = await self.event_loop.sock_accept(self.sock)
             except ConnectionResetError:
                 break
-            except socket.error:
-                self.logger.error("Socket error")
-                continue
+            # if socket closed by stop() method [WinError 995] Der E/A-Vorgang wurde wegen eines Threadendes oder einer Anwendungsanforderung abgebrochen
+            except socket.error as e:
+                if e.winerror == 995:
+                    break
+                else:
+                    self.logger.error(e)
+                    continue
             else:
                 self.logger.debug("Received connection from {}".format(addr))
                 self.event_loop.create_task(self.handle(client, addr))
 
     async def handle(self, client:socket.socket, addr):
         try:
             
@@ -301,14 +308,18 @@
             else:
                 self.logger.debug("Received data from {}: {}".format(addr, data))
                 await self.handle_request(client, data)
                 client.close()
 
 
     async def handle_request(self, client, data):
+        if "test" in data:
+            await self.event_loop.sock_sendall(client, "ok".encode())
+            return
+
         searchObj = re.search(r'content-length: (\d+)', data, re.I)
         if searchObj and int(searchObj.group(1)) > 0:
             contentLength = int(searchObj.group(1))
             headerLength = data.find("\r\n\r\n") + 4
             self.logger.debug("Header-Length={} Content-Length={}".format(headerLength, contentLength))
             # got the header--now grab the remaining content if any
             #if len(data) < headerLength + contentLength:
@@ -743,15 +754,16 @@
             device.init(len(self.devices), self.logger)
             self.devices.append(device)
 
     async def run(self):
         global UPNP_BROADCAST, DESCRIPTION_XML, APICONFIG_JSON
         # same as the MACADDRESS with colons removed
         # Put our info in the responses
-        self.config["IP"] = self.get_ip()
+        if self.config.get("IP") is None:
+            self.config["IP"] = self.get_ip()
 
         UPNP_BROADCAST = UPNP_BROADCAST.format(self.config['IP'], self.config['HTTP_PORT'], self.config['SERIALNO'])
         DESCRIPTION_XML = DESCRIPTION_XML.format(self.config['IP'], self.config['HTTP_PORT'], self.config['IP'], self.config['SERIALNO'], self.config['SERIALNO'])
         APICONFIG_JSON = APICONFIG_JSON % (self.config['MACADDRESS'])
 
         self.responder = Responder(self.config, self.logger)
         self.broadcaster = Broadcaster(self.config, self.logger)
```

