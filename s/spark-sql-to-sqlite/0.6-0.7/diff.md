# Comparing `tmp/spark_sql_to_sqlite-0.6.tar.gz` & `tmp/spark_sql_to_sqlite-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_sql_to_sqlite-0.6.tar", last modified: Fri Apr 21 19:17:04 2023, max compression
+gzip compressed data, was "spark_sql_to_sqlite-0.7.tar", last modified: Sat Apr 22 00:00:17 2023, max compression
```

## Comparing `spark_sql_to_sqlite-0.6.tar` & `spark_sql_to_sqlite-0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 19:17:04.554319 spark_sql_to_sqlite-0.6/
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      939 2023-04-21 19:17:04.554110 spark_sql_to_sqlite-0.6/PKG-INFO
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      836 2023-04-21 19:16:45.000000 spark_sql_to_sqlite-0.6/README.md
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)       38 2023-04-21 19:17:04.554376 spark_sql_to_sqlite-0.6/setup.cfg
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      484 2023-04-21 19:16:58.000000 spark_sql_to_sqlite-0.6/setup.py
-drwxr-xr-x   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 19:17:04.552498 spark_sql_to_sqlite-0.6/spark_sql_to_sqlite/
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      839 2023-04-21 17:14:27.000000 spark_sql_to_sqlite-0.6/spark_sql_to_sqlite/__init__.py
-drwxr-xr-x   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 19:17:04.553829 spark_sql_to_sqlite-0.6/spark_sql_to_sqlite.egg-info/
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      939 2023-04-21 19:17:04.000000 spark_sql_to_sqlite-0.6/spark_sql_to_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      264 2023-04-21 19:17:04.000000 spark_sql_to_sqlite-0.6/spark_sql_to_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)        1 2023-04-21 19:17:04.000000 spark_sql_to_sqlite-0.6/spark_sql_to_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)       15 2023-04-21 19:17:04.000000 spark_sql_to_sqlite-0.6/spark_sql_to_sqlite.egg-info/requires.txt
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)       20 2023-04-21 19:17:04.000000 spark_sql_to_sqlite-0.6/spark_sql_to_sqlite.egg-info/top_level.txt
+drwxr-xr-x   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-22 00:00:17.531109 spark_sql_to_sqlite-0.7/
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)     1437 2023-04-22 00:00:17.530905 spark_sql_to_sqlite-0.7/PKG-INFO
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)     1334 2023-04-21 23:59:34.000000 spark_sql_to_sqlite-0.7/README.md
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)       38 2023-04-22 00:00:17.531160 spark_sql_to_sqlite-0.7/setup.cfg
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      484 2023-04-22 00:00:10.000000 spark_sql_to_sqlite-0.7/setup.py
+drwxr-xr-x   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-22 00:00:17.529254 spark_sql_to_sqlite-0.7/spark_sql_to_sqlite/
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      839 2023-04-21 17:14:27.000000 spark_sql_to_sqlite-0.7/spark_sql_to_sqlite/__init__.py
+drwxr-xr-x   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-22 00:00:17.530634 spark_sql_to_sqlite-0.7/spark_sql_to_sqlite.egg-info/
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)     1437 2023-04-22 00:00:17.000000 spark_sql_to_sqlite-0.7/spark_sql_to_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      264 2023-04-22 00:00:17.000000 spark_sql_to_sqlite-0.7/spark_sql_to_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)        1 2023-04-22 00:00:17.000000 spark_sql_to_sqlite-0.7/spark_sql_to_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)       15 2023-04-22 00:00:17.000000 spark_sql_to_sqlite-0.7/spark_sql_to_sqlite.egg-info/requires.txt
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)       20 2023-04-22 00:00:17.000000 spark_sql_to_sqlite-0.7/spark_sql_to_sqlite.egg-info/top_level.txt
```

### Comparing `spark_sql_to_sqlite-0.6/PKG-INFO` & `spark_sql_to_sqlite-0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-Metadata-Version: 2.1
-Name: spark_sql_to_sqlite
-Version: 0.6
-Description-Content-Type: text/markdown
-
 # spark_sql_to_sqlite
 
 Easily save a Spark dataframe into a SQLite database.
 
+#### Why do you need it
+
+Although you can use jdbc with Spark to write to SQLite, this method is error prone, and doesn't handle complex data types such as Map, Struct and Array.
+
+`spark_sql_to_sqlite` automatically converts these complex data types to json, which can be used in SQLite queries using standard [json functions](https://www.sqlite.org/json1.html) such as json_extract.
+
+It also has sensible defaults to create or replace the SQLite database and table(s) as needed.
+
+#### How To Use
+
 You can use this on Spark environments such as Databricks, where you have a `spark` variable available that represents the SparkContext.
 
 Install it as follows:
 
 ```
 %pip install spark-sql-to-sqlite
 ```
@@ -28,8 +33,8 @@
 ```
 
 Example:
 ```
 spark_sql_to_sqlite(spark, "SELECT * FROM hive_metastore.fire.bronze", "/tmp/fire.db", "bronze")
 ```
 
-The above command will create a SQLite database at `/tmp/fire.db` if it doesn't already exists. It will create or replace the `bronze` table in this database and overwrite it with the results of the Spark SQL query
+The above command will create a SQLite database at `/tmp/fire.db` if it doesn't already exists. It will create or replace the `bronze` table in this database and overwrite it with the results of the Spark SQL query
```

### Comparing `spark_sql_to_sqlite-0.6/spark_sql_to_sqlite/__init__.py` & `spark_sql_to_sqlite-0.7/spark_sql_to_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_sql_to_sqlite-0.6/spark_sql_to_sqlite.egg-info/PKG-INFO` & `spark_sql_to_sqlite-0.7/spark_sql_to_sqlite.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 Metadata-Version: 2.1
 Name: spark-sql-to-sqlite
-Version: 0.6
+Version: 0.7
 Description-Content-Type: text/markdown
 
 # spark_sql_to_sqlite
 
 Easily save a Spark dataframe into a SQLite database.
 
+#### Why do you need it
+
+Although you can use jdbc with Spark to write to SQLite, this method is error prone, and doesn't handle complex data types such as Map, Struct and Array.
+
+`spark_sql_to_sqlite` automatically converts these complex data types to json, which can be used in SQLite queries using standard [json functions](https://www.sqlite.org/json1.html) such as json_extract.
+
+It also has sensible defaults to create or replace the SQLite database and table(s) as needed.
+
+#### How To Use
+
 You can use this on Spark environments such as Databricks, where you have a `spark` variable available that represents the SparkContext.
 
 Install it as follows:
 
 ```
 %pip install spark-sql-to-sqlite
 ```
```

