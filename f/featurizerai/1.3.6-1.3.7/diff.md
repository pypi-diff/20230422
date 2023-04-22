# Comparing `tmp/featurizerai-1.3.6.tar.gz` & `tmp/featurizerai-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.3.6.tar", last modified: Sat Apr 22 13:10:03 2023, max compression
+gzip compressed data, was "featurizerai-1.3.7.tar", last modified: Sat Apr 22 16:33:03 2023, max compression
```

## Comparing `featurizerai-1.3.6.tar` & `featurizerai-1.3.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:10:03.799797 featurizerai-1.3.6/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.3.6/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.3.6/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 13:10:03.799856 featurizerai-1.3.6/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.3.6/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 13:10:03.800063 featurizerai-1.3.6/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 13:09:54.000000 featurizerai-1.3.6/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:10:03.797546 featurizerai-1.3.6/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:10:03.798609 featurizerai-1.3.6/src/featurizerai/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.3.6/src/featurizerai/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:10:03.799540 featurizerai-1.3.6/src/featurizerai/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     5087 2023-04-22 13:09:40.000000 featurizerai-1.3.6/src/featurizerai/features/FeatureStore.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.3.6/src/featurizerai/features/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:10:03.799223 featurizerai-1.3.6/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 13:10:03.000000 featurizerai-1.3.6/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      425 2023-04-22 13:10:03.000000 featurizerai-1.3.6/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 13:10:03.000000 featurizerai-1.3.6/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 13:10:03.000000 featurizerai-1.3.6/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 13:10:03.000000 featurizerai-1.3.6/src/featurizerai.egg-info/top_level.txt
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:10:03.799691 featurizerai-1.3.6/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      810 2023-04-22 12:43:54.000000 featurizerai-1.3.6/tests/test_module1.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:33:03.057821 featurizerai-1.3.7/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.3.7/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.3.7/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 16:33:03.057886 featurizerai-1.3.7/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.3.7/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 16:33:03.058091 featurizerai-1.3.7/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 16:32:32.000000 featurizerai-1.3.7/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:33:03.055083 featurizerai-1.3.7/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:33:03.056233 featurizerai-1.3.7/src/featurizerai/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.3.7/src/featurizerai/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:33:03.057409 featurizerai-1.3.7/src/featurizerai/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     5285 2023-04-22 16:31:46.000000 featurizerai-1.3.7/src/featurizerai/features/FeatureStore.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.3.7/src/featurizerai/features/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:33:03.056873 featurizerai-1.3.7/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 16:33:03.000000 featurizerai-1.3.7/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      425 2023-04-22 16:33:03.000000 featurizerai-1.3.7/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 16:33:03.000000 featurizerai-1.3.7/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 16:33:03.000000 featurizerai-1.3.7/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 16:33:03.000000 featurizerai-1.3.7/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:33:03.057572 featurizerai-1.3.7/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      810 2023-04-22 16:32:43.000000 featurizerai-1.3.7/tests/test_module1.py
```

### Comparing `featurizerai-1.3.6/LICENSE` & `featurizerai-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.3.6/PKG-INFO` & `featurizerai-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.3.6
+Version: 1.3.7
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.3.6/setup.py` & `featurizerai-1.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.3.6',
+    version='1.3.7',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakgloba/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.3.6/src/featurizerai/features/FeatureStore.py` & `featurizerai-1.3.7/src/featurizerai/features/FeatureStore.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,41 +27,46 @@
     def is_epoch(self, timestamp):
         try:
             datetime.fromtimestamp(int(timestamp))
             return True
         except ValueError:
             return False
 
-    def process_change_event(self, change, aggregated_data_collection, spark, schema, aggregation_date, lookback):
+    def process_change_event(self, change, aggregated_data_collection, spark, schema, aggregation_date):
         document = change["fullDocument"]
         df = spark.createDataFrame([document], schema)
+
         start_time = datetime.strptime(aggregation_date, "%Y-%m-%d")
-        end_time = start_time + timedelta(days=lookback)
+        end_time_1_day = start_time + timedelta(days=1)
+        end_time_15_days = start_time + timedelta(days=15)
+
         aggregated_data = df \
-            .where((df.timestamp < start_time) & (df.timestamp > end_time)) \
-            .groupBy(
-            window("timestamp", "1 day"),
-            "deviceid"
-        ) \
+            .groupBy("deviceid") \
             .agg(
-            count("email").alias("email_count"),
-            count("name").alias("name_count")
-        )
-        aggregated_data = aggregated_data.withColumn("window", col("window")["start"].cast("string"))
+            count(df.email).over(window(df.timestamp, "1 day")).alias("email_count_1_day"),
+            count(df.name).over(window(df.timestamp, "1 day")).alias("name_count_1_day"),
+            count(df.email).over(window(df.timestamp, "15 days")).alias("email_count_15_days"),
+            count(df.name).over(window(df.timestamp, "15 days")).alias("name_count_15_days")
+        ) \
+            .withColumn("date", start_time.strftime("%Y-%m-%d")) \
+            .dropDuplicates()
+
         aggregated_data_dict = aggregated_data.collect()[0].asDict()
-        print((aggregated_data_dict))
-        print(start_time, end_time)
+        print(aggregated_data_dict)
+        print(start_time, end_time_1_day, end_time_15_days)
+
         try:
             json_aggregated_data = json.dumps(aggregated_data_dict)
         except Exception as e:
             logging.error("Error serializing aggregated data as JSON: %s", e)
             json_aggregated_data = None
+
         if json_aggregated_data is not None:
             aggregated_data_collection.update_one(
-                {"window": aggregated_data_dict["window"], "deviceid": aggregated_data_dict["deviceid"]},
+                {"date": aggregated_data_dict["date"], "deviceid": aggregated_data_dict["deviceid"]},
                 {"$set": {"aggregated_data": json_aggregated_data}},
                 upsert=True
             )
         else:
             logging.error("Serialized aggregated data is None, skipping update")
 
     def run(self):
@@ -102,15 +107,15 @@
                         message_value["timestamp"] = datetime.fromtimestamp(int(message_value["timestamp"]))
                     else:
                         message_value["timestamp"] = datetime.now()
 
                     raw_data_collection.insert_one(message_value)
 
                 for change in change_stream:
-                    self.process_change_event(change, aggregated_data_collection, spark, schema, "2023-03-30", 30)
+                    self.process_change_event(change, aggregated_data_collection, spark, schema, "2023-03-30")
                     change_stream.close()
                     change_stream = raw_data_collection.watch(full_document='updateLookup')
 
 if __name__ == "__main__":
     kafka_conn = {
         "bootstrap.servers": "your-bootstrap-server",
         "group.id": "your-group-id",
```

### Comparing `featurizerai-1.3.6/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.3.7/src/featurizerai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.3.6
+Version: 1.3.7
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.3.6/tests/test_module1.py` & `featurizerai-1.3.7/tests/test_module1.py`

 * *Files identical despite different names*

