# Comparing `tmp/aiopygismeteo-5.0.6.tar.gz` & `tmp/aiopygismeteo-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopygismeteo-5.0.6.tar", max compression
+gzip compressed data, was "aiopygismeteo-5.1.0.tar", max compression
```

## Comparing `aiopygismeteo-5.0.6.tar` & `aiopygismeteo-5.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-01-30 17:30:13.723784 aiopygismeteo-5.0.6/LICENSE
--rw-r--r--   0        0        0     1368 2023-01-30 17:30:13.723784 aiopygismeteo-5.0.6/README.md
--rw-r--r--   0        0        0      158 2023-01-30 17:30:13.724784 aiopygismeteo-5.0.6/aiopygismeteo/__init__.py
--rw-r--r--   0        0        0     1422 2023-01-30 17:30:13.724784 aiopygismeteo-5.0.6/aiopygismeteo/_current.py
--rw-r--r--   0        0        0     2858 2023-01-30 17:30:13.724784 aiopygismeteo-5.0.6/aiopygismeteo/_gismeteo.py
--rw-r--r--   0        0        0     1268 2023-01-30 17:30:13.724784 aiopygismeteo-5.0.6/aiopygismeteo/_http.py
--rw-r--r--   0        0        0     1988 2023-01-30 17:30:56.883861 aiopygismeteo-5.0.6/aiopygismeteo/_search.py
--rw-r--r--   0        0        0     2487 2023-01-30 17:30:13.724784 aiopygismeteo-5.0.6/aiopygismeteo/_step_n.py
--rw-r--r--   0        0        0        0 2023-01-30 17:30:13.724784 aiopygismeteo-5.0.6/aiopygismeteo/py.typed
--rw-r--r--   0        0        0     3223 2023-01-30 17:33:31.355138 aiopygismeteo-5.0.6/pyproject.toml
--rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 aiopygismeteo-5.0.6/setup.py
--rw-r--r--   0        0        0     2462 1970-01-01 00:00:00.000000 aiopygismeteo-5.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-16 13:33:16.149443 aiopygismeteo-5.1.0/LICENSE
+-rw-r--r--   0        0        0     1479 2023-04-21 20:15:26.923674 aiopygismeteo-5.1.0/README.md
+-rw-r--r--   0        0        0      232 2023-04-22 17:46:15.729259 aiopygismeteo-5.1.0/aiopygismeteo/__init__.py
+-rw-r--r--   0        0        0     1418 2023-04-22 08:58:30.556323 aiopygismeteo-5.1.0/aiopygismeteo/_current.py
+-rw-r--r--   0        0        0     2890 2023-04-22 08:58:38.266323 aiopygismeteo-5.1.0/aiopygismeteo/_gismeteo.py
+-rw-r--r--   0        0        0     1464 2023-04-21 20:18:19.323691 aiopygismeteo-5.1.0/aiopygismeteo/_http.py
+-rw-r--r--   0        0        0     4003 2023-04-22 17:43:45.689248 aiopygismeteo-5.1.0/aiopygismeteo/_search.py
+-rw-r--r--   0        0        0     4722 2023-04-22 17:47:47.299246 aiopygismeteo-5.1.0/aiopygismeteo/_step_n.py
+-rw-r--r--   0        0        0        0 2023-04-16 13:33:16.149443 aiopygismeteo-5.1.0/aiopygismeteo/py.typed
+-rw-r--r--   0        0        0      322 2023-04-22 18:15:10.209263 aiopygismeteo-5.1.0/aiopygismeteo/types.py
+-rw-r--r--   0        0        0     3199 2023-04-22 19:45:20.959236 aiopygismeteo-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3042 1970-01-01 00:00:00.000000 aiopygismeteo-5.1.0/PKG-INFO
```

### Comparing `aiopygismeteo-5.0.6/LICENSE` & `aiopygismeteo-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopygismeteo-5.0.6/README.md` & `aiopygismeteo-5.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # aiopygismeteo
 
-[![CI](https://github.com/monosans/aiopygismeteo/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/aiopygismeteo/actions/workflows/ci.yml)
+[![CI](https://github.com/monosans/aiopygismeteo/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/aiopygismeteo/actions/workflows/ci.yml?query=event%3Apush+branch%3Amain)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/aiopygismeteo/main.svg)](https://results.pre-commit.ci/latest/github/monosans/aiopygismeteo/main)
-[![codecov](https://codecov.io/gh/monosans/aiopygismeteo/branch/main/graph/badge.svg)](https://codecov.io/gh/monosans/aiopygismeteo)
+[![Coverage](https://img.shields.io/codecov/c/github/monosans/aiopygismeteo/main?logo=codecov)](https://codecov.io/gh/monosans/aiopygismeteo)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/aiopygismeteo?logo=pypi)](https://pypi.org/project/aiopygismeteo/)
 
 Асинхронная обёртка для [Gismeteo API](https://gismeteo.ru/api/).
 
 Синхронная версия [здесь](https://github.com/monosans/pygismeteo).
 
 ## Установка
 
 ```bash
 python -m pip install -U aiopygismeteo
 ```
 
 ## Документация
 
-[aiopygismeteo.readthedocs.io](https://aiopygismeteo.readthedocs.io/)
+<https://aiopygismeteo.readthedocs.io/>
 
 ## Пример, выводящий температуру в Москве сейчас
 
 ```python
 import asyncio
 
-from aiopygismeteo import Gismeteo
+import aiopygismeteo
 
 
 async def main():
-    gismeteo = Gismeteo()
-    search_results = await gismeteo.search.by_query("Москва")
+    gm = aiopygismeteo.Gismeteo()
+    search_results = await gm.search.by_query("Москва")
     city_id = search_results[0].id
-    current = await gismeteo.current.by_id(city_id)
+    current = await gm.current.by_id(city_id)
     print(current.temperature.air.c)
 
 
 asyncio.run(main())
 ```
 
 ## License / Лицензия
```

### Comparing `aiopygismeteo-5.0.6/aiopygismeteo/_gismeteo.py` & `aiopygismeteo-5.1.0/aiopygismeteo/_gismeteo.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,20 @@
         lang: Optional[Lang] = None,
         token: Optional[str] = None,
         session: Optional[ClientSession] = None,
     ) -> None:
         """Асинхронная обёртка для Gismeteo API.
 
         Args:
-            lang: язык. По умолчанию "ru".
-            token: X-Gismeteo-Token,
-                если используемый по умолчанию перестал работать.
-            session: экземпляр aiohttp.ClientSession.
+            lang:
+                Язык. По умолчанию "ru".
+            token:
+                X-Gismeteo-Token, если используемый по умолчанию перестал работать.
+            session:
+                Экземпляр aiohttp.ClientSession.
                 По умолчанию для каждого запроса создаётся новый экземпляр.
         """
         self._settings = Settings(lang=lang, token=token)
         self._session = AiohttpClient(session, self._settings)
         self._current = Current(self._session)
         self._step3 = Step3(self._session)
         self._step6 = Step6(self._session)
```

### Comparing `aiopygismeteo-5.0.6/aiopygismeteo/_http.py` & `aiopygismeteo-5.1.0/aiopygismeteo/_http.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 from __future__ import annotations
 
 from typing import Any
 
-from aiohttp import ClientSession
+from aiohttp import ClientResponse, ClientSession
 from pygismeteo_base.http import BaseHttpClient
-from pygismeteo_base.types import Params
+from pygismeteo_base.types import Headers, Params
 
 
 class AiohttpClient(BaseHttpClient[ClientSession]):
     __slots__ = ()
 
-    async def get_response(
-        self, endpoint: str, *, params: Params = None
-    ) -> Any:
+    async def get_response(self, endpoint: str, *, params: Params = None) -> Any:
         response = await self._get_json(endpoint, params=params)
         return response["response"]
 
     async def _get_json(self, endpoint: str, *, params: Params = None) -> Any:
+        params, headers = self._get_params_and_headers(params)
         if isinstance(self.session, ClientSession) and not self.session.closed:
-            return await self._fetch(
-                endpoint, params=params, session=self.session
+            response = await self._fetch(
+                endpoint, params=params, headers=headers, session=self.session
             )
-        async with ClientSession() as session:
-            return await self._fetch(endpoint, params=params, session=session)
+        else:
+            async with ClientSession() as session:
+                response = await self._fetch(
+                    endpoint, params=params, headers=headers, session=session
+                )
+        return await response.json()
 
     async def _fetch(
-        self, endpoint: str, *, params: Params, session: ClientSession
-    ) -> Any:
-        params, headers = self._get_params_and_headers(params)
+        self, endpoint: str, *, params: Params, headers: Headers, session: ClientSession
+    ) -> ClientResponse:
         async with session.get(
             f"https://api.gismeteo.net/v2/{endpoint}/",
             params=params,
             headers=headers,
             raise_for_status=True,
         ) as response:
-            return await response.json()
+            await response.read()
+        return response
```

### Comparing `aiopygismeteo-5.0.6/PKG-INFO` & `aiopygismeteo-5.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,79 @@
 Metadata-Version: 2.1
 Name: aiopygismeteo
-Version: 5.0.6
+Version: 5.1.0
 Summary: Asynchronous wrapper for Gismeteo API
 Home-page: https://github.com/monosans/aiopygismeteo
 License: MIT
 Author: monosans
 Author-email: hsyqixco@protonmail.com
-Requires-Python: >=3.7.2,<4.0.0
+Requires-Python: >=3.7,<4.0
+Classifier: Environment :: Web Environment
+Classifier: Framework :: AsyncIO
+Classifier: Framework :: Pydantic
+Classifier: Framework :: Pydantic :: 1
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
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
-Requires-Dist: pygismeteo-base (>=4.0,<5.0)
+Requires-Dist: pygismeteo-base (>=4.3,<5.0)
 Project-URL: Documentation, https://aiopygismeteo.readthedocs.io
 Project-URL: Repository, https://github.com/monosans/aiopygismeteo
 Description-Content-Type: text/markdown
 
 # aiopygismeteo
 
-[![CI](https://github.com/monosans/aiopygismeteo/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/aiopygismeteo/actions/workflows/ci.yml)
+[![CI](https://github.com/monosans/aiopygismeteo/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/aiopygismeteo/actions/workflows/ci.yml?query=event%3Apush+branch%3Amain)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/aiopygismeteo/main.svg)](https://results.pre-commit.ci/latest/github/monosans/aiopygismeteo/main)
-[![codecov](https://codecov.io/gh/monosans/aiopygismeteo/branch/main/graph/badge.svg)](https://codecov.io/gh/monosans/aiopygismeteo)
+[![Coverage](https://img.shields.io/codecov/c/github/monosans/aiopygismeteo/main?logo=codecov)](https://codecov.io/gh/monosans/aiopygismeteo)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/aiopygismeteo?logo=pypi)](https://pypi.org/project/aiopygismeteo/)
 
 Асинхронная обёртка для [Gismeteo API](https://gismeteo.ru/api/).
 
 Синхронная версия [здесь](https://github.com/monosans/pygismeteo).
 
 ## Установка
 
 ```bash
 python -m pip install -U aiopygismeteo
 ```
 
 ## Документация
 
-[aiopygismeteo.readthedocs.io](https://aiopygismeteo.readthedocs.io/)
+<https://aiopygismeteo.readthedocs.io/>
 
 ## Пример, выводящий температуру в Москве сейчас
 
 ```python
 import asyncio
 
-from aiopygismeteo import Gismeteo
+import aiopygismeteo
 
 
 async def main():
-    gismeteo = Gismeteo()
-    search_results = await gismeteo.search.by_query("Москва")
+    gm = aiopygismeteo.Gismeteo()
+    search_results = await gm.search.by_query("Москва")
     city_id = search_results[0].id
-    current = await gismeteo.current.by_id(city_id)
+    current = await gm.current.by_id(city_id)
     print(current.temperature.air.c)
 
 
 asyncio.run(main())
 ```
 
 ## License / Лицензия
```

