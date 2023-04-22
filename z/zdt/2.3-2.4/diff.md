# Comparing `tmp/zdt-2.3.tar.gz` & `tmp/zdt-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zdt-2.3.tar", last modified: Sat Apr 22 19:35:38 2023, max compression
+gzip compressed data, was "zdt-2.4.tar", last modified: Sat Apr 22 20:25:19 2023, max compression
```

## Comparing `zdt-2.3.tar` & `zdt-2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 19:35:38.689855 zdt-2.3/
--rw-rw-rw-   0        0        0      497 2023-04-22 19:35:38.682797 zdt-2.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-22 19:35:38.689855 zdt-2.3/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-04-22 19:35:27.000000 zdt-2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 19:35:38.631668 zdt-2.3/zdt/
--rw-rw-rw-   0        0        0       14 2023-01-28 14:07:23.000000 zdt-2.3/zdt/__init__.py
--rw-rw-rw-   0        0        0     3862 2023-04-22 18:57:55.000000 zdt-2.3/zdt/connector_utils.py
--rw-rw-rw-   0        0        0     2305 2023-01-11 07:53:57.000000 zdt-2.3/zdt/country_map_master.py
--rw-rw-rw-   0        0        0     2039 2022-12-06 02:32:30.000000 zdt-2.3/zdt/hana_connector_utils.py
--rw-rw-rw-   0        0        0      644 2022-12-08 09:40:05.000000 zdt-2.3/zdt/log_func.py
--rw-rw-rw-   0        0        0      813 2022-11-29 12:48:34.000000 zdt-2.3/zdt/random_utils.py
--rw-rw-rw-   0        0        0    10407 2023-04-22 19:33:30.000000 zdt-2.3/zdt/time_func.py
-drwxrwxrwx   0        0        0        0 2023-04-22 19:35:38.675798 zdt-2.3/zdt.egg-info/
--rw-rw-rw-   0        0        0      497 2023-04-22 19:35:38.000000 zdt-2.3/zdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-04-22 19:35:38.000000 zdt-2.3/zdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 19:35:38.000000 zdt-2.3/zdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-04-22 19:35:38.000000 zdt-2.3/zdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-22 19:35:38.000000 zdt-2.3/zdt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 20:25:19.405942 zdt-2.4/
+-rw-rw-rw-   0        0        0      497 2023-04-22 20:25:19.398988 zdt-2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-22 20:25:19.405942 zdt-2.4/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-04-22 20:23:36.000000 zdt-2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 20:25:19.331866 zdt-2.4/zdt/
+-rw-rw-rw-   0        0        0       14 2023-01-28 14:07:23.000000 zdt-2.4/zdt/__init__.py
+-rw-rw-rw-   0        0        0     4067 2023-04-22 20:23:02.000000 zdt-2.4/zdt/connector_utils.py
+-rw-rw-rw-   0        0        0     2305 2023-01-11 07:53:57.000000 zdt-2.4/zdt/country_map_master.py
+-rw-rw-rw-   0        0        0     2039 2022-12-06 02:32:30.000000 zdt-2.4/zdt/hana_connector_utils.py
+-rw-rw-rw-   0        0        0      644 2022-12-08 09:40:05.000000 zdt-2.4/zdt/log_func.py
+-rw-rw-rw-   0        0        0      813 2022-11-29 12:48:34.000000 zdt-2.4/zdt/random_utils.py
+-rw-rw-rw-   0        0        0    10407 2023-04-22 19:33:30.000000 zdt-2.4/zdt/time_func.py
+drwxrwxrwx   0        0        0        0 2023-04-22 20:25:19.390360 zdt-2.4/zdt.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-04-22 20:25:18.000000 zdt-2.4/zdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-04-22 20:25:19.000000 zdt-2.4/zdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 20:25:18.000000 zdt-2.4/zdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-04-22 20:25:18.000000 zdt-2.4/zdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-22 20:25:18.000000 zdt-2.4/zdt.egg-info/top_level.txt
```

### Comparing `zdt-2.3/setup.py` & `zdt-2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '2.3'
+VERSION = '2.4'
 DESCRIPTION = 'zdt'
 
 # Setting up
 setup(
     name="zdt",
     version=VERSION,
     author="Dickson",
```

### Comparing `zdt-2.3/zdt/connector_utils.py` & `zdt-2.4/zdt/connector_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -105,15 +105,21 @@
 
     download = file_client.download_file()
 
     downloaded_bytes = download.readall()
 
     return BytesIO(downloaded_bytes)
 
-def get_azure_file_paths(variable_name = 'dag_var1', account_name = 'zpcsmdevdatalake',container_name = 'raw', directory_name = "BDP",):
+def get_azure_file_paths(account_key = 'default_airflow', variable_name = 'dag_var1', account_name = 'zpcsmdevdatalake',container_name = 'raw', directory_name = "BDP",):
+
+    if account_key == 'default_airflow':
+
+        variable_list = Variable.get(variable_name, deserialize_json=True)
+
+        account_key = variable_list['acc_key']
 
     variable_list = Variable.get(variable_name, deserialize_json=True)
 
     account_key = variable_list['acc_key']
 
     service_client = DataLakeServiceClient(account_url="{}://{}.dfs.core.windows.net".format(
             "https", account_name), credential=account_key)
```

### Comparing `zdt-2.3/zdt/country_map_master.py` & `zdt-2.4/zdt/country_map_master.py`

 * *Files identical despite different names*

### Comparing `zdt-2.3/zdt/hana_connector_utils.py` & `zdt-2.4/zdt/hana_connector_utils.py`

 * *Files identical despite different names*

### Comparing `zdt-2.3/zdt/log_func.py` & `zdt-2.4/zdt/log_func.py`

 * *Files identical despite different names*

### Comparing `zdt-2.3/zdt/random_utils.py` & `zdt-2.4/zdt/random_utils.py`

 * *Files identical despite different names*

### Comparing `zdt-2.3/zdt/time_func.py` & `zdt-2.4/zdt/time_func.py`

 * *Files identical despite different names*

