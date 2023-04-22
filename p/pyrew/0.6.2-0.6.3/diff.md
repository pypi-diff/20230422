# Comparing `tmp/pyrew-0.6.2.tar.gz` & `tmp/pyrew-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrew-0.6.2.tar", last modified: Sat Apr 22 06:40:21 2023, max compression
+gzip compressed data, was "pyrew-0.6.3.tar", last modified: Sat Apr 22 06:50:27 2023, max compression
```

## Comparing `pyrew-0.6.2.tar` & `pyrew-0.6.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:40:21.782803 pyrew-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 06:40:21.782803 pyrew-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-22 06:40:08.000000 pyrew-0.6.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 06:40:08.000000 pyrew-0.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:40:21.782803 pyrew-0.6.2/pyrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 06:40:21.000000 pyrew-0.6.2/pyrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-22 06:40:21.000000 pyrew-0.6.2/pyrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 06:40:21.000000 pyrew-0.6.2/pyrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 06:40:21.000000 pyrew-0.6.2/pyrew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-04-22 06:40:08.000000 pyrew-0.6.2/pyrew.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 06:40:21.782803 pyrew-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-22 06:40:08.000000 pyrew-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:50:27.600237 pyrew-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 06:50:27.600237 pyrew-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-22 06:50:17.000000 pyrew-0.6.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 06:50:17.000000 pyrew-0.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:50:27.600237 pyrew-0.6.3/pyrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 06:50:27.000000 pyrew-0.6.3/pyrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-22 06:50:27.000000 pyrew-0.6.3/pyrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 06:50:27.000000 pyrew-0.6.3/pyrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 06:50:27.000000 pyrew-0.6.3/pyrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-04-22 06:50:17.000000 pyrew-0.6.3/pyrew.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 06:50:27.600237 pyrew-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-22 06:50:17.000000 pyrew-0.6.3/setup.py
```

### Comparing `pyrew-0.6.2/PKG-INFO` & `pyrew-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrew
-Version: 0.6.2
+Version: 0.6.3
 Summary: A Python library for writing shorter and more efficient Python code.
 Home-page: https://github.com/AquaQuokka/pyrew
 Author: AquaQuokka
 License: BSD-3-Clause
 
 =============
 Pyrew
```

### Comparing `pyrew-0.6.2/pyrew.egg-info/PKG-INFO` & `pyrew-0.6.3/pyrew.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrew
-Version: 0.6.2
+Version: 0.6.3
 Summary: A Python library for writing shorter and more efficient Python code.
 Home-page: https://github.com/AquaQuokka/pyrew
 Author: AquaQuokka
 License: BSD-3-Clause
 
 =============
 Pyrew
```

### Comparing `pyrew-0.6.2/pyrew.py` & `pyrew-0.6.3/pyrew.py`

 * *Files identical despite different names*

