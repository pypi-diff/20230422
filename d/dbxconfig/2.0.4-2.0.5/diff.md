# Comparing `tmp/dbxconfig-2.0.4.tar.gz` & `tmp/dbxconfig-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-2.0.4.tar", last modified: Sat Apr 22 17:11:31 2023, max compression
+gzip compressed data, was "dbxconfig-2.0.5.tar", last modified: Sat Apr 22 17:18:23 2023, max compression
```

## Comparing `dbxconfig-2.0.4.tar` & `dbxconfig-2.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:11:31.665827 dbxconfig-2.0.4/
--rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-22 17:11:31.665827 dbxconfig-2.0.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     2936 2023-04-22 17:10:34.000000 dbxconfig-2.0.4/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:11:31.661827 dbxconfig-2.0.4/dbxconfig/
--rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-04-22 17:10:34.000000 dbxconfig-2.0.4/dbxconfig/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2847 2023-04-22 17:10:34.000000 dbxconfig-2.0.4/dbxconfig/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)      166 2023-04-22 17:10:34.000000 dbxconfig-2.0.4/dbxconfig/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      780 2023-04-22 17:10:34.000000 dbxconfig-2.0.4/dbxconfig/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3513 2023-04-22 17:10:34.000000 dbxconfig-2.0.4/dbxconfig/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-04-22 17:10:34.000000 dbxconfig-2.0.4/dbxconfig/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1979 2023-04-22 17:10:34.000000 dbxconfig-2.0.4/dbxconfig/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:11:31.665827 dbxconfig-2.0.4/dbxconfig/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      200 2023-04-22 17:10:34.000000 dbxconfig-2.0.4/dbxconfig/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      903 2023-04-22 17:10:34.000000 dbxconfig-2.0.4/dbxconfig/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3230 2023-04-22 17:10:34.000000 dbxconfig-2.0.4/dbxconfig/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2781 2023-04-22 17:10:34.000000 dbxconfig-2.0.4/dbxconfig/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4982 2023-04-22 17:10:34.000000 dbxconfig-2.0.4/dbxconfig/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-04-22 17:10:34.000000 dbxconfig-2.0.4/dbxconfig/dataset/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:11:31.661827 dbxconfig-2.0.4/dbxconfig.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-22 17:11:31.000000 dbxconfig-2.0.4/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      544 2023-04-22 17:11:31.000000 dbxconfig-2.0.4/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-22 17:11:31.000000 dbxconfig-2.0.4/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-22 17:11:31.000000 dbxconfig-2.0.4/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       31 2023-04-22 17:11:31.000000 dbxconfig-2.0.4/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-22 17:11:31.000000 dbxconfig-2.0.4/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-22 17:11:31.665827 dbxconfig-2.0.4/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1103 2023-04-22 17:10:34.000000 dbxconfig-2.0.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:18:23.240940 dbxconfig-2.0.5/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-22 17:18:23.240940 dbxconfig-2.0.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     2936 2023-04-22 17:17:27.000000 dbxconfig-2.0.5/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:18:23.236940 dbxconfig-2.0.5/dbxconfig/
+-rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-04-22 17:17:27.000000 dbxconfig-2.0.5/dbxconfig/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2848 2023-04-22 17:17:27.000000 dbxconfig-2.0.5/dbxconfig/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      166 2023-04-22 17:17:27.000000 dbxconfig-2.0.5/dbxconfig/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      780 2023-04-22 17:17:27.000000 dbxconfig-2.0.5/dbxconfig/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3513 2023-04-22 17:17:27.000000 dbxconfig-2.0.5/dbxconfig/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-04-22 17:17:27.000000 dbxconfig-2.0.5/dbxconfig/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1979 2023-04-22 17:17:27.000000 dbxconfig-2.0.5/dbxconfig/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:18:23.240940 dbxconfig-2.0.5/dbxconfig/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      200 2023-04-22 17:17:27.000000 dbxconfig-2.0.5/dbxconfig/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      903 2023-04-22 17:17:27.000000 dbxconfig-2.0.5/dbxconfig/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3233 2023-04-22 17:17:27.000000 dbxconfig-2.0.5/dbxconfig/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2781 2023-04-22 17:17:27.000000 dbxconfig-2.0.5/dbxconfig/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4982 2023-04-22 17:17:27.000000 dbxconfig-2.0.5/dbxconfig/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-04-22 17:17:27.000000 dbxconfig-2.0.5/dbxconfig/dataset/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:18:23.236940 dbxconfig-2.0.5/dbxconfig.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-22 17:18:23.000000 dbxconfig-2.0.5/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      544 2023-04-22 17:18:23.000000 dbxconfig-2.0.5/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-22 17:18:23.000000 dbxconfig-2.0.5/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-22 17:18:23.000000 dbxconfig-2.0.5/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       31 2023-04-22 17:18:23.000000 dbxconfig-2.0.5/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-22 17:18:23.000000 dbxconfig-2.0.5/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-22 17:18:23.240940 dbxconfig-2.0.5/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1103 2023-04-22 17:17:27.000000 dbxconfig-2.0.5/setup.py
```

### Comparing `dbxconfig-2.0.4/PKG-INFO` & `dbxconfig-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 2.0.4
+Version: 2.0.5
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-2.0.4/README.md` & `dbxconfig-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.4/dbxconfig/_config.py` & `dbxconfig-2.0.5/dbxconfig/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,9 +80,9 @@
     ):
         if not checkpoint_name:
             checkpoint_name = f"{source.database}.{source.table}-{destination.database}.{destination.table}"
 
         source.checkpoint = checkpoint_name
         source._render()
         destination.checkpoint = checkpoint_name
-        destination.options["checkpointLocation"] = destination.checkpointLocation
+        destination.options["checkpointLocation"] = destination.checkpoint_location
         destination._render()
```

### Comparing `dbxconfig-2.0.4/dbxconfig/_table.py` & `dbxconfig-2.0.5/dbxconfig/_table.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.4/dbxconfig/_tables.py` & `dbxconfig-2.0.5/dbxconfig/_tables.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.4/dbxconfig/_timeslice.py` & `dbxconfig-2.0.5/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.4/dbxconfig/_utils.py` & `dbxconfig-2.0.5/dbxconfig/_utils.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.4/dbxconfig/dataset/_dataset.py` & `dbxconfig-2.0.5/dbxconfig/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.4/dbxconfig/dataset/_deltalake.py` & `dbxconfig-2.0.5/dbxconfig/dataset/_deltalake.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     container: str = Field(...)
     root: str = Field(...)
     path: str = Field(...)
     options: Union[dict, None] = Field(default=None)
     timeslice: Timeslice = Field(...)
     location: str = Field(default=None)
     checkpoint: str = Field(default=None)
-    checkpointLocation: str = Field(default=None)
+    checkpoint_location: str = Field(default=None)
     table_properties: Dict[str, str] = Field(default=None)
     stage: StageType = Field(...)
 
     def _render(self):
         self._replacements = {
             JinjaVariables.TABLE: self.destination_table,
             JinjaVariables.DATABASE: self.database,
@@ -48,15 +48,15 @@
             JinjaVariables.CHECKPOINT: self.checkpoint,
         }
 
         self.root = render_jinja(self.root, self._replacements)
         self.path = render_jinja(self.path, self._replacements)
         self.database = render_jinja(self.database, self._replacements)
         self.table = render_jinja(self.table, self._replacements)
-        self.checkpointLocation = render_jinja(self.checkpointLocation, self._replacements)
+        self.checkpoint_location = render_jinja(self.checkpoint_location, self._replacements)
         if self.options:
             for option, value in self.options.items():
                 self.options[option] = render_jinja(value, self._replacements)
 
         self.location = os.path.join(self.root, self.path)
 
     def create_table(self):
```

### Comparing `dbxconfig-2.0.4/dbxconfig/dataset/_factory.py` & `dbxconfig-2.0.5/dbxconfig/dataset/_factory.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.4/dbxconfig/dataset/_read.py` & `dbxconfig-2.0.5/dbxconfig/dataset/_read.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.4/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-2.0.5/dbxconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 2.0.4
+Version: 2.0.5
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-2.0.4/dbxconfig.egg-info/SOURCES.txt` & `dbxconfig-2.0.5/dbxconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.4/setup.py` & `dbxconfig-2.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="2.0.4",
+    version="2.0.5",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```
