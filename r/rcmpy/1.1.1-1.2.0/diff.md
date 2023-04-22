# Comparing `tmp/rcmpy-1.1.1.tar.gz` & `tmp/rcmpy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcmpy-1.1.1.tar", last modified: Fri Apr 21 01:18:13 2023, max compression
+gzip compressed data, was "rcmpy-1.2.0.tar", last modified: Sat Apr 22 17:18:35 2023, max compression
```

## Comparing `rcmpy-1.1.1.tar` & `rcmpy-1.2.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-21 01:17:09.000000 rcmpy-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-21 01:18:13.222054 rcmpy-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-04-21 01:17:09.000000 rcmpy-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-21 01:17:09.000000 rcmpy-1.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.218054 rcmpy-1.1.1/rcmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/rcmpy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/commands/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/commands/use.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/commands/variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/commands/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/rcmpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/config/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.218054 rcmpy-1.1.1/rcmpy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/rcmpy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/data/schemas/ManagedFile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/data/schemas/State.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/rcmpy/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/environment/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/rcmpy/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/rcmpy/state/
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/rcmpy/xdg/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-21 01:17:09.000000 rcmpy-1.1.1/rcmpy/xdg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.218054 rcmpy-1.1.1/rcmpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-21 01:18:13.000000 rcmpy-1.1.1/rcmpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-21 01:18:13.000000 rcmpy-1.1.1/rcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 01:18:13.000000 rcmpy-1.1.1/rcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 01:18:13.000000 rcmpy-1.1.1/rcmpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-21 01:18:13.000000 rcmpy-1.1.1/rcmpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 01:18:13.000000 rcmpy-1.1.1/rcmpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 01:18:13.222054 rcmpy-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-21 01:17:09.000000 rcmpy-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:18:13.222054 rcmpy-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-21 01:17:09.000000 rcmpy-1.1.1/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-21 01:17:09.000000 rcmpy-1.1.1/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-21 01:17:09.000000 rcmpy-1.1.1/tests/test_xdg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-22 17:17:28.000000 rcmpy-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-22 17:18:35.164189 rcmpy-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-04-22 17:17:28.000000 rcmpy-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-22 17:17:28.000000 rcmpy-1.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.160189 rcmpy-1.2.0/rcmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/commands/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/commands/use.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/commands/variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/commands/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/config/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.160189 rcmpy-1.2.0/rcmpy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/data/schemas/ManagedFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/data/schemas/State.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/environment/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy/xdg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/xdg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-22 17:18:35.000000 rcmpy-1.2.0/rcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-22 17:18:35.000000 rcmpy-1.2.0/rcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:18:35.000000 rcmpy-1.2.0/rcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-22 17:18:35.000000 rcmpy-1.2.0/rcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-22 17:18:35.000000 rcmpy-1.2.0/rcmpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 17:18:35.000000 rcmpy-1.2.0/rcmpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 17:18:35.164189 rcmpy-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-22 17:17:28.000000 rcmpy-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-22 17:17:28.000000 rcmpy-1.2.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-22 17:17:28.000000 rcmpy-1.2.0/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-22 17:17:28.000000 rcmpy-1.2.0/tests/test_xdg.py
```

### Comparing `rcmpy-1.1.1/LICENSE` & `rcmpy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/PKG-INFO` & `rcmpy-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.1.1
+Version: 1.2.0
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=e17a2a1feecf3316dd227e4ef69c4351
+    hash=a4e47be8738ab981e11e2267b94bc9fc
     =====================================
 -->
 
-# rcmpy ([1.1.1](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.2.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-1.1.1/README.md` & `rcmpy-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=e17a2a1feecf3316dd227e4ef69c4351
+    hash=a4e47be8738ab981e11e2267b94bc9fc
     =====================================
 -->
 
-# rcmpy ([1.1.1](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.2.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-1.1.1/pyproject.toml` & `rcmpy-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "rcmpy"
-version = "1.1.1"
+version = "1.2.0"
 description = "A configuration-file management system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `rcmpy-1.1.1/rcmpy/app.py` & `rcmpy-1.2.0/rcmpy/app.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/rcmpy/commands/all.py` & `rcmpy-1.2.0/rcmpy/commands/all.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/rcmpy/commands/apply.py` & `rcmpy-1.2.0/rcmpy/commands/apply.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     for file in env.config.files:
         # Check if a template is found for this file.
         if file.template not in env.templates_by_name:
             result += 1
             env.logger.error("Template '%s' not found!", file.template)
             continue
 
+        if not file.platform:
+            continue
+
         is_new = env.state.is_new()
 
         # Check if this file has any updated templates.
         if args.force or is_new or env.is_updated(file):
             template = env.templates_by_name[file.template]
 
             # If a template doesn't require rendering, use it as-is.
```

### Comparing `rcmpy-1.1.1/rcmpy/commands/use.py` & `rcmpy-1.2.0/rcmpy/commands/use.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/rcmpy/commands/variant.py` & `rcmpy-1.2.0/rcmpy/commands/variant.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/rcmpy/commands/watch.py` & `rcmpy-1.2.0/rcmpy/commands/watch.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/rcmpy/config/__init__.py` & `rcmpy-1.2.0/rcmpy/config/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
             new = ManagedFile(
                 file["template"],
                 set(file.get("extra_templates", [])),
                 # Resolve environment variables and any '~' here.
                 Path(expandvars(file["directory"])).expanduser(),
                 file.get("name", file["template"]),
                 file["link"],
+                set(file.get("platforms", [])),
             )
 
             # Keep track of all templates used in any file.
             self.templates.add(new.template)
             for template in new.extra_templates:
                 self.templates.add(template)
```

### Comparing `rcmpy-1.1.1/rcmpy/config/file.py` & `rcmpy-1.2.0/rcmpy/config/file.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 # built-in
 from contextlib import suppress
 from dataclasses import dataclass
 from pathlib import Path
 from shutil import copyfile
+import sys
 from typing import Set
 
 # third-party
 from vcorelib.logging import LoggerType
 from vcorelib.paths import rel
 
 
@@ -24,19 +25,26 @@
     extra_templates: Set[str]
 
     directory: Path
     name: str
 
     link: bool
 
+    platforms: Set[str]
+
     @property
     def output(self) -> Path:
         """Get the full output path."""
         return self.directory.joinpath(self.name)
 
+    @property
+    def platform(self) -> bool:
+        """Determine if the platform is correct for handling this file."""
+        return not self.platforms or sys.platform in self.platforms
+
     def update_root(self, root: Path) -> None:
         """
         If the output directory is a relative path, update it to be an
         absolute one based on the provided root directory.
         """
 
         if not self.directory.is_absolute():
```

### Comparing `rcmpy-1.1.1/rcmpy/entry.py` & `rcmpy-1.2.0/rcmpy/entry.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/rcmpy/environment/__init__.py` & `rcmpy-1.2.0/rcmpy/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/rcmpy/environment/base.py` & `rcmpy-1.2.0/rcmpy/environment/base.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/rcmpy/environment/template.py` & `rcmpy-1.2.0/rcmpy/environment/template.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/rcmpy/paths/__init__.py` & `rcmpy-1.2.0/rcmpy/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/rcmpy/schemas.py` & `rcmpy-1.2.0/rcmpy/schemas.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/rcmpy/state/__init__.py` & `rcmpy-1.2.0/rcmpy/state/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/rcmpy/xdg/__init__.py` & `rcmpy-1.2.0/rcmpy/xdg/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/rcmpy.egg-info/PKG-INFO` & `rcmpy-1.2.0/rcmpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.1.1
+Version: 1.2.0
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=e17a2a1feecf3316dd227e4ef69c4351
+    hash=a4e47be8738ab981e11e2267b94bc9fc
     =====================================
 -->
 
-# rcmpy ([1.1.1](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.2.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-1.1.1/rcmpy.egg-info/SOURCES.txt` & `rcmpy-1.2.0/rcmpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/setup.py` & `rcmpy-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.1.1/tests/test_entry.py` & `rcmpy-1.2.0/tests/test_entry.py`

 * *Files identical despite different names*

