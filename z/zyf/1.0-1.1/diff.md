# Comparing `tmp/zyf-1.0.tar.gz` & `tmp/zyf-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zyf-1.0.tar", last modified: Thu Aug 19 13:21:16 2021, max compression
+gzip compressed data, was "dist\zyf-1.1.tar", last modified: Sat Apr 22 15:00:46 2023, max compression
```

## Comparing `zyf-1.0.tar` & `zyf-1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2021-08-19 13:21:16.816918 zyf-1.0/
--rw-rw-rw-   0        0        0    18674 2021-08-19 13:21:16.814917 zyf-1.0/PKG-INFO
--rw-rw-rw-   0        0        0    14465 2021-05-09 10:26:34.000000 zyf-1.0/README.md
--rw-rw-rw-   0        0        0       42 2021-08-19 13:21:16.816918 zyf-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1175 2021-08-19 13:21:12.000000 zyf-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-08-19 13:21:16.787836 zyf-1.0/zyf/
--rw-rw-rw-   0        0        0      164 2021-02-27 09:17:00.000000 zyf-1.0/zyf/__init__.py
--rw-rw-rw-   0        0        0     1020 2021-04-05 11:32:40.000000 zyf-1.0/zyf/color.py
-drwxrwxrwx   0        0        0        0 2021-08-19 13:21:16.799272 zyf-1.0/zyf/crawler/
--rw-rw-rw-   0        0        0       76 2021-05-09 08:27:19.000000 zyf-1.0/zyf/crawler/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-19 13:21:16.804273 zyf-1.0/zyf/crawler/image/
--rw-rw-rw-   0        0        0        0 2021-08-13 03:37:59.000000 zyf-1.0/zyf/crawler/image/__init__.py
--rw-rw-rw-   0        0        0     9017 2021-05-09 09:23:02.000000 zyf-1.0/zyf/crawler/image/netbian.py
--rw-rw-rw-   0        0        0     7116 2021-05-09 09:52:45.000000 zyf-1.0/zyf/crawler/image/netnr.py
-drwxrwxrwx   0        0        0        0 2021-08-19 13:21:16.811917 zyf-1.0/zyf/crawler/policy/
--rw-rw-rw-   0        0        0        0 2021-08-13 03:37:49.000000 zyf-1.0/zyf/crawler/policy/__init__.py
--rw-rw-rw-   0        0        0    14184 2021-05-09 08:45:56.000000 zyf-1.0/zyf/crawler/policy/goverment_policy.py
--rw-rw-rw-   0        0        0    15910 2021-05-09 09:52:45.000000 zyf-1.0/zyf/crawler/policy/lexis_policy.py
--rw-rw-rw-   0        0        0    15530 2021-08-19 13:17:54.000000 zyf-1.0/zyf/crawler/policy/pkulaw_policy.py
-drwxrwxrwx   0        0        0        0 2021-08-19 13:21:16.813917 zyf-1.0/zyf/db/
--rw-rw-rw-   0        0        0     6384 2021-05-09 10:27:03.000000 zyf-1.0/zyf/db/__init__.py
--rw-rw-rw-   0        0        0     2610 2021-04-17 14:27:41.000000 zyf-1.0/zyf/file.py
--rw-rw-rw-   0        0        0     7702 2021-02-21 09:03:09.000000 zyf-1.0/zyf/settings.py
--rw-rw-rw-   0        0        0     8125 2021-04-15 09:30:58.000000 zyf-1.0/zyf/timer.py
--rw-rw-rw-   0        0        0      730 2021-02-27 09:09:03.000000 zyf-1.0/zyf/user_agent.py
-drwxrwxrwx   0        0        0        0 2021-08-19 13:21:16.796846 zyf-1.0/zyf.egg-info/
--rw-rw-rw-   0        0        0    18674 2021-08-19 13:21:16.000000 zyf-1.0/zyf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2021-08-19 13:21:16.000000 zyf-1.0/zyf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-19 13:21:16.000000 zyf-1.0/zyf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2021-08-19 13:21:16.000000 zyf-1.0/zyf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2021-08-19 13:21:16.000000 zyf-1.0/zyf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 15:00:46.957243 zyf-1.1/
+-rw-rw-rw-   0        0        0    18674 2023-04-22 15:00:46.955176 zyf-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14465 2021-05-09 10:26:34.000000 zyf-1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-22 15:00:46.957243 zyf-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1175 2023-04-22 14:45:46.000000 zyf-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 15:00:46.924846 zyf-1.1/zyf/
+-rw-rw-rw-   0        0        0      164 2021-02-27 09:17:00.000000 zyf-1.1/zyf/__init__.py
+-rw-rw-rw-   0        0        0     1020 2021-04-05 11:32:40.000000 zyf-1.1/zyf/color.py
+drwxrwxrwx   0        0        0        0 2023-04-22 15:00:46.934735 zyf-1.1/zyf/crawler/
+-rw-rw-rw-   0        0        0       76 2021-05-09 08:27:19.000000 zyf-1.1/zyf/crawler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 15:00:46.944123 zyf-1.1/zyf/crawler/image/
+-rw-rw-rw-   0        0        0        0 2021-08-13 03:37:59.000000 zyf-1.1/zyf/crawler/image/__init__.py
+-rw-rw-rw-   0        0        0     9017 2021-05-09 09:23:02.000000 zyf-1.1/zyf/crawler/image/netbian.py
+-rw-rw-rw-   0        0        0     7116 2021-05-09 09:52:45.000000 zyf-1.1/zyf/crawler/image/netnr.py
+drwxrwxrwx   0        0        0        0 2023-04-22 15:00:46.951522 zyf-1.1/zyf/crawler/policy/
+-rw-rw-rw-   0        0        0        0 2021-08-13 03:37:49.000000 zyf-1.1/zyf/crawler/policy/__init__.py
+-rw-rw-rw-   0        0        0    14184 2021-05-09 08:45:56.000000 zyf-1.1/zyf/crawler/policy/goverment_policy.py
+-rw-rw-rw-   0        0        0    15910 2021-05-09 09:52:45.000000 zyf-1.1/zyf/crawler/policy/lexis_policy.py
+-rw-rw-rw-   0        0        0    15557 2021-08-19 14:08:59.000000 zyf-1.1/zyf/crawler/policy/pkulaw_policy.py
+drwxrwxrwx   0        0        0        0 2023-04-22 15:00:46.953952 zyf-1.1/zyf/db/
+-rw-rw-rw-   0        0        0     6442 2023-04-22 14:44:34.000000 zyf-1.1/zyf/db/__init__.py
+-rw-rw-rw-   0        0        0     2610 2021-04-17 14:27:41.000000 zyf-1.1/zyf/file.py
+-rw-rw-rw-   0        0        0     7702 2021-02-21 09:03:09.000000 zyf-1.1/zyf/settings.py
+-rw-rw-rw-   0        0        0     8125 2021-04-15 09:30:58.000000 zyf-1.1/zyf/timer.py
+-rw-rw-rw-   0        0        0      730 2021-02-27 09:09:03.000000 zyf-1.1/zyf/user_agent.py
+drwxrwxrwx   0        0        0        0 2023-04-22 15:00:46.932735 zyf-1.1/zyf.egg-info/
+-rw-rw-rw-   0        0        0    18674 2023-04-22 15:00:46.000000 zyf-1.1/zyf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-04-22 15:00:46.000000 zyf-1.1/zyf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 15:00:46.000000 zyf-1.1/zyf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-22 15:00:46.000000 zyf-1.1/zyf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-22 15:00:46.000000 zyf-1.1/zyf.egg-info/top_level.txt
```

### Comparing `zyf-1.0/PKG-INFO` & `zyf-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyf
-Version: 1.0
+Version: 1.1
 Summary: 常用函数工具包
 Home-page: UNKNOWN
 Author: zhangyafei
 Author-email: zhangyafeii@foxmail.com
 License: UNKNOWN
 Description: ## 安装
```

### Comparing `zyf-1.0/README.md` & `zyf-1.1/README.md`

 * *Files identical despite different names*

### Comparing `zyf-1.0/setup.py` & `zyf-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='zyf',  # 模块名称
-    version="1.0",  # 当前版本
+    version="1.1",  # 当前版本
     author="zhangyafei",  # 作者
     author_email="zhangyafeii@foxmail.com",  # 作者邮箱
     description="常用函数工具包",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     # url="https://github.com/zhangyafeii/timer",  # 模块github地址
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
```

### Comparing `zyf-1.0/zyf/color.py` & `zyf-1.1/zyf/color.py`

 * *Files identical despite different names*

### Comparing `zyf-1.0/zyf/crawler/image/netbian.py` & `zyf-1.1/zyf/crawler/image/netbian.py`

 * *Files identical despite different names*

### Comparing `zyf-1.0/zyf/crawler/image/netnr.py` & `zyf-1.1/zyf/crawler/image/netnr.py`

 * *Files identical despite different names*

### Comparing `zyf-1.0/zyf/crawler/policy/goverment_policy.py` & `zyf-1.1/zyf/crawler/policy/goverment_policy.py`

 * *Files identical despite different names*

### Comparing `zyf-1.0/zyf/crawler/policy/lexis_policy.py` & `zyf-1.1/zyf/crawler/policy/lexis_policy.py`

 * *Files identical despite different names*

### Comparing `zyf-1.0/zyf/crawler/policy/pkulaw_policy.py` & `zyf-1.1/zyf/crawler/policy/pkulaw_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,17 +149,19 @@
                 if suffix and not file.endswith(suffix):
                     continue
                 yield os.path.join(base_path, file)
 
     def download_search_html(self):
         self.get_start_search_requests()
         request_sets = self.filter_requests()
-        if request_sets:
-            if not os.path.exists(self.html_dir):
-                os.makedirs(self.html_dir)
+        if not request_sets:
+            return 
+        if not os.path.exists(self.html_dir):
+            os.makedirs(self.html_dir)
+        
         is_download = False
         while len(request_sets) > 0:
             keyword, year, level, level_title, page_num = request_sets.pop()
             based64_request = self.search_query_based64_request[keyword]
             print(f'start download {keyword} {year} {level_title} 第{page_num}页...')
             self.download_search_pages(level=level, keyword=keyword, based64_request=based64_request, page_num=page_num,
                                        year=year)
```

### Comparing `zyf-1.0/zyf/db/__init__.py` & `zyf-1.1/zyf/db/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import json
 
 import pandas as pd
 from dbutils.pooled_db import PooledDB
 
 
 class DBPoolHelper(object):
-    def __init__(self, dbname, user=None, password=None, db_type='postgressql', host='localhost', port=5432):
+    def __init__(self, dbname, user=None, password=None, db_type='postgressql', host='localhost', port=5432, maxconnections=1000, charset='utf8'):
         """
         # sqlite3
         # 连接数据库文件名，sqlite不支持加密，不使用用户名和密码
         import sqlite3
         config = {"datanase": "path/to/your/dbname.db"}
         pool = PooledDB(sqlite3, maxcached=50, maxconnections=1000, maxusage=1000, **config)
         # mysql
@@ -29,20 +29,19 @@
         :param type:
         """
         if db_type == 'postgressql':
             import psycopg2
             pool = PooledDB(creator=psycopg2, host=host, port=port, user=user, password=password, database=dbname)
         elif db_type == 'mysql':
             import pymysql
-            pool = PooledDB(pymysql, 5, host='localhost', user='root', passwd='pwd', db='myDB',
-                            port=3306)  # 5为连接池里的最少连接数
+            pool = PooledDB(creator=pymysql, maxconnections=max, host=host, user=user, passwd=password, database=dbname, port=port, charset=charset)  # 5为连接池里的最少连接数
         elif db_type == 'sqlite':
             import sqlite3
             config = {"database": dbname}
-            pool = PooledDB(sqlite3, maxcached=50, maxconnections=1000, maxusage=1000, **config)
+            pool = PooledDB(creator=sqlite3, maxcached=50, maxconnections=1000, maxusage=1000, **config)
         else:
             raise Exception('请输入正确的数据库类型, db_type="postgresql" or db_type="mysql" or db_type="sqlite"')
         self.__conn = pool.connection()
         self.__cursor = self.__conn.cursor()
 
     def __connect_close(self):
         """关闭连接"""
```

### Comparing `zyf-1.0/zyf/file.py` & `zyf-1.1/zyf/file.py`

 * *Files identical despite different names*

### Comparing `zyf-1.0/zyf/settings.py` & `zyf-1.1/zyf/settings.py`

 * *Files identical despite different names*

### Comparing `zyf-1.0/zyf/timer.py` & `zyf-1.1/zyf/timer.py`

 * *Files identical despite different names*

### Comparing `zyf-1.0/zyf/user_agent.py` & `zyf-1.1/zyf/user_agent.py`

 * *Files identical despite different names*

### Comparing `zyf-1.0/zyf.egg-info/PKG-INFO` & `zyf-1.1/zyf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyf
-Version: 1.0
+Version: 1.1
 Summary: 常用函数工具包
 Home-page: UNKNOWN
 Author: zhangyafei
 Author-email: zhangyafeii@foxmail.com
 License: UNKNOWN
 Description: ## 安装
```

