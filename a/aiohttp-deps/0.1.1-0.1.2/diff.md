# Comparing `tmp/aiohttp_deps-0.1.1.tar.gz` & `tmp/aiohttp_deps-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_deps-0.1.1.tar", max compression
+gzip compressed data, was "aiohttp_deps-0.1.2.tar", max compression
```

## Comparing `aiohttp_deps-0.1.1.tar` & `aiohttp_deps-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-04-21 01:35:32.989308 aiohttp_deps-0.1.1/LICENSE
--rw-r--r--   0        0        0     5955 2023-04-21 01:35:32.989308 aiohttp_deps-0.1.1/README.md
--rw-r--r--   0        0        0      357 2023-04-21 01:35:32.989308 aiohttp_deps-0.1.1/aiohttp_deps/__init__.py
--rw-r--r--   0        0        0     2221 2023-04-21 01:35:32.989308 aiohttp_deps-0.1.1/aiohttp_deps/initializer.py
--rw-r--r--   0        0        0        0 2023-04-21 01:35:32.989308 aiohttp_deps-0.1.1/aiohttp_deps/py.typed
--rw-r--r--   0        0        0      342 2023-04-21 01:35:32.989308 aiohttp_deps-0.1.1/aiohttp_deps/router.py
--rw-r--r--   0        0        0      792 2023-04-21 01:35:32.989308 aiohttp_deps-0.1.1/aiohttp_deps/router.pyi
--rw-r--r--   0        0        0     5916 2023-04-21 01:35:32.989308 aiohttp_deps-0.1.1/aiohttp_deps/utils.py
--rw-r--r--   0        0        0     1317 2023-04-21 01:35:32.989308 aiohttp_deps-0.1.1/aiohttp_deps/view.py
--rw-r--r--   0        0        0     1766 2023-04-21 01:35:32.989308 aiohttp_deps-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7262 1970-01-01 00:00:00.000000 aiohttp_deps-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-22 15:35:11.839741 aiohttp_deps-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6819 2023-04-22 15:35:11.839741 aiohttp_deps-0.1.2/README.md
+-rw-r--r--   0        0        0      375 2023-04-22 15:35:11.839741 aiohttp_deps-0.1.2/aiohttp_deps/__init__.py
+-rw-r--r--   0        0        0     2221 2023-04-22 15:35:11.839741 aiohttp_deps-0.1.2/aiohttp_deps/initializer.py
+-rw-r--r--   0        0        0        0 2023-04-22 15:35:11.839741 aiohttp_deps-0.1.2/aiohttp_deps/py.typed
+-rw-r--r--   0        0        0     1211 2023-04-22 15:35:11.839741 aiohttp_deps-0.1.2/aiohttp_deps/router.py
+-rw-r--r--   0        0        0      890 2023-04-22 15:35:11.843741 aiohttp_deps-0.1.2/aiohttp_deps/router.pyi
+-rw-r--r--   0        0        0     7447 2023-04-22 15:35:11.843741 aiohttp_deps-0.1.2/aiohttp_deps/utils.py
+-rw-r--r--   0        0        0     1317 2023-04-22 15:35:11.843741 aiohttp_deps-0.1.2/aiohttp_deps/view.py
+-rw-r--r--   0        0        0     1766 2023-04-22 15:35:11.843741 aiohttp_deps-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     8126 1970-01-01 00:00:00.000000 aiohttp_deps-0.1.2/PKG-INFO
```

### Comparing `aiohttp_deps-0.1.1/LICENSE` & `aiohttp_deps-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.1/README.md` & `aiohttp_deps-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -48,14 +48,28 @@
 
 app.on_startup.append(deps_init)
 
 web.run_app(app)
 
 ```
 
+Also, you can nest routers with prefixes,
+
+```python
+api_router = Router()
+
+memes_router = Router()
+
+main_router = Router()
+
+main_router.add_routes(api_router, prefix="/api")
+main_router.add_routes(memes_router, prefix="/memes")
+```
+
+
 ## Default dependencies
 
 By default this library provides only two injectables. `web.Request` and `web.Application`.
 
 ```python
 
 async def handler(app: web.Application = Depends()): ...
@@ -229,7 +243,38 @@
 
 @router.view("/view")
 class MyView(View):
     async def get(self, app: web.Application = Depends()):
         return web.json_response({"app": str(app)})
 
 ```
+
+
+## Forms
+
+Now you can easiy get and validate form data from your request.
+To make the magic happen, please add `arbitrary_types_allowed` to the config of your model.
+
+
+```python
+from pydantic import BaseModel
+from aiohttp_deps import Router, Depends, Form
+from aiohttp import web
+
+router = Router()
+
+
+class MyForm(BaseModel):
+    id: int
+    file: web.FileField
+
+    class Config:
+        arbitrary_types_allowed = True
+
+
+@router.post("/")
+async def handler(my_form: MyForm = Depends(Form())):
+    with open("my_file", "wb") as f:
+        f.write(my_form.file.file.read())
+    return web.json_response({"id": my_form.id})
+
+```
```

### Comparing `aiohttp_deps-0.1.1/aiohttp_deps/initializer.py` & `aiohttp_deps-0.1.2/aiohttp_deps/initializer.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.1/aiohttp_deps/router.pyi` & `aiohttp_deps-0.1.2/aiohttp_deps/router.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Awaitable, Callable, Type, Union
+from typing import Any, Awaitable, Callable, Iterable, Type, Union
 
 from aiohttp import web
 from aiohttp.abc import AbstractView
 
 _Handler = Callable[..., Awaitable[web.StreamResponse]]
 
 _ViewedHandler = Union[Type[AbstractView], _Handler]
@@ -14,7 +14,8 @@
     def get(self, path: str, **kwargs: Any) -> _Deco: ...
     def post(self, path: str, **kwargs: Any) -> _Deco: ...
     def put(self, path: str, **kwargs: Any) -> _Deco: ...
     def patch(self, path: str, **kwargs: Any) -> _Deco: ...
     def delete(self, path: str, **kwargs: Any) -> _Deco: ...
     def options(self, path: str, **kwargs: Any) -> _Deco: ...
     def view(self, path: str, **kwargs: Any) -> _Deco: ...
+    def add_routes(self, router: Iterable[web.RouteDef], prefix: str = "") -> None: ...
```

### Comparing `aiohttp_deps-0.1.1/aiohttp_deps/utils.py` & `aiohttp_deps-0.1.2/aiohttp_deps/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,15 +66,18 @@
             return value
 
         try:
             return pydantic.parse_obj_as(definition, value)
         except pydantic.ValidationError as err:
             errors = err.errors()
             for error in errors:
-                error["loc"] = (f"header:{header_name}",)
+                error["loc"] = (
+                    "header",
+                    header_name,
+                ) + error["loc"]
             raise web.HTTPBadRequest(
                 headers={"Content-Type": "application/json"},
                 text=json.dumps(errors),
             )
 
 
 class Json:
@@ -115,15 +118,15 @@
             return body
 
         try:
             return pydantic.parse_obj_as(definition, body)
         except pydantic.ValidationError as err:
             errors = err.errors()
             for error in errors:
-                error["loc"] = ("body",)
+                error["loc"] = ("body",) + error["loc"]
             raise web.HTTPBadRequest(
                 headers={"Content-Type": "application/json"},
                 text=json.dumps(errors),
             )
 
 
 class Query:
@@ -185,12 +188,62 @@
             return value
 
         try:
             return pydantic.parse_obj_as(definition, value)
         except pydantic.ValidationError as err:
             errors = err.errors()
             for error in errors:
-                error["loc"] = (f"querystring:{param_name}",)
+                error["loc"] = (
+                    "query",
+                    param_name,
+                ) + error["loc"]
+            raise web.HTTPBadRequest(
+                headers={"Content-Type": "application/json"},
+                text=json.dumps(errors),
+            )
+
+
+class Form:
+    """
+    Get and validate form data.
+
+    This dependency grabs form data and validates
+    it against given schema.
+
+    You should provide schema with typehints.
+    """
+
+    async def __call__(
+        self,
+        param_info: ParamInfo = Depends(),
+        request: web.Request = Depends(),
+    ) -> Any:
+        """
+        Performs actual logic, described above.
+
+        :param param_info: information about how the dependency
+            was defined with name and type.
+        :param request: current request.
+        :raises HTTPBadRequest: if incorrect data was found.
+        :return: parsed data.
+        """
+        form_data = await request.post()
+        definition = None
+        if (  # noqa: WPS337
+            param_info.definition
+            and param_info.definition.annotation != inspect.Parameter.empty
+        ):
+            definition = param_info.definition.annotation
+
+        if definition is None:
+            return form_data
+
+        try:
+            return pydantic.parse_obj_as(definition, form_data)
+        except pydantic.ValidationError as err:
+            errors = err.errors()
+            for error in errors:
+                error["loc"] = ("form",) + error["loc"]
             raise web.HTTPBadRequest(
                 headers={"Content-Type": "application/json"},
                 text=json.dumps(errors),
             )
```

### Comparing `aiohttp_deps-0.1.1/aiohttp_deps/view.py` & `aiohttp_deps-0.1.2/aiohttp_deps/view.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.1/pyproject.toml` & `aiohttp_deps-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "aiohttp-deps"
 description = "Dependency injection for AioHTTP"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `aiohttp_deps-0.1.1/PKG-INFO` & `aiohttp_deps-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-deps
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dependency injection for AioHTTP
 Home-page: https://github.com/taskiq-python/aiohttp-deps
 License: LICENSE
 Keywords: aiohttp,taskiq-dependencies
 Author: Taskiq team
 Author-email: taskiq@no-reply.com
 Maintainer: Taskiq team
@@ -82,14 +82,28 @@
 
 app.on_startup.append(deps_init)
 
 web.run_app(app)
 
 ```
 
+Also, you can nest routers with prefixes,
+
+```python
+api_router = Router()
+
+memes_router = Router()
+
+main_router = Router()
+
+main_router.add_routes(api_router, prefix="/api")
+main_router.add_routes(memes_router, prefix="/memes")
+```
+
+
 ## Default dependencies
 
 By default this library provides only two injectables. `web.Request` and `web.Application`.
 
 ```python
 
 async def handler(app: web.Application = Depends()): ...
@@ -264,7 +278,38 @@
 @router.view("/view")
 class MyView(View):
     async def get(self, app: web.Application = Depends()):
         return web.json_response({"app": str(app)})
 
 ```
 
+
+## Forms
+
+Now you can easiy get and validate form data from your request.
+To make the magic happen, please add `arbitrary_types_allowed` to the config of your model.
+
+
+```python
+from pydantic import BaseModel
+from aiohttp_deps import Router, Depends, Form
+from aiohttp import web
+
+router = Router()
+
+
+class MyForm(BaseModel):
+    id: int
+    file: web.FileField
+
+    class Config:
+        arbitrary_types_allowed = True
+
+
+@router.post("/")
+async def handler(my_form: MyForm = Depends(Form())):
+    with open("my_file", "wb") as f:
+        f.write(my_form.file.file.read())
+    return web.json_response({"id": my_form.id})
+
+```
+
```

