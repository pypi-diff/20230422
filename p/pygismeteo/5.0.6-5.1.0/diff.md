# Comparing `tmp/pygismeteo-5.0.6.tar.gz` & `tmp/pygismeteo-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygismeteo-5.0.6.tar", max compression
+gzip compressed data, was "pygismeteo-5.1.0.tar", max compression
```

## Comparing `pygismeteo-5.0.6.tar` & `pygismeteo-5.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-01-30 17:12:08.907209 pygismeteo-5.0.6/LICENSE
--rw-r--r--   0        0        0     1225 2023-01-30 17:12:08.907209 pygismeteo-5.0.6/README.md
--rw-r--r--   0        0        0      135 2023-01-30 17:12:08.908209 pygismeteo-5.0.6/pygismeteo/__init__.py
--rw-r--r--   0        0        0     1388 2023-01-30 17:12:08.908209 pygismeteo-5.0.6/pygismeteo/_current.py
--rw-r--r--   0        0        0     2786 2023-01-30 17:12:08.908209 pygismeteo-5.0.6/pygismeteo/_gismeteo.py
--rw-r--r--   0        0        0     1119 2023-01-30 17:12:08.908209 pygismeteo-5.0.6/pygismeteo/_http.py
--rw-r--r--   0        0        0     1928 2023-01-30 17:30:49.184847 pygismeteo-5.0.6/pygismeteo/_search.py
--rw-r--r--   0        0        0     2453 2023-01-30 17:12:08.908209 pygismeteo-5.0.6/pygismeteo/_step_n.py
--rw-r--r--   0        0        0        0 2023-01-30 17:12:08.908209 pygismeteo-5.0.6/pygismeteo/py.typed
--rw-r--r--   0        0        0     3183 2023-01-30 17:33:27.936132 pygismeteo-5.0.6/pyproject.toml
--rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 pygismeteo-5.0.6/setup.py
--rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 pygismeteo-5.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-19 14:48:31.640689 pygismeteo-5.1.0/LICENSE
+-rw-r--r--   0        0        0     1330 2023-04-21 20:07:41.333689 pygismeteo-5.1.0/README.md
+-rw-r--r--   0        0        0      209 2023-04-21 20:30:00.863662 pygismeteo-5.1.0/pygismeteo/__init__.py
+-rw-r--r--   0        0        0     1356 2023-04-22 09:03:37.506335 pygismeteo-5.1.0/pygismeteo/_current.py
+-rw-r--r--   0        0        0     2818 2023-04-22 09:02:08.356344 pygismeteo-5.1.0/pygismeteo/_gismeteo.py
+-rw-r--r--   0        0        0     1288 2023-04-21 20:13:03.143666 pygismeteo-5.1.0/pygismeteo/_http.py
+-rw-r--r--   0        0        0     3921 2023-04-22 17:44:22.569254 pygismeteo-5.1.0/pygismeteo/_search.py
+-rw-r--r--   0        0        0     4632 2023-04-22 17:48:05.969246 pygismeteo-5.1.0/pygismeteo/_step_n.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:48:31.650689 pygismeteo-5.1.0/pygismeteo/py.typed
+-rw-r--r--   0        0        0      322 2023-04-22 18:14:51.489227 pygismeteo-5.1.0/pygismeteo/types.py
+-rw-r--r--   0        0        0     3132 2023-04-22 19:45:13.249235 pygismeteo-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2837 1970-01-01 00:00:00.000000 pygismeteo-5.1.0/PKG-INFO
```

### Comparing `pygismeteo-5.0.6/LICENSE` & `pygismeteo-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygismeteo-5.0.6/README.md` & `pygismeteo-5.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # pygismeteo
 
-[![CI](https://github.com/monosans/pygismeteo/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/pygismeteo/actions/workflows/ci.yml)
+[![CI](https://github.com/monosans/pygismeteo/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/pygismeteo/actions/workflows/ci.yml?query=event%3Apush+branch%3Amain)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/pygismeteo/main.svg)](https://results.pre-commit.ci/latest/github/monosans/pygismeteo/main)
-[![codecov](https://codecov.io/gh/monosans/pygismeteo/branch/main/graph/badge.svg)](https://codecov.io/gh/monosans/pygismeteo)
+[![Coverage](https://img.shields.io/codecov/c/github/monosans/pygismeteo/main?logo=codecov)](https://codecov.io/gh/monosans/pygismeteo)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/pygismeteo?logo=pypi)](https://pypi.org/project/pygismeteo/)
 
 Обёртка для [Gismeteo API](https://gismeteo.ru/api/).
 
 Асинхронная версия [здесь](https://github.com/monosans/aiopygismeteo).
 
 ## Установка
 
 ```bash
 python -m pip install -U pygismeteo
 ```
 
 ## Документация
 
-[pygismeteo.readthedocs.io](https://pygismeteo.readthedocs.io/)
+<https://pygismeteo.readthedocs.io/>
 
 ## Пример, выводящий температуру в Москве сейчас
 
 ```python
-from pygismeteo import Gismeteo
+import pygismeteo
 
-gismeteo = Gismeteo()
-search_results = gismeteo.search.by_query("Москва")
+gm = pygismeteo.Gismeteo()
+search_results = gm.search.by_query("Москва")
 city_id = search_results[0].id
-current = gismeteo.current.by_id(city_id)
+current = gm.current.by_id(city_id)
 print(current.temperature.air.c)
 ```
 
 ## License / Лицензия
 
 [MIT](https://github.com/monosans/pygismeteo/blob/main/LICENSE)
```

### Comparing `pygismeteo-5.0.6/pygismeteo/_current.py` & `pygismeteo-5.1.0/pygismeteo/_current.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,37 +8,32 @@
 
 
 class Current(CurrentBase[RequestsClient]):
     """Текущая погода."""
 
     __slots__ = ()
 
-    def by_coordinates(
-        self, latitude: float, longitude: float
-    ) -> models.current.Model:
+    def by_coordinates(self, latitude: float, longitude: float) -> models.current.Model:
         """По координатам.
 
         Args:
-            latitude: Широта (от -90 до 90).
-            longitude: Долгота (от -180 до 180).
+            latitude (-90 ≤ float ≤ 90):
+                Широта.
+            longitude (-180 ≤ float ≤ 180):
+                Долгота.
         """
         url, params = self._get_params_by_coordinates(latitude, longitude)
         return self._get_result(url, params=params)
 
-    def by_id(
-        self,
-        # pylint: disable-next=invalid-name,redefined-builtin
-        id: int,
-    ) -> models.current.Model:
+    def by_id(self, id: int) -> models.current.Model:  # noqa: A002
         """По ID географического объекта.
 
         Args:
-            id: ID географического объекта. Получить можно через поиск.
+            id (int >= 1):
+                ID географического объекта. Получить можно через поиск.
         """
         url, params = self._get_params_by_id(id)
         return self._get_result(url, params=params)
 
-    def _get_result(
-        self, url: str, *, params: Params = None
-    ) -> models.current.Model:
+    def _get_result(self, url: str, *, params: Params = None) -> models.current.Model:
         response = self._session.get_response(url, params=params)
         return models.current.Model.parse_obj(response)
```

### Comparing `pygismeteo-5.0.6/pygismeteo/_gismeteo.py` & `pygismeteo-5.1.0/pygismeteo/_gismeteo.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,20 @@
         lang: Optional[Lang] = None,
         token: Optional[str] = None,
         session: Optional[Session] = None,
     ) -> None:
         """Обёртка для Gismeteo API.
 
         Args:
-            lang: язык. По умолчанию "ru".
-            token: X-Gismeteo-Token,
-                если используемый по умолчанию перестал работать.
-            session: экземпляр requests.Session.
+            lang:
+                Язык. По умолчанию "ru".
+            token:
+                X-Gismeteo-Token, если используемый по умолчанию перестал работать.
+            session:
+                Экземпляр requests.Session.
                 По умолчанию для каждого запроса создаётся новый экземпляр.
         """
         self._settings = Settings(lang=lang, token=token)
         self._session = RequestsClient(session, self._settings)
         self._current = Current(self._session)
         self._step3 = Step3(self._session)
         self._step6 = Step6(self._session)
```

