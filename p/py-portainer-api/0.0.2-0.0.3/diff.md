# Comparing `tmp/py_portainer_api-0.0.2-py3-none-any.whl.zip` & `tmp/py_portainer_api-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6880 bytes, number of entries: 11
--rw-r--r--  2.0 unx       87 b- defN 23-Apr-18 20:30 portainer/__init__.py
--rw-r--r--  2.0 unx      757 b- defN 23-Apr-18 20:30 portainer/const.py
--rw-r--r--  2.0 unx     4688 b- defN 23-Apr-18 20:30 portainer/docker_container.py
--rw-r--r--  2.0 unx     2225 b- defN 23-Apr-18 20:30 portainer/endpoint.py
--rw-r--r--  2.0 unx      417 b- defN 23-Apr-18 20:30 portainer/exceptions.py
--rw-r--r--  2.0 unx     4353 b- defN 23-Apr-18 20:30 portainer/portainer.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Apr-18 20:31 py_portainer_api-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1400 b- defN 23-Apr-18 20:31 py_portainer_api-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 20:31 py_portainer_api-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-18 20:31 py_portainer_api-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      903 b- defN 23-Apr-18 20:31 py_portainer_api-0.0.2.dist-info/RECORD
-11 files, 15999 bytes uncompressed, 5346 bytes compressed:  66.6%
+Zip file size: 7848 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       87 b- defN 23-Apr-22 09:17 portainer/__init__.py
+-rw-r--r--  2.0 unx      757 b- defN 23-Apr-22 09:17 portainer/const.py
+-rw-r--r--  2.0 unx     4513 b- defN 23-Apr-22 09:17 portainer/docker_container.py
+-rw-r--r--  2.0 unx     2191 b- defN 23-Apr-22 09:17 portainer/endpoint.py
+-rw-r--r--  2.0 unx     1266 b- defN 23-Apr-22 09:17 portainer/exceptions.py
+-rw-r--r--  2.0 unx     7468 b- defN 23-Apr-22 09:17 portainer/portainer.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-22 09:18 py_portainer_api-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1369 b- defN 23-Apr-22 09:18 py_portainer_api-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 09:18 py_portainer_api-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-22 09:18 py_portainer_api-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      904 b- defN 23-Apr-22 09:18 py_portainer_api-0.0.3.dist-info/RECORD
+11 files, 19724 bytes uncompressed, 6314 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: portainer/exceptions.py
 Comment: 
 
 Filename: portainer/portainer.py
 Comment: 
 
-Filename: py_portainer_api-0.0.2.dist-info/LICENSE
+Filename: py_portainer_api-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: py_portainer_api-0.0.2.dist-info/METADATA
+Filename: py_portainer_api-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: py_portainer_api-0.0.2.dist-info/WHEEL
+Filename: py_portainer_api-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: py_portainer_api-0.0.2.dist-info/top_level.txt
+Filename: py_portainer_api-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: py_portainer_api-0.0.2.dist-info/RECORD
+Filename: py_portainer_api-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## portainer/docker_container.py

```diff
@@ -1,11 +1,10 @@
 """Class to interact with Portainer docker containers."""
 from __future__ import annotations
 
-import json
 from typing import TYPE_CHECKING, Any
 
 from .const import (
     API_CONTAINER_RESTART,
     API_CONTAINER_START,
     API_CONTAINER_STOP,
     API_IMAGE_STATUS,
@@ -23,15 +22,15 @@
 
     def __init__(
         self, portainer: Portainer, endpoint_id: str, docker_container: dict
     ) -> None:
         """Constructor method."""
         self._portainer = portainer
         self._endpoint_id = endpoint_id
-        self.image_status = ""
+        self.image_status: dict[Any, Any] = {}
         self.container_id = ""
         self.status = ""
         self.stats: dict[Any, Any] = {}
         self.after_refresh(docker_container)
 
     def after_refresh(self, docker_container: dict) -> None:
         """Sets all variables."""
@@ -44,86 +43,90 @@
         self.created = docker_container["Created"]
 
     async def get_image_status(self) -> dict:
         """Request the status of the container."""
         api = API_IMAGE_STATUS.format(
             environment_id=self._endpoint_id, container_id=self.container_id
         )
-        response = await self._portainer.run_command("GET", api, None)
+        response = await self._portainer.get(api, None)
+
+        if response["status_code"] == 200:
+            self.image_status = response["body"]["Status"]
+            return self.image_status
 
-        if response.status_code == 200:
-            image_status = {}
-            image_status = json.loads(response.text)
-            self.image_status = image_status["Status"]
-            return image_status
-        data = json.loads(response.text)
         raise PortainerException(
-            api, response.status_code, data["message"], data["details"]
+            api,
+            response["status_code"],
+            response["body"]["message"],
+            response["body"]["details"],
         )
 
     async def get_stats(self) -> dict:
         """Request the stats of the container."""
         api = API_STATS.format(
             environment_id=self._endpoint_id, container_id=self.container_id
         )
         api += "?stream=false"
-        response = await self._portainer.run_command("GET", api, None)
+        response = await self._portainer.get(api, None)
 
-        if response.status_code == 200:
-            stats = {}
-            stats = json.loads(response.text)
-            self.stats = stats
-            return stats
+        if response["status_code"] == 200:
+            self.stats = response["body"]
+            return self.stats
 
-        data = json.loads(response.text)
         raise PortainerException(
-            api, response.status_code, data["message"], data["details"]
+            api,
+            response["status_code"],
+            response["body"]["message"],
+            response["body"]["details"],
         )
 
     async def recreate(self, pull_image: bool = True) -> dict:
         """Recreate the container."""
         api = API_RECREATE.format(
             environment_id=self._endpoint_id, container_id=self.container_id
         )
         param = {"PullImage": pull_image}
-        response = await self._portainer.run_command("POST", api, param)
+        response = await self._portainer.post(api, param)
 
-        if response.status_code == 200:
-            container = {}
-            container = json.loads(response.text)
-            self.container_id = container["Id"]
-            self.status = container["State"]["Status"]
-            return container
-        data = json.loads(response.text)
+        if response["status_code"] == 200:
+            self.container_id = response["body"]["Id"]
+            self.status = response["body"]["State"]["Status"]
+            return dict(response["body"])
         raise PortainerException(
-            api, response.status_code, data["message"], data["details"]
+            api,
+            response["status_code"],
+            response["body"]["message"],
+            response["body"]["details"],
         )
 
     async def stop(self) -> None:
         """Stop the container."""
         api = API_CONTAINER_STOP.format(
             environment_id=self._endpoint_id, container_id=self.container_id
         )
-        response = await self._portainer.run_command("POST", api, None)
-        if response.status_code != 204:
-            data = json.loads(response.text)
-            raise PortainerException(api, response.status_code, data["message"], "")
+        response = await self._portainer.post(api, None)
+        if response["status_code"] != 204:
+            raise PortainerException(
+                api, response["status_code"], response["body"]["message"], ""
+            )
 
     async def start(self) -> None:
         """Start the container."""
         api = API_CONTAINER_START.format(
             environment_id=self._endpoint_id, container_id=self.container_id
         )
-        response = await self._portainer.run_command("POST", api, None)
-        if response.status_code != 204:
-            data = json.loads(response.text)
-            raise PortainerException(api, response.status_code, data["message"], "")
+        response = await self._portainer.post(api, None)
+        if response["status_code"] != 204:
+            raise PortainerException(
+                api, response["status_code"], response["body"]["message"], ""
+            )
 
     async def restart(self) -> None:
         """Restart the container."""
         api = API_CONTAINER_RESTART.format(
             environment_id=self._endpoint_id, container_id=self.container_id
         )
-        response = await self._portainer.run_command("POST", api, None)
-        if response.status_code != 204:
-            data = json.loads(response.text)
-            raise PortainerException(api, response.status_code, data["message"], "")
+        response = await self._portainer.post(api, None)
+        if response["status_code"] != 204:
+            raise PortainerException(
+                api, response["status_code"], response["body"]["message"], ""
+            )
```

## portainer/endpoint.py

```diff
@@ -1,11 +1,10 @@
 """Class to interact with Portainer endpoints."""
 from __future__ import annotations
 
-import json
 from typing import TYPE_CHECKING, Dict
 
 from .const import API_ENDPOINT
 from .docker_container import PortainerDockerContainer
 from .exceptions import PortainerException
 
 if TYPE_CHECKING:
@@ -20,22 +19,23 @@
         self._portainer = portainer
         self.docker_container: Dict[str, PortainerDockerContainer] = {}
         self.after_refresh(endpoint)
 
     async def refresh(self) -> None:
         """Refresh properties."""
         api = API_ENDPOINT.format(environment_id=self._id)
-        response = await self._portainer.run_command("GET", api, None)
-        if response.status_code == 200:
-            endpoint = json.loads(response.text)
-            self.after_refresh(endpoint)
+        response = await self._portainer.get(api, None)
+        if response["status_code"] == 200:
+            self.after_refresh(response["body"])
         else:
-            data = json.loads(response.text)
             raise PortainerException(
-                api, response.status_code, data["message"], data["details"]
+                api,
+                response["status_code"],
+                response["body"]["message"],
+                response["body"]["details"],
             )
 
     def after_refresh(self, endpoint: dict) -> None:
         """Set variables from a refresh."""
         self._id = endpoint["Id"]
         self._name = endpoint["Name"]
         self._type = endpoint["Type"]
```

## portainer/exceptions.py

```diff
@@ -1,15 +1,44 @@
 """Library exceptions."""
 
 
 class PortainerException(Exception):
     """Generic Portainer exception."""
 
-    def __init__(self, api: str | None, code: int, message: str, details: str) -> None:
+    def __init__(
+        self,
+        api: str | None,
+        code: int,
+        message: str | None = None,
+        details: str | None = None,
+    ) -> None:
         """Constructor method."""
         error_message = {
             "api": api,
             "code": code,
             "message": message,
             "details": details,
         }
         super().__init__(error_message)
+
+
+class PortainerNotLoggedInException(PortainerException):
+    """Not logged in exception."""
+
+    def __init__(self) -> None:
+        """Constructor method."""
+        super().__init__(None, -1, "Not logged in. You have to do login() first.", "")
+
+
+class PortainerRequestException(PortainerException):
+    """Request exception."""
+
+    def __init__(self, exception: Exception) -> None:
+        """Constructor method."""
+        ex_class = exception.__class__.__name__
+        if not exception.args:
+            super().__init__(None, -1, None, ex_class)
+            return
+        ex_reason = exception.args[0]
+        if hasattr(exception.args[0], "reason"):
+            ex_reason = exception.args[0].reason
+        super().__init__(None, -1, f"{ex_class} = {ex_reason}")
```

## portainer/portainer.py

```diff
@@ -1,105 +1,192 @@
 """Class to interact with Portainer."""
 from __future__ import annotations
 
-import json
+import asyncio
 import logging
+from json import JSONDecodeError
 from typing import List, Union
+from urllib.parse import quote, urlencode
 
-import requests
-from requests import Response
+import aiohttp
+import async_timeout
+from yarl import URL
 
 from .const import API_AUTH, API_ENDPOINTS
 from .endpoint import PortainerEndpoint
-from .exceptions import PortainerException
+from .exceptions import (
+    PortainerException,
+    PortainerNotLoggedInException,
+    PortainerRequestException,
+)
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Portainer:
     """Class containing the main Portainer functions."""
 
     def __init__(
         self,
+        session: aiohttp.ClientSession,
         portainer_ip: str,
         portainer_port: int,
         username: str,
         password: str,
+        timeout: int = 600,
         use_https: bool = False,
         debugmode: bool = False,
     ):
         """Constructor method."""
         self._username = username
         self._password = password
         self._debugmode = debugmode
 
+        self._timeout = timeout
+
+        # Session
+        self._session = session
+
         # Login
         self._auth_token: str | None = None
 
         # Build variables
         if use_https:
-            self._base_url = f"https://{portainer_ip}:{portainer_port}/api/"
+            self._base_url = f"https://{portainer_ip}:{portainer_port}/api"
         else:
-            self._base_url = f"http://{portainer_ip}:{portainer_port}/api/"
+            self._base_url = f"http://{portainer_ip}:{portainer_port}/api"
 
     def _debuglog(self, message: str) -> None:
         """Outputs message if debug mode is enabled."""
         _LOGGER.debug(message)
         if self._debugmode:
             print("DEBUG: " + message)
 
-    async def post(self, api: str, params: dict | None) -> Response:
+    async def post(self, api: str, params: dict | None = None) -> dict:
         """Handles API POST request."""
-        api_url = self._base_url + api
-        headers = {"Authorization": f"Bearer {self._auth_token}"}
-        return requests.post(api_url, headers=headers, json=params, timeout=600)
+        return await self._request("POST", api, params)
 
-    async def get(self, api: str, params: dict | None) -> Response:
+    async def get(self, api: str, params: dict | None = None) -> dict:
         """Handles API GET request."""
-        api_url = self._base_url + api
-        headers = {"Authorization": f"Bearer {self._auth_token}"}
-        return requests.get(api_url, headers=headers, json=params, timeout=600)
-
-    async def run_command(
-        self, method: str, api: str, params: dict | None, auto_login: bool = True
-    ) -> Response:
-        """Run command."""
-        self._debuglog(
-            "method: " + method + "api: " + api + "params: " + json.dumps(params)
-        )
-        if method == "POST":
-            response = await self.post(api, params)
-        elif method == "GET":
-            response = await self.get(api, params)
-        if response.status_code == 401 and auto_login:  # not authorized, retry login
+        return await self._request("GET", api, params)
+
+    async def _request(
+        self,
+        request_method: str,
+        api: str,
+        params: dict | None = None,
+        retry_once: bool = True,
+    ) -> dict:
+        """Handles API request."""
+        url, params, headers = await self._prepare_request(api, params)
+
+        # Request data
+        self._debuglog("API: " + api)
+        self._debuglog("Request Method: " + request_method)
+        response = await self._execute_request(request_method, url, params, headers)
+        self._debuglog("Successful returned data")
+        self._debuglog("RESPONSE: " + str(response))
+
+        # Handle data errors
+        if api != API_AUTH and response["status_code"] == 401 and retry_once:
+            # Session ID is expired
             if self.login():
-                response = await self.run_command(method, api, params, False)
-        self._debuglog(f"Response status code: {response.status_code}")
+                response = await self._request(request_method, api, params, False)
         return response
 
+    async def _prepare_request(
+        self,
+        api: str,
+        params: dict | None = None,
+    ) -> tuple[str, dict, dict | None]:
+        """Prepare the url and parameters for a request."""
+        # Check if logged
+        if not self._auth_token and api not in [API_AUTH]:
+            raise PortainerNotLoggedInException
+        # Build request params
+        if not params:
+            params = {}
+        headers = None
+        if self._auth_token:
+            headers = {"Authorization": f"Bearer {self._auth_token}"}
+        url = f"{self._base_url}/{api}"
+        return (url, params, headers)
+
+    async def _execute_request(
+        self, method: str, url: str, params: dict | None, headers: dict | None = None
+    ) -> dict:
+        """Function to execute and handle a request."""
+        if params:
+            # special handling for spaces in parameters
+            # because yarl.URL does encode a space as + instead of %20
+            # safe extracted from yarl.URL._QUERY_PART_QUOTER
+            safe = "?/:@-._~!$'()*,"
+            query = urlencode(params, safe=safe, quote_via=quote)
+            url_encoded = URL(str(URL(url)) + "?" + query, encoded=True)
+        else:
+            url_encoded = URL(url)
+
+        try:
+            if method == "GET":
+                async with async_timeout.timeout(self._timeout):
+                    response = await self._session.get(url_encoded, headers=headers)
+            elif method == "POST":
+                self._debuglog("POST data: " + str(params))
+                async with async_timeout.timeout(self._timeout):
+                    response = await self._session.post(
+                        url, json=params, headers=headers
+                    )
+
+            # mask sesitiv parameters
+            response_url = response.url
+            # for param in SENSITIV_PARAMS:
+            #    if params is not None and params.get(param):
+            #        response_url = response_url.update_query({param: "*********"})
+            self._debuglog("Request url: " + str(response_url))
+            self._debuglog("Response status_code: " + str(response.status))
+            self._debuglog("Response headers: " + str(dict(response.headers)))
+
+            content_type = response.headers.get("Content-Type", "").split(";")[0]
+            ret: dict[str, str | int] = {}
+            ret["status_code"] = response.status
+            if content_type in [
+                "application/json",
+                "text/json",
+            ]:
+                ret["body"] = await response.json(content_type=content_type)
+            else:
+                ret["body"] = await response.text()
+            return ret
+        except (asyncio.TimeoutError, JSONDecodeError) as exp:
+            raise PortainerRequestException(exp) from exp
+
     async def login(self) -> bool:
         """Create a logged session."""
         # First reset the session
         self._debuglog("Creating new session")
 
         params = {
             "username": self._username,
             "password": self._password,
         }
 
         # Request login
         response = await self.post(API_AUTH, params)
-        self._debuglog(f"Response status code: {response.status_code}")
-        if response.status_code == 200:
-            self._auth_token = response.json()["jwt"]
+        if response["status_code"] == 200:
+            self._auth_token = response["body"]["jwt"]
             return True
-        data = json.loads(response.text)
-        raise PortainerException(
-            API_AUTH, response.status_code, data["message"], data["details"]
-        )
+
+        if isinstance(response["body"], dict):
+            raise PortainerException(
+                API_AUTH,
+                response["status_code"],
+                response["body"]["message"],
+                response["body"]["details"],
+            )
+        raise PortainerException(API_AUTH, response["status_code"], response["body"])
 
     async def get_endpoints(
         self,
         start: int | None = None,
         limit: int | None = None,
         group_ids: List[int] | None = None,
         endpoint_ids: List[int] | None = None,
@@ -111,18 +198,20 @@
         if limit is not None:
             params["limit"] = limit
         if group_ids is not None:
             params["groupIds"] = group_ids
         if endpoint_ids is not None:
             params["endpointIds"] = endpoint_ids
 
-        response = await self.run_command("GET", API_ENDPOINTS, params)
-        if response.status_code == 200:
+        response = await self.get(API_ENDPOINTS, params)
+        if response["status_code"] == 200:
             ret = []
-            endpoints = json.loads(response.text)
+            endpoints = response["body"]
             for endpoint in endpoints:
                 ret.append(PortainerEndpoint(self, endpoint))
             return ret
-        data = json.loads(response.text)
         raise PortainerException(
-            API_ENDPOINTS, response.status_code, data["message"], data["details"]
+            API_ENDPOINTS,
+            response["status_code"],
+            response["body"]["message"],
+            response["body"]["details"],
         )
```

## Comparing `py_portainer_api-0.0.2.dist-info/LICENSE` & `py_portainer_api-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `py_portainer_api-0.0.2.dist-info/METADATA` & `py_portainer_api-0.0.3.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: py-portainer-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python API for communication with Portainer
 Author: Lode Smets (lodesmets)
 License: MIT
 Project-URL: Repository, https://github.com/lodesmets/py-portainer-api
 Keywords: portainer
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: types-requests
+Requires-Dist: aiohttp
 
 # py-portainer-api
 
 Python library to interface with portainer
 
 # WARNING this is still very alpha, and a lot will change
```

## Comparing `py_portainer_api-0.0.2.dist-info/RECORD` & `py_portainer_api-0.0.3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 portainer/__init__.py,sha256=Bi7XWJNRlYeWxbBumsip9bTz1eVsS1g-ZuRNxXDcor8,87
 portainer/const.py,sha256=YK-HbJKoIvuAKhV4bXYmYOtNgk5bVbKv9Wn5zRZPmyc,757
-portainer/docker_container.py,sha256=LTOUEafURcvITzZoDsVx_L8tNYd3bnq6k8aXKqHcGQg,4688
-portainer/endpoint.py,sha256=dciu300jrYwzAle09HAHOLQJDPPpT2o6vORtNfHSEUU,2225
-portainer/exceptions.py,sha256=kYSqegizlBqSlGNbimjOeLs2odVMBmGK3DlMJOX1c9w,417
-portainer/portainer.py,sha256=kE8LL3zt2gBFBxuG8Q6cbUEGvgMSvwUhtMN5FI8DLAc,4353
-py_portainer_api-0.0.2.dist-info/LICENSE,sha256=BkBshnVhZIDwvlivC6TtcJemCEx-yRDjQyc8s2Zk7To,1067
-py_portainer_api-0.0.2.dist-info/METADATA,sha256=AS8q6bLQp-b4Z5X-zY8FNiwnlqXwc__p-82w9T0NGgY,1400
-py_portainer_api-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-py_portainer_api-0.0.2.dist-info/top_level.txt,sha256=BnNcKriqq2U_E5qE2lqPAdN21NPc-J5kfUOFeb2jAj8,10
-py_portainer_api-0.0.2.dist-info/RECORD,,
+portainer/docker_container.py,sha256=ZlFTuiqJai_mIvjL1Rl0EqUrAOtvlwAjr89793PJptk,4513
+portainer/endpoint.py,sha256=O2vds7ZEo3-Q83Rok0gYi1iuvfwMh7-r3vfAg_sFwUA,2191
+portainer/exceptions.py,sha256=UjkqRsy661CJpZwOAaJXgwBwMmEpCwdbqkRYBFuJ2FE,1266
+portainer/portainer.py,sha256=bswtnPdx7_qnnA_aBldnHyLbWBprV4IW8JwRbk3wHgc,7468
+py_portainer_api-0.0.3.dist-info/LICENSE,sha256=BkBshnVhZIDwvlivC6TtcJemCEx-yRDjQyc8s2Zk7To,1067
+py_portainer_api-0.0.3.dist-info/METADATA,sha256=24PkcWih4OWH6Myq8Z7GckNYC-1emJbHqp4lXFoMNdw,1369
+py_portainer_api-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+py_portainer_api-0.0.3.dist-info/top_level.txt,sha256=BnNcKriqq2U_E5qE2lqPAdN21NPc-J5kfUOFeb2jAj8,10
+py_portainer_api-0.0.3.dist-info/RECORD,,
```

