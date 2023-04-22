# Comparing `tmp/zdt-2.5.tar.gz` & `tmp/zdt-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zdt-2.5.tar", last modified: Sat Apr 22 20:48:23 2023, max compression
+gzip compressed data, was "zdt-2.6.tar", last modified: Sat Apr 22 21:10:29 2023, max compression
```

## Comparing `zdt-2.5.tar` & `zdt-2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 20:48:23.108101 zdt-2.5/
--rw-rw-rw-   0        0        0      497 2023-04-22 20:48:23.102101 zdt-2.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-22 20:48:23.109081 zdt-2.5/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-04-22 20:48:11.000000 zdt-2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 20:48:23.041557 zdt-2.5/zdt/
--rw-rw-rw-   0        0        0       14 2023-01-28 14:07:23.000000 zdt-2.5/zdt/__init__.py
--rw-rw-rw-   0        0        0     4117 2023-04-22 20:47:21.000000 zdt-2.5/zdt/connector_utils.py
--rw-rw-rw-   0        0        0     2305 2023-01-11 07:53:57.000000 zdt-2.5/zdt/country_map_master.py
--rw-rw-rw-   0        0        0     2039 2022-12-06 02:32:30.000000 zdt-2.5/zdt/hana_connector_utils.py
--rw-rw-rw-   0        0        0      644 2022-12-08 09:40:05.000000 zdt-2.5/zdt/log_func.py
--rw-rw-rw-   0        0        0      813 2022-11-29 12:48:34.000000 zdt-2.5/zdt/random_utils.py
--rw-rw-rw-   0        0        0    10407 2023-04-22 19:33:30.000000 zdt-2.5/zdt/time_func.py
-drwxrwxrwx   0        0        0        0 2023-04-22 20:48:23.096101 zdt-2.5/zdt.egg-info/
--rw-rw-rw-   0        0        0      497 2023-04-22 20:48:22.000000 zdt-2.5/zdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-04-22 20:48:22.000000 zdt-2.5/zdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 20:48:22.000000 zdt-2.5/zdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-04-22 20:48:22.000000 zdt-2.5/zdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-22 20:48:22.000000 zdt-2.5/zdt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 21:10:29.136013 zdt-2.6/
+-rw-rw-rw-   0        0        0      497 2023-04-22 21:10:29.128053 zdt-2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-22 21:10:29.136989 zdt-2.6/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-04-22 21:10:02.000000 zdt-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 21:10:29.060656 zdt-2.6/zdt/
+-rw-rw-rw-   0        0        0       14 2023-01-28 14:07:23.000000 zdt-2.6/zdt/__init__.py
+-rw-rw-rw-   0        0        0     4106 2023-04-22 21:09:07.000000 zdt-2.6/zdt/connector_utils.py
+-rw-rw-rw-   0        0        0     2305 2023-01-11 07:53:57.000000 zdt-2.6/zdt/country_map_master.py
+-rw-rw-rw-   0        0        0     2039 2022-12-06 02:32:30.000000 zdt-2.6/zdt/hana_connector_utils.py
+-rw-rw-rw-   0        0        0      644 2022-12-08 09:40:05.000000 zdt-2.6/zdt/log_func.py
+-rw-rw-rw-   0        0        0      813 2022-11-29 12:48:34.000000 zdt-2.6/zdt/random_utils.py
+-rw-rw-rw-   0        0        0    10407 2023-04-22 19:33:30.000000 zdt-2.6/zdt/time_func.py
+drwxrwxrwx   0        0        0        0 2023-04-22 21:10:29.117979 zdt-2.6/zdt.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-04-22 21:10:28.000000 zdt-2.6/zdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-04-22 21:10:28.000000 zdt-2.6/zdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 21:10:28.000000 zdt-2.6/zdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-04-22 21:10:28.000000 zdt-2.6/zdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-22 21:10:28.000000 zdt-2.6/zdt.egg-info/top_level.txt
```

### Comparing `zdt-2.5/setup.py` & `zdt-2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '2.5'
+VERSION = '2.6'
 DESCRIPTION = 'zdt'
 
 # Setting up
 setup(
     name="zdt",
     version=VERSION,
     author="Dickson",
```

### Comparing `zdt-2.5/zdt/connector_utils.py` & `zdt-2.6/zdt/connector_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
     return BytesIO(downloaded_bytes)
 
 def get_azure_file_paths(account_key = 'default_airflow', variable_name = 'dag_var1', account_name = 'zpcsmdevdatalake',container_name = 'raw', directory_name = "BDP",):
  
     '''If account_key = default_airflow, then will get from airflow variables'''
 
-    if account_key == 'default_airflow': 
+    if account_key == 'default_airflow':
 
         variable_list = Variable.get(variable_name, deserialize_json=True)
 
         account_key = variable_list['acc_key']
 
     service_client = DataLakeServiceClient(account_url="{}://{}.dfs.core.windows.net".format(
             "https", account_name), credential=account_key)
@@ -128,10 +128,10 @@
 
     paths = file_system_client.get_paths(path=directory_name)
 
     path_list = [*paths]
 
     path_list2=[path.name for path in path_list]
 
-    path_list3 = [x.split(directory_name)[1] for x in path_list2]
+    path_list3 = [x.split('/')[-1] for x in path_list2]
 
     return path_list3
```

### Comparing `zdt-2.5/zdt/country_map_master.py` & `zdt-2.6/zdt/country_map_master.py`

 * *Files identical despite different names*

### Comparing `zdt-2.5/zdt/hana_connector_utils.py` & `zdt-2.6/zdt/hana_connector_utils.py`

 * *Files identical despite different names*

### Comparing `zdt-2.5/zdt/log_func.py` & `zdt-2.6/zdt/log_func.py`

 * *Files identical despite different names*

### Comparing `zdt-2.5/zdt/random_utils.py` & `zdt-2.6/zdt/random_utils.py`

 * *Files identical despite different names*

### Comparing `zdt-2.5/zdt/time_func.py` & `zdt-2.6/zdt/time_func.py`

 * *Files identical despite different names*

