# Comparing `tmp/soccerdata-1.3.4.tar.gz` & `tmp/soccerdata-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soccerdata-1.3.4.tar", max compression
+gzip compressed data, was "soccerdata-1.3.5.tar", max compression
```

## Comparing `soccerdata-1.3.4.tar` & `soccerdata-1.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1384 2023-03-11 22:22:40.897797 soccerdata-1.3.4/LICENSE.rst
--rw-r--r--   0        0        0     3130 2023-03-11 22:22:40.897797 soccerdata-1.3.4/README.rst
--rw-r--r--   0        0        0     2353 2023-03-11 22:22:52.393596 soccerdata-1.3.4/pyproject.toml
--rw-r--r--   0        0        0      457 2023-03-11 22:22:52.393596 soccerdata-1.3.4/soccerdata/__init__.py
--rw-r--r--   0        0        0    20112 2023-03-11 22:22:40.905796 soccerdata-1.3.4/soccerdata/_common.py
--rw-r--r--   0        0        0     5144 2023-03-11 22:22:40.905796 soccerdata-1.3.4/soccerdata/_config.py
--rw-r--r--   0        0        0     6218 2023-03-11 22:22:40.905796 soccerdata-1.3.4/soccerdata/clubelo.py
--rw-r--r--   0        0        0    12693 2023-03-11 22:22:40.905796 soccerdata-1.3.4/soccerdata/espn.py
--rw-r--r--   0        0        0    30230 2023-03-11 22:22:40.905796 soccerdata-1.3.4/soccerdata/fbref.py
--rw-r--r--   0        0        0     8584 2023-03-11 22:22:40.905796 soccerdata-1.3.4/soccerdata/fivethirtyeight.py
--rw-r--r--   0        0        0     4397 2023-03-11 22:22:40.905796 soccerdata-1.3.4/soccerdata/match_history.py
--rw-r--r--   0        0        0     9712 2023-03-11 22:22:40.905796 soccerdata-1.3.4/soccerdata/sofifa.py
--rw-r--r--   0        0        0    32302 2023-03-11 22:22:40.905796 soccerdata-1.3.4/soccerdata/whoscored.py
--rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 soccerdata-1.3.4/setup.py
--rw-r--r--   0        0        0     4471 1970-01-01 00:00:00.000000 soccerdata-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1384 2023-04-22 09:17:56.031795 soccerdata-1.3.5/LICENSE.rst
+-rw-r--r--   0        0        0     3130 2023-04-22 09:17:56.031795 soccerdata-1.3.5/README.rst
+-rw-r--r--   0        0        0     2352 2023-04-22 09:18:08.391831 soccerdata-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0      457 2023-04-22 09:18:08.391831 soccerdata-1.3.5/soccerdata/__init__.py
+-rw-r--r--   0        0        0    20126 2023-04-22 09:17:56.039795 soccerdata-1.3.5/soccerdata/_common.py
+-rw-r--r--   0        0        0     5144 2023-04-22 09:17:56.039795 soccerdata-1.3.5/soccerdata/_config.py
+-rw-r--r--   0        0        0     6218 2023-04-22 09:17:56.039795 soccerdata-1.3.5/soccerdata/clubelo.py
+-rw-r--r--   0        0        0    12693 2023-04-22 09:17:56.039795 soccerdata-1.3.5/soccerdata/espn.py
+-rw-r--r--   0        0        0    30578 2023-04-22 09:17:56.039795 soccerdata-1.3.5/soccerdata/fbref.py
+-rw-r--r--   0        0        0     8584 2023-04-22 09:17:56.043794 soccerdata-1.3.5/soccerdata/fivethirtyeight.py
+-rw-r--r--   0        0        0     4547 2023-04-22 09:17:56.043794 soccerdata-1.3.5/soccerdata/match_history.py
+-rw-r--r--   0        0        0     9712 2023-04-22 09:17:56.043794 soccerdata-1.3.5/soccerdata/sofifa.py
+-rw-r--r--   0        0        0    32302 2023-04-22 09:17:56.043794 soccerdata-1.3.5/soccerdata/whoscored.py
+-rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 soccerdata-1.3.5/setup.py
+-rw-r--r--   0        0        0     4471 1970-01-01 00:00:00.000000 soccerdata-1.3.5/PKG-INFO
```

### Comparing `soccerdata-1.3.4/LICENSE.rst` & `soccerdata-1.3.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.4/README.rst` & `soccerdata-1.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.4/pyproject.toml` & `soccerdata-1.3.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "soccerdata"
-version = "1.3.4"
+version = "1.3.5"
 description = "A collection of wrappers over soccer data from various websites / APIs."
 authors = ["Pieter Robberechts <pieter.robberechts@kuleuven.be>"]
 license = "Apache-2.0"
 readme = 'README.rst'
 homepage = "https://github.com/probberechts/soccerdata"
 repository = "https://github.com/probberechts/soccerdata"
 keywords = ["soccer", "football", "soccer data", "web scraping", "soccer analytics"]
@@ -33,29 +33,29 @@
 mypy = "^1.0"
 pylint = "^2.15.5"
 pytest-deadfixtures = "^2.2.1"
 unify = "^0.5"
 black = "^23.0.0"
 Sphinx = "^6.0.0"
 sphinx-autobuild = "^2021.3.14"
-furo = "^2022.9.29"
+furo = "^2023.0.0"
 coverage = {version = "^7.0", extras = ["toml"]}
 pre-commit = "^3.0.0"
 flake8 = "^6.0.0"
 flake8-bugbear = "^23.0.0"
 flake8-docstrings = "^1.6.0"
 flake8-rst-docstrings = "^0.3.0"
 pep8-naming = "^0.13.2"
 darglint = "^1.8.1"
 pre-commit-hooks = "^4.3.0"
 Pygments = "^2.13.0"
 time-machine = "^2.8.2"
 pytest-mock = "^3.10.0"
 bumpversion = "^0.6.0"
-nbsphinx = "^0.8.8"
+nbsphinx = "^0.9.0"
 
 [tool.isort]
 profile = "black"
 src_paths = ["soccerdata", "tests"]
 balanced_wrapping = true
 default_section = "THIRDPARTY"
 include_trailing_comma = true
```

### Comparing `soccerdata-1.3.4/soccerdata/_common.py` & `soccerdata-1.3.5/soccerdata/_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,15 +455,15 @@
 
     if re.match(pat1, season):
         if int(season[2:]) == int(season[:2]) + 1:
             if season == "2021":
                 msg = 'Season id "{}" is ambiguous: interpreting as "{}-{}"'.format(
                     season, season[:2], season[-2:]
                 )
-                warnings.warn(msg)
+                warnings.warn(msg, stacklevel=1)
             return season  # 9495
         elif season[2:] == "99":
             return "".join([season[2:], "00"])  # 1999
         else:
             return "".join([season[-2:], f"{int(season[-2:]) + 1:02d}"])  # 1994
     elif re.match(pat2, season):
         if season == "99":
```

### Comparing `soccerdata-1.3.4/soccerdata/_config.py` & `soccerdata-1.3.5/soccerdata/_config.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.4/soccerdata/clubelo.py` & `soccerdata-1.3.5/soccerdata/clubelo.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.4/soccerdata/espn.py` & `soccerdata-1.3.5/soccerdata/espn.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.4/soccerdata/fbref.py` & `soccerdata-1.3.5/soccerdata/fbref.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Scraper for http://fbref.com."""
 import itertools
 import warnings
+from datetime import date, datetime
 from functools import reduce
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Union
 
 import pandas as pd
 from lxml import etree, html
 
@@ -85,20 +86,20 @@
             no_cache=no_cache,
             no_store=no_store,
             data_dir=data_dir,
         )
         self.rate_limit = 3
         self.seasons = seasons  # type: ignore
         # check if all top 5 leagues are selected
-        selected_leagues = set(self._leagues_dict.keys())
-        if set(BIG_FIVE_DICT.values()).issubset(selected_leagues):
+        if set(BIG_FIVE_DICT.values()).issubset(self.leagues):
             warnings.warn(
                 "You are trying to scrape data for all of the Big 5 European leagues. "
                 "This can be done more efficiently by setting "
-                "leagues='Big 5 European Leagues Combined'."
+                "leagues='Big 5 European Leagues Combined'.",
+                stacklevel=1,
             )
 
     @property
     def leagues(self) -> List[str]:
         """Return a list of selected leagues."""
         selected_leagues = set(self._leagues_dict.keys())
         if "Big 5 European Leagues Combined" in selected_leagues:
@@ -108,14 +109,21 @@
     @classmethod
     def _all_leagues(cls) -> Dict[str, str]:
         """Return a dict mapping all canonical league IDs to source league IDs."""
         res = super()._all_leagues()
         res.update({"Big 5 European Leagues Combined": "Big 5 European Leagues Combined"})
         return res
 
+    def _is_complete(self, league: str, season: str) -> bool:
+        """Check if a season is complete."""
+        if league == "Big 5 European Leagues Combined":
+            season_ends = date(datetime.strptime(season[-2:], "%y").year, 7, 1)
+            return date.today() >= season_ends
+        return super()._is_complete(league, season)
+
     def read_leagues(self) -> pd.DataFrame:
         """Retrieve selected leagues from the datasource.
 
         Returns
         -------
         pd.DataFrame
         """
```

### Comparing `soccerdata-1.3.4/soccerdata/fivethirtyeight.py` & `soccerdata-1.3.5/soccerdata/fivethirtyeight.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.4/soccerdata/match_history.py` & `soccerdata-1.3.5/soccerdata/match_history.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,20 +89,22 @@
         df_list = []
         for lkey, skey in itertools.product(self._selected_leagues.values(), self.seasons):
             filepath = self.data_dir / filemask.format(lkey, skey)
             url = urlmask.format(skey, lkey)
             current_season = not self._is_complete(lkey, skey)
             reader = self.get(url, filepath, no_cache=current_season)
 
-            df_list.append(
-                pd.read_csv(
-                    reader,
-                    encoding='ISO-8859-1',
-                ).assign(season=skey)
-            )
+            df_games = pd.read_csv(
+                reader,
+                encoding='ISO-8859-1',
+            ).assign(season=skey)
+            if 'Time' not in df_games.columns:
+                df_games['Time'] = "12:00:00"
+            df_games["Time"] = df_games["Time"].fillna("12:00:00")
+            df_list.append(df_games)
 
         df = (
             pd.concat(df_list, sort=False)
             .rename(columns=col_rename)
             .assign(date=lambda x: pd.to_datetime(x["date"] + ' ' + x['time']))
             .drop("time", axis=1)
             .pipe(self._translate_league)
```

### Comparing `soccerdata-1.3.4/soccerdata/sofifa.py` & `soccerdata-1.3.5/soccerdata/sofifa.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.4/soccerdata/whoscored.py` & `soccerdata-1.3.5/soccerdata/whoscored.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.4/setup.py` & `soccerdata-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'rich>=13.0.0,<14.0.0',
  'selenium>=4.0.0,<5.0.0',
  'undetected-chromedriver>=3.1.3,<4.0.0',
  'unicode>=2.7,<3.0']
 
 setup_kwargs = {
     'name': 'soccerdata',
-    'version': '1.3.4',
+    'version': '1.3.5',
     'description': 'A collection of wrappers over soccer data from various websites / APIs.',
     'long_description': ".. image:: https://raw.githubusercontent.com/probberechts/soccerdata/master/docs/_static/logo2.png\n   :align: center\n   :alt: SoccerData\n   :width: 600px\n\n.. badges-begin\n\n|PyPI| |Python Version| |License| |Read the Docs| |Tests| |Codecov| |pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/soccerdata.svg\n   :target: https://pypi.org/project/soccerdata/\n   :alt: PyPI\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/soccerdata\n   :target: https://pypi.org/project/soccerdata\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/pypi/l/soccerdata.svg\n   :target: https://opensource.org/licenses/Apache-2.0\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/soccerdata/latest.svg?label=Read%20the%20Docs\n   :target: https://soccerdata.readthedocs.io/\n   :alt: Read the documentation at https://soccerdata.readthedocs.io/\n.. |Tests| image:: https://github.com/probberechts/soccerdata/workflows/CI/badge.svg\n   :target: https://github.com/probberechts/soccerdata/actions?workflow=CI\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/probberechts/soccerdata/branch/master/graph/badge.svg\n   :target: https://app.codecov.io/gh/probberechts/soccerdata\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n.. badges-end\n\nSoccerData is a collection of wrappers over soccer data from `Club Elo`_,\n`ESPN`_, `FBref`_, `FiveThirtyEight`_, `Football-Data.co.uk`_, `SoFIFA`_ and\n`WhoScored`_. You get Pandas DataFrames with sensible, matching column names\nand identifiers across datasets. Data is downloaded when needed and cached\nlocally.\n\n.. code:: python\n\n   import soccerdata as sd\n\n   # Create scraper class instance for the Premier League\n   five38 = sd.FiveThirtyEight('ENG-Premier League', '1819')\n\n   # Fetch dataframes\n   games = five38.read_games()\n\nTo learn how to install, configure and use SoccerData, see the\n`Quickstart guide <https://soccerdata.readthedocs.io/en/latest/usage.html>`__. For documentation on each of the\nsupported data sources, see the `example notebooks <https://soccerdata.readthedocs.io/en/latest/datasources/>`__ and `API reference <https://soccerdata.readthedocs.io/en/latest/reference/>`__.\n\n.. _Club Elo: https://www.clubelo.com/\n.. _ESPN: https://www.espn.com/soccer/\n.. _FBref: https://www.fbref.com/en/\n.. _FiveThirtyEight: https://fivethirtyeight.com/soccer-predictions/\n.. _Football-Data.co.uk: https://www.football-data.co.uk/\n.. _SoFIFA: https://sofifa.com/\n.. _WhoScored: https://www.whoscored.com/\n\n**Disclaimer:** As soccerdata relies on web scraping, any changes to the\nscraped websites will break the package. Hence, do not expect that all code\nwill work all the time. If you spot any bugs, then please `fork it and start\na pull request <https://github.com/probberechts/soccerdata/blob/master/CONTRIBUTING.rst>`__.\n",
     'author': 'Pieter Robberechts',
     'author_email': 'pieter.robberechts@kuleuven.be',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/probberechts/soccerdata',
```

### Comparing `soccerdata-1.3.4/PKG-INFO` & `soccerdata-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soccerdata
-Version: 1.3.4
+Version: 1.3.5
 Summary: A collection of wrappers over soccer data from various websites / APIs.
 Home-page: https://github.com/probberechts/soccerdata
 License: Apache-2.0
 Keywords: soccer,football,soccer data,web scraping,soccer analytics
 Author: Pieter Robberechts
 Author-email: pieter.robberechts@kuleuven.be
 Requires-Python: >=3.8.1,<4.0.0
```

