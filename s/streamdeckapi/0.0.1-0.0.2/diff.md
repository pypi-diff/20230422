# Comparing `tmp/streamdeckapi-0.0.1.tar.gz` & `tmp/streamdeckapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamdeckapi-0.0.1.tar", last modified: Fri Apr 21 15:44:39 2023, max compression
+gzip compressed data, was "streamdeckapi-0.0.2.tar", last modified: Sat Apr 22 12:03:02 2023, max compression
```

## Comparing `streamdeckapi-0.0.1.tar` & `streamdeckapi-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:44:39.247705 streamdeckapi-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-21 15:44:39.247705 streamdeckapi-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-21 15:44:27.000000 streamdeckapi-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 15:44:39.247705 streamdeckapi-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-21 15:44:27.000000 streamdeckapi-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:44:39.243705 streamdeckapi-0.0.1/streamdeckapi/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-21 15:44:27.000000 streamdeckapi-0.0.1/streamdeckapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-04-21 15:44:27.000000 streamdeckapi-0.0.1/streamdeckapi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-21 15:44:27.000000 streamdeckapi-0.0.1/streamdeckapi/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-21 15:44:27.000000 streamdeckapi-0.0.1/streamdeckapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:44:39.243705 streamdeckapi-0.0.1/streamdeckapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-21 15:44:39.000000 streamdeckapi-0.0.1/streamdeckapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-21 15:44:39.000000 streamdeckapi-0.0.1/streamdeckapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:44:39.000000 streamdeckapi-0.0.1/streamdeckapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 15:44:39.000000 streamdeckapi-0.0.1/streamdeckapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 15:44:39.000000 streamdeckapi-0.0.1/streamdeckapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:03:02.724804 streamdeckapi-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-22 12:03:02.724804 streamdeckapi-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-22 12:02:46.000000 streamdeckapi-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 12:03:02.724804 streamdeckapi-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-22 12:02:46.000000 streamdeckapi-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:03:02.724804 streamdeckapi-0.0.2/streamdeckapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-22 12:02:46.000000 streamdeckapi-0.0.2/streamdeckapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-04-22 12:02:46.000000 streamdeckapi-0.0.2/streamdeckapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-22 12:02:46.000000 streamdeckapi-0.0.2/streamdeckapi/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-22 12:02:46.000000 streamdeckapi-0.0.2/streamdeckapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:03:02.724804 streamdeckapi-0.0.2/streamdeckapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-22 12:03:02.000000 streamdeckapi-0.0.2/streamdeckapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-22 12:03:02.000000 streamdeckapi-0.0.2/streamdeckapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 12:03:02.000000 streamdeckapi-0.0.2/streamdeckapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 12:03:02.000000 streamdeckapi-0.0.2/streamdeckapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-22 12:03:02.000000 streamdeckapi-0.0.2/streamdeckapi.egg-info/top_level.txt
```

### Comparing `streamdeckapi-0.0.1/PKG-INFO` & `streamdeckapi-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeckapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Stream Deck API Library
 Home-page: https://github.com/Patrick762/streamdeckapi
 Author: Patrick762
 Author-email: <pip-stream-deck-api@hosting-rt.de>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `streamdeckapi-0.0.1/setup.py` & `streamdeckapi-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Stream Deck API Library'
 
 # Setting up
 setup(
     name="streamdeckapi",
     version=VERSION,
     author="Patrick762",
```

### Comparing `streamdeckapi-0.0.1/streamdeckapi/api.py` & `streamdeckapi-0.0.2/streamdeckapi/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,21 +24,23 @@
     def __init__(
         self,
         host: str,
         on_button_press: Callable[[str], None] | None = None,
         on_button_release: Callable[[str], None] | None = None,
         on_status_update: Callable[[SDInfo], None] | None = None,
         on_ws_message: Callable[[SDWebsocketMessage], None] | None = None,
+        on_ws_connect: Callable[[], None] | None = None,
     ) -> None:
         """Init Stream Deck API object."""
         self._host = host
         self._on_button_press = on_button_press
         self._on_button_release = on_button_release
         self._on_status_update = on_status_update
         self._on_ws_message = on_ws_message
+        self._on_ws_connect = on_ws_connect
         self._loop = asyncio.get_event_loop()
         self._running = False
         self._task: asyncio.Task | None = None
 
     #
     #   Properties
     #
@@ -86,18 +88,18 @@
 
     @staticmethod
     def _post_request(url: str, data: str, headers) -> None | requests.Response:
         """Handle POST requests."""
         try:
             res = requests.post(url, data, headers=headers, timeout=5)
         except requests.RequestException:
-            _LOGGER.error("Error sending data to Stream Deck Plugin (exception)")
+            _LOGGER.debug("Error sending data to Stream Deck Plugin (exception)")
             return None
         if res.status_code != 200:
-            _LOGGER.info(
+            _LOGGER.debug(
                 "Error sending data to Stream Deck Plugin (%s). Is the button currently visible?",
                 res.reason,
             )
             return None
         return res
 
     async def get_info(self, in_executor: bool = True) -> None | SDInfo:
@@ -110,31 +112,31 @@
         else:
             res = self._get_request(self._info_url)
         if res is None or res.status_code != 200:
             return None
         try:
             rjson = res.json()
         except requests.JSONDecodeError:
-            _LOGGER.error("Error decoding response from %s", self._info_url)
+            _LOGGER.debug("Error decoding response from %s", self._info_url)
             return None
         try:
             info = SDInfo(rjson)
         except KeyError:
-            _LOGGER.error("Error parsing response from %s to SDInfo", self._info_url)
+            _LOGGER.debug("Error parsing response from %s to SDInfo", self._info_url)
             return None
         return info
 
     async def get_icon(self, btn: str) -> None | str:
         """Get svg icon from Stream Deck button."""
         url = f"{self._icon_url}{btn}"
         res = await self._loop.run_in_executor(None, self._get_request, url)
         if res is None or res.status_code != 200:
             return None
         if res.headers.get("Content-Type", "") != "image/svg+xml":
-            _LOGGER.error("Invalid content type received from %s", url)
+            _LOGGER.debug("Invalid content type received from %s", url)
             return None
         return res.text
 
     async def update_icon(self, btn: str, svg: str) -> bool:
         """Update svg icon of Stream Deck button."""
         url = f"{self._icon_url}{btn}"
         res = await self._loop.run_in_executor(
@@ -174,20 +176,20 @@
             return
 
         _LOGGER.debug(msg)
 
         try:
             datajson = json.loads(msg)
         except json.JSONDecodeError:
-            _LOGGER.warning("Method _on_message: Websocket message couldn't get parsed")
+            _LOGGER.debug("Method _on_message: Websocket message couldn't get parsed")
             return
         try:
             data = SDWebsocketMessage(datajson)
         except KeyError:
-            _LOGGER.warning(
+            _LOGGER.debug(
                 "Method _on_message: Websocket message couldn't get parsed to SDWebsocketMessage"
             )
             return
 
         _LOGGER.debug("Method _on_message: Got event %s", data.event)
 
         if self._on_ws_message is not None:
@@ -208,35 +210,37 @@
 
     async def _websocket_loop(self):
         """Start the websocket client loop."""
         self._running = True
         while self._running:
             info = await self.get_info()
             if isinstance(info, SDInfo):
-                _LOGGER.info("Method _websocket_loop: Streamdeck online")
+                _LOGGER.debug("Method _websocket_loop: Streamdeck online")
                 try:
                     async with connect(self._websocket_url) as websocket:
+                        if self._on_ws_connect is not None:
+                            self._on_ws_connect()
                         try:
                             while self._running:
                                 data = await asyncio.wait_for(
                                     websocket.recv(), timeout=60
                                 )
                                 self._on_message(data)
                             await websocket.close()
-                            _LOGGER.info("Method _websocket_loop: Websocket closed")
+                            _LOGGER.debug("Method _websocket_loop: Websocket closed")
                         except WebSocketException:
-                            _LOGGER.warning(
+                            _LOGGER.debug(
                                 "Method _websocket_loop: Websocket client crashed. Restarting it"
                             )
                         except asyncio.TimeoutError:
-                            _LOGGER.warning(
+                            _LOGGER.debug(
                                 "Method _websocket_loop: Websocket client timed out. Restarting it"
                             )
                 except WebSocketException:
-                    _LOGGER.warning(
+                    _LOGGER.debug(
                         "Method _websocket_loop: Websocket client not connecting. Restarting it"
                     )
 
     def start_websocket_loop(self):
         """Start the websocket client."""
         self._task = asyncio.create_task(self._websocket_loop())
```

### Comparing `streamdeckapi-0.0.1/streamdeckapi/tools.py` & `streamdeckapi-0.0.2/streamdeckapi/tools.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.1/streamdeckapi/types.py` & `streamdeckapi-0.0.2/streamdeckapi/types.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.1/streamdeckapi.egg-info/PKG-INFO` & `streamdeckapi-0.0.2/streamdeckapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeckapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Stream Deck API Library
 Home-page: https://github.com/Patrick762/streamdeckapi
 Author: Patrick762
 Author-email: <pip-stream-deck-api@hosting-rt.de>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

