# Comparing `tmp/featurizerai-1.3.5.tar.gz` & `tmp/featurizerai-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.3.5.tar", last modified: Sat Apr 22 13:07:20 2023, max compression
+gzip compressed data, was "featurizerai-1.3.6.tar", last modified: Sat Apr 22 13:10:03 2023, max compression
```

## Comparing `featurizerai-1.3.5.tar` & `featurizerai-1.3.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:07:20.875567 featurizerai-1.3.5/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.3.5/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.3.5/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 13:07:20.875636 featurizerai-1.3.5/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.3.5/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 13:07:20.875855 featurizerai-1.3.5/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 13:07:12.000000 featurizerai-1.3.5/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:07:20.873364 featurizerai-1.3.5/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:07:20.874402 featurizerai-1.3.5/src/featurizerai/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.3.5/src/featurizerai/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:07:20.875289 featurizerai-1.3.5/src/featurizerai/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     5089 2023-04-22 13:07:04.000000 featurizerai-1.3.5/src/featurizerai/features/FeatureStore.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.3.5/src/featurizerai/features/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:07:20.874995 featurizerai-1.3.5/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 13:07:20.000000 featurizerai-1.3.5/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      425 2023-04-22 13:07:20.000000 featurizerai-1.3.5/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 13:07:20.000000 featurizerai-1.3.5/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 13:07:20.000000 featurizerai-1.3.5/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 13:07:20.000000 featurizerai-1.3.5/src/featurizerai.egg-info/top_level.txt
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:07:20.875450 featurizerai-1.3.5/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      810 2023-04-22 12:43:54.000000 featurizerai-1.3.5/tests/test_module1.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:10:03.799797 featurizerai-1.3.6/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.3.6/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.3.6/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 13:10:03.799856 featurizerai-1.3.6/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.3.6/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 13:10:03.800063 featurizerai-1.3.6/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 13:09:54.000000 featurizerai-1.3.6/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:10:03.797546 featurizerai-1.3.6/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:10:03.798609 featurizerai-1.3.6/src/featurizerai/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.3.6/src/featurizerai/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:10:03.799540 featurizerai-1.3.6/src/featurizerai/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     5087 2023-04-22 13:09:40.000000 featurizerai-1.3.6/src/featurizerai/features/FeatureStore.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.3.6/src/featurizerai/features/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:10:03.799223 featurizerai-1.3.6/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 13:10:03.000000 featurizerai-1.3.6/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      425 2023-04-22 13:10:03.000000 featurizerai-1.3.6/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 13:10:03.000000 featurizerai-1.3.6/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 13:10:03.000000 featurizerai-1.3.6/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 13:10:03.000000 featurizerai-1.3.6/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:10:03.799691 featurizerai-1.3.6/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      810 2023-04-22 12:43:54.000000 featurizerai-1.3.6/tests/test_module1.py
```

### Comparing `featurizerai-1.3.5/LICENSE` & `featurizerai-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.3.5/PKG-INFO` & `featurizerai-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.3.5/setup.py` & `featurizerai-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.3.5',
+    version='1.3.6',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakgloba/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.3.5/src/featurizerai/features/FeatureStore.py` & `featurizerai-1.3.6/src/featurizerai/features/FeatureStore.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         document = change["fullDocument"]
         df = spark.createDataFrame([document], schema)
         start_time = datetime.strptime(aggregation_date, "%Y-%m-%d")
         end_time = start_time + timedelta(days=lookback)
         aggregated_data = df \
             .where((df.timestamp < start_time) & (df.timestamp > end_time)) \
             .groupBy(
-            window("timestamp", "30 days"),
+            window("timestamp", "1 day"),
             "deviceid"
         ) \
             .agg(
             count("email").alias("email_count"),
             count("name").alias("name_count")
         )
         aggregated_data = aggregated_data.withColumn("window", col("window")["start"].cast("string"))
```

### Comparing `featurizerai-1.3.5/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.3.6/src/featurizerai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.3.5/tests/test_module1.py` & `featurizerai-1.3.6/tests/test_module1.py`

 * *Files identical despite different names*

