# Comparing `tmp/zdt-2.1.tar.gz` & `tmp/zdt-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zdt-2.1.tar", last modified: Fri Feb  3 20:14:27 2023, max compression
+gzip compressed data, was "zdt-2.2.tar", last modified: Sat Apr 22 19:15:46 2023, max compression
```

## Comparing `zdt-2.1.tar` & `zdt-2.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-03 20:14:27.698943 zdt-2.1/
--rw-rw-rw-   0        0        0      418 2023-02-03 20:14:27.695940 zdt-2.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-02-03 20:14:27.698943 zdt-2.1/setup.cfg
--rw-rw-rw-   0        0        0      750 2023-02-03 20:11:56.000000 zdt-2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-03 20:14:27.664942 zdt-2.1/zdt/
--rw-rw-rw-   0        0        0       14 2023-01-28 14:07:23.000000 zdt-2.1/zdt/__init__.py
--rw-rw-rw-   0        0        0     2305 2023-01-11 07:53:57.000000 zdt-2.1/zdt/country_map_master.py
--rw-rw-rw-   0        0        0     2039 2022-12-06 02:32:30.000000 zdt-2.1/zdt/hana_connector_utils.py
--rw-rw-rw-   0        0        0      644 2022-12-08 09:40:05.000000 zdt-2.1/zdt/log_func.py
--rw-rw-rw-   0        0        0      813 2022-11-29 12:48:34.000000 zdt-2.1/zdt/random_utils.py
--rw-rw-rw-   0        0        0     9854 2023-02-03 20:09:24.000000 zdt-2.1/zdt/time_func.py
-drwxrwxrwx   0        0        0        0 2023-02-03 20:14:27.692940 zdt-2.1/zdt.egg-info/
--rw-rw-rw-   0        0        0      418 2023-02-03 20:14:27.000000 zdt-2.1/zdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-02-03 20:14:27.000000 zdt-2.1/zdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-03 20:14:27.000000 zdt-2.1/zdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-02-03 20:14:27.000000 zdt-2.1/zdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-02-03 20:14:27.000000 zdt-2.1/zdt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 19:15:46.933099 zdt-2.2/
+-rw-rw-rw-   0        0        0      497 2023-04-22 19:15:46.926093 zdt-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-22 19:15:46.933099 zdt-2.2/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-04-22 18:50:10.000000 zdt-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 19:15:46.874330 zdt-2.2/zdt/
+-rw-rw-rw-   0        0        0       14 2023-01-28 14:07:23.000000 zdt-2.2/zdt/__init__.py
+-rw-rw-rw-   0        0        0     3862 2023-04-22 18:57:55.000000 zdt-2.2/zdt/connector_utils.py
+-rw-rw-rw-   0        0        0     2305 2023-01-11 07:53:57.000000 zdt-2.2/zdt/country_map_master.py
+-rw-rw-rw-   0        0        0     2039 2022-12-06 02:32:30.000000 zdt-2.2/zdt/hana_connector_utils.py
+-rw-rw-rw-   0        0        0      644 2022-12-08 09:40:05.000000 zdt-2.2/zdt/log_func.py
+-rw-rw-rw-   0        0        0      813 2022-11-29 12:48:34.000000 zdt-2.2/zdt/random_utils.py
+-rw-rw-rw-   0        0        0    10380 2023-04-22 19:11:18.000000 zdt-2.2/zdt/time_func.py
+drwxrwxrwx   0        0        0        0 2023-04-22 19:15:46.919078 zdt-2.2/zdt.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-04-22 19:15:46.000000 zdt-2.2/zdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-04-22 19:15:46.000000 zdt-2.2/zdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 19:15:46.000000 zdt-2.2/zdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-04-22 19:15:46.000000 zdt-2.2/zdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-22 19:15:46.000000 zdt-2.2/zdt.egg-info/top_level.txt
```

### Comparing `zdt-2.1/setup.py` & `zdt-2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '2.1'
+VERSION = '2.2'
 DESCRIPTION = 'zdt'
 
 # Setting up
 setup(
     name="zdt",
     version=VERSION,
     author="Dickson",
     author_email="<suwon2912@gmail.com>",
     description=DESCRIPTION,
     packages=find_packages(),
-    install_requires=['sqlalchemy', 'typing', 'hdbcli','redmail','pandas>=1.1','datetime','python-dateutil','numpy'],
+    install_requires=['sqlalchemy', 'typing', 'hdbcli','redmail','pandas>=1.1','datetime','python-dateutil','numpy','apache-airflow','azure-storage-file-datalake'],
     keywords=['python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `zdt-2.1/zdt/country_map_master.py` & `zdt-2.2/zdt/country_map_master.py`

 * *Files identical despite different names*

### Comparing `zdt-2.1/zdt/hana_connector_utils.py` & `zdt-2.2/zdt/hana_connector_utils.py`

 * *Files identical despite different names*

### Comparing `zdt-2.1/zdt/log_func.py` & `zdt-2.2/zdt/log_func.py`

 * *Files identical despite different names*

### Comparing `zdt-2.1/zdt/random_utils.py` & `zdt-2.2/zdt/random_utils.py`

 * *Files identical despite different names*

### Comparing `zdt-2.1/zdt/time_func.py` & `zdt-2.2/zdt/time_func.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,41 @@
 import pytz
 
 def astimezone_sg(row):
     return row.astimezone(pytz.timezone('Singapore'))
 
 def get_year_start(date, delta= 0):
 
+    '''Takes in a datetime object and returns datetime object'''
+
     year = date.year - delta
 
     return dt.datetime(year,1,1).date()
 
 def get_month_start(date, delta= 0):
 
+    '''Takes in a datetime object and returns datetime object'''
+
     month = (date - relativedelta(months=delta)).month
     
     year = (date - relativedelta(months=delta)).year
 
     #if month <= 0:
     #    month = month + 12
 
     return dt.datetime(year,month,1).date()
 
+def get_day_start(date, delta= 0):
+
+    '''Takes in a datetime object and returns datetime object'''
+
+    days_date = (date-dt.timedelta(days=delta))
+
+    return days_date.date()
+
 def get_month_end_date(date1: dt):
 
     '''This functions takes in any date and returns the month end date'''
 
     month = date1.month
     next_month = month+1
     if next_month >12:
@@ -309,14 +321,20 @@
 
     if delta_unit =='months_whole':
 
         start_date = get_month_start(dt.datetime.now(), delta)
 
         period_start, period_end = [start_date.strftime('%Y%m%d')], [end_date.strftime('%Y%m%d')]
 
+    if delta_unit =='days_whole':
+
+        start_date = get_day_start(dt.datetime.now(), delta)
+
+        period_start, period_end = [start_date.strftime('%Y%m%d')], [end_date.strftime('%Y%m%d')]
+
     return period_start, period_end
 
 def get_time_hh_mm_ss(sec):
     # create timedelta and convert it into string
 
     dt_str = str(dt.timedelta(seconds=sec))
```

