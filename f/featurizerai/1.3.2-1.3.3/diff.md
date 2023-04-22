# Comparing `tmp/featurizerai-1.3.2.tar.gz` & `tmp/featurizerai-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.3.2.tar", last modified: Sat Apr 22 12:41:50 2023, max compression
+gzip compressed data, was "featurizerai-1.3.3.tar", last modified: Sat Apr 22 12:55:14 2023, max compression
```

## Comparing `featurizerai-1.3.2.tar` & `featurizerai-1.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:41:50.854220 featurizerai-1.3.2/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.3.2/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.3.2/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 12:41:50.854279 featurizerai-1.3.2/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.3.2/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 12:41:50.854484 featurizerai-1.3.2/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 12:38:24.000000 featurizerai-1.3.2/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:41:50.851987 featurizerai-1.3.2/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:41:50.853034 featurizerai-1.3.2/src/featurizerai/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.3.2/src/featurizerai/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:41:50.853940 featurizerai-1.3.2/src/featurizerai/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4834 2023-04-22 12:37:54.000000 featurizerai-1.3.2/src/featurizerai/features/FeatureStore.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.3.2/src/featurizerai/features/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:41:50.853632 featurizerai-1.3.2/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 12:41:50.000000 featurizerai-1.3.2/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      425 2023-04-22 12:41:50.000000 featurizerai-1.3.2/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 12:41:50.000000 featurizerai-1.3.2/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 12:41:50.000000 featurizerai-1.3.2/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 12:41:50.000000 featurizerai-1.3.2/src/featurizerai.egg-info/top_level.txt
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:41:50.854113 featurizerai-1.3.2/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      816 2023-04-22 12:38:09.000000 featurizerai-1.3.2/tests/test_module1.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:55:14.557599 featurizerai-1.3.3/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.3.3/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.3.3/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 12:55:14.557665 featurizerai-1.3.3/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.3.3/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 12:55:14.557890 featurizerai-1.3.3/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 12:55:09.000000 featurizerai-1.3.3/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:55:14.555217 featurizerai-1.3.3/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:55:14.556261 featurizerai-1.3.3/src/featurizerai/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.3.3/src/featurizerai/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:55:14.557192 featurizerai-1.3.3/src/featurizerai/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     5054 2023-04-22 12:55:03.000000 featurizerai-1.3.3/src/featurizerai/features/FeatureStore.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.3.3/src/featurizerai/features/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:55:14.556876 featurizerai-1.3.3/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 12:55:14.000000 featurizerai-1.3.3/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      425 2023-04-22 12:55:14.000000 featurizerai-1.3.3/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 12:55:14.000000 featurizerai-1.3.3/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 12:55:14.000000 featurizerai-1.3.3/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 12:55:14.000000 featurizerai-1.3.3/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:55:14.557461 featurizerai-1.3.3/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      810 2023-04-22 12:43:54.000000 featurizerai-1.3.3/tests/test_module1.py
```

### Comparing `featurizerai-1.3.2/LICENSE` & `featurizerai-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.3.2/PKG-INFO` & `featurizerai-1.3.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.3.2/setup.py` & `featurizerai-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.3.2',
+    version='1.3.3',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakgloba/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.3.2/src/featurizerai/features/FeatureStore.py` & `featurizerai-1.3.3/src/featurizerai/features/FeatureStore.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import ast
 import logging
-from datetime import datetime
+from datetime import datetime, timedelta
 from pymongo import MongoClient
 from pymongo.server_api import ServerApi
 from confluent_kafka import Consumer, KafkaError
 from pyspark.sql import SparkSession
 from pyspark.sql.functions import count, col, window, from_json, current_timestamp
 from pyspark.sql.types import StringType, StructType, StructField, TimestampType, IntegerType
 import certifi
@@ -27,32 +27,33 @@
     def is_epoch(self, timestamp):
         try:
             datetime.fromtimestamp(int(timestamp))
             return True
         except ValueError:
             return False
 
-    from pyspark.sql.functions import col
-
-    def process_change_event(self, change, aggregated_data_collection, spark, schema):
+    def process_change_event(self, change, aggregated_data_collection, spark, schema, aggregation_date):
         document = change["fullDocument"]
         df = spark.createDataFrame([document], schema)
+        start_time = datetime.strptime(aggregation_date, "%Y-%m-%d")
+        end_time = start_time + timedelta(days=1)
         aggregated_data = df \
+            .where((df.timestamp >= start_time) & (df.timestamp < end_time)) \
             .groupBy(
-            window("timestamp", "1 day"),
+            window("timestamp", "30 day"),
             "deviceid"
         ) \
             .agg(
             count("email").alias("email_count"),
             count("name").alias("name_count")
         )
         aggregated_data = aggregated_data.withColumn("window", col("window")["start"].cast("string"))
         aggregated_data_dict = aggregated_data.collect()[0].asDict()
         print((aggregated_data_dict))
-
+        print(start_time, end_time)
         try:
             json_aggregated_data = json.dumps(aggregated_data_dict)
         except Exception as e:
             logging.error("Error serializing aggregated data as JSON: %s", e)
             json_aggregated_data = None
         if json_aggregated_data is not None:
             aggregated_data_collection.update_one(
```

### Comparing `featurizerai-1.3.2/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.3.3/src/featurizerai.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.3.2/tests/test_module1.py` & `featurizerai-1.3.3/tests/test_module1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..src.featurizerai.features.featurestore import create_stream_source
+from featurizerai.features.FeatureStore import create_stream_source
 
 def main():
     kafka_connection = {
         "bootstrap.servers": "buraks-air.lan:9092",
         "group.id": "your-group-id",
         "auto.offset.reset": "earliest"
     }
```

