# Comparing `tmp/whirlpool_sixth_sense-0.18.2.tar.gz` & `tmp/whirlpool_sixth_sense-0.18.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whirlpool_sixth_sense-0.18.2.tar", last modified: Wed Jan 11 00:25:45 2023, max compression
+gzip compressed data, was "whirlpool_sixth_sense-0.18.3.tar", last modified: Sat Apr 22 00:35:51 2023, max compression
```

## Comparing `whirlpool_sixth_sense-0.18.2.tar` & `whirlpool_sixth_sense-0.18.3.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:25:45.019229 whirlpool_sixth_sense-0.18.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-11 00:25:35.000000 whirlpool_sixth_sense-0.18.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 00:25:35.000000 whirlpool_sixth_sense-0.18.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-01-11 00:25:45.019229 whirlpool_sixth_sense-0.18.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-01-11 00:25:35.000000 whirlpool_sixth_sense-0.18.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-11 00:25:35.000000 whirlpool_sixth_sense-0.18.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-11 00:25:35.000000 whirlpool_sixth_sense-0.18.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 00:25:45.019229 whirlpool_sixth_sense-0.18.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-01-11 00:25:35.000000 whirlpool_sixth_sense-0.18.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:25:45.015228 whirlpool_sixth_sense-0.18.2/whirlpool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 00:25:35.000000 whirlpool_sixth_sense-0.18.2/whirlpool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-01-11 00:25:35.000000 whirlpool_sixth_sense-0.18.2/whirlpool/aircon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-01-11 00:25:35.000000 whirlpool_sixth_sense-0.18.2/whirlpool/appliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-01-11 00:25:35.000000 whirlpool_sixth_sense-0.18.2/whirlpool/appliancesmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-01-11 00:25:35.000000 whirlpool_sixth_sense-0.18.2/whirlpool/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-01-11 00:25:35.000000 whirlpool_sixth_sense-0.18.2/whirlpool/backendselector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-01-11 00:25:35.000000 whirlpool_sixth_sense-0.18.2/whirlpool/eventsocket.py
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-01-11 00:25:35.000000 whirlpool_sixth_sense-0.18.2/whirlpool/oven.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-01-11 00:25:35.000000 whirlpool_sixth_sense-0.18.2/whirlpool/washerdryer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:25:45.015228 whirlpool_sixth_sense-0.18.2/whirlpool_sixth_sense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-01-11 00:25:44.000000 whirlpool_sixth_sense-0.18.2/whirlpool_sixth_sense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-01-11 00:25:44.000000 whirlpool_sixth_sense-0.18.2/whirlpool_sixth_sense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 00:25:44.000000 whirlpool_sixth_sense-0.18.2/whirlpool_sixth_sense.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-11 00:25:44.000000 whirlpool_sixth_sense-0.18.2/whirlpool_sixth_sense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-11 00:25:44.000000 whirlpool_sixth_sense-0.18.2/whirlpool_sixth_sense.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:35:51.134040 whirlpool_sixth_sense-0.18.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-22 00:35:51.134040 whirlpool_sixth_sense-0.18.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:35:51.134040 whirlpool_sixth_sense-0.18.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:35:51.130040 whirlpool_sixth_sense-0.18.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/tests/test_aircon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86676 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/tests/test_oven.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:35:51.130040 whirlpool_sixth_sense-0.18.3/whirlpool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/aircon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/appliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/appliancesmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/backendselector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/eventsocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/oven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/washerdryer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:35:51.134040 whirlpool_sixth_sense-0.18.3/whirlpool_sixth_sense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-22 00:35:51.000000 whirlpool_sixth_sense-0.18.3/whirlpool_sixth_sense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-22 00:35:51.000000 whirlpool_sixth_sense-0.18.3/whirlpool_sixth_sense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:35:51.000000 whirlpool_sixth_sense-0.18.3/whirlpool_sixth_sense.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-22 00:35:51.000000 whirlpool_sixth_sense-0.18.3/whirlpool_sixth_sense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-22 00:35:51.000000 whirlpool_sixth_sense-0.18.3/whirlpool_sixth_sense.egg-info/top_level.txt
```

### Comparing `whirlpool_sixth_sense-0.18.2/LICENSE` & `whirlpool_sixth_sense-0.18.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.2/PKG-INFO` & `whirlpool_sixth_sense-0.18.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: whirlpool_sixth_sense
-Version: 0.18.2
+Version: 0.18.3
 Summary: Unofficial API for Whirlpool's 6th Sense appliances
-Home-page: https://github.com/abmantis/whirlpool-sixth-sense/
-Author: Abílio Costa
-Author-email: amfcalt@gmail.com
+Author-email: Abílio Costa <amfcalt@gmail.com>
+Project-URL: Homepage, https://github.com/abmantis/whirlpool-sixth-sense/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `whirlpool_sixth_sense-0.18.2/README.md` & `whirlpool_sixth_sense-0.18.3/README.md`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.2/whirlpool/aircon.py` & `whirlpool_sixth_sense-0.18.3/whirlpool/aircon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from enum import Enum
 from typing import Callable
+
 import aiohttp
 
 from .appliance import Appliance
 
 LOGGER = logging.getLogger(__name__)
 
 ATTR_MODE = "Cavity_OpStatusMode"
```

### Comparing `whirlpool_sixth_sense-0.18.2/whirlpool/appliancesmanager.py` & `whirlpool_sixth_sense-0.18.3/whirlpool/appliancesmanager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import aiohttp
-import logging
 import json
+import logging
 
-
-from .backendselector import BackendSelector
+import aiohttp
 
 from .auth import Auth
+from .backendselector import BackendSelector
 
 LOGGER = logging.getLogger(__name__)
 
 
 class AppliancesManager:
     def __init__(
         self,
@@ -31,15 +30,14 @@
             # "Host": "api.whrcloud.eu",
             "User-Agent": "okhttp/3.12.0",
             "Pragma": "no-cache",
             "Cache-Control": "no-cache",
         }
 
     async def fetch_appliances(self):
-
         account_id = None
         async with self._session.get(
             f"{self._backend_selector.base_url}/api/v1/getUserDetails",
             headers=self._create_headers(),
         ) as r:
             if r.status != 200:
                 LOGGER.error(f"Failed to get account id: {r.status}")
@@ -62,14 +60,16 @@
             for appliances in locations.values():
                 for appliance in appliances:
                     appliance_data = {
                         "SAID": appliance["SAID"],
                         "NAME": appliance["APPLIANCE_NAME"],
                         "DATA_MODEL": appliance["DATA_MODEL_KEY"],
                         "CATEGORY": appliance["CATEGORY_NAME"],
+                        "MODEL_NUMBER": appliance.get("MODEL_NO"),
+                        "SERIAL_NUMBER": appliance.get("SERIAL"),
                     }
                     data_model = appliance["DATA_MODEL_KEY"].lower()
                     if "airconditioner" in data_model:
                         self._aircons.append(appliance_data)
                     elif "dryer" in data_model or "washer" in data_model:
                         self._washer_dryers.append(appliance_data)
                     elif "cooking_minerva" in data_model or "cooking_vsi" in data_model:
```

### Comparing `whirlpool_sixth_sense-0.18.2/whirlpool/auth.py` & `whirlpool_sixth_sense-0.18.3/whirlpool/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import aiohttp
 import asyncio
-import async_timeout
-import logging
 import json
-from datetime import datetime, timedelta, timedelta
+import logging
+from datetime import datetime, timedelta
+
+import aiohttp
+import async_timeout
 
 from .backendselector import BackendSelector
 
 LOGGER = logging.getLogger(__name__)
 
 AUTH_JSON_FILE = ".whirlpool_auth.json"
 AUTO_REFRESH_DELTA = timedelta(minutes=15)
@@ -53,15 +54,15 @@
         self.cancel_auto_renewal()
         self._auto_renewal_task = asyncio.create_task(self._do_auto_renewal())
 
     def _save_auth_data(self):
         with open(AUTH_JSON_FILE, "w") as f:
             json.dump(self._auth_dict, f)
 
-    async def _do_auth(self, refresh_token):
+    async def _do_auth(self, refresh_token: str) -> str | None:
         auth_url = f"{self._backend_selector.base_url}/oauth/token"
         auth_header = {
             "Content-Type": "application/x-www-form-urlencoded",
             # "Brand": "Whirlpool",
             # "WP-CLIENT-REGION": "EMEA",
             # "WP-CLIENT-BRAND": "WHIRLPOOL",
             # "WP-CLIENT-COUNTRY": "EN",
@@ -97,35 +98,36 @@
                 LOGGER.debug("Auth status: " + str(r.status))
                 if r.status == 200:
                     return json.loads(await r.text())
                 elif refresh_token:
                     return await self._do_auth(refresh_token=None)
                 return None
 
-    async def do_auth(self, store=True):
+    async def do_auth(self, store: bool = False) -> bool:
         fetched_auth_data = await self._do_auth(
             self._auth_dict.get("refresh_token", None)
         )
 
         if not fetched_auth_data:
             self._auth_dict = {}
             LOGGER.error("Authentication failed")
-            return
+            return False
 
         curr_timestamp = datetime.now().timestamp()
         self._auth_dict = {
             "access_token": fetched_auth_data.get("access_token", ""),
             "refresh_token": fetched_auth_data.get("refresh_token", ""),
             "expire_date": curr_timestamp + fetched_auth_data.get("expires_in", ""),
             "accountId": fetched_auth_data.get("accountId", ""),
             "SAID": fetched_auth_data.get("SAID", ""),
         }
         if store:
             self._save_auth_data()
         self._schedule_auto_renewal()
+        return True
 
     async def load_auth_file(self):
         try:
             with open(AUTH_JSON_FILE, "r") as f:
                 LOGGER.info("Loading auth from file")
                 self._auth_dict = json.load(f)
         except FileNotFoundError:
```

### Comparing `whirlpool_sixth_sense-0.18.2/whirlpool/backendselector.py` & `whirlpool_sixth_sense-0.18.3/whirlpool/backendselector.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.2/whirlpool/eventsocket.py` & `whirlpool_sixth_sense-0.18.3/whirlpool/eventsocket.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-import aiohttp
-from socket import gaierror
 import asyncio
 import logging
 import re
 import uuid
-
+from socket import gaierror
 from typing import Callable
 
+import aiohttp
+
 from .auth import Auth
 
 LOGGER = logging.getLogger(__name__)
 
 MSG_TERMINATION = "\n\n\0"
 
-RECV_MSG_MATCHER = re.compile("{(.*)}\\x00")
+DATA_MSG_MATCHER = re.compile("{(.*)}\\x00")
+TOKEN_INVALID_MSG_MATCHER = re.compile(".*Token Invalid.*")
 
 WS_STATUS_GOING_AWAY = 1001
 WS_STATUS_UNAUTHORIZED = 3000
 
 RECONNECT_COUNT = 3
 RECONNECT_SHORT_DELAY = 30
 RECONNECT_LONG_DELAY = 60 * 4
 GOING_AWAY_DELAY = (60 * 5) - RECONNECT_SHORT_DELAY
 
 
 class EventSocket:
+    """Event socket listener class"""
+
     def __init__(
         self,
         url,
         auth: Auth,
         said,
         msg_listener: Callable[[str], None],
         con_up_listener: Callable,
@@ -58,109 +61,131 @@
 
     async def _recv_msg(self, websocket: aiohttp.ClientWebSocketResponse):
         msg = await websocket.receive()
         LOGGER.debug(f"< {msg}")
         return msg
 
     async def _run(self):
-        if not self._running:
-            return
-        timeout = aiohttp.ClientTimeout(total=None, connect=60, sock_connect=60)
+        while self._running:
+            timeout = aiohttp.ClientTimeout(total=None, connect=60, sock_connect=60)
 
-        try:
-            LOGGER.debug(f"Connecting to {self._url}")
-            async with self._session.ws_connect(
-                self._url,
-                timeout=timeout,
-                autoclose=True,
-                autoping=True,
-                heartbeat=45,
-            ) as ws:
-                self._websocket = ws
-                await self._send_msg(ws, self._create_connect_msg())
-                await self._recv_msg(ws)
-                await self._send_msg(ws, self._create_subscribe_msg())
-                await self._con_up_listener()
-
-                self._reconnect_tries = RECONNECT_COUNT
-
-                while not ws.closed:
-                    msg = await self._recv_msg(ws)
-                    if not msg:
-                        continue
-                    if msg.type == aiohttp.WSMsgType.ERROR:
-                        LOGGER.error("Socket message error")
-                        break
-                    if msg.type in [
-                        aiohttp.WSMsgType.CLOSE,
-                        aiohttp.WSMsgType.CLOSING,
-                        aiohttp.WSMsgType.CLOSED,
-                    ]:
-                        LOGGER.warn(
-                            f"Stopping receiving. Message type: {str(msg.type)}"
-                        )
-
-                        if (
-                            not self._auth.is_access_token_valid()
-                            or msg.data == WS_STATUS_UNAUTHORIZED
-                        ):
-                            LOGGER.debug("auth key expired, doing reauth now")
-                            await self._auth.do_auth()
-
-                        elif msg.data == WS_STATUS_GOING_AWAY:
-                            LOGGER.warn(
-                                f"Received Going Away message: Waiting for {GOING_AWAY_DELAY} seconds"
+            try:
+                LOGGER.debug(f"Connecting to {self._url}")
+                async with self._session.ws_connect(
+                    self._url,
+                    timeout=timeout,
+                    autoclose=True,
+                    autoping=True,
+                    heartbeat=45,
+                ) as ws:
+                    self._websocket = ws
+                    self._reconnect_tries = RECONNECT_COUNT
+                    connected_msg_done = False
+                    subscribe_msg_done = False
+
+                    while not ws.closed:
+                        if not connected_msg_done:
+                            await self._send_msg(ws, self._create_connect_msg())
+                        elif not subscribe_msg_done:
+                            await self._send_msg(ws, self._create_subscribe_msg())
+
+                        msg = await self._recv_msg(ws)
+                        if not msg:
+                            continue
+                        if msg.type == aiohttp.WSMsgType.ERROR:
+                            LOGGER.error("Socket message error")
+                            break
+                        if msg.type in [
+                            aiohttp.WSMsgType.CLOSE,
+                            aiohttp.WSMsgType.CLOSING,
+                            aiohttp.WSMsgType.CLOSED,
+                        ]:
+                            LOGGER.warning(
+                                f"Stopping receiving. Message type: {str(msg.type)}"
                             )
-                            # Give server some time to come back up.
-                            await asyncio.sleep(GOING_AWAY_DELAY)
 
-                        break
+                            if (
+                                not self._auth.is_access_token_valid()
+                                or msg.data == WS_STATUS_UNAUTHORIZED
+                            ):
+                                LOGGER.debug("auth key expired, doing reauth now")
+                                while not await self._auth.do_auth():
+                                    await asyncio.sleep(RECONNECT_LONG_DELAY)
+
+                            elif msg.data == WS_STATUS_GOING_AWAY:
+                                LOGGER.warning(
+                                    f"Received Going Away message: Waiting for {GOING_AWAY_DELAY} seconds"
+                                )
+                                # Give server some time to come back up.
+                                await asyncio.sleep(GOING_AWAY_DELAY)
 
-                    if msg.type != aiohttp.WSMsgType.TEXT:
-                        LOGGER.error(f"Socket message type is invalid: {str(msg.type)}")
-                        continue
-
-                    match = RECV_MSG_MATCHER.findall(msg.data)
-                    if not match:
-                        continue
-                    self._msg_listener("{" + match[0] + "}")
-        except (
-            aiohttp.ClientError,
-            asyncio.TimeoutError,
-            gaierror,
-        ) as e:
-            LOGGER.error(f"Websocket could not connect: {e}")
+                            break
 
-        self._websocket = None
+                        invalid_token_match = TOKEN_INVALID_MSG_MATCHER.findall(
+                            msg.data
+                        )
+                        if invalid_token_match:
+                            LOGGER.debug("received invalid token msg, doing reauth now")
+                            while not await self._auth.do_auth():
+                                await asyncio.sleep(RECONNECT_LONG_DELAY)
+                            break
+
+                        if not connected_msg_done:
+                            connected_msg_done = True
+                            continue
+
+                        if not subscribe_msg_done:
+                            subscribe_msg_done = True
+                            await self._con_up_listener()
+                            continue
+
+                        if msg.type != aiohttp.WSMsgType.TEXT:
+                            LOGGER.error(
+                                f"Socket message type is invalid: {str(msg.type)}"
+                            )
+                            continue
 
-        if self._running:
+                        match = DATA_MSG_MATCHER.findall(msg.data)
+                        if not match:
+                            continue
+                        self._msg_listener("{" + match[0] + "}")
+            except (
+                aiohttp.ClientError,
+                asyncio.TimeoutError,
+                gaierror,
+            ) as ex:
+                LOGGER.error(f"Websocket could not connect: {ex}")
+
+            self._websocket = None
+
+            if self._running:
+                self._reconnect_tries -= 1
+                if self._reconnect_tries < 0:
+                    self._reconnect_tries = 0
+                    LOGGER.info(
+                        f"Waiting to reconnect long delay {RECONNECT_LONG_DELAY} seconds"
+                    )
+
+                    # Give server some time to come back up.
+                    await asyncio.sleep(RECONNECT_LONG_DELAY)
 
-            self._reconnect_tries -= 1
-            if self._reconnect_tries < 0:
-                self._reconnect_tries = 0
                 LOGGER.info(
-                    f"Waiting to reconnect long delay {RECONNECT_LONG_DELAY} seconds"
+                    f"Waiting to reconnect short delay {RECONNECT_SHORT_DELAY} seconds"
                 )
+                await asyncio.sleep(RECONNECT_SHORT_DELAY)
 
-                # Give server some time to come back up.
-                await asyncio.sleep(RECONNECT_LONG_DELAY)
-
-            LOGGER.info(
-                f"Waiting to reconnect short delay {RECONNECT_SHORT_DELAY} seconds"
-            )
-            await asyncio.sleep(RECONNECT_SHORT_DELAY)
-
-            LOGGER.info("Reconnecting...")
-            self._run_future = asyncio.get_event_loop().create_task(self._run())
+                LOGGER.info("Reconnecting...")
 
     def start(self):
+        """Start the event socket listener"""
         self._running = True
         self._run_future = asyncio.get_event_loop().create_task(self._run())
 
     async def stop(self):
+        """Stop the event socket listener"""
         self._running = False
         if not self._websocket:
             return
         await self._websocket.close()
         self._websocket = None
-
-        await self._run_future
+        if not self._run_future.done():
+            await self._run_future
```

### Comparing `whirlpool_sixth_sense-0.18.2/whirlpool/oven.py` & `whirlpool_sixth_sense-0.18.3/whirlpool/oven.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 from enum import Enum
+
 import aiohttp
 
 from .appliance import Appliance
 
 LOGGER = logging.getLogger(__name__)
 
 ATTR_DISPLAY_BRIGHTNESS = "Sys_DisplaySetBrightnessPercent"
@@ -56,14 +57,15 @@
 class Cavity(Enum):
     Upper = 0
     Lower = 1
 
 
 CAVITY_PREFIX_MAP = {Cavity.Upper: "OvenUpperCavity", Cavity.Lower: "OvenLowerCavity"}
 
+
 # todo: figure out/plug in the other enums
 class CookMode(Enum):
     Standby = 0
     Bake = 2
     ConvectBake = 6
     Broil = 8
     ConvectBroil = 9
@@ -79,14 +81,15 @@
     CookMode.Broil: ATTRVAL_COOK_MODE_BROIL,
     CookMode.ConvectBroil: ATTRVAL_COOK_MODE_CONVECT_BROIL,
     CookMode.ConvectRoast: ATTRVAL_COOK_MODE_CONVECT_ROAST,
     CookMode.KeepWarm: ATTRVAL_COOK_MODE_KEEP_WARM,
     CookMode.AirFry: ATTRVAL_COOK_MODE_AIR_FRY,
 }
 
+
 # todo: figure out/plug in the other enums
 class CookOperation(Enum):
     Cancel = 1
     Start = 2
     Modify = 4
     Pause = 5
 
@@ -94,14 +97,15 @@
 COOK_OPERATION_MAP = {
     CookOperation.Cancel: ATTRVAL_CAVITY_OPERATION_CANCEL,
     CookOperation.Start: ATTRVAL_CAVITY_OPERATION_START,
     CookOperation.Modify: ATTRVAL_CAVITY_OPERATION_MODIFY,
     CookOperation.Pause: ATTRVAL_CAVITY_OPERATION_PAUSE,
 }
 
+
 # todo: figure out/plug in the other enums
 class CavityState(Enum):
     Standby = 0
     Preheating = 1
     Cooking = 2
     NotPresent = 4
 
@@ -109,14 +113,15 @@
 CAVITY_STATE_MAP = {
     CavityState.Standby: ATTRVAL_CAVITY_STATE_STANDBY,
     CavityState.Preheating: ATTRVAL_CAVITY_STATE_PREHEATING,
     CavityState.Cooking: ATTRVAL_CAVITY_STATE_COOKING,
     CavityState.NotPresent: ATTRVAL_CAVITY_STATE_NOT_PRESENT,
 }
 
+
 # todo: figure out/plug in what state = 2 is
 class KitchenTimerState(Enum):
     Standby = 0
     Running = 1
     Completed = 3
```

### Comparing `whirlpool_sixth_sense-0.18.2/whirlpool/washerdryer.py` & `whirlpool_sixth_sense-0.18.3/whirlpool/washerdryer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 from enum import Enum
+
 import aiohttp
 
 from .appliance import Appliance
 
 LOGGER = logging.getLogger(__name__)
 
 ATTR_CYCLE_STATUS_SENSING = "WashCavity_CycleStatusSensing"
```

### Comparing `whirlpool_sixth_sense-0.18.2/whirlpool_sixth_sense.egg-info/PKG-INFO` & `whirlpool_sixth_sense-0.18.3/whirlpool_sixth_sense.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: whirlpool-sixth-sense
-Version: 0.18.2
+Version: 0.18.3
 Summary: Unofficial API for Whirlpool's 6th Sense appliances
-Home-page: https://github.com/abmantis/whirlpool-sixth-sense/
-Author: Abílio Costa
-Author-email: amfcalt@gmail.com
+Author-email: Abílio Costa <amfcalt@gmail.com>
+Project-URL: Homepage, https://github.com/abmantis/whirlpool-sixth-sense/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

