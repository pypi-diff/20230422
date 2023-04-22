# Comparing `tmp/withwait-0.1.0.tar.gz` & `tmp/withwait-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "withwait-0.1.0.tar", max compression
+gzip compressed data, was "withwait-0.1.1.tar", max compression
```

## Comparing `withwait-0.1.0.tar` & `withwait-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1092 2023-04-22 19:40:59.483281 withwait-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     1280 2023-04-22 19:40:59.483281 withwait-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      337 2023-04-22 19:40:59.483281 withwait-0.1.0/withwait/__init__.py
--rw-r--r--   0        0        0     4930 2023-04-22 19:40:59.483281 withwait-0.1.0/withwait/__withwait.py
--rw-r--r--   0        0        0        0 2023-04-22 19:40:59.483281 withwait-0.1.0/withwait/py.typed
--rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 withwait-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-22 19:45:15.124062 withwait-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     2235 2023-04-22 19:45:15.124062 withwait-0.1.1/README.md
+-rw-r--r--   0        0        0     1302 2023-04-22 19:45:15.124062 withwait-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      337 2023-04-22 19:45:15.124062 withwait-0.1.1/withwait/__init__.py
+-rw-r--r--   0        0        0     4930 2023-04-22 19:45:15.124062 withwait-0.1.1/withwait/__withwait.py
+-rw-r--r--   0        0        0        0 2023-04-22 19:45:15.124062 withwait-0.1.1/withwait/py.typed
+-rw-r--r--   0        0        0     3540 1970-01-01 00:00:00.000000 withwait-0.1.1/PKG-INFO
```

### Comparing `withwait-0.1.0/LICENSE.md` & `withwait-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `withwait-0.1.0/pyproject.toml` & `withwait-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 [tool.poetry]
 name = "withwait"
-version = "0.1.0"
+version = "0.1.1"
 description = "A simple utility to ensure that sleep operations always complete"
+readme = "README.md"
+
 authors = ["Miguel Guthridge <hdsq@outlook.com.au>"]
 license = "MIT"
 
 repository = "https://github.com/MiguelGuthridge/withwait"
 documentation = "https://miguelguthridge.github.io/withwait"
 
 keywords = [
```

### Comparing `withwait-0.1.0/withwait/__withwait.py` & `withwait-0.1.1/withwait/__withwait.py`

 * *Files identical despite different names*

