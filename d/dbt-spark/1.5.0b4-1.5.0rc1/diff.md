# Comparing `tmp/dbt-spark-1.5.0b4.tar.gz` & `tmp/dbt-spark-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-spark-1.5.0b4.tar", last modified: Thu Mar 30 20:53:56 2023, max compression
+gzip compressed data, was "dbt-spark-1.5.0rc1.tar", last modified: Sat Apr 22 13:25:25 2023, max compression
```

## Comparing `dbt-spark-1.5.0b4.tar` & `dbt-spark-1.5.0rc1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:53:56.990090 dbt-spark-1.5.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-03-30 20:53:56.990090 dbt-spark-1.5.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:53:56.978089 dbt-spark-1.5.0b4/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:53:56.978089 dbt-spark-1.5.0b4/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:53:56.982089 dbt-spark-1.5.0b4/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    19924 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/adapters/spark/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/adapters/spark/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:53:56.978089 dbt-spark-1.5.0b4/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:53:56.982089 dbt-spark-1.5.0b4/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:53:56.982089 dbt-spark-1.5.0b4/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/apply_grants.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:53:56.986090 dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:53:56.986090 dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/incremental/validate.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:53:56.986090 dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:53:56.990090 dbt-spark-1.5.0b4/dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-03-30 20:53:56.000000 dbt-spark-1.5.0b4/dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-30 20:53:56.000000 dbt-spark-1.5.0b4/dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 20:53:56.000000 dbt-spark-1.5.0b4/dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 20:53:56.000000 dbt-spark-1.5.0b4/dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-30 20:53:56.000000 dbt-spark-1.5.0b4/dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-30 20:53:56.000000 dbt-spark-1.5.0b4/dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 20:53:56.990090 dbt-spark-1.5.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-03-30 20:53:42.000000 dbt-spark-1.5.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.038011 dbt-spark-1.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-22 13:25:25.038011 dbt-spark-1.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.030011 dbt-spark-1.5.0rc1/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.030011 dbt-spark-1.5.0rc1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.034011 dbt-spark-1.5.0rc1/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19924 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.030011 dbt-spark-1.5.0rc1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.034011 dbt-spark-1.5.0rc1/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.034011 dbt-spark-1.5.0rc1/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/apply_grants.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.034011 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.034011 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.038011 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.038011 dbt-spark-1.5.0rc1/dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-22 13:25:24.000000 dbt-spark-1.5.0rc1/dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-22 13:25:25.000000 dbt-spark-1.5.0rc1/dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 13:25:24.000000 dbt-spark-1.5.0rc1/dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 13:25:24.000000 dbt-spark-1.5.0rc1/dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-22 13:25:24.000000 dbt-spark-1.5.0rc1/dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-22 13:25:24.000000 dbt-spark-1.5.0rc1/dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 13:25:25.038011 dbt-spark-1.5.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/setup.py
```

### Comparing `dbt-spark-1.5.0b4/PKG-INFO` & `dbt-spark-1.5.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-spark
-Version: 1.5.0b4
+Version: 1.5.0rc1
 Summary: The Apache Spark adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-spark Version: 1.5.0b4 Summary: The Apache
+Metadata-Version: 2.1 Name: dbt-spark Version: 1.5.0rc1 Summary: The Apache
 Spark adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dbt-spark-1.5.0b4/README.md` & `dbt-spark-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/adapters/spark/__init__.py` & `dbt-spark-1.5.0rc1/dbt/adapters/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/adapters/spark/column.py` & `dbt-spark-1.5.0rc1/dbt/adapters/spark/column.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/adapters/spark/connections.py` & `dbt-spark-1.5.0rc1/dbt/adapters/spark/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/adapters/spark/impl.py` & `dbt-spark-1.5.0rc1/dbt/adapters/spark/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/adapters/spark/python_submissions.py` & `dbt-spark-1.5.0rc1/dbt/adapters/spark/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/adapters/spark/relation.py` & `dbt-spark-1.5.0rc1/dbt/adapters/spark/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/adapters/spark/session.py` & `dbt-spark-1.5.0rc1/dbt/adapters/spark/session.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/include/spark/macros/adapters.sql` & `dbt-spark-1.5.0rc1/dbt/include/spark/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/include/spark/macros/apply_grants.sql` & `dbt-spark-1.5.0rc1/dbt/include/spark/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/incremental/column_helpers.sql` & `dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/incremental/incremental.sql` & `dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/incremental/validate.sql` & `dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/seed.sql` & `dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/snapshot.sql` & `dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/include/spark/macros/materializations/table.sql` & `dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/table.sql`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,30 @@
                                                 type='table') -%}
 
   {{ run_hooks(pre_hooks) }}
 
   -- setup: if the target relation already exists, drop it
   -- in case if the existing and future table is delta or iceberg, we want to do a
   -- create or replace table instead of dropping, so we don't have the table unavailable
-  {% if old_relation and not (old_relation.is_delta and config.get('file_format', validator=validation.any[basestring]) == 'delta') -%}
-    {{ adapter.drop_relation(old_relation) }}
-  {%- endif %}
-
-  {% if old_relation and not (old_relation.is_iceberg and config.get('file_format', validator=validation.any[basestring]) == 'iceberg') -%}
-    {{ adapter.drop_relation(old_relation) }}
-  {%- endif %}
+  {% if old_relation is not none %}
+    {% set is_delta = (old_relation.is_delta and config.get('file_format', validator=validation.any[basestring]) == 'delta') %}
+    {% set is_iceberg = (old_relation.is_iceberg and config.get('file_format', validator=validation.any[basestring]) == 'iceberg') %}
+    {% set old_relation_type = old_relation.type %}
+  {% else %}
+    {% set is_delta = false %}
+    {% set is_iceberg = false %}
+    {% set old_relation_type = target_relation.type %}
+  {% endif %}
+
+  {% if not is_delta and not is_iceberg %}
+    {% set existing_relation = target_relation %}
+    {{ adapter.drop_relation(existing_relation.incorporate(type=old_relation_type)) }}
+  {% endif %}
 
   -- build model
-
   {%- call statement('main', language=language) -%}
     {{ create_table_as(False, target_relation, compiled_code, language) }}
   {%- endcall -%}
 
   {% set should_revoke = should_revoke(old_relation, full_refresh_mode=True) %}
   {% do apply_grants(target_relation, grant_config, should_revoke) %}
```

### Comparing `dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/dateadd.sql` & `dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/datediff.sql` & `dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/listagg.sql` & `dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/include/spark/macros/utils/split_part.sql` & `dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt/include/spark/profile_template.yml` & `dbt-spark-1.5.0rc1/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/dbt_spark.egg-info/PKG-INFO` & `dbt-spark-1.5.0rc1/dbt_spark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-spark
-Version: 1.5.0b4
+Version: 1.5.0rc1
 Summary: The Apache Spark adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-spark Version: 1.5.0b4 Summary: The Apache
+Metadata-Version: 2.1 Name: dbt-spark Version: 1.5.0rc1 Summary: The Apache
 Spark adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dbt-spark-1.5.0b4/dbt_spark.egg-info/SOURCES.txt` & `dbt-spark-1.5.0rc1/dbt_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0b4/setup.py` & `dbt-spark-1.5.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-spark"
-package_version = "1.5.0b4"
+package_version = "1.5.0rc1"
 dbt_core_version = _get_dbt_core_version()
 description = """The Apache Spark adapter plugin for dbt"""
 
 odbc_extras = ["pyodbc>=4.0.30"]
 pyhive_extras = [
     "PyHive[hive]>=0.6.0,<0.7.0",
     "thrift>=0.11.0,<0.17.0",
```

