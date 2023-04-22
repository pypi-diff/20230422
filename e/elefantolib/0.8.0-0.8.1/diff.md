# Comparing `tmp/elefantolib-0.8.0.tar.gz` & `tmp/elefantolib-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefantolib-0.8.0.tar", max compression
+gzip compressed data, was "elefantolib-0.8.1.tar", max compression
```

## Comparing `elefantolib-0.8.0.tar` & `elefantolib-0.8.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1073 2023-04-17 04:59:26.914971 elefantolib-0.8.0/LICENSE
--rw-r--r--   0        0        0        0 2023-04-17 04:59:26.914971 elefantolib-0.8.0/README.rst
--rw-r--r--   0        0        0       22 2023-04-21 06:07:50.189568 elefantolib-0.8.0/elefantolib/__init__.py
--rw-r--r--   0        0        0       36 2023-04-17 04:59:26.914971 elefantolib-0.8.0/elefantolib/constants.py
--rw-r--r--   0        0        0     1573 2023-04-21 05:53:22.414891 elefantolib-0.8.0/elefantolib/context/__init__.py
--rw-r--r--   0        0        0      662 2023-04-21 05:53:22.418891 elefantolib-0.8.0/elefantolib/context/context_service.py
--rw-r--r--   0        0        0      460 2023-04-21 05:53:22.418891 elefantolib-0.8.0/elefantolib/exceptions.py
--rw-r--r--   0        0        0      577 2023-04-17 04:59:26.914971 elefantolib-0.8.0/elefantolib/http_client/__init__.py
--rw-r--r--   0        0        0     2367 2023-04-17 04:59:26.914971 elefantolib-0.8.0/elefantolib/http_client/httpx_client.py
--rw-r--r--   0        0        0      373 2023-04-17 04:59:26.914971 elefantolib-0.8.0/elefantolib/logger_config.py
--rw-r--r--   0        0        0      908 2023-04-21 05:53:22.418891 elefantolib-0.8.0/elefantolib/middleware.py
--rw-r--r--   0        0        0      518 2023-04-17 04:59:26.914971 elefantolib-0.8.0/elefantolib/provider/__init__.py
--rw-r--r--   0        0        0      392 2023-04-20 12:43:37.565481 elefantolib-0.8.0/elefantolib/provider/django_provider/__init__.py
--rw-r--r--   0        0        0      386 2023-04-20 12:43:37.565481 elefantolib-0.8.0/elefantolib/provider/fastapi_provider/__init__.py
--rw-r--r--   0        0        0      404 2023-04-21 05:53:22.418891 elefantolib-0.8.0/elefantolib/websocket_client/__init__.py
--rw-r--r--   0        0        0      380 2023-04-21 05:53:22.418891 elefantolib-0.8.0/elefantolib/websocket_client/websocket_client.py
--rw-r--r--   0        0        0     1258 2023-04-21 06:07:11.022261 elefantolib-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 elefantolib-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-22 10:03:44.969858 elefantolib-0.8.1/LICENSE
+-rw-r--r--   0        0        0      154 2023-04-22 10:03:44.969858 elefantolib-0.8.1/README.rst
+-rw-r--r--   0        0        0       22 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/__init__.py
+-rw-r--r--   0        0        0       36 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/constants.py
+-rw-r--r--   0        0        0     1572 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/context/__init__.py
+-rw-r--r--   0        0        0      663 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/context/context_service.py
+-rw-r--r--   0        0        0      460 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/exceptions.py
+-rw-r--r--   0        0        0      577 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/http_client/__init__.py
+-rw-r--r--   0        0        0     2367 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/http_client/httpx_client.py
+-rw-r--r--   0        0        0      373 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/logger_config.py
+-rw-r--r--   0        0        0      889 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/middleware.py
+-rw-r--r--   0        0        0      542 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/provider/__init__.py
+-rw-r--r--   0        0        0      392 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/provider/django_provider/__init__.py
+-rw-r--r--   0        0        0      386 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/provider/fastapi_provider/__init__.py
+-rw-r--r--   0        0        0      404 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/websocket_client/__init__.py
+-rw-r--r--   0        0        0      380 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/websocket_client/websocket_client.py
+-rw-r--r--   0        0        0     1258 2023-04-22 10:03:44.969858 elefantolib-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 elefantolib-0.8.1/setup.py
+-rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 elefantolib-0.8.1/PKG-INFO
```

### Comparing `elefantolib-0.8.0/LICENSE` & `elefantolib-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elefantolib-0.8.0/elefantolib/context/__init__.py` & `elefantolib-0.8.1/elefantolib/context/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from typing import NoReturn, Iterable
+from typing import Iterable, NoReturn
 
-from elefantolib.context import context_service
 from elefantolib import exceptions, provider
-
+from elefantolib.context import context_service
 from elefantolib.http_client import httpx_client
 from elefantolib.websocket_client import websocket_client
 
 
 class BaseContext:
     HTTP_CLIENT = None
     WEBSOCKET_CLIENT = None
```

### Comparing `elefantolib-0.8.0/elefantolib/context/context_service.py` & `elefantolib-0.8.1/elefantolib/context/context_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,14 @@
     def __getattr__(self, item):
         if service := self.__services.get(item):
             return service
 
         self.__services[item] = type(
             item,
             (self._http_client, self._ws_client),
-            {'service_name': item, 'platform_context': self._context}
+            {'service_name': item, 'platform_context': self._context},
         )
 
         return self.__services[item]
 
     def __getitem__(self, item):
         return getattr(self, item)
```

### Comparing `elefantolib-0.8.0/elefantolib/http_client/__init__.py` & `elefantolib-0.8.1/elefantolib/http_client/__init__.py`

 * *Files identical despite different names*

### Comparing `elefantolib-0.8.0/elefantolib/http_client/httpx_client.py` & `elefantolib-0.8.1/elefantolib/http_client/httpx_client.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from functools import partial
 
-import httpx
-
 from elefantolib import logger_config
 from elefantolib.http_client import BaseClient
 
+import httpx
+
 
 logger = logger_config.configure_logger(__name__)
 
 
 class HttpxClient(BaseClient):
 
     def __getattr__(self, item):
```

### Comparing `elefantolib-0.8.0/elefantolib/middleware.py` & `elefantolib-0.8.1/elefantolib/middleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from elefantolib.provider import django_provider, fastapi_provider
-
 from elefantolib import context
+from elefantolib.provider import django_provider
 
 
 class DjangoPlatformContextMiddleware:
 
     def __init__(self, get_response):
         self._get_response = get_response
```

### Comparing `elefantolib-0.8.0/elefantolib/provider/__init__.py` & `elefantolib-0.8.1/elefantolib/provider/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from typing import Protocol, Any
+from typing import Any, Protocol
 
 
 class Provider(Protocol):
 
-    def auth_token(self): ...
+    def auth_token(self):
+        ...
 
-    def correlation_id(self): ...
+    def correlation_id(self):
+        ...
 
-    def locale(self): ...
+    def locale(self):
+        ...
 
 
 class DictProvider:
 
     def __init__(self, context: dict[str, Any]):
         self.context = context
```

### Comparing `elefantolib-0.8.0/pyproject.toml` & `elefantolib-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elefantolib"
-version = "0.8.0"
+version = "0.8.1"
 description = "Elefanto lib"
 authors = ["Elefanto <elefanto@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/elefanto-organization/elefantolib"
 repository = "https://github.com/elefanto-organization/elefantolib"
 classifiers = [
```

### Comparing `elefantolib-0.8.0/PKG-INFO` & `elefantolib-0.8.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elefantolib
-Version: 0.8.0
+Version: 0.8.1
 Summary: Elefanto lib
 Home-page: https://github.com/elefanto-organization/elefantolib
 License: MIT
 Author: Elefanto
 Author-email: elefanto@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,8 +17,14 @@
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: exceptiongroup (>=1.1.1,<2.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: websockets (>=11.0,<12.0)
 Project-URL: Repository, https://github.com/elefanto-organization/elefantolib
 Description-Content-Type: text/x-rst
 
+Elefantolib
+-----------------------
+
+   **NOTE:** After clone this repository you should run command:
+
+   ``console git config core.hooksPath .githooks``
```

