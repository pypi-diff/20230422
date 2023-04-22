# Comparing `tmp/dbxconfig-2.0.6.tar.gz` & `tmp/dbxconfig-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-2.0.6.tar", last modified: Sat Apr 22 17:28:17 2023, max compression
+gzip compressed data, was "dbxconfig-2.1.0.tar", last modified: Sat Apr 22 18:30:41 2023, max compression
```

## Comparing `dbxconfig-2.0.6.tar` & `dbxconfig-2.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:28:17.917150 dbxconfig-2.0.6/
--rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-22 17:28:17.917150 dbxconfig-2.0.6/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     2936 2023-04-22 17:27:26.000000 dbxconfig-2.0.6/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:28:17.913150 dbxconfig-2.0.6/dbxconfig/
--rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-04-22 17:27:26.000000 dbxconfig-2.0.6/dbxconfig/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2848 2023-04-22 17:27:26.000000 dbxconfig-2.0.6/dbxconfig/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)      166 2023-04-22 17:27:26.000000 dbxconfig-2.0.6/dbxconfig/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      780 2023-04-22 17:27:26.000000 dbxconfig-2.0.6/dbxconfig/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3513 2023-04-22 17:27:26.000000 dbxconfig-2.0.6/dbxconfig/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-04-22 17:27:26.000000 dbxconfig-2.0.6/dbxconfig/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1979 2023-04-22 17:27:26.000000 dbxconfig-2.0.6/dbxconfig/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:28:17.917150 dbxconfig-2.0.6/dbxconfig/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      200 2023-04-22 17:27:26.000000 dbxconfig-2.0.6/dbxconfig/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      903 2023-04-22 17:27:26.000000 dbxconfig-2.0.6/dbxconfig/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3139 2023-04-22 17:27:26.000000 dbxconfig-2.0.6/dbxconfig/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2781 2023-04-22 17:27:26.000000 dbxconfig-2.0.6/dbxconfig/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4982 2023-04-22 17:27:26.000000 dbxconfig-2.0.6/dbxconfig/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-04-22 17:27:26.000000 dbxconfig-2.0.6/dbxconfig/dataset/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:28:17.913150 dbxconfig-2.0.6/dbxconfig.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-22 17:28:17.000000 dbxconfig-2.0.6/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      544 2023-04-22 17:28:17.000000 dbxconfig-2.0.6/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-22 17:28:17.000000 dbxconfig-2.0.6/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-22 17:28:17.000000 dbxconfig-2.0.6/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       31 2023-04-22 17:28:17.000000 dbxconfig-2.0.6/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-22 17:28:17.000000 dbxconfig-2.0.6/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-22 17:28:17.917150 dbxconfig-2.0.6/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1103 2023-04-22 17:27:26.000000 dbxconfig-2.0.6/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 18:30:41.318809 dbxconfig-2.1.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-22 18:30:41.318809 dbxconfig-2.1.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     2936 2023-04-22 18:29:49.000000 dbxconfig-2.1.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 18:30:41.318809 dbxconfig-2.1.0/dbxconfig/
+-rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-04-22 18:29:49.000000 dbxconfig-2.1.0/dbxconfig/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2848 2023-04-22 18:29:49.000000 dbxconfig-2.1.0/dbxconfig/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      166 2023-04-22 18:29:49.000000 dbxconfig-2.1.0/dbxconfig/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1206 2023-04-22 18:29:49.000000 dbxconfig-2.1.0/dbxconfig/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3513 2023-04-22 18:29:49.000000 dbxconfig-2.1.0/dbxconfig/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-04-22 18:29:49.000000 dbxconfig-2.1.0/dbxconfig/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1979 2023-04-22 18:29:49.000000 dbxconfig-2.1.0/dbxconfig/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 18:30:41.318809 dbxconfig-2.1.0/dbxconfig/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      200 2023-04-22 18:29:49.000000 dbxconfig-2.1.0/dbxconfig/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      903 2023-04-22 18:29:49.000000 dbxconfig-2.1.0/dbxconfig/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3314 2023-04-22 18:29:49.000000 dbxconfig-2.1.0/dbxconfig/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3031 2023-04-22 18:29:49.000000 dbxconfig-2.1.0/dbxconfig/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4982 2023-04-22 18:29:49.000000 dbxconfig-2.1.0/dbxconfig/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-04-22 18:29:49.000000 dbxconfig-2.1.0/dbxconfig/dataset/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 18:30:41.318809 dbxconfig-2.1.0/dbxconfig.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-22 18:30:41.000000 dbxconfig-2.1.0/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      544 2023-04-22 18:30:41.000000 dbxconfig-2.1.0/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-22 18:30:41.000000 dbxconfig-2.1.0/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-22 18:30:41.000000 dbxconfig-2.1.0/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       31 2023-04-22 18:30:41.000000 dbxconfig-2.1.0/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-22 18:30:41.000000 dbxconfig-2.1.0/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-22 18:30:41.318809 dbxconfig-2.1.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1103 2023-04-22 18:29:49.000000 dbxconfig-2.1.0/setup.py
```

### Comparing `dbxconfig-2.0.6/PKG-INFO` & `dbxconfig-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 2.0.6
+Version: 2.1.0
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-2.0.6/README.md` & `dbxconfig-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.6/dbxconfig/_config.py` & `dbxconfig-2.1.0/dbxconfig/_config.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.6/dbxconfig/_table.py` & `dbxconfig-2.1.0/dbxconfig/_table.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 from pydantic import BaseModel, Field
 from typing import Union, List, Any, Dict
 from ._stage_type import StageType
 
 
+class ValidationThreshold(BaseModel):
+    def __init__(self, **data: Any) -> None:
+        super().__init__(**data)
+
+    invalid_ratio: float = Field(default=None)
+    invalid_rows: float = Field(default=None)
+    max_rows: int = Field(default=None)
+    min_rows: int = Field(default=None)
+
+
 class BaseTable(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     stage: StageType = Field(...)
     database: str = Field(...)
     name: str = Field(...)
@@ -15,14 +25,16 @@
 
 class Table(BaseTable):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     depends_on: List[str] = Field(default=[])
     table_properties: Dict[str, str] = Field(default=None)
+    warning_thresholds: ValidationThreshold = Field(default=None)
+    exception_thresholds: ValidationThreshold = Field(default=None)
 
 
 class TableMapping(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     destination: Table = Field(...)
```

### Comparing `dbxconfig-2.0.6/dbxconfig/_tables.py` & `dbxconfig-2.1.0/dbxconfig/_tables.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.6/dbxconfig/_timeslice.py` & `dbxconfig-2.1.0/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.6/dbxconfig/_utils.py` & `dbxconfig-2.1.0/dbxconfig/_utils.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.6/dbxconfig/dataset/_dataset.py` & `dbxconfig-2.1.0/dbxconfig/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.6/dbxconfig/dataset/_deltalake.py` & `dbxconfig-2.1.0/dbxconfig/dataset/_deltalake.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pydantic import Field, PrivateAttr
 from .._utils import JinjaVariables, render_jinja
 from typing import Any, Dict, Union
 from .._timeslice import Timeslice
 import os
 from .._stage_type import StageType
 from ._dataset import DataSet
+from .._table import ValidationThreshold
 
 try:
     from databricks.sdk.runtime import *  # noqa F403
 except ModuleNotFoundError:
     pass
 
 
@@ -35,14 +36,16 @@
     options: Union[dict, None] = Field(default=None)
     timeslice: Timeslice = Field(...)
     location: str = Field(default=None)
     checkpoint: str = Field(default=None)
     checkpoint_location: str = Field(default=None)
     table_properties: Dict[str, str] = Field(default=None)
     stage: StageType = Field(...)
+    warning_thresholds: ValidationThreshold = Field(default=None)
+    exception_thresholds: ValidationThreshold = Field(default=None)
 
     def _render(self):
         self._replacements = {
             JinjaVariables.TABLE: self.destination_table,
             JinjaVariables.DATABASE: self.database,
             JinjaVariables.CONTAINER: self.container,
             JinjaVariables.CHECKPOINT: self.checkpoint,
```

### Comparing `dbxconfig-2.0.6/dbxconfig/dataset/_factory.py` & `dbxconfig-2.1.0/dbxconfig/dataset/_factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 class _DatasetFactory:
     _TIMESLICE = "timeslice"
     _TABLE = "destination_table"
     _TABLE_PROPERTIES = "table_properties"
     _STAGE = "stage"
     _DATABASE = "database"
     _CONFIG_PATH = "config_path"
+    _WARNING_THRESHOLDS = "warning_thresholds"
+    _EXCEPTION_THRESHOLDS = "exception_thresholds"
 
     def __init__(self) -> None:
         self._logger = logging.getLogger(self.__class__.__name__)
         self._dataset = {}
 
     def register_dataset_type(self, io_type: StageType, dataset_type: type):
         self._logger.debug(f"Register dataset type {dataset_type} as {type}")
@@ -72,14 +74,16 @@
         stage_config = config[table.stage.name]
         stage_config[self._TIMESLICE] = timeslice
         stage_config[self._TABLE] = table.name
         stage_config[self._TABLE_PROPERTIES] = table.table_properties
         stage_config[self._STAGE] = table.stage
         stage_config[self._DATABASE] = table.database
         stage_config[self._CONFIG_PATH] = config[self._CONFIG_PATH]
+        stage_config[self._WARNING_THRESHOLDS] = table.warning_thresholds
+        stage_config[self._EXCEPTION_THRESHOLDS] = table.exception_thresholds
 
         return stage_config
 
 
 factory = _DatasetFactory()
 factory.register_dataset_type(IOType.READ, Read)
 factory.register_dataset_type(IOType.DELTALAKE, DeltaLake)
```

### Comparing `dbxconfig-2.0.6/dbxconfig/dataset/_read.py` & `dbxconfig-2.1.0/dbxconfig/dataset/_read.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.6/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-2.1.0/dbxconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 2.0.6
+Version: 2.1.0
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-2.0.6/dbxconfig.egg-info/SOURCES.txt` & `dbxconfig-2.1.0/dbxconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.6/setup.py` & `dbxconfig-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="2.0.6",
+    version="2.1.0",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```

