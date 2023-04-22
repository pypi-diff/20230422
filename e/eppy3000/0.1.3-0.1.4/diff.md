# Comparing `tmp/eppy3000-0.1.3.tar.gz` & `tmp/eppy3000-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eppy3000-0.1.3.tar", last modified: Wed May 13 21:30:21 2020, max compression
+gzip compressed data, was "dist/eppy3000-0.1.4.tar", last modified: Thu Jul  9 19:02:45 2020, max compression
```

## Comparing `eppy3000-0.1.3.tar` & `eppy3000-0.1.4.tar`

### file list

```diff
@@ -1,73 +1,59 @@
-drwxr-xr-x   0 santoshphilip   (503) staff       (20)        0 2020-05-13 21:30:21.000000 eppy3000-0.1.3/
--rw-r--r--   0 santoshphilip   (503) staff       (20)      118 2020-05-13 20:20:24.000000 eppy3000-0.1.3/AUTHORS.rst
--rw-r--r--   0 santoshphilip   (503) staff       (20)     1417 2020-05-13 20:20:24.000000 eppy3000-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0 santoshphilip   (503) staff       (20)      227 2020-05-13 20:20:24.000000 eppy3000-0.1.3/HISTORY.rst
--rw-r--r--   0 santoshphilip   (503) staff       (20)    16725 2020-05-13 20:20:24.000000 eppy3000-0.1.3/LICENSE
--rw-r--r--   0 santoshphilip   (503) staff       (20)      262 2020-05-13 20:20:24.000000 eppy3000-0.1.3/MANIFEST.in
--rw-r--r--   0 santoshphilip   (503) staff       (20)     6313 2020-05-13 21:30:21.000000 eppy3000-0.1.3/PKG-INFO
--rw-r--r--   0 santoshphilip   (503) staff       (20)     4545 2020-05-13 20:20:24.000000 eppy3000-0.1.3/README.rst
-drwxr-xr-x   0 santoshphilip   (503) staff       (20)        0 2020-05-13 21:30:21.000000 eppy3000-0.1.3/docs/
--rw-r--r--   0 santoshphilip   (503) staff       (20)      609 2020-05-13 20:20:24.000000 eppy3000-0.1.3/docs/Makefile
-drwxr-xr-x   0 santoshphilip   (503) staff       (20)        0 2020-05-13 21:30:21.000000 eppy3000-0.1.3/docs/_build/
-drwxr-xr-x   0 santoshphilip   (503) staff       (20)        0 2020-05-13 21:30:21.000000 eppy3000-0.1.3/docs/_build/html/
-drwxr-xr-x   0 santoshphilip   (503) staff       (20)        0 2020-05-13 21:30:21.000000 eppy3000-0.1.3/docs/_build/html/_static/
--rw-r--r--   0 santoshphilip   (503) staff       (20)      673 2020-05-13 20:36:10.000000 eppy3000-0.1.3/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0 santoshphilip   (503) staff       (20)      756 2020-05-13 20:36:10.000000 eppy3000-0.1.3/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 santoshphilip   (503) staff       (20)      829 2020-05-13 20:36:10.000000 eppy3000-0.1.3/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 santoshphilip   (503) staff       (20)      641 2020-05-13 20:36:10.000000 eppy3000-0.1.3/docs/_build/html/_static/comment.png
--rw-r--r--   0 santoshphilip   (503) staff       (20)      222 2020-05-13 20:36:10.000000 eppy3000-0.1.3/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 santoshphilip   (503) staff       (20)      202 2020-05-13 20:36:10.000000 eppy3000-0.1.3/docs/_build/html/_static/down.png
--rw-r--r--   0 santoshphilip   (503) staff       (20)      286 2020-05-13 20:36:10.000000 eppy3000-0.1.3/docs/_build/html/_static/file.png
--rw-r--r--   0 santoshphilip   (503) staff       (20)       90 2020-05-13 20:36:10.000000 eppy3000-0.1.3/docs/_build/html/_static/minus.png
--rw-r--r--   0 santoshphilip   (503) staff       (20)       90 2020-05-13 20:36:10.000000 eppy3000-0.1.3/docs/_build/html/_static/plus.png
--rw-r--r--   0 santoshphilip   (503) staff       (20)      214 2020-05-13 20:36:10.000000 eppy3000-0.1.3/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 santoshphilip   (503) staff       (20)      203 2020-05-13 20:36:10.000000 eppy3000-0.1.3/docs/_build/html/_static/up.png
--rw-r--r--   0 santoshphilip   (503) staff       (20)       28 2020-05-13 20:20:24.000000 eppy3000-0.1.3/docs/authors.rst
--rwxr-xr-x   0 santoshphilip   (503) staff       (20)     4869 2020-05-13 20:20:24.000000 eppy3000-0.1.3/docs/conf.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)       33 2020-05-13 20:20:24.000000 eppy3000-0.1.3/docs/contributing.rst
--rw-r--r--   0 santoshphilip   (503) staff       (20)      189 2020-05-13 20:20:24.000000 eppy3000-0.1.3/docs/eppy3000.experimental.rst
--rw-r--r--   0 santoshphilip   (503) staff       (20)      389 2020-05-13 20:20:24.000000 eppy3000-0.1.3/docs/eppy3000.oldeppy.rst
--rw-r--r--   0 santoshphilip   (503) staff       (20)     1280 2020-05-13 21:25:15.000000 eppy3000-0.1.3/docs/eppy3000.rst
--rw-r--r--   0 santoshphilip   (503) staff       (20)       28 2020-05-13 20:20:24.000000 eppy3000-0.1.3/docs/history.rst
--rw-r--r--   0 santoshphilip   (503) staff       (20)      320 2020-05-13 20:20:24.000000 eppy3000-0.1.3/docs/index.rst
--rw-r--r--   0 santoshphilip   (503) staff       (20)     1138 2020-05-13 20:20:24.000000 eppy3000-0.1.3/docs/installation.rst
--rw-r--r--   0 santoshphilip   (503) staff       (20)      770 2020-05-13 20:20:24.000000 eppy3000-0.1.3/docs/make.bat
--rw-r--r--   0 santoshphilip   (503) staff       (20)       61 2020-05-13 21:25:15.000000 eppy3000-0.1.3/docs/modules.rst
--rw-r--r--   0 santoshphilip   (503) staff       (20)       27 2020-05-13 20:20:24.000000 eppy3000-0.1.3/docs/readme.rst
-drwxr-xr-x   0 santoshphilip   (503) staff       (20)        0 2020-05-13 21:30:21.000000 eppy3000-0.1.3/eppy3000/
--rw-r--r--   0 santoshphilip   (503) staff       (20)      154 2020-05-13 21:27:33.000000 eppy3000-0.1.3/eppy3000/__init__.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)     5149 2020-05-13 20:20:24.000000 eppy3000-0.1.3/eppy3000/epMunch.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)       44 2020-05-13 20:20:24.000000 eppy3000-0.1.3/eppy3000/eppy3000.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)     2205 2020-05-13 20:20:24.000000 eppy3000-0.1.3/eppy3000/epschema.py
-drwxr-xr-x   0 santoshphilip   (503) staff       (20)        0 2020-05-13 21:30:21.000000 eppy3000-0.1.3/eppy3000/experimental/
--rw-r--r--   0 santoshphilip   (503) staff       (20)      542 2020-05-13 20:20:24.000000 eppy3000-0.1.3/eppy3000/experimental/__init__.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)      130 2020-05-13 20:20:24.000000 eppy3000-0.1.3/eppy3000/experimental/hello.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)      688 2020-05-13 20:20:24.000000 eppy3000-0.1.3/eppy3000/experimental/listfields.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)     6652 2020-05-13 20:20:24.000000 eppy3000-0.1.3/eppy3000/idfjsonconverter.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)     5387 2020-05-13 20:20:24.000000 eppy3000-0.1.3/eppy3000/modelmaker.py
-drwxr-xr-x   0 santoshphilip   (503) staff       (20)        0 2020-05-13 21:30:21.000000 eppy3000-0.1.3/eppy3000/oldeppy/
--rw-r--r--   0 santoshphilip   (503) staff       (20)     1361 2020-05-13 20:20:24.000000 eppy3000-0.1.3/eppy3000/oldeppy/__init__.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)     2192 2020-05-13 20:20:24.000000 eppy3000-0.1.3/eppy3000/rawidf.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)     2821 2020-05-13 20:20:24.000000 eppy3000-0.1.3/eppy3000/readepj.py
-drwxr-xr-x   0 santoshphilip   (503) staff       (20)        0 2020-05-13 21:30:21.000000 eppy3000-0.1.3/eppy3000.egg-info/
--rw-r--r--   0 santoshphilip   (503) staff       (20)     6313 2020-05-13 21:30:20.000000 eppy3000-0.1.3/eppy3000.egg-info/PKG-INFO
--rw-r--r--   0 santoshphilip   (503) staff       (20)     1521 2020-05-13 21:30:20.000000 eppy3000-0.1.3/eppy3000.egg-info/SOURCES.txt
--rw-r--r--   0 santoshphilip   (503) staff       (20)        1 2020-05-13 21:30:20.000000 eppy3000-0.1.3/eppy3000.egg-info/dependency_links.txt
--rw-r--r--   0 santoshphilip   (503) staff       (20)        1 2020-05-13 21:30:20.000000 eppy3000-0.1.3/eppy3000.egg-info/not-zip-safe
--rw-r--r--   0 santoshphilip   (503) staff       (20)        6 2020-05-13 21:30:20.000000 eppy3000-0.1.3/eppy3000.egg-info/requires.txt
--rw-r--r--   0 santoshphilip   (503) staff       (20)        9 2020-05-13 21:30:20.000000 eppy3000-0.1.3/eppy3000.egg-info/top_level.txt
--rw-r--r--   0 santoshphilip   (503) staff       (20)      450 2020-05-13 21:30:21.000000 eppy3000-0.1.3/setup.cfg
--rwxr-xr-x   0 santoshphilip   (503) staff       (20)     1394 2020-05-13 21:27:33.000000 eppy3000-0.1.3/setup.py
-drwxr-xr-x   0 santoshphilip   (503) staff       (20)        0 2020-05-13 21:30:21.000000 eppy3000-0.1.3/tests/
--rw-r--r--   0 santoshphilip   (503) staff       (20)        0 2020-05-13 20:20:24.000000 eppy3000-0.1.3/tests/__init__.py
-drwxr-xr-x   0 santoshphilip   (503) staff       (20)        0 2020-05-13 21:30:21.000000 eppy3000-0.1.3/tests/experimental/
--rw-r--r--   0 santoshphilip   (503) staff       (20)        1 2020-05-13 20:20:24.000000 eppy3000-0.1.3/tests/experimental/__init__.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)     1467 2020-05-13 20:20:24.000000 eppy3000-0.1.3/tests/experimental/test_listfields.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)     4431 2020-05-13 20:20:24.000000 eppy3000-0.1.3/tests/oldeppytests.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)     1927 2020-05-13 20:20:24.000000 eppy3000-0.1.3/tests/schemafortesting.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)     5974 2020-05-13 20:20:24.000000 eppy3000-0.1.3/tests/test_epMunch.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)    11811 2020-05-13 20:20:24.000000 eppy3000-0.1.3/tests/test_epschema.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)     4626 2020-05-13 20:20:24.000000 eppy3000-0.1.3/tests/test_idfjsonconverter.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)     2754 2020-05-13 20:20:24.000000 eppy3000-0.1.3/tests/test_modelmaker.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)     2359 2020-05-13 20:20:24.000000 eppy3000-0.1.3/tests/test_rawidf.py
--rw-r--r--   0 santoshphilip   (503) staff       (20)     2019 2020-05-13 20:20:24.000000 eppy3000-0.1.3/tests/test_readidf.py
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      118 2020-04-07 19:39:27.000000 eppy3000-0.1.4/AUTHORS.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     1417 2020-04-07 19:39:27.000000 eppy3000-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     2241 2020-07-09 18:53:09.000000 eppy3000-0.1.4/HISTORY.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)    16725 2020-04-07 19:39:27.000000 eppy3000-0.1.4/LICENSE
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      262 2020-04-07 19:39:27.000000 eppy3000-0.1.4/MANIFEST.in
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     9023 2020-07-09 19:02:45.000000 eppy3000-0.1.4/PKG-INFO
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     4545 2020-04-07 19:39:27.000000 eppy3000-0.1.4/README.rst
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/docs/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      609 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/Makefile
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       28 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/authors.rst
+-rwxr-xr-x   0 santoshphilip   (501) staff       (20)     4869 2020-07-09 18:43:53.000000 eppy3000-0.1.4/docs/conf.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       33 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/contributing.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      189 2020-07-09 18:43:53.000000 eppy3000-0.1.4/docs/eppy3000.experimental.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      389 2020-07-09 18:43:53.000000 eppy3000-0.1.4/docs/eppy3000.oldeppy.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     1280 2020-07-09 18:43:53.000000 eppy3000-0.1.4/docs/eppy3000.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       28 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/history.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      346 2020-07-09 18:43:53.000000 eppy3000-0.1.4/docs/index.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     1138 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/installation.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      770 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/make.bat
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       61 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/modules.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       27 2020-04-07 19:39:27.000000 eppy3000-0.1.4/docs/readme.rst
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      154 2020-07-09 18:53:50.000000 eppy3000-0.1.4/eppy3000/__init__.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     5149 2020-04-07 19:39:27.000000 eppy3000-0.1.4/eppy3000/epMunch.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       44 2020-04-07 19:39:27.000000 eppy3000-0.1.4/eppy3000/eppy3000.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     2205 2020-07-09 18:43:53.000000 eppy3000-0.1.4/eppy3000/epschema.py
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000/experimental/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      542 2020-07-09 18:43:53.000000 eppy3000-0.1.4/eppy3000/experimental/__init__.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      130 2020-07-09 18:43:53.000000 eppy3000-0.1.4/eppy3000/experimental/hello.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      688 2020-07-09 18:43:53.000000 eppy3000-0.1.4/eppy3000/experimental/listfields.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     6652 2020-07-09 18:43:53.000000 eppy3000-0.1.4/eppy3000/idfjsonconverter.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     5387 2020-07-09 18:43:53.000000 eppy3000-0.1.4/eppy3000/modelmaker.py
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000/oldeppy/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     1362 2020-07-09 18:43:53.000000 eppy3000-0.1.4/eppy3000/oldeppy/__init__.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     2192 2020-04-07 19:39:27.000000 eppy3000-0.1.4/eppy3000/rawidf.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     2821 2020-04-07 19:39:27.000000 eppy3000-0.1.4/eppy3000/readepj.py
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000.egg-info/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     9023 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000.egg-info/PKG-INFO
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     1105 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000.egg-info/SOURCES.txt
+-rw-r--r--   0 santoshphilip   (501) staff       (20)        1 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000.egg-info/dependency_links.txt
+-rw-r--r--   0 santoshphilip   (501) staff       (20)        1 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000.egg-info/not-zip-safe
+-rw-r--r--   0 santoshphilip   (501) staff       (20)        6 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000.egg-info/requires.txt
+-rw-r--r--   0 santoshphilip   (501) staff       (20)        9 2020-07-09 19:02:45.000000 eppy3000-0.1.4/eppy3000.egg-info/top_level.txt
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      450 2020-07-09 19:02:45.000000 eppy3000-0.1.4/setup.cfg
+-rwxr-xr-x   0 santoshphilip   (501) staff       (20)     1394 2020-07-09 18:53:50.000000 eppy3000-0.1.4/setup.py
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/tests/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)        0 2020-04-07 19:39:27.000000 eppy3000-0.1.4/tests/__init__.py
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2020-07-09 19:02:45.000000 eppy3000-0.1.4/tests/experimental/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)        1 2020-07-09 18:43:54.000000 eppy3000-0.1.4/tests/experimental/__init__.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     1467 2020-07-09 18:43:54.000000 eppy3000-0.1.4/tests/experimental/test_listfields.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     4431 2020-07-09 18:43:54.000000 eppy3000-0.1.4/tests/oldeppytests.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     1927 2020-07-09 18:43:54.000000 eppy3000-0.1.4/tests/schemafortesting.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     5974 2020-04-07 19:39:27.000000 eppy3000-0.1.4/tests/test_epMunch.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)    11811 2020-04-07 19:39:27.000000 eppy3000-0.1.4/tests/test_epschema.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     4626 2020-07-09 18:43:54.000000 eppy3000-0.1.4/tests/test_idfjsonconverter.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     2754 2020-07-09 18:43:54.000000 eppy3000-0.1.4/tests/test_modelmaker.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     2359 2020-04-07 19:39:27.000000 eppy3000-0.1.4/tests/test_rawidf.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     2019 2020-04-07 19:39:27.000000 eppy3000-0.1.4/tests/test_readidf.py
```

### Comparing `eppy3000-0.1.3/CONTRIBUTING.rst` & `eppy3000-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/LICENSE` & `eppy3000-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/README.rst` & `eppy3000-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/docs/Makefile` & `eppy3000-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/docs/conf.py` & `eppy3000-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/docs/eppy3000.rst` & `eppy3000-0.1.4/docs/eppy3000.rst`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/docs/installation.rst` & `eppy3000-0.1.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/docs/make.bat` & `eppy3000-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/eppy3000/epMunch.py` & `eppy3000-0.1.4/eppy3000/epMunch.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/eppy3000/epschema.py` & `eppy3000-0.1.4/eppy3000/epschema.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/eppy3000/experimental/__init__.py` & `eppy3000-0.1.4/eppy3000/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/eppy3000/experimental/listfields.py` & `eppy3000-0.1.4/eppy3000/experimental/listfields.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/eppy3000/idfjsonconverter.py` & `eppy3000-0.1.4/eppy3000/idfjsonconverter.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/eppy3000/modelmaker.py` & `eppy3000-0.1.4/eppy3000/modelmaker.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/eppy3000/oldeppy/__init__.py` & `eppy3000-0.1.4/eppy3000/oldeppy/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
     return EPJ(StringIO(epjstr))
     
     
 def epj2idf(epj, epjsonhandle, iddhandle=None):
     """convert json to idf"""
     jsonhandle = epj.savecopy()
     idfstr =  eppy3000.idfjsonconverter.json2idf(jsonhandle, epjsonhandle) 
-    return eppy.openidf(StringIO(idfstr), idd=iddhandle)
+    return eppy.openidf(StringIO(idfstr), idd=iddhandle)
```

### Comparing `eppy3000-0.1.3/eppy3000/rawidf.py` & `eppy3000-0.1.4/eppy3000/rawidf.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/eppy3000/readepj.py` & `eppy3000-0.1.4/eppy3000/readepj.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/setup.py` & `eppy3000-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     keywords='eppy3000',
     name='eppy3000',
     packages=find_packages(include=['eppy3000', 'eppy3000.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/pyenergyplus/eppy3000',
-    version='0.1.3',
+    version='0.1.4',
     zip_safe=False,
 )
```

### Comparing `eppy3000-0.1.3/tests/experimental/test_listfields.py` & `eppy3000-0.1.4/tests/experimental/test_listfields.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/tests/oldeppytests.py` & `eppy3000-0.1.4/tests/oldeppytests.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/tests/schemafortesting.py` & `eppy3000-0.1.4/tests/schemafortesting.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/tests/test_epMunch.py` & `eppy3000-0.1.4/tests/test_epMunch.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/tests/test_epschema.py` & `eppy3000-0.1.4/tests/test_epschema.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/tests/test_idfjsonconverter.py` & `eppy3000-0.1.4/tests/test_idfjsonconverter.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/tests/test_modelmaker.py` & `eppy3000-0.1.4/tests/test_modelmaker.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/tests/test_rawidf.py` & `eppy3000-0.1.4/tests/test_rawidf.py`

 * *Files identical despite different names*

### Comparing `eppy3000-0.1.3/tests/test_readidf.py` & `eppy3000-0.1.4/tests/test_readidf.py`

 * *Files identical despite different names*

