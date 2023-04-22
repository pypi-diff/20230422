# Comparing `tmp/pyrew-0.9.1.tar.gz` & `tmp/pyrew-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrew-0.9.1.tar", last modified: Sat Apr 22 09:06:40 2023, max compression
+gzip compressed data, was "pyrew-0.9.2.tar", last modified: Sat Apr 22 09:09:07 2023, max compression
```

## Comparing `pyrew-0.9.1.tar` & `pyrew-0.9.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:06:40.481284 pyrew-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 09:06:40.481284 pyrew-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-22 09:06:22.000000 pyrew-0.9.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 09:06:22.000000 pyrew-0.9.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:06:40.481284 pyrew-0.9.1/pyrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 09:06:40.000000 pyrew-0.9.1/pyrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-22 09:06:40.000000 pyrew-0.9.1/pyrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:06:40.000000 pyrew-0.9.1/pyrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 09:06:40.000000 pyrew-0.9.1/pyrew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-22 09:06:22.000000 pyrew-0.9.1/pyrew.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 09:06:40.481284 pyrew-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-22 09:06:22.000000 pyrew-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:09:07.918482 pyrew-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 09:09:07.918482 pyrew-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-22 09:08:54.000000 pyrew-0.9.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 09:08:54.000000 pyrew-0.9.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:09:07.914482 pyrew-0.9.2/pyrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 09:09:07.000000 pyrew-0.9.2/pyrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-22 09:09:07.000000 pyrew-0.9.2/pyrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:09:07.000000 pyrew-0.9.2/pyrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 09:09:07.000000 pyrew-0.9.2/pyrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-04-22 09:08:54.000000 pyrew-0.9.2/pyrew.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 09:09:07.918482 pyrew-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-22 09:08:54.000000 pyrew-0.9.2/setup.py
```

### Comparing `pyrew-0.9.1/PKG-INFO` & `pyrew-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrew
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Python library for writing shorter and more efficient Python code.
 Home-page: https://github.com/AquaQuokka/pyrew
 Author: AquaQuokka
 License: BSD-3-Clause
 
 =============
 Pyrew
```

### Comparing `pyrew-0.9.1/pyrew.egg-info/PKG-INFO` & `pyrew-0.9.2/pyrew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrew
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Python library for writing shorter and more efficient Python code.
 Home-page: https://github.com/AquaQuokka/pyrew
 Author: AquaQuokka
 License: BSD-3-Clause
 
 =============
 Pyrew
```

### Comparing `pyrew-0.9.1/pyrew.py` & `pyrew-0.9.2/pyrew.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
 
         try:
             func()
 
         finally:
             stop_spinner.set()
             spinner_thread.join()
-            sys.stdout.write("\r\nDone!\n")
+            sys.stdout.write("Done!\n")
             sys.stdout.flush()
 
     class validate:
 
         @staticmethod
         def email(*emails):
```

