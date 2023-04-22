# Comparing `tmp/tabularcompare-0.0.2.tar.gz` & `tmp/tabularcompare-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabularcompare-0.0.2.tar", last modified: Thu Apr 20 08:25:28 2023, max compression
+gzip compressed data, was "tabularcompare-0.0.3.tar", last modified: Sat Apr 22 06:12:16 2023, max compression
```

## Comparing `tabularcompare-0.0.2.tar` & `tabularcompare-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/
-drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/.github/
-drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/.github/workflows/
--rw-r--r--   0 erich     (1000) erich     (1000)      844 2023-04-20 04:57:46.000000 tabularcompare-0.0.2/.github/workflows/python-package.yml
--rw-r--r--   0 erich     (1000) erich     (1000)     1901 2023-04-20 03:16:17.000000 tabularcompare-0.0.2/.gitignore
--rw-r--r--   0 erich     (1000) erich     (1000)    11357 2023-04-14 19:34:43.000000 tabularcompare-0.0.2/LICENSE
--rw-r--r--   0 erich     (1000) erich     (1000)      312 2023-04-20 04:59:23.000000 tabularcompare-0.0.2/Makefile
--rw-r--r--   0 erich     (1000) erich     (1000)     7202 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/PKG-INFO
--rw-r--r--   0 erich     (1000) erich     (1000)     6370 2023-04-20 08:20:58.000000 tabularcompare-0.0.2/README.md
--rw-r--r--   0 erich     (1000) erich     (1000)     1358 2023-04-20 08:25:12.000000 tabularcompare-0.0.2/pyproject.toml
--rw-r--r--   0 erich     (1000) erich     (1000)      840 2023-04-20 04:56:50.000000 tabularcompare-0.0.2/requirements.txt
--rw-r--r--   0 erich     (1000) erich     (1000)       38 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/setup.cfg
--rw-r--r--   0 erich     (1000) erich     (1000)       68 2023-04-18 07:14:15.000000 tabularcompare-0.0.2/setup.py
-drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/src/
-drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/src/tabularcompare/
--rw-r--r--   0 erich     (1000) erich     (1000)       69 2023-04-20 08:25:16.000000 tabularcompare-0.0.2/src/tabularcompare/__init__.py
--rw-r--r--   0 erich     (1000) erich     (1000)     4308 2023-04-20 08:08:11.000000 tabularcompare-0.0.2/src/tabularcompare/app.py
--rw-r--r--   0 erich     (1000) erich     (1000)    19210 2023-04-20 06:58:42.000000 tabularcompare-0.0.2/src/tabularcompare/compare.py
--rw-r--r--   0 erich     (1000) erich     (1000)     3397 2023-04-18 08:13:40.000000 tabularcompare-0.0.2/src/tabularcompare/utils.py
-drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/src/tabularcompare.egg-info/
--rw-r--r--   0 erich     (1000) erich     (1000)     7202 2023-04-20 08:25:28.000000 tabularcompare-0.0.2/src/tabularcompare.egg-info/PKG-INFO
--rw-r--r--   0 erich     (1000) erich     (1000)      542 2023-04-20 08:25:28.000000 tabularcompare-0.0.2/src/tabularcompare.egg-info/SOURCES.txt
--rw-r--r--   0 erich     (1000) erich     (1000)        1 2023-04-20 08:25:28.000000 tabularcompare-0.0.2/src/tabularcompare.egg-info/dependency_links.txt
--rw-r--r--   0 erich     (1000) erich     (1000)       58 2023-04-20 08:25:28.000000 tabularcompare-0.0.2/src/tabularcompare.egg-info/entry_points.txt
--rw-r--r--   0 erich     (1000) erich     (1000)      246 2023-04-20 08:25:28.000000 tabularcompare-0.0.2/src/tabularcompare.egg-info/requires.txt
--rw-r--r--   0 erich     (1000) erich     (1000)       15 2023-04-20 08:25:28.000000 tabularcompare-0.0.2/src/tabularcompare.egg-info/top_level.txt
-drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-20 08:25:28.943849 tabularcompare-0.0.2/tests/
--rw-r--r--   0 erich     (1000) erich     (1000)        0 2023-04-18 07:21:18.000000 tabularcompare-0.0.2/tests/__init__.py
--rw-r--r--   0 erich     (1000) erich     (1000)      204 2023-04-18 08:05:33.000000 tabularcompare-0.0.2/tests/test_app.py
--rw-r--r--   0 erich     (1000) erich     (1000)     8295 2023-04-20 07:21:31.000000 tabularcompare-0.0.2/tests/test_compare.py
+drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-22 06:12:16.646200 tabularcompare-0.0.3/
+drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-22 06:12:16.626200 tabularcompare-0.0.3/.github/
+drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-22 06:12:16.636200 tabularcompare-0.0.3/.github/workflows/
+-rw-r--r--   0 erich     (1000) erich     (1000)      844 2023-04-20 04:57:46.000000 tabularcompare-0.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0 erich     (1000) erich     (1000)     1901 2023-04-20 03:16:17.000000 tabularcompare-0.0.3/.gitignore
+-rw-r--r--   0 erich     (1000) erich     (1000)      261 2023-04-22 06:08:51.000000 tabularcompare-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 erich     (1000) erich     (1000)    11357 2023-04-14 19:34:43.000000 tabularcompare-0.0.3/LICENSE
+-rw-r--r--   0 erich     (1000) erich     (1000)      309 2023-04-22 06:08:51.000000 tabularcompare-0.0.3/Makefile
+-rw-r--r--   0 erich     (1000) erich     (1000)     7897 2023-04-22 06:12:16.646200 tabularcompare-0.0.3/PKG-INFO
+-rw-r--r--   0 erich     (1000) erich     (1000)     7066 2023-04-22 06:08:51.000000 tabularcompare-0.0.3/README.md
+-rw-r--r--   0 erich     (1000) erich     (1000)     1383 2023-04-22 06:08:51.000000 tabularcompare-0.0.3/pyproject.toml
+-rw-r--r--   0 erich     (1000) erich     (1000)      840 2023-04-20 04:56:50.000000 tabularcompare-0.0.3/requirements.txt
+-rw-r--r--   0 erich     (1000) erich     (1000)       38 2023-04-22 06:12:16.646200 tabularcompare-0.0.3/setup.cfg
+-rw-r--r--   0 erich     (1000) erich     (1000)       68 2023-04-18 07:14:15.000000 tabularcompare-0.0.3/setup.py
+drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-22 06:12:16.626200 tabularcompare-0.0.3/src/
+drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-22 06:12:16.636200 tabularcompare-0.0.3/src/tabularcompare/
+-rw-r--r--   0 erich     (1000) erich     (1000)       78 2023-04-22 06:08:51.000000 tabularcompare-0.0.3/src/tabularcompare/__init__.py
+-rw-r--r--   0 erich     (1000) erich     (1000)     4486 2023-04-22 06:08:51.000000 tabularcompare-0.0.3/src/tabularcompare/app.py
+-rw-r--r--   0 erich     (1000) erich     (1000)    19368 2023-04-20 08:58:08.000000 tabularcompare-0.0.3/src/tabularcompare/core.py
+-rw-r--r--   0 erich     (1000) erich     (1000)     3421 2023-04-22 06:08:51.000000 tabularcompare-0.0.3/src/tabularcompare/utils.py
+drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-22 06:12:16.646200 tabularcompare-0.0.3/src/tabularcompare.egg-info/
+-rw-r--r--   0 erich     (1000) erich     (1000)     7897 2023-04-22 06:12:16.000000 tabularcompare-0.0.3/src/tabularcompare.egg-info/PKG-INFO
+-rw-r--r--   0 erich     (1000) erich     (1000)      545 2023-04-22 06:12:16.000000 tabularcompare-0.0.3/src/tabularcompare.egg-info/SOURCES.txt
+-rw-r--r--   0 erich     (1000) erich     (1000)        1 2023-04-22 06:12:16.000000 tabularcompare-0.0.3/src/tabularcompare.egg-info/dependency_links.txt
+-rw-r--r--   0 erich     (1000) erich     (1000)       58 2023-04-22 06:12:16.000000 tabularcompare-0.0.3/src/tabularcompare.egg-info/entry_points.txt
+-rw-r--r--   0 erich     (1000) erich     (1000)      262 2023-04-22 06:12:16.000000 tabularcompare-0.0.3/src/tabularcompare.egg-info/requires.txt
+-rw-r--r--   0 erich     (1000) erich     (1000)       15 2023-04-22 06:12:16.000000 tabularcompare-0.0.3/src/tabularcompare.egg-info/top_level.txt
+drwxr-xr-x   0 erich     (1000) erich     (1000)        0 2023-04-22 06:12:16.646200 tabularcompare-0.0.3/tests/
+-rw-r--r--   0 erich     (1000) erich     (1000)      204 2023-04-18 08:05:33.000000 tabularcompare-0.0.3/tests/test_app.py
+-rw-r--r--   0 erich     (1000) erich     (1000)     8234 2023-04-22 04:44:57.000000 tabularcompare-0.0.3/tests/test_compare.py
```

### Comparing `tabularcompare-0.0.2/.github/workflows/python-package.yml` & `tabularcompare-0.0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tabularcompare-0.0.2/.gitignore` & `tabularcompare-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tabularcompare-0.0.2/LICENSE` & `tabularcompare-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tabularcompare-0.0.2/PKG-INFO` & `tabularcompare-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabularcompare
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tabular data comparison wrapper for DataComPy
 Author-email: Erich Henrique <erich.hs13@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/erich-hs/tabularcompare
 Project-URL: Bug Tracker, https://github.com/erich-hs/tabularcompare/issues
 Keywords: Tabular,Compare,Data
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,29 +19,29 @@
 Provides-Extra: qa
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
 
 # TabularCompare
 
-[![Python package](https://github.com/erich-hs/tabularcompare/actions/workflows/python-package.yml/badge.svg)](https://github.com/erich-hs/tabularcompare/actions/workflows/python-package.yml) ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg) [![PyPI license](https://img.shields.io/pypi/l/tabularcompare.svg)](https://pypi.python.org/pypi/tabularcompare/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tabularcompare.svg)](https://pypi.python.org/pypi/tabularcompare/)
+[![Python package](https://github.com/erich-hs/tabularcompare/actions/workflows/python-package.yml/badge.svg)](https://github.com/erich-hs/tabularcompare/actions/workflows/python-package.yml) [![PyPI license](https://img.shields.io/pypi/l/tabularcompare)](https://pypi.python.org/pypi/tabularcompare/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tabularcompare.svg)](https://img.shields.io/pypi/pyversions/tabularcompare) ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 Tabular data comparison wrapper for [DataComPy](https://capitalone.github.io/datacompy/).
 
 ## Quick Install
 ```bash
 pip install tabularcompare
 ```
 
 ## Basic Usage
 
 ### Comparison object
 ```python
 import pandas as pd
-from tabularcompare import compare
+from tabularcompare import Comparison
 
 df1 = pd.DataFrame(
     {
         "idx1": ["A", "B", "B", "C"],
         "idx2": ["01", "01", "02", "03"],
         "colA": ["AA", "BA", "BB", "CA"],
         "colB": [100, 200, 200, 300]
@@ -53,61 +53,80 @@
         "idx2": ["01", "01", "03"],
         "colA": ["AA", "XA", "CA"],
         "colB": [101, 200, 300],
         "colC": ["foo", "bar", "baz"]
      }
 )
 
-comparison = compare.Comparison(
+comparison = Comparison(
     df1, df2, join_columns=["idx1", "idx2"]
 )
 ```
 ### Added Functionalities
-#### Diverging Subset
-This method introduces an enhanced view focused on the changes identified between the dataframes, following the notation ```{df1} --> {df2}```.
+- #### Diverging Subset
+This method introduces an enhanced look at the changes identified at the intersection of compared DataFrames, following the notation ```{df1} --> {df2}```.
 ```python
 comparison.diverging_subset()
 ```
-Will return the following result:
 |   | idx1 | idx2 |          colA |            colB |
 |:-:|-----:|-----:|--------------:|----------------:|
-| 0 | A    | 01   | NaN           | {100} --> {}    |
+| 0 | A    | 01   | NaN           | {100} --> {101} |
 | 1 | B    | 01   | {BA} --> {XA} | NaN             |
 
-#### Enhanced Reporting
+Rows that are unique to either DataFrame can be called via ```.df1_unq_rows()``` and ```.df2_unq_rows()``` methods.
+
+```python
+comparison.df1_unq_rows()
+```
+|   | idx1 | idx2 |	colA | colB |
+|:-:|-----:|-----:|-----:|-----:|
+| 2 |	B  |  02  |  BB  |	200 |
+
+Columns that are unique to either DataFrame can be called via ```.df1_unq_columns()``` and ```.df2_unq_columns()``` methods.
+
+```python
+comparison.df2_unq_columns()
+```
+|   | idx1 | idx2 |	 colC |
+|:-:|-----:|-----:|------:|
+| 0 |	A  |  01  |  foo  |
+| 0 |	B  |  01  |  bar  |
+| 0 |	C  |  03  |  baz  |
+
+- #### Enhanced Reporting
 The report functionality is now callable from the comparison object. It includes a .txt, .html, and .xlsx version.
 ```python
 comparison.report_to_txt("./results/Report.txt")
 comparison.report_to_html("./results/Report.html")
 comparison.report_to_xlsx("./results/Report.xlsx", write_originals=True)
 ```
 The Excel report will output complete comparison results, with tabs dedicated to:
-* Original dataframes (when write_originals=True).
+* Original dataframes (when ```write_originals=True```).
 * Columns present only on df1 and/or df2.
 * Rows present only on df1 and/or df2.
 * Diverging subset showing all the changes identified from df1 to df2.
 
 The HTML report will also output a rendered table of the diverging subset on top of the file, alongside the native DataComPy summary report.
 
-#### [Fully-fledged Command Line Interface](#CLI)
+- #### Fully-fledged [Command Line Interface](#CLI)
 ---
 ### DataComPy Methods
-Most methods native to ```DataComPy.Compare``` functionality are still present, including;
-* .report()
-* .df1_unq_columns()/.df2_unq_columns()
-* .df1_unq_rows()/.df2_unq_rows()
-* .intersect_columns()
-* .intersect_rows()
+Most methods native to ```datacompy.Compare``` functionality are still present, including;
+* ```.report()```
+* ```.df1_unq_rows()``` / ```.df2_unq_rows()```
+* ```.df1_unq_columns()``` / ```.df2_unq_columns()```
+* ```.intersect_columns()```
+* ```.intersect_rows()```
 
-The native ```DataComPy.Compare``` method is also callable from the ```compare``` module via the same import:
+The native ```datacompy.Compare``` method is also callable from the ```tabularcompare``` core module:
 ```python
-from tabularcompare import compare
+from tabularcompare import Compare
 
-# DataComPy.Compare method
-comparison = compare.Compare(
+# datacompy.Compare method
+comparison = Compare(
     df1, df2, join_columns=["idx1", "idx2"]
 )
 print(comparison.report())
 ```
 For a complete documentation on DataComPy you can head to [DataComPy](https://capitalone.github.io/datacompy/).
 
 -----
@@ -128,14 +147,16 @@
                               df1 and df2.
   -n1, --df1_name TEXT        Alias for Data frame 1. Default = df1
   -n2, --df2_name TEXT        Alias for Data frame 2. Default = df2
   -is, --ignore_spaces        Flag to strip and ignore whitespaces from string
                               columns.
   -ci, --case_insensitive     Flag to compare string columns on a case-
                               insensitive manner.
+  -cl, --cast_lowercase       Flag to cast column names to lower case before
+                              comparison.
   -at, --abs_tol FLOAT        Absolute tolerance between two numeric values.
   -rt, --rel_tol FLOAT        Relative tolerance between two numeric values.
   -txt, --txt                 Flag to output a .txt report with a comparison
                               summary.
   -html, --html               Flag to output an HTML report with a comparison
                               summary.
   -od, --only_deltas          Flag to suppress original dataframes from the
@@ -156,15 +177,15 @@
 
 -----
 ## Caveat
 > The comparison results will take into account data types across columns. I.E. If we update our sample dataframe df2 to include a missing value on colB, it will now be of dtype ```object```, as oposed to ```Int64``` in df1. This might lead to miss-leading interpretations of the results to users without information on data types.
 
 ```python
 import pandas as pd
-from tabularcompare import compare
+from tabularcompare import Comparison
 
 df1 = pd.DataFrame(
     {
         "idx1": ["A", "B", "B", "C"],
         "idx2": ["01", "01", "02", "03"],
         "colA": ["AA", "BA", "BB", "CA"],
         "colB": [100, 200, 200, 300]
@@ -176,15 +197,15 @@
         "idx2": ["01", "01", "03"],
         "colA": ["AA", "XA", "CA"],
         "colB": [pd.NA, 200, 300],
         "colC": ["foo", "bar", "baz"]
      }
 )
 
-comparison = compare.Comparison(
+comparison = Comparison(
     df1, df2, join_columns=["idx1", "idx2"]
 )
 comparison.diverging_subset()
 ```
 Which will return:
 |   | idx1 | idx2 |          colA |            colB |
 |:-:|-----:|-----:|--------------:|----------------:|
```

### Comparing `tabularcompare-0.0.2/README.md` & `tabularcompare-0.0.3/src/tabularcompare.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,47 @@
+Metadata-Version: 2.1
+Name: tabularcompare
+Version: 0.0.3
+Summary: Tabular data comparison wrapper for DataComPy
+Author-email: Erich Henrique <erich.hs13@gmail.com>
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/erich-hs/tabularcompare
+Project-URL: Bug Tracker, https://github.com/erich-hs/tabularcompare/issues
+Keywords: Tabular,Compare,Data
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: qa
+Provides-Extra: build
+Provides-Extra: dev
+License-File: LICENSE
+
 # TabularCompare
 
-[![Python package](https://github.com/erich-hs/tabularcompare/actions/workflows/python-package.yml/badge.svg)](https://github.com/erich-hs/tabularcompare/actions/workflows/python-package.yml) ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg) [![PyPI license](https://img.shields.io/pypi/l/tabularcompare.svg)](https://pypi.python.org/pypi/tabularcompare/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tabularcompare.svg)](https://pypi.python.org/pypi/tabularcompare/)
+[![Python package](https://github.com/erich-hs/tabularcompare/actions/workflows/python-package.yml/badge.svg)](https://github.com/erich-hs/tabularcompare/actions/workflows/python-package.yml) [![PyPI license](https://img.shields.io/pypi/l/tabularcompare)](https://pypi.python.org/pypi/tabularcompare/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tabularcompare.svg)](https://img.shields.io/pypi/pyversions/tabularcompare) ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 Tabular data comparison wrapper for [DataComPy](https://capitalone.github.io/datacompy/).
 
 ## Quick Install
 ```bash
 pip install tabularcompare
 ```
 
 ## Basic Usage
 
 ### Comparison object
 ```python
 import pandas as pd
-from tabularcompare import compare
+from tabularcompare import Comparison
 
 df1 = pd.DataFrame(
     {
         "idx1": ["A", "B", "B", "C"],
         "idx2": ["01", "01", "02", "03"],
         "colA": ["AA", "BA", "BB", "CA"],
         "colB": [100, 200, 200, 300]
@@ -30,61 +53,80 @@
         "idx2": ["01", "01", "03"],
         "colA": ["AA", "XA", "CA"],
         "colB": [101, 200, 300],
         "colC": ["foo", "bar", "baz"]
      }
 )
 
-comparison = compare.Comparison(
+comparison = Comparison(
     df1, df2, join_columns=["idx1", "idx2"]
 )
 ```
 ### Added Functionalities
-#### Diverging Subset
-This method introduces an enhanced view focused on the changes identified between the dataframes, following the notation ```{df1} --> {df2}```.
+- #### Diverging Subset
+This method introduces an enhanced look at the changes identified at the intersection of compared DataFrames, following the notation ```{df1} --> {df2}```.
 ```python
 comparison.diverging_subset()
 ```
-Will return the following result:
 |   | idx1 | idx2 |          colA |            colB |
 |:-:|-----:|-----:|--------------:|----------------:|
-| 0 | A    | 01   | NaN           | {100} --> {}    |
+| 0 | A    | 01   | NaN           | {100} --> {101} |
 | 1 | B    | 01   | {BA} --> {XA} | NaN             |
 
-#### Enhanced Reporting
+Rows that are unique to either DataFrame can be called via ```.df1_unq_rows()``` and ```.df2_unq_rows()``` methods.
+
+```python
+comparison.df1_unq_rows()
+```
+|   | idx1 | idx2 |	colA | colB |
+|:-:|-----:|-----:|-----:|-----:|
+| 2 |	B  |  02  |  BB  |	200 |
+
+Columns that are unique to either DataFrame can be called via ```.df1_unq_columns()``` and ```.df2_unq_columns()``` methods.
+
+```python
+comparison.df2_unq_columns()
+```
+|   | idx1 | idx2 |	 colC |
+|:-:|-----:|-----:|------:|
+| 0 |	A  |  01  |  foo  |
+| 0 |	B  |  01  |  bar  |
+| 0 |	C  |  03  |  baz  |
+
+- #### Enhanced Reporting
 The report functionality is now callable from the comparison object. It includes a .txt, .html, and .xlsx version.
 ```python
 comparison.report_to_txt("./results/Report.txt")
 comparison.report_to_html("./results/Report.html")
 comparison.report_to_xlsx("./results/Report.xlsx", write_originals=True)
 ```
 The Excel report will output complete comparison results, with tabs dedicated to:
-* Original dataframes (when write_originals=True).
+* Original dataframes (when ```write_originals=True```).
 * Columns present only on df1 and/or df2.
 * Rows present only on df1 and/or df2.
 * Diverging subset showing all the changes identified from df1 to df2.
 
 The HTML report will also output a rendered table of the diverging subset on top of the file, alongside the native DataComPy summary report.
 
-#### [Fully-fledged Command Line Interface](#CLI)
+- #### Fully-fledged [Command Line Interface](#CLI)
 ---
 ### DataComPy Methods
-Most methods native to ```DataComPy.Compare``` functionality are still present, including;
-* .report()
-* .df1_unq_columns()/.df2_unq_columns()
-* .df1_unq_rows()/.df2_unq_rows()
-* .intersect_columns()
-* .intersect_rows()
+Most methods native to ```datacompy.Compare``` functionality are still present, including;
+* ```.report()```
+* ```.df1_unq_rows()``` / ```.df2_unq_rows()```
+* ```.df1_unq_columns()``` / ```.df2_unq_columns()```
+* ```.intersect_columns()```
+* ```.intersect_rows()```
 
-The native ```DataComPy.Compare``` method is also callable from the ```compare``` module via the same import:
+The native ```datacompy.Compare``` method is also callable from the ```tabularcompare``` core module:
 ```python
-from tabularcompare import compare
+from tabularcompare import Compare
 
-# DataComPy.Compare method
-comparison = compare.Compare(
+# datacompy.Compare method
+comparison = Compare(
     df1, df2, join_columns=["idx1", "idx2"]
 )
 print(comparison.report())
 ```
 For a complete documentation on DataComPy you can head to [DataComPy](https://capitalone.github.io/datacompy/).
 
 -----
@@ -105,14 +147,16 @@
                               df1 and df2.
   -n1, --df1_name TEXT        Alias for Data frame 1. Default = df1
   -n2, --df2_name TEXT        Alias for Data frame 2. Default = df2
   -is, --ignore_spaces        Flag to strip and ignore whitespaces from string
                               columns.
   -ci, --case_insensitive     Flag to compare string columns on a case-
                               insensitive manner.
+  -cl, --cast_lowercase       Flag to cast column names to lower case before
+                              comparison.
   -at, --abs_tol FLOAT        Absolute tolerance between two numeric values.
   -rt, --rel_tol FLOAT        Relative tolerance between two numeric values.
   -txt, --txt                 Flag to output a .txt report with a comparison
                               summary.
   -html, --html               Flag to output an HTML report with a comparison
                               summary.
   -od, --only_deltas          Flag to suppress original dataframes from the
@@ -133,15 +177,15 @@
 
 -----
 ## Caveat
 > The comparison results will take into account data types across columns. I.E. If we update our sample dataframe df2 to include a missing value on colB, it will now be of dtype ```object```, as oposed to ```Int64``` in df1. This might lead to miss-leading interpretations of the results to users without information on data types.
 
 ```python
 import pandas as pd
-from tabularcompare import compare
+from tabularcompare import Comparison
 
 df1 = pd.DataFrame(
     {
         "idx1": ["A", "B", "B", "C"],
         "idx2": ["01", "01", "02", "03"],
         "colA": ["AA", "BA", "BB", "CA"],
         "colB": [100, 200, 200, 300]
@@ -153,18 +197,18 @@
         "idx2": ["01", "01", "03"],
         "colA": ["AA", "XA", "CA"],
         "colB": [pd.NA, 200, 300],
         "colC": ["foo", "bar", "baz"]
      }
 )
 
-comparison = compare.Comparison(
+comparison = Comparison(
     df1, df2, join_columns=["idx1", "idx2"]
 )
 comparison.diverging_subset()
 ```
 Which will return:
 |   | idx1 | idx2 |          colA |            colB |
 |:-:|-----:|-----:|--------------:|----------------:|
 | 0 | A    | 01   | NaN           | {100} --> {}    |
 | 1 | B    | 01   | {BA} --> {XA} | {200} --> {200} |
-| 3 | C    | 03   | NaN           | {300} --> {300} |
+| 3 | C    | 03   | NaN           | {300} --> {300} |
```

### Comparing `tabularcompare-0.0.2/pyproject.toml` & `tabularcompare-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tabularcompare"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Erich Henrique", email="erich.hs13@gmail.com" },
 ]
 description = "Tabular data comparison wrapper for DataComPy"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["Tabular", "Compare", "Data"]
@@ -24,31 +24,33 @@
 dependencies = [
     "numpy<=1.24.2,>=1.11.3",
     "pandas<=1.5.3,>=0.25.0",
     "datacompy<=0.9.0,>=0.8.4",
     "pretty-html-table==0.9.16",
     "click",
     "xlwt",
-    "openpyxl",    
+    "xlrd",
+    "openpyxl",
 ]
 # dynamic = ["version", "readme"]
 
 [project.optional-dependencies]
 tests = ["pytest", "pytest-cov"]
 qa = ["pylint", "black"]
 build = ["build", "twine", "wheel"]
 dev = [
   "pytest",
   "pytest-cov",
   "pylint",
+  "pre-commit",
   "black",
   "build",
   "twine",
   "wheel"
 ]
 
 [project.scripts]
 tabularcompare = "tabularcompare.app:cli"
 
 [project.urls]
 "Homepage" = "https://github.com/erich-hs/tabularcompare"
-"Bug Tracker" = "https://github.com/erich-hs/tabularcompare/issues"
+"Bug Tracker" = "https://github.com/erich-hs/tabularcompare/issues"
```

### Comparing `tabularcompare-0.0.2/requirements.txt` & `tabularcompare-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `tabularcompare-0.0.2/src/tabularcompare/app.py` & `tabularcompare-0.0.3/src/tabularcompare/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import click
-from tabularcompare.utils import (
+from .utils import (
     load_from_file,
     report_to_xlsx,
     report_to_txt,
     report_to_html,
 )
-from tabularcompare.compare import Comparison
+from .core import Comparison
 
 
 @click.command()
 @click.argument("df1", type=click.Path(exists=True), required=True)
 @click.argument("df2", type=click.Path(exists=True), required=True)
 @click.option(
     "-c",
@@ -38,14 +38,20 @@
 @click.option(
     "-ci",
     "--case_insensitive",
     is_flag=True,
     help="Flag to compare string columns on a case-insensitive manner.",
 )
 @click.option(
+    "-cl",
+    "--cast_lowercase",
+    is_flag=True,
+    help="Flag to cast column names to lower case before comparison.",
+)
+@click.option(
     "-at",
     "--abs_tol",
     default=0.0,
     help="Absolute tolerance between two numeric values.",
 )
 @click.option(
     "-rt",
@@ -88,14 +94,15 @@
     df2,
     columns,
     ignore_columns,
     df1_name,
     df2_name,
     ignore_spaces,
     case_insensitive,
+    cast_lowercase,
     abs_tol,
     rel_tol,
     txt,
     html,
     only_deltas,
     output,
     encoding,
@@ -117,15 +124,17 @@
 
     # Join params
     if columns:
         join_columns = [col.strip() for col in columns.split(",")]
         on_index = False
     else:
         if verbose:
-            print("join_columns not provided. Performing comparison on DataFrame indices.")
+            print(
+                "join_columns not provided. Performing comparison on DataFrame indices."
+            )
         join_columns = None
         on_index = True
 
     if ignore_columns:
         ignore_columns = [col.strip() for col in ignore_columns.split(",")]
 
     # Comparison object
@@ -140,15 +149,15 @@
             on_index=on_index,
             abs_tol=abs_tol,
             rel_tol=rel_tol,
             df1_name=df1_name,
             df2_name=df2_name,
             ignore_spaces=ignore_spaces,
             ignore_case=case_insensitive,
-            cast_column_names_lower=False,
+            cast_column_names_lower=cast_lowercase,
         )
     except Exception as e:
         click.echo(click.style(f"{type(e).__name__}: {e}", fg="red"))
         quit(-1)
 
     # Reporting
     report_to_xlsx(comparison, only_deltas, verbose, output)
```

### Comparing `tabularcompare-0.0.2/src/tabularcompare/compare.py` & `tabularcompare-0.0.3/src/tabularcompare/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,18 @@
         df2_unq_rows: Returns a pandas DataFrame with the df2 subset that is unique to df2.
         intersect_columns: Returns a set of columns present in both df1 and df2.
         report_to_txt: Saves datacompy.Compare report in txt.
         report_to_html: Saves datacompy.Compare report in HTML.
         report_to_xlsx: Saves a .xlsx report with the diverging subset, unique columns, and unique rows to df1 and df2.
     """
 
+    # TODO:
+    # 1. Handle case when df1 has column completely missing and df2 doesn't.
+    #   TypeError: boolean value of NA is ambiguous
+
     def __init__(
         self,
         df1: pd.DataFrame,
         df2: pd.DataFrame,
         join_columns: Union[list, str] = None,
         ignore_columns: Union[list, str] = None,
         on_index: bool = False,
@@ -335,15 +339,15 @@
             file_location (str, optional): Destination file path. Default = current directory '.'.
         """
         if not file_name.endswith(".html"):
             file_name += ".html"
         file_path = os.path.join(file_location, file_name)
         col_widths = []
         for col in self._diverging_subset_df.columns:
-            col_max_length = self._diverging_subset_df[col].str.len().max()
+            col_max_length = self._diverging_subset_df[col].astype(str).str.len().max()
             col_width = "auto" if col_max_length < 25 else "160px"
             col_widths.append(col_width)
         html_table_rows = self._diverging_subset_df.index[:max_diverging_records]
         html_table_cols = self._diverging_subset_df.columns[:max_diverging_columns]
         html_table = self._diverging_subset_df.loc[html_table_rows, html_table_cols]
         html_table = build_table(
             html_table,
```

### Comparing `tabularcompare-0.0.2/src/tabularcompare/utils.py` & `tabularcompare-0.0.3/src/tabularcompare/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         except Exception as e:
             click.echo(click.style(f"{type(e).__name__}: {e}", fg="red"))
 
     return inner_func
 
 
 @decoding_handler
+@cli_exception_handler
 def load_from_file(file: str, encoding: Union[str, None] = None) -> pd.DataFrame:
     if file.endswith(".csv"):
         df = pd.read_csv(file, encoding=encoding)
     elif file.endswith(".json"):
         df = pd.read_json(file, encoding=encoding)
     elif file.endswith(".xlsx") or file.endswith(".xls"):
         df = pd.read_excel(file)
```

### Comparing `tabularcompare-0.0.2/src/tabularcompare.egg-info/PKG-INFO` & `tabularcompare-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,24 @@
-Metadata-Version: 2.1
-Name: tabularcompare
-Version: 0.0.2
-Summary: Tabular data comparison wrapper for DataComPy
-Author-email: Erich Henrique <erich.hs13@gmail.com>
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/erich-hs/tabularcompare
-Project-URL: Bug Tracker, https://github.com/erich-hs/tabularcompare/issues
-Keywords: Tabular,Compare,Data
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: qa
-Provides-Extra: build
-Provides-Extra: dev
-License-File: LICENSE
-
 # TabularCompare
 
-[![Python package](https://github.com/erich-hs/tabularcompare/actions/workflows/python-package.yml/badge.svg)](https://github.com/erich-hs/tabularcompare/actions/workflows/python-package.yml) ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg) [![PyPI license](https://img.shields.io/pypi/l/tabularcompare.svg)](https://pypi.python.org/pypi/tabularcompare/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tabularcompare.svg)](https://pypi.python.org/pypi/tabularcompare/)
+[![Python package](https://github.com/erich-hs/tabularcompare/actions/workflows/python-package.yml/badge.svg)](https://github.com/erich-hs/tabularcompare/actions/workflows/python-package.yml) [![PyPI license](https://img.shields.io/pypi/l/tabularcompare)](https://pypi.python.org/pypi/tabularcompare/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tabularcompare.svg)](https://img.shields.io/pypi/pyversions/tabularcompare) ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 Tabular data comparison wrapper for [DataComPy](https://capitalone.github.io/datacompy/).
 
 ## Quick Install
 ```bash
 pip install tabularcompare
 ```
 
 ## Basic Usage
 
 ### Comparison object
 ```python
 import pandas as pd
-from tabularcompare import compare
+from tabularcompare import Comparison
 
 df1 = pd.DataFrame(
     {
         "idx1": ["A", "B", "B", "C"],
         "idx2": ["01", "01", "02", "03"],
         "colA": ["AA", "BA", "BB", "CA"],
         "colB": [100, 200, 200, 300]
@@ -53,61 +30,80 @@
         "idx2": ["01", "01", "03"],
         "colA": ["AA", "XA", "CA"],
         "colB": [101, 200, 300],
         "colC": ["foo", "bar", "baz"]
      }
 )
 
-comparison = compare.Comparison(
+comparison = Comparison(
     df1, df2, join_columns=["idx1", "idx2"]
 )
 ```
 ### Added Functionalities
-#### Diverging Subset
-This method introduces an enhanced view focused on the changes identified between the dataframes, following the notation ```{df1} --> {df2}```.
+- #### Diverging Subset
+This method introduces an enhanced look at the changes identified at the intersection of compared DataFrames, following the notation ```{df1} --> {df2}```.
 ```python
 comparison.diverging_subset()
 ```
-Will return the following result:
 |   | idx1 | idx2 |          colA |            colB |
 |:-:|-----:|-----:|--------------:|----------------:|
-| 0 | A    | 01   | NaN           | {100} --> {}    |
+| 0 | A    | 01   | NaN           | {100} --> {101} |
 | 1 | B    | 01   | {BA} --> {XA} | NaN             |
 
-#### Enhanced Reporting
+Rows that are unique to either DataFrame can be called via ```.df1_unq_rows()``` and ```.df2_unq_rows()``` methods.
+
+```python
+comparison.df1_unq_rows()
+```
+|   | idx1 | idx2 |	colA | colB |
+|:-:|-----:|-----:|-----:|-----:|
+| 2 |	B  |  02  |  BB  |	200 |
+
+Columns that are unique to either DataFrame can be called via ```.df1_unq_columns()``` and ```.df2_unq_columns()``` methods.
+
+```python
+comparison.df2_unq_columns()
+```
+|   | idx1 | idx2 |	 colC |
+|:-:|-----:|-----:|------:|
+| 0 |	A  |  01  |  foo  |
+| 0 |	B  |  01  |  bar  |
+| 0 |	C  |  03  |  baz  |
+
+- #### Enhanced Reporting
 The report functionality is now callable from the comparison object. It includes a .txt, .html, and .xlsx version.
 ```python
 comparison.report_to_txt("./results/Report.txt")
 comparison.report_to_html("./results/Report.html")
 comparison.report_to_xlsx("./results/Report.xlsx", write_originals=True)
 ```
 The Excel report will output complete comparison results, with tabs dedicated to:
-* Original dataframes (when write_originals=True).
+* Original dataframes (when ```write_originals=True```).
 * Columns present only on df1 and/or df2.
 * Rows present only on df1 and/or df2.
 * Diverging subset showing all the changes identified from df1 to df2.
 
 The HTML report will also output a rendered table of the diverging subset on top of the file, alongside the native DataComPy summary report.
 
-#### [Fully-fledged Command Line Interface](#CLI)
+- #### Fully-fledged [Command Line Interface](#CLI)
 ---
 ### DataComPy Methods
-Most methods native to ```DataComPy.Compare``` functionality are still present, including;
-* .report()
-* .df1_unq_columns()/.df2_unq_columns()
-* .df1_unq_rows()/.df2_unq_rows()
-* .intersect_columns()
-* .intersect_rows()
+Most methods native to ```datacompy.Compare``` functionality are still present, including;
+* ```.report()```
+* ```.df1_unq_rows()``` / ```.df2_unq_rows()```
+* ```.df1_unq_columns()``` / ```.df2_unq_columns()```
+* ```.intersect_columns()```
+* ```.intersect_rows()```
 
-The native ```DataComPy.Compare``` method is also callable from the ```compare``` module via the same import:
+The native ```datacompy.Compare``` method is also callable from the ```tabularcompare``` core module:
 ```python
-from tabularcompare import compare
+from tabularcompare import Compare
 
-# DataComPy.Compare method
-comparison = compare.Compare(
+# datacompy.Compare method
+comparison = Compare(
     df1, df2, join_columns=["idx1", "idx2"]
 )
 print(comparison.report())
 ```
 For a complete documentation on DataComPy you can head to [DataComPy](https://capitalone.github.io/datacompy/).
 
 -----
@@ -128,14 +124,16 @@
                               df1 and df2.
   -n1, --df1_name TEXT        Alias for Data frame 1. Default = df1
   -n2, --df2_name TEXT        Alias for Data frame 2. Default = df2
   -is, --ignore_spaces        Flag to strip and ignore whitespaces from string
                               columns.
   -ci, --case_insensitive     Flag to compare string columns on a case-
                               insensitive manner.
+  -cl, --cast_lowercase       Flag to cast column names to lower case before
+                              comparison.
   -at, --abs_tol FLOAT        Absolute tolerance between two numeric values.
   -rt, --rel_tol FLOAT        Relative tolerance between two numeric values.
   -txt, --txt                 Flag to output a .txt report with a comparison
                               summary.
   -html, --html               Flag to output an HTML report with a comparison
                               summary.
   -od, --only_deltas          Flag to suppress original dataframes from the
@@ -156,15 +154,15 @@
 
 -----
 ## Caveat
 > The comparison results will take into account data types across columns. I.E. If we update our sample dataframe df2 to include a missing value on colB, it will now be of dtype ```object```, as oposed to ```Int64``` in df1. This might lead to miss-leading interpretations of the results to users without information on data types.
 
 ```python
 import pandas as pd
-from tabularcompare import compare
+from tabularcompare import Comparison
 
 df1 = pd.DataFrame(
     {
         "idx1": ["A", "B", "B", "C"],
         "idx2": ["01", "01", "02", "03"],
         "colA": ["AA", "BA", "BB", "CA"],
         "colB": [100, 200, 200, 300]
@@ -176,15 +174,15 @@
         "idx2": ["01", "01", "03"],
         "colA": ["AA", "XA", "CA"],
         "colB": [pd.NA, 200, 300],
         "colC": ["foo", "bar", "baz"]
      }
 )
 
-comparison = compare.Comparison(
+comparison = Comparison(
     df1, df2, join_columns=["idx1", "idx2"]
 )
 comparison.diverging_subset()
 ```
 Which will return:
 |   | idx1 | idx2 |          colA |            colB |
 |:-:|-----:|-----:|--------------:|----------------:|
```

### Comparing `tabularcompare-0.0.2/tests/test_compare.py` & `tabularcompare-0.0.3/tests/test_compare.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 import numpy as np
 import pandas as pd
-from tabularcompare import compare
+from tabularcompare import Comparison
 
 # Test parameters
 @pytest.fixture
 def create_test_data():
     df1 = pd.DataFrame(
         {"idx1": [1, 1, 2, 3, 3, 4],
         "idx2": ["A", "B", "A", "A", "B", "A"],
@@ -30,49 +30,49 @@
     df2["dob"] = pd.to_datetime(df2["dob"])
     join_columns = ["idx1", "idx2"]
     return df1, df2, join_columns
 
 def test_report(create_test_data: tuple):
     expected_partial_report = 'DataComPy Comparison\n--------------------\n\nDataFrame Summary\n-----------------\n\n  DataFrame  Columns  Rows\n0       df1        8     6\n1       df2        8     6\n\nColumn Summary\n--------------\n\nNumber of columns in common: 8\nNumber of columns in df1 but not in df2: 0\nNumber of columns in df2 but not in df1: 0\n\nRow Summary\n-----------\n\nMatched on: idx1, idx2\nAny duplicates on match values: Yes\nAbsolute Tolerance: 0\nRelative Tolerance: 0\nNumber of rows in common: 5\nNumber of rows in df1 but not in df2: 1\nNumber of rows in df2 but not in df1: 1\n\nNumber of rows with some compared columns unequal: 3\nNumber of rows with all compared columns equal: 2\n\nColumn Comparison\n-----------------\n\nNumber of columns compared with some values unequal: 2\nNumber of columns compared with all values equal: 6\nTotal number of values which compare unequal: 4\n\nColumns with Unequal Values or Types\n------------------------------------'
     df1, df2, join_columns = create_test_data
-    comparison = compare.Comparison(df1, df2, join_columns)
+    comparison = Comparison(df1, df2, join_columns)
     report = comparison.report()
     assert expected_partial_report in report
 
 def test_diverging_subset(create_test_data: tuple):
     expected_diverging_subset = pd.DataFrame(
     {'idx1': {0: 1, 1: 1, 3: 3},
      'idx2': {0: 'A', 1: 'B', 3: 'A'},
      'fname': {0: '{Nikola} --> {Nick}', 1: '{Nikola} --> {Nick}', 3: np.nan},
      'dob': {0: np.nan,
              1: '{1856-07-10} --> {NaT}',
              3: '{1942-01-08} --> {1942-03-08}'}}
     )
     df1, df2, join_columns = create_test_data
-    comparison = compare.Comparison(df1, df2, join_columns)
+    comparison = Comparison(df1, df2, join_columns)
     diverging_subset = comparison.diverging_subset()
     assert diverging_subset.equals(expected_diverging_subset)
 
 def test_df1_unq_columns(create_test_data: tuple):
     expected_df1_unq_columns = pd.DataFrame(
     {'idx1': {0: 1, 1: 1, 2: 2, 3: 3, 4: 3, 5: 4},
      'idx2': {0: 'A', 1: 'B', 2: 'A', 3: 'A', 4: 'B', 5: 'A'}}
     )
     df1, df2, join_columns = create_test_data
-    comparison = compare.Comparison(df1, df2, join_columns)
+    comparison = Comparison(df1, df2, join_columns)
     df1_unq_columns = comparison.df1_unq_columns()
     assert df1_unq_columns.equals(expected_df1_unq_columns)
 
 def test_df2_unq_columns(create_test_data: tuple):
     expected_df2_unq_columns = pd.DataFrame(
     {'idx1': {0: 1, 1: 1, 2: 2, 3: 3, 4: 3, 5: 2},
      'idx2': {0: 'A', 1: 'B', 2: 'A', 3: 'A', 4: 'B', 5: 'A'}}
     )
     df1, df2, join_columns = create_test_data
-    comparison = compare.Comparison(df1, df2, join_columns)
+    comparison = Comparison(df1, df2, join_columns)
     df2_unq_columns = comparison.df2_unq_columns()
     assert df2_unq_columns.equals(expected_df2_unq_columns)
 
 def test_df1_unq_rows(create_test_data: tuple):
     expected_df1_unq_rows = pd.DataFrame(
     {'idx1': {5: 4},
      'idx2': {5: 'A'},
@@ -80,15 +80,15 @@
      'lname': {5: 'Jobs'},
      'emptycol': {5: ""},
      'email': {5: 'sj@apple.com'},
      'dob': {5: pd.Timestamp('1955-02-24 00:00:00')},
      'active': {5: True}}
     )
     df1, df2, join_columns = create_test_data
-    comparison = compare.Comparison(df1, df2, join_columns)
+    comparison = Comparison(df1, df2, join_columns)
     df1_unq_rows = comparison.df1_unq_rows().fillna("")
     assert df1_unq_rows.equals(expected_df1_unq_rows)
 
 def test_df2_unq_rows(create_test_data: tuple):
     expected_df2_unq_rows = pd.DataFrame(
     {'idx1': {6: 2},
      'idx2': {6: 'A'},
@@ -96,22 +96,22 @@
      'lname': {6: 'Einstein'},
      'emptycol': {6: ""},
      'email': {6: 'ae@hotmail.com'},
      'dob': {6: pd.Timestamp('1879-03-14 00:00:00')},
      'active': {6: ""}}
     )
     df1, df2, join_columns = create_test_data
-    comparison = compare.Comparison(df1, df2, join_columns)
+    comparison = Comparison(df1, df2, join_columns)
     df2_unq_rows = comparison.df2_unq_rows().fillna("")
     assert df2_unq_rows.equals(expected_df2_unq_rows)
 
 def test_intersect_columns(create_test_data: tuple):
     expected_intersect_columns = ['idx1', 'idx2', 'fname', 'lname', 'emptycol', 'email', 'dob', 'active']
     df1, df2, join_columns = create_test_data
-    comparison = compare.Comparison(df1, df2, join_columns)
+    comparison = Comparison(df1, df2, join_columns)
     intersect_columns = comparison.intersect_columns()
     assert intersect_columns == expected_intersect_columns
 
 def test_intersect_rows(create_test_data: tuple):
     expected_intersect_rows = pd.DataFrame({
         'idx1': {0: 1, 1: 1, 2: 2, 3: 3, 4: 3},
         'idx2': {0: 'A', 1: 'B', 2: 'A', 3: 'A', 4: 'B'},
@@ -160,13 +160,13 @@
         'lname_match': {0: True, 1: True, 2: True, 3: True, 4: True},
         'emptycol_match': {0: True, 1: True, 2: True, 3: True, 4: True},
         'email_match': {0: True, 1: True, 2: True, 3: True, 4: True},
         'dob_match': {0: True, 1: False, 2: True, 3: False, 4: True},
         'active_match': {0: True, 1: True, 2: True, 3: True, 4: True}
     })
     df1, df2, join_columns = create_test_data
-    comparison = compare.Comparison(df1, df2, join_columns)
+    comparison = Comparison(df1, df2, join_columns)
     intersect_rows = comparison.intersect_rows().fillna("")
     dtime_cols = intersect_rows.select_dtypes(include=['datetime'])
     intersect_rows[dtime_cols.columns] = dtime_cols.fillna(pd.to_datetime('2000-01-01'))
     intersect_rows["_merge"] = intersect_rows["_merge"].astype("object")
     assert intersect_rows.equals(expected_intersect_rows)
```

