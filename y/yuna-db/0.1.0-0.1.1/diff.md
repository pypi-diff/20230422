# Comparing `tmp/yuna-db-0.1.0.tar.gz` & `tmp/yuna-db-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuna-db-0.1.0.tar", last modified: Sat Apr 22 08:06:14 2023, max compression
+gzip compressed data, was "yuna-db-0.1.1.tar", last modified: Sat Apr 22 09:09:37 2023, max compression
```

## Comparing `yuna-db-0.1.0.tar` & `yuna-db-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.1.0/LICENSE
--rw-r--r--   0        0        0     1078 2023-04-22 08:03:57.581385 yuna-db-0.1.0/README.md
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.1.0/__init__.py
--rw-r--r--   0        0        0      424 2023-04-22 07:50:30.728671 yuna-db-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.1.0/requirements.txt
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.1.0/src/__init__.py
--rw-r--r--   0        0        0     9152 2023-04-22 08:04:48.210433 yuna-db-0.1.0/src/yuna/__init__.py
--rw-r--r--   0        0        0     8857 2023-04-22 05:28:48.552375 yuna-db-0.1.0/src/yuna/lmdb_util.py
--rw-r--r--   0        0        0    15469 2023-04-22 08:02:32.127615 yuna-db-0.1.0/src/yuna/plugins.py
--rwxr-xr-x   0        0        0     1776 2023-04-22 05:31:18.871506 yuna-db-0.1.0/test_yuna.py
--rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      417 2023-04-11 08:21:59.924544 yuna-db-0.1.0/tests/test_simple.py
--rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.1.0/version.txt
--rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 yuna-db-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1623 2023-04-22 08:52:20.397496 yuna-db-0.1.1/README.md
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.1.1/__init__.py
+-rw-r--r--   0        0        0      424 2023-04-22 07:50:30.728671 yuna-db-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.1.1/requirements.txt
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.1.1/src/__init__.py
+-rw-r--r--   0        0        0     9010 2023-04-22 08:53:31.206956 yuna-db-0.1.1/src/yuna/__init__.py
+-rw-r--r--   0        0        0     8857 2023-04-22 05:28:48.552375 yuna-db-0.1.1/src/yuna/lmdb_util.py
+-rw-r--r--   0        0        0    15469 2023-04-22 08:02:32.127615 yuna-db-0.1.1/src/yuna/plugins.py
+-rwxr-xr-x   0        0        0     1776 2023-04-22 05:31:18.871506 yuna-db-0.1.1/test_yuna.py
+-rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      417 2023-04-11 08:21:59.924544 yuna-db-0.1.1/tests/test_simple.py
+-rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.1.1/version.txt
+-rw-r--r--   0        0        0     1923 1970-01-01 00:00:00.000000 yuna-db-0.1.1/PKG-INFO
```

### Comparing `yuna-db-0.1.0/LICENSE` & `yuna-db-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yuna-db-0.1.0/src/yuna/__init__.py` & `yuna-db-0.1.1/src/yuna/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 db.tables.foo.put(key, x)
 
 After that .put() you can call .get():
 
 x = db.tables.foo.get(key)
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 import types
 
 from json import dumps as json_dumps
 from json import loads as json_loads
 from types import SimpleNamespace
 from typing import Optional
@@ -107,37 +107,37 @@
 
     Provides method functions for delete, get, put, etc.
     """
     def __init__(self,
         shared: YunaSharedData,
         name: str,
         key_serialize: Optional[str],
-        value_serialize: Optional[str],
-        value_compress: Optional[str],
+        serialize: Optional[str],
+        compress: Optional[str],
     ):
         if name in shared.tables_map:
             raise ValueError(f"table '{name}' is already open in this database")
 
         # TODO: check key_serialize to see if we are doing integer keys here
         try:
             temp = plugins.get_serialize_plugins(key_serialize)
         except ValueError:
             raise ValueError("unknown serialization format for key_serialize: {repr(key_serialize)}")
         try:
-            temp = plugins.get_serialize_plugins(value_serialize)
+            temp = plugins.get_serialize_plugins(serialize)
         except ValueError:
-            raise ValueError("unknown serialization format for value_serialize: {repr(value_serialize)}")
+            raise ValueError("unknown serialization format for serialize: {repr(serialize)}")
         try:
-            temp = plugins.get_compress_plugins(value_compress)
+            temp = plugins.get_compress_plugins(compress)
         except ValueError:
-            raise ValueError("unknown compression format for value_compress: {repr(value_compress)}")
+            raise ValueError("unknown compression format for compress: {repr(compress)}")
 
         meta = SimpleNamespace(
             name=name,
-            key_serialize=key_serialize, value_serialize=value_serialize, value_compress=value_compress
+            key_serialize=key_serialize, serialize=serialize, compress=compress
         )
         self._shared = shared
 
         # Check to see if the table name is in the metadata.  If it is in there, assume the table exists
         # in the LMDB file, so we wouldn't want to create.  If it's not in there, we need to create it.
         create = name not in self._shared.metadata["tables"]
 
@@ -150,16 +150,16 @@
         key_serialize = meta.key_serialize
 
         # add method functions based on what's documented in the metadata
         env = self._shared.env
         lmdb_table = self.lmdb_table
 
         fn_delete = plugins.delete_factory(env, lmdb_table, key_serialize)
-        fn_get = plugins.get_factory(env, lmdb_table, key_serialize, value_serialize, value_compress)
-        fn_put = plugins.put_factory(env, lmdb_table, key_serialize, value_serialize, value_compress)
+        fn_get = plugins.get_factory(env, lmdb_table, key_serialize, serialize, compress)
+        fn_put = plugins.put_factory(env, lmdb_table, key_serialize, serialize, compress)
 
         # turn the freshly-created function objects into bound method functions of the class
         self.delete = types.MethodType(fn_delete, self)
         self.get = types.MethodType(fn_get, self)
         self.put = types.MethodType(fn_put, self)
 
         # Table instance fully created so keep track of it
@@ -183,16 +183,16 @@
 class Yuna(object):
     """
     Key/value store with dict-like semantics.  A wrapper around LMDB.
     """
     def __init__(self,
         fname: str,
         # YunaDB name and version
-        name: Optional[str],
-        version: Optional[int],
+        name: Optional[str]=None,
+        version: Optional[int]=None,
 
         # details of an LMDB file follow
         read_only: bool=True,
         create: bool=False,
         safety_mode: str='a',
         single_file: bool=True,
         max_tables: int=YUNA_DEFAULT_MAX_TABLES,
@@ -217,16 +217,15 @@
         self.metadata = metadata
         self.reserved = reserved
         self._shared = YunaSharedData(env=env, tables_map=vars(tables), metadata=metadata)
         self.tables = tables
 
         # Set up an entry in .tables for each table listed in metadata, with delete/get/put functions ready to use.
         for meta in metadata["tables"].values():
-            YunaTable(self._shared,
-                    meta["name"], meta["key_serialize"], meta["value_serialize"], meta["value_compress"])
+            YunaTable(self._shared, meta["name"], meta["key_serialize"], meta["serialize"], meta["compress"])
 
     def sync(self):
         """
         Ensure that all data is flushed to disk.
 
         Useful when Yuna was opened in "unsafe" mode.
         """
@@ -242,24 +241,24 @@
         del self._shared
     @property
     def table_names(self):
         return sorted(vars(self.tables))
     def new_table(self,
         name: str,
         key_serialize: Optional[str]=SERIALIZE_STR,
-        value_serialize: Optional[str]=None,
-        value_compress: Optional[str]=None
+        serialize: Optional[str]=None,
+        compress: Optional[str]=None
     ):
         """
         Open a new Yuna table.
 
         Creates the table in the LMDB file, updates the Yuna metadata,
         and sets up serialization and optional compression as requested.
         """
-        tbl = YunaTable(self._shared, name, key_serialize, value_serialize, value_compress)
+        tbl = YunaTable(self._shared, name, key_serialize, serialize, compress)
 
         # YunaTable takes care of adding the new table to self.tables
         assert name in vars(self.tables)
         # YunaTable also updates the metadata
         assert name in self._shared.metadata["tables"]
 
         return tbl
```

### Comparing `yuna-db-0.1.0/src/yuna/lmdb_util.py` & `yuna-db-0.1.1/src/yuna/lmdb_util.py`

 * *Files identical despite different names*

### Comparing `yuna-db-0.1.0/src/yuna/plugins.py` & `yuna-db-0.1.1/src/yuna/plugins.py`

 * *Files identical despite different names*

### Comparing `yuna-db-0.1.0/test_yuna.py` & `yuna-db-0.1.1/test_yuna.py`

 * *Files identical despite different names*

### Comparing `yuna-db-0.1.0/PKG-INFO` & `yuna-db-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: yuna-db
-Version: 0.1.0
-Summary: Yuna DB: dict-like semantics for LMDB
-Author-email: "Steve R. Hastings" <steve@hastings.org>
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: lmdb >=1.4.1,<2
-
 Yuna DB: dict-like semantics for LMDB
 
 Yuna is a key/value store that's built upon LMDB (the Symas Lightning
 Memory-mapped Database).  LMDB really is lightning-fast, but as a C
 library only allows you to lookup a byte string value, using either
 an integer key or a byte string key.
 
@@ -19,22 +9,47 @@
 format, and optionally a compression format to use, and Yuna will serialize
 values and write them to the database as byte strings.  It will
 automatically recover the value from the bytes string.
 
 For example, if x is any Python value that can be serialized by the chosen
 serialization format in table foo, this would work:
 
-`db.tables.foo.put("x_value", x)`
+`db.tables.foo.put(key, x)`
 
 After that .put() you can call .get():
 
-`x = db.tables.foo.get("x_value")`
+`x = db.tables.foo.get(key)`
+
+
+# Example
+
+```
+from yuna import Yuna, SERIALIZE_JSON, SERIALIZE_STR
+
+db = Yuna("/tmp/test.ydb", create=True)
+db.new_table("names", serialize=SERIALIZE_JSON)
 
+key = "feynman"
+value = dict(first_name="Richard", last_name="Feynman")
+db.tables.names.put(key, value)
+
+temp = db.tables.names.get(key)
+assert temp == value
+
+db.new_table("abbrevs", serialize=SERIALIZE_STR)
+key = "l8r"
+value = "see you later"
+
+db.tables.abbrevs.put(key, value)
+temp = db.tables.abbrevs.get(key)
+assert temp == value
+
+db.close()
+```
 
 # Planned new features to come:
 
 * Implement a context manager on the Yuna class
-* Support integer keys
+* Support integer keys with a .insert() method providing autoincrement
 * Finish the Zstandard compression support
 * Add iterators to quickly find keys within a specified range
 * Add a REPL (Python with the yuna module already loaded and the DB open)
-
```

