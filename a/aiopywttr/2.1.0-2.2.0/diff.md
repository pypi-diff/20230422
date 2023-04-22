# Comparing `tmp/aiopywttr-2.1.0.tar.gz` & `tmp/aiopywttr-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopywttr-2.1.0.tar", max compression
+gzip compressed data, was "aiopywttr-2.2.0.tar", max compression
```

## Comparing `aiopywttr-2.1.0.tar` & `aiopywttr-2.2.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1065 2022-11-26 18:29:32.848032 aiopywttr-2.1.0/LICENSE
--rw-r--r--   0        0        0     1608 2022-11-26 18:29:32.848032 aiopywttr-2.1.0/README.md
--rw-r--r--   0        0        0      142 2022-11-26 18:29:32.848032 aiopywttr-2.1.0/aiopywttr/__init__.py
--rw-r--r--   0        0        0     5662 2022-11-26 19:36:21.373218 aiopywttr-2.1.0/aiopywttr/_wttr.py
--rw-r--r--   0        0        0        0 2022-11-26 18:29:32.848032 aiopywttr-2.1.0/aiopywttr/py.typed
--rw-r--r--   0        0        0     2820 2022-11-26 19:54:10.959696 aiopywttr-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     2347 1970-01-01 00:00:00.000000 aiopywttr-2.1.0/setup.py
--rw-r--r--   0        0        0     2609 1970-01-01 00:00:00.000000 aiopywttr-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-20 07:24:39.800123 aiopywttr-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1738 2023-04-22 20:08:34.439262 aiopywttr-2.2.0/README.md
+-rw-r--r--   0        0        0      183 2023-04-22 19:53:57.019253 aiopywttr-2.2.0/aiopywttr/__init__.py
+-rw-r--r--   0        0        0     5591 2023-04-20 07:24:39.800123 aiopywttr-2.2.0/aiopywttr/_wttr.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:24:39.800123 aiopywttr-2.2.0/aiopywttr/py.typed
+-rw-r--r--   0        0        0     3046 2023-04-22 20:17:01.709267 aiopywttr-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3202 1970-01-01 00:00:00.000000 aiopywttr-2.2.0/PKG-INFO
```

### Comparing `aiopywttr-2.1.0/LICENSE` & `aiopywttr-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopywttr-2.1.0/README.md` & `aiopywttr-2.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 # aiopywttr
 
-[![CI](https://github.com/monosans/aiopywttr/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/aiopywttr/actions/workflows/ci.yml)
+[![CI](https://github.com/monosans/aiopywttr/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/aiopywttr/actions/workflows/ci.yml?query=event%3Apush+branch%3Amain)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/aiopywttr/main.svg)](https://results.pre-commit.ci/latest/github/monosans/aiopywttr/main)
-[![codecov](https://codecov.io/gh/monosans/aiopywttr/branch/main/graph/badge.svg)](https://codecov.io/gh/monosans/aiopywttr)
+[![Coverage](https://img.shields.io/codecov/c/github/monosans/aiopywttr/main?logo=codecov)](https://codecov.io/gh/monosans/aiopywttr)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/aiopywttr?logo=pypi)](https://pypi.org/project/aiopywttr/)
 
 Asynchronous wrapper for [wttr.in](https://wttr.in) weather forecast API.
 
 Synchronous version [here](https://github.com/monosans/pywttr).
 
 ## Installation
 
 ```bash
-python -m pip install aiopywttr
+python -m pip install -U aiopywttr pywttr-models
 ```
 
 ## Example
 
 This example prints the average temperature in New York today.
 
 ```python
 import asyncio
 
-from aiopywttr import Wttr
+import aiopywttr
 
 
 async def main():
-    wttr = Wttr("New York")
+    wttr = aiopywttr.Wttr("New York")
     forecast = await wttr.en()
     print(forecast.weather[0].avgtemp_c)
 
 
 asyncio.run(main())
 ```
 
 Other languages may also be used instead of `en`. For a complete list of supported languages, follow the code completion in your IDE.
 
 ## Documentation
 
-There is no documentation, just follow the code completion in your IDE.
+There is no documentation, just follow the example and code completion in your IDE.
 
-For an example of type annotations, see `pywttr-models` [README.md](https://github.com/monosans/pywttr-models#usage-for-type-annotation).
+All types of objects returned by the wttr.in API are in the `aiopywttr.models` package.
 
 ## Recommended IDEs
 
 - [Visual Studio Code](https://code.visualstudio.com) (with [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python))
 - [PyCharm](https://jetbrains.com/pycharm)
 
 ## License
```

### Comparing `aiopywttr-2.1.0/aiopywttr/_wttr.py` & `aiopywttr-2.2.0/aiopywttr/_wttr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from __future__ import annotations
 
 from typing import Any, Optional
 
 import pywttr_models
-from aiohttp import ClientSession
+from aiohttp import ClientResponse, ClientSession
 
 
-# pylint: disable-next=too-many-public-methods
 class Wttr:
     """Asynchronous wrapper for wttr.in weather forecast API."""
 
     __slots__ = ("location", "session")
 
-    def __init__(
-        self, location: str, session: Optional[ClientSession] = None
-    ) -> None:
+    def __init__(self, location: str, session: Optional[ClientSession] = None) -> None:
         self.location = location
         self.session = session
 
-    # pylint: disable=invalid-name
     async def af(self) -> pywttr_models.af.Model:
         return pywttr_models.af.Model.parse_obj(await self._get_json("af"))
 
     async def am(self) -> pywttr_models.am.Model:
         return pywttr_models.am.Model.parse_obj(await self._get_json("am"))
 
     async def ar(self) -> pywttr_models.ar.Model:
@@ -66,15 +62,15 @@
 
     async def hu(self) -> pywttr_models.hu.Model:
         return pywttr_models.hu.Model.parse_obj(await self._get_json("hu"))
 
     async def ia(self) -> pywttr_models.ia.Model:
         return pywttr_models.ia.Model.parse_obj(await self._get_json("ia"))
 
-    async def id(self) -> pywttr_models.id.Model:
+    async def id(self) -> pywttr_models.id.Model:  # noqa: A003
         return pywttr_models.id.Model.parse_obj(await self._get_json("id"))
 
     async def it(self) -> pywttr_models.it.Model:
         return pywttr_models.it.Model.parse_obj(await self._get_json("it"))
 
     async def lt(self) -> pywttr_models.lt.Model:
         return pywttr_models.lt.Model.parse_obj(await self._get_json("lt"))
@@ -91,17 +87,15 @@
     async def oc(self) -> pywttr_models.oc.Model:
         return pywttr_models.oc.Model.parse_obj(await self._get_json("oc"))
 
     async def pl(self) -> pywttr_models.pl.Model:
         return pywttr_models.pl.Model.parse_obj(await self._get_json("pl"))
 
     async def pt_br(self) -> pywttr_models.pt_br.Model:
-        return pywttr_models.pt_br.Model.parse_obj(
-            await self._get_json("pt-br")
-        )
+        return pywttr_models.pt_br.Model.parse_obj(await self._get_json("pt-br"))
 
     async def ro(self) -> pywttr_models.ro.Model:
         return pywttr_models.ro.Model.parse_obj(await self._get_json("ro"))
 
     async def ru(self) -> pywttr_models.ru.Model:
         return pywttr_models.ru.Model.parse_obj(await self._get_json("ru"))
 
@@ -117,30 +111,28 @@
     async def uk(self) -> pywttr_models.uk.Model:
         return pywttr_models.uk.Model.parse_obj(await self._get_json("uk"))
 
     async def vi(self) -> pywttr_models.vi.Model:
         return pywttr_models.vi.Model.parse_obj(await self._get_json("vi"))
 
     async def zh_cn(self) -> pywttr_models.zh_cn.Model:
-        return pywttr_models.zh_cn.Model.parse_obj(
-            await self._get_json("zh-cn")
-        )
+        return pywttr_models.zh_cn.Model.parse_obj(await self._get_json("zh-cn"))
 
     async def zh_tw(self) -> pywttr_models.zh_tw.Model:
-        return pywttr_models.zh_tw.Model.parse_obj(
-            await self._get_json("zh-tw")
-        )
+        return pywttr_models.zh_tw.Model.parse_obj(await self._get_json("zh-tw"))
 
-    # pylint: enable=invalid-name
-    async def _fetch(self, lang: str, session: ClientSession) -> Any:
+    async def _get_json(self, lang: str) -> Any:
+        if isinstance(self.session, ClientSession) and not self.session.closed:
+            response = await self._fetch(lang, self.session)
+        else:
+            async with ClientSession() as session:
+                response = await self._fetch(lang, session)
+        return await response.json()
+
+    async def _fetch(self, lang: str, session: ClientSession) -> ClientResponse:
         async with session.get(
             f"https://wttr.in/{self.location}",
             params={"format": "j1", "lang": lang},
             raise_for_status=True,
         ) as response:
-            return await response.json()
-
-    async def _get_json(self, lang: str) -> Any:
-        if isinstance(self.session, ClientSession) and not self.session.closed:
-            return await self._fetch(lang, self.session)
-        async with ClientSession() as session:
-            return await self._fetch(lang, session)
+            await response.read()
+        return response
```

### Comparing `aiopywttr-2.1.0/PKG-INFO` & `aiopywttr-2.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,87 @@
 Metadata-Version: 2.1
 Name: aiopywttr
-Version: 2.1.0
+Version: 2.2.0
 Summary: Asynchronous wrapper for wttr.in API
 Home-page: https://github.com/monosans/aiopywttr
 License: MIT
 Keywords: forecast,weather
 Author: monosans
 Author-email: hsyqixco@protonmail.com
 Requires-Python: >=3.7.2,<4.0.0
+Classifier: Environment :: Web Environment
+Classifier: Framework :: AsyncIO
+Classifier: Framework :: Pydantic
+Classifier: Framework :: Pydantic :: 1
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: aiohttp (>=3.8,<4.0)
 Requires-Dist: pywttr-models (>=1.1,<2.0)
 Project-URL: Repository, https://github.com/monosans/aiopywttr
 Description-Content-Type: text/markdown
 
 # aiopywttr
 
-[![CI](https://github.com/monosans/aiopywttr/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/aiopywttr/actions/workflows/ci.yml)
+[![CI](https://github.com/monosans/aiopywttr/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/aiopywttr/actions/workflows/ci.yml?query=event%3Apush+branch%3Amain)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/aiopywttr/main.svg)](https://results.pre-commit.ci/latest/github/monosans/aiopywttr/main)
-[![codecov](https://codecov.io/gh/monosans/aiopywttr/branch/main/graph/badge.svg)](https://codecov.io/gh/monosans/aiopywttr)
+[![Coverage](https://img.shields.io/codecov/c/github/monosans/aiopywttr/main?logo=codecov)](https://codecov.io/gh/monosans/aiopywttr)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/aiopywttr?logo=pypi)](https://pypi.org/project/aiopywttr/)
 
 Asynchronous wrapper for [wttr.in](https://wttr.in) weather forecast API.
 
 Synchronous version [here](https://github.com/monosans/pywttr).
 
 ## Installation
 
 ```bash
-python -m pip install aiopywttr
+python -m pip install -U aiopywttr pywttr-models
 ```
 
 ## Example
 
 This example prints the average temperature in New York today.
 
 ```python
 import asyncio
 
-from aiopywttr import Wttr
+import aiopywttr
 
 
 async def main():
-    wttr = Wttr("New York")
+    wttr = aiopywttr.Wttr("New York")
     forecast = await wttr.en()
     print(forecast.weather[0].avgtemp_c)
 
 
 asyncio.run(main())
 ```
 
 Other languages may also be used instead of `en`. For a complete list of supported languages, follow the code completion in your IDE.
 
 ## Documentation
 
-There is no documentation, just follow the code completion in your IDE.
+There is no documentation, just follow the example and code completion in your IDE.
 
-For an example of type annotations, see `pywttr-models` [README.md](https://github.com/monosans/pywttr-models#usage-for-type-annotation).
+All types of objects returned by the wttr.in API are in the `aiopywttr.models` package.
 
 ## Recommended IDEs
 
 - [Visual Studio Code](https://code.visualstudio.com) (with [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python))
 - [PyCharm](https://jetbrains.com/pycharm)
 
 ## License
```

