# Comparing `tmp/featurizerai-1.3.9.tar.gz` & `tmp/featurizerai-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.3.9.tar", last modified: Sat Apr 22 16:57:57 2023, max compression
+gzip compressed data, was "featurizerai-1.4.0.tar", last modified: Sat Apr 22 17:01:16 2023, max compression
```

## Comparing `featurizerai-1.3.9.tar` & `featurizerai-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:57:57.247027 featurizerai-1.3.9/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.3.9/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.3.9/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 16:57:57.247094 featurizerai-1.3.9/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.3.9/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 16:57:57.247302 featurizerai-1.3.9/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 16:57:36.000000 featurizerai-1.3.9/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:57:57.244766 featurizerai-1.3.9/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:57:57.245823 featurizerai-1.3.9/src/featurizerai/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.3.9/src/featurizerai/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:57:57.246730 featurizerai-1.3.9/src/featurizerai/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     5565 2023-04-22 16:57:27.000000 featurizerai-1.3.9/src/featurizerai/features/FeatureStore.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.3.9/src/featurizerai/features/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:57:57.246425 featurizerai-1.3.9/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 16:57:57.000000 featurizerai-1.3.9/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      425 2023-04-22 16:57:57.000000 featurizerai-1.3.9/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 16:57:57.000000 featurizerai-1.3.9/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 16:57:57.000000 featurizerai-1.3.9/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 16:57:57.000000 featurizerai-1.3.9/src/featurizerai.egg-info/top_level.txt
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 16:57:57.246918 featurizerai-1.3.9/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      810 2023-04-22 16:32:43.000000 featurizerai-1.3.9/tests/test_module1.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:01:16.333853 featurizerai-1.4.0/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.4.0/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.4.0/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 17:01:16.333922 featurizerai-1.4.0/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.4.0/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 17:01:16.334134 featurizerai-1.4.0/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 16:59:53.000000 featurizerai-1.4.0/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:01:16.331590 featurizerai-1.4.0/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:01:16.332639 featurizerai-1.4.0/src/featurizerai/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.4.0/src/featurizerai/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:01:16.333579 featurizerai-1.4.0/src/featurizerai/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     5672 2023-04-22 17:01:08.000000 featurizerai-1.4.0/src/featurizerai/features/FeatureStore.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.4.0/src/featurizerai/features/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:01:16.333263 featurizerai-1.4.0/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 17:01:16.000000 featurizerai-1.4.0/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      425 2023-04-22 17:01:16.000000 featurizerai-1.4.0/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 17:01:16.000000 featurizerai-1.4.0/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 17:01:16.000000 featurizerai-1.4.0/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 17:01:16.000000 featurizerai-1.4.0/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:01:16.333741 featurizerai-1.4.0/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      810 2023-04-22 16:32:43.000000 featurizerai-1.4.0/tests/test_module1.py
```

### Comparing `featurizerai-1.3.9/LICENSE` & `featurizerai-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.3.9/PKG-INFO` & `featurizerai-1.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.3.9
+Version: 1.4.0
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.3.9/setup.py` & `featurizerai-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.3.9',
+    version='1.4.0',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakgloba/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.3.9/src/featurizerai/features/FeatureStore.py` & `featurizerai-1.4.0/src/featurizerai/features/FeatureStore.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
             .withColumn("name_count_1_day", F.count("name").over(window_1_day)) \
             .withColumn("email_count_15_days", F.count("email").over(window_15_days)) \
             .withColumn("name_count_15_days", F.count("name").over(window_15_days)) \
             .withColumn("date", F.lit(start_time.strftime("%Y-%m-%d"))) \
             .dropDuplicates(["deviceid", "date"])
 
         aggregated_data_dict = aggregated_data.collect()[0].asDict()
+        aggregated_data_dict["timestamp"] = aggregated_data_dict["timestamp"].strftime("%Y-%m-%d %H:%M:%S")
         print(aggregated_data_dict)
         print(start_time, end_time_1_day, end_time_15_days)
 
         try:
             json_aggregated_data = json.dumps(aggregated_data_dict)
         except Exception as e:
             logging.error("Error serializing aggregated data as JSON: %s", e)
@@ -66,15 +67,14 @@
             aggregated_data_collection.update_one(
                 {"date": aggregated_data_dict["date"], "deviceid": aggregated_data_dict["deviceid"]},
                 {"$set": {"aggregated_data": json_aggregated_data}},
                 upsert=True
             )
         else:
             logging.error("Serialized aggregated data is None, skipping update")
-
     def run(self):
         schema = StructType([
             StructField("timestamp", TimestampType(), True),
             StructField("name", StringType(), True),
             StructField("email", StringType(), True),
             StructField("deviceid", IntegerType(), True)
         ])
```

### Comparing `featurizerai-1.3.9/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.4.0/src/featurizerai.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.3.9
+Version: 1.4.0
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.3.9/tests/test_module1.py` & `featurizerai-1.4.0/tests/test_module1.py`

 * *Files identical despite different names*

