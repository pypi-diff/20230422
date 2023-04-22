# Comparing `tmp/yuna-db-0.0.4.tar.gz` & `tmp/yuna-db-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuna-db-0.0.4.tar", last modified: Sat Apr 22 07:57:23 2023, max compression
+gzip compressed data, was "yuna-db-0.1.0.tar", last modified: Sat Apr 22 08:06:14 2023, max compression
```

## Comparing `yuna-db-0.0.4.tar` & `yuna-db-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.0.4/LICENSE
--rw-r--r--   0        0        0     1075 2023-04-22 07:50:02.664090 yuna-db-0.0.4/README.md
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.0.4/__init__.py
--rw-r--r--   0        0        0      424 2023-04-22 07:50:30.728671 yuna-db-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.0.4/requirements.txt
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.0.4/src/__init__.py
--rw-r--r--   0        0        0     9147 2023-04-22 07:55:16.566594 yuna-db-0.0.4/src/yuna/__init__.py
--rw-r--r--   0        0        0     8857 2023-04-22 05:28:48.552375 yuna-db-0.0.4/src/yuna/lmdb_util.py
--rw-r--r--   0        0        0    15465 2023-04-22 07:54:58.474220 yuna-db-0.0.4/src/yuna/plugins.py
--rwxr-xr-x   0        0        0     1776 2023-04-22 05:31:18.871506 yuna-db-0.0.4/test_yuna.py
--rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      417 2023-04-11 08:21:59.924544 yuna-db-0.0.4/tests/test_simple.py
--rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.0.4/version.txt
--rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 yuna-db-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1078 2023-04-22 08:03:57.581385 yuna-db-0.1.0/README.md
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.1.0/__init__.py
+-rw-r--r--   0        0        0      424 2023-04-22 07:50:30.728671 yuna-db-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.1.0/requirements.txt
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.1.0/src/__init__.py
+-rw-r--r--   0        0        0     9152 2023-04-22 08:04:48.210433 yuna-db-0.1.0/src/yuna/__init__.py
+-rw-r--r--   0        0        0     8857 2023-04-22 05:28:48.552375 yuna-db-0.1.0/src/yuna/lmdb_util.py
+-rw-r--r--   0        0        0    15469 2023-04-22 08:02:32.127615 yuna-db-0.1.0/src/yuna/plugins.py
+-rwxr-xr-x   0        0        0     1776 2023-04-22 05:31:18.871506 yuna-db-0.1.0/test_yuna.py
+-rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      417 2023-04-11 08:21:59.924544 yuna-db-0.1.0/tests/test_simple.py
+-rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.1.0/version.txt
+-rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 yuna-db-0.1.0/PKG-INFO
```

### Comparing `yuna-db-0.0.4/LICENSE` & `yuna-db-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yuna-db-0.0.4/README.md` & `yuna-db-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Yuna: dict-like semantics for LMDB
+Yuna DB: dict-like semantics for LMDB
 
 Yuna is a key/value store that's built upon LMDB (the Symas Lightning
 Memory-mapped Database).  LMDB really is lightning-fast, but as a C
 library only allows you to lookup a byte string value, using either
 an integer key or a byte string key.
 
 Yuna provides semantics similar to a dict.  You can specify a serialization
```

### Comparing `yuna-db-0.0.4/src/yuna/__init__.py` & `yuna-db-0.1.0/src/yuna/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # -*- coding: utf-8 -*-
 
 """
-Yuna database, Python implementation.
+Yuna DB: dict-like semantics for LMDB
 
 Yuna is a key/value store that's built upon LMDB (the Symas Lightning
 Memory-mapped Database).  LMDB really is lightning-fast, but as a C
 library only allows you to lookup a byte string value, using either
 an integer key or a byte string key.
 
 Yuna provides semantics similar to a dict.  You can specify a serialization
 format, and optionally a compression format to use, and Yuna will serialize
 values and write them to the database as byte strings.  It will
 automatically recover the value from the bytes string.
 
 For example, if x is any Python value that can be serialized by the chosen
 serialization format in table foo, this would work:
 
-db.tables.foo.put("x_value", x)
+db.tables.foo.put(key, x)
 
 After that .put() you can call .get():
 
-x = db.tables.foo.get("x_value")
+x = db.tables.foo.get(key)
 """
 
-__version__ = "0.0.4"
+__version__ = "0.1.0"
 
 import types
 
 from json import dumps as json_dumps
 from json import loads as json_loads
 from types import SimpleNamespace
 from typing import Optional
 
 import lmdb
 
 
-from lmdb_util import YUNA_DEFAULT_MAX_DB_SIZE, YUNA_DEFAULT_MAX_TABLES
-from lmdb_util import YUNA_DB_META_KEY, YUNA_FILE_EXTENSION
+from .lmdb_util import YUNA_DEFAULT_MAX_DB_SIZE, YUNA_DEFAULT_MAX_TABLES
+from .lmdb_util import YUNA_DB_META_KEY, YUNA_FILE_EXTENSION
 
-from lmdb_util import _lmdb_open, _yuna_get_meta, _yuna_new_meta, _yuna_put_meta
-from lmdb_util import _lmdb_reserved_delete, _lmdb_reserved_get, _lmdb_reserved_put
-from lmdb_util import _lmdb_table_drop, _lmdb_table_open, _lmdb_table_truncate
-
-import plugins
-from plugins import _YUNA_NOT_PROVIDED
-from plugins import SERIALIZE_JSON, SERIALIZE_MSGPACK, SERIALIZE_STR
-from plugins import COMPRESS_LZ4, COMPRESS_ZLIB, COMPRESS_ZSTD
-from plugins import serialize_json
+from .lmdb_util import _lmdb_open, _yuna_get_meta, _yuna_new_meta, _yuna_put_meta
+from .lmdb_util import _lmdb_reserved_delete, _lmdb_reserved_get, _lmdb_reserved_put
+from .lmdb_util import _lmdb_table_drop, _lmdb_table_open, _lmdb_table_truncate
+
+from . import plugins
+from .plugins import _YUNA_NOT_PROVIDED
+from .plugins import SERIALIZE_JSON, SERIALIZE_MSGPACK, SERIALIZE_STR
+from .plugins import COMPRESS_LZ4, COMPRESS_ZLIB, COMPRESS_ZSTD
+from .plugins import serialize_json
 
 
 class YunaSharedData(object):
     """
     Private data for Yuna, in a class by itself so it can be shared
     among the multiple classes implementing Yuna.
     """
@@ -224,15 +224,15 @@
             YunaTable(self._shared,
                     meta["name"], meta["key_serialize"], meta["value_serialize"], meta["value_compress"])
 
     def sync(self):
         """
         Ensure that all data is flushed to disk.
 
-        Useful when Yuna was opend in "unsafe" mode.
+        Useful when Yuna was opened in "unsafe" mode.
         """
         _lmdb_sync(self._shared.env)
     def close(self):
         """
         Close the Yuna instance.
 
         Ensures that all data is flushed to disk.
```

### Comparing `yuna-db-0.0.4/src/yuna/lmdb_util.py` & `yuna-db-0.1.0/src/yuna/lmdb_util.py`

 * *Files identical despite different names*

### Comparing `yuna-db-0.0.4/src/yuna/plugins.py` & `yuna-db-0.1.0/src/yuna/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 from types import SimpleNamespace
 from typing import Optional
 
 
 import lmdb
 
 
-from lmdb_util import YUNA_DEFAULT_MAX_DB_SIZE, YUNA_DEFAULT_MAX_TABLES
-from lmdb_util import YUNA_DB_META_KEY, YUNA_FILE_EXTENSION
+from .lmdb_util import YUNA_DEFAULT_MAX_DB_SIZE, YUNA_DEFAULT_MAX_TABLES
+from .lmdb_util import YUNA_DB_META_KEY, YUNA_FILE_EXTENSION
 
-from lmdb_util import _lmdb_open, _yuna_get_meta, _yuna_put_meta
-from lmdb_util import _lmdb_table_delete, _lmdb_table_get, _lmdb_table_put
+from .lmdb_util import _lmdb_open, _yuna_get_meta, _yuna_put_meta
+from .lmdb_util import _lmdb_table_delete, _lmdb_table_get, _lmdb_table_put
 
 
 # Create a unique object used to detect if optional arg not provided.
 # Can't use None because user might want to provide None.
 _YUNA_NOT_PROVIDED = object()
```

### Comparing `yuna-db-0.0.4/test_yuna.py` & `yuna-db-0.1.0/test_yuna.py`

 * *Files identical despite different names*

### Comparing `yuna-db-0.0.4/PKG-INFO` & `yuna-db-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: yuna-db
-Version: 0.0.4
-Summary: Yuna database, Python implementation.
+Version: 0.1.0
+Summary: Yuna DB: dict-like semantics for LMDB
 Author-email: "Steve R. Hastings" <steve@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: lmdb >=1.4.1,<2
 
-Yuna: dict-like semantics for LMDB
+Yuna DB: dict-like semantics for LMDB
 
 Yuna is a key/value store that's built upon LMDB (the Symas Lightning
 Memory-mapped Database).  LMDB really is lightning-fast, but as a C
 library only allows you to lookup a byte string value, using either
 an integer key or a byte string key.
 
 Yuna provides semantics similar to a dict.  You can specify a serialization
```

