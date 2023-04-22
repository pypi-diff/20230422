# Comparing `tmp/asyncio_simple_http_server-0.0.1.tar.gz` & `tmp/asyncio_simple_http_server-0.0.2.tar.gz`

## Comparing `asyncio_simple_http_server-0.0.1.tar` & `asyncio_simple_http_server-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,13 @@
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/demo.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/.idea/asyncio-simple-http-server.iml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/src/asyncio_simple_http_server/__init__.py
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/src/asyncio_simple_http_server/http_util.py
--rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/src/asyncio_simple_http_server/server.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/tests/test_http_util.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/LICENSE
--rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/README.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.2/demo.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.2/src/asyncio_simple_http_server/__init__.py
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.2/src/asyncio_simple_http_server/http_util.py
+-rw-r--r--   0        0        0     9332 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.2/src/asyncio_simple_http_server/server.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.2/tests/test_http_util.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.2/README.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 asyncio_simple_http_server-0.0.2/PKG-INFO
```

### Comparing `asyncio_simple_http_server-0.0.1/demo.py` & `asyncio_simple_http_server-0.0.2/demo.py`

 * *Files identical despite different names*

### Comparing `asyncio_simple_http_server-0.0.1/.github/workflows/python-package.yml` & `asyncio_simple_http_server-0.0.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `asyncio_simple_http_server-0.0.1/src/asyncio_simple_http_server/__init__.py` & `asyncio_simple_http_server-0.0.2/src/asyncio_simple_http_server/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncio_simple_http_server-0.0.1/src/asyncio_simple_http_server/http_util.py` & `asyncio_simple_http_server-0.0.2/src/asyncio_simple_http_server/http_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,26 +96,30 @@
     if path.startswith('//'):
         path = '/' + path.lstrip('/')  # Reduce to a single /
     return path
 
 
 async def http_parser(reader: asyncio.StreamReader, timeout=10) -> HttpRequest:
     line = await asyncio.wait_for(reader.readuntil(b'\r\n'), timeout)
+    if not line:
+        return None
+
     words = line.decode().split()
 
     method, path, version = (words[0], words[1], words[2])
     path = _clean_path(path)
 
     headers = HttpHeaders()
     while True:
         line = await asyncio.wait_for(reader.readuntil(b'\r\n'), timeout)
-        if line == b'\r\n':
+        if not line or line == b'\r\n':
             break
-        key, value = line.decode().strip().split(': ', 1)
-        headers.add(key, value)
+
+        key, value = line.decode().split(': ', 1)
+        headers.add(key.strip(), value.strip())
 
     content_length = headers.get('content-length', -1, int)
 
     if content_length > 0:
         body = await asyncio.wait_for(reader.readexactly(content_length), timeout)
     else:
         body = None
```

### Comparing `asyncio_simple_http_server-0.0.1/src/asyncio_simple_http_server/server.py` & `asyncio_simple_http_server-0.0.2/src/asyncio_simple_http_server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,35 +164,36 @@
 
     async def serve_forever(self):
         if self._server is None:
             raise RuntimeError('Server not started yet')
 
         async with self._server:
             await self._server.serve_forever()
-        print('foo')
 
     def bind_address_description(self):
         return ', '.join(str(sock.getsockname()) for sock in self._server.sockets)
 
     async def _handle_client(self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter) -> None:
         try:
             while True:
                 request = await http_parser(reader, self.read_timeout)
+                if request is None:
+                    break
                 logger.debug('received request %s %s', request.method, request.path)
 
                 route, method = self._find_route(request)
                 if method:
                     logger.debug('found matching route %s calling method %s', route, method)
                     await self._process_request(writer, route, method, request)
                 else:
                     logger.warning('unable to find any matching route for %s %s', request.method, request.path)
                     response = self.build_http_404_response(request.method, request.path)
                     await self._send_response(writer, request, response)
 
-        except asyncio.exceptions.IncompleteReadError as e:
+        except (TimeoutError, asyncio.TimeoutError, asyncio.exceptions.IncompleteReadError) as e:
             logger.warning('got a failure %s. disconnecting the client', type(e))
         except Exception as e:
             logger.exception('got a failure %s. disconnecting the client: %s', type(e), e)
         finally:
             writer.close()
 
     def build_http_404_response(self, _method: str, _path: str) -> HttpResponse:
```

### Comparing `asyncio_simple_http_server-0.0.1/tests/test_http_util.py` & `asyncio_simple_http_server-0.0.2/tests/test_http_util.py`

 * *Files identical despite different names*

### Comparing `asyncio_simple_http_server-0.0.1/.gitignore` & `asyncio_simple_http_server-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `asyncio_simple_http_server-0.0.1/LICENSE` & `asyncio_simple_http_server-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncio_simple_http_server-0.0.1/README.md` & `asyncio_simple_http_server-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 ## asyncio simple HTTP Server
 
 This package contains a really Simple Http API Server using asyncio.
 **It is not meant to be used in production**. It is more a lightweight alternative to SimpleHTTPServer but for writing HTTP APIs.
 
+### Install the package
+You can find the package at https://pypi.org/project/asyncio-simple-http-server. and install it using pip. (Python >=3.8 is required)
+```bash
+$ pip install asyncio-simple-http-server
+```
+
 ### Usage Example
 To start the server is the usual straightforward asyncio server code,
 plus some registration for your HTTP API handlers.
 
 ```python
 from asyncio_simple_http_server import HttpServer
 import asyncio
@@ -43,15 +49,15 @@
 class MyHandler:
     # The @uri_mapping decorator exposes this method as an HTTP API
     # so you can just do a HTTP GET /test-get
     # and you'll get back a 200 OK with a json body of {a: 10}
     # return values will be converted with json.dumps()
     @uri_mapping('/test-get')
     def test_get(self):
-        return {a: 10}
+        return {'a': 10}
 
     # In this case the mapping says that we want a POST method
     # and by passing an argument named 'body' we will get the
     # body passed to the endpoint parsed with json.loads()
     # We execute "some logic" and we return the body
     @uri_mapping('/test-post', method='POST')
     def test_post(self, body):
```

### Comparing `asyncio_simple_http_server-0.0.1/pyproject.toml` & `asyncio_simple_http_server-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "asyncio_simple_http_server"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Matteo Bertozzi", email="mbertozzi@apache.org" },
 ]
 description = "A Simple Http API Server using asyncio"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/matteobertozzi/asyncio-simple-http-server"
-"Bug Tracker" = "https://github.com/matteobertozzi/asyncio-simple-http-server/issues"
+"Bug Tracker" = "https://github.com/matteobertozzi/asyncio-simple-http-server/issues"
```

### Comparing `asyncio_simple_http_server-0.0.1/PKG-INFO` & `asyncio_simple_http_server-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncio_simple_http_server
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Simple Http API Server using asyncio
 Project-URL: Homepage, https://github.com/matteobertozzi/asyncio-simple-http-server
 Project-URL: Bug Tracker, https://github.com/matteobertozzi/asyncio-simple-http-server/issues
 Author-email: Matteo Bertozzi <mbertozzi@apache.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,20 @@
 Description-Content-Type: text/markdown
 
 ## asyncio simple HTTP Server
 
 This package contains a really Simple Http API Server using asyncio.
 **It is not meant to be used in production**. It is more a lightweight alternative to SimpleHTTPServer but for writing HTTP APIs.
 
+### Install the package
+You can find the package at https://pypi.org/project/asyncio-simple-http-server. and install it using pip. (Python >=3.8 is required)
+```bash
+$ pip install asyncio-simple-http-server
+```
+
 ### Usage Example
 To start the server is the usual straightforward asyncio server code,
 plus some registration for your HTTP API handlers.
 
 ```python
 from asyncio_simple_http_server import HttpServer
 import asyncio
@@ -57,15 +63,15 @@
 class MyHandler:
     # The @uri_mapping decorator exposes this method as an HTTP API
     # so you can just do a HTTP GET /test-get
     # and you'll get back a 200 OK with a json body of {a: 10}
     # return values will be converted with json.dumps()
     @uri_mapping('/test-get')
     def test_get(self):
-        return {a: 10}
+        return {'a': 10}
 
     # In this case the mapping says that we want a POST method
     # and by passing an argument named 'body' we will get the
     # body passed to the endpoint parsed with json.loads()
     # We execute "some logic" and we return the body
     @uri_mapping('/test-post', method='POST')
     def test_post(self, body):
```

