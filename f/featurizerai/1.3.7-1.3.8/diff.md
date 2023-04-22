# Comparing `tmp/featurizerai-1.3.7.tar.gz` & `tmp/featurizerai-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.3.7.tar", last modified: Sat Apr 22 16:33:03 2023, max compression
+gzip compressed data, was "featurizerai-1.3.8.tar", last modified: Sat Apr 22 16:54:30 2023, max compression
```

## Comparing `featurizerai-1.3.7.tar` & `featurizerai-1.3.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:33:03.057821 featurizerai-1.3.7/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.3.7/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.3.7/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 16:33:03.057886 featurizerai-1.3.7/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.3.7/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 16:33:03.058091 featurizerai-1.3.7/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 16:32:32.000000 featurizerai-1.3.7/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:33:03.055083 featurizerai-1.3.7/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:33:03.056233 featurizerai-1.3.7/src/featurizerai/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.3.7/src/featurizerai/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:33:03.057409 featurizerai-1.3.7/src/featurizerai/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     5285 2023-04-22 16:31:46.000000 featurizerai-1.3.7/src/featurizerai/features/FeatureStore.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.3.7/src/featurizerai/features/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:33:03.056873 featurizerai-1.3.7/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 16:33:03.000000 featurizerai-1.3.7/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      425 2023-04-22 16:33:03.000000 featurizerai-1.3.7/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 16:33:03.000000 featurizerai-1.3.7/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 16:33:03.000000 featurizerai-1.3.7/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 16:33:03.000000 featurizerai-1.3.7/src/featurizerai.egg-info/top_level.txt
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:33:03.057572 featurizerai-1.3.7/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      810 2023-04-22 16:32:43.000000 featurizerai-1.3.7/tests/test_module1.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:54:30.753827 featurizerai-1.3.8/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.3.8/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.3.8/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 16:54:30.753898 featurizerai-1.3.8/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.3.8/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 16:54:30.754109 featurizerai-1.3.8/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 16:35:20.000000 featurizerai-1.3.8/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:54:30.751459 featurizerai-1.3.8/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:54:30.752515 featurizerai-1.3.8/src/featurizerai/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.3.8/src/featurizerai/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:54:30.753413 featurizerai-1.3.8/src/featurizerai/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     5475 2023-04-22 16:54:14.000000 featurizerai-1.3.8/src/featurizerai/features/FeatureStore.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.3.8/src/featurizerai/features/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:54:30.753124 featurizerai-1.3.8/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 16:54:30.000000 featurizerai-1.3.8/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      425 2023-04-22 16:54:30.000000 featurizerai-1.3.8/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 16:54:30.000000 featurizerai-1.3.8/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 16:54:30.000000 featurizerai-1.3.8/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 16:54:30.000000 featurizerai-1.3.8/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:54:30.753579 featurizerai-1.3.8/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      810 2023-04-22 16:32:43.000000 featurizerai-1.3.8/tests/test_module1.py
```

### Comparing `featurizerai-1.3.7/LICENSE` & `featurizerai-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.3.7/PKG-INFO` & `featurizerai-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.3.7
+Version: 1.3.8
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.3.7/setup.py` & `featurizerai-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.3.7',
+    version='1.3.8',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakgloba/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.3.7/src/featurizerai/features/FeatureStore.py` & `featurizerai-1.3.8/src/featurizerai/features/FeatureStore.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import ast
 import logging
 from datetime import datetime, timedelta
 from pymongo import MongoClient
+from pyspark.sql import functions as F
 from pymongo.server_api import ServerApi
 from confluent_kafka import Consumer, KafkaError
-from pyspark.sql import SparkSession
+from pyspark.sql import SparkSession, Window
 from pyspark.sql.functions import count, col, window, from_json, current_timestamp
 from pyspark.sql.types import StringType, StructType, StructField, TimestampType, IntegerType
 import certifi
 import os
 
 class create_stream_source:
     def __init__(self, kafka_connection, mongo_connection=None, time_aggregation_params=None):
@@ -35,24 +36,24 @@
         document = change["fullDocument"]
         df = spark.createDataFrame([document], schema)
 
         start_time = datetime.strptime(aggregation_date, "%Y-%m-%d")
         end_time_1_day = start_time + timedelta(days=1)
         end_time_15_days = start_time + timedelta(days=15)
 
+        window_1_day = Window.partitionBy("deviceid").orderBy("timestamp").rangeBetween(0, 24 * 3600)
+        window_15_days = Window.partitionBy("deviceid").orderBy("timestamp").rangeBetween(0, 15 * 24 * 3600)
+
         aggregated_data = df \
-            .groupBy("deviceid") \
-            .agg(
-            count(df.email).over(window(df.timestamp, "1 day")).alias("email_count_1_day"),
-            count(df.name).over(window(df.timestamp, "1 day")).alias("name_count_1_day"),
-            count(df.email).over(window(df.timestamp, "15 days")).alias("email_count_15_days"),
-            count(df.name).over(window(df.timestamp, "15 days")).alias("name_count_15_days")
-        ) \
-            .withColumn("date", start_time.strftime("%Y-%m-%d")) \
-            .dropDuplicates()
+            .withColumn("email_count_1_day", F.count("email").over(window_1_day)) \
+            .withColumn("name_count_1_day", F.count("name").over(window_1_day)) \
+            .withColumn("email_count_15_days", F.count("email").over(window_15_days)) \
+            .withColumn("name_count_15_days", F.count("name").over(window_15_days)) \
+            .withColumn("date", F.lit(start_time.strftime("%Y-%m-%d"))) \
+            .dropDuplicates(["deviceid", "date"])
 
         aggregated_data_dict = aggregated_data.collect()[0].asDict()
         print(aggregated_data_dict)
         print(start_time, end_time_1_day, end_time_15_days)
 
         try:
             json_aggregated_data = json.dumps(aggregated_data_dict)
```

### Comparing `featurizerai-1.3.7/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.3.8/src/featurizerai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.3.7
+Version: 1.3.8
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.3.7/tests/test_module1.py` & `featurizerai-1.3.8/tests/test_module1.py`

 * *Files identical despite different names*

