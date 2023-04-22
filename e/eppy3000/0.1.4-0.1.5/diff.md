# Comparing `tmp/eppy3000-0.1.4.tar.gz` & `tmp/eppy3000-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eppy3000-0.1.4.tar", last modified: Thu Jul  9 19:02:45 2020, max compression
+gzip compressed data, was "eppy3000-0.1.5.tar", last modified: Sat Apr 22 01:13:13 2023, max compression
```

## Comparing `eppy3000-0.1.4.tar` & `eppy3000-0.1.5.tar`

### file list

```diff
@@ -1,59 +1,84 @@
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/
--rw-r--r--   0 santoshphilip   (501) staff       (20)      118 2020-04-07 19:39:27.000000 eppy3000-0.1.4/AUTHORS.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)     1417 2020-04-07 19:39:27.000000 eppy3000-0.1.4/CONTRIBUTING.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)     2241 2020-07-09 18:53:09.000000 eppy3000-0.1.4/HISTORY.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)    16725 2020-04-07 19:39:27.000000 eppy3000-0.1.4/LICENSE
--rw-r--r--   0 santoshphilip   (501) staff       (20)      262 2020-04-07 19:39:27.000000 eppy3000-0.1.4/MANIFEST.in
--rw-r--r--   0 santoshphilip   (501) staff       (20)     9023 2020-07-09 19:02:45.000000 eppy3000-0.1.4/PKG-INFO
--rw-r--r--   0 santoshphilip   (501) staff       (20)     4545 2020-04-07 19:39:27.000000 eppy3000-0.1.4/README.rst
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/docs/
--rw-r--r--   0 santoshphilip   (501) staff       (20)      609 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/Makefile
--rw-r--r--   0 santoshphilip   (501) staff       (20)       28 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/authors.rst
--rwxr-xr-x   0 santoshphilip   (501) staff       (20)     4869 2020-07-09 18:43:53.000000 eppy3000-0.1.4/docs/conf.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)       33 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/contributing.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)      189 2020-07-09 18:43:53.000000 eppy3000-0.1.4/docs/eppy3000.experimental.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)      389 2020-07-09 18:43:53.000000 eppy3000-0.1.4/docs/eppy3000.oldeppy.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)     1280 2020-07-09 18:43:53.000000 eppy3000-0.1.4/docs/eppy3000.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)       28 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/history.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)      346 2020-07-09 18:43:53.000000 eppy3000-0.1.4/docs/index.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)     1138 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/installation.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)      770 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/make.bat
--rw-r--r--   0 santoshphilip   (501) staff       (20)       61 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/modules.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)       27 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/readme.rst
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000/
--rw-r--r--   0 santoshphilip   (501) staff       (20)      154 2020-07-09 18:53:50.000000 eppy3000-0.1.4/eppy3000/__init__.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)     5149 2020-04-07 19:39:27.000000 eppy3000-0.1.4/eppy3000/epMunch.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)       44 2020-04-07 19:39:27.000000 eppy3000-0.1.4/eppy3000/eppy3000.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)     2205 2020-07-09 18:43:53.000000 eppy3000-0.1.4/eppy3000/epschema.py
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000/experimental/
--rw-r--r--   0 santoshphilip   (501) staff       (20)      542 2020-07-09 18:43:53.000000 eppy3000-0.1.4/eppy3000/experimental/__init__.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)      130 2020-07-09 18:43:53.000000 eppy3000-0.1.4/eppy3000/experimental/hello.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)      688 2020-07-09 18:43:53.000000 eppy3000-0.1.4/eppy3000/experimental/listfields.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)     6652 2020-07-09 18:43:53.000000 eppy3000-0.1.4/eppy3000/idfjsonconverter.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)     5387 2020-07-09 18:43:53.000000 eppy3000-0.1.4/eppy3000/modelmaker.py
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000/oldeppy/
--rw-r--r--   0 santoshphilip   (501) staff       (20)     1362 2020-07-09 18:43:53.000000 eppy3000-0.1.4/eppy3000/oldeppy/__init__.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)     2192 2020-04-07 19:39:27.000000 eppy3000-0.1.4/eppy3000/rawidf.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)     2821 2020-04-07 19:39:27.000000 eppy3000-0.1.4/eppy3000/readepj.py
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000.egg-info/
--rw-r--r--   0 santoshphilip   (501) staff       (20)     9023 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000.egg-info/PKG-INFO
--rw-r--r--   0 santoshphilip   (501) staff       (20)     1105 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000.egg-info/SOURCES.txt
--rw-r--r--   0 santoshphilip   (501) staff       (20)        1 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000.egg-info/dependency_links.txt
--rw-r--r--   0 santoshphilip   (501) staff       (20)        1 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000.egg-info/not-zip-safe
--rw-r--r--   0 santoshphilip   (501) staff       (20)        6 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000.egg-info/requires.txt
--rw-r--r--   0 santoshphilip   (501) staff       (20)        9 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000.egg-info/top_level.txt
--rw-r--r--   0 santoshphilip   (501) staff       (20)      450 2020-07-09 19:02:45.000000 eppy3000-0.1.4/setup.cfg
--rwxr-xr-x   0 santoshphilip   (501) staff       (20)     1394 2020-07-09 18:53:50.000000 eppy3000-0.1.4/setup.py
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/tests/
--rw-r--r--   0 santoshphilip   (501) staff       (20)        0 2020-04-07 19:39:27.000000 eppy3000-0.1.4/tests/__init__.py
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/tests/experimental/
--rw-r--r--   0 santoshphilip   (501) staff       (20)        1 2020-07-09 18:43:54.000000 eppy3000-0.1.4/tests/experimental/__init__.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)     1467 2020-07-09 18:43:54.000000 eppy3000-0.1.4/tests/experimental/test_listfields.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)     4431 2020-07-09 18:43:54.000000 eppy3000-0.1.4/tests/oldeppytests.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)     1927 2020-07-09 18:43:54.000000 eppy3000-0.1.4/tests/schemafortesting.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)     5974 2020-04-07 19:39:27.000000 eppy3000-0.1.4/tests/test_epMunch.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)    11811 2020-04-07 19:39:27.000000 eppy3000-0.1.4/tests/test_epschema.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)     4626 2020-07-09 18:43:54.000000 eppy3000-0.1.4/tests/test_idfjsonconverter.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)     2754 2020-07-09 18:43:54.000000 eppy3000-0.1.4/tests/test_modelmaker.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)     2359 2020-04-07 19:39:27.000000 eppy3000-0.1.4/tests/test_rawidf.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)     2019 2020-04-07 19:39:27.000000 eppy3000-0.1.4/tests/test_readidf.py
+drwxr-xr-x   0 santosh    (501) staff       (20)        0 2023-04-22 01:13:13.563669 eppy3000-0.1.5/
+-rw-r--r--   0 santosh    (501) staff       (20)      118 2023-04-22 00:24:22.000000 eppy3000-0.1.5/AUTHORS.rst
+-rw-r--r--   0 santosh    (501) staff       (20)     1417 2023-04-22 00:24:22.000000 eppy3000-0.1.5/CONTRIBUTING.rst
+-rw-r--r--   0 santosh    (501) staff       (20)     2935 2023-04-22 00:24:22.000000 eppy3000-0.1.5/HISTORY.rst
+-rw-r--r--   0 santosh    (501) staff       (20)    16725 2023-04-22 00:24:22.000000 eppy3000-0.1.5/LICENSE
+-rw-r--r--   0 santosh    (501) staff       (20)      262 2023-04-22 00:24:22.000000 eppy3000-0.1.5/MANIFEST.in
+-rw-r--r--   0 santosh    (501) staff       (20)     8206 2023-04-22 01:13:13.563863 eppy3000-0.1.5/PKG-INFO
+-rw-r--r--   0 santosh    (501) staff       (20)     4545 2023-04-22 00:24:22.000000 eppy3000-0.1.5/README.rst
+drwxr-xr-x   0 santosh    (501) staff       (20)        0 2023-04-22 01:13:13.545936 eppy3000-0.1.5/docs/
+-rw-r--r--   0 santosh    (501) staff       (20)      609 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/Makefile
+-rw-r--r--   0 santosh    (501) staff       (20)       28 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/authors.rst
+-rwxr-xr-x   0 santosh    (501) staff       (20)     4966 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/conf.py
+-rw-r--r--   0 santosh    (501) staff       (20)       33 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/contributing.rst
+-rw-r--r--   0 santosh    (501) staff       (20)     1382 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/developmentnotes.rst
+-rw-r--r--   0 santosh    (501) staff       (20)      591 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/eppy3000.dbm_functions.rst
+-rw-r--r--   0 santosh    (501) staff       (20)      189 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/eppy3000.experimental.rst
+-rw-r--r--   0 santosh    (501) staff       (20)      389 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/eppy3000.oldeppy.rst
+-rw-r--r--   0 santosh    (501) staff       (20)     1772 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/eppy3000.rst
+-rw-r--r--   0 santosh    (501) staff       (20)      376 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/eppy3000.runner.rst
+-rw-r--r--   0 santosh    (501) staff       (20)       28 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/history.rst
+drwxr-xr-x   0 santosh    (501) staff       (20)        0 2023-04-22 01:13:13.536567 eppy3000-0.1.5/docs/images/
+drwxr-xr-x   0 santosh    (501) staff       (20)        0 2023-04-22 01:13:13.546300 eppy3000-0.1.5/docs/images/developmentnotes/
+-rw-r--r--   0 santosh    (501) staff       (20)   391269 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/images/developmentnotes/epJSON_structure.png
+drwxr-xr-x   0 santosh    (501) staff       (20)        0 2023-04-22 01:13:13.548472 eppy3000-0.1.5/docs/images/htmlviewer/
+-rw-r--r--   0 santosh    (501) staff       (20)    87888 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/images/htmlviewer/epjhtml.png
+-rw-r--r--   0 santosh    (501) staff       (20)    12977 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/images/htmlviewer/epmunchhtml.png
+-rw-r--r--   0 santosh    (501) staff       (20)    79110 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/images/htmlviewer/epobjectshtml.png
+-rw-r--r--   0 santosh    (501) staff       (20)      395 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/index.rst
+-rw-r--r--   0 santosh    (501) staff       (20)     1138 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/installation.rst
+-rw-r--r--   0 santosh    (501) staff       (20)      770 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/make.bat
+-rw-r--r--   0 santosh    (501) staff       (20)       61 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/modules.rst
+-rw-r--r--   0 santosh    (501) staff       (20)       27 2023-04-22 00:24:22.000000 eppy3000-0.1.5/docs/readme.rst
+drwxr-xr-x   0 santosh    (501) staff       (20)        0 2023-04-22 01:13:13.552744 eppy3000-0.1.5/eppy3000/
+-rw-r--r--   0 santosh    (501) staff       (20)     2213 2023-04-22 01:10:58.000000 eppy3000-0.1.5/eppy3000/__init__.py
+drwxr-xr-x   0 santosh    (501) staff       (20)        0 2023-04-22 01:13:13.555671 eppy3000-0.1.5/eppy3000/dbm_functions/
+-rw-r--r--   0 santosh    (501) staff       (20)      781 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/dbm_functions/__init__.py
+-rw-r--r--   0 santosh    (501) staff       (20)     7080 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/dbm_functions/json2dbm.py
+-rw-r--r--   0 santosh    (501) staff       (20)     8643 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/dbm_functions/schemaindbm.py
+-rw-r--r--   0 santosh    (501) staff       (20)     9369 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/epMunch.py
+-rw-r--r--   0 santosh    (501) staff       (20)     5401 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/epj_mmapping.py
+-rw-r--r--   0 santosh    (501) staff       (20)     4357 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/epjviewer.py
+-rw-r--r--   0 santosh    (501) staff       (20)       44 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/eppy3000.py
+-rw-r--r--   0 santosh    (501) staff       (20)     2853 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/epschema.py
+drwxr-xr-x   0 santosh    (501) staff       (20)        0 2023-04-22 01:13:13.556583 eppy3000-0.1.5/eppy3000/experimental/
+-rw-r--r--   0 santosh    (501) staff       (20)      542 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/experimental/__init__.py
+-rw-r--r--   0 santosh    (501) staff       (20)      125 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/experimental/hello.py
+-rw-r--r--   0 santosh    (501) staff       (20)      734 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/experimental/listfields.py
+-rw-r--r--   0 santosh    (501) staff       (20)    14473 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/idfjsonconverter.py
+-rw-r--r--   0 santosh    (501) staff       (20)     1333 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/installlocation.py
+-rw-r--r--   0 santosh    (501) staff       (20)     7469 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/modelmaker.py
+drwxr-xr-x   0 santosh    (501) staff       (20)        0 2023-04-22 01:13:13.556916 eppy3000-0.1.5/eppy3000/oldeppy/
+-rw-r--r--   0 santosh    (501) staff       (20)     1481 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/oldeppy/__init__.py
+-rw-r--r--   0 santosh    (501) staff       (20)     2192 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/rawidf.py
+-rw-r--r--   0 santosh    (501) staff       (20)     2973 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/readepj.py
+drwxr-xr-x   0 santosh    (501) staff       (20)        0 2023-04-22 01:13:13.557464 eppy3000-0.1.5/eppy3000/runner/
+-rw-r--r--   0 santosh    (501) staff       (20)       41 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/runner/__init__.py
+-rw-r--r--   0 santosh    (501) staff       (20)    11354 2023-04-22 00:24:22.000000 eppy3000-0.1.5/eppy3000/runner/run_functions.py
+drwxr-xr-x   0 santosh    (501) staff       (20)        0 2023-04-22 01:13:13.554722 eppy3000-0.1.5/eppy3000.egg-info/
+-rw-r--r--   0 santosh    (501) staff       (20)     8206 2023-04-22 01:13:13.000000 eppy3000-0.1.5/eppy3000.egg-info/PKG-INFO
+-rw-r--r--   0 santosh    (501) staff       (20)     1727 2023-04-22 01:13:13.000000 eppy3000-0.1.5/eppy3000.egg-info/SOURCES.txt
+-rw-r--r--   0 santosh    (501) staff       (20)        1 2023-04-22 01:13:13.000000 eppy3000-0.1.5/eppy3000.egg-info/dependency_links.txt
+-rw-r--r--   0 santosh    (501) staff       (20)        1 2023-04-22 01:13:13.000000 eppy3000-0.1.5/eppy3000.egg-info/not-zip-safe
+-rw-r--r--   0 santosh    (501) staff       (20)       21 2023-04-22 01:13:13.000000 eppy3000-0.1.5/eppy3000.egg-info/requires.txt
+-rw-r--r--   0 santosh    (501) staff       (20)        9 2023-04-22 01:13:13.000000 eppy3000-0.1.5/eppy3000.egg-info/top_level.txt
+-rw-r--r--   0 santosh    (501) staff       (20)      450 2023-04-22 01:13:13.564742 eppy3000-0.1.5/setup.cfg
+-rwxr-xr-x   0 santosh    (501) staff       (20)     1423 2023-04-22 01:12:58.000000 eppy3000-0.1.5/setup.py
+drwxr-xr-x   0 santosh    (501) staff       (20)        0 2023-04-22 01:13:13.562613 eppy3000-0.1.5/tests/
+-rw-r--r--   0 santosh    (501) staff       (20)        0 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/__init__.py
+drwxr-xr-x   0 santosh    (501) staff       (20)        0 2023-04-22 01:13:13.563424 eppy3000-0.1.5/tests/experimental/
+-rw-r--r--   0 santosh    (501) staff       (20)        1 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/experimental/__init__.py
+-rw-r--r--   0 santosh    (501) staff       (20)     1512 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/experimental/test_listfields.py
+-rw-r--r--   0 santosh    (501) staff       (20)     4464 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/oldeppytests.py
+-rw-r--r--   0 santosh    (501) staff       (20)     1928 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/schemafortesting.py
+-rw-r--r--   0 santosh    (501) staff       (20)    11221 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/test_epMunch.py
+-rw-r--r--   0 santosh    (501) staff       (20)     5012 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/test_epj_mmapping.py
+-rw-r--r--   0 santosh    (501) staff       (20)     6348 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/test_epjviewer.py
+-rw-r--r--   0 santosh    (501) staff       (20)    11780 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/test_epschema.py
+-rw-r--r--   0 santosh    (501) staff       (20)    17302 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/test_idfjsonconverter.py
+-rw-r--r--   0 santosh    (501) staff       (20)     2359 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/test_installlocation.py
+-rw-r--r--   0 santosh    (501) staff       (20)     5592 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/test_json2dbm.py
+-rw-r--r--   0 santosh    (501) staff       (20)     6857 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/test_modelmaker.py
+-rw-r--r--   0 santosh    (501) staff       (20)     2355 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/test_rawidf.py
+-rw-r--r--   0 santosh    (501) staff       (20)     2013 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/test_readidf.py
+-rw-r--r--   0 santosh    (501) staff       (20)     7024 2023-04-22 00:24:22.000000 eppy3000-0.1.5/tests/test_schemaindbm.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `eppy3000-0.1.4/CONTRIBUTING.rst` & `eppy3000-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.4/HISTORY.rst` & `eppy3000-0.1.5/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,56 @@
 =======
 History
 =======
 
 Releases
 --------
 
+
+Release 0.1.13  (2021-03-16)
+----------------------------
+
+2021-03-16
+~~~~~~~~~~
+
+Fixed #76
+
+:Problem: Need easier conversion from IDF to epJSON
+:Solution: ``idffile2epjfile`` will convert a single file and ``idffolder2epjfolder`` will do batch conversion
+
+Date: Mon Jan 18 21:53:40 PST 2021
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+fixed issue #73
+
+:Problem: Would be nice to have an html viewer for epj
+:Solution: pytested eppy3000.epjviewer with sphinx user documentation
+
+Date: Tue Jan 12 14:18:37 PST 2021
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+fixed issue #69
+
+:Problem: no EPJ.run() function
+:Solution: EPJ.run() function implemented
+
+
+Release 0.1.4  (2020-07-09)
+---------------------------
+
+
 Date:   Tue Jul 7 08:09:26 2020 -0700
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Fixed issue #48
 
 :Problem: No Tutorial for eppy3000
 :Solution: tutorial for eppy3000
 
-+ This tutorial is based on eppy turorial
++ This tutorial is based on eppy tutorial
 + Identifies the gaps in the eppy3000 tagged by TODO in the tutorial
 + open issues on these TODOs and resolve
 
 
 Release 0.1.3 (2020-07-04)
 --------------------------
```

### Comparing `eppy3000-0.1.4/LICENSE` & `eppy3000-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.4/PKG-INFO` & `eppy3000-0.1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,210 +1,244 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: eppy3000
-Version: 0.1.4
+Version: 0.1.5
 Summary: E+ scripting using epJSON file format
 Home-page: https://github.com/pyenergyplus/eppy3000
 Author: Santosh Philip
 Author-email: santosh@noemail.com
 License: Mozilla Public License, v. 2.0
-Description: ========
-        eppy3000
-        ========
-        
-        
-        .. image:: https://img.shields.io/pypi/v/eppy3000.svg
-                :target: https://pypi.python.org/pypi/eppy3000
-        
-        .. image:: https://img.shields.io/travis/pyenergyplus/eppy3000.svg
-                :target: https://travis-ci.org/pyenergyplus/eppy3000
-        
-        .. image:: https://readthedocs.org/projects/eppy3000/badge/?version=latest
-                :target: https://eppy3000.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        
-        
-        
-        E+ scripting using epJSON file format
-        
-        
-        * Free software: Mozilla Public License, v. 2.0
-        * Documentation: https://eppy3000.readthedocs.io.
-        * Home Page: https://github.com/pyenergyplus/eppy3000
-        
-        
-        Features - so far :-)
-        ---------------------
-        
-        * Open and read an epJSON file with *some* `eppy <https://github.com/santoshphilip/eppy>`_ functionality.
-        * Right now the `eppy <https://github.com/santoshphilip/eppy>`_ functionality is only partial
-        
-        
-        Background
-        ----------
-        
-        E+ has been moving from the IDD/IDF text format to a JSON format. `Eppy <https://github.com/santoshphilip/eppy>`_ reads the old IDD/IDF format. There is a need to have `eppy <https://github.com/santoshphilip/eppy>`_ read the JSON format and/or have a new package that will read the JSON format.
-        
-        Whats in a name
-        ---------------
-        
-        Why is this package called eppy3000 ?
-        
-        It is a play on the word python3000. Guido van van Rossum said about python in 2007 *"The first time I came up with the idea of Python 3000 was probably at a Python conference in the year 2000. The name was a take on Windows 2000. ...<snip>...  The idea was that Python 3000 would be the first Python release to give up backwards compatibility in favor of making it the best language going forward."*
-        
-        Eppy3000 will also break backward compatibility with eppy. Also eppy3000 will be written only for python3. Eppy3000 and eppy will continue to remain the best scripting language for modelling :-)
-        
-        
-        So what is eppy3000
-        -------------------
-        
-        This project is an attempt to read JSON file formats and work like eppy. There is some value in trying to do this from scratch. The dot syntax that makes the original eppy useful can be recreated with a couple of lines in eppy3000. It took a lot of deep hacking to make the dot syntax work in the original eppy. Eppy3000 reads the JSON format as a dictionary. The package `Munch <https://github.com/Infinidat/munch>`_ (what was `Bunch <https://github.com/dsc/bunch>`_) allows the use of dot format syntax with a dictionary. The code is as simple as::
-        
-            as_json = json.load(open(fname, 'r'))
-            for_dot_syntax = DefaultMunch.fromDict(as_json)
-        
-        At this point eppy3000 is an exploration to find out what is possible. The API in eppy3000 will not be stable as we explore the possibilities. So, don't use it as production code yet :-)
-        
-        
-        What about eppy
-        ---------------
-        
-        Eppy will be continue to be developed and maintained. A major task will be to make eppy read the new JSON formats. Initial investigations shows that it is not too hard to develop this functionality. Internally eppy will continue to use the old format. Hopefully this will make the JSON reading functionality trivially easy. At the moment, E+ maintains a one to one mapping between the old IDD/IDF format and the new JSON format. This mapping is embedded in the file Energy+.schema.epJSON, pointing to an easy compatibility strategy.
-        
-        In the long term, this may not be a viable strategy, as E+ may totally abandon the IDD/IDF file format breaking the link between JSON and IDD/IDF. Discussion thread at `unmethours <https://unmethours.com/question/36062/hvac-templates-to-be-discontinued/>`_ seems to indicate that this is about 5 yers in the future.
-        
-        
-        Future possibilites
-        -------------------
-        
-        A number of possibilites came up in discussions at Simbuild 2018 in Chicago. The biggest takeaway was that the code base for the JSON format and the dot syntax can lead to a universal translator between modelling file formats. The thinking here is that if there exists a schema.JSON for two modelling file structures, the possibility of translating between the two exists.
-        
-        Of course *the proof is in the pudding*. So we are going to write some quick and dirty translators between E+ and DOE2.1E (or EQuest) as well as between the older idds and the new epJSON. Lets see how that goes.
-        
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        Releases
-        --------
-        
-        Date:   Tue Jul 7 08:09:26 2020 -0700
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Fixed issue #48
-        
-        :Problem: No Tutorial for eppy3000
-        :Solution: tutorial for eppy3000
-        
-        + This tutorial is based on eppy turorial
-        + Identifies the gaps in the eppy3000 tagged by TODO in the tutorial
-        + open issues on these TODOs and resolve
-        
-        
-        Release 0.1.3 (2020-07-04)
-        --------------------------
-        
-        Date:   Wed May 13 14:20:34 2020 -0700
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-            fixed issue # 45
-            
-            Problem: setup.py not including folders `oldeppy` and `experimental`
-            Solution: setup.py updated and tested
-        
-        
-        
-        Release 0.1.2 (2020-05-12)
-        --------------------------
-        
-        Date:   Tue May 12 08:11:39 2020 -0700
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-            fixed issue #41
-            
-            Problem: function to get an array of xyz points from the surfaces
-            Solution: function in eppy300.experimental.listfields.surf2list()
-        
-        
-        Date:   Mon May 11 08:15:50 2020 -0700
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-            fixed issue #34
-            
-            Problem: need an easy to use converter between
-            epj (epyy300 format) and idf (eppy format)
-            
-            Solution: functions idf2epj() epj2idf() do this.
-            epj.saveas(filename) and idf.saveas(filename)
-            will save it to disk
-        
-        
-        
-        Date:   Mon May 11 15:35:54 2020 -0700
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-            fixed issue #39
-        
-            **Problem:** need a place to put experimental functions
-            **Solution:** created an experimental folder in eppy3000
-        
-        
-        Date:   Mon May 11 08:15:50 2020 -0700
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-            fixed issue #34
-            
-            Problem: need an easy to use converter between
-            epj (epyy300 format) and idf (eppy format)
-            
-            Solution: functions idf2epj() epj2idf() do this.
-            epj.saveas(filename) and idf.saveas(filename)
-            will save it to disk
-        
-        
-        
-        Sun May 10 09:26:32 2020 -0700
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-            fixed issue #36
-        
-            Problem: modelbuilder.EPJ need savecopy() to fix issue #34
-            Solution: coded EPJ.savecopy and EPJ.jsonstr()
-        
-        
-        
-        
-        
-        Release 0.1.1 (2019-06-06)
-        --------------------------
-        
-        2019-06-06
-        ~~~~~~~~~~
-        
-        - functions to read and write IDF files
-            - issue #20
-        
-        0.1.0 (2018-10-15)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: eppy3000
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+========
+eppy3000
+========
+
+
+.. image:: https://img.shields.io/pypi/v/eppy3000.svg
+        :target: https://pypi.python.org/pypi/eppy3000
+
+.. image:: https://img.shields.io/travis/pyenergyplus/eppy3000.svg
+        :target: https://travis-ci.org/pyenergyplus/eppy3000
+
+.. image:: https://readthedocs.org/projects/eppy3000/badge/?version=latest
+        :target: https://eppy3000.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+
+
+
+E+ scripting using epJSON file format
+
+
+* Free software: Mozilla Public License, v. 2.0
+* Documentation: https://eppy3000.readthedocs.io.
+* Home Page: https://github.com/pyenergyplus/eppy3000
+
+
+Features - so far :-)
+---------------------
+
+* Open and read an epJSON file with *some* `eppy <https://github.com/santoshphilip/eppy>`_ functionality.
+* Right now the `eppy <https://github.com/santoshphilip/eppy>`_ functionality is only partial
+
+
+Background
+----------
+
+E+ has been moving from the IDD/IDF text format to a JSON format. `Eppy <https://github.com/santoshphilip/eppy>`_ reads the old IDD/IDF format. There is a need to have `eppy <https://github.com/santoshphilip/eppy>`_ read the JSON format and/or have a new package that will read the JSON format.
+
+Whats in a name
+---------------
+
+Why is this package called eppy3000 ?
+
+It is a play on the word python3000. Guido van van Rossum said about python in 2007 *"The first time I came up with the idea of Python 3000 was probably at a Python conference in the year 2000. The name was a take on Windows 2000. ...<snip>...  The idea was that Python 3000 would be the first Python release to give up backwards compatibility in favor of making it the best language going forward."*
+
+Eppy3000 will also break backward compatibility with eppy. Also eppy3000 will be written only for python3. Eppy3000 and eppy will continue to remain the best scripting language for modelling :-)
+
+
+So what is eppy3000
+-------------------
+
+This project is an attempt to read JSON file formats and work like eppy. There is some value in trying to do this from scratch. The dot syntax that makes the original eppy useful can be recreated with a couple of lines in eppy3000. It took a lot of deep hacking to make the dot syntax work in the original eppy. Eppy3000 reads the JSON format as a dictionary. The package `Munch <https://github.com/Infinidat/munch>`_ (what was `Bunch <https://github.com/dsc/bunch>`_) allows the use of dot format syntax with a dictionary. The code is as simple as::
+
+    as_json = json.load(open(fname, 'r'))
+    for_dot_syntax = DefaultMunch.fromDict(as_json)
+
+At this point eppy3000 is an exploration to find out what is possible. The API in eppy3000 will not be stable as we explore the possibilities. So, don't use it as production code yet :-)
+
+
+What about eppy
+---------------
+
+Eppy will be continue to be developed and maintained. A major task will be to make eppy read the new JSON formats. Initial investigations shows that it is not too hard to develop this functionality. Internally eppy will continue to use the old format. Hopefully this will make the JSON reading functionality trivially easy. At the moment, E+ maintains a one to one mapping between the old IDD/IDF format and the new JSON format. This mapping is embedded in the file Energy+.schema.epJSON, pointing to an easy compatibility strategy.
+
+In the long term, this may not be a viable strategy, as E+ may totally abandon the IDD/IDF file format breaking the link between JSON and IDD/IDF. Discussion thread at `unmethours <https://unmethours.com/question/36062/hvac-templates-to-be-discontinued/>`_ seems to indicate that this is about 5 yers in the future.
+
+
+Future possibilites
+-------------------
+
+A number of possibilites came up in discussions at Simbuild 2018 in Chicago. The biggest takeaway was that the code base for the JSON format and the dot syntax can lead to a universal translator between modelling file formats. The thinking here is that if there exists a schema.JSON for two modelling file structures, the possibility of translating between the two exists.
+
+Of course *the proof is in the pudding*. So we are going to write some quick and dirty translators between E+ and DOE2.1E (or EQuest) as well as between the older idds and the new epJSON. Lets see how that goes.
+
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+Releases
+--------
+
+
+Release 0.1.13  (2021-03-16)
+----------------------------
+
+2021-03-16
+~~~~~~~~~~
+
+Fixed #76
+
+:Problem: Need easier conversion from IDF to epJSON
+:Solution: ``idffile2epjfile`` will convert a single file and ``idffolder2epjfolder`` will do batch conversion
+
+Date: Mon Jan 18 21:53:40 PST 2021
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+fixed issue #73
+
+:Problem: Would be nice to have an html viewer for epj
+:Solution: pytested eppy3000.epjviewer with sphinx user documentation
+
+Date: Tue Jan 12 14:18:37 PST 2021
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+fixed issue #69
+
+:Problem: no EPJ.run() function
+:Solution: EPJ.run() function implemented
+
+
+Release 0.1.4  (2020-07-09)
+---------------------------
+
+
+Date:   Tue Jul 7 08:09:26 2020 -0700
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Fixed issue #48
+
+:Problem: No Tutorial for eppy3000
+:Solution: tutorial for eppy3000
+
++ This tutorial is based on eppy tutorial
++ Identifies the gaps in the eppy3000 tagged by TODO in the tutorial
++ open issues on these TODOs and resolve
+
+
+Release 0.1.3 (2020-07-04)
+--------------------------
+
+Date:   Wed May 13 14:20:34 2020 -0700
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    fixed issue # 45
+    
+    Problem: setup.py not including folders `oldeppy` and `experimental`
+    Solution: setup.py updated and tested
+
+
+
+Release 0.1.2 (2020-05-12)
+--------------------------
+
+Date:   Tue May 12 08:11:39 2020 -0700
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    fixed issue #41
+    
+    Problem: function to get an array of xyz points from the surfaces
+    Solution: function in eppy300.experimental.listfields.surf2list()
+
+
+Date:   Mon May 11 08:15:50 2020 -0700
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    fixed issue #34
+    
+    Problem: need an easy to use converter between
+    epj (epyy300 format) and idf (eppy format)
+    
+    Solution: functions idf2epj() epj2idf() do this.
+    epj.saveas(filename) and idf.saveas(filename)
+    will save it to disk
+
+
+
+Date:   Mon May 11 15:35:54 2020 -0700
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    fixed issue #39
+
+    **Problem:** need a place to put experimental functions
+    **Solution:** created an experimental folder in eppy3000
+
+
+Date:   Mon May 11 08:15:50 2020 -0700
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    fixed issue #34
+    
+    Problem: need an easy to use converter between
+    epj (epyy300 format) and idf (eppy format)
+    
+    Solution: functions idf2epj() epj2idf() do this.
+    epj.saveas(filename) and idf.saveas(filename)
+    will save it to disk
+
+
+
+Sun May 10 09:26:32 2020 -0700
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    fixed issue #36
+
+    Problem: modelbuilder.EPJ need savecopy() to fix issue #34
+    Solution: coded EPJ.savecopy and EPJ.jsonstr()
+
+
+
+
+
+Release 0.1.1 (2019-06-06)
+--------------------------
+
+2019-06-06
+~~~~~~~~~~
+
+- functions to read and write IDF files
+    - issue #20
+
+0.1.0 (2018-10-15)
+------------------
+
+* First release on PyPI.
```

### Comparing `eppy3000-0.1.4/README.rst` & `eppy3000-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.4/docs/Makefile` & `eppy3000-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.4/docs/conf.py` & `eppy3000-0.1.5/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,45 +16,49 @@
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
-sys.path.insert(0, os.path.abspath('..'))
+
+sys.path.insert(0, os.path.abspath(".."))
 
 import eppy3000
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode',
-    'sphinx.ext.napoleon', 'nbsphinx',
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.napoleon",
+    "nbsphinx",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'eppy3000'
-copyright = u"2018, Santosh Philip"
+project = u"eppy3000"
+copyright = u"2018-2020, Santosh Philip"
 author = u"Santosh Philip"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
@@ -68,98 +72,96 @@
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+# html_theme = 'alabaster'
+html_theme = "classic"
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'eppy3000doc'
+htmlhelp_basename = "eppy3000doc"
 
 
 # -- Options for LaTeX output ------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'eppy3000.tex',
-     u'eppy3000 Documentation',
-     u'Santosh Philip', 'manual'),
+    (
+        master_doc,
+        "eppy3000.tex",
+        u"eppy3000 Documentation",
+        u"Santosh Philip",
+        "manual",
+    ),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'eppy3000',
-     u'eppy3000 Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "eppy3000", u"eppy3000 Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'eppy3000',
-     u'eppy3000 Documentation',
-     author,
-     'eppy3000',
-     'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "eppy3000",
+        u"eppy3000 Documentation",
+        author,
+        "eppy3000",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
-
-
-
```

### Comparing `eppy3000-0.1.4/docs/eppy3000.rst` & `eppy3000-0.1.5/docs/eppy3000.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,104 @@
 eppy3000 package
 ================
 
 Subpackages
 -----------
 
 .. toctree::
+   :maxdepth: 4
 
-    eppy3000.experimental
-    eppy3000.oldeppy
+   eppy3000.dbm_functions
+   eppy3000.experimental
+   eppy3000.oldeppy
+   eppy3000.runner
 
 Submodules
 ----------
 
 eppy3000.epMunch module
 -----------------------
 
 .. automodule:: eppy3000.epMunch
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+eppy3000.epj\_mmapping module
+-----------------------------
+
+.. automodule:: eppy3000.epj_mmapping
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+eppy3000.epjviewer module
+-------------------------
+
+.. automodule:: eppy3000.epjviewer
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 eppy3000.eppy3000 module
 ------------------------
 
 .. automodule:: eppy3000.eppy3000
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 eppy3000.epschema module
 ------------------------
 
 .. automodule:: eppy3000.epschema
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 eppy3000.idfjsonconverter module
 --------------------------------
 
 .. automodule:: eppy3000.idfjsonconverter
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+eppy3000.installlocation module
+-------------------------------
+
+.. automodule:: eppy3000.installlocation
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 eppy3000.modelmaker module
 --------------------------
 
 .. automodule:: eppy3000.modelmaker
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 eppy3000.rawidf module
 ----------------------
 
 .. automodule:: eppy3000.rawidf
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 eppy3000.readepj module
 -----------------------
 
 .. automodule:: eppy3000.readepj
-    :members:
-    :undoc-members:
-    :show-inheritance:
-
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 Module contents
 ---------------
 
 .. automodule:: eppy3000
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `eppy3000-0.1.4/docs/installation.rst` & `eppy3000-0.1.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.4/docs/make.bat` & `eppy3000-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.4/eppy3000/epschema.py` & `eppy3000-0.1.5/eppy3000/epschema.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,27 +13,30 @@
 def read_epschema_asmunch(fhandle):
     """read the epschema json as a munch"""
     try:
         epjs = json.load(fhandle)
         as_munch = EPSchemaMunch.fromDict(epjs)
     except AttributeError as e:
         try:
-            fhandle = open(fhandle, 'r')
+            fhandle = open(fhandle, "r")
             epjs = json.load(fhandle)
             as_munch = EPSchemaMunch.fromDict(epjs)
         except TypeError as e:
             if isinstance(fhandle, EPSchemaMunch):
                 return fhandle
             else:
-                raise TypeError(f"expected str, bytes, os.PathLike object or Munch, not {type(fhandle)}")  # noqa: E501
+                raise TypeError(
+                    f"expected str, bytes, os.PathLike object or Munch, not {type(fhandle)}"
+                )  # noqa: E501
     return as_munch
 
 
 class EPSchemaMunch(Munch):
     """Munch subcalssed to for the EPSchema json"""
+
     def __init__(self, *args, **kwargs):
         super(EPSchemaMunch, self).__init__(*args, **kwargs)
 
     def fieldnames(self):
         """field names of the EPSchema object"""
         return [key for key in self.keys()]
 
@@ -43,20 +46,35 @@
 
     def fieldproperty(self, fieldname):
         """field names of the EPSchema object"""
         return self[fieldname]
 
 
 class EPSchema(object):
-    """hold the data from the json epschema file """
+    """hold the data from the json epschema file"""
+
     def __init__(self, epschemaname):
         super(EPSchema, self).__init__()
         self.epschemaname = epschemaname
         self.read()
 
     def read(self):
         """read the json file"""
+
+        def prop_in_patternProp(val):
+            """return the property in patternProperty"""
+            # assume that val['patternProperties'] has a single key, val
+            # key is either ".*" or "^.*\\S.*$"
+            for key in val["patternProperties"].keys():
+                return val["patternProperties"][key]
+
         self.epschema = read_epschema_asmunch(self.epschemaname)
-        self.version = self.epschema['epJSON_schema_version']
-        self.required = self.epschema['required']
-        self.epschemaobjects = {key: val['patternProperties']['.*']['properties']
-                           for key, val in self.epschema['properties'].items()}
+        self.version = self.epschema["epJSON_schema_version"]
+        self.required = self.epschema["required"]
+        # self.epschemaobjects = {key: val['patternProperties']['.*']['properties']
+        #                    for key, val in self.epschema['properties'].items()}
+        # the above line stopped working in E+ V9.3. ".*" stopped being the only key
+        # workaround is below
+        self.epschemaobjects = {
+            key: prop_in_patternProp(val)["properties"]
+            for key, val in self.epschema["properties"].items()
+        }
```

### Comparing `eppy3000-0.1.4/eppy3000/experimental/__init__.py` & `eppy3000-0.1.5/eppy3000/experimental/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,8 +3,8 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 # =======================================================================
 
 """Experimental functions sit here
 these functions will be unstable and the API's can change.
-But we can experiment with them to see if the design is good""" 
+But we can experiment with them to see if the design is good"""
```

### Comparing `eppy3000-0.1.4/eppy3000/experimental/listfields.py` & `eppy3000-0.1.5/eppy3000/experimental/listfields.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,13 +2,19 @@
 # =======================================================================
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 # =======================================================================
 """functions to work with list fields"""
 
+
 def surf2list(surfobject):
     """return a list of xyz coords from the epobject"""
-    vertices = surfobject['vertices']
-    return [(vrt['vertex_x_coordinate'],
-            vrt['vertex_y_coordinate'],
-            vrt['vertex_z_coordinate'],) for vrt in vertices]
+    vertices = surfobject["vertices"]
+    return [
+        (
+            vrt["vertex_x_coordinate"],
+            vrt["vertex_y_coordinate"],
+            vrt["vertex_z_coordinate"],
+        )
+        for vrt in vertices
+    ]
```

### Comparing `eppy3000-0.1.4/eppy3000/modelmaker.py` & `eppy3000-0.1.5/eppy3000/modelmaker.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from io import StringIO
 from munch import Munch
 from eppy3000.readepj import readepjjson
 from eppy3000.epschema import read_epschema_asmunch
 from eppy3000.readepj import removeeppykeys
 from eppy3000.epschema import EPSchema
 from eppy3000.epMunch import EPMunch
+from eppy3000.epj_mmapping import EpjMapping
+import eppy3000.runner.run_functions as run_functions
 
 
 class EPJ(object):
     def __init__(self, epjname=None, epw=None, epschemaname=None):
         super(EPJ, self).__init__()
         self.epjname = epjname
         self.epw = epw
@@ -24,120 +26,187 @@
         if self.epschemaname:
             self.readepschema()
         self.read()
 
     def read_epschema_asmunch(self):
         """Read the epschema file - will become a frozen singleton"""
         read_epschema_asmunch(self.epschemaname)
+        # not used ???
 
     def read(self):
         """read the epj file"""
         self.epj = readepjjson(self.epjname)
-        self.epobjects = {key: [val1 for val1 in val.values()]
-                           for key, val in self.epj.items()}
+        self.epobjects = EpjMapping(self.epj)
+        # {
+        #     key: [val1 for val1 in val.values()] for key, val in self.epj.items()
+        # }
+        # TODO: the above line should get the epobjects from the schema
+        # This should happen whenever the schema is read.
+        # in case the schema reading happens far in the future
+        # eppy3000 should partilly work even without the schema
+        # -
+
+        # insert epj into the epobject
+        # this allows the epobject to access all other objects in the epj
+        for epobjects in self.epobjects.values():
+            for epobject in epobjects:
+                epobject["eppy_epj"] = self.epj
         if self.epschemaname:
             for key in self.epobjects.keys():
                 for epobject in self.epobjects[key]:
-                    epobject['eppy_objepschema'] = self.epschema.epschemaobjects[key]
+                    epobject["eppy_objepschema"] = self.epschema.epschemaobjects[key]
 
     def readepschema(self):
         """read the epschema file"""
         self.epschema = EPSchema(self.epschemaname)
 
     def __repr__(self):
         """print this"""
         return self.epj.__repr__()
 
     def saveas(self, filename, indent=4):
         """saveas in filename"""
         self.epjname = filename
         self.save(filename, indent=indent)
-        
+
     def savecopy(self, filename=None, indent=4):
-        """save a copy of the file 
+        """save a copy of the file
         if filename==None: return copy in StringIO
         NOT unit TESTED at all. Not even use tested"""
         if filename:
             self.save(filename=filename, indent=indent)
         else:
             tosave = self.epj.toDict()
             tosave = Munch.fromDict(tosave)
             removeeppykeys(tosave)
             fhandle = StringIO()
             fhandle.write(tosave.toJSON(indent=indent))
             fhandle.seek(0)
             return fhandle
-            
 
     def save(self, filename=None, indent=4):
         """save the file"""
         if not filename:
             filename = self.epjname
-        with open(filename, 'w') as fhandle:
+        try:
+            with open(filename, "w") as fhandle:
+                tosave = self.epj.toDict()
+                tosave = Munch.fromDict(tosave)
+                removeeppykeys(tosave)
+                fhandle.write(tosave.toJSON(indent=indent))
+        except TypeError as e:
+            fhandle = filename
             tosave = self.epj.toDict()
             tosave = Munch.fromDict(tosave)
             removeeppykeys(tosave)
             fhandle.write(tosave.toJSON(indent=indent))
-            
+
     def jsonstr(self, indent=4):
         """return a json string of the file"""
         fhandle = self.savecopy(indent=indent)
-        return '\n'.join([line.rstrip() for line in fhandle])
+        return "\n".join([line.rstrip() for line in fhandle])
 
     def newepobject(self, key, objname, defaultvalues=True, **kwargs):
         """create a new epj object"""
         # TODO test for dup name
         # TODO Kwargs strategy for array -
         #     delay implementation for now, throw exception
         # TODO exceptions for wrong field name
         # TODO exception for wrong field value type
         # TODO documentation in usage.rst
+        # should self.epobjects be updated here
         objepschema = self.epschema.epschemaobjects[key]
         try:
             nobj = self.epj[key][objname] = EPMunch()
         except KeyError as e:
             self.epj[key] = EPMunch()
             nobj = self.epj[key][objname] = EPMunch()
         for fieldname in objepschema.fieldnames():
             try:
                 if defaultvalues:
                     fieldfprop = objepschema.fieldproperty(fieldname)
-                    nobj[fieldname] = fieldfprop['default']
+                    nobj[fieldname] = fieldfprop["default"]
             except KeyError as e:
                 prop = objepschema.fieldproperty(fieldname)
                 # print(fieldname, prop.keys())
-                if 'type' in prop:
-                    if prop['type'] == 'array':
+                if "type" in prop:
+                    if prop["type"] == "array":
                         # pprint(prop['items'])
                         pass
                 pass
         for key1, val1 in kwargs.items():
             nobj[key1] = val1
-        nobj['eppykey'] = key
-        nobj['eppyname'] = objname
-        nobj['eppy_objepschema'] = objepschema
+        nobj["eppykey"] = key
+        nobj["eppyname"] = objname
+        nobj["eppy_objepschema"] = objepschema
         return nobj
 
-    def removeepobject(self, key, objname):
-        """remove an epj object"""
-        return self.epj[key].pop(objname)
+    # def removeepobject(self, key, objname):
+    #     """remove an epj object"""
+    #     # should self.epobjects be updated here
+    #     return self.epj[key].pop(objname)
+
+    def popepobject(self, key, index):
+        """Pop an EPJ object from the EPJ.
+
+        Parameters
+        ----------
+        key : str
+            The type of EPJ object.
+        index : int
+            The index of the object to pop.
+
+        Returns
+        -------
+        EpBunch object.
+
+        """
+        return self.epobjects[key].pop(index)
+
+    def removeepobject(self, epobject):
+        """Remove an EPJ object from the EPJ.
+
+        Parameters
+        ----------
+        epobject : EpBunch object
+            The epobject to remove.
+
+        """
+        key = epobject.eppykey
+        self.epobjects[key].remove(epobject)
+
+    def removeallepobjects(self, epjkey):
+        """Remove all epobjects of a certain type from the EPJ.
+
+        Parameters
+        ----------
+        epjkey : key of the epobjects to remove
+
+        """
+        while len(self.epobjects[epjkey]) > 0:
+            self.popepobject(epjkey, 0)
+
 
     def copyepobject(self, key, objname, newname):
         """copy an epj object with a new name"""
         # don't use the function dict.items() since the json for array has
         # field name `items`
+        # should self.epobjects be updated here
         oldobj = self.epj[key][objname]
         newobj = EPMunch()
         self.epj[key][newname] = newobj
         for key1 in oldobj.keys():
-            if not key1.startswith('eppy'):
+            if not key1.startswith("eppy"):
                 val1 = oldobj[key1]
                 if isinstance(val1, list):
                     newobj[key1] = list()
                     for item in val1:
                         newobj[key1].append(item.copy())
                 else:
                     newobj[key1] = val1
-        newobj['eppyname'] = newname
-        newobj['eppykey'] = key
-        newobj['eppy_objepschema'] = oldobj['eppy_objepschema']
+        newobj["eppyname"] = newname
+        newobj["eppykey"] = key
+        newobj["eppy_objepschema"] = oldobj["eppy_objepschema"]
         return newobj
+
+    def run(self, **runoptions):
+        return run_functions.run(self, **runoptions)
```

### Comparing `eppy3000-0.1.4/eppy3000/oldeppy/__init__.py` & `eppy3000-0.1.5/eppy3000/oldeppy/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 # Copyright (c) 2020 Santosh Philip
 # =======================================================================
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 # =======================================================================
 """convertion functions - to convert from JSON to IDF and in reverse.
-These functions return a epyy.IDF or eppy300.IDF structure"""
+These functions return a eppy.IDF or eppy3000.EPJ structure"""
+
 
 class NeedsEppyError(Exception):
     pass
 
+
 try:
     import eppy
 except ModuleNotFoundError as e:
     raise NeedsEppyError("you need to install eppy to run these functions")
 
 
 from io import StringIO
 import eppy3000
 from eppy3000.modelmaker import EPJ
 import eppy3000.idfjsonconverter
-# - 
+
+# -
 from eppy import modeleditor
 from eppy.modeleditor import IDF
 
 
 def idf2epj(idf, epjsonhandle):
     """convert idf to json. return a eppy3000.IDF structure"""
     idfhandle = StringIO(idf.idfstr())
     epjstr = eppy3000.idfjsonconverter.idf2json(idfhandle, epjsonhandle)
-    return EPJ(StringIO(epjstr))
-    
-    
+    epjsonhandle.seek(0)  # need to reset, since we are reading it again
+    return EPJ(StringIO(epjstr), epw=idf.epw, epschemaname=epjsonhandle)
+
+
 def epj2idf(epj, epjsonhandle, iddhandle=None):
     """convert json to idf"""
     jsonhandle = epj.savecopy()
-    idfstr =  eppy3000.idfjsonconverter.json2idf(jsonhandle, epjsonhandle) 
-    return eppy.openidf(StringIO(idfstr), idd=iddhandle)
+    idfstr = eppy3000.idfjsonconverter.json2idf(jsonhandle, epjsonhandle)
+    return eppy.openidf(StringIO(idfstr), idd=iddhandle, epw=epj.epw)
```

### Comparing `eppy3000-0.1.4/eppy3000/rawidf.py` & `eppy3000-0.1.5/eppy3000/rawidf.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,27 +22,27 @@
     # linesep = mylib3.getlinesep(astr)
     alist = astr.splitlines()
     for i in range(len(alist)):
         alist1 = alist[i].split(cphrase)
         alist[i] = alist1[0]
 
     # return string.join(alist, linesep)
-    return '\n'.join(alist)
+    return "\n".join(alist)
 
 
 def readrawidf(fhandle):
     """read the idf file as a dict. Dict keys are idfobjkeys,
     dict values are list in list"""
     astr = fhandle.read()
-    nocom = removecomment(astr, '!')
+    nocom = removecomment(astr, "!")
     idfst = nocom
-    alist = idfst.split(';')
+    alist = idfst.split(";")
     rawdata = {}
     for element in alist:
-        lst = element.split(',')
+        lst = element.split(",")
         lst = [item.strip() for item in lst]
         # key = lst[0].strip().upper()
         # not sure of implications here
         key = lst[0].strip()
         if not key:
             continue
         rawdata.setdefault(key, [])
@@ -56,16 +56,16 @@
     if order:
         keys = order
     else:
         keys = rawdata.keys()
     for key in keys:
         try:
             for vals in rawdata[key]:
-                lst.append('{},'.format(key))
+                lst.append("{},".format(key))
                 for val in vals[1:]:
-                    lst.append('     {},'.format(val))
+                    lst.append("     {},".format(val))
                 lst.pop(-1)
-                lst.append('    {};'.format(val))
-                lst.append('')
+                lst.append("    {};".format(val))
+                lst.append("")
         except KeyError as e:
             continue
-    return '\n'.join(lst)
+    return "\n".join(lst)
```

### Comparing `eppy3000-0.1.4/eppy3000/readepj.py` & `eppy3000-0.1.5/eppy3000/readepj.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         can be a file open for read or a io.StringIO object
 
     Returns
     -------
     eppy.EPMunch
     """
     try:
-        fhandle = open(fhandle, 'r')
+        fhandle = open(fhandle, "r")
     except TypeError as e:
         pass
     as_json = json.load(fhandle)
     as_munch = EPMunch.fromDict(as_json)
     addeppykeys(as_munch)
     return as_munch
 
@@ -66,16 +66,17 @@
     Returns
     -------
     None
 
     """
     for key, epobjects in epmunch.items():
         for name, epobject in epobjects.items():
-            epobject['eppykey'] = key
-            epobject['eppyname'] = name
+            epobject["eppykey"] = key
+            epobject["eppyname"] = name
+            epobject["eppy_epobjects"] = epobjects
 
 
 def removeeppykeys(epmunch, rkeys=None):
     """remove the eppykeys
 
     This will remove all the additional keys that eppy added
     in addeppykeys(). This is usually called before saving
@@ -89,12 +90,18 @@
         rkeys is set to ['eppykey', 'eppyname', 'eppy_objepschema']
 
     Returns
     -------
     None
     """
     if not rkeys:
-        rkeys = ['eppykey', 'eppyname', 'eppy_objepschema']
+        rkeys = [
+            "eppykey",
+            "eppyname",
+            "eppy_objepschema",
+            "eppy_epj",
+            "eppy_epobjects",
+        ]
     for key, epobjects in epmunch.items():
         for name, epobject in epobjects.items():
             for rkey in rkeys:
                 epobject.pop(rkey, None)
```

### Comparing `eppy3000-0.1.4/eppy3000.egg-info/PKG-INFO` & `eppy3000-0.1.5/eppy3000.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,210 +1,244 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: eppy3000
-Version: 0.1.4
+Version: 0.1.5
 Summary: E+ scripting using epJSON file format
 Home-page: https://github.com/pyenergyplus/eppy3000
 Author: Santosh Philip
 Author-email: santosh@noemail.com
 License: Mozilla Public License, v. 2.0
-Description: ========
-        eppy3000
-        ========
-        
-        
-        .. image:: https://img.shields.io/pypi/v/eppy3000.svg
-                :target: https://pypi.python.org/pypi/eppy3000
-        
-        .. image:: https://img.shields.io/travis/pyenergyplus/eppy3000.svg
-                :target: https://travis-ci.org/pyenergyplus/eppy3000
-        
-        .. image:: https://readthedocs.org/projects/eppy3000/badge/?version=latest
-                :target: https://eppy3000.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        
-        
-        
-        E+ scripting using epJSON file format
-        
-        
-        * Free software: Mozilla Public License, v. 2.0
-        * Documentation: https://eppy3000.readthedocs.io.
-        * Home Page: https://github.com/pyenergyplus/eppy3000
-        
-        
-        Features - so far :-)
-        ---------------------
-        
-        * Open and read an epJSON file with *some* `eppy <https://github.com/santoshphilip/eppy>`_ functionality.
-        * Right now the `eppy <https://github.com/santoshphilip/eppy>`_ functionality is only partial
-        
-        
-        Background
-        ----------
-        
-        E+ has been moving from the IDD/IDF text format to a JSON format. `Eppy <https://github.com/santoshphilip/eppy>`_ reads the old IDD/IDF format. There is a need to have `eppy <https://github.com/santoshphilip/eppy>`_ read the JSON format and/or have a new package that will read the JSON format.
-        
-        Whats in a name
-        ---------------
-        
-        Why is this package called eppy3000 ?
-        
-        It is a play on the word python3000. Guido van van Rossum said about python in 2007 *"The first time I came up with the idea of Python 3000 was probably at a Python conference in the year 2000. The name was a take on Windows 2000. ...<snip>...  The idea was that Python 3000 would be the first Python release to give up backwards compatibility in favor of making it the best language going forward."*
-        
-        Eppy3000 will also break backward compatibility with eppy. Also eppy3000 will be written only for python3. Eppy3000 and eppy will continue to remain the best scripting language for modelling :-)
-        
-        
-        So what is eppy3000
-        -------------------
-        
-        This project is an attempt to read JSON file formats and work like eppy. There is some value in trying to do this from scratch. The dot syntax that makes the original eppy useful can be recreated with a couple of lines in eppy3000. It took a lot of deep hacking to make the dot syntax work in the original eppy. Eppy3000 reads the JSON format as a dictionary. The package `Munch <https://github.com/Infinidat/munch>`_ (what was `Bunch <https://github.com/dsc/bunch>`_) allows the use of dot format syntax with a dictionary. The code is as simple as::
-        
-            as_json = json.load(open(fname, 'r'))
-            for_dot_syntax = DefaultMunch.fromDict(as_json)
-        
-        At this point eppy3000 is an exploration to find out what is possible. The API in eppy3000 will not be stable as we explore the possibilities. So, don't use it as production code yet :-)
-        
-        
-        What about eppy
-        ---------------
-        
-        Eppy will be continue to be developed and maintained. A major task will be to make eppy read the new JSON formats. Initial investigations shows that it is not too hard to develop this functionality. Internally eppy will continue to use the old format. Hopefully this will make the JSON reading functionality trivially easy. At the moment, E+ maintains a one to one mapping between the old IDD/IDF format and the new JSON format. This mapping is embedded in the file Energy+.schema.epJSON, pointing to an easy compatibility strategy.
-        
-        In the long term, this may not be a viable strategy, as E+ may totally abandon the IDD/IDF file format breaking the link between JSON and IDD/IDF. Discussion thread at `unmethours <https://unmethours.com/question/36062/hvac-templates-to-be-discontinued/>`_ seems to indicate that this is about 5 yers in the future.
-        
-        
-        Future possibilites
-        -------------------
-        
-        A number of possibilites came up in discussions at Simbuild 2018 in Chicago. The biggest takeaway was that the code base for the JSON format and the dot syntax can lead to a universal translator between modelling file formats. The thinking here is that if there exists a schema.JSON for two modelling file structures, the possibility of translating between the two exists.
-        
-        Of course *the proof is in the pudding*. So we are going to write some quick and dirty translators between E+ and DOE2.1E (or EQuest) as well as between the older idds and the new epJSON. Lets see how that goes.
-        
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        Releases
-        --------
-        
-        Date:   Tue Jul 7 08:09:26 2020 -0700
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Fixed issue #48
-        
-        :Problem: No Tutorial for eppy3000
-        :Solution: tutorial for eppy3000
-        
-        + This tutorial is based on eppy turorial
-        + Identifies the gaps in the eppy3000 tagged by TODO in the tutorial
-        + open issues on these TODOs and resolve
-        
-        
-        Release 0.1.3 (2020-07-04)
-        --------------------------
-        
-        Date:   Wed May 13 14:20:34 2020 -0700
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-            fixed issue # 45
-            
-            Problem: setup.py not including folders `oldeppy` and `experimental`
-            Solution: setup.py updated and tested
-        
-        
-        
-        Release 0.1.2 (2020-05-12)
-        --------------------------
-        
-        Date:   Tue May 12 08:11:39 2020 -0700
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-            fixed issue #41
-            
-            Problem: function to get an array of xyz points from the surfaces
-            Solution: function in eppy300.experimental.listfields.surf2list()
-        
-        
-        Date:   Mon May 11 08:15:50 2020 -0700
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-            fixed issue #34
-            
-            Problem: need an easy to use converter between
-            epj (epyy300 format) and idf (eppy format)
-            
-            Solution: functions idf2epj() epj2idf() do this.
-            epj.saveas(filename) and idf.saveas(filename)
-            will save it to disk
-        
-        
-        
-        Date:   Mon May 11 15:35:54 2020 -0700
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-            fixed issue #39
-        
-            **Problem:** need a place to put experimental functions
-            **Solution:** created an experimental folder in eppy3000
-        
-        
-        Date:   Mon May 11 08:15:50 2020 -0700
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-            fixed issue #34
-            
-            Problem: need an easy to use converter between
-            epj (epyy300 format) and idf (eppy format)
-            
-            Solution: functions idf2epj() epj2idf() do this.
-            epj.saveas(filename) and idf.saveas(filename)
-            will save it to disk
-        
-        
-        
-        Sun May 10 09:26:32 2020 -0700
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-            fixed issue #36
-        
-            Problem: modelbuilder.EPJ need savecopy() to fix issue #34
-            Solution: coded EPJ.savecopy and EPJ.jsonstr()
-        
-        
-        
-        
-        
-        Release 0.1.1 (2019-06-06)
-        --------------------------
-        
-        2019-06-06
-        ~~~~~~~~~~
-        
-        - functions to read and write IDF files
-            - issue #20
-        
-        0.1.0 (2018-10-15)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: eppy3000
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+========
+eppy3000
+========
+
+
+.. image:: https://img.shields.io/pypi/v/eppy3000.svg
+        :target: https://pypi.python.org/pypi/eppy3000
+
+.. image:: https://img.shields.io/travis/pyenergyplus/eppy3000.svg
+        :target: https://travis-ci.org/pyenergyplus/eppy3000
+
+.. image:: https://readthedocs.org/projects/eppy3000/badge/?version=latest
+        :target: https://eppy3000.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+
+
+
+E+ scripting using epJSON file format
+
+
+* Free software: Mozilla Public License, v. 2.0
+* Documentation: https://eppy3000.readthedocs.io.
+* Home Page: https://github.com/pyenergyplus/eppy3000
+
+
+Features - so far :-)
+---------------------
+
+* Open and read an epJSON file with *some* `eppy <https://github.com/santoshphilip/eppy>`_ functionality.
+* Right now the `eppy <https://github.com/santoshphilip/eppy>`_ functionality is only partial
+
+
+Background
+----------
+
+E+ has been moving from the IDD/IDF text format to a JSON format. `Eppy <https://github.com/santoshphilip/eppy>`_ reads the old IDD/IDF format. There is a need to have `eppy <https://github.com/santoshphilip/eppy>`_ read the JSON format and/or have a new package that will read the JSON format.
+
+Whats in a name
+---------------
+
+Why is this package called eppy3000 ?
+
+It is a play on the word python3000. Guido van van Rossum said about python in 2007 *"The first time I came up with the idea of Python 3000 was probably at a Python conference in the year 2000. The name was a take on Windows 2000. ...<snip>...  The idea was that Python 3000 would be the first Python release to give up backwards compatibility in favor of making it the best language going forward."*
+
+Eppy3000 will also break backward compatibility with eppy. Also eppy3000 will be written only for python3. Eppy3000 and eppy will continue to remain the best scripting language for modelling :-)
+
+
+So what is eppy3000
+-------------------
+
+This project is an attempt to read JSON file formats and work like eppy. There is some value in trying to do this from scratch. The dot syntax that makes the original eppy useful can be recreated with a couple of lines in eppy3000. It took a lot of deep hacking to make the dot syntax work in the original eppy. Eppy3000 reads the JSON format as a dictionary. The package `Munch <https://github.com/Infinidat/munch>`_ (what was `Bunch <https://github.com/dsc/bunch>`_) allows the use of dot format syntax with a dictionary. The code is as simple as::
+
+    as_json = json.load(open(fname, 'r'))
+    for_dot_syntax = DefaultMunch.fromDict(as_json)
+
+At this point eppy3000 is an exploration to find out what is possible. The API in eppy3000 will not be stable as we explore the possibilities. So, don't use it as production code yet :-)
+
+
+What about eppy
+---------------
+
+Eppy will be continue to be developed and maintained. A major task will be to make eppy read the new JSON formats. Initial investigations shows that it is not too hard to develop this functionality. Internally eppy will continue to use the old format. Hopefully this will make the JSON reading functionality trivially easy. At the moment, E+ maintains a one to one mapping between the old IDD/IDF format and the new JSON format. This mapping is embedded in the file Energy+.schema.epJSON, pointing to an easy compatibility strategy.
+
+In the long term, this may not be a viable strategy, as E+ may totally abandon the IDD/IDF file format breaking the link between JSON and IDD/IDF. Discussion thread at `unmethours <https://unmethours.com/question/36062/hvac-templates-to-be-discontinued/>`_ seems to indicate that this is about 5 yers in the future.
+
+
+Future possibilites
+-------------------
+
+A number of possibilites came up in discussions at Simbuild 2018 in Chicago. The biggest takeaway was that the code base for the JSON format and the dot syntax can lead to a universal translator between modelling file formats. The thinking here is that if there exists a schema.JSON for two modelling file structures, the possibility of translating between the two exists.
+
+Of course *the proof is in the pudding*. So we are going to write some quick and dirty translators between E+ and DOE2.1E (or EQuest) as well as between the older idds and the new epJSON. Lets see how that goes.
+
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+Releases
+--------
+
+
+Release 0.1.13  (2021-03-16)
+----------------------------
+
+2021-03-16
+~~~~~~~~~~
+
+Fixed #76
+
+:Problem: Need easier conversion from IDF to epJSON
+:Solution: ``idffile2epjfile`` will convert a single file and ``idffolder2epjfolder`` will do batch conversion
+
+Date: Mon Jan 18 21:53:40 PST 2021
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+fixed issue #73
+
+:Problem: Would be nice to have an html viewer for epj
+:Solution: pytested eppy3000.epjviewer with sphinx user documentation
+
+Date: Tue Jan 12 14:18:37 PST 2021
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+fixed issue #69
+
+:Problem: no EPJ.run() function
+:Solution: EPJ.run() function implemented
+
+
+Release 0.1.4  (2020-07-09)
+---------------------------
+
+
+Date:   Tue Jul 7 08:09:26 2020 -0700
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Fixed issue #48
+
+:Problem: No Tutorial for eppy3000
+:Solution: tutorial for eppy3000
+
++ This tutorial is based on eppy tutorial
++ Identifies the gaps in the eppy3000 tagged by TODO in the tutorial
++ open issues on these TODOs and resolve
+
+
+Release 0.1.3 (2020-07-04)
+--------------------------
+
+Date:   Wed May 13 14:20:34 2020 -0700
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    fixed issue # 45
+    
+    Problem: setup.py not including folders `oldeppy` and `experimental`
+    Solution: setup.py updated and tested
+
+
+
+Release 0.1.2 (2020-05-12)
+--------------------------
+
+Date:   Tue May 12 08:11:39 2020 -0700
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    fixed issue #41
+    
+    Problem: function to get an array of xyz points from the surfaces
+    Solution: function in eppy300.experimental.listfields.surf2list()
+
+
+Date:   Mon May 11 08:15:50 2020 -0700
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    fixed issue #34
+    
+    Problem: need an easy to use converter between
+    epj (epyy300 format) and idf (eppy format)
+    
+    Solution: functions idf2epj() epj2idf() do this.
+    epj.saveas(filename) and idf.saveas(filename)
+    will save it to disk
+
+
+
+Date:   Mon May 11 15:35:54 2020 -0700
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    fixed issue #39
+
+    **Problem:** need a place to put experimental functions
+    **Solution:** created an experimental folder in eppy3000
+
+
+Date:   Mon May 11 08:15:50 2020 -0700
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    fixed issue #34
+    
+    Problem: need an easy to use converter between
+    epj (epyy300 format) and idf (eppy format)
+    
+    Solution: functions idf2epj() epj2idf() do this.
+    epj.saveas(filename) and idf.saveas(filename)
+    will save it to disk
+
+
+
+Sun May 10 09:26:32 2020 -0700
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    fixed issue #36
+
+    Problem: modelbuilder.EPJ need savecopy() to fix issue #34
+    Solution: coded EPJ.savecopy and EPJ.jsonstr()
+
+
+
+
+
+Release 0.1.1 (2019-06-06)
+--------------------------
+
+2019-06-06
+~~~~~~~~~~
+
+- functions to read and write IDF files
+    - issue #20
+
+0.1.0 (2018-10-15)
+------------------
+
+* First release on PyPI.
```

### Comparing `eppy3000-0.1.4/setup.py` & `eppy3000-0.1.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-with open('README.rst') as readme_file:
+with open("README.rst") as readme_file:
     readme = readme_file.read()
 
-with open('HISTORY.rst') as history_file:
+with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-requirements = ["munch", ]
+requirements = ["munch", "eppy", "json2html"]
 
-setup_requirements = ['pytest-runner', ]
-
-test_requirements = ['pytest', ]
+setup_requirements = [
+    "pytest-runner",
+]
+
+test_requirements = [
+    "pytest",
+]
 
 setup(
     author="Santosh Philip",
-    author_email='santosh@noemail.com',
+    author_email="santosh@noemail.com",
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Developers",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
     ],
     description="E+ scripting using epJSON file format",
     install_requires=requirements,
     license="Mozilla Public License, v. 2.0",
-    long_description=readme + '\n\n' + history,
+    long_description=readme + "\n\n" + history,
     include_package_data=True,
-    keywords='eppy3000',
-    name='eppy3000',
-    packages=find_packages(include=['eppy3000', 'eppy3000.*']),
+    keywords="eppy3000",
+    name="eppy3000",
+    packages=find_packages(include=["eppy3000", "eppy3000.*"]),
     setup_requires=setup_requirements,
-    test_suite='tests',
+    test_suite="tests",
     tests_require=test_requirements,
-    url='https://github.com/pyenergyplus/eppy3000',
-    version='0.1.4',
+    url="https://github.com/pyenergyplus/eppy3000",
+    version="0.1.5",
     zip_safe=False,
 )
```

### Comparing `eppy3000-0.1.4/tests/experimental/test_listfields.py` & `eppy3000-0.1.5/tests/experimental/test_listfields.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 import pytest
 from io import StringIO
 
 from eppy3000.experimental import listfields
 from eppy3000.modelmaker import EPJ
 
 
-@pytest.mark.parametrize('surfobjecttxt, expected', [
-    (
-"""{ "BuildingSurface:Detailed": {
+@pytest.mark.parametrize(
+    "surfobjecttxt, expected",
+    [
+        (
+            """{ "BuildingSurface:Detailed": {
         "BACK-1": {
             "construction_name": "WALL-1",
             "idf_max_extensible_fields": 12,
             "idf_max_fields": 22,
             "idf_order": 101,
             "number_of_vertices": 4,
             "outside_boundary_condition": "Outdoors",
@@ -32,19 +34,19 @@
                 }
             ],
             "view_factor_to_ground": 0.5,
             "wind_exposure": "WindExposed",
             "zone_name": "SPACE3-1"
         }
 }
-}"""
-,
-    [(30.5, 15.2, 2.4), (1, 2, 3)]
-    ), # surfobjecttxt, expected
-])
+}""",
+            [(30.5, 15.2, 2.4), (1, 2, 3)],
+        ),  # surfobjecttxt, expected
+    ],
+)
 def test_surf2list(surfobjecttxt, expected):
     """py.test for surf2list"""
     epj = EPJ(StringIO(surfobjecttxt))
-    surfs = epj.epobjects['BuildingSurface:Detailed']
+    surfs = epj.epobjects["BuildingSurface:Detailed"]
     surfobject = surfs[0]
     result = listfields.surf2list(surfobject)
-    assert result == expected
+    assert result == expected
```

### Comparing `eppy3000-0.1.4/tests/oldeppytests.py` & `eppy3000-0.1.5/tests/oldeppytests.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,34 @@
 from io import StringIO
 from pathlib import Path
 import os
 
 # from eppy3000 import idfjsonconverter
 from tests import schemafortesting
 from eppy3000.modelmaker import EPJ
+
 # import eppy3000.oldeppy.idfjsonconverter as idfjsonconverter
 import eppy3000.oldeppy as oldeppy
 import eppy
 
 SCHEMA_FILE = schemafortesting.schema_file
 
 # path for iddfile -> clean this later
 THIS_DIR = Path(os.path.dirname(os.path.abspath(__file__)))
-IDDFILE = THIS_DIR / os.pardir / 'eppy3000/resources/snippets/V9_1/iddV9_1_snippet.idd'
+IDDFILE = THIS_DIR / os.pardir / "eppy3000/resources/snippets/V9_1/iddV9_1_snippet.idd"
 iddfile = IDDFILE
 
+
 def test_idf2idj_epj2idf():
     """py.test for idf2idj and epj2idf"""
-    # rearranged the order of so that it matches the order in the idd file. 
+    # rearranged the order of so that it matches the order in the idd file.
     # So the tests can pass
-    data = (("""
+    data = (
+        (
+            """
   Version,9.1;
 
 Building,
     Bldg one,                !- Name
     30,                     !- North Axis {deg}
     City,                    !- Terrain
     0.04,                    !- Loads Convergence Tolerance Value
@@ -98,18 +102,18 @@
     Reheat Coil Air Inlet Node,  !- Node 4 Name
     VAV Sys 1 Outlet Node;   !- Node 5 Name
 
 OutdoorAir:NodeList,
     OutsideAirInletNodes;    !- Node or NodeList Name 1
 
 """,  # noqa: E501
-),  # idftxt
+        ),  # idftxt
     )
-    for idftxt, in data:
-        iddhandle = open(iddfile, 'r')
+    for (idftxt,) in data:
+        iddhandle = open(iddfile, "r")
         iddtxt = iddhandle.read()
         iddstringio = StringIO(iddtxt)
 
         # convert idf to epj, then epj to idf and lastly idf to epj
         # compare the first epj.json and last epj.json
         idfhandle = StringIO(idftxt)
         idf = eppy.openidf(idfhandle, idd=iddstringio)
```

### Comparing `eppy3000-0.1.4/tests/schemafortesting.py` & `eppy3000-0.1.5/tests/schemafortesting.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 # =======================================================================
 """the schema used for testing is in this module
 It will be loaded only once, since that is how imports work"""
 
 import os
 
 from eppy3000 import epschema
+
 THIS_DIR = os.path.dirname(os.path.abspath(__file__))
 
-RESOURCES_DIR = os.path.join(THIS_DIR, os.pardir, 'eppy3000', 'resources')
-VERSION = '9-0-1'  # current default for integration tests on local system
+RESOURCES_DIR = os.path.join(THIS_DIR, os.pardir, "eppy3000", "resources")
+VERSION = "9-0-1"  # current default for integration tests on local system
 
 
-SCHEMA_FILES = os.path.join(RESOURCES_DIR, 'schema')
+SCHEMA_FILES = os.path.join(RESOURCES_DIR, "schema")
 TEST_SCHEMA = f"V{VERSION[:3].replace('-', '_')}/Energy+.schema.epJSON"
 schema_file = os.path.join(SCHEMA_FILES, TEST_SCHEMA)
 
 schema = epschema.read_epschema_asmunch(schema_file)
 
 
 # IDD_FILES = os.path.join(RESOURCES_DIR, 'iddfiles')
```

### Comparing `eppy3000-0.1.4/tests/test_epschema.py` & `eppy3000-0.1.5/tests/test_epschema.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from tests import schemafortesting
 
 
 def test_read_epschema_asmunch():
     """py.test for read_epschema_asmunch"""
     SCHEMA_FILE = schemafortesting.schema_file
-    schemahandle = open(SCHEMA_FILE, 'r')
+    schemahandle = open(SCHEMA_FILE, "r")
     result = epschema.read_epschema_asmunch(schemahandle)
     assert isinstance(result, epschema.EPSchemaMunch)
 
     result = epschema.read_epschema_asmunch(SCHEMA_FILE)
     assert isinstance(result, epschema.EPSchemaMunch)
 
     schemahandle = schemafortesting.schema
@@ -232,40 +232,48 @@
                     }
                 }
             },
             "extensible_size": 1.0
         }
     },
     "epJSON_schema_build": "40101eaafd"
-}"""   # noqa: E501
+}"""  # noqa: E501
 
     # expected
     version = "8.9.0"
-    required = ['Building', 'GlobalGeometryRules']
-    epschemaobjectskeys = ['Building', 'OutdoorAir:NodeList']
-    buildingkeys = ['solar_distribution', 'terrain', 'north_axis',
-                    'maximum_number_of_warmup_days',
-                    'loads_convergence_tolerance_value',
-                    'temperature_convergence_tolerance_value',
-                    'minimum_number_of_warmup_days']
+    required = ["Building", "GlobalGeometryRules"]
+    epschemaobjectskeys = ["Building", "OutdoorAir:NodeList"]
+    buildingkeys = [
+        "solar_distribution",
+        "terrain",
+        "north_axis",
+        "maximum_number_of_warmup_days",
+        "loads_convergence_tolerance_value",
+        "temperature_convergence_tolerance_value",
+        "minimum_number_of_warmup_days",
+    ]
     buildingterraintype = "string"
-    bfieldnames = ['solar_distribution', 'terrain', 'north_axis',
-                   'maximum_number_of_warmup_days',
-                   'loads_convergence_tolerance_value',
-                   'temperature_convergence_tolerance_value',
-                   'minimum_number_of_warmup_days']
+    bfieldnames = [
+        "solar_distribution",
+        "terrain",
+        "north_axis",
+        "maximum_number_of_warmup_days",
+        "loads_convergence_tolerance_value",
+        "temperature_convergence_tolerance_value",
+        "minimum_number_of_warmup_days",
+    ]
     fieldnameslist = None  # not yet coded
     #
     # tests
     fhandle = StringIO(txt)
     result = epschema.EPSchema(fhandle)
 
     assert version == result.version
     assert required == result.required
     assert epschemaobjectskeys == list(result.epschemaobjects.keys())
-    assert buildingkeys == list(result.epschemaobjects['Building'].keys())
+    assert buildingkeys == list(result.epschemaobjects["Building"].keys())
     #
-    bldg = result.epschemaobjects['Building']
-    assert buildingterraintype == bldg.fieldproperty('terrain')['type']
-    assert bfieldnames == result.epschemaobjects['Building'].fieldnames()
-    oairnode = result.epschemaobjects['OutdoorAir:NodeList']
+    bldg = result.epschemaobjects["Building"]
+    assert buildingterraintype == bldg.fieldproperty("terrain")["type"]
+    assert bfieldnames == result.epschemaobjects["Building"].fieldnames()
+    oairnode = result.epschemaobjects["OutdoorAir:NodeList"]
     assert fieldnameslist == oairnode.fieldnames_list()
```

### Comparing `eppy3000-0.1.4/tests/test_rawidf.py` & `eppy3000-0.1.5/tests/test_rawidf.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,37 +38,37 @@
     CONTINUOUS;              !- Numeric Type
     """
     expected = {
         "version": [["version", "9.0"]],
         "Timestep": [["Timestep", "4"]],
         "ScheduleTypeLimits": [
             ["ScheduleTypeLimits", "Fraction", "0.0", "1.0", "CONTINUOUS"],
-            ["ScheduleTypeLimits", "Other", "0.0", "1.0", "CONTINUOUS"]]
-        }
+            ["ScheduleTypeLimits", "Other", "0.0", "1.0", "CONTINUOUS"],
+        ],
+    }
     result = rawidf.readrawidf(StringIO(txt))
     assert result == expected
 
 
 def test_rawidf2str():
     """py.test rawidf2str"""
-    rawdata = {
-        "version".upper(): [["version", "9.0"]]
-        }
+    rawdata = {"version".upper(): [["version", "9.0"]]}
     expected = """VERSION,
     9.0;
 """
     result = rawidf.rawidf2str(rawdata)
     assert result == expected
     rawdata = {
         "version".upper(): [["version", "9.0"]],
         "Timestep".upper(): [["Timestep", "4"]],
         "ScheduleTypeLimits".upper(): [
             ["ScheduleTypeLimits", "Fraction", "0.0", "1.0", "CONTINUOUS"],
-            ["ScheduleTypeLimits", "Other", "0.0", "1.0", "CONTINUOUS"]]
-        }
+            ["ScheduleTypeLimits", "Other", "0.0", "1.0", "CONTINUOUS"],
+        ],
+    }
     order = ["TIMESTEP", "VERSION", "SCHEDULETYPELIMITS", "badkey"]
     expected = """TIMESTEP,
     4;
 
 VERSION,
     9.0;
```

### Comparing `eppy3000-0.1.4/tests/test_readidf.py` & `eppy3000-0.1.5/tests/test_readidf.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,48 +11,51 @@
 import eppy3000.readepj as readepj
 from eppy3000.epMunch import EPMunch
 
 
 def test_readepjjson():
     """py.test for readepjjson"""
     dct = dict(
-            a=dict(aa=dict(z=-1, y=-2), bb=dict(zz=-11, yy=-22)),
-            b=dict(cc=dict(ab=12, bc=23), dd=dict(cd=34, de=45)))
+        a=dict(aa=dict(z=-1, y=-2), bb=dict(zz=-11, yy=-22)),
+        b=dict(cc=dict(ab=12, bc=23), dd=dict(cd=34, de=45)),
+    )
     dctstr = json.dumps(dct)
     fhandle = StringIO(dctstr)
     result = readepj.readepjjson(fhandle)
     assert isinstance(result, EPMunch)
 
 
 def test_addeppykeys():
     """py.test for addeppykeys"""
     dct = dict(
-            a=dict(aa=dict(z=-1, y=-2), bb=dict(zz=-11, yy=-22)),
-            b=dict(cc=dict(ab=12, bc=23), dd=dict(cd=34, de=45)))
+        a=dict(aa=dict(z=-1, y=-2), bb=dict(zz=-11, yy=-22)),
+        b=dict(cc=dict(ab=12, bc=23), dd=dict(cd=34, de=45)),
+    )
     dctstr = json.dumps(dct)
     fhandle = StringIO(dctstr)
     epmunch = readepj.readepjjson(fhandle)
     epobject = epmunch.a.aa
-    assert 'eppykey' in epobject
-    assert 'eppyname' in epobject
+    assert "eppykey" in epobject
+    assert "eppyname" in epobject
 
 
 def test_removeeppykeys():
     """py.test for removeeppykeys"""
     dct = dict(
-            a=dict(aa=dict(z=-1, y=-2), bb=dict(zz=-11, yy=-22)),
-            b=dict(cc=dict(ab=12, bc=23), dd=dict(cd=34, de=45)))
+        a=dict(aa=dict(z=-1, y=-2), bb=dict(zz=-11, yy=-22)),
+        b=dict(cc=dict(ab=12, bc=23), dd=dict(cd=34, de=45)),
+    )
     dctstr = json.dumps(dct)
     # test for rkeys=None
     fhandle = StringIO(dctstr)
     epmunch = readepj.readepjjson(fhandle)
     readepj.removeeppykeys(epmunch)
     epobject = epmunch.a.aa
-    assert 'eppykey' not in epobject
-    assert 'eppyname' not in epobject
+    assert "eppykey" not in epobject
+    assert "eppyname" not in epobject
     # test for rkeys=['eppykey']
     fhandle = StringIO(dctstr)
     epmunch = readepj.readepjjson(fhandle)
-    readepj.removeeppykeys(epmunch, rkeys=['eppykey'])
+    readepj.removeeppykeys(epmunch, rkeys=["eppykey"])
     epobject = epmunch.a.aa
-    assert 'eppykey' not in epobject
-    assert 'eppyname' in epobject
+    assert "eppykey" not in epobject
+    assert "eppyname" in epobject
```

