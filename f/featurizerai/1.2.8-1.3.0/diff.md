# Comparing `tmp/featurizerai-1.2.8.tar.gz` & `tmp/featurizerai-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.2.8.tar", last modified: Sat Apr  8 16:21:20 2023, max compression
+gzip compressed data, was "dist/featurizerai-1.3.0.tar", last modified: Sat Apr 22 11:07:25 2023, max compression
```

## Comparing `featurizerai-1.2.8.tar` & `featurizerai-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,21 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:20.533523 featurizerai-1.2.8/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.2.8/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.2.8/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-08 16:21:20.533615 featurizerai-1.2.8/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.2.8/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-08 16:21:20.533849 featurizerai-1.2.8/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-08 16:21:17.000000 featurizerai-1.2.8/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:20.529840 featurizerai-1.2.8/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:20.531138 featurizerai-1.2.8/src/featurizerai/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.2.8/src/featurizerai/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:20.532457 featurizerai-1.2.8/src/featurizerai/datasource/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:04.000000 featurizerai-1.2.8/src/featurizerai/datasource/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      573 2023-03-30 14:51:50.000000 featurizerai-1.2.8/src/featurizerai/datasource/create_batch_source.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      858 2023-03-30 14:35:45.000000 featurizerai-1.2.8/src/featurizerai/datasource/create_parquet_sample_file.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:20.532943 featurizerai-1.2.8/src/featurizerai/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.2.8/src/featurizerai/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4539 2023-04-08 15:20:31.000000 featurizerai-1.2.8/src/featurizerai/features/featureview.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:20.531841 featurizerai-1.2.8/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-08 16:21:20.000000 featurizerai-1.2.8/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      531 2023-04-08 16:21:20.000000 featurizerai-1.2.8/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-08 16:21:20.000000 featurizerai-1.2.8/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-08 16:21:20.000000 featurizerai-1.2.8/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-08 16:21:20.000000 featurizerai-1.2.8/src/featurizerai.egg-info/top_level.txt
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:20.533268 featurizerai-1.2.8/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      815 2023-04-08 16:04:55.000000 featurizerai-1.2.8/tests/test_module1.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 11:07:25.003768 featurizerai-1.3.0/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.3.0/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.3.0/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 11:07:25.003852 featurizerai-1.3.0/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.3.0/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 11:07:25.004130 featurizerai-1.3.0/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 11:06:01.000000 featurizerai-1.3.0/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 11:07:25.001041 featurizerai-1.3.0/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 11:07:25.002227 featurizerai-1.3.0/src/featurizerai/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.3.0/src/featurizerai/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 11:07:25.003479 featurizerai-1.3.0/src/featurizerai/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.3.0/src/featurizerai/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4539 2023-04-08 15:20:31.000000 featurizerai-1.3.0/src/featurizerai/features/create_stream_source.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 11:07:25.003182 featurizerai-1.3.0/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 11:07:24.000000 featurizerai-1.3.0/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      391 2023-04-22 11:07:24.000000 featurizerai-1.3.0/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 11:07:24.000000 featurizerai-1.3.0/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 11:07:24.000000 featurizerai-1.3.0/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 11:07:24.000000 featurizerai-1.3.0/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 11:07:25.003629 featurizerai-1.3.0/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      824 2023-04-22 11:05:47.000000 featurizerai-1.3.0/tests/test_module1.py
```

### Comparing `featurizerai-1.2.8/LICENSE` & `featurizerai-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.2.8/PKG-INFO` & `featurizerai-1.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.2.8
+Version: 1.3.0
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.2.8/setup.py` & `featurizerai-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.2.8',
+    version='1.3.0',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakgloba/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.2.8/src/featurizerai/features/featureview.py` & `featurizerai-1.3.0/src/featurizerai/features/create_stream_source.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.2.8/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.3.0/src/featurizerai.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.2.8
+Version: 1.3.0
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.2.8/tests/test_module1.py` & `featurizerai-1.3.0/tests/test_module1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..src.featurizerai.features.featureview import create_stream_source
+from ..src.featurizerai.features.create_stream_source import create_stream_source
 
 def main():
     kafka_connection = {
         "bootstrap.servers": "buraks-air.lan:9092",
         "group.id": "your-group-id",
         "auto.offset.reset": "earliest"
     }
```

