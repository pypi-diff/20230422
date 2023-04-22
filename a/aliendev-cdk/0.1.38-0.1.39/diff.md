# Comparing `tmp/aliendev_cdk-0.1.38.tar.gz` & `tmp/aliendev_cdk-0.1.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliendev_cdk-0.1.38.tar", max compression
+gzip compressed data, was "aliendev_cdk-0.1.39.tar", max compression
```

## Comparing `aliendev_cdk-0.1.38.tar` & `aliendev_cdk-0.1.39.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1912 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/README.md
--rw-r--r--   0        0        0        0 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/__init__.py
--rw-r--r--   0        0        0      824 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc
--rw-r--r--   0        0        0     1541 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc
--rw-r--r--   0        0        0      486 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/config/mongo.py
--rw-r--r--   0        0        0      744 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/config/rabbit.py
--rw-r--r--   0        0        0      689 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/main.py
--rw-r--r--   0        0        0     3431 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc
--rw-r--r--   0        0        0     2567 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc
--rw-r--r--   0        0        0     2568 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc
--rw-r--r--   0        0        0     1151 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc
--rw-r--r--   0        0        0     1595 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/service/deployService.py
--rw-r--r--   0        0        0     1237 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/service/loginService.py
--rw-r--r--   0        0        0      284 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/service/logoutService.py
--rw-r--r--   0        0        0     1193 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/service/registerService.py
--rw-r--r--   0        0        0       25 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/service/template/README.md
--rw-r--r--   0        0        0       38 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/service/template/helper/test_get.py
--rw-r--r--   0        0        0      128 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/service/template/helper/test_post.py
--rw-r--r--   0        0        0      356 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/service/template/lib/stack.py
--rw-r--r--   0        0        0     1442 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/aliendev_cdk/service/templateService.py
--rw-r--r--   0        0        0      452 2023-04-22 14:56:19.390441 aliendev_cdk-0.1.38/pyproject.toml
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 aliendev_cdk-0.1.38/PKG-INFO
+-rw-r--r--   0        0        0     1912 2023-04-22 19:09:23.259084 aliendev_cdk-0.1.39/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 19:09:23.259084 aliendev_cdk-0.1.39/aliendev_cdk/__init__.py
+-rw-r--r--   0        0        0      824 2023-04-22 19:09:23.259084 aliendev_cdk-0.1.39/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc
+-rw-r--r--   0        0        0     1541 2023-04-22 19:09:23.259084 aliendev_cdk-0.1.39/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc
+-rw-r--r--   0        0        0      486 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/config/mongo.py
+-rw-r--r--   0        0        0      789 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/config/rabbit.py
+-rw-r--r--   0        0        0      689 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/main.py
+-rw-r--r--   0        0        0     3431 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc
+-rw-r--r--   0        0        0     2567 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc
+-rw-r--r--   0        0        0     2568 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc
+-rw-r--r--   0        0        0     1151 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc
+-rw-r--r--   0        0        0     1597 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/service/deployService.py
+-rw-r--r--   0        0        0     1237 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/service/loginService.py
+-rw-r--r--   0        0        0      284 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/service/logoutService.py
+-rw-r--r--   0        0        0     1193 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/service/registerService.py
+-rw-r--r--   0        0        0       25 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/service/template/README.md
+-rw-r--r--   0        0        0       38 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/service/template/helper/test_get.py
+-rw-r--r--   0        0        0      128 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/service/template/helper/test_post.py
+-rw-r--r--   0        0        0      356 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/service/template/lib/stack.py
+-rw-r--r--   0        0        0     1442 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/aliendev_cdk/service/templateService.py
+-rw-r--r--   0        0        0      452 2023-04-22 19:09:23.263084 aliendev_cdk-0.1.39/pyproject.toml
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 aliendev_cdk-0.1.39/PKG-INFO
```

### Comparing `aliendev_cdk-0.1.38/README.md` & `aliendev_cdk-0.1.39/README.md`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.38/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc` & `aliendev_cdk-0.1.39/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.38/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc` & `aliendev_cdk-0.1.39/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.38/aliendev_cdk/config/rabbit.py` & `aliendev_cdk-0.1.39/aliendev_cdk/config/rabbit.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,8 +13,9 @@
     connection = pika.BlockingConnection(parameters)
     channel = connection.channel()
     channel.queue_declare(queue=queue)
 
     channel.exchange_declare(exchange="aliendev", exchange_type="topic")
     channel.queue_bind(queue=queue, exchange="aliendev",routing_key="aliendev-route")
     channel.basic_publish(exchange="aliendev", routing_key="aliendev-route", body=json.dumps(body))
-    print(f"Sent message '{json.dumps(body)}'")
+    # print(f"Sent message '{json.dumps(body)}'")
+    print("Your engine has deployed 😀")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aliendev_cdk-0.1.38/aliendev_cdk/main.py` & `aliendev_cdk-0.1.39/aliendev_cdk/main.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.38/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc` & `aliendev_cdk-0.1.39/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.38/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc` & `aliendev_cdk-0.1.39/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.38/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc` & `aliendev_cdk-0.1.39/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.38/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc` & `aliendev_cdk-0.1.39/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.38/aliendev_cdk/service/deployService.py` & `aliendev_cdk-0.1.39/aliendev_cdk/service/deployService.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,9 +37,9 @@
             file_name = file.split("/")[-1]
             with open(file, 'r') as f:
                 # print(f.read())
                 strings['username'] = self.username
                 strings['account_id'] = self.account_id
                 strings['file_name'] = file_name
                 strings['data'] = f.read()
-                print(strings)
+                # print(strings)
                 rabbit.produce('helper',strings)
```

### Comparing `aliendev_cdk-0.1.38/aliendev_cdk/service/loginService.py` & `aliendev_cdk-0.1.39/aliendev_cdk/service/loginService.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.38/aliendev_cdk/service/registerService.py` & `aliendev_cdk-0.1.39/aliendev_cdk/service/registerService.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.38/aliendev_cdk/service/templateService.py` & `aliendev_cdk-0.1.39/aliendev_cdk/service/templateService.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.38/PKG-INFO` & `aliendev_cdk-0.1.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliendev-cdk
-Version: 0.1.38
+Version: 0.1.39
 Summary: 
 Author: Nasri Adzlani
 Author-email: nasri@jkt1.ebdesk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

