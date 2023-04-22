# Comparing `tmp/yuna-db-0.0.3.tar.gz` & `tmp/yuna-db-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuna-db-0.0.3.tar", last modified: Sat Apr 22 07:51:30 2023, max compression
+gzip compressed data, was "yuna-db-0.0.4.tar", last modified: Sat Apr 22 07:57:23 2023, max compression
```

## Comparing `yuna-db-0.0.3.tar` & `yuna-db-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.0.3/LICENSE
--rw-r--r--   0        0        0     1075 2023-04-22 07:50:02.664090 yuna-db-0.0.3/README.md
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.0.3/__init__.py
--rw-r--r--   0        0        0      424 2023-04-22 07:50:30.728671 yuna-db-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.0.3/requirements.txt
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.0.3/src/__init__.py
--rw-r--r--   0        0        0     9242 2023-04-22 07:50:37.512812 yuna-db-0.0.3/src/yuna/__init__.py
--rw-r--r--   0        0        0     8857 2023-04-22 05:28:48.552375 yuna-db-0.0.3/src/yuna/lmdb_util.py
--rw-r--r--   0        0        0    15501 2023-04-22 05:08:39.487465 yuna-db-0.0.3/src/yuna/plugins.py
--rwxr-xr-x   0        0        0     1776 2023-04-22 05:31:18.871506 yuna-db-0.0.3/test_yuna.py
--rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      417 2023-04-11 08:21:59.924544 yuna-db-0.0.3/tests/test_simple.py
--rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.0.3/version.txt
--rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 yuna-db-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1075 2023-04-22 07:50:02.664090 yuna-db-0.0.4/README.md
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.0.4/__init__.py
+-rw-r--r--   0        0        0      424 2023-04-22 07:50:30.728671 yuna-db-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.0.4/requirements.txt
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0     9147 2023-04-22 07:55:16.566594 yuna-db-0.0.4/src/yuna/__init__.py
+-rw-r--r--   0        0        0     8857 2023-04-22 05:28:48.552375 yuna-db-0.0.4/src/yuna/lmdb_util.py
+-rw-r--r--   0        0        0    15465 2023-04-22 07:54:58.474220 yuna-db-0.0.4/src/yuna/plugins.py
+-rwxr-xr-x   0        0        0     1776 2023-04-22 05:31:18.871506 yuna-db-0.0.4/test_yuna.py
+-rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      417 2023-04-11 08:21:59.924544 yuna-db-0.0.4/tests/test_simple.py
+-rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.0.4/version.txt
+-rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 yuna-db-0.0.4/PKG-INFO
```

### Comparing `yuna-db-0.0.3/LICENSE` & `yuna-db-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yuna-db-0.0.3/README.md` & `yuna-db-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `yuna-db-0.0.3/src/yuna/__init__.py` & `yuna-db-0.0.4/src/yuna/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,38 +19,38 @@
 db.tables.foo.put("x_value", x)
 
 After that .put() you can call .get():
 
 x = db.tables.foo.get("x_value")
 """
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 import types
 
 from json import dumps as json_dumps
 from json import loads as json_loads
 from types import SimpleNamespace
 from typing import Optional
 
 import lmdb
 
 
-from src.yuna.lmdb_util import YUNA_DEFAULT_MAX_DB_SIZE, YUNA_DEFAULT_MAX_TABLES
-from src.yuna.lmdb_util import YUNA_DB_META_KEY, YUNA_FILE_EXTENSION
+from lmdb_util import YUNA_DEFAULT_MAX_DB_SIZE, YUNA_DEFAULT_MAX_TABLES
+from lmdb_util import YUNA_DB_META_KEY, YUNA_FILE_EXTENSION
 
-from src.yuna.lmdb_util import _lmdb_open, _yuna_get_meta, _yuna_new_meta, _yuna_put_meta
-from src.yuna.lmdb_util import _lmdb_reserved_delete, _lmdb_reserved_get, _lmdb_reserved_put
-from src.yuna.lmdb_util import _lmdb_table_drop, _lmdb_table_open, _lmdb_table_truncate
-
-from src.yuna import plugins
-from src.yuna.plugins import _YUNA_NOT_PROVIDED
-from src.yuna.plugins import SERIALIZE_JSON, SERIALIZE_MSGPACK, SERIALIZE_STR
-from src.yuna.plugins import COMPRESS_LZ4, COMPRESS_ZLIB, COMPRESS_ZSTD
-from src.yuna.plugins import serialize_json
+from lmdb_util import _lmdb_open, _yuna_get_meta, _yuna_new_meta, _yuna_put_meta
+from lmdb_util import _lmdb_reserved_delete, _lmdb_reserved_get, _lmdb_reserved_put
+from lmdb_util import _lmdb_table_drop, _lmdb_table_open, _lmdb_table_truncate
+
+import plugins
+from plugins import _YUNA_NOT_PROVIDED
+from plugins import SERIALIZE_JSON, SERIALIZE_MSGPACK, SERIALIZE_STR
+from plugins import COMPRESS_LZ4, COMPRESS_ZLIB, COMPRESS_ZSTD
+from plugins import serialize_json
 
 
 class YunaSharedData(object):
     """
     Private data for Yuna, in a class by itself so it can be shared
     among the multiple classes implementing Yuna.
     """
```

### Comparing `yuna-db-0.0.3/src/yuna/lmdb_util.py` & `yuna-db-0.0.4/src/yuna/lmdb_util.py`

 * *Files identical despite different names*

### Comparing `yuna-db-0.0.3/src/yuna/plugins.py` & `yuna-db-0.0.4/src/yuna/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 from types import SimpleNamespace
 from typing import Optional
 
 
 import lmdb
 
 
-from src.yuna.lmdb_util import YUNA_DEFAULT_MAX_DB_SIZE, YUNA_DEFAULT_MAX_TABLES
-from src.yuna.lmdb_util import YUNA_DB_META_KEY, YUNA_FILE_EXTENSION
+from lmdb_util import YUNA_DEFAULT_MAX_DB_SIZE, YUNA_DEFAULT_MAX_TABLES
+from lmdb_util import YUNA_DB_META_KEY, YUNA_FILE_EXTENSION
 
-from src.yuna.lmdb_util import _lmdb_open, _yuna_get_meta, _yuna_put_meta
-from src.yuna.lmdb_util import _lmdb_table_delete, _lmdb_table_get, _lmdb_table_put
+from lmdb_util import _lmdb_open, _yuna_get_meta, _yuna_put_meta
+from lmdb_util import _lmdb_table_delete, _lmdb_table_get, _lmdb_table_put
 
 
 # Create a unique object used to detect if optional arg not provided.
 # Can't use None because user might want to provide None.
 _YUNA_NOT_PROVIDED = object()
```

### Comparing `yuna-db-0.0.3/test_yuna.py` & `yuna-db-0.0.4/test_yuna.py`

 * *Files identical despite different names*

### Comparing `yuna-db-0.0.3/PKG-INFO` & `yuna-db-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuna-db
-Version: 0.0.3
+Version: 0.0.4
 Summary: Yuna database, Python implementation.
 Author-email: "Steve R. Hastings" <steve@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: lmdb >=1.4.1,<2
```

