# Comparing `tmp/featurizerai-1.3.3.tar.gz` & `tmp/featurizerai-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.3.3.tar", last modified: Sat Apr 22 12:55:14 2023, max compression
+gzip compressed data, was "featurizerai-1.3.4.tar", last modified: Sat Apr 22 13:02:30 2023, max compression
```

## Comparing `featurizerai-1.3.3.tar` & `featurizerai-1.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:55:14.557599 featurizerai-1.3.3/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.3.3/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.3.3/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 12:55:14.557665 featurizerai-1.3.3/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.3.3/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 12:55:14.557890 featurizerai-1.3.3/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 12:55:09.000000 featurizerai-1.3.3/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:55:14.555217 featurizerai-1.3.3/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:55:14.556261 featurizerai-1.3.3/src/featurizerai/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.3.3/src/featurizerai/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:55:14.557192 featurizerai-1.3.3/src/featurizerai/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     5054 2023-04-22 12:55:03.000000 featurizerai-1.3.3/src/featurizerai/features/FeatureStore.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.3.3/src/featurizerai/features/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:55:14.556876 featurizerai-1.3.3/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 12:55:14.000000 featurizerai-1.3.3/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      425 2023-04-22 12:55:14.000000 featurizerai-1.3.3/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 12:55:14.000000 featurizerai-1.3.3/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 12:55:14.000000 featurizerai-1.3.3/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 12:55:14.000000 featurizerai-1.3.3/src/featurizerai.egg-info/top_level.txt
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 12:55:14.557461 featurizerai-1.3.3/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      810 2023-04-22 12:43:54.000000 featurizerai-1.3.3/tests/test_module1.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:02:30.789128 featurizerai-1.3.4/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.3.4/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.3.4/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 13:02:30.789187 featurizerai-1.3.4/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.3.4/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 13:02:30.789394 featurizerai-1.3.4/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 12:59:02.000000 featurizerai-1.3.4/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:02:30.786861 featurizerai-1.3.4/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:02:30.787932 featurizerai-1.3.4/src/featurizerai/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.3.4/src/featurizerai/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:02:30.788842 featurizerai-1.3.4/src/featurizerai/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     5054 2023-04-22 13:02:20.000000 featurizerai-1.3.4/src/featurizerai/features/FeatureStore.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.3.4/src/featurizerai/features/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:02:30.788543 featurizerai-1.3.4/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 13:02:30.000000 featurizerai-1.3.4/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      425 2023-04-22 13:02:30.000000 featurizerai-1.3.4/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 13:02:30.000000 featurizerai-1.3.4/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 13:02:30.000000 featurizerai-1.3.4/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 13:02:30.000000 featurizerai-1.3.4/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 13:02:30.789018 featurizerai-1.3.4/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      810 2023-04-22 12:43:54.000000 featurizerai-1.3.4/tests/test_module1.py
```

### Comparing `featurizerai-1.3.3/LICENSE` & `featurizerai-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.3.3/PKG-INFO` & `featurizerai-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.3.3/setup.py` & `featurizerai-1.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.3.3',
+    version='1.3.4',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakgloba/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.3.3/src/featurizerai/features/FeatureStore.py` & `featurizerai-1.3.4/src/featurizerai/features/FeatureStore.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         document = change["fullDocument"]
         df = spark.createDataFrame([document], schema)
         start_time = datetime.strptime(aggregation_date, "%Y-%m-%d")
         end_time = start_time + timedelta(days=1)
         aggregated_data = df \
             .where((df.timestamp >= start_time) & (df.timestamp < end_time)) \
             .groupBy(
-            window("timestamp", "30 day"),
+            window(start_time, "30 days"),
             "deviceid"
         ) \
             .agg(
             count("email").alias("email_count"),
             count("name").alias("name_count")
         )
         aggregated_data = aggregated_data.withColumn("window", col("window")["start"].cast("string"))
```

### Comparing `featurizerai-1.3.3/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.3.4/src/featurizerai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.3.3/tests/test_module1.py` & `featurizerai-1.3.4/tests/test_module1.py`

 * *Files identical despite different names*

