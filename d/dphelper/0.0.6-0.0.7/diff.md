# Comparing `tmp/dphelper-0.0.6.tar.gz` & `tmp/dphelper-0.0.7.tar.gz`

## Comparing `dphelper-0.0.6.tar` & `dphelper-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 dphelper-0.0.6/steps.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dphelper-0.0.6/src/dphelper/__init__.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 dphelper-0.0.6/src/dphelper/config.py
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 dphelper-0.0.6/src/dphelper/helper.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 dphelper-0.0.6/src/dphelper/schemas.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 dphelper-0.0.6/src/dphelper/connection/__init__.py
--rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 dphelper-0.0.6/src/dphelper/connection/fetch.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dphelper-0.0.6/src/dphelper/snapshot/__init__.py
--rw-r--r--   0        0        0     8981 2020-02-02 00:00:00.000000 dphelper-0.0.6/src/dphelper/snapshot/snapshot.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 dphelper-0.0.6/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dphelper-0.0.6/license
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 dphelper-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 dphelper-0.0.6/readme.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 dphelper-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 dphelper-0.0.7/steps.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/__init__.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/config.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/helper.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/schemas.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/connection/__init__.py
+-rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/connection/fetch.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/snapshot/__init__.py
+-rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/snapshot/snapshot.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 dphelper-0.0.7/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dphelper-0.0.7/license
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 dphelper-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 dphelper-0.0.7/readme.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 dphelper-0.0.7/PKG-INFO
```

### Comparing `dphelper-0.0.6/src/dphelper/config.py` & `dphelper-0.0.7/src/dphelper/config.py`

 * *Files identical despite different names*

### Comparing `dphelper-0.0.6/src/dphelper/helper.py` & `dphelper-0.0.7/src/dphelper/helper.py`

 * *Files identical despite different names*

### Comparing `dphelper-0.0.6/src/dphelper/schemas.py` & `dphelper-0.0.7/src/dphelper/schemas.py`

 * *Files identical despite different names*

### Comparing `dphelper-0.0.6/src/dphelper/connection/fetch.py` & `dphelper-0.0.7/src/dphelper/connection/fetch.py`

 * *Files identical despite different names*

### Comparing `dphelper-0.0.6/src/dphelper/snapshot/snapshot.py` & `dphelper-0.0.7/src/dphelper/snapshot/snapshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         return self.__get_result_by_url_or_id(
             is_loadable=meta.is_result_json_loadable,
             result_file_url=meta.result_file_url,
             snapshot_id=snapshot_id,
         )
 
     def get_by_id(self, snapshot_id: int) -> _schemas.Snapshot:
-        "gets snapshot meta + snapshot result as a whole object. snapshot result is placed inside `json_data`"
+        "gets snapshot meta + snapshot result as a whole object. snapshot result is placed inside `result` attribute"
         meta = self.get_meta_by_id(snapshot_id)
         return _schemas.Snapshot(
             **meta.dict(),
             result=self.__get_result_by_url_or_id(
                 is_loadable=meta.is_result_json_loadable,
                 result_file_url=meta.result_file_url,
                 snapshot_id=snapshot_id,
@@ -176,15 +176,15 @@
         *,
         by_challenge_id: None | int = None,
         by_user_id: None | int = None,
         by_is_verified: None | bool = None,
         by_validation_statuses: None | list[str] = None,
         by_is_from_robot: None | bool = None,
     ) -> _schemas.Snapshot:
-        """gets latest snapshot meta+result by specified filters. result is stored inside `json_data` attribute
+        """gets latest snapshot meta+result by specified filters. result is stored inside `result` attribute
 
         :param by_challenge_id: to what challenge shall snapshot belong? If None, any will match.
         :param by_user_id: to what user shall snapshot belong? If None, any will match.
         :param by_is_verified: shall the snapshot be moderator-approved? If None, any will match.
         :param by_validation_statuses: searched statuses of snapshot validation. If None, any will match.
         :param by_is_from_robot: shall the snapshot be generated from robot code run (True) or uploaded by human (False)? If None, any will match.
         """
```

### Comparing `dphelper-0.0.6/.gitignore` & `dphelper-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `dphelper-0.0.6/PKG-INFO` & `dphelper-0.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dphelper
-Version: 0.0.6
+Version: 0.0.7
 Summary: Handle common scraping problems, help linking data platform entities
 Author-email: Egidijus Gylys <EgidijusGylys1@gmail.com>
 License-File: license
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.0
 Requires-Dist: fake-headers
```

