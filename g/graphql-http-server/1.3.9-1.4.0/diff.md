# Comparing `tmp/graphql_http_server-1.3.9.tar.gz` & `tmp/graphql_http_server-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_http_server-1.3.9.tar", last modified: Mon Oct 17 10:28:23 2022, max compression
+gzip compressed data, was "graphql_http_server-1.4.0.tar", last modified: Sat Apr 22 11:47:56 2023, max compression
```

## Comparing `graphql_http_server-1.3.9.tar` & `graphql_http_server-1.4.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 10:28:23.374986 graphql_http_server-1.3.9/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2022-10-17 10:28:14.000000 graphql_http_server-1.3.9/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      143 2022-10-17 10:28:14.000000 graphql_http_server-1.3.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      747 2022-10-17 10:28:23.374986 graphql_http_server-1.3.9/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       90 2022-10-17 10:28:14.000000 graphql_http_server-1.3.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-10-17 10:28:22.000000 graphql_http_server-1.3.9/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 10:28:23.370986 graphql_http_server-1.3.9/graphql_http_server/
--rwxrwxrwx   0 root         (0) root         (0)       71 2022-10-17 10:28:14.000000 graphql_http_server-1.3.9/graphql_http_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      809 2022-10-17 10:28:14.000000 graphql_http_server-1.3.9/graphql_http_server/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 10:28:23.372986 graphql_http_server-1.3.9/graphql_http_server/graphiql/
--rw-rw-rw-   0 root         (0) root         (0)   916167 2022-10-17 10:28:14.000000 graphql_http_server-1.3.9/graphql_http_server/graphiql/index.html
--rw-rw-rw-   0 root         (0) root         (0)     6793 2022-10-17 10:28:14.000000 graphql_http_server-1.3.9/graphql_http_server/helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     8517 2022-10-17 10:28:14.000000 graphql_http_server-1.3.9/graphql_http_server/server.py
--rw-rw-rw-   0 root         (0) root         (0)    12924 2022-10-17 10:28:14.000000 graphql_http_server-1.3.9/graphql_http_server/service_directory.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2022-10-17 10:28:14.000000 graphql_http_server-1.3.9/graphql_http_server/service_directory_default.graphql
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 10:28:23.371986 graphql_http_server-1.3.9/graphql_http_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2022-10-17 10:28:23.000000 graphql_http_server-1.3.9/graphql_http_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      602 2022-10-17 10:28:23.000000 graphql_http_server-1.3.9/graphql_http_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-17 10:28:23.000000 graphql_http_server-1.3.9/graphql_http_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       74 2022-10-17 10:28:23.000000 graphql_http_server-1.3.9/graphql_http_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2022-10-17 10:28:23.000000 graphql_http_server-1.3.9/graphql_http_server.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2022-10-17 10:28:23.375986 graphql_http_server-1.3.9/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1263 2022-10-17 10:28:14.000000 graphql_http_server-1.3.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 10:28:23.374986 graphql_http_server-1.3.9/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-10-17 10:28:14.000000 graphql_http_server-1.3.9/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2022-10-17 10:28:14.000000 graphql_http_server-1.3.9/tests/app.py
--rwxrwxrwx   0 root         (0) root         (0)      476 2022-10-17 10:28:14.000000 graphql_http_server-1.3.9/tests/conftest.py
--rwxrwxrwx   0 root         (0) root         (0)     4884 2022-10-17 10:28:14.000000 graphql_http_server-1.3.9/tests/test_application.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:47:56.753238 graphql_http_server-1.4.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      149 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      747 2023-04-22 11:47:56.753238 graphql_http_server-1.4.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       90 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-22 11:47:56.000000 graphql_http_server-1.4.0/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:47:56.749238 graphql_http_server-1.4.0/graphql_http_server/
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/graphql_http_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/graphql_http_server/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:47:56.751238 graphql_http_server-1.4.0/graphql_http_server/graphiql/
+-rw-rw-rw-   0 root         (0) root         (0)     3103 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/graphql_http_server/graphiql/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     6785 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/graphql_http_server/helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     9135 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/graphql_http_server/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:47:56.751238 graphql_http_server-1.4.0/graphql_http_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      747 2023-04-22 11:47:56.000000 graphql_http_server-1.4.0/graphql_http_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      525 2023-04-22 11:47:56.000000 graphql_http_server-1.4.0/graphql_http_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 11:47:56.000000 graphql_http_server-1.4.0/graphql_http_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-22 11:47:56.000000 graphql_http_server-1.4.0/graphql_http_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-22 11:47:56.000000 graphql_http_server-1.4.0/graphql_http_server.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-22 11:47:56.753238 graphql_http_server-1.4.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:47:56.753238 graphql_http_server-1.4.0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/tests/app.py
+-rwxrwxrwx   0 root         (0) root         (0)      476 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/tests/conftest.py
+-rwxrwxrwx   0 root         (0) root         (0)     1984 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/tests/test_app.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/tests/test_graphql_api.py
```

### Comparing `graphql_http_server-1.3.9/LICENSE` & `graphql_http_server-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.3.9/PKG-INFO` & `graphql_http_server-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql_http_server
-Version: 1.3.9
+Version: 1.4.0
 Summary: HTTPServer for GraphQL.
 Home-page: https://gitlab.com/parob/graphql-http-server
-Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.3.9.zip
+Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.0.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,HTTPServer,werkzeug
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_http_server-1.3.9/graphql_http_server/error.py` & `graphql_http_server-1.4.0/graphql_http_server/error.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.3.9/graphql_http_server/helpers.py` & `graphql_http_server-1.4.0/graphql_http_server/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -177,21 +177,23 @@
     format_error: Optional[Callable[[Exception], Dict]] = None,
 ) -> GraphQLResponse:
     if not format_error:
         from graphql_http_server import GraphQLHTTPServer
         format_error = GraphQLHTTPServer.format_error
 
     if execution_result:
+        response = {}
         if execution_result.errors:
-            response: Optional[Dict[str, Any]] = {
-                "errors": [format_error(e) for e in execution_result.errors]}
-            status_code = 200
-        else:
-            response = {"data": execution_result.data}
-            status_code = 200
+            response["errors"] = [
+                format_error(e) for e in execution_result.errors
+            ]
+        if execution_result.data:
+            response["data"] = execution_result.data
+        status_code = 200
+
     else:
         response = None
         status_code = 200
 
     return GraphQLResponse(response, status_code)
```

### Comparing `graphql_http_server-1.3.9/graphql_http_server/server.py` & `graphql_http_server-1.4.0/graphql_http_server/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import copy
 import json
 
 from inspect import signature
-from typing import Any, List, Callable
+from typing import Any, List, Callable, Optional, Type
 
-from graphql import GraphQLError, GraphQLFormattedError
+from graphql import GraphQLError
 from werkzeug.wrappers import Request, Response
 from werkzeug.test import Client
 
 from graphql.type.schema import GraphQLSchema
 from graphql.execution.execute import ExecutionContext
 
 from graphql_http_server.helpers import (
@@ -18,46 +18,46 @@
     json_encode,
     load_json_body,
     run_http_query
 )
 
 
 def run_simple(
-    schema,
-    root_value: Any = None,
-    middleware: List[Callable[[Callable, Any], Any]] = None,
-    hostname: str = None,
-    port: int = None,
-    **kwargs
+        schema,
+        root_value: Any = None,
+        middleware: List[Callable[[Callable, Any], Any]] = None,
+        hostname: str = None,
+        port: int = None,
+        **kwargs
 ):
-    return GraphQLHTTPServer.from_schema(
+    return GraphQLHTTPServer.from_api(
         schema=schema,
         root_value=root_value,
         middleware=middleware,
         **kwargs
-    ).run_app(
+    ).run(
         hostname=hostname,
         port=port,
         **kwargs
     )
 
 
 graphiql_dir = os.path.join(os.path.dirname(__file__), 'graphiql')
 
 
 class GraphQLHTTPServer:
 
     @classmethod
     def from_api(
-        cls,
-        api,
-        root_value: Any = None,
-        middleware: List[Callable[[Callable, Any], Any]] = None,
-        middleware_on_introspection: bool = False,
-        **kwargs
+            cls,
+            api,
+            root_value: Any = None,
+            middleware: List[Callable[[Callable, Any], Any]] = None,
+            middleware_on_introspection: bool = False,
+            **kwargs
     ) -> 'GraphQLHTTPServer':
         try:
             from graphql_api import GraphQLAPI, GraphQLExecutor
             from graphql_api.context import GraphQLContext
 
         except ImportError:
             raise ImportError(
@@ -65,77 +65,89 @@
             )
 
         api: GraphQLAPI = api
 
         executor = api.executor(
             root_value=root_value,
             middleware=middleware,
-            middleware_on_introspection=middleware_on_introspection
+            middleware_on_introspection=middleware_on_introspection,
+            error_protection=api.error_protection
         )
 
         schema: GraphQLSchema = executor.schema
         meta = executor.meta
         root_value = executor.root_value
 
         middleware = GraphQLExecutor.adapt_middleware(executor.middleware)
         context = GraphQLContext(schema=schema, meta=meta, executor=executor)
 
         return GraphQLHTTPServer(
             schema=schema,
             root_value=root_value,
             middleware=middleware,
             context=context,
+            execution_context_class=executor.execution_context_class,
             **kwargs
         )
 
     def __init__(
-        self,
-        schema: GraphQLSchema,
-        root_value: Any = None,
-        middleware: List[Callable[[Callable, Any], Any]] = None,
-        context: Any = None,
-        serve_graphiql: bool = True,
-        graphiql_default_query: str = None,
-        graphiql_default_variables: str = None,
-        allow_cors: bool = False
+            self,
+            schema: GraphQLSchema,
+            root_value: Any = None,
+            middleware: List[Callable[[Callable, Any], Any]] = None,
+            context: Any = None,
+            serve_graphiql: bool = True,
+            graphiql_default_query: str = None,
+            graphiql_default_variables: str = None,
+            allow_cors: bool = False,
+            health_path: str = None,
+            execution_context_class: Optional[Type[ExecutionContext]] = None
     ):
 
         if middleware is None:
             middleware = []
 
         self.schema = schema
         self.root_value = root_value
         self.middleware = middleware
         self.context = context
         self.serve_graphiql = serve_graphiql
         self.graphiql_default_query = graphiql_default_query
         self.graphiql_default_variables = graphiql_default_variables
         self.allow_cors = allow_cors
+        self.health_path = health_path
+        self.execution_context_class = execution_context_class
 
     def create_context(self):
         return copy.copy(self.context)
 
     @staticmethod
-    def format_error(error: GraphQLError) -> GraphQLFormattedError:
+    def format_error(error: GraphQLError) -> {}:
         return error.formatted
 
     encode = staticmethod(json_encode)
 
     def dispatch(
-        self,
-        request: Request,
-        context=None,
-        execution_context_class: ExecutionContext = None
+            self,
+            request: Request,
+            context=None,
+            execution_context_class: ExecutionContext = None
     ) -> Response:
         headers = {}
 
+        if execution_context_class is None:
+            execution_context_class = self.execution_context_class
+
         try:
             request_method = request.method.lower()
             data = self.parse_body(request=request)
 
+            if self.health_path and request.path == self.health_path:
+                return Response("OK")
+
             if context is None:
                 context = self.create_context()
 
             is_get = request_method == 'get'
             should_serve = self.should_serve_graphiql(request=request)
 
             show_graphiql = is_get and should_serve
@@ -143,26 +155,26 @@
                 graphiql_path = os.path.join(
                     graphiql_dir,
                     'index.html'
                 )
                 if self.graphiql_default_query:
                     default_query = json.dumps(self.graphiql_default_query)
                 else:
-                    default_query = 'undefined'
+                    default_query = '""'
 
                 if self.graphiql_default_variables:
                     default_variables = json.dumps(
                         self.graphiql_default_variables
                     )
                 else:
-                    default_variables = 'undefined'
+                    default_variables = '""'
 
                 html = open(graphiql_path, 'r').read()
-                html = html.replace('"DEFAULT_QUERY"', default_query)
-                html = html.replace('"DEFAULT_VARIABLES"', default_variables)
+                html = html.replace('DEFAULT_QUERY', default_query)
+                html = html.replace('DEFAULT_VARIABLES', default_variables)
 
                 return Response(html, content_type='text/html')
 
             if self.allow_cors:
                 headers = {
                     "Access-Control-Allow-Credentials": "true",
                     "Access-Control-Allow-Headers": "Content-Type",
@@ -184,38 +196,40 @@
                 middleware=self.middleware,
                 context_value=context,
                 execution_context_class=execution_context_class
             )
             result, status_code = encode_execution_results(
                 execution_results,
                 is_batch=isinstance(data, list),
-                format_error=self.format_error,
                 encode=self.encode
             )
 
             return Response(
                 result,
                 status=status_code,
                 content_type='application/json',
                 headers=headers
             )
 
         except HttpQueryError as e:
             return self.error_response(e, headers)
 
-    def error_response(self, e, headers={}):
+    def error_response(self, e, headers=None):
+        if headers is None:
+            headers = {}
         return Response(
             self.encode({
                 'errors': [str(e)]
             }),
             status=getattr(e, "status_code", 200),
-            headers={**getattr(e, "headers", {}), **headers},
+            headers={**(getattr(e, "headers", {}) or {}), **headers},
             content_type='application/json'
         )
 
+    # noinspection PyMethodMayBeStatic
     def parse_body(self, request):
         content_type = request.mimetype
         if content_type == 'application/graphql':
             return {'query': request.data.decode('utf8')}
 
         elif content_type == 'application/json':
             return load_json_body(request.data.decode('utf8'))
@@ -230,50 +244,47 @@
 
     def should_serve_graphiql(self, request):
         if not self.serve_graphiql or 'raw' in request.args:
             return False
 
         return self.request_wants_html(request=request)
 
+    # noinspection PyMethodMayBeStatic
     def request_wants_html(self, request):
         best = request.accept_mimetypes \
             .best_match(['application/json', 'text/html'])
 
         if best == 'text/html':
             accept_best = request.accept_mimetypes[best]
             accept_json = request.accept_mimetypes['application/json']
             return accept_best > accept_json
 
         return False
 
     def app(
-        self,
-        main: Callable[[Request], Response] = None
+            self,
+            main: Callable[[Request], Response] = None
     ):
-
         @Request.application
         def app(request):
-            try:
-                if main is not None:
-                    return main(request)
-                return self.dispatch(request=request)
-            except Exception as e:
-                return self.error_response(e)
+            if main is not None:
+                return main(request)
+            return self.dispatch(request=request)
 
         return app
 
     def client(self, main=None):
         return Client(self.app(main=main), Response)
 
     def run(
-        self,
-        main: Callable[[Request], Response] = None,
-        hostname: str = None,
-        port: int = None,
-        **kwargs
+            self,
+            main: Callable[[Request], Response] = None,
+            hostname: str = None,
+            port: int = None,
+            **kwargs
     ):
         if hostname is None:
             hostname = 'localhost'
 
         if port is None:
             port = 5000
```

### Comparing `graphql_http_server-1.3.9/graphql_http_server.egg-info/PKG-INFO` & `graphql_http_server-1.4.0/graphql_http_server.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-http-server
-Version: 1.3.9
+Version: 1.4.0
 Summary: HTTPServer for GraphQL.
 Home-page: https://gitlab.com/parob/graphql-http-server
-Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.3.9.zip
+Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.0.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,HTTPServer,werkzeug
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_http_server-1.3.9/graphql_http_server.egg-info/SOURCES.txt` & `graphql_http_server-1.4.0/graphql_http_server.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 VERSION
 setup.cfg
 setup.py
 graphql_http_server/__init__.py
 graphql_http_server/error.py
 graphql_http_server/helpers.py
 graphql_http_server/server.py
-graphql_http_server/service_directory.py
-graphql_http_server/service_directory_default.graphql
 graphql_http_server.egg-info/PKG-INFO
 graphql_http_server.egg-info/SOURCES.txt
 graphql_http_server.egg-info/dependency_links.txt
 graphql_http_server.egg-info/requires.txt
 graphql_http_server.egg-info/top_level.txt
 graphql_http_server/graphiql/index.html
 tests/__init__.py
 tests/app.py
 tests/conftest.py
-tests/test_application.py
+tests/test_app.py
+tests/test_graphql_api.py
```

### Comparing `graphql_http_server-1.3.9/setup.py` & `graphql_http_server-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,19 @@
                  f'archive/master/graphql-http-server-v{version}.zip',
     keywords=['GraphQL', 'HTTPServer', 'werkzeug'],
     description='HTTPServer for GraphQL.',
     long_description=readme,
     long_description_content_type='text/markdown',
     install_requires=[
         "graphql-core>=3.2.0",
+        "graphql-api>=1.3.0",
         "werkzeug>=2.2.2",
         "context-helper>=1.0.2",
         "packaging>=21.3",
+        "graphql-schema-diff>=1.2.4"
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

