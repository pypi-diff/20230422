# Comparing `tmp/dbxconfig-2.0.1.tar.gz` & `tmp/dbxconfig-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-2.0.1.tar", last modified: Sat Apr 22 16:27:31 2023, max compression
+gzip compressed data, was "dbxconfig-2.0.3.tar", last modified: Sat Apr 22 17:04:21 2023, max compression
```

## Comparing `dbxconfig-2.0.1.tar` & `dbxconfig-2.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 16:27:31.903112 dbxconfig-2.0.1/
--rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-22 16:27:31.903112 dbxconfig-2.0.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     2936 2023-04-22 16:26:38.000000 dbxconfig-2.0.1/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 16:27:31.903112 dbxconfig-2.0.1/dbxconfig/
--rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-04-22 16:26:38.000000 dbxconfig-2.0.1/dbxconfig/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2827 2023-04-22 16:26:38.000000 dbxconfig-2.0.1/dbxconfig/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)      166 2023-04-22 16:26:38.000000 dbxconfig-2.0.1/dbxconfig/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      780 2023-04-22 16:26:38.000000 dbxconfig-2.0.1/dbxconfig/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3513 2023-04-22 16:26:38.000000 dbxconfig-2.0.1/dbxconfig/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-04-22 16:26:38.000000 dbxconfig-2.0.1/dbxconfig/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1979 2023-04-22 16:26:38.000000 dbxconfig-2.0.1/dbxconfig/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 16:27:31.903112 dbxconfig-2.0.1/dbxconfig/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      200 2023-04-22 16:26:38.000000 dbxconfig-2.0.1/dbxconfig/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      903 2023-04-22 16:26:38.000000 dbxconfig-2.0.1/dbxconfig/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3088 2023-04-22 16:26:38.000000 dbxconfig-2.0.1/dbxconfig/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2781 2023-04-22 16:26:38.000000 dbxconfig-2.0.1/dbxconfig/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4982 2023-04-22 16:26:38.000000 dbxconfig-2.0.1/dbxconfig/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-04-22 16:26:38.000000 dbxconfig-2.0.1/dbxconfig/dataset/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 16:27:31.903112 dbxconfig-2.0.1/dbxconfig.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-22 16:27:31.000000 dbxconfig-2.0.1/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      544 2023-04-22 16:27:31.000000 dbxconfig-2.0.1/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-22 16:27:31.000000 dbxconfig-2.0.1/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-22 16:27:31.000000 dbxconfig-2.0.1/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       31 2023-04-22 16:27:31.000000 dbxconfig-2.0.1/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-22 16:27:31.000000 dbxconfig-2.0.1/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-22 16:27:31.903112 dbxconfig-2.0.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1103 2023-04-22 16:26:38.000000 dbxconfig-2.0.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:04:21.788038 dbxconfig-2.0.3/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-22 17:04:21.788038 dbxconfig-2.0.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     2936 2023-04-22 17:03:27.000000 dbxconfig-2.0.3/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:04:21.788038 dbxconfig-2.0.3/dbxconfig/
+-rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-04-22 17:03:27.000000 dbxconfig-2.0.3/dbxconfig/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2835 2023-04-22 17:03:27.000000 dbxconfig-2.0.3/dbxconfig/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      166 2023-04-22 17:03:27.000000 dbxconfig-2.0.3/dbxconfig/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      780 2023-04-22 17:03:27.000000 dbxconfig-2.0.3/dbxconfig/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3513 2023-04-22 17:03:27.000000 dbxconfig-2.0.3/dbxconfig/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-04-22 17:03:27.000000 dbxconfig-2.0.3/dbxconfig/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1979 2023-04-22 17:03:27.000000 dbxconfig-2.0.3/dbxconfig/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:04:21.788038 dbxconfig-2.0.3/dbxconfig/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      200 2023-04-22 17:03:27.000000 dbxconfig-2.0.3/dbxconfig/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      903 2023-04-22 17:03:27.000000 dbxconfig-2.0.3/dbxconfig/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3088 2023-04-22 17:03:27.000000 dbxconfig-2.0.3/dbxconfig/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2781 2023-04-22 17:03:27.000000 dbxconfig-2.0.3/dbxconfig/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4982 2023-04-22 17:03:27.000000 dbxconfig-2.0.3/dbxconfig/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-04-22 17:03:27.000000 dbxconfig-2.0.3/dbxconfig/dataset/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-22 17:04:21.788038 dbxconfig-2.0.3/dbxconfig.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-22 17:04:21.000000 dbxconfig-2.0.3/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      544 2023-04-22 17:04:21.000000 dbxconfig-2.0.3/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-22 17:04:21.000000 dbxconfig-2.0.3/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-22 17:04:21.000000 dbxconfig-2.0.3/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       31 2023-04-22 17:04:21.000000 dbxconfig-2.0.3/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-22 17:04:21.000000 dbxconfig-2.0.3/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-22 17:04:21.788038 dbxconfig-2.0.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1103 2023-04-22 17:03:27.000000 dbxconfig-2.0.3/setup.py
```

### Comparing `dbxconfig-2.0.1/PKG-INFO` & `dbxconfig-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 2.0.1
+Version: 2.0.3
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-2.0.1/README.md` & `dbxconfig-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.1/dbxconfig/_config.py` & `dbxconfig-2.0.3/dbxconfig/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,9 +80,9 @@
     ):
         if not checkpoint_name:
             checkpoint_name = f"{source.database}.{source.table}-{destination.database}.{destination.table}"
 
         source.checkpoint = checkpoint_name
         source._render()
         destination.checkpoint = checkpoint_name
-        destination.options["checkpoint"] = "{{ checkpoint }}"
+        destination.options["checkpointLocation"] = "{{ checkpoint }}"
         destination._render()
```

### Comparing `dbxconfig-2.0.1/dbxconfig/_table.py` & `dbxconfig-2.0.3/dbxconfig/_table.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.1/dbxconfig/_tables.py` & `dbxconfig-2.0.3/dbxconfig/_tables.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.1/dbxconfig/_timeslice.py` & `dbxconfig-2.0.3/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.1/dbxconfig/_utils.py` & `dbxconfig-2.0.3/dbxconfig/_utils.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.1/dbxconfig/dataset/_dataset.py` & `dbxconfig-2.0.3/dbxconfig/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.1/dbxconfig/dataset/_deltalake.py` & `dbxconfig-2.0.3/dbxconfig/dataset/_deltalake.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.1/dbxconfig/dataset/_factory.py` & `dbxconfig-2.0.3/dbxconfig/dataset/_factory.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.1/dbxconfig/dataset/_read.py` & `dbxconfig-2.0.3/dbxconfig/dataset/_read.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.1/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-2.0.3/dbxconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 2.0.1
+Version: 2.0.3
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-2.0.1/dbxconfig.egg-info/SOURCES.txt` & `dbxconfig-2.0.3/dbxconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.0.1/setup.py` & `dbxconfig-2.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="2.0.1",
+    version="2.0.3",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```

