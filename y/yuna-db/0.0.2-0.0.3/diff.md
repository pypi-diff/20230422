# Comparing `tmp/yuna-db-0.0.2.tar.gz` & `tmp/yuna-db-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuna-db-0.0.2.tar", last modified: Sat Apr 22 07:45:06 2023, max compression
+gzip compressed data, was "yuna-db-0.0.3.tar", last modified: Sat Apr 22 07:51:30 2023, max compression
```

## Comparing `yuna-db-0.0.2.tar` & `yuna-db-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.0.2/LICENSE
--rw-r--r--   0        0        0     1076 2023-04-22 07:39:41.427206 yuna-db-0.0.2/README.md
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.0.2/__init__.py
--rw-r--r--   0        0        0      420 2023-04-22 07:44:46.945544 yuna-db-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.0.2/requirements.txt
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.0.2/src/__init__.py
--rw-r--r--   0        0        0     9242 2023-04-22 07:35:44.814296 yuna-db-0.0.2/src/yuna/__init__.py
--rw-r--r--   0        0        0     8857 2023-04-22 05:28:48.552375 yuna-db-0.0.2/src/yuna/lmdb_util.py
--rw-r--r--   0        0        0    15501 2023-04-22 05:08:39.487465 yuna-db-0.0.2/src/yuna/plugins.py
--rwxr-xr-x   0        0        0     1776 2023-04-22 05:31:18.871506 yuna-db-0.0.2/test_yuna.py
--rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      417 2023-04-11 08:21:59.924544 yuna-db-0.0.2/tests/test_simple.py
--rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.0.2/version.txt
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 yuna-db-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1075 2023-04-22 07:50:02.664090 yuna-db-0.0.3/README.md
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.0.3/__init__.py
+-rw-r--r--   0        0        0      424 2023-04-22 07:50:30.728671 yuna-db-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.0.3/requirements.txt
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0     9242 2023-04-22 07:50:37.512812 yuna-db-0.0.3/src/yuna/__init__.py
+-rw-r--r--   0        0        0     8857 2023-04-22 05:28:48.552375 yuna-db-0.0.3/src/yuna/lmdb_util.py
+-rw-r--r--   0        0        0    15501 2023-04-22 05:08:39.487465 yuna-db-0.0.3/src/yuna/plugins.py
+-rwxr-xr-x   0        0        0     1776 2023-04-22 05:31:18.871506 yuna-db-0.0.3/test_yuna.py
+-rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      417 2023-04-11 08:21:59.924544 yuna-db-0.0.3/tests/test_simple.py
+-rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.0.3/version.txt
+-rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 yuna-db-0.0.3/PKG-INFO
```

### Comparing `yuna-db-0.0.2/LICENSE` & `yuna-db-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yuna-db-0.0.2/README.md` & `yuna-db-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#Yuna: dict-like semantics for LMDB
+Yuna: dict-like semantics for LMDB
 
 Yuna is a key/value store that's built upon LMDB (the Symas Lightning
 Memory-mapped Database).  LMDB really is lightning-fast, but as a C
 library only allows you to lookup a byte string value, using either
 an integer key or a byte string key.
 
 Yuna provides semantics similar to a dict.  You can specify a serialization
```

### Comparing `yuna-db-0.0.2/src/yuna/__init__.py` & `yuna-db-0.0.3/src/yuna/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 db.tables.foo.put("x_value", x)
 
 After that .put() you can call .get():
 
 x = db.tables.foo.get("x_value")
 """
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 import types
 
 from json import dumps as json_dumps
 from json import loads as json_loads
 from types import SimpleNamespace
 from typing import Optional
```

### Comparing `yuna-db-0.0.2/src/yuna/lmdb_util.py` & `yuna-db-0.0.3/src/yuna/lmdb_util.py`

 * *Files identical despite different names*

### Comparing `yuna-db-0.0.2/src/yuna/plugins.py` & `yuna-db-0.0.3/src/yuna/plugins.py`

 * *Files identical despite different names*

### Comparing `yuna-db-0.0.2/test_yuna.py` & `yuna-db-0.0.3/test_yuna.py`

 * *Files identical despite different names*

### Comparing `yuna-db-0.0.2/PKG-INFO` & `yuna-db-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: yuna-db
-Version: 0.0.2
+Version: 0.0.3
 Summary: Yuna database, Python implementation.
 Author-email: "Steve R. Hastings" <steve@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
+Requires-Dist: lmdb >=1.4.1,<2
 
-#Yuna: dict-like semantics for LMDB
+Yuna: dict-like semantics for LMDB
 
 Yuna is a key/value store that's built upon LMDB (the Symas Lightning
 Memory-mapped Database).  LMDB really is lightning-fast, but as a C
 library only allows you to lookup a byte string value, using either
 an integer key or a byte string key.
 
 Yuna provides semantics similar to a dict.  You can specify a serialization
```

