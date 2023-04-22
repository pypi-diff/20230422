# Comparing `tmp/zyf-1.1.tar.gz` & `tmp/zyf-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zyf-1.1.tar", last modified: Sat Apr 22 15:00:46 2023, max compression
+gzip compressed data, was "dist\zyf-1.2.tar", last modified: Sat Apr 22 15:13:45 2023, max compression
```

## Comparing `zyf-1.1.tar` & `zyf-1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 15:00:46.957243 zyf-1.1/
--rw-rw-rw-   0        0        0    18674 2023-04-22 15:00:46.955176 zyf-1.1/PKG-INFO
--rw-rw-rw-   0        0        0    14465 2021-05-09 10:26:34.000000 zyf-1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-22 15:00:46.957243 zyf-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1175 2023-04-22 14:45:46.000000 zyf-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 15:00:46.924846 zyf-1.1/zyf/
--rw-rw-rw-   0        0        0      164 2021-02-27 09:17:00.000000 zyf-1.1/zyf/__init__.py
--rw-rw-rw-   0        0        0     1020 2021-04-05 11:32:40.000000 zyf-1.1/zyf/color.py
-drwxrwxrwx   0        0        0        0 2023-04-22 15:00:46.934735 zyf-1.1/zyf/crawler/
--rw-rw-rw-   0        0        0       76 2021-05-09 08:27:19.000000 zyf-1.1/zyf/crawler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 15:00:46.944123 zyf-1.1/zyf/crawler/image/
--rw-rw-rw-   0        0        0        0 2021-08-13 03:37:59.000000 zyf-1.1/zyf/crawler/image/__init__.py
--rw-rw-rw-   0        0        0     9017 2021-05-09 09:23:02.000000 zyf-1.1/zyf/crawler/image/netbian.py
--rw-rw-rw-   0        0        0     7116 2021-05-09 09:52:45.000000 zyf-1.1/zyf/crawler/image/netnr.py
-drwxrwxrwx   0        0        0        0 2023-04-22 15:00:46.951522 zyf-1.1/zyf/crawler/policy/
--rw-rw-rw-   0        0        0        0 2021-08-13 03:37:49.000000 zyf-1.1/zyf/crawler/policy/__init__.py
--rw-rw-rw-   0        0        0    14184 2021-05-09 08:45:56.000000 zyf-1.1/zyf/crawler/policy/goverment_policy.py
--rw-rw-rw-   0        0        0    15910 2021-05-09 09:52:45.000000 zyf-1.1/zyf/crawler/policy/lexis_policy.py
--rw-rw-rw-   0        0        0    15557 2021-08-19 14:08:59.000000 zyf-1.1/zyf/crawler/policy/pkulaw_policy.py
-drwxrwxrwx   0        0        0        0 2023-04-22 15:00:46.953952 zyf-1.1/zyf/db/
--rw-rw-rw-   0        0        0     6442 2023-04-22 14:44:34.000000 zyf-1.1/zyf/db/__init__.py
--rw-rw-rw-   0        0        0     2610 2021-04-17 14:27:41.000000 zyf-1.1/zyf/file.py
--rw-rw-rw-   0        0        0     7702 2021-02-21 09:03:09.000000 zyf-1.1/zyf/settings.py
--rw-rw-rw-   0        0        0     8125 2021-04-15 09:30:58.000000 zyf-1.1/zyf/timer.py
--rw-rw-rw-   0        0        0      730 2021-02-27 09:09:03.000000 zyf-1.1/zyf/user_agent.py
-drwxrwxrwx   0        0        0        0 2023-04-22 15:00:46.932735 zyf-1.1/zyf.egg-info/
--rw-rw-rw-   0        0        0    18674 2023-04-22 15:00:46.000000 zyf-1.1/zyf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-04-22 15:00:46.000000 zyf-1.1/zyf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 15:00:46.000000 zyf-1.1/zyf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-22 15:00:46.000000 zyf-1.1/zyf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-22 15:00:46.000000 zyf-1.1/zyf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 15:13:45.750771 zyf-1.2/
+-rw-rw-rw-   0        0        0    18674 2023-04-22 15:13:45.749770 zyf-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14465 2021-05-09 10:26:34.000000 zyf-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-22 15:13:45.750771 zyf-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1175 2023-04-22 15:13:22.000000 zyf-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 15:13:45.720514 zyf-1.2/zyf/
+-rw-rw-rw-   0        0        0      164 2021-02-27 09:17:00.000000 zyf-1.2/zyf/__init__.py
+-rw-rw-rw-   0        0        0     1020 2021-04-05 11:32:40.000000 zyf-1.2/zyf/color.py
+drwxrwxrwx   0        0        0        0 2023-04-22 15:13:45.735016 zyf-1.2/zyf/crawler/
+-rw-rw-rw-   0        0        0       76 2021-05-09 08:27:19.000000 zyf-1.2/zyf/crawler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 15:13:45.739018 zyf-1.2/zyf/crawler/image/
+-rw-rw-rw-   0        0        0        0 2021-08-13 03:37:59.000000 zyf-1.2/zyf/crawler/image/__init__.py
+-rw-rw-rw-   0        0        0     9017 2021-05-09 09:23:02.000000 zyf-1.2/zyf/crawler/image/netbian.py
+-rw-rw-rw-   0        0        0     7116 2021-05-09 09:52:45.000000 zyf-1.2/zyf/crawler/image/netnr.py
+drwxrwxrwx   0        0        0        0 2023-04-22 15:13:45.746312 zyf-1.2/zyf/crawler/policy/
+-rw-rw-rw-   0        0        0        0 2021-08-13 03:37:49.000000 zyf-1.2/zyf/crawler/policy/__init__.py
+-rw-rw-rw-   0        0        0    14184 2021-05-09 08:45:56.000000 zyf-1.2/zyf/crawler/policy/goverment_policy.py
+-rw-rw-rw-   0        0        0    15910 2021-05-09 09:52:45.000000 zyf-1.2/zyf/crawler/policy/lexis_policy.py
+-rw-rw-rw-   0        0        0    15557 2021-08-19 14:08:59.000000 zyf-1.2/zyf/crawler/policy/pkulaw_policy.py
+drwxrwxrwx   0        0        0        0 2023-04-22 15:13:45.747769 zyf-1.2/zyf/db/
+-rw-rw-rw-   0        0        0     6581 2023-04-22 15:11:17.000000 zyf-1.2/zyf/db/__init__.py
+-rw-rw-rw-   0        0        0     2610 2021-04-17 14:27:41.000000 zyf-1.2/zyf/file.py
+-rw-rw-rw-   0        0        0     7702 2021-02-21 09:03:09.000000 zyf-1.2/zyf/settings.py
+-rw-rw-rw-   0        0        0     8125 2021-04-15 09:30:58.000000 zyf-1.2/zyf/timer.py
+-rw-rw-rw-   0        0        0      730 2021-02-27 09:09:03.000000 zyf-1.2/zyf/user_agent.py
+drwxrwxrwx   0        0        0        0 2023-04-22 15:13:45.733016 zyf-1.2/zyf.egg-info/
+-rw-rw-rw-   0        0        0    18674 2023-04-22 15:13:45.000000 zyf-1.2/zyf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-04-22 15:13:45.000000 zyf-1.2/zyf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 15:13:45.000000 zyf-1.2/zyf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-22 15:13:45.000000 zyf-1.2/zyf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-22 15:13:45.000000 zyf-1.2/zyf.egg-info/top_level.txt
```

### Comparing `zyf-1.1/PKG-INFO` & `zyf-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyf
-Version: 1.1
+Version: 1.2
 Summary: 常用函数工具包
 Home-page: UNKNOWN
 Author: zhangyafei
 Author-email: zhangyafeii@foxmail.com
 License: UNKNOWN
 Description: ## 安装
```

### Comparing `zyf-1.1/README.md` & `zyf-1.2/README.md`

 * *Files identical despite different names*

### Comparing `zyf-1.1/setup.py` & `zyf-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='zyf',  # 模块名称
-    version="1.1",  # 当前版本
+    version="1.2",  # 当前版本
     author="zhangyafei",  # 作者
     author_email="zhangyafeii@foxmail.com",  # 作者邮箱
     description="常用函数工具包",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     # url="https://github.com/zhangyafeii/timer",  # 模块github地址
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
```

### Comparing `zyf-1.1/zyf/color.py` & `zyf-1.2/zyf/color.py`

 * *Files identical despite different names*

### Comparing `zyf-1.1/zyf/crawler/image/netbian.py` & `zyf-1.2/zyf/crawler/image/netbian.py`

 * *Files identical despite different names*

### Comparing `zyf-1.1/zyf/crawler/image/netnr.py` & `zyf-1.2/zyf/crawler/image/netnr.py`

 * *Files identical despite different names*

### Comparing `zyf-1.1/zyf/crawler/policy/goverment_policy.py` & `zyf-1.2/zyf/crawler/policy/goverment_policy.py`

 * *Files identical despite different names*

### Comparing `zyf-1.1/zyf/crawler/policy/lexis_policy.py` & `zyf-1.2/zyf/crawler/policy/lexis_policy.py`

 * *Files identical despite different names*

### Comparing `zyf-1.1/zyf/crawler/policy/pkulaw_policy.py` & `zyf-1.2/zyf/crawler/policy/pkulaw_policy.py`

 * *Files identical despite different names*

### Comparing `zyf-1.1/zyf/db/__init__.py` & `zyf-1.2/zyf/db/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import json
 
 import pandas as pd
 from dbutils.pooled_db import PooledDB
 
 
 class DBPoolHelper(object):
-    def __init__(self, dbname, user=None, password=None, db_type='postgressql', host='localhost', port=5432, maxconnections=1000, charset='utf8'):
+    def __init__(self, dbname, user=None, password=None, db_type='postgressql', host='localhost', port=5432, maxconnections=1000,
+                 charset='utf8',  maxcached=50, maxusage=1000, **config):
         """
         # sqlite3
         # 连接数据库文件名，sqlite不支持加密，不使用用户名和密码
         import sqlite3
         config = {"datanase": "path/to/your/dbname.db"}
         pool = PooledDB(sqlite3, maxcached=50, maxconnections=1000, maxusage=1000, **config)
         # mysql
@@ -26,22 +27,23 @@
         # sqlserver
         import pymssql
         pool = PooledDB(creator=pymssql, host=host, port=port, user=user, password=password, database=database, charset="utf8")
         :param type:
         """
         if db_type == 'postgressql':
             import psycopg2
-            pool = PooledDB(creator=psycopg2, host=host, port=port, user=user, password=password, database=dbname)
+            pool = PooledDB(creator=psycopg2, host=host, port=port, user=user, password=password, database=dbname, **config)
         elif db_type == 'mysql':
             import pymysql
-            pool = PooledDB(creator=pymysql, maxconnections=max, host=host, user=user, passwd=password, database=dbname, port=port, charset=charset)  # 5为连接池里的最少连接数
+            pool = PooledDB(creator=pymysql, maxconnections=maxconnections, host=host, user=user, passwd=password,
+                            database=dbname, port=port, charset=charset, **config)  # 5为连接池里的最少连接数
         elif db_type == 'sqlite':
             import sqlite3
             config = {"database": dbname}
-            pool = PooledDB(creator=sqlite3, maxcached=50, maxconnections=1000, maxusage=1000, **config)
+            pool = PooledDB(creator=sqlite3, maxcached=maxcached, maxconnections=maxconnections, maxusage=maxusage, **config)
         else:
             raise Exception('请输入正确的数据库类型, db_type="postgresql" or db_type="mysql" or db_type="sqlite"')
         self.__conn = pool.connection()
         self.__cursor = self.__conn.cursor()
 
     def __connect_close(self):
         """关闭连接"""
```

### Comparing `zyf-1.1/zyf/file.py` & `zyf-1.2/zyf/file.py`

 * *Files identical despite different names*

### Comparing `zyf-1.1/zyf/settings.py` & `zyf-1.2/zyf/settings.py`

 * *Files identical despite different names*

### Comparing `zyf-1.1/zyf/timer.py` & `zyf-1.2/zyf/timer.py`

 * *Files identical despite different names*

### Comparing `zyf-1.1/zyf/user_agent.py` & `zyf-1.2/zyf/user_agent.py`

 * *Files identical despite different names*

### Comparing `zyf-1.1/zyf.egg-info/PKG-INFO` & `zyf-1.2/zyf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyf
-Version: 1.1
+Version: 1.2
 Summary: 常用函数工具包
 Home-page: UNKNOWN
 Author: zhangyafei
 Author-email: zhangyafeii@foxmail.com
 License: UNKNOWN
 Description: ## 安装
```

