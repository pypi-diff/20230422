# Comparing `tmp/aliendev_api-0.1.5.tar.gz` & `tmp/aliendev_api-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliendev_api-0.1.5.tar", max compression
+gzip compressed data, was "aliendev_api-0.1.7.tar", max compression
```

## Comparing `aliendev_api-0.1.5.tar` & `aliendev_api-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-18 17:45:56.435969 aliendev_api-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-04-18 17:45:56.435917 aliendev_api-0.1.5/aliendev_api/__init__.py
--rw-r--r--   0        0        0      824 2023-04-19 19:11:20.493960 aliendev_api-0.1.5/aliendev_api/config/__pycache__/mongo.cpython-311.pyc
--rw-r--r--   0        0        0      479 2023-04-19 18:47:44.244132 aliendev_api-0.1.5/aliendev_api/config/mongo.py
--rw-r--r--   0        0        0     2898 2023-04-20 18:53:54.796929 aliendev_api-0.1.5/aliendev_api/main.py
--rw-r--r--   0        0        0      377 2023-04-20 18:57:58.489136 aliendev_api-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 aliendev_api-0.1.5/setup.py
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 aliendev_api-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-22 08:44:09.528123 aliendev_api-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 08:44:09.528123 aliendev_api-0.1.7/aliendev_api/__init__.py
+-rw-r--r--   0        0        0      824 2023-04-22 08:44:09.528123 aliendev_api-0.1.7/aliendev_api/config/__pycache__/mongo.cpython-311.pyc
+-rw-r--r--   0        0        0      479 2023-04-22 08:44:09.528123 aliendev_api-0.1.7/aliendev_api/config/mongo.py
+-rw-r--r--   0        0        0     2898 2023-04-22 08:44:09.528123 aliendev_api-0.1.7/aliendev_api/main.py
+-rw-r--r--   0        0        0      377 2023-04-22 08:44:33.432344 aliendev_api-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 aliendev_api-0.1.7/PKG-INFO
```

### Comparing `aliendev_api-0.1.5/aliendev_api/config/__pycache__/mongo.cpython-311.pyc` & `aliendev_api-0.1.7/aliendev_api/config/__pycache__/mongo.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_api-0.1.5/aliendev_api/main.py` & `aliendev_api-0.1.7/aliendev_api/main.py`

 * *Files identical despite different names*

### Comparing `aliendev_api-0.1.5/PKG-INFO` & `aliendev_api-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliendev-api
-Version: 0.1.5
+Version: 0.1.7
 Summary: 
 Author: Nasri Adzlani
 Author-email: nasri@jkt1.ebdesk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

