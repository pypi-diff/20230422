# Comparing `tmp/pywttr-2.1.0.tar.gz` & `tmp/pywttr-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywttr-2.1.0.tar", max compression
+gzip compressed data, was "pywttr-2.2.0.tar", max compression
```

## Comparing `pywttr-2.1.0.tar` & `pywttr-2.2.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1065 2022-11-26 18:29:40.271043 pywttr-2.1.0/LICENSE
--rw-r--r--   0        0        0     1494 2022-11-26 18:29:40.271043 pywttr-2.1.0/README.md
--rw-r--r--   0        0        0     2783 2022-11-26 19:54:13.969700 pywttr-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      129 2022-11-26 18:29:40.272043 pywttr-2.1.0/pywttr/__init__.py
--rw-r--r--   0        0        0     5069 2022-11-26 19:26:53.956255 pywttr-2.1.0/pywttr/_wttr.py
--rw-r--r--   0        0        0        0 2022-11-26 18:29:40.272043 pywttr-2.1.0/pywttr/py.typed
--rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 pywttr-2.1.0/setup.py
--rw-r--r--   0        0        0     2475 1970-01-01 00:00:00.000000 pywttr-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-20 07:24:52.970123 pywttr-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1612 2023-04-22 20:08:26.179262 pywttr-2.2.0/README.md
+-rw-r--r--   0        0        0     2982 2023-04-22 20:16:41.419265 pywttr-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-04-22 19:53:35.889252 pywttr-2.2.0/pywttr/__init__.py
+-rw-r--r--   0        0        0     5005 2023-04-20 07:24:52.970123 pywttr-2.2.0/pywttr/_wttr.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:24:52.970123 pywttr-2.2.0/pywttr/py.typed
+-rw-r--r--   0        0        0     3023 1970-01-01 00:00:00.000000 pywttr-2.2.0/PKG-INFO
```

### Comparing `pywttr-2.1.0/LICENSE` & `pywttr-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywttr-2.1.0/pywttr/_wttr.py` & `pywttr-2.2.0/pywttr/_wttr.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from __future__ import annotations
 
 from typing import Any, Optional
 
 import pywttr_models
-from requests import Session
+from requests import Response, Session
 
 
-# pylint: disable-next=too-many-public-methods
 class Wttr:
     """Wrapper for wttr.in weather forecast API."""
 
     __slots__ = ("location", "session")
 
-    def __init__(
-        self, location: str, session: Optional[Session] = None
-    ) -> None:
+    def __init__(self, location: str, session: Optional[Session] = None) -> None:
         self.location = location
         self.session = session
 
-    # pylint: disable=invalid-name
     def af(self) -> pywttr_models.af.Model:
         return pywttr_models.af.Model.parse_obj(self._get_json("af"))
 
     def am(self) -> pywttr_models.am.Model:
         return pywttr_models.am.Model.parse_obj(self._get_json("am"))
 
     def ar(self) -> pywttr_models.ar.Model:
@@ -66,15 +62,15 @@
 
     def hu(self) -> pywttr_models.hu.Model:
         return pywttr_models.hu.Model.parse_obj(self._get_json("hu"))
 
     def ia(self) -> pywttr_models.ia.Model:
         return pywttr_models.ia.Model.parse_obj(self._get_json("ia"))
 
-    def id(self) -> pywttr_models.id.Model:
+    def id(self) -> pywttr_models.id.Model:  # noqa: A003
         return pywttr_models.id.Model.parse_obj(self._get_json("id"))
 
     def it(self) -> pywttr_models.it.Model:
         return pywttr_models.it.Model.parse_obj(self._get_json("it"))
 
     def lt(self) -> pywttr_models.lt.Model:
         return pywttr_models.lt.Model.parse_obj(self._get_json("lt"))
@@ -120,21 +116,21 @@
 
     def zh_cn(self) -> pywttr_models.zh_cn.Model:
         return pywttr_models.zh_cn.Model.parse_obj(self._get_json("zh-cn"))
 
     def zh_tw(self) -> pywttr_models.zh_tw.Model:
         return pywttr_models.zh_tw.Model.parse_obj(self._get_json("zh-tw"))
 
-    # pylint: enable=invalid-name
-    def _fetch(self, lang: str, session: Session) -> Any:
-        with session.get(
-            f"https://wttr.in/{self.location}",
-            params={"format": "j1", "lang": lang},
-        ) as response:
-            response.raise_for_status()
-            return response.json()
-
     def _get_json(self, lang: str) -> Any:
         if isinstance(self.session, Session):
-            return self._fetch(lang, self.session)
-        with Session() as session:
-            return self._fetch(lang, session)
+            response = self._fetch(lang, self.session)
+        else:
+            with Session() as session:
+                response = self._fetch(lang, session)
+        response.raise_for_status()
+        return response.json()
+
+    def _fetch(self, lang: str, session: Session) -> Response:
+        with session.get(
+            f"https://wttr.in/{self.location}", params={"format": "j1", "lang": lang}
+        ) as response:
+            return response
```

### Comparing `pywttr-2.1.0/setup.py` & `pywttr-2.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,45 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# pywttr
 
-packages = \
-['pywttr']
+[![CI](https://github.com/monosans/pywttr/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/pywttr/actions/workflows/ci.yml?query=event%3Apush+branch%3Amain)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/pywttr/main.svg)](https://results.pre-commit.ci/latest/github/monosans/pywttr/main)
+[![Coverage](https://img.shields.io/codecov/c/github/monosans/pywttr/main?logo=codecov)](https://codecov.io/gh/monosans/pywttr)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/pywttr?logo=pypi)](https://pypi.org/project/pywttr/)
 
-package_data = \
-{'': ['*']}
+Wrapper for [wttr.in](https://wttr.in) weather forecast API.
 
-install_requires = \
-['pywttr-models>=1.1,<2.0', 'requests>=2.28,<3.0']
-
-setup_kwargs = {
-    'name': 'pywttr',
-    'version': '2.1.0',
-    'description': 'Wrapper for wttr.in API',
-    'long_description': '# pywttr\n\n[![CI](https://github.com/monosans/pywttr/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/pywttr/actions/workflows/ci.yml)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/pywttr/main.svg)](https://results.pre-commit.ci/latest/github/monosans/pywttr/main)\n[![codecov](https://codecov.io/gh/monosans/pywttr/branch/main/graph/badge.svg)](https://codecov.io/gh/monosans/pywttr)\n\nWrapper for [wttr.in](https://wttr.in) weather forecast API.\n\nAsynchronous version [here](https://github.com/monosans/aiopywttr).\n\n## Installation\n\n```bash\npython -m pip install pywttr\n```\n\n## Example\n\nThis example prints the average temperature in New York today.\n\n```python\nfrom pywttr import Wttr\n\nwttr = Wttr("New York")\nforecast = wttr.en()\nprint(forecast.weather[0].avgtemp_c)\n```\n\nOther languages may also be used instead of `en`. For a complete list of supported languages, follow the code completion in your IDE.\n\n## Documentation\n\nThere is no documentation, just follow the code completion in your IDE.\n\nFor an example of type annotations, see `pywttr-models` [README.md](https://github.com/monosans/pywttr-models#usage-for-type-annotation).\n\n## Recommended IDEs\n\n- [Visual Studio Code](https://code.visualstudio.com) (with [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python))\n- [PyCharm](https://jetbrains.com/pycharm)\n\n## License\n\n[MIT](https://github.com/monosans/pywttr/blob/main/LICENSE)\n',
-    'author': 'monosans',
-    'author_email': 'hsyqixco@protonmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/monosans/pywttr',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.2,<4.0.0',
-}
+Asynchronous version [here](https://github.com/monosans/aiopywttr).
 
+## Installation
 
-setup(**setup_kwargs)
+```bash
+python -m pip install -U pywttr pywttr-models
+```
+
+## Example
+
+This example prints the average temperature in New York today.
+
+```python
+import pywttr
+
+wttr = pywttr.Wttr("New York")
+forecast = wttr.en()
+print(forecast.weather[0].avgtemp_c)
+```
+
+Other languages may also be used instead of `en`. For a complete list of supported languages, follow the code completion in your IDE.
+
+## Documentation
+
+There is no documentation, just follow the example and code completion in your IDE.
+
+All types of objects returned by the wttr.in API are in the `pywttr.models` package.
+
+## Recommended IDEs
+
+- [Visual Studio Code](https://code.visualstudio.com) (with [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python))
+- [PyCharm](https://jetbrains.com/pycharm)
+
+## License
+
+[MIT](https://github.com/monosans/pywttr/blob/main/LICENSE)
```

### Comparing `pywttr-2.1.0/PKG-INFO` & `pywttr-2.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,79 @@
 Metadata-Version: 2.1
 Name: pywttr
-Version: 2.1.0
+Version: 2.2.0
 Summary: Wrapper for wttr.in API
 Home-page: https://github.com/monosans/pywttr
 License: MIT
 Keywords: forecast,weather
 Author: monosans
 Author-email: hsyqixco@protonmail.com
 Requires-Python: >=3.7.2,<4.0.0
+Classifier: Environment :: Web Environment
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
 Requires-Dist: pywttr-models (>=1.1,<2.0)
 Requires-Dist: requests (>=2.28,<3.0)
 Project-URL: Repository, https://github.com/monosans/pywttr
 Description-Content-Type: text/markdown
 
 # pywttr
 
-[![CI](https://github.com/monosans/pywttr/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/pywttr/actions/workflows/ci.yml)
+[![CI](https://github.com/monosans/pywttr/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/pywttr/actions/workflows/ci.yml?query=event%3Apush+branch%3Amain)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/pywttr/main.svg)](https://results.pre-commit.ci/latest/github/monosans/pywttr/main)
-[![codecov](https://codecov.io/gh/monosans/pywttr/branch/main/graph/badge.svg)](https://codecov.io/gh/monosans/pywttr)
+[![Coverage](https://img.shields.io/codecov/c/github/monosans/pywttr/main?logo=codecov)](https://codecov.io/gh/monosans/pywttr)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/pywttr?logo=pypi)](https://pypi.org/project/pywttr/)
 
 Wrapper for [wttr.in](https://wttr.in) weather forecast API.
 
 Asynchronous version [here](https://github.com/monosans/aiopywttr).
 
 ## Installation
 
 ```bash
-python -m pip install pywttr
+python -m pip install -U pywttr pywttr-models
 ```
 
 ## Example
 
 This example prints the average temperature in New York today.
 
 ```python
-from pywttr import Wttr
+import pywttr
 
-wttr = Wttr("New York")
+wttr = pywttr.Wttr("New York")
 forecast = wttr.en()
 print(forecast.weather[0].avgtemp_c)
 ```
 
 Other languages may also be used instead of `en`. For a complete list of supported languages, follow the code completion in your IDE.
 
 ## Documentation
 
-There is no documentation, just follow the code completion in your IDE.
+There is no documentation, just follow the example and code completion in your IDE.
 
-For an example of type annotations, see `pywttr-models` [README.md](https://github.com/monosans/pywttr-models#usage-for-type-annotation).
+All types of objects returned by the wttr.in API are in the `pywttr.models` package.
 
 ## Recommended IDEs
 
 - [Visual Studio Code](https://code.visualstudio.com) (with [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python))
 - [PyCharm](https://jetbrains.com/pycharm)
 
 ## License
```

