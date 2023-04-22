# Comparing `tmp/aliendev_api-0.1.7.tar.gz` & `tmp/aliendev_api-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliendev_api-0.1.7.tar", max compression
+gzip compressed data, was "aliendev_api-0.1.8.tar", max compression
```

## Comparing `aliendev_api-0.1.7.tar` & `aliendev_api-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0        0 2023-04-22 08:44:09.528123 aliendev_api-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-04-22 08:44:09.528123 aliendev_api-0.1.7/aliendev_api/__init__.py
--rw-r--r--   0        0        0      824 2023-04-22 08:44:09.528123 aliendev_api-0.1.7/aliendev_api/config/__pycache__/mongo.cpython-311.pyc
--rw-r--r--   0        0        0      479 2023-04-22 08:44:09.528123 aliendev_api-0.1.7/aliendev_api/config/mongo.py
--rw-r--r--   0        0        0     2898 2023-04-22 08:44:09.528123 aliendev_api-0.1.7/aliendev_api/main.py
--rw-r--r--   0        0        0      377 2023-04-22 08:44:33.432344 aliendev_api-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 aliendev_api-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-22 18:56:26.767149 aliendev_api-0.1.8/README.md
+-rw-r--r--   0        0        0      824 2023-04-22 18:56:26.767149 aliendev_api-0.1.8/aliendev_api/config/__pycache__/mongo.cpython-311.pyc
+-rw-r--r--   0        0        0      479 2023-04-22 18:56:26.767149 aliendev_api-0.1.8/aliendev_api/config/mongo.py
+-rw-r--r--   0        0        0     2898 2023-04-22 18:56:26.767149 aliendev_api-0.1.8/aliendev_api/main.py
+-rw-r--r--   0        0        0      435 2023-04-22 18:56:47.015447 aliendev_api-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 aliendev_api-0.1.8/PKG-INFO
```

### Comparing `aliendev_api-0.1.7/aliendev_api/config/__pycache__/mongo.cpython-311.pyc` & `aliendev_api-0.1.8/aliendev_api/config/__pycache__/mongo.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_api-0.1.7/aliendev_api/main.py` & `aliendev_api-0.1.8/aliendev_api/main.py`

 * *Files identical despite different names*

### Comparing `aliendev_api-0.1.7/PKG-INFO` & `aliendev_api-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliendev-api
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Nasri Adzlani
 Author-email: nasri@jkt1.ebdesk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

