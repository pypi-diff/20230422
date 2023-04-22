# Comparing `tmp/featurizerai-1.3.1.tar.gz` & `tmp/featurizerai-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.3.1.tar", last modified: Sat Apr 22 11:43:29 2023, max compression
+gzip compressed data, was "featurizerai-1.3.2.tar", last modified: Sat Apr 22 12:41:50 2023, max compression
```

## Comparing `featurizerai-1.3.1.tar` & `featurizerai-1.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 11:43:29.568484 featurizerai-1.3.1/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.3.1/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.3.1/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 11:43:29.568545 featurizerai-1.3.1/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.3.1/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 11:43:29.568740 featurizerai-1.3.1/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 11:41:18.000000 featurizerai-1.3.1/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 11:43:29.566068 featurizerai-1.3.1/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 11:43:29.567124 featurizerai-1.3.1/src/featurizerai/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.3.1/src/featurizerai/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 11:43:29.568155 featurizerai-1.3.1/src/featurizerai/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4539 2023-04-22 11:18:01.000000 featurizerai-1.3.1/src/featurizerai/features/FeatureStore.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.3.1/src/featurizerai/features/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 11:43:29.567728 featurizerai-1.3.1/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 11:43:29.000000 featurizerai-1.3.1/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      383 2023-04-22 11:43:29.000000 featurizerai-1.3.1/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 11:43:29.000000 featurizerai-1.3.1/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 11:43:29.000000 featurizerai-1.3.1/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 11:43:29.000000 featurizerai-1.3.1/src/featurizerai.egg-info/top_level.txt
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 11:43:29.568271 featurizerai-1.3.1/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      816 2023-04-22 11:41:13.000000 featurizerai-1.3.1/tests/test_module1.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:41:50.854220 featurizerai-1.3.2/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.3.2/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.3.2/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 12:41:50.854279 featurizerai-1.3.2/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.3.2/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 12:41:50.854484 featurizerai-1.3.2/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 12:38:24.000000 featurizerai-1.3.2/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:41:50.851987 featurizerai-1.3.2/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:41:50.853034 featurizerai-1.3.2/src/featurizerai/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.3.2/src/featurizerai/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:41:50.853940 featurizerai-1.3.2/src/featurizerai/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4834 2023-04-22 12:37:54.000000 featurizerai-1.3.2/src/featurizerai/features/FeatureStore.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.3.2/src/featurizerai/features/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:41:50.853632 featurizerai-1.3.2/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 12:41:50.000000 featurizerai-1.3.2/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      425 2023-04-22 12:41:50.000000 featurizerai-1.3.2/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 12:41:50.000000 featurizerai-1.3.2/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 12:41:50.000000 featurizerai-1.3.2/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 12:41:50.000000 featurizerai-1.3.2/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:41:50.854113 featurizerai-1.3.2/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      816 2023-04-22 12:38:09.000000 featurizerai-1.3.2/tests/test_module1.py
```

### Comparing `featurizerai-1.3.1/LICENSE` & `featurizerai-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.3.1/PKG-INFO` & `featurizerai-1.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.3.1/setup.py` & `featurizerai-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.3.1',
+    version='1.3.2',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakgloba/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.3.1/src/featurizerai/features/FeatureStore.py` & `featurizerai-1.3.2/src/featurizerai/features/FeatureStore.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,46 +5,54 @@
 from pymongo import MongoClient
 from pymongo.server_api import ServerApi
 from confluent_kafka import Consumer, KafkaError
 from pyspark.sql import SparkSession
 from pyspark.sql.functions import count, col, window, from_json, current_timestamp
 from pyspark.sql.types import StringType, StructType, StructField, TimestampType, IntegerType
 import certifi
+import os
 
 class create_stream_source:
     def __init__(self, kafka_connection, mongo_connection=None, time_aggregation_params=None):
         self.kafka_connection = kafka_connection
         self.mongo_connection = mongo_connection or {
             'uri': "mongodb+srv://admin:6lHqq9LqgwDlninK@cluster0.aqtcyq2.mongodb.net/?retryWrites=true&w=majority",
             'database': 'kafkastream',
             'rawcollection': 'rawdata',
             'collection': 'sparkaggregate'
         }
         self.time_aggregation_params = time_aggregation_params
 
+    os.environ['HADOOP_OPTS'] = f"{os.environ.get('HADOOP_OPTS', '')} -Djava.library.path=/Library/hadoop/lib/native"
+
     def is_epoch(self, timestamp):
         try:
             datetime.fromtimestamp(int(timestamp))
             return True
         except ValueError:
             return False
 
+    from pyspark.sql.functions import col
+
     def process_change_event(self, change, aggregated_data_collection, spark, schema):
         document = change["fullDocument"]
         df = spark.createDataFrame([document], schema)
         aggregated_data = df \
             .groupBy(
-                window("timestamp", "1 day"),
-                "deviceid"
-            ) \
+            window("timestamp", "1 day"),
+            "deviceid"
+        ) \
             .agg(
-                count("email").alias("email_count"),
-                count("name").alias("name_count")
-            )
+            count("email").alias("email_count"),
+            count("name").alias("name_count")
+        )
+        aggregated_data = aggregated_data.withColumn("window", col("window")["start"].cast("string"))
         aggregated_data_dict = aggregated_data.collect()[0].asDict()
+        print((aggregated_data_dict))
+
         try:
             json_aggregated_data = json.dumps(aggregated_data_dict)
         except Exception as e:
             logging.error("Error serializing aggregated data as JSON: %s", e)
             json_aggregated_data = None
         if json_aggregated_data is not None:
             aggregated_data_collection.update_one(
@@ -72,15 +80,15 @@
         mongo_db = mongo_client[self.mongo_connection['database']]
         raw_data_collection = mongo_db[self.mongo_connection['rawcollection']]
         aggregated_data_collection = mongo_db[self.mongo_connection['collection']]
 
         change_stream = raw_data_collection.watch(full_document='updateLookup')
 
         consumer = Consumer(self.kafka_connection)
-        kafka_topic = "fake-data"
+        kafka_topic = "fake-data_test2"
         consumer.subscribe([kafka_topic])
 
         while True:
             msg = consumer.poll(1.0)
 
             if msg is None:
                 continue
```

### Comparing `featurizerai-1.3.1/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.3.2/src/featurizerai.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.3.1/tests/test_module1.py` & `featurizerai-1.3.2/tests/test_module1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..src.featurizerai.features.FeatureStore import create_stream_source
+from ..src.featurizerai.features.featurestore import create_stream_source
 
 def main():
     kafka_connection = {
         "bootstrap.servers": "buraks-air.lan:9092",
         "group.id": "your-group-id",
         "auto.offset.reset": "earliest"
     }
```

