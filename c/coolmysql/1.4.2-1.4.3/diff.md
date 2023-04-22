# Comparing `tmp/coolmysql-1.4.2.tar.gz` & `tmp/coolmysql-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmysql-1.4.2.tar", last modified: Tue Apr 18 11:13:09 2023, max compression
+gzip compressed data, was "coolmysql-1.4.3.tar", last modified: Sat Apr 22 15:48:41 2023, max compression
```

## Comparing `coolmysql-1.4.2.tar` & `coolmysql-1.4.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.4.2/LICENSE
--rw-r--r--   0        0        0     4343 2023-04-16 20:01:06.306928 coolmysql-1.4.2/README.md
--rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.4.2/coolmysql.py
--rw-r--r--   0        0        0      566 2023-04-18 11:13:01.590911 coolmysql-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 coolmysql-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.4.3/LICENSE
+-rw-r--r--   0        0        0     4343 2023-04-16 20:01:06.306928 coolmysql-1.4.3/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.4.3/coolmysql.py
+-rw-r--r--   0        0        0      566 2023-04-22 15:48:30.912926 coolmysql-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 coolmysql-1.4.3/PKG-INFO
```

### Comparing `coolmysql-1.4.2/LICENSE` & `coolmysql-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmysql-1.4.2/README.md` & `coolmysql-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `coolmysql-1.4.2/pyproject.toml` & `coolmysql-1.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolmysql"
-version = "1.4.2"
+version = "1.4.3"
 description = "史上最优雅的 mysql ORM"
-dependencies = ["lccpy >=1.4.4"]
+dependencies = ["lccpy >=1.4.5"]
 keywords = ["coolmysql", "pymysql", "mysql"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `coolmysql-1.4.2/PKG-INFO` & `coolmysql-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: coolmysql
-Version: 1.4.2
+Version: 1.4.3
 Summary: 史上最优雅的 mysql ORM
 Keywords: coolmysql,pymysql,mysql
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.4
+Requires-Dist: lccpy >=1.4.5
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/coolmysql
 
 # 项目描述
 
 史上最优雅的 mysql ORM 。
 
 # 安装与教程
```

