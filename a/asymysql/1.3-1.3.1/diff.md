# Comparing `tmp/asymysql-1.3.tar.gz` & `tmp/asymysql-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asymysql-1.3.tar", last modified: Mon Apr 10 14:24:22 2023, max compression
+gzip compressed data, was "asymysql-1.3.1.tar", last modified: Sat Apr 22 15:49:31 2023, max compression
```

## Comparing `asymysql-1.3.tar` & `asymysql-1.3.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymysql-1.3/LICENSE
--rw-r--r--   0        0        0     4862 2023-04-09 11:16:24.511029 asymysql-1.3/README.md
--rw-r--r--   0        0        0       28 2023-04-10 03:48:57.281686 asymysql-1.3/asymysql.py
--rw-r--r--   0        0        0      562 2023-04-10 09:20:03.028976 asymysql-1.3/pyproject.toml
--rw-r--r--   0        0        0     5096 1970-01-01 00:00:00.000000 asymysql-1.3/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymysql-1.3.1/LICENSE
+-rw-r--r--   0        0        0     4815 2023-04-16 20:01:06.324279 asymysql-1.3.1/README.md
+-rw-r--r--   0        0        0       28 2023-04-10 03:48:57.281686 asymysql-1.3.1/asymysql.py
+-rw-r--r--   0        0        0      566 2023-04-22 15:49:10.106710 asymysql-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5052 1970-01-01 00:00:00.000000 asymysql-1.3.1/PKG-INFO
```

### Comparing `asymysql-1.3/LICENSE` & `asymysql-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asymysql-1.3/README.md` & `asymysql-1.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     return await connect(
         host = 'localhost',
         port = 3306,
         user = 'root',
         password = '123456789'
     )
 
-orm = await ORM(mkconn=mkconn)  # 账户ORM
+orm = await ORM(mkconn)  # 账户ORM
 db = orm['泉州市']  # 库ORM
 sheet = db['希望小学']  # 表ORM
 ```
 
 新增数据：
 
 ```python
@@ -110,31 +110,31 @@
 | **代码**               | **解释**                   |
 | ---------------------------- | -------------------------------- |
 | mc.年级.isin('初三', '高二') | 若字段值是传入值的成员，则符合   |
 | mc.年级.notin(10, 30, 45)    | 若字段值不是传入值的成员，则符合 |
 
 过滤器的集合运算：
 
-| **代码**                                                                  | **解释** |
-| ------------------------------------------------------------------------------- | -------------- |
-| [ mc.年龄>3 ][ mc.年龄<100 ]                                                    | 交集           |
-| [ (mc.年龄==30) \| (mc.年龄>30) \| (mc.年龄<30) \| (mc.年龄==None) ] | 并集           |
-| [ (mc.年龄>3) - (mc.年龄>100) ]                                                 | 差集           |
-| [ ~(mc.年龄>100) ]                                                              | 补集           |
+| **代码**                                                         | **解释** |
+| ---------------------------------------------------------------------- | -------------- |
+| [ mc.年龄>3 ][ mc.年龄<100 ]                                           | 交集           |
+| [ (mc.年龄<30) \| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集           |
+| [ (mc.年龄>3) - (mc.年龄>100) ]                                        | 差集           |
+| [ ~(mc.年龄>100) ]                                                     | 补集           |
 
 只返回姓名、年龄这2个字段：
 
 ```python
-await sheet[mc.年龄>11][mc.年龄<30]['姓名','年龄'][:]
+await sheet[mc.年级=='高一']['姓名','年龄'][:]
 ```
 
-优先按年龄降序，其次按姓名升序，排序后返回第2~4条数据：
+优先按年龄降序，其次按姓名升序，排序后返回第2\~4条数据：
 
 ```python
-await sheet[mc.年龄>12].order(年龄=False, 姓名=True)[2:4]
+await sheet[mc.年级=='高一'].order(年龄=False, 姓名=True)[2:4]
 ```
 
 执行原生SQL语句：
 
 ```python
 data, cursor = await sheet.execute('select 姓名 from 希望小学 limit 1')
 data
@@ -157,8 +157,8 @@
 
 # 支持作者1元
 
 asymysql 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
```

### Comparing `asymysql-1.3/pyproject.toml` & `asymysql-1.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "asymysql"
-version = "1.3"
+version = "1.3.1"
 description = "异步的 mysql ORM"
-dependencies = ["lccpy >=1.3"]
+dependencies = ["lccpy >=1.4.5"]
 keywords = ["asymysql", "aiomysql", "mysql", "pymysql"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `asymysql-1.3/PKG-INFO` & `asymysql-1.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: asymysql
-Version: 1.3
+Version: 1.3.1
 Summary: 异步的 mysql ORM
 Keywords: asymysql,aiomysql,mysql,pymysql
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.3
+Requires-Dist: lccpy >=1.4.5
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/asymysql
 
 # 项目描述
 
 异步的 mysql ORM 。
 
 # 安装与教程
@@ -50,15 +50,15 @@
     return await connect(
         host = 'localhost',
         port = 3306,
         user = 'root',
         password = '123456789'
     )
 
-orm = await ORM(mkconn=mkconn)  # 账户ORM
+orm = await ORM(mkconn)  # 账户ORM
 db = orm['泉州市']  # 库ORM
 sheet = db['希望小学']  # 表ORM
 ```
 
 新增数据：
 
 ```python
@@ -122,31 +122,31 @@
 | **代码**               | **解释**                   |
 | ---------------------------- | -------------------------------- |
 | mc.年级.isin('初三', '高二') | 若字段值是传入值的成员，则符合   |
 | mc.年级.notin(10, 30, 45)    | 若字段值不是传入值的成员，则符合 |
 
 过滤器的集合运算：
 
-| **代码**                                                                  | **解释** |
-| ------------------------------------------------------------------------------- | -------------- |
-| [ mc.年龄>3 ][ mc.年龄<100 ]                                                    | 交集           |
-| [ (mc.年龄==30) \| (mc.年龄>30) \| (mc.年龄<30) \| (mc.年龄==None) ] | 并集           |
-| [ (mc.年龄>3) - (mc.年龄>100) ]                                                 | 差集           |
-| [ ~(mc.年龄>100) ]                                                              | 补集           |
+| **代码**                                                         | **解释** |
+| ---------------------------------------------------------------------- | -------------- |
+| [ mc.年龄>3 ][ mc.年龄<100 ]                                           | 交集           |
+| [ (mc.年龄<30) \| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集           |
+| [ (mc.年龄>3) - (mc.年龄>100) ]                                        | 差集           |
+| [ ~(mc.年龄>100) ]                                                     | 补集           |
 
 只返回姓名、年龄这2个字段：
 
 ```python
-await sheet[mc.年龄>11][mc.年龄<30]['姓名','年龄'][:]
+await sheet[mc.年级=='高一']['姓名','年龄'][:]
 ```
 
-优先按年龄降序，其次按姓名升序，排序后返回第2~4条数据：
+优先按年龄降序，其次按姓名升序，排序后返回第2\~4条数据：
 
 ```python
-await sheet[mc.年龄>12].order(年龄=False, 姓名=True)[2:4]
+await sheet[mc.年级=='高一'].order(年龄=False, 姓名=True)[2:4]
 ```
 
 执行原生SQL语句：
 
 ```python
 data, cursor = await sheet.execute('select 姓名 from 希望小学 limit 1')
 data
@@ -170,7 +170,8 @@
 # 支持作者1元
 
 asymysql 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
 ![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+
```

