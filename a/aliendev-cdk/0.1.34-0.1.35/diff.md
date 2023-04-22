# Comparing `tmp/aliendev_cdk-0.1.34.tar.gz` & `tmp/aliendev_cdk-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliendev_cdk-0.1.34.tar", max compression
+gzip compressed data, was "aliendev_cdk-0.1.35.tar", max compression
```

## Comparing `aliendev_cdk-0.1.34.tar` & `aliendev_cdk-0.1.35.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/README.md
--rw-r--r--   0        0        0        0 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/__init__.py
--rw-r--r--   0        0        0      824 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc
--rw-r--r--   0        0        0     1541 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc
--rw-r--r--   0        0        0      480 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/config/mongo.py
--rw-r--r--   0        0        0      744 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/config/rabbit.py
--rw-r--r--   0        0        0      689 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/main.py
--rw-r--r--   0        0        0     3431 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc
--rw-r--r--   0        0        0     2567 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc
--rw-r--r--   0        0        0     2568 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc
--rw-r--r--   0        0        0     1151 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc
--rw-r--r--   0        0        0     1595 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/service/deployService.py
--rw-r--r--   0        0        0     1237 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/service/loginService.py
--rw-r--r--   0        0        0      288 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/service/logoutService.py
--rw-r--r--   0        0        0     1193 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/service/registerService.py
--rw-r--r--   0        0        0       25 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/service/template/README.md
--rw-r--r--   0        0        0       38 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/service/template/helper/test_get.py
--rw-r--r--   0        0        0      128 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/service/template/helper/test_post.py
--rw-r--r--   0        0        0      356 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/service/template/lib/stack.py
--rw-r--r--   0        0        0     1516 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/aliendev_cdk/service/templateService.py
--rw-r--r--   0        0        0      452 2023-04-22 08:45:33.127702 aliendev_cdk-0.1.34/pyproject.toml
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 aliendev_cdk-0.1.34/PKG-INFO
+-rw-r--r--   0        0        0     1912 2023-04-22 14:39:00.184198 aliendev_cdk-0.1.35/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 14:39:00.184198 aliendev_cdk-0.1.35/aliendev_cdk/__init__.py
+-rw-r--r--   0        0        0      824 2023-04-22 14:39:00.184198 aliendev_cdk-0.1.35/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc
+-rw-r--r--   0        0        0     1541 2023-04-22 14:39:00.184198 aliendev_cdk-0.1.35/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc
+-rw-r--r--   0        0        0      480 2023-04-22 14:39:00.184198 aliendev_cdk-0.1.35/aliendev_cdk/config/mongo.py
+-rw-r--r--   0        0        0      744 2023-04-22 14:39:00.184198 aliendev_cdk-0.1.35/aliendev_cdk/config/rabbit.py
+-rw-r--r--   0        0        0      689 2023-04-22 14:39:00.184198 aliendev_cdk-0.1.35/aliendev_cdk/main.py
+-rw-r--r--   0        0        0     3431 2023-04-22 14:39:00.184198 aliendev_cdk-0.1.35/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc
+-rw-r--r--   0        0        0     2567 2023-04-22 14:39:00.188198 aliendev_cdk-0.1.35/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc
+-rw-r--r--   0        0        0     2568 2023-04-22 14:39:00.188198 aliendev_cdk-0.1.35/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc
+-rw-r--r--   0        0        0     1151 2023-04-22 14:39:00.188198 aliendev_cdk-0.1.35/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc
+-rw-r--r--   0        0        0     1595 2023-04-22 14:39:00.188198 aliendev_cdk-0.1.35/aliendev_cdk/service/deployService.py
+-rw-r--r--   0        0        0     1237 2023-04-22 14:39:00.188198 aliendev_cdk-0.1.35/aliendev_cdk/service/loginService.py
+-rw-r--r--   0        0        0      288 2023-04-22 14:39:00.188198 aliendev_cdk-0.1.35/aliendev_cdk/service/logoutService.py
+-rw-r--r--   0        0        0     1193 2023-04-22 14:39:00.188198 aliendev_cdk-0.1.35/aliendev_cdk/service/registerService.py
+-rw-r--r--   0        0        0       25 2023-04-22 14:39:00.188198 aliendev_cdk-0.1.35/aliendev_cdk/service/template/README.md
+-rw-r--r--   0        0        0       38 2023-04-22 14:39:00.188198 aliendev_cdk-0.1.35/aliendev_cdk/service/template/helper/test_get.py
+-rw-r--r--   0        0        0      128 2023-04-22 14:39:00.188198 aliendev_cdk-0.1.35/aliendev_cdk/service/template/helper/test_post.py
+-rw-r--r--   0        0        0      356 2023-04-22 14:39:00.188198 aliendev_cdk-0.1.35/aliendev_cdk/service/template/lib/stack.py
+-rw-r--r--   0        0        0     1464 2023-04-22 14:39:00.188198 aliendev_cdk-0.1.35/aliendev_cdk/service/templateService.py
+-rw-r--r--   0        0        0      452 2023-04-22 14:39:00.188198 aliendev_cdk-0.1.35/pyproject.toml
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 aliendev_cdk-0.1.35/PKG-INFO
```

### Comparing `aliendev_cdk-0.1.34/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc` & `aliendev_cdk-0.1.35/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.34/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc` & `aliendev_cdk-0.1.35/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.34/aliendev_cdk/config/rabbit.py` & `aliendev_cdk-0.1.35/aliendev_cdk/config/rabbit.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.34/aliendev_cdk/main.py` & `aliendev_cdk-0.1.35/aliendev_cdk/main.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.34/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc` & `aliendev_cdk-0.1.35/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.34/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc` & `aliendev_cdk-0.1.35/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.34/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc` & `aliendev_cdk-0.1.35/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.34/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc` & `aliendev_cdk-0.1.35/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.34/aliendev_cdk/service/deployService.py` & `aliendev_cdk-0.1.35/aliendev_cdk/service/deployService.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.34/aliendev_cdk/service/loginService.py` & `aliendev_cdk-0.1.35/aliendev_cdk/service/loginService.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.34/aliendev_cdk/service/registerService.py` & `aliendev_cdk-0.1.35/aliendev_cdk/service/registerService.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.34/aliendev_cdk/service/templateService.py` & `aliendev_cdk-0.1.35/aliendev_cdk/service/templateService.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 
 def init(name):
     os.makedirs(name)
     os.makedirs(name+"/config")
     os.makedirs(name+"/helper")
     os.makedirs(name+"/lib")
-    shutil.copy2('aliendev_cdk/service/template/helper/test_get.py', name+"/helper/")
-    shutil.copy2('aliendev_cdk/service/template/helper/test_post.py', name+"/helper/")
-    shutil.copy2('aliendev_cdk/service/template/lib/stack.py', name+"/lib/")
-    shutil.copy2('aliendev_cdk/service/template/README.md', name+"/")
+    shutil.copy2('service/template/helper/test_get.py', name+"/helper/")
+    shutil.copy2('service/template/helper/test_post.py', name+"/helper/")
+    shutil.copy2('service/template/lib/stack.py', name+"/lib/")
+    shutil.copy2('service/template/README.md', name+"/")
 
     # with open(name+"/helper/test_get.py","w") as file:
     #     file.write("def handler(event:dict):\n")
     #     file.write("\treturn event")
     
     # with open(name+"/helper/test_post.py","w") as file:
     #     file.write("def handler(event:dict):\n")
```

