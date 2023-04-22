# Comparing `tmp/aliendev_cdk-0.1.36.tar.gz` & `tmp/aliendev_cdk-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliendev_cdk-0.1.36.tar", max compression
+gzip compressed data, was "aliendev_cdk-0.1.37.tar", max compression
```

## Comparing `aliendev_cdk-0.1.36.tar` & `aliendev_cdk-0.1.37.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1912 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/README.md
--rw-r--r--   0        0        0        0 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/__init__.py
--rw-r--r--   0        0        0      824 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc
--rw-r--r--   0        0        0     1541 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc
--rw-r--r--   0        0        0      480 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/config/mongo.py
--rw-r--r--   0        0        0      744 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/config/rabbit.py
--rw-r--r--   0        0        0      689 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/main.py
--rw-r--r--   0        0        0     3431 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc
--rw-r--r--   0        0        0     2567 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc
--rw-r--r--   0        0        0     2568 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc
--rw-r--r--   0        0        0     1151 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc
--rw-r--r--   0        0        0     1595 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/service/deployService.py
--rw-r--r--   0        0        0     1237 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/service/loginService.py
--rw-r--r--   0        0        0      288 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/service/logoutService.py
--rw-r--r--   0        0        0     1193 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/service/registerService.py
--rw-r--r--   0        0        0       25 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/service/template/README.md
--rw-r--r--   0        0        0       38 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/service/template/helper/test_get.py
--rw-r--r--   0        0        0      128 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/service/template/helper/test_post.py
--rw-r--r--   0        0        0      356 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/service/template/lib/stack.py
--rw-r--r--   0        0        0     1442 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/aliendev_cdk/service/templateService.py
--rw-r--r--   0        0        0      452 2023-04-22 14:43:09.636064 aliendev_cdk-0.1.36/pyproject.toml
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 aliendev_cdk-0.1.36/PKG-INFO
+-rw-r--r--   0        0        0     1912 2023-04-22 14:51:42.252964 aliendev_cdk-0.1.37/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 14:51:42.252964 aliendev_cdk-0.1.37/aliendev_cdk/__init__.py
+-rw-r--r--   0        0        0      824 2023-04-22 14:51:42.252964 aliendev_cdk-0.1.37/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc
+-rw-r--r--   0        0        0     1541 2023-04-22 14:51:42.252964 aliendev_cdk-0.1.37/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc
+-rw-r--r--   0        0        0      480 2023-04-22 14:51:42.252964 aliendev_cdk-0.1.37/aliendev_cdk/config/mongo.py
+-rw-r--r--   0        0        0      744 2023-04-22 14:51:42.252964 aliendev_cdk-0.1.37/aliendev_cdk/config/rabbit.py
+-rw-r--r--   0        0        0      689 2023-04-22 14:51:42.252964 aliendev_cdk-0.1.37/aliendev_cdk/main.py
+-rw-r--r--   0        0        0     3431 2023-04-22 14:51:42.252964 aliendev_cdk-0.1.37/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc
+-rw-r--r--   0        0        0     2567 2023-04-22 14:51:42.256964 aliendev_cdk-0.1.37/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc
+-rw-r--r--   0        0        0     2568 2023-04-22 14:51:42.256964 aliendev_cdk-0.1.37/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc
+-rw-r--r--   0        0        0     1151 2023-04-22 14:51:42.256964 aliendev_cdk-0.1.37/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc
+-rw-r--r--   0        0        0     1595 2023-04-22 14:51:42.256964 aliendev_cdk-0.1.37/aliendev_cdk/service/deployService.py
+-rw-r--r--   0        0        0     1237 2023-04-22 14:51:42.256964 aliendev_cdk-0.1.37/aliendev_cdk/service/loginService.py
+-rw-r--r--   0        0        0      284 2023-04-22 14:51:42.256964 aliendev_cdk-0.1.37/aliendev_cdk/service/logoutService.py
+-rw-r--r--   0        0        0     1193 2023-04-22 14:51:42.256964 aliendev_cdk-0.1.37/aliendev_cdk/service/registerService.py
+-rw-r--r--   0        0        0       25 2023-04-22 14:51:42.256964 aliendev_cdk-0.1.37/aliendev_cdk/service/template/README.md
+-rw-r--r--   0        0        0       38 2023-04-22 14:51:42.256964 aliendev_cdk-0.1.37/aliendev_cdk/service/template/helper/test_get.py
+-rw-r--r--   0        0        0      128 2023-04-22 14:51:42.256964 aliendev_cdk-0.1.37/aliendev_cdk/service/template/helper/test_post.py
+-rw-r--r--   0        0        0      356 2023-04-22 14:51:42.256964 aliendev_cdk-0.1.37/aliendev_cdk/service/template/lib/stack.py
+-rw-r--r--   0        0        0     1442 2023-04-22 14:51:42.256964 aliendev_cdk-0.1.37/aliendev_cdk/service/templateService.py
+-rw-r--r--   0        0        0      452 2023-04-22 14:51:42.256964 aliendev_cdk-0.1.37/pyproject.toml
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 aliendev_cdk-0.1.37/PKG-INFO
```

### Comparing `aliendev_cdk-0.1.36/README.md` & `aliendev_cdk-0.1.37/README.md`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.36/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc` & `aliendev_cdk-0.1.37/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.36/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc` & `aliendev_cdk-0.1.37/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.36/aliendev_cdk/config/rabbit.py` & `aliendev_cdk-0.1.37/aliendev_cdk/config/rabbit.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.36/aliendev_cdk/main.py` & `aliendev_cdk-0.1.37/aliendev_cdk/main.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.36/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc` & `aliendev_cdk-0.1.37/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.36/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc` & `aliendev_cdk-0.1.37/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.36/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc` & `aliendev_cdk-0.1.37/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.36/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc` & `aliendev_cdk-0.1.37/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.36/aliendev_cdk/service/deployService.py` & `aliendev_cdk-0.1.37/aliendev_cdk/service/deployService.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.36/aliendev_cdk/service/loginService.py` & `aliendev_cdk-0.1.37/aliendev_cdk/service/loginService.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.36/aliendev_cdk/service/registerService.py` & `aliendev_cdk-0.1.37/aliendev_cdk/service/registerService.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.36/aliendev_cdk/service/templateService.py` & `aliendev_cdk-0.1.37/aliendev_cdk/service/templateService.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.36/PKG-INFO` & `aliendev_cdk-0.1.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliendev-cdk
-Version: 0.1.36
+Version: 0.1.37
 Summary: 
 Author: Nasri Adzlani
 Author-email: nasri@jkt1.ebdesk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

