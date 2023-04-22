# Comparing `tmp/pygnuutils-0.0.6.tar.gz` & `tmp/pygnuutils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygnuutils-0.0.6.tar", last modified: Sun Nov 27 13:39:50 2022, max compression
+gzip compressed data, was "pygnuutils-0.0.7.tar", last modified: Sat Apr 22 21:14:31 2023, max compression
```

## Comparing `pygnuutils-0.0.6.tar` & `pygnuutils-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 13:39:50.959802 pygnuutils-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2308 2022-11-27 13:39:50.959802 pygnuutils-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 13:39:50.959802 pygnuutils-0.0.6/pygnuutils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/pygnuutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      420 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/pygnuutils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/pygnuutils/basename.py
--rw-r--r--   0 runner    (1001) docker     (122)     8496 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/pygnuutils/basenc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 13:39:50.959802 pygnuutils-0.0.6/pygnuutils/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/pygnuutils/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      390 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/pygnuutils/cli/basename.py
--rw-r--r--   0 runner    (1001) docker     (122)     1088 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/pygnuutils/cli/basenc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9746 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/pygnuutils/cli/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      174 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/pygnuutils/cli/yes.py
--rw-r--r--   0 runner    (1001) docker     (122)      179 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/pygnuutils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2580 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/pygnuutils/filevercmp.py
--rw-r--r--   0 runner    (1001) docker     (122)     6071 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/pygnuutils/human_readable.py
--rw-r--r--   0 runner    (1001) docker     (122)    39147 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/pygnuutils/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      552 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/pygnuutils/yes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 13:39:50.959802 pygnuutils-0.0.6/pygnuutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2308 2022-11-27 13:39:50.000000 pygnuutils-0.0.6/pygnuutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      558 2022-11-27 13:39:50.000000 pygnuutils-0.0.6/pygnuutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-27 13:39:50.000000 pygnuutils-0.0.6/pygnuutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2022-11-27 13:39:50.000000 pygnuutils-0.0.6/pygnuutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2022-11-27 13:39:50.000000 pygnuutils-0.0.6/pygnuutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-11-27 13:39:50.000000 pygnuutils-0.0.6/pygnuutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-27 13:39:50.959802 pygnuutils-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1544 2022-11-27 13:39:38.000000 pygnuutils-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:14:31.565856 pygnuutils-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-22 21:14:31.565856 pygnuutils-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:14:31.561856 pygnuutils-0.0.7/pygnuutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/basenc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:14:31.565856 pygnuutils-0.0.7/pygnuutils/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/cli/basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/cli/basenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/cli/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/cli/yes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/filevercmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/human_readable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39147 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/yes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:14:31.565856 pygnuutils-0.0.7/pygnuutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-22 21:14:31.000000 pygnuutils-0.0.7/pygnuutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-22 21:14:31.000000 pygnuutils-0.0.7/pygnuutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 21:14:31.000000 pygnuutils-0.0.7/pygnuutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-22 21:14:31.000000 pygnuutils-0.0.7/pygnuutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-22 21:14:31.000000 pygnuutils-0.0.7/pygnuutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 21:14:31.000000 pygnuutils-0.0.7/pygnuutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 21:14:31.565856 pygnuutils-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/setup.py
```

### Comparing `pygnuutils-0.0.6/LICENSE` & `pygnuutils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.6/PKG-INFO` & `pygnuutils-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygnuutils
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python implementation for GNU utils
 Home-page: https://github.com/matan1008/pygnuutils
 Author: Matan Perelman
 Project-URL: pygnuutils, https://github.com/matan1008/pygnuutils
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pygnuutils-0.0.6/README.md` & `pygnuutils-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.6/pygnuutils/basename.py` & `pygnuutils-0.0.7/pygnuutils/basename.py`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.6/pygnuutils/basenc.py` & `pygnuutils-0.0.7/pygnuutils/basenc.py`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.6/pygnuutils/cli/basenc.py` & `pygnuutils-0.0.7/pygnuutils/cli/basenc.py`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.6/pygnuutils/cli/ls.py` & `pygnuutils-0.0.7/pygnuutils/cli/ls.py`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.6/pygnuutils/filevercmp.py` & `pygnuutils-0.0.7/pygnuutils/filevercmp.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,16 @@
         while (s1 and not s1[0].isdigit()) or (s2 and not s2[0].isdigit()):
             s1_c = order(s1[0]) if s1 else 0
             s2_c = order(s2[0]) if s2 else 0
             if s1_c != s2_c:
                 return s1_c - s2_c
             s1 = s1[1:]
             s2 = s2[1:]
-        s1.lstrip('0')
-        s2.lstrip('0')
+        s1 = s1.lstrip('0')
+        s2 = s2.lstrip('0')
         while (s1 and s1[0].isdigit()) and (s2 and s2[0].isdigit()):
             if not first_diff:
                 first_diff = ord(s1[0]) - ord(s2[0])
             s1 = s1[1:]
             s2 = s2[1:]
         if s1 and s1[0].isdigit():
             return 1
```

### Comparing `pygnuutils-0.0.6/pygnuutils/human_readable.py` & `pygnuutils-0.0.7/pygnuutils/human_readable.py`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.6/pygnuutils/ls.py` & `pygnuutils-0.0.7/pygnuutils/ls.py`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.6/pygnuutils/yes.py` & `pygnuutils-0.0.7/pygnuutils/yes.py`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.6/pygnuutils.egg-info/PKG-INFO` & `pygnuutils-0.0.7/pygnuutils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygnuutils
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python implementation for GNU utils
 Home-page: https://github.com/matan1008/pygnuutils
 Author: Matan Perelman
 Project-URL: pygnuutils, https://github.com/matan1008/pygnuutils
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pygnuutils-0.0.6/pygnuutils.egg-info/SOURCES.txt` & `pygnuutils-0.0.7/pygnuutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.6/setup.py` & `pygnuutils-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 from setuptools import setup, find_packages
 
 BASE_DIR = Path(__file__).parent.resolve(strict=True)
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 PACKAGE_NAME = 'pygnuutils'
 PACKAGES = [p for p in find_packages() if not p.startswith('tests')]
 
 
 def parse_requirements():
     reqs = []
     with open(BASE_DIR / 'requirements.txt', 'r') as fd:
```

