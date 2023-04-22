# Comparing `tmp/fastapi_class-3.1.0.tar.gz` & `tmp/fastapi_class-3.2.0.tar.gz`

## Comparing `fastapi_class-3.1.0.tar` & `fastapi_class-3.2.0.tar`

### file list

```diff
@@ -1,28 +1,32 @@
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/codecov.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/fastapi_class/__init__.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/fastapi_class/exceptions.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/fastapi_class/logger.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/fastapi_class/openapi.py
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/fastapi_class/routers.py
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/fastapi_class/views.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/scripts/clean.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/scripts/format.sh
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/scripts/lint.sh
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/scripts/test.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/tests/__init__.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/tests/test_exceptions.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/tests/test_openapi.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/tests/test_routers.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/tests/test_version.py
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/tests/test_views.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/LICENSE
--rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/README.md
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 fastapi_class-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/codecov.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/fastapi_class/__init__.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/fastapi_class/logger.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/fastapi_class/openapi.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/fastapi_class/routers.py
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/fastapi_class/views.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/fastapi_class/exception/__init__.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/fastapi_class/exception/handler.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/scripts/clean.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/scripts/format.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/scripts/lint.sh
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/scripts/test.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/factory.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/test_logger.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/test_metadata.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/test_openapi.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/test_routers.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/test_version.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/test_views.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/LICENSE
+-rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/README.md
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6648 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/PKG-INFO
```

### Comparing `fastapi_class-3.1.0/.pre-commit-config.yaml` & `fastapi_class-3.2.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
     rev: v3.3.1
     hooks:
     -   id: pyupgrade
         args:
         - --py3-plus
         - --keep-runtime-typing
 -   repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.255
+    rev: v0.0.262
     hooks:
     -   id: ruff
         args:
         - --fix
 -   repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
     -   id: isort
         name: isort (python)
 -   repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
     -   id: black
```

### Comparing `fastapi_class-3.1.0/.github/workflows/lint.yaml` & `fastapi_class-3.2.0/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.1.0/.github/workflows/publish.yml` & `fastapi_class-3.2.0/.github/workflows/publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,14 @@
           key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-publish
       - name: Install build dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install build
       - name: Build distribution
         run: python -m build
       - name: Publish
-        uses: pypa/gh-action-pypi-publish@v1.8.1
+        uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
       - name: Dump GitHub context
         env:
           GITHUB_CONTEXT: ${{ toJson(github) }}
         run: echo "$GITHUB_CONTEXT"
```

### Comparing `fastapi_class-3.1.0/.github/workflows/test.yml` & `fastapi_class-3.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.1.0/fastapi_class/__init__.py` & `fastapi_class-3.2.0/fastapi_class/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,29 +33,23 @@
     def post(self, user: ItemModel):
         pass
 ```
 
 """
 
 
-__version__ = "3.1.0"
+__version__ = "3.2.0"
 
-from fastapi_class.exceptions import (
-    UNKNOWN_SERVER_ERROR_DETAIL,
-    ExceptionAbstract,
-    FormattedMessageException,
-)
+from fastapi_class.exception import FormattedMessageException
 from fastapi_class.openapi import ExceptionModel, _exceptions_to_responses
 from fastapi_class.routers import Metadata, Method, endpoint
 from fastapi_class.views import View
 
 __all__ = [
     "View",
     "endpoint",
     "Method",
     "Metadata",
     "FormattedMessageException",
-    "UNKNOWN_SERVER_ERROR_DETAIL",
-    "ExceptionAbstract",
     "ExceptionModel",
     "_exceptions_to_responses",
 ]
```

### Comparing `fastapi_class-3.1.0/fastapi_class/exceptions.py` & `fastapi_class-3.2.0/fastapi_class/exception/handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 from abc import ABC, abstractmethod
-from typing import Any, List
+from collections.abc import Iterable
+from typing import Any
 
 from fastapi import HTTPException, status
-from pydantic import BaseModel
 
-UNKNOWN_SERVER_ERROR_DETAIL = "Unknown server error"
+UNKOWN_SERVER_ERROR_DETAIL = "Unknown server error"
 
 
 class ExceptionAbstract(ABC):
-    """Abstract class for exception."""
+    _DEFAULT_DETAIL_SPECIAL_NAME = "__detail__"
 
-    _DEFAULT_DETAIL_SPECIAL_NAME = "DEFAULT_DETAIL"
-    exceptions: List[tuple[int, str]] = []
-
-    def __init__(self, *, exceptions: List[tuple[int, str]] = None) -> None:
-        self.exceptions = exceptions or [
-            (status.HTTP_500_INTERNAL_SERVER_ERROR, UNKNOWN_SERVER_ERROR_DETAIL)
+    def __init__(self, *, exceptions: Iterable[tuple[int, str]] | None = None) -> None:
+        self._exceptions = exceptions or [
+            (status.HTTP_500_INTERNAL_SERVER_ERROR, UNKOWN_SERVER_ERROR_DETAIL)
         ]
 
     @classmethod
     @abstractmethod
     def __call__(cls, *args: Any, **kwds: Any) -> Any:
         raise NotImplementedError
 
 
-class FormattedMessageException(BaseModel, ExceptionAbstract):
-    """Exception with formatted message."""
-
-    exceptions: List[tuple[int, str]]
-
+class FormattedMessageException(ExceptionAbstract):
     def __call__(self, *_, **kwargs):
-        _exception = self.exceptions[0]
+        _exception = self._exceptions[0]
 
         try:
             detail = _exception[1].format(**kwargs)
         except (IndexError, KeyError):
             detail = _exception[1]
-
         return HTTPException(status_code=_exception[0], detail=detail)
```

### Comparing `fastapi_class-3.1.0/fastapi_class/openapi.py` & `fastapi_class-3.2.0/fastapi_class/openapi.py`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.1.0/scripts/clean.sh` & `fastapi_class-3.2.0/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.1.0/tests/test_exceptions.py` & `fastapi_class-3.2.0/tests/test_exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 from unittest.mock import patch
 
 import pytest
 
-from fastapi_class import (
-    UNKNOWN_SERVER_ERROR_DETAIL,
+from fastapi_class.exception import (
+    UNKOWN_SERVER_ERROR_DETAIL,
     ExceptionAbstract,
     FormattedMessageException,
 )
 
 
-@patch("fastapi_class.ExceptionAbstract.__abstractmethods__", set())
+@patch("fastapi_class.exception.ExceptionAbstract.__abstractmethods__", set())
 def test_abstract_factory_creation__defaults():
     _instance = ExceptionAbstract()
-    assert _instance.exceptions[0][0] == 500
-    assert _instance.exceptions[0][1] == UNKNOWN_SERVER_ERROR_DETAIL
+    assert _instance._exceptions[0][0] == 500
+    assert _instance._exceptions[0][1] == UNKOWN_SERVER_ERROR_DETAIL
 
 
 @pytest.mark.parametrize("keyword_args", ({}, {"some_var": 0}))
 def test_formatted_message_factory__non_formattable_string(keyword_args: dict):
     _instance = FormattedMessageException(exceptions=((500, "Test"),))
     assert _instance(keyword_args).detail == "Test"
 
 
 @pytest.mark.parametrize("arg", ("t", 0, 3.141592, False))
 def test_formatted_message_factory__format_string(arg: str | int | float | bool):
     _instance = FormattedMessageException(exceptions=((500, "Test {test}"),))
     assert _instance(**{"test": arg}).detail == f"Test {arg}"
+
+
+@patch("fastapi_class.exception.ExceptionAbstract.__abstractmethods__", set())
+def test_formatted_message_factory__format_string__missing_key():
+    _instance = FormattedMessageException(exceptions=((500, "Test {test}"),))
+    assert _instance().detail == "Test {test}"
```

### Comparing `fastapi_class-3.1.0/tests/test_openapi.py` & `fastapi_class-3.2.0/tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.1.0/tests/test_routers.py` & `fastapi_class-3.2.0/tests/test_routers.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import pytest
 
 from fastapi_class import Method, endpoint
 
 
 async def dummy_function():
-    pass
+    pass  # pragma: no cover
 
 
 def assert_methods_in_metadata(_endpoint: Callable, methods: Iterable[Method]):
     assert _endpoint.__endpoint_metadata
     assert len(_endpoint.__endpoint_metadata.methods) == len(methods)
     assert all(method in _endpoint.__endpoint_metadata.methods for method in methods)
 
@@ -43,15 +43,15 @@
     with pytest.raises(AssertionError):
         endpoint(response_class=object)(dummy_function)
 
 
 @pytest.mark.parametrize("method", Method)
 def test_endpoint__method_inferred_from_name(method: Method):
     def foo():
-        pass
+        pass  # pragma: no cover
 
     _endpoint = endpoint(name=method.value)(foo)
     assert_methods_in_metadata(_endpoint, [method])
 
 
 @pytest.mark.parametrize("method", Method)
 def test_endpoint__method_inferred_from_function_name(method: Method):
```

### Comparing `fastapi_class-3.1.0/tests/test_views.py` & `fastapi_class-3.2.0/tests/test_views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-from typing import Any, Generic, TypeVar
-
 import pytest
-from fastapi import APIRouter, FastAPI
-
-from fastapi_class import Method, View, endpoint
-
-T = TypeVar("T")
-
+from fastapi import APIRouter, FastAPI, status
 
-class Factory(Generic[T]):
-    def __call__(self, *args: Any, **kwds: Any) -> T:
-        ...
+from fastapi_class import Method, View
+from tests.factory import Factory
 
 
-def decorate_view(app: FastAPI, router: APIRouter | None, class_base_view: object):
-    View(router or app)(class_base_view)
+def decorate_view(
+    app: FastAPI,
+    router: APIRouter | None,
+    class_base_view: object,
+    default_status_code: int = status.HTTP_200_OK,
+):
+    View(router or app, default_status_code=default_status_code)(class_base_view)
     if router:
         app.include_router(router)
 
 
 @pytest.fixture(name="application")
 def fixture_application():
     yield FastAPI()
 
 
 @pytest.fixture(name="router_factory")
 def fixture_router_factory():
-    def _factory():
-        router = APIRouter()
+    def _factory(prefix: str = ""):
+        router = APIRouter(prefix=prefix)
         return router
 
     return _factory
 
 
 @pytest.fixture(name="class_base_view_factory")
 def fixture_class_base_view_factory():
@@ -52,15 +49,15 @@
             dummy.__name__ = method.value
             data[method.value] = dummy
         for _endpoint in endpoints:
 
             def dummy(self):
                 ...
 
-            data[dummy.__name__ or _endpoint["alternative_name"]] = _endpoint[
+            data[_endpoint.get("alternative_name") or dummy.__name__] = _endpoint[
                 "decorator"
             ](dummy)
         class_base_view = type(name, (object,), data)
 
         return class_base_view
 
     return _factory
@@ -80,30 +77,7 @@
         assert method.value in schema["paths"]["/"]
         assert (
             schema["paths"]["/"][method.value]["summary"]
             == f"{method.value.capitalize()} Test Class Based"
         )
         responses = schema["paths"]["/"][method.value]["responses"]
         assert "200" in responses
-
-
-@pytest.mark.skip(reason="The assertion is not working")
-def test_view__use_name_in_endpoint_decorator(
-    application: FastAPI,
-    class_base_view_factory: Factory[object],
-    router_factory: Factory[APIRouter],
-):
-    router = router_factory()
-    class_base_view = class_base_view_factory(
-        endpoints=[
-            {
-                "decorator": endpoint(
-                    methods=["POST"], name="Edit Test Class Based", path="edit"
-                )
-            }
-        ]
-    )
-    decorate_view(application, router, class_base_view)
-    schema = application.openapi()
-    assert "/edit" in schema["paths"]
-    assert "post" in schema["paths"]["/edit"]
-    assert schema["paths"]["/edit"]["post"]["summary"] == "Edit Test Class Based"
```

### Comparing `fastapi_class-3.1.0/.gitignore` & `fastapi_class-3.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.1.0/LICENSE` & `fastapi_class-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.1.0/README.md` & `fastapi_class-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.1.0/pyproject.toml` & `fastapi_class-3.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -36,24 +36,23 @@
 
 [project.urls]
 Homepage = "https://github.com/yezz123/fastapi-class"
 Funding = 'https://github.com/sponsors/yezz123'
 
 [project.optional-dependencies]
 lint = [
-    "pre-commit==3.2.0",
-    "mypy==1.1.1",
+    "pre-commit==3.2.2",
+    "mypy==1.2.0",
 ]
 test = [
     "requests==2.28.2",
-    "pytest==7.2.2",
+    "pytest==7.3.1",
     "pytest-asyncio == 0.21.0",
-    "codecov==2.1.12",
     "pytest-cov==4.0.0",
-    "pytest-pretty==1.1.0",
+    "pytest-pretty==1.2.0",
 ]
 
 [tool.hatch.version]
 path = "fastapi_class/__init__.py"
 
 [tool.isort]
 profile = "black"
@@ -68,14 +67,15 @@
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
 ]
 ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "C901",  # too complex
+    "B018",  # Found useless expression
 ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.isort]
 known-third-party = ["pydantic", "typing_extensions"]
```

### Comparing `fastapi_class-3.1.0/PKG-INFO` & `fastapi_class-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_class
-Version: 3.1.0
+Version: 3.2.0
 Summary: Simplifies class-based views for more organized and maintainable code in FastAPI.
 Project-URL: Homepage, https://github.com/yezz123/fastapi-class
 Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri <hello@yezz.me>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Framework :: AsyncIO
@@ -19,22 +19,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: fastapi<0.96.0,>=0.65.2
 Requires-Dist: pydantic!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<2.0.0,>=1.6.2
 Provides-Extra: lint
-Requires-Dist: mypy==1.1.1; extra == 'lint'
-Requires-Dist: pre-commit==3.2.0; extra == 'lint'
+Requires-Dist: mypy==1.2.0; extra == 'lint'
+Requires-Dist: pre-commit==3.2.2; extra == 'lint'
 Provides-Extra: test
-Requires-Dist: codecov==2.1.12; extra == 'test'
 Requires-Dist: pytest-asyncio==0.21.0; extra == 'test'
 Requires-Dist: pytest-cov==4.0.0; extra == 'test'
-Requires-Dist: pytest-pretty==1.1.0; extra == 'test'
-Requires-Dist: pytest==7.2.2; extra == 'test'
+Requires-Dist: pytest-pretty==1.2.0; extra == 'test'
+Requires-Dist: pytest==7.3.1; extra == 'test'
 Requires-Dist: requests==2.28.2; extra == 'test'
 Description-Content-Type: text/markdown
 
 ![Class](https://user-images.githubusercontent.com/52716203/137606695-f110f129-08b1-45f3-a445-962c1f28378c.png)
 
 <p align="center">
     <em>Classes and Decorators to use FastAPI with Class based routing</em>
```

