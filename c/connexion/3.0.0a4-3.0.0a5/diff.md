# Comparing `tmp/connexion-3.0.0a4.tar.gz` & `tmp/connexion-3.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connexion-3.0.0a4.tar", max compression
+gzip compressed data, was "connexion-3.0.0a5.tar", max compression
```

## Comparing `connexion-3.0.0a4.tar` & `connexion-3.0.0a5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     3091 2023-03-30 20:21:17.453194 connexion-3.0.0a4/ARCHITECTURE.rst
--rw-r--r--   0        0        0      878 2023-03-30 20:21:17.453194 connexion-3.0.0a4/CONTRIBUTING.rst
--rw-r--r--   0        0        0      556 2023-03-30 20:21:17.453194 connexion-3.0.0a4/LICENSE.txt
--rw-r--r--   0        0        0    25923 2023-03-30 20:21:17.453194 connexion-3.0.0a4/README.rst
--rwxr-xr-x   0        0        0     1351 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/__init__.py
--rw-r--r--   0        0        0      144 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/__main__.py
--rw-r--r--   0        0        0      250 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/apps/__init__.py
--rw-r--r--   0        0        0    11578 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/apps/abstract.py
--rw-r--r--   0        0        0     7579 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/apps/asynchronous.py
--rw-r--r--   0        0        0    10343 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/apps/flask.py
--rw-r--r--   0        0        0     6592 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/cli.py
--rw-r--r--   0        0        0      981 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/context.py
--rw-r--r--   0        0        0     1081 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/datastructures.py
--rw-r--r--   0        0        0      174 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/decorators/__init__.py
--rw-r--r--   0        0        0     6489 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/decorators/main.py
--rw-r--r--   0        0        0    15506 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/decorators/parameter.py
--rw-r--r--   0        0        0     7026 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/decorators/response.py
--rw-r--r--   0        0        0     5541 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/frameworks/__init__.py
--rw-r--r--   0        0        0     1069 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/frameworks/abstract.py
--rw-r--r--   0        0        0     4096 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/frameworks/flask.py
--rw-r--r--   0        0        0     2795 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/frameworks/starlette.py
--rw-r--r--   0        0        0     1259 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/handlers.py
--rw-r--r--   0        0        0      227 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/http_facts.py
--rw-r--r--   0        0        0     4661 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/json_schema.py
--rw-r--r--   0        0        0     2856 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/jsonifier.py
--rw-r--r--   0        0        0     6973 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/lifecycle.py
--rw-r--r--   0        0        0       91 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/middleware/__init__.py
--rw-r--r--   0        0        0     9853 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/middleware/abstract.py
--rw-r--r--   0        0        0     1407 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/middleware/context.py
--rw-r--r--   0        0        0     2411 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/middleware/exceptions.py
--rw-r--r--   0        0        0      964 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/middleware/lifespan.py
--rw-r--r--   0        0        0    14784 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/middleware/main.py
--rw-r--r--   0        0        0     5470 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/middleware/request_validation.py
--rw-r--r--   0        0        0     5598 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/middleware/response_validation.py
--rw-r--r--   0        0        0     4918 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/middleware/routing.py
--rw-r--r--   0        0        0     9322 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/middleware/security.py
--rw-r--r--   0        0        0     8208 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/middleware/swagger_ui.py
--rw-r--r--   0        0        0     1828 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/mock.py
--rw-r--r--   0        0        0      531 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/operations/__init__.py
--rw-r--r--   0        0        0     6666 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/operations/abstract.py
--rw-r--r--   0        0        0     8983 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/operations/openapi.py
--rw-r--r--   0        0        0    11327 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/operations/swagger2.py
--rw-r--r--   0        0        0     4376 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/options.py
--rw-r--r--   0        0        0     2255 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/problem.py
--rw-r--r--   0        0        0    12118 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/resolver.py
--rw-r--r--   0        0        0    40020 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/resources/schemas/v2.0/schema.json
--rw-r--r--   0        0        0    35456 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/resources/schemas/v3.0/schema.json
--rw-r--r--   0        0        0    16336 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/security.py
--rw-r--r--   0        0        0     9537 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/spec.py
--rw-r--r--   0        0        0     2153 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/testing.py
--rw-r--r--   0        0        0    11661 2023-03-30 20:21:17.453194 connexion-3.0.0a4/connexion/uri_parsing.py
--rw-r--r--   0        0        0    12142 2023-03-30 20:21:17.457194 connexion-3.0.0a4/connexion/utils.py
--rw-r--r--   0        0        0      892 2023-03-30 20:21:17.457194 connexion-3.0.0a4/connexion/validators/__init__.py
--rw-r--r--   0        0        0     7075 2023-03-30 20:21:17.457194 connexion-3.0.0a4/connexion/validators/abstract.py
--rw-r--r--   0        0        0     3280 2023-03-30 20:21:17.457194 connexion-3.0.0a4/connexion/validators/form_data.py
--rw-r--r--   0        0        0     4753 2023-03-30 20:21:17.457194 connexion-3.0.0a4/connexion/validators/json.py
--rw-r--r--   0        0        0     4682 2023-03-30 20:21:17.457194 connexion-3.0.0a4/connexion/validators/parameter.py
--rw-r--r--   0        0        0     2874 2023-03-30 20:21:17.825196 connexion-3.0.0a4/pyproject.toml
--rw-r--r--   0        0        0    28529 1970-01-01 00:00:00.000000 connexion-3.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0     3091 2023-04-22 20:10:31.091928 connexion-3.0.0a5/ARCHITECTURE.rst
+-rw-r--r--   0        0        0      878 2023-04-22 20:10:31.091928 connexion-3.0.0a5/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      556 2023-04-22 20:10:31.091928 connexion-3.0.0a5/LICENSE.txt
+-rw-r--r--   0        0        0    25923 2023-04-22 20:10:31.091928 connexion-3.0.0a5/README.rst
+-rwxr-xr-x   0        0        0     1351 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/__main__.py
+-rw-r--r--   0        0        0      250 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/apps/__init__.py
+-rw-r--r--   0        0        0    12633 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/apps/abstract.py
+-rw-r--r--   0        0        0     7794 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/apps/asynchronous.py
+-rw-r--r--   0        0        0    10558 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/apps/flask.py
+-rw-r--r--   0        0        0     5332 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/cli.py
+-rw-r--r--   0        0        0      981 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/context.py
+-rw-r--r--   0        0        0     1081 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/datastructures.py
+-rw-r--r--   0        0        0      174 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/decorators/__init__.py
+-rw-r--r--   0        0        0     6489 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/decorators/main.py
+-rw-r--r--   0        0        0    15027 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/decorators/parameter.py
+-rw-r--r--   0        0        0     7026 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/decorators/response.py
+-rw-r--r--   0        0        0     5541 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/frameworks/__init__.py
+-rw-r--r--   0        0        0     1069 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/frameworks/abstract.py
+-rw-r--r--   0        0        0     4096 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/frameworks/flask.py
+-rw-r--r--   0        0        0     2795 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/frameworks/starlette.py
+-rw-r--r--   0        0        0     1259 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/handlers.py
+-rw-r--r--   0        0        0      227 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/http_facts.py
+-rw-r--r--   0        0        0     4661 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/json_schema.py
+-rw-r--r--   0        0        0     2856 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/jsonifier.py
+-rw-r--r--   0        0        0     6973 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/lifecycle.py
+-rw-r--r--   0        0        0      111 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/__init__.py
+-rw-r--r--   0        0        0     9843 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/abstract.py
+-rw-r--r--   0        0        0     1407 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/context.py
+-rw-r--r--   0        0        0     2394 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/exceptions.py
+-rw-r--r--   0        0        0      940 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/lifespan.py
+-rw-r--r--   0        0        0    17217 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/main.py
+-rw-r--r--   0        0        0     6591 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/request_validation.py
+-rw-r--r--   0        0        0     5598 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/response_validation.py
+-rw-r--r--   0        0        0     4908 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/routing.py
+-rw-r--r--   0        0        0     4659 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/security.py
+-rw-r--r--   0        0        0     8198 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/swagger_ui.py
+-rw-r--r--   0        0        0     1828 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/mock.py
+-rw-r--r--   0        0        0      531 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/operations/__init__.py
+-rw-r--r--   0        0        0     6666 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/operations/abstract.py
+-rw-r--r--   0        0        0     8983 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/operations/openapi.py
+-rw-r--r--   0        0        0    11327 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/operations/swagger2.py
+-rw-r--r--   0        0        0     4376 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/options.py
+-rw-r--r--   0        0        0     2255 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/problem.py
+-rw-r--r--   0        0        0    12118 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/resolver.py
+-rw-r--r--   0        0        0    40020 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/resources/schemas/v2.0/schema.json
+-rw-r--r--   0        0        0    35456 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/resources/schemas/v3.0/schema.json
+-rw-r--r--   0        0        0    21402 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/security.py
+-rw-r--r--   0        0        0     9537 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/spec.py
+-rw-r--r--   0        0        0     2153 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/testing.py
+-rw-r--r--   0        0        0    11661 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/uri_parsing.py
+-rw-r--r--   0        0        0    12674 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/utils.py
+-rw-r--r--   0        0        0      892 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/validators/__init__.py
+-rw-r--r--   0        0        0     7075 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/validators/abstract.py
+-rw-r--r--   0        0        0     3280 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/validators/form_data.py
+-rw-r--r--   0        0        0     4753 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/validators/json.py
+-rw-r--r--   0        0        0     5181 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/validators/parameter.py
+-rw-r--r--   0        0        0     2874 2023-04-22 20:10:32.479941 connexion-3.0.0a5/pyproject.toml
+-rw-r--r--   0        0        0    28529 1970-01-01 00:00:00.000000 connexion-3.0.0a5/PKG-INFO
```

### Comparing `connexion-3.0.0a4/ARCHITECTURE.rst` & `connexion-3.0.0a5/ARCHITECTURE.rst`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/CONTRIBUTING.rst` & `connexion-3.0.0a5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/LICENSE.txt` & `connexion-3.0.0a5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/README.rst` & `connexion-3.0.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/__init__.py` & `connexion-3.0.0a5/connexion/__init__.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/apps/abstract.py` & `connexion-3.0.0a5/connexion/apps/abstract.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 application.
 """
 import abc
 import pathlib
 import typing as t
 
 from starlette.testclient import TestClient
-from starlette.types import Receive, Scope, Send
+from starlette.types import ASGIApp, Receive, Scope, Send
 
 from connexion.jsonifier import Jsonifier
-from connexion.middleware import ConnexionMiddleware, SpecMiddleware
+from connexion.middleware import ConnexionMiddleware, MiddlewarePosition, SpecMiddleware
 from connexion.middleware.lifespan import Lifespan
 from connexion.resolver import Resolver
 from connexion.uri_parsing import AbstractURIParser
 
 
 class AbstractApp:
     """
@@ -43,14 +43,15 @@
         resolver: t.Optional[t.Union[Resolver, t.Callable]] = None,
         resolver_error: t.Optional[int] = None,
         strict_validation: t.Optional[bool] = None,
         swagger_ui_options: t.Optional[dict] = None,
         uri_parser_class: t.Optional[AbstractURIParser] = None,
         validate_responses: t.Optional[bool] = None,
         validator_map: t.Optional[dict] = None,
+        security_map: t.Optional[dict] = None,
     ) -> None:
         """
         :param import_name: The name of the package or module that this object belongs to. If you
             are using a single module, __name__ is always the correct value. If you however are
             using a package, it’s usually recommended to hardcode the name of your package there.
         :param middlewares: The list of middlewares to wrap around the application. Defaults to
             :obj:`middleware.main.ConnexionmMiddleware.default_middlewares`
@@ -73,14 +74,16 @@
         :param swagger_ui_options: A :class:`options.ConnexionOptions` instance with configuration
             options for the swagger ui.
         :param uri_parser_class: Class to use for uri parsing. See :mod:`uri_parsing`.
         :param validate_responses: Whether to validate responses against the specification. This has
             an impact on performance. Defaults to False.
         :param validator_map: A dictionary of validators to use. Defaults to
             :obj:`validators.VALIDATOR_MAP`.
+        :param security_map: A dictionary of security handlers to use. Defaults to
+            :obj:`security.SECURITY_HANDLERS`
         """
         self.middleware = ConnexionMiddleware(
             self.middleware_app,
             import_name=import_name,
             lifespan=lifespan,
             middlewares=middlewares,
             specification_dir=specification_dir,
@@ -91,16 +94,31 @@
             pythonic_params=pythonic_params,
             resolver=resolver,
             resolver_error=resolver_error,
             strict_validation=strict_validation,
             uri_parser_class=uri_parser_class,
             validate_responses=validate_responses,
             validator_map=validator_map,
+            security_map=security_map,
         )
 
+    def add_middleware(
+        self,
+        middleware_class: t.Type[ASGIApp],
+        position: MiddlewarePosition = MiddlewarePosition.BEFORE_CONTEXT,
+        **options: t.Any,
+    ) -> None:
+        """Add a middleware to the stack on the specified position.
+
+        :param middleware_class: Middleware class to add
+        :param position: Position to add the middleware, one of the MiddlewarePosition Enum
+        :param options: Options to pass to the middleware_class on initialization
+        """
+        self.middleware.add_middleware(middleware_class, position=position, **options)
+
     def add_api(
         self,
         specification: t.Union[pathlib.Path, str, dict],
         *,
         base_path: t.Optional[str] = None,
         arguments: t.Optional[dict] = None,
         auth_all_paths: t.Optional[bool] = None,
@@ -109,14 +127,15 @@
         resolver: t.Optional[t.Union[Resolver, t.Callable]] = None,
         resolver_error: t.Optional[int] = None,
         strict_validation: t.Optional[bool] = None,
         swagger_ui_options: t.Optional[dict] = None,
         uri_parser_class: t.Optional[AbstractURIParser] = None,
         validate_responses: t.Optional[bool] = None,
         validator_map: t.Optional[dict] = None,
+        security_map: t.Optional[dict] = None,
         **kwargs,
     ) -> t.Any:
         """
         Register een API represented by a single OpenAPI specification on this application.
         Multiple APIs can be registered on a single application.
 
         :param specification: OpenAPI specification. Can be provided either as dict, or as path
@@ -139,14 +158,16 @@
         :param swagger_ui_options: A :class:`options.ConnexionOptions` instance with configuration
             options for the swagger ui.
         :param uri_parser_class: Class to use for uri parsing. See :mod:`uri_parsing`.
         :param validate_responses: Whether to validate responses against the specification. This has
             an impact on performance. Defaults to False.
         :param validator_map: A dictionary of validators to use. Defaults to
             :obj:`validators.VALIDATOR_MAP`
+        :param security_map: A dictionary of security handlers to use. Defaults to
+            :obj:`security.SECURITY_HANDLERS`
         :param kwargs: Additional keyword arguments to pass to the `add_api` method of the managed
             middlewares. This can be used to pass arguments to middlewares added beyond the default
             ones.
 
         :return: The Api registered on the middleware application wrapping the framework.
         """
         return self.middleware.add_api(
@@ -159,14 +180,15 @@
             resolver=resolver,
             resolver_error=resolver_error,
             strict_validation=strict_validation,
             swagger_ui_options=swagger_ui_options,
             uri_parser_class=uri_parser_class,
             validate_responses=validate_responses,
             validator_map=validator_map,
+            security_map=security_map,
             **kwargs,
         )
 
     def add_url_rule(
         self, rule, endpoint: str = None, view_func: t.Callable = None, **options
     ):
         """
```

### Comparing `connexion-3.0.0a4/connexion/apps/asynchronous.py` & `connexion-3.0.0a5/connexion/apps/asynchronous.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,14 +131,15 @@
         resolver: t.Optional[t.Union[Resolver, t.Callable]] = None,
         resolver_error: t.Optional[int] = None,
         strict_validation: t.Optional[bool] = None,
         swagger_ui_options: t.Optional[dict] = None,
         uri_parser_class: t.Optional[AbstractURIParser] = None,
         validate_responses: t.Optional[bool] = None,
         validator_map: t.Optional[dict] = None,
+        security_map: t.Optional[dict] = None,
     ) -> None:
         """
         :param import_name: The name of the package or module that this object belongs to. If you
             are using a single module, __name__ is always the correct value. If you however are
             using a package, it’s usually recommended to hardcode the name of your package there.
         :param middlewares: The list of middlewares to wrap around the application. Defaults to
             :obj:`middleware.main.ConnexionmMiddleware.default_middlewares`
@@ -161,14 +162,16 @@
         :param swagger_ui_options: A :class:`options.ConnexionOptions` instance with configuration
             options for the swagger ui.
         :param uri_parser_class: Class to use for uri parsing. See :mod:`uri_parsing`.
         :param validate_responses: Whether to validate responses against the specification. This has
             an impact on performance. Defaults to False.
         :param validator_map: A dictionary of validators to use. Defaults to
             :obj:`validators.VALIDATOR_MAP`.
+        :param security_map: A dictionary of security handlers to use. Defaults to
+            :obj:`security.SECURITY_HANDLERS`
         """
         self.middleware_app: AsyncMiddlewareApp = AsyncMiddlewareApp()
 
         super().__init__(
             import_name,
             lifespan=lifespan,
             middlewares=middlewares,
@@ -180,14 +183,15 @@
             resolver=resolver,
             resolver_error=resolver_error,
             strict_validation=strict_validation,
             swagger_ui_options=swagger_ui_options,
             uri_parser_class=uri_parser_class,
             validate_responses=validate_responses,
             validator_map=validator_map,
+            security_map=security_map,
         )
 
     def add_url_rule(
         self, rule, endpoint: str = None, view_func: t.Callable = None, **options
     ):
         self.middleware_app.add_url_rule(
             rule, endpoint=endpoint, view_func=view_func, **options
```

### Comparing `connexion-3.0.0a4/connexion/apps/flask.py` & `connexion-3.0.0a5/connexion/apps/flask.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,15 @@
         resolver: t.Optional[t.Union[Resolver, t.Callable]] = None,
         resolver_error: t.Optional[int] = None,
         strict_validation: t.Optional[bool] = None,
         swagger_ui_options: t.Optional[dict] = None,
         uri_parser_class: t.Optional[AbstractURIParser] = None,
         validate_responses: t.Optional[bool] = None,
         validator_map: t.Optional[dict] = None,
+        security_map: t.Optional[dict] = None,
     ):
         """
         :param import_name: The name of the package or module that this object belongs to. If you
             are using a single module, __name__ is always the correct value. If you however are
             using a package, it’s usually recommended to hardcode the name of your package there.
         :param lifespan: A lifespan context function, which can be used to perform startup and
             shutdown tasks.
@@ -221,14 +222,16 @@
         :param strict_validation: When True, extra form or query parameters not defined in the
             specification result in a validation error. Defaults to False.
         :param uri_parser_class: Class to use for uri parsing. See :mod:`uri_parsing`.
         :param validate_responses: Whether to validate responses against the specification. This has
             an impact on performance. Defaults to False.
         :param validator_map: A dictionary of validators to use. Defaults to
             :obj:`validators.VALIDATOR_MAP`.
+        :param security_map: A dictionary of security handlers to use. Defaults to
+            :obj:`security.SECURITY_HANDLERS`
         """
         self.middleware_app = FlaskMiddlewareApp(import_name, server_args or {})
         self.app = self.middleware_app.app
         super().__init__(
             import_name,
             lifespan=lifespan,
             middlewares=middlewares,
@@ -240,14 +243,15 @@
             resolver=resolver,
             resolver_error=resolver_error,
             strict_validation=strict_validation,
             swagger_ui_options=swagger_ui_options,
             uri_parser_class=uri_parser_class,
             validate_responses=validate_responses,
             validator_map=validator_map,
+            security_map=security_map,
         )
 
     def add_url_rule(
         self, rule, endpoint: str = None, view_func: t.Callable = None, **options
     ):
         self.middleware_app.add_url_rule(
             rule, endpoint=endpoint, view_func=view_func, **options
```

### Comparing `connexion-3.0.0a4/connexion/cli.py` & `connexion-3.0.0a5/connexion/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,58 +5,41 @@
 
 import logging
 import sys
 from os import path
 
 import click
 import importlib_metadata
-from clickclick import AliasedGroup, fatal_error
+from clickclick import AliasedGroup
 
 import connexion
 from connexion.mock import MockResolver
 
 logger = logging.getLogger("connexion.cli")
-CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
+
 FLASK_APP = "flask"
-AVAILABLE_SERVERS = {
-    "flask": [FLASK_APP],
-    "gevent": [FLASK_APP],
-    "tornado": [FLASK_APP],
-}
+ASYNC_APP = "async"
 AVAILABLE_APPS = {
-    FLASK_APP: "connexion.apps.flask_app.FlaskApp",
+    FLASK_APP: "connexion.apps.flask.FlaskApp",
+    ASYNC_APP: "connexion.apps.asynchronous.AsyncApp",
 }
-DEFAULT_SERVERS = {
-    FLASK_APP: FLASK_APP,
-}
-
 
-def validate_server_requirements(ctx, param, value):
-    if value == "gevent":
-        try:
-            import gevent  # NOQA
-        except ImportError:
-            fatal_error("gevent library is not installed")
-    elif value == "tornado":
-        try:
-            import tornado  # NOQA
-        except ImportError:
-            fatal_error("tornado library is not installed")
-    else:
-        return value
+# app is defined globally so it can be passed as an import_string to `app.run`, which is needed
+# to enable reloading
+app = None
 
 
 def print_version(ctx, param, value):
     if not value or ctx.resilient_parsing:
         return
     click.echo(f"Connexion {importlib_metadata.version('connexion')}")
     ctx.exit()
 
 
-@click.group(cls=AliasedGroup, context_settings=CONTEXT_SETTINGS)
+@click.group(cls=AliasedGroup, context_settings={"help_option_names": ["-h", "--help"]})
 @click.option(
     "-V",
     "--version",
     is_flag=True,
     callback=print_version,
     expose_value=False,
     is_eager=True,
@@ -66,28 +49,16 @@
     pass
 
 
 @main.command()
 @click.argument("spec_file")
 @click.argument("base_module_path", required=False)
 @click.option("--port", "-p", default=5000, type=int, help="Port to listen.")
-@click.option("--host", "-H", type=str, help="Host interface to bind on.")
 @click.option(
-    "--wsgi-server",
-    "-w",
-    type=click.Choice(list(AVAILABLE_SERVERS)),
-    callback=validate_server_requirements,
-    help="Which WSGI server container to use. (deprecated, use --server instead)",
-)
-@click.option(
-    "--server",
-    "-s",
-    type=click.Choice(list(AVAILABLE_SERVERS)),
-    callback=validate_server_requirements,
-    help="Which server container to use.",
+    "--host", "-H", default="127.0.0.1", type=str, help="Host interface to bind on."
 )
 @click.option(
     "--stub",
     help="Returns status code 501, and `Not Implemented Yet` payload, for "
     "the endpoints which handlers are not found.",
     is_flag=True,
     default=False,
@@ -143,25 +114,23 @@
 @click.option("--verbose", "-v", help="Show verbose information.", count=True)
 @click.option(
     "--base-path", metavar="PATH", help="Override the basePath in the API spec."
 )
 @click.option(
     "--app-framework",
     "-f",
-    default=FLASK_APP,
+    default=ASYNC_APP,
     type=click.Choice(list(AVAILABLE_APPS)),
     help="The app framework used to run the server",
 )
 def run(
     spec_file,
     base_module_path,
     port,
     host,
-    wsgi_server,
-    server,
     stub,
     mock,
     hide_spec,
     hide_console_ui,
     console_ui_url,
     console_ui_from,
     auth_all_paths,
@@ -177,31 +146,14 @@
 
     Arguments:
 
     - SPEC_FILE: specification file that describes the server endpoints.
 
     - BASE_MODULE_PATH (optional): filesystem path where the API endpoints handlers are going to be imported from.
     """
-    if wsgi_server and server:
-        raise click.BadParameter(
-            "these options are mutually exclusive",
-            param_hint="'wsgi-server' and 'server'",
-        )
-    elif wsgi_server:
-        server = wsgi_server
-
-    if server is None:
-        server = DEFAULT_SERVERS[app_framework]
-
-    if app_framework not in AVAILABLE_SERVERS[server]:
-        message = "Invalid server '{}' for app-framework '{}'".format(
-            server, app_framework
-        )
-        raise click.UsageError(message)
-
     logging_level = logging.WARN
     if verbose > 0:
         logging_level = logging.INFO
 
     if debug or verbose > 1:
         logging_level = logging.DEBUG
         debug = True
@@ -220,30 +172,33 @@
     api_extra_args = {}
     if mock:
         resolver = MockResolver(mock_all=mock == "all")
         api_extra_args["resolver"] = resolver
 
     app_cls = connexion.utils.get_function_from_name(AVAILABLE_APPS[app_framework])
 
-    options = {
+    swagger_ui_options = {
         "serve_spec": not hide_spec,
         "swagger_path": console_ui_from or None,
         "swagger_ui": not hide_console_ui,
         "swagger_url": console_ui_url or None,
     }
 
-    app = app_cls(__name__, auth_all_paths=auth_all_paths, options=options)
+    global app
+    app = app_cls(
+        __name__, auth_all_paths=auth_all_paths, swagger_ui_options=swagger_ui_options
+    )
 
     app.add_api(
         spec_file_full_path,
         base_path=base_path,
         resolver_error=resolver_error,
         validate_responses=validate_responses,
         strict_validation=strict_validation,
         **api_extra_args,
     )
 
-    app.run(port=port, host=host, server=server, debug=debug)
+    app.run("connexion.cli:app", port=port, host=host, debug=debug)
 
 
 if __name__ == "__main__":  # pragma: no cover
     main()
```

### Comparing `connexion-3.0.0a4/connexion/context.py` & `connexion-3.0.0a5/connexion/context.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/datastructures.py` & `connexion-3.0.0a5/connexion/datastructures.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/decorators/main.py` & `connexion-3.0.0a5/connexion/decorators/main.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/decorators/parameter.py` & `connexion-3.0.0a5/connexion/decorators/parameter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """
 This module defines a decorator to convert request parameters to arguments for the view function.
 """
 import abc
 import asyncio
 import builtins
 import functools
-import inspect
 import keyword
 import logging
 import re
 import typing as t
 from copy import copy, deepcopy
 
 import inflection
 
 from connexion.context import context, operation
 from connexion.frameworks.abstract import Framework
 from connexion.http_facts import FORM_CONTENT_TYPES
 from connexion.lifecycle import ASGIRequest, WSGIRequest
 from connexion.operations import AbstractOperation, Swagger2Operation
-from connexion.utils import deep_merge, is_null, is_nullable, make_type
+from connexion.utils import (
+    deep_merge,
+    inspect_function_arguments,
+    is_null,
+    is_nullable,
+    make_type,
+)
 
 logger = logging.getLogger(__name__)
 
 CONTEXT_NAME = "context_"
 
 
 class BaseParameterDecorator:
@@ -152,29 +157,14 @@
 def unwrap_decorators(function: t.Callable) -> t.Callable:
     """Unwrap decorators to return the original function."""
     while hasattr(function, "__wrapped__"):
         function = function.__wrapped__  # type: ignore
     return function
 
 
-def inspect_function_arguments(function: t.Callable) -> t.Tuple[t.List[str], bool]:
-    """
-    Returns the list of variables names of a function and if it
-    accepts keyword arguments.
-    """
-    parameters = inspect.signature(function).parameters
-    bound_arguments = [
-        name
-        for name, p in parameters.items()
-        if p.kind not in (p.VAR_POSITIONAL, p.VAR_KEYWORD)
-    ]
-    has_kwargs = any(p.kind == p.VAR_KEYWORD for p in parameters.values())
-    return list(bound_arguments), has_kwargs
-
-
 def snake_and_shadow(name: str) -> str:
     """
     Converts the given name into Pythonic form. Firstly it converts CamelCase names to snake_case. Secondly it looks to
     see if the name matches a known built-in and if it does it appends an underscore to the name.
     :param name: The parameter name
     """
     snake = inflection.underscore(name)
```

### Comparing `connexion-3.0.0a4/connexion/decorators/response.py` & `connexion-3.0.0a5/connexion/decorators/response.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/exceptions.py` & `connexion-3.0.0a5/connexion/exceptions.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/frameworks/abstract.py` & `connexion-3.0.0a5/connexion/frameworks/abstract.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/frameworks/flask.py` & `connexion-3.0.0a5/connexion/frameworks/flask.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/frameworks/starlette.py` & `connexion-3.0.0a5/connexion/frameworks/starlette.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/handlers.py` & `connexion-3.0.0a5/connexion/handlers.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/json_schema.py` & `connexion-3.0.0a5/connexion/json_schema.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/jsonifier.py` & `connexion-3.0.0a5/connexion/jsonifier.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/lifecycle.py` & `connexion-3.0.0a5/connexion/lifecycle.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/middleware/abstract.py` & `connexion-3.0.0a5/connexion/middleware/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
     operations by operation_id at startup. At request time, the operation is fetched by an
     operation_id lookup.
     """
 
     api_cls: t.Type[API]
     """The subclass of RoutedAPI this middleware uses."""
 
-    def __init__(self, app: ASGIApp, **kwargs) -> None:
+    def __init__(self, app: ASGIApp) -> None:
         self.app = app
         self.apis: t.Dict[str, API] = {}
 
     def add_api(self, specification: t.Union[pathlib.Path, str, dict], **kwargs) -> API:
         api = self.api_cls(specification, next_app=self.app, **kwargs)
         self.apis[api.base_path] = api
         return api
```

### Comparing `connexion-3.0.0a4/connexion/middleware/context.py` & `connexion-3.0.0a5/connexion/middleware/context.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/middleware/exceptions.py` & `connexion-3.0.0a5/connexion/middleware/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 logger = logging.getLogger(__name__)
 
 
 class ExceptionMiddleware(StarletteExceptionMiddleware):
     """Subclass of starlette ExceptionMiddleware to change handling of HTTP exceptions to
     existing connexion behavior."""
 
-    def __init__(self, next_app: ASGIApp, *args, **kwargs):
+    def __init__(self, next_app: ASGIApp):
         super().__init__(next_app)
         self.add_exception_handler(ProblemException, self.problem_handler)
         self.add_exception_handler(Exception, self.common_error_handler)
 
     @staticmethod
     def problem_handler(_request: StarletteRequest, exc: ProblemException):
         logger.exception(exc)
```

### Comparing `connexion-3.0.0a4/connexion/middleware/lifespan.py` & `connexion-3.0.0a5/connexion/middleware/lifespan.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 
 class LifespanMiddleware:
     """
     Middleware that adds support for Starlette lifespan handlers
     (https://www.starlette.io/lifespan/).
     """
 
-    def __init__(
-        self, next_app: ASGIApp, *, lifespan: t.Optional[Lifespan], **kwargs
-    ) -> None:
+    def __init__(self, next_app: ASGIApp, *, lifespan: t.Optional[Lifespan]) -> None:
         self.next_app = next_app
         self._lifespan = lifespan
         # Leverage a Starlette Router for lifespan handling only
         self.router = Router(lifespan=lifespan)
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         # If no lifespan is registered, pass to next app so it can be handled downstream.
```

### Comparing `connexion-3.0.0a4/connexion/middleware/main.py` & `connexion-3.0.0a5/connexion/middleware/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import dataclasses
+import enum
 import logging
 import pathlib
 import typing as t
 from dataclasses import dataclass, field
+from functools import partial
 
 from starlette.types import ASGIApp, Receive, Scope, Send
 
 from connexion import utils
 from connexion.handlers import ResolverErrorHandler
 from connexion.jsonifier import Jsonifier
 from connexion.middleware.abstract import SpecMiddleware
@@ -16,14 +18,15 @@
 from connexion.middleware.request_validation import RequestValidationMiddleware
 from connexion.middleware.response_validation import ResponseValidationMiddleware
 from connexion.middleware.routing import RoutingMiddleware
 from connexion.middleware.security import SecurityMiddleware
 from connexion.middleware.swagger_ui import SwaggerUIMiddleware
 from connexion.resolver import Resolver
 from connexion.uri_parsing import AbstractURIParser
+from connexion.utils import inspect_function_arguments
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class _Options:
     """
@@ -47,14 +50,15 @@
     resolver_error: t.Optional[int] = None
     resolver_error_handler: t.Optional[t.Callable] = field(init=False)
     strict_validation: t.Optional[bool] = False
     swagger_ui_options: t.Optional[dict] = None
     uri_parser_class: t.Optional[AbstractURIParser] = None
     validate_responses: t.Optional[bool] = False
     validator_map: t.Optional[dict] = None
+    security_map: t.Optional[dict] = None
 
     def __post_init__(self):
         self.resolver = (
             Resolver(self.resolver) if callable(self.resolver) else self.resolver
         )
         self.resolver_error_handler = self._resolver_error_handler_factory()
 
@@ -77,48 +81,65 @@
 
         :return: An new _Options object with updated arguments.
         """
         changes = {key: value for key, value in changes.items() if value is not None}
         return dataclasses.replace(self, **changes)
 
 
+class MiddlewarePosition(enum.Enum):
+
+    BEFORE_SWAGGER = SwaggerUIMiddleware
+    BEFORE_ROUTING = RoutingMiddleware
+    BEFORE_SECURITY = SecurityMiddleware
+    BEFORE_VALIDATION = RequestValidationMiddleware
+    BEFORE_CONTEXT = ContextMiddleware
+
+
+class API:
+    def __init__(self, specification, *, base_path, **kwargs) -> None:
+        self.specification = specification
+        self.base_path = base_path
+        self.kwargs = kwargs
+
+
 class ConnexionMiddleware:
     """The main Connexion middleware, which wraps a list of specialized middlewares around the
     provided application."""
 
     default_middlewares = [
         ExceptionMiddleware,
         SwaggerUIMiddleware,
         RoutingMiddleware,
         SecurityMiddleware,
         RequestValidationMiddleware,
         ResponseValidationMiddleware,
-        ContextMiddleware,
         LifespanMiddleware,
+        ContextMiddleware,
     ]
 
     def __init__(
         self,
         app: ASGIApp,
         *,
         import_name: t.Optional[str] = None,
         lifespan: t.Optional[Lifespan] = None,
-        middlewares: t.Optional[list] = None,
+        middlewares: t.Optional[t.List[ASGIApp]] = None,
         specification_dir: t.Union[pathlib.Path, str] = "",
         arguments: t.Optional[dict] = None,
         auth_all_paths: t.Optional[bool] = None,
         jsonifier: t.Optional[Jsonifier] = None,
         pythonic_params: t.Optional[bool] = None,
         resolver: t.Optional[t.Union[Resolver, t.Callable]] = None,
         resolver_error: t.Optional[int] = None,
         strict_validation: t.Optional[bool] = None,
         swagger_ui_options: t.Optional[dict] = None,
         uri_parser_class: t.Optional[AbstractURIParser] = None,
         validate_responses: t.Optional[bool] = None,
         validator_map: t.Optional[dict] = None,
+        security_map: t.Optional[dict] = None,
     ):
         """
         :param import_name: The name of the package or module that this object belongs to. If you
             are using a single module, __name__ is always the correct value. If you however are
             using a package, it’s usually recommended to hardcode the name of your package there.
         :param middlewares: The list of middlewares to wrap around the application. Defaults to
             :obj:`middleware.main.ConnexionmMiddleware.default_middlewares`
@@ -141,68 +162,107 @@
         :param swagger_ui_options: A :class:`options.ConnexionOptions` instance with configuration
             options for the swagger ui.
         :param uri_parser_class: Class to use for uri parsing. See :mod:`uri_parsing`.
         :param validate_responses: Whether to validate responses against the specification. This has
             an impact on performance. Defaults to False.
         :param validator_map: A dictionary of validators to use. Defaults to
             :obj:`validators.VALIDATOR_MAP`.
+        :param security_map: A dictionary of security handlers to use. Defaults to
+            :obj:`security.SECURITY_HANDLERS`.
         """
         import_name = import_name or str(pathlib.Path.cwd())
         self.root_path = utils.get_root_path(import_name)
 
-        self.specification_dir = self.ensure_absolute(specification_dir)
+        spec_dir = pathlib.Path(specification_dir)
+        self.specification_dir = (
+            spec_dir if spec_dir.is_absolute() else self.root_path / spec_dir
+        )
 
-        if middlewares is None:
-            middlewares = self.default_middlewares
-        self.app, self.apps = self._apply_middlewares(
-            app, middlewares, lifespan=lifespan
+        self.app = app
+        self.lifespan = lifespan
+        self.middlewares = (
+            middlewares if middlewares is not None else self.default_middlewares
         )
+        self.middleware_stack: t.Optional[t.Iterable[ASGIApp]] = None
+        self.apis: t.List[API] = []
+        self.error_handlers: t.List[tuple] = []
 
         self.options = _Options(
             arguments=arguments,
             auth_all_paths=auth_all_paths,
             jsonifier=jsonifier,
             pythonic_params=pythonic_params,
             resolver=resolver,
             resolver_error=resolver_error,
             strict_validation=strict_validation,
             swagger_ui_options=swagger_ui_options,
             uri_parser_class=uri_parser_class,
             validate_responses=validate_responses,
             validator_map=validator_map,
+            security_map=security_map,
         )
 
         self.extra_files: t.List[str] = []
 
-    def ensure_absolute(self, path: t.Union[str, pathlib.Path]) -> pathlib.Path:
-        """Ensure that a path is absolute. If the path is not absolute, it is assumed to relative
-        to the application root path and made absolute."""
-        path = pathlib.Path(path)
-        if path.is_absolute():
-            return path
-        else:
-            return self.root_path / path
+    def add_middleware(
+        self,
+        middleware_class: t.Type[ASGIApp],
+        *,
+        position: MiddlewarePosition = MiddlewarePosition.BEFORE_CONTEXT,
+        **options: t.Any,
+    ) -> None:
+        """Add a middleware to the stack on the specified position.
 
-    def _apply_middlewares(
-        self, app: ASGIApp, middlewares: t.List[t.Type[ASGIApp]], **kwargs
-    ) -> t.Tuple[ASGIApp, t.Iterable[ASGIApp]]:
-        """Apply all middlewares to the provided app.
+        :param middleware_class: Middleware class to add
+        :param position: Position to add the middleware, one of the MiddlewarePosition Enum
+        :param options: Options to pass to the middleware_class on initialization
+        """
+        if self.middleware_stack is not None:
+            raise RuntimeError("Cannot add middleware after an application has started")
 
-        :param app: App to wrap in middlewares.
-        :param middlewares: List of middlewares to wrap around app. The list should be ordered
-                            from outer to inner middleware.
+        for m, middleware in enumerate(self.middlewares):
+            if isinstance(middleware, partial):
+                middleware = middleware.func
+
+            if middleware == position:
+                self.middlewares.insert(
+                    m, t.cast(ASGIApp, partial(middleware_class, **options))
+                )
+                break
+
+    def _build_middleware_stack(self) -> t.Tuple[ASGIApp, t.Iterable[ASGIApp]]:
+        """Apply all middlewares to the provided app.
 
         :return: Tuple of the outer middleware wrapping the application and a list of the wrapped
             middlewares, including the wrapped application.
         """
         # Include the wrapped application in the returned list.
+        app = self.app
         apps = [app]
-        for middleware in reversed(middlewares):
-            app = middleware(app, **kwargs)  # type: ignore
+        for middleware in reversed(self.middlewares):
+            arguments, _ = inspect_function_arguments(middleware)
+            if "lifespan" in arguments:
+                app = middleware(app, lifespan=self.lifespan)  # type: ignore
+            else:
+                app = middleware(app)  # type: ignore
             apps.append(app)
+
+        for app in apps:
+            if isinstance(app, SpecMiddleware):
+                for api in self.apis:
+                    app.add_api(
+                        api.specification,
+                        base_path=api.base_path,
+                        **api.kwargs,
+                    )
+
+            if isinstance(app, ExceptionMiddleware):
+                for error_handler in self.error_handlers:
+                    app.add_exception_handler(error_handler)
+
         return app, list(reversed(apps))
 
     def add_api(
         self,
         specification: t.Union[pathlib.Path, str, dict],
         *,
         base_path: t.Optional[str] = None,
@@ -213,16 +273,17 @@
         resolver: t.Optional[t.Union[Resolver, t.Callable]] = None,
         resolver_error: t.Optional[int] = None,
         strict_validation: t.Optional[bool] = None,
         swagger_ui_options: t.Optional[dict] = None,
         uri_parser_class: t.Optional[AbstractURIParser] = None,
         validate_responses: t.Optional[bool] = None,
         validator_map: t.Optional[dict] = None,
+        security_map: t.Optional[dict] = None,
         **kwargs,
-    ) -> t.Any:
+    ) -> None:
         """
         Register een API represented by a single OpenAPI specification on this middleware.
         Multiple APIs can be registered on a single middleware.
 
         :param specification: OpenAPI specification. Can be provided either as dict, or as path
             to file.
         :param base_path: Base path to host the API. This overrides the basePath / servers in the
@@ -243,20 +304,25 @@
         :param swagger_ui_options: A :class:`options.ConnexionOptions` instance with configuration
             options for the swagger ui.
         :param uri_parser_class: Class to use for uri parsing. See :mod:`uri_parsing`.
         :param validate_responses: Whether to validate responses against the specification. This has
             an impact on performance. Defaults to False.
         :param validator_map: A dictionary of validators to use. Defaults to
             :obj:`validators.VALIDATOR_MAP`
+        :param security_map: A dictionary of security handlers to use. Defaults to
+            :obj:`security.SECURITY_HANDLERS`
         :param kwargs: Additional keyword arguments to pass to the `add_api` method of the managed
             middlewares. This can be used to pass arguments to middlewares added beyond the default
             ones.
 
         :return: The Api registered on the wrapped application.
         """
+        if self.middleware_stack is not None:
+            raise RuntimeError("Cannot add api after an application has started")
+
         if isinstance(specification, dict):
             specification = specification
         else:
             specification = t.cast(pathlib.Path, self.specification_dir / specification)
             # Add specification as file to watch for reloading
             if pathlib.Path.cwd() in specification.parents:
                 self.extra_files.append(
@@ -271,34 +337,30 @@
             pythonic_params=pythonic_params,
             resolver=resolver,
             resolver_error=resolver_error,
             strict_validation=strict_validation,
             uri_parser_class=uri_parser_class,
             validate_responses=validate_responses,
             validator_map=validator_map,
+            security_map=security_map,
         )
 
-        for app in self.apps:
-            if isinstance(app, SpecMiddleware):
-                api = app.add_api(
-                    specification,
-                    base_path=base_path,
-                    **options.__dict__,
-                    **kwargs,
-                )
-
-        # Api registered on the inner application.
-        return api
+        api = API(specification, base_path=base_path, **options.__dict__, **kwargs)
+        self.apis.append(api)
 
     def add_error_handler(
         self, code_or_exception: t.Union[int, t.Type[Exception]], function: t.Callable
     ) -> None:
-        for app in self.apps:
-            if isinstance(app, ExceptionMiddleware):
-                app.add_exception_handler(code_or_exception, function)
+        if self.middleware_stack is not None:
+            raise RuntimeError(
+                "Cannot add error handler after an application has started"
+            )
+
+        error_handler = (code_or_exception, function)
+        self.error_handlers.append(error_handler)
 
     def run(self, import_string: str = None, **kwargs):
         """Run the application using uvicorn.
 
         :param import_string: application as import string (eg. "main:app"). This is needed to run
                               using reload.
         :param kwargs: kwargs to pass to `uvicorn.run`.
@@ -325,8 +387,10 @@
             )
         else:
             app = self
 
         uvicorn.run(app, **kwargs)
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
+        if self.middleware_stack is None:
+            self.app, self.middleware_stack = self._build_middleware_stack()
         await self.app(scope, receive, send)
```

### Comparing `connexion-3.0.0a4/connexion/middleware/request_validation.py` & `connexion-3.0.0a5/connexion/middleware/request_validation.py`

 * *Files 14% similar despite different names*

```diff
@@ -66,25 +66,49 @@
         )
         if mime_type.lower() not in media_type_dict:
             raise UnsupportedMediaTypeProblem(
                 detail=f"Invalid Content-type ({mime_type}), "
                 f"expected {self._operation.consumes}"
             )
 
+    @property
+    def security_query_params(self) -> t.List[str]:
+        """Get the names of query parameters that are used for security."""
+        if not hasattr(self, "_security_query_params"):
+            security_query_params: t.List[str] = []
+            if self._operation.security is None:
+                self._security_query_params = security_query_params
+                return self._security_query_params
+
+            for security_req in self._operation.security:
+                for scheme_name in security_req:
+                    security_scheme = self._operation.security_schemes[scheme_name]
+
+                    if (
+                        security_scheme["type"] == "apiKey"
+                        and security_scheme["in"] == "query"
+                    ):
+                        # Only query parameters need to be considered for strict_validation
+                        security_query_params.append(security_scheme["name"])
+            self._security_query_params = security_query_params
+
+        return self._security_query_params
+
     async def __call__(self, scope: Scope, receive: Receive, send: Send):
         # Validate parameters & headers
         uri_parser_class = self._operation._uri_parser_class
         uri_parser = uri_parser_class(
             self._operation.parameters, self._operation.body_definition()
         )
         parameter_validator_cls = self._validator_map["parameter"]
         parameter_validator = parameter_validator_cls(  # type: ignore
             self._operation.parameters,
             uri_parser=uri_parser,
             strict_validation=self.strict_validation,
+            security_query_params=self.security_query_params,
         )
         parameter_validator.validate(scope)
 
         # Extract content type
         headers = scope["headers"]
         mime_type, encoding = self.extract_content_type(headers)
         self.validate_mime_type(mime_type)
```

### Comparing `connexion-3.0.0a4/connexion/middleware/response_validation.py` & `connexion-3.0.0a5/connexion/middleware/response_validation.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/middleware/routing.py` & `connexion-3.0.0a5/connexion/middleware/routing.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     def _add_operation_internal(
         self, method: str, path: str, operation: RoutingOperation, name: str = None
     ) -> None:
         self.router.add_route(path, operation, methods=[method])
 
 
 class RoutingMiddleware(SpecMiddleware):
-    def __init__(self, app: ASGIApp, **kwargs) -> None:
+    def __init__(self, app: ASGIApp) -> None:
         """Middleware that resolves the Operation for an incoming request and attaches it to the
         scope.
 
         :param app: app to wrap in middleware.
         """
         self.app = app
         # Pass unknown routes to next app
```

### Comparing `connexion-3.0.0a4/connexion/middleware/swagger_ui.py` & `connexion-3.0.0a5/connexion/middleware/swagger_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
             status_code=200,
             media_type="application/json",
             content=json.dumps(self.options.openapi_console_ui_config),
         )
 
 
 class SwaggerUIMiddleware(SpecMiddleware):
-    def __init__(self, app: ASGIApp, **kwargs) -> None:
+    def __init__(self, app: ASGIApp) -> None:
         """Middleware that hosts a swagger UI.
 
         :param app: app to wrap in middleware.
         """
         self.app = app
         # Set default to pass unknown routes to next app
         self.router = Router(default=self.default_fn)
```

### Comparing `connexion-3.0.0a4/connexion/mock.py` & `connexion-3.0.0a5/connexion/mock.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/operations/__init__.py` & `connexion-3.0.0a5/connexion/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/operations/abstract.py` & `connexion-3.0.0a5/connexion/operations/abstract.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/operations/openapi.py` & `connexion-3.0.0a5/connexion/operations/openapi.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/operations/swagger2.py` & `connexion-3.0.0a5/connexion/operations/swagger2.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/options.py` & `connexion-3.0.0a5/connexion/options.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/problem.py` & `connexion-3.0.0a5/connexion/problem.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/resolver.py` & `connexion-3.0.0a5/connexion/resolver.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/resources/schemas/v2.0/schema.json` & `connexion-3.0.0a5/connexion/resources/schemas/v2.0/schema.json`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/resources/schemas/v3.0/schema.json` & `connexion-3.0.0a5/connexion/resources/schemas/v3.0/schema.json`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/security.py` & `connexion-3.0.0a5/connexion/security.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,318 @@
 """
-This module defines an abstract SecurityHandlerFactory which supports the creation of security
-handlers for operations.
+This module defines a SecurityHandlerFactory which supports the creation of
+SecurityHandler instances for different security schemes.
+
+It also exposes a `SECURITY_HANDLERS` dictionary which maps security scheme
+types to SecurityHandler classes. This dictionary can be used to register
+custom SecurityHandler classes for custom security schemes, or to overwrite
+existing SecurityHandler classes.
+This can be done by supplying a value for `security_map` argument of the
+SecurityHandlerFactory.
+
+Swagger 2.0 lets you define the following authentication types for an API:
+
+- Basic authentication
+- API key (as a header or a query string parameter)
+- OAuth 2 common flows (authorization code, implicit, resource owner password credentials, client credentials)
+
+
+Changes from OpenAPI 2.0 to OpenAPI 3.0
+If you used OpenAPI 2.0 before, here is a summary of changes to help you get started with OpenAPI 3.0:
+- securityDefinitions were renamed to securitySchemes and moved inside components.
+- type: basic was replaced with type: http and scheme: basic.
+- The new type: http is an umbrella type for all HTTP security schemes, including Basic, Bearer and other,
+and the scheme keyword indicates the scheme type.
+- API keys can now be sent in: cookie.
+- Added support for OpenID Connect Discovery (type: openIdConnect).
+- OAuth 2 security schemes can now define multiple flows.
+- OAuth 2 flows were renamed to match the OAuth 2 Specification: accessCode is now authorizationCode,
+and application is now clientCredentials.
+
+
+OpenAPI uses the term security scheme for authentication and authorization schemes.
+OpenAPI 3.0 lets you describe APIs protected using the following security schemes:
+
+- HTTP authentication schemes (they use the Authorization header):
+    - Basic
+    - Bearer
+    - other HTTP schemes as defined by RFC 7235 and HTTP Authentication Scheme Registry
+- API keys in headers, query string or cookies
+    - Cookie authentication
+- OAuth 2
+- OpenID Connect Discovery
+
 """
 
 import asyncio
 import base64
 import http.cookies
 import logging
 import os
-import textwrap
 import typing as t
 
 import httpx
 
 from connexion.decorators.parameter import inspect_function_arguments
-from connexion.exceptions import (
-    ConnexionException,
-    OAuthProblem,
-    OAuthResponseProblem,
-    OAuthScopeProblem,
-)
+from connexion.exceptions import OAuthProblem, OAuthResponseProblem, OAuthScopeProblem
+from connexion.lifecycle import ASGIRequest
 from connexion.utils import get_function_from_name
 
-logger = logging.getLogger("connexion.api.security")
-
+logger = logging.getLogger(__name__)
 
-class SecurityHandlerFactory:
-    """
-    get_*_func -> _get_function -> get_function_from_name (name=security function defined in spec)
-        (if url defined instead of a function -> get_token_info_remote)
 
-    std security functions: security_{passthrough,deny}
+NO_VALUE = object()
+"""Sentinel value to indicate that no security credentials were found."""
 
-    verify_* -> returns a security wrapper around the security function
-        check_* -> returns a function tasked with doing auth for use inside the verify wrapper
-            check helpers (used outside wrappers): _need_to_add_context_or_scopes
-            the security function
 
-        verify helpers (used inside wrappers): get_auth_header_value, get_cookie_value
-    """
+class AbstractSecurityHandler:
 
-    no_value = object()
     required_scopes_kw = "required_scopes"
-    context_kw = "context_"
     client = None
+    security_definition_key: str
+    """The key which contains the value for the function name to resolve."""
+    environ_key: str
+    """The name of the environment variable that can be used alternatively for the function name."""
+
+    def get_fn(self, security_scheme, required_scopes):
+        """Returns the handler function"""
+        security_func = self._resolve_func(security_scheme)
+        if not security_func:
+            logger.warning("... %s missing", self.security_definition_key)
+            return None
 
-    @staticmethod
+        return self._get_verify_func(security_func)
+
+    @classmethod
     def _get_function(
-        security_definition, security_definition_key, environ_key, default=None
+        cls,
+        security_definition: dict,
+        security_definition_key: str,
+        environ_key: str,
+        default: t.Optional[t.Callable] = None,
     ):
         """
         Return function by getting its name from security_definition or environment variable
+
+        :param security_definition: Security Definition (scheme) from the spec.
+        :param security_definition_key: The key which contains the value for the function name to resolve.
+        :param environ_key: The name of the environment variable that can be used alternatively for the function name.
+        :param default: The default to use in case the function cannot be found based on the security_definition_key or the environ_key
         """
-        func = security_definition.get(security_definition_key) or os.environ.get(
+        func_name = security_definition.get(security_definition_key) or os.environ.get(
             environ_key
         )
-        if func:
-            return get_function_from_name(func)
+        if func_name:
+            return get_function_from_name(func_name)
         return default
 
+    def _generic_check(self, func, exception_msg):
+        need_to_add_required_scopes = self._need_to_add_scopes(func)
+
+        async def wrapper(request, *args, required_scopes=None):
+            kwargs = {}
+            if need_to_add_required_scopes:
+                kwargs[self.required_scopes_kw] = required_scopes
+            token_info = func(*args, **kwargs)
+            while asyncio.iscoroutine(token_info):
+                token_info = await token_info
+            if token_info is NO_VALUE:
+                return NO_VALUE
+            if token_info is None:
+                raise OAuthResponseProblem(detail=exception_msg)
+            return token_info
+
+        return wrapper
+
+    @staticmethod
+    def get_auth_header_value(request):
+        """
+        Return Authorization type and value if any.
+        If not Authorization, return (None, None)
+        Raise OAuthProblem for invalid Authorization header
+        """
+        authorization = request.headers.get("Authorization")
+        if not authorization:
+            return None, None
+
+        try:
+            auth_type, value = authorization.split(maxsplit=1)
+        except ValueError:
+            raise OAuthProblem(detail="Invalid authorization header")
+        return auth_type.lower(), value
+
+    def _need_to_add_scopes(self, func):
+        arguments, has_kwargs = inspect_function_arguments(func)
+        need_required_scopes = has_kwargs or self.required_scopes_kw in arguments
+        return need_required_scopes
+
+    def _resolve_func(self, security_scheme):
+        """
+        Get the user function object based on the security scheme or the environment variable.
+
+        :param security_scheme: Security Definition (scheme) from the spec.
+        """
+        return self._get_function(
+            security_scheme, self.security_definition_key, self.environ_key
+        )
+
+    def _get_verify_func(self, function):
+        """
+        Wraps the user security function in a function that checks the request for the correct
+        security credentials and calls the user function with the correct arguments.
+        """
+        return self._generic_check(function, "Provided authorization is not valid")
+
+
+class BasicSecurityHandler(AbstractSecurityHandler):
+    """
+    Security Handler for
+    - `type: basic` (Swagger 2), and
+    - `type: http` and `scheme: basic` (OpenAPI 3)
+    """
+
+    security_definition_key = "x-basicInfoFunc"
+    environ_key = "BASICINFO_FUNC"
+
+    def _get_verify_func(self, basic_info_func):
+        check_basic_info_func = self.check_basic_auth(basic_info_func)
+
+        def wrapper(request):
+            auth_type, user_pass = self.get_auth_header_value(request)
+            if auth_type != "basic":
+                return NO_VALUE
+
+            try:
+                username, password = (
+                    base64.b64decode(user_pass).decode("latin1").split(":", 1)
+                )
+            except Exception:
+                raise OAuthProblem(detail="Invalid authorization header")
+
+            return check_basic_info_func(request, username, password)
+
+        return wrapper
+
+    def check_basic_auth(self, basic_info_func):
+        return self._generic_check(
+            basic_info_func, "Provided authorization is not valid"
+        )
+
+
+class BearerSecurityHandler(AbstractSecurityHandler):
+    """
+    Security Handler for HTTP Bearer authentication.
+    """
+
+    security_definition_key = "x-bearerInfoFunc"
+    environ_key = "BEARERINFO_FUNC"
+
+    def check_bearer_token(self, token_info_func):
+        return self._generic_check(token_info_func, "Provided token is not valid")
+
+    def _get_verify_func(self, token_info_func):
+        """
+        :param token_info_func: types.FunctionType
+        :rtype: types.FunctionType
+        """
+        check_bearer_func = self.check_bearer_token(token_info_func)
+
+        def wrapper(request):
+            auth_type, token = self.get_auth_header_value(request)
+            if auth_type != "bearer":
+                return NO_VALUE
+            return check_bearer_func(request, token)
+
+        return wrapper
+
+
+class ApiKeySecurityHandler(AbstractSecurityHandler):
+    """
+    Security Handler for API Keys.
+    """
+
+    security_definition_key = "x-apikeyInfoFunc"
+    environ_key = "APIKEYINFO_FUNC"
+
+    def get_fn(self, security_scheme, required_scopes):
+        apikey_info_func = self._resolve_func(security_scheme)
+        if not apikey_info_func:
+            logger.warning("... %s missing", self.security_definition_key)
+            return None
+
+        return self._get_verify_func(
+            apikey_info_func,
+            security_scheme["in"],
+            security_scheme["name"],
+        )
+
+    def _get_verify_func(self, api_key_info_func, loc, name):
+        check_api_key_func = self.check_api_key(api_key_info_func)
+
+        def wrapper(request: ASGIRequest):
+            if loc == "query":
+                api_key = request.query_params.get(name)
+            elif loc == "header":
+                api_key = request.headers.get(name)
+            elif loc == "cookie":
+                cookie_list = request.headers.get("Cookie")
+                api_key = self.get_cookie_value(cookie_list, name)
+            else:
+                return NO_VALUE
+
+            if api_key is None:
+                return NO_VALUE
+
+            return check_api_key_func(request, api_key)
+
+        return wrapper
+
+    def check_api_key(self, api_key_info_func):
+        return self._generic_check(api_key_info_func, "Provided apikey is not valid")
+
+    @staticmethod
+    def get_cookie_value(cookies, name):
+        """
+        Returns cookie value by its name. `None` if no such value.
+
+        :param cookies: str: cookies raw data
+        :param name: str: cookies key
+        """
+        cookie_parser = http.cookies.SimpleCookie()
+        cookie_parser.load(str(cookies))
+        try:
+            return cookie_parser[name].value
+        except KeyError:
+            return None
+
+
+class OAuthSecurityHandler(AbstractSecurityHandler):
+    """
+    Security Handler for the OAuth security scheme.
+    """
+
+    def get_fn(self, security_scheme, required_scopes):
+        token_info_func = self.get_tokeninfo_func(security_scheme)
+        scope_validate_func = self.get_scope_validate_func(security_scheme)
+        if not token_info_func:
+            logger.warning("... x-tokenInfoFunc missing")
+            return None
+
+        return self._get_verify_func(
+            token_info_func, scope_validate_func, required_scopes
+        )
+
     def get_tokeninfo_func(self, security_definition: dict) -> t.Optional[t.Callable]:
         """
-        :type security_definition: dict
+        Gets the function for retrieving the token info.
+        It is possible to specify a function or a URL. The function variant is
+        preferred. If it is not found, the URL variant is used with the
+        `get_token_info_remote` function.
 
-        >>> get_tokeninfo_url({'x-tokenInfoFunc': 'foo.bar'})
+        >>> get_tokeninfo_func({'x-tokenInfoFunc': 'foo.bar'})
         '<function foo.bar>'
         """
         token_info_func = self._get_function(
             security_definition, "x-tokenInfoFunc", "TOKENINFO_FUNC"
         )
         if token_info_func:
             return token_info_func
@@ -79,82 +324,27 @@
             return self.get_token_info_remote(token_info_url)
 
         return None
 
     @classmethod
     def get_scope_validate_func(cls, security_definition):
         """
-        :type security_definition: dict
-        :rtype: function
+        Gets the function for validating the token scopes.
+        If it is not found, the default `validate_scope` function is used.
 
         >>> get_scope_validate_func({'x-scopeValidateFunc': 'foo.bar'})
         '<function foo.bar>'
         """
         return cls._get_function(
             security_definition,
             "x-scopeValidateFunc",
             "SCOPEVALIDATE_FUNC",
             cls.validate_scope,
         )
 
-    @classmethod
-    def get_basicinfo_func(cls, security_definition):
-        """
-        :type security_definition: dict
-        :rtype: function
-
-        >>> get_basicinfo_func({'x-basicInfoFunc': 'foo.bar'})
-        '<function foo.bar>'
-        """
-        return cls._get_function(
-            security_definition, "x-basicInfoFunc", "BASICINFO_FUNC"
-        )
-
-    @classmethod
-    def get_apikeyinfo_func(cls, security_definition):
-        """
-        :type security_definition: dict
-        :rtype: function
-
-        >>> get_apikeyinfo_func({'x-apikeyInfoFunc': 'foo.bar'})
-        '<function foo.bar>'
-        """
-        return cls._get_function(
-            security_definition, "x-apikeyInfoFunc", "APIKEYINFO_FUNC"
-        )
-
-    @classmethod
-    def get_bearerinfo_func(cls, security_definition):
-        """
-        :type security_definition: dict
-        :rtype: function
-
-        >>> get_bearerinfo_func({'x-bearerInfoFunc': 'foo.bar'})
-        '<function foo.bar>'
-        """
-        return cls._get_function(
-            security_definition, "x-bearerInfoFunc", "BEARERINFO_FUNC"
-        )
-
-    @staticmethod
-    async def security_passthrough(request):
-        return request
-
-    @staticmethod
-    def security_deny(function):
-        """
-        :type function: types.FunctionType
-        :rtype: types.FunctionType
-        """
-
-        def deny(*args, **kwargs):
-            raise ConnexionException("Error in security definitions")
-
-        return deny
-
     @staticmethod
     def validate_scope(required_scopes, token_scopes):
         """
         :param required_scopes: Scopes required to access operation
         :param token_scopes: Scopes granted by authorization server
         :rtype: bool
         """
@@ -163,142 +353,182 @@
             token_scopes = set(token_scopes)
         else:
             token_scopes = set(token_scopes.split())
         logger.debug("... Scopes required: %s", required_scopes)
         logger.debug("... Token scopes: %s", token_scopes)
         if not required_scopes <= token_scopes:
             logger.info(
-                textwrap.dedent(
-                    """
-                        ... Token scopes (%s) do not match the scopes necessary to call endpoint (%s).
-                         Aborting with 403."""
-                ).replace("\n", ""),
+                "... Token scopes (%s) do not match the scopes necessary to call endpoint (%s)."
+                " Aborting with 403.",
                 token_scopes,
                 required_scopes,
             )
             return False
         return True
 
-    @staticmethod
-    def get_auth_header_value(request):
+    def get_token_info_remote(self, token_info_url: str) -> t.Callable:
         """
-        Called inside security wrapper functions
+        Return a function which will call `token_info_url` to retrieve token info.
 
-        Return Authorization type and value if any.
-        If not Authorization, return (None, None)
-        Raise OAuthProblem for invalid Authorization header
+        Returned function must accept oauth token in parameter.
+        It must return a token_info dict in case of success, None otherwise.
+
+        :param token_info_url: URL to get information about the token
         """
-        authorization = request.headers.get("Authorization")
-        if not authorization:
-            return None, None
 
-        try:
-            auth_type, value = authorization.split(None, 1)
-        except ValueError:
-            raise OAuthProblem(detail="Invalid authorization header")
-        return auth_type.lower(), value
+        async def wrapper(token):
+            if self.client is None:
+                self.client = httpx.AsyncClient()
+            headers = {"Authorization": f"Bearer {token}"}
+            token_request = await self.client.get(
+                token_info_url, headers=headers, timeout=5
+            )
+            if token_request.status_code != 200:
+                return
+            return token_request.json()
+
+        return wrapper
 
-    def verify_oauth(self, token_info_func, scope_validate_func, required_scopes):
+    def _get_verify_func(self, token_info_func, scope_validate_func, required_scopes):
         check_oauth_func = self.check_oauth_func(token_info_func, scope_validate_func)
 
         def wrapper(request):
             auth_type, token = self.get_auth_header_value(request)
             if auth_type != "bearer":
-                return self.no_value
+                return NO_VALUE
 
             return check_oauth_func(request, token, required_scopes=required_scopes)
 
         return wrapper
 
-    def verify_basic(self, basic_info_func):
-        check_basic_info_func = self.check_basic_auth(basic_info_func)
+    def check_oauth_func(self, token_info_func, scope_validate_func):
+        get_token_info = self._generic_check(
+            token_info_func, "Provided token is not valid"
+        )
 
-        def wrapper(request):
-            auth_type, user_pass = self.get_auth_header_value(request)
-            if auth_type != "basic":
-                return self.no_value
+        async def wrapper(request, token, required_scopes):
+            token_info = await get_token_info(
+                request, token, required_scopes=required_scopes
+            )
 
-            try:
-                username, password = (
-                    base64.b64decode(user_pass).decode("latin1").split(":", 1)
+            # Fallback to 'scopes' for backward compatibility
+            token_scopes = token_info.get("scope", token_info.get("scopes", ""))
+
+            validation = scope_validate_func(required_scopes, token_scopes)
+            while asyncio.iscoroutine(validation):
+                validation = await validation
+            if not validation:
+                raise OAuthScopeProblem(
+                    required_scopes=required_scopes,
+                    token_scopes=token_scopes,
                 )
-            except Exception:
-                raise OAuthProblem(detail="Invalid authorization header")
 
-            return check_basic_info_func(request, username, password)
+            return token_info
 
         return wrapper
 
-    @staticmethod
-    def get_cookie_value(cookies, name):
-        """
-        Called inside security wrapper functions
 
-        Returns cookie value by its name. None if no such value.
-        :param cookies: str: cookies raw data
-        :param name: str: cookies key
-        """
-        cookie_parser = http.cookies.SimpleCookie()
-        cookie_parser.load(str(cookies))
-        try:
-            return cookie_parser[name].value
-        except KeyError:
-            return None
+SECURITY_HANDLERS = {
+    # Swagger 2: `type: basic`
+    # OpenAPI 3: `type: http` and `scheme: basic`
+    "basic": BasicSecurityHandler,
+    # Swagger 2 and OpenAPI 3
+    "apiKey": ApiKeySecurityHandler,
+    "oauth2": OAuthSecurityHandler,
+    # OpenAPI 3: http schemes
+    "bearer": BearerSecurityHandler,
+}
 
-    def verify_api_key(self, api_key_info_func, loc, name):
-        check_api_key_func = self.check_api_key(api_key_info_func)
 
-        def wrapper(request):
-            def _immutable_pop(_dict, key):
-                """
-                Pops the key from an immutable dict and returns the value that was popped,
-                and a new immutable dict without the popped key.
-                """
-                cls = type(_dict)
-                try:
-                    _dict = _dict.to_dict(flat=False)
-                    return _dict.pop(key)[0], cls(_dict)
-                except AttributeError:
-                    _dict = dict(_dict.items())
-                    return _dict.pop(key), cls(_dict)
+class SecurityHandlerFactory:
+    """
+    A factory class for parsing security schemes and returning the appropriate
+    security handler.
 
-            if loc == "query":
-                try:
-                    api_key, request.query = _immutable_pop(request.query, name)
-                except KeyError:
-                    api_key = None
-            elif loc == "header":
-                api_key = request.headers.get(name)
-            elif loc == "cookie":
-                cookie_list = request.headers.get("Cookie")
-                api_key = self.get_cookie_value(cookie_list, name)
+    By default, it will use the built-in security handlers specified in the
+    SECURITY_HANDLERS dict, but you can also pass in your own security handlers
+    to override the built-in ones.
+    """
+
+    def __init__(
+        self,
+        security_handlers: t.Optional[dict] = None,
+    ) -> None:
+        self.security_handlers = SECURITY_HANDLERS.copy()
+        if security_handlers is not None:
+            self.security_handlers.update(security_handlers)
+
+    def parse_security_scheme(
+        self,
+        security_scheme: dict,
+        required_scopes: t.List[str],
+    ) -> t.Optional[t.Callable]:
+        """Parses the security scheme and returns the function for verifying it.
+
+        :param security_scheme: The security scheme from the spec.
+        :param required_scopes: List of scopes for this security scheme.
+        """
+        security_type = security_scheme["type"]
+        if security_type in ("basic", "oauth2"):
+            security_handler = self.security_handlers[security_type]
+            return security_handler().get_fn(security_scheme, required_scopes)
+
+        # OpenAPI 3.0.0
+        elif security_type == "http":
+            scheme = security_scheme["scheme"].lower()
+            if scheme in self.security_handlers:
+                security_handler = self.security_handlers[scheme]
+                return security_handler().get_fn(security_scheme, required_scopes)
             else:
-                return self.no_value
+                logger.warning("... Unsupported http authorization scheme %s", scheme)
+                return None
 
-            if api_key is None:
-                return self.no_value
+        elif security_type == "apiKey":
+            scheme = security_scheme.get("x-authentication-scheme", "").lower()
+            if scheme == "bearer":
+                return BearerSecurityHandler().get_fn(security_scheme, required_scopes)
+            else:
+                security_handler = self.security_handlers["apiKey"]
+                return security_handler().get_fn(security_scheme, required_scopes)
 
-            return check_api_key_func(request, api_key)
+        else:
+            logger.warning(
+                "... Unsupported security scheme type %s",
+                security_type,
+            )
+            return None
 
-        return wrapper
+    @staticmethod
+    async def security_passthrough(request):
+        """Used when no security is required for the operation.
 
-    def verify_bearer(self, token_info_func):
-        """
-        :param token_info_func: types.FunctionType
-        :rtype: types.FunctionType
+        Equivalent OpenAPI snippet:
+
+        .. code-block:: yaml
+
+            /helloworld
+              get:
+                security: []   # No security
+                ...
         """
-        check_bearer_func = self.check_bearer_token(token_info_func)
+        return request
 
-        def wrapper(request):
-            auth_type, token = self.get_auth_header_value(request)
-            if auth_type != "bearer":
-                return self.no_value
-            return check_bearer_func(request, token)
+    @staticmethod
+    def verify_none(request):
+        """Used for optional security.
 
-        return wrapper
+        Equivalent OpenAPI snippet:
+
+        .. code-block:: yaml
+
+            security:
+              - {}  # <--
+              - myapikey: []
+        """
+        return {}
 
     def verify_multiple_schemes(self, schemes):
         """
         Verifies multiple authentication schemes in AND fashion.
         If any scheme fails, the entire authentication fails.
 
         :param schemes: mapping scheme_name to auth function
@@ -308,116 +538,33 @@
 
         async def wrapper(request):
             token_info = {}
             for scheme_name, func in schemes.items():
                 result = func(request)
                 while asyncio.iscoroutine(result):
                     result = await result
-                if result is self.no_value:
-                    return self.no_value
+                if result is NO_VALUE:
+                    return NO_VALUE
                 token_info[scheme_name] = result
 
             return token_info
 
         return wrapper
 
-    @staticmethod
-    def verify_none():
-        """
-        :rtype: types.FunctionType
-        """
-
-        def wrapper(request):
-            return {}
-
-        return wrapper
-
-    def _need_to_add_context_or_scopes(self, func):
-        arguments, has_kwargs = inspect_function_arguments(func)
-        need_context = self.context_kw in arguments
-        need_required_scopes = has_kwargs or self.required_scopes_kw in arguments
-        return need_context, need_required_scopes
-
-    def _generic_check(self, func, exception_msg):
-        (
-            need_to_add_context,
-            need_to_add_required_scopes,
-        ) = self._need_to_add_context_or_scopes(func)
-
-        async def wrapper(request, *args, required_scopes=None):
-            kwargs = {}
-            if need_to_add_context:
-                kwargs[self.context_kw] = request.context
-            if need_to_add_required_scopes:
-                kwargs[self.required_scopes_kw] = required_scopes
-            token_info = func(*args, **kwargs)
-            while asyncio.iscoroutine(token_info):
-                token_info = await token_info
-            if token_info is self.no_value:
-                return self.no_value
-            if token_info is None:
-                raise OAuthResponseProblem(detail=exception_msg)
-            return token_info
-
-        return wrapper
-
-    def check_bearer_token(self, token_info_func):
-        return self._generic_check(token_info_func, "Provided token is not valid")
-
-    def check_basic_auth(self, basic_info_func):
-        return self._generic_check(
-            basic_info_func, "Provided authorization is not valid"
-        )
-
-    def check_api_key(self, api_key_info_func):
-        return self._generic_check(api_key_info_func, "Provided apikey is not valid")
-
-    def check_oauth_func(self, token_info_func, scope_validate_func):
-        get_token_info = self._generic_check(
-            token_info_func, "Provided token is not valid"
-        )
-        need_to_add_context, _ = self._need_to_add_context_or_scopes(
-            scope_validate_func
-        )
-
-        async def wrapper(request, token, required_scopes):
-            token_info = await get_token_info(
-                request, token, required_scopes=required_scopes
-            )
-
-            # Fallback to 'scopes' for backward compatibility
-            token_scopes = token_info.get("scope", token_info.get("scopes", ""))
-
-            kwargs = {}
-            if need_to_add_context:
-                kwargs[self.context_kw] = request.context
-            validation = scope_validate_func(required_scopes, token_scopes, **kwargs)
-            while asyncio.iscoroutine(validation):
-                validation = await validation
-            if not validation:
-                raise OAuthScopeProblem(
-                    required_scopes=required_scopes,
-                    token_scopes=token_scopes,
-                )
-
-            return token_info
-
-        return wrapper
-
     @classmethod
     def verify_security(cls, auth_funcs):
         async def verify_fn(request):
-            token_info = cls.no_value
+            token_info = NO_VALUE
             errors = []
             for func in auth_funcs:
                 try:
                     token_info = func(request)
                     while asyncio.iscoroutine(token_info):
                         token_info = await token_info
-                    if token_info is not cls.no_value:
+                    if token_info is not NO_VALUE:
                         break
                 except Exception as err:
                     errors.append(err)
 
             else:
                 if errors != []:
                     cls._raise_most_specific(errors)
@@ -461,32 +608,7 @@
         if 403 in status_to_exc:
             raise status_to_exc[403]
         elif 401 in status_to_exc:
             raise status_to_exc[401]
         else:
             lowest_status_code = min(status_to_exc)
             raise status_to_exc[lowest_status_code]
-
-    def get_token_info_remote(self, token_info_url):
-        """
-        Return a function which will call `token_info_url` to retrieve token info.
-
-        Returned function must accept oauth token in parameter.
-        It must return a token_info dict in case of success, None otherwise.
-
-        :param token_info_url: Url to get information about the token
-        :type token_info_url: str
-        :rtype: types.FunctionType
-        """
-
-        async def wrapper(token):
-            if self.client is None:
-                self.client = httpx.AsyncClient()
-            headers = {"Authorization": f"Bearer {token}"}
-            token_request = await self.client.get(
-                token_info_url, headers=headers, timeout=5
-            )
-            if token_request.status_code != 200:
-                return
-            return token_request.json()
-
-        return wrapper
```

### Comparing `connexion-3.0.0a4/connexion/spec.py` & `connexion-3.0.0a5/connexion/spec.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/testing.py` & `connexion-3.0.0a5/connexion/testing.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/uri_parsing.py` & `connexion-3.0.0a5/connexion/uri_parsing.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/utils.py` & `connexion-3.0.0a5/connexion/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module provides general utility functions used within Connexion.
 """
 
 import asyncio
 import functools
 import importlib
+import inspect
 import os
 import pkgutil
 import sys
 import typing as t
 
 import yaml
 
@@ -403,7 +404,22 @@
                 " name information or because it's a namespace package."
                 " In this case the root path needs to be explicitly"
                 " provided."
             )
 
     # filepath is import_name.py for a module, or __init__.py for a package.
     return os.path.dirname(os.path.abspath(filepath))
+
+
+def inspect_function_arguments(function: t.Callable) -> t.Tuple[t.List[str], bool]:
+    """
+    Returns the list of variables names of a function and if it
+    accepts keyword arguments.
+    """
+    parameters = inspect.signature(function).parameters
+    bound_arguments = [
+        name
+        for name, p in parameters.items()
+        if p.kind not in (p.VAR_POSITIONAL, p.VAR_KEYWORD)
+    ]
+    has_kwargs = any(p.kind == p.VAR_KEYWORD for p in parameters.values())
+    return list(bound_arguments), has_kwargs
```

### Comparing `connexion-3.0.0a4/connexion/validators/__init__.py` & `connexion-3.0.0a5/connexion/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/validators/abstract.py` & `connexion-3.0.0a5/connexion/validators/abstract.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/validators/form_data.py` & `connexion-3.0.0a5/connexion/validators/form_data.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/validators/json.py` & `connexion-3.0.0a5/connexion/validators/json.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a4/connexion/validators/parameter.py` & `connexion-3.0.0a5/connexion/validators/parameter.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,26 +15,36 @@
 try:
     draft4_format_checker = Draft4Validator.FORMAT_CHECKER  # type: ignore
 except AttributeError:  # jsonschema < 4.5.0
     from jsonschema import draft4_format_checker
 
 
 class ParameterValidator:
-    def __init__(self, parameters, uri_parser, strict_validation=False):
+    def __init__(
+        self,
+        parameters,
+        uri_parser,
+        strict_validation=False,
+        security_query_params=None,
+    ):
         """
         :param parameters: List of request parameter dictionaries
         :param uri_parser: class to use for uri parsing
         :param strict_validation: Flag indicating if parameters not in spec are allowed
+        :param security_query_params: List of query parameter names used for security.
+            These parameters will be ignored when checking for extra parameters in case of
+            strict validation.
         """
         self.parameters = collections.defaultdict(list)
         for p in parameters:
             self.parameters[p["in"]].append(p)
 
         self.uri_parser = uri_parser
         self.strict_validation = strict_validation
+        self.security_query_params = set(security_query_params or [])
 
     @staticmethod
     def validate_parameter(parameter_type, value, param, param_name=None):
         if is_nullable(param) and is_null(value):
             return
 
         elif value is not None:
@@ -55,17 +65,18 @@
     @staticmethod
     def validate_parameter_list(request_params, spec_params):
         request_params = set(request_params)
         spec_params = set(spec_params)
 
         return request_params.difference(spec_params)
 
-    def validate_query_parameter_list(self, request):
+    def validate_query_parameter_list(self, request, security_params=None):
         request_params = request.query_params.keys()
         spec_params = [x["name"] for x in self.parameters.get("query", [])]
+        spec_params.extend(security_params or [])
         return self.validate_parameter_list(request_params, spec_params)
 
     def validate_query_parameter(self, param, request):
         """
         Validate a single query parameter (request.args in Flask)
 
         :type param: dict
@@ -95,17 +106,18 @@
     def validate(self, scope):
         logger.debug("%s validating parameters...", scope.get("path"))
 
         request = Request(scope)
         self.validate_request(request)
 
     def validate_request(self, request):
-
         if self.strict_validation:
-            query_errors = self.validate_query_parameter_list(request)
+            query_errors = self.validate_query_parameter_list(
+                request, security_params=self.security_query_params
+            )
 
             if query_errors:
                 raise ExtraParameterProblem(
                     param_type="query", extra_params=query_errors
                 )
 
         for param in self.parameters.get("query", []):
```

### Comparing `connexion-3.0.0a4/pyproject.toml` & `connexion-3.0.0a5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connexion"
-version = '3.0.0a4'
+version = '3.0.0a5'
 description = "Connexion - API first applications with OpenAPI/Swagger"
 readme = "README.rst"
 keywords = ["api", "swagger", "openapi"]
 license = "Apache-2.0"
 authors = [
     "Daniel Grossmann-Kavanagh <me@danielgk.com>",
     "Henning Jacobs <henning.jacobs@zalando.de>",
```

### Comparing `connexion-3.0.0a4/PKG-INFO` & `connexion-3.0.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connexion
-Version: 3.0.0a4
+Version: 3.0.0a5
 Summary: Connexion - API first applications with OpenAPI/Swagger
 Home-page: https://github.com/spec-first/connexion
 License: Apache-2.0
 Keywords: api,swagger,openapi
 Author: Daniel Grossmann-Kavanagh
 Author-email: me@danielgk.com
 Maintainer: Robbe Sneyders
```

