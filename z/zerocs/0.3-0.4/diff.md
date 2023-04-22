# Comparing `tmp/zerocs-0.3.tar.gz` & `tmp/zerocs-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerocs-0.3.tar", last modified: Sat Apr 22 02:49:20 2023, max compression
+gzip compressed data, was "zerocs-0.4.tar", last modified: Sat Apr 22 02:59:59 2023, max compression
```

## Comparing `zerocs-0.3.tar` & `zerocs-0.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:49:20.006047 zerocs-0.3/
--rw-r--r--   0 yanping   (1000) yanping   (1000)    17736 2023-04-22 02:49:20.006047 zerocs-0.3/PKG-INFO
--rw-r--r--   0 yanping   (1000) yanping   (1000)       38 2023-04-22 02:49:20.006047 zerocs-0.3/setup.cfg
--rw-r--r--   0 yanping   (1000) yanping   (1000)      867 2023-04-22 02:48:50.000000 zerocs-0.3/setup.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:49:20.002047 zerocs-0.3/zerocs/
--rw-r--r--   0 yanping   (1000) yanping   (1000)     4778 2023-04-22 01:33:23.000000 zerocs-0.3/zerocs/__init__.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:49:20.006047 zerocs-0.3/zerocs/base/
--rw-r--r--   0 yanping   (1000) yanping   (1000)      134 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/base/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1845 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/base/_base.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     7208 2023-04-20 05:50:35.000000 zerocs-0.3/zerocs/base/_default_func.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      496 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/base/_function.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     2674 2023-04-19 11:33:05.000000 zerocs-0.3/zerocs/base/base_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      529 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/base/default_func_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      670 2023-04-19 11:33:05.000000 zerocs-0.3/zerocs/base/function_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:49:20.006047 zerocs-0.3/zerocs/fork/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       35 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/fork/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1994 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/fork/_func.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1115 2023-04-19 11:33:05.000000 zerocs-0.3/zerocs/fork/fork_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:49:20.006047 zerocs-0.3/zerocs/logger/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       41 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/logger/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1860 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/logger/_logger.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      392 2023-04-19 11:33:05.000000 zerocs-0.3/zerocs/logger/logger_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     7354 2023-04-20 03:18:43.000000 zerocs-0.3/zerocs/mate.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:49:20.006047 zerocs-0.3/zerocs/network/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       44 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/network/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      425 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/network/_network.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      508 2023-04-19 11:33:05.000000 zerocs-0.3/zerocs/network/network_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:49:20.006047 zerocs-0.3/zerocs/rabbitmq/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       47 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/rabbitmq/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1288 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/rabbitmq/_rabbitmq.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1293 2023-04-19 11:33:05.000000 zerocs-0.3/zerocs/rabbitmq/rabbitmq_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:49:20.006047 zerocs-0.3/zerocs/script/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       39 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/script/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1460 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/script/_queue.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      708 2023-04-19 11:33:05.000000 zerocs-0.3/zerocs/script/queue_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:49:20.006047 zerocs-0.3/zerocs/snowflakeId/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       55 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/snowflakeId/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1918 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/snowflakeId/_snowflakeId.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      469 2023-04-19 11:33:05.000000 zerocs-0.3/zerocs/snowflakeId/snowflakeId.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:49:20.006047 zerocs-0.3/zerocs/sqlite/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       42 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/sqlite/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     5529 2023-04-20 04:53:25.000000 zerocs-0.3/zerocs/sqlite/_sqlite.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     3577 2023-04-20 03:18:43.000000 zerocs-0.3/zerocs/sqlite/sqlite3_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     8662 2023-04-20 05:52:13.000000 zerocs-0.3/zerocs/zerocs_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:49:20.006047 zerocs-0.3/zerocs.egg-info/
--rw-r--r--   0 yanping   (1000) yanping   (1000)    17736 2023-04-22 02:49:19.000000 zerocs-0.3/zerocs.egg-info/PKG-INFO
--rw-r--r--   0 yanping   (1000) yanping   (1000)      943 2023-04-22 02:49:19.000000 zerocs-0.3/zerocs.egg-info/SOURCES.txt
--rw-r--r--   0 yanping   (1000) yanping   (1000)        1 2023-04-22 02:49:19.000000 zerocs-0.3/zerocs.egg-info/dependency_links.txt
--rw-r--r--   0 yanping   (1000) yanping   (1000)       12 2023-04-22 02:49:19.000000 zerocs-0.3/zerocs.egg-info/requires.txt
--rw-r--r--   0 yanping   (1000) yanping   (1000)        7 2023-04-22 02:49:19.000000 zerocs-0.3/zerocs.egg-info/top_level.txt
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:59:59.243586 zerocs-0.4/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)    17736 2023-04-22 02:59:59.243586 zerocs-0.4/PKG-INFO
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       38 2023-04-22 02:59:59.243586 zerocs-0.4/setup.cfg
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      867 2023-04-22 02:59:58.000000 zerocs-0.4/setup.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:59:59.239586 zerocs-0.4/zerocs/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     4785 2023-04-22 02:58:49.000000 zerocs-0.4/zerocs/__init__.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:59:59.243586 zerocs-0.4/zerocs/base/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      134 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/base/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1845 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/base/_base.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     7208 2023-04-20 05:50:35.000000 zerocs-0.4/zerocs/base/_default_func.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      496 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/base/_function.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     2674 2023-04-19 11:33:05.000000 zerocs-0.4/zerocs/base/base_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      529 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/base/default_func_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      670 2023-04-19 11:33:05.000000 zerocs-0.4/zerocs/base/function_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:59:59.243586 zerocs-0.4/zerocs/fork/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       35 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/fork/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1994 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/fork/_func.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1115 2023-04-19 11:33:05.000000 zerocs-0.4/zerocs/fork/fork_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:59:59.243586 zerocs-0.4/zerocs/logger/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       41 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/logger/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1860 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/logger/_logger.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      392 2023-04-19 11:33:05.000000 zerocs-0.4/zerocs/logger/logger_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     7354 2023-04-20 03:18:43.000000 zerocs-0.4/zerocs/mate.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:59:59.243586 zerocs-0.4/zerocs/network/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       44 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/network/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      425 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/network/_network.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      508 2023-04-19 11:33:05.000000 zerocs-0.4/zerocs/network/network_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:59:59.243586 zerocs-0.4/zerocs/rabbitmq/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       47 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/rabbitmq/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1288 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/rabbitmq/_rabbitmq.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1293 2023-04-19 11:33:05.000000 zerocs-0.4/zerocs/rabbitmq/rabbitmq_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:59:59.243586 zerocs-0.4/zerocs/script/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       39 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/script/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1460 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/script/_queue.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      708 2023-04-19 11:33:05.000000 zerocs-0.4/zerocs/script/queue_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:59:59.243586 zerocs-0.4/zerocs/snowflakeId/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       55 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/snowflakeId/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1918 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/snowflakeId/_snowflakeId.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      469 2023-04-19 11:33:05.000000 zerocs-0.4/zerocs/snowflakeId/snowflakeId.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:59:59.243586 zerocs-0.4/zerocs/sqlite/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       42 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/sqlite/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     5529 2023-04-20 04:53:25.000000 zerocs-0.4/zerocs/sqlite/_sqlite.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     3577 2023-04-20 03:18:43.000000 zerocs-0.4/zerocs/sqlite/sqlite3_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     8662 2023-04-20 05:52:13.000000 zerocs-0.4/zerocs/zerocs_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-22 02:59:59.239586 zerocs-0.4/zerocs.egg-info/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)    17736 2023-04-22 02:59:59.000000 zerocs-0.4/zerocs.egg-info/PKG-INFO
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      943 2023-04-22 02:59:59.000000 zerocs-0.4/zerocs.egg-info/SOURCES.txt
+-rw-r--r--   0 yanping   (1000) yanping   (1000)        1 2023-04-22 02:59:59.000000 zerocs-0.4/zerocs.egg-info/dependency_links.txt
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       12 2023-04-22 02:59:59.000000 zerocs-0.4/zerocs.egg-info/requires.txt
+-rw-r--r--   0 yanping   (1000) yanping   (1000)        7 2023-04-22 02:59:59.000000 zerocs-0.4/zerocs.egg-info/top_level.txt
```

### Comparing `zerocs-0.3/PKG-INFO` & `zerocs-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocs
-Version: 0.3
+Version: 0.4
 Summary: zerocs
 Home-page: https://github.com/ZYPGITA/zerocs
 Author: YanPing
 Author-email: zyphhxx@foxmail.com
 Maintainer: YanPing
 Maintainer-email: zyphhxx@foxmail.com
 License: MIT License
```

### Comparing `zerocs-0.3/zerocs/__init__.py` & `zerocs-0.4/zerocs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             The software will not be used on any platform in violation of Chinese laws and regulations.
 """
 import eventlet
 
 eventlet.monkey_patch()
 
 import os
-from zerocs_ import MetaClass
+from zerocs.zerocs_ import MetaClass
 
 
 class _Service(MetaClass):
 
     def __init__(self, **kwargs):
         """
         Initialize zerocs service
```

### Comparing `zerocs-0.3/zerocs/base/_base.py` & `zerocs-0.4/zerocs/base/_base.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/base/_default_func.py` & `zerocs-0.4/zerocs/base/_default_func.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/base/base_.py` & `zerocs-0.4/zerocs/base/base_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/base/default_func_.py` & `zerocs-0.4/zerocs/base/default_func_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/base/function_.py` & `zerocs-0.4/zerocs/base/function_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/fork/_func.py` & `zerocs-0.4/zerocs/fork/_func.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/fork/fork_.py` & `zerocs-0.4/zerocs/fork/fork_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/logger/_logger.py` & `zerocs-0.4/zerocs/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/mate.py` & `zerocs-0.4/zerocs/mate.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/rabbitmq/_rabbitmq.py` & `zerocs-0.4/zerocs/rabbitmq/_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/rabbitmq/rabbitmq_.py` & `zerocs-0.4/zerocs/rabbitmq/rabbitmq_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/script/_queue.py` & `zerocs-0.4/zerocs/script/_queue.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/script/queue_.py` & `zerocs-0.4/zerocs/script/queue_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/snowflakeId/_snowflakeId.py` & `zerocs-0.4/zerocs/snowflakeId/_snowflakeId.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/sqlite/_sqlite.py` & `zerocs-0.4/zerocs/sqlite/_sqlite.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/sqlite/sqlite3_.py` & `zerocs-0.4/zerocs/sqlite/sqlite3_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs/zerocs_.py` & `zerocs-0.4/zerocs/zerocs_.py`

 * *Files identical despite different names*

### Comparing `zerocs-0.3/zerocs.egg-info/PKG-INFO` & `zerocs-0.4/zerocs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocs
-Version: 0.3
+Version: 0.4
 Summary: zerocs
 Home-page: https://github.com/ZYPGITA/zerocs
 Author: YanPing
 Author-email: zyphhxx@foxmail.com
 Maintainer: YanPing
 Maintainer-email: zyphhxx@foxmail.com
 License: MIT License
```

### Comparing `zerocs-0.3/zerocs.egg-info/SOURCES.txt` & `zerocs-0.4/zerocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

