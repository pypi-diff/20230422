# Comparing `tmp/zdt-2.2.tar.gz` & `tmp/zdt-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zdt-2.2.tar", last modified: Sat Apr 22 19:15:46 2023, max compression
+gzip compressed data, was "zdt-2.3.tar", last modified: Sat Apr 22 19:35:38 2023, max compression
```

## Comparing `zdt-2.2.tar` & `zdt-2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 19:15:46.933099 zdt-2.2/
--rw-rw-rw-   0        0        0      497 2023-04-22 19:15:46.926093 zdt-2.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-22 19:15:46.933099 zdt-2.2/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-04-22 18:50:10.000000 zdt-2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 19:15:46.874330 zdt-2.2/zdt/
--rw-rw-rw-   0        0        0       14 2023-01-28 14:07:23.000000 zdt-2.2/zdt/__init__.py
--rw-rw-rw-   0        0        0     3862 2023-04-22 18:57:55.000000 zdt-2.2/zdt/connector_utils.py
--rw-rw-rw-   0        0        0     2305 2023-01-11 07:53:57.000000 zdt-2.2/zdt/country_map_master.py
--rw-rw-rw-   0        0        0     2039 2022-12-06 02:32:30.000000 zdt-2.2/zdt/hana_connector_utils.py
--rw-rw-rw-   0        0        0      644 2022-12-08 09:40:05.000000 zdt-2.2/zdt/log_func.py
--rw-rw-rw-   0        0        0      813 2022-11-29 12:48:34.000000 zdt-2.2/zdt/random_utils.py
--rw-rw-rw-   0        0        0    10380 2023-04-22 19:11:18.000000 zdt-2.2/zdt/time_func.py
-drwxrwxrwx   0        0        0        0 2023-04-22 19:15:46.919078 zdt-2.2/zdt.egg-info/
--rw-rw-rw-   0        0        0      497 2023-04-22 19:15:46.000000 zdt-2.2/zdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-04-22 19:15:46.000000 zdt-2.2/zdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 19:15:46.000000 zdt-2.2/zdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-04-22 19:15:46.000000 zdt-2.2/zdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-22 19:15:46.000000 zdt-2.2/zdt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 19:35:38.689855 zdt-2.3/
+-rw-rw-rw-   0        0        0      497 2023-04-22 19:35:38.682797 zdt-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-22 19:35:38.689855 zdt-2.3/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-04-22 19:35:27.000000 zdt-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 19:35:38.631668 zdt-2.3/zdt/
+-rw-rw-rw-   0        0        0       14 2023-01-28 14:07:23.000000 zdt-2.3/zdt/__init__.py
+-rw-rw-rw-   0        0        0     3862 2023-04-22 18:57:55.000000 zdt-2.3/zdt/connector_utils.py
+-rw-rw-rw-   0        0        0     2305 2023-01-11 07:53:57.000000 zdt-2.3/zdt/country_map_master.py
+-rw-rw-rw-   0        0        0     2039 2022-12-06 02:32:30.000000 zdt-2.3/zdt/hana_connector_utils.py
+-rw-rw-rw-   0        0        0      644 2022-12-08 09:40:05.000000 zdt-2.3/zdt/log_func.py
+-rw-rw-rw-   0        0        0      813 2022-11-29 12:48:34.000000 zdt-2.3/zdt/random_utils.py
+-rw-rw-rw-   0        0        0    10407 2023-04-22 19:33:30.000000 zdt-2.3/zdt/time_func.py
+drwxrwxrwx   0        0        0        0 2023-04-22 19:35:38.675798 zdt-2.3/zdt.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-04-22 19:35:38.000000 zdt-2.3/zdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-04-22 19:35:38.000000 zdt-2.3/zdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 19:35:38.000000 zdt-2.3/zdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-04-22 19:35:38.000000 zdt-2.3/zdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-22 19:35:38.000000 zdt-2.3/zdt.egg-info/top_level.txt
```

### Comparing `zdt-2.2/setup.py` & `zdt-2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '2.2'
+VERSION = '2.3'
 DESCRIPTION = 'zdt'
 
 # Setting up
 setup(
     name="zdt",
     version=VERSION,
     author="Dickson",
```

### Comparing `zdt-2.2/zdt/connector_utils.py` & `zdt-2.3/zdt/connector_utils.py`

 * *Files identical despite different names*

### Comparing `zdt-2.2/zdt/country_map_master.py` & `zdt-2.3/zdt/country_map_master.py`

 * *Files identical despite different names*

### Comparing `zdt-2.2/zdt/hana_connector_utils.py` & `zdt-2.3/zdt/hana_connector_utils.py`

 * *Files identical despite different names*

### Comparing `zdt-2.2/zdt/log_func.py` & `zdt-2.3/zdt/log_func.py`

 * *Files identical despite different names*

### Comparing `zdt-2.2/zdt/random_utils.py` & `zdt-2.3/zdt/random_utils.py`

 * *Files identical despite different names*

### Comparing `zdt-2.2/zdt/time_func.py` & `zdt-2.3/zdt/time_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,15 @@
     if part == 2:
 
         split_start_list = start_period_list[split_point:]
         split_end_list = end_period_list[split_point:]
 
         return split_start_list, split_end_list
 
-def get_time_periods(delta: int, delta_unit: str, time_func_name: str, end_date = (dt.datetime.now().date()-dt.timedelta(days=1))):
+def get_time_periods(delta: int, delta_unit: str, time_func_name='generate_monthly_time_periods', end_date = (dt.datetime.now().date()-dt.timedelta(days=1))):
 
     '''
 
     This function creates the start and end periods in the form of lists
     '''
     # default end_date is yesterday's date
```

