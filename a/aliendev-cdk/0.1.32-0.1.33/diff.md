# Comparing `tmp/aliendev_cdk-0.1.32.tar.gz` & `tmp/aliendev_cdk-0.1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliendev_cdk-0.1.32.tar", max compression
+gzip compressed data, was "aliendev_cdk-0.1.33.tar", max compression
```

## Comparing `aliendev_cdk-0.1.32.tar` & `aliendev_cdk-0.1.33.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0        0 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/README.md
--rw-r--r--   0        0        0        0 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/__init__.py
--rw-r--r--   0        0        0      824 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc
--rw-r--r--   0        0        0     1541 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc
--rw-r--r--   0        0        0      480 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/config/mongo.py
--rw-r--r--   0        0        0      744 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/config/rabbit.py
--rw-r--r--   0        0        0      609 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/main.py
--rw-r--r--   0        0        0     3431 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc
--rw-r--r--   0        0        0     2567 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc
--rw-r--r--   0        0        0     2568 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc
--rw-r--r--   0        0        0     1151 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc
--rw-r--r--   0        0        0     1581 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/service/deployService.py
--rw-r--r--   0        0        0     1237 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/service/loginService.py
--rw-r--r--   0        0        0     1193 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/service/registerService.py
--rw-r--r--   0        0        0       25 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/service/template/README.md
--rw-r--r--   0        0        0       38 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/service/template/helper/test_get.py
--rw-r--r--   0        0        0      128 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/service/template/helper/test_post.py
--rw-r--r--   0        0        0      368 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/service/template/lib/stack.py
--rw-r--r--   0        0        0     1516 2023-04-22 08:34:50.395641 aliendev_cdk-0.1.32/aliendev_cdk/service/templateService.py
--rw-r--r--   0        0        0      452 2023-04-22 08:34:50.399641 aliendev_cdk-0.1.32/pyproject.toml
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 aliendev_cdk-0.1.32/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-22 08:42:06.407152 aliendev_cdk-0.1.33/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 08:42:06.407152 aliendev_cdk-0.1.33/aliendev_cdk/__init__.py
+-rw-r--r--   0        0        0      824 2023-04-22 08:42:06.407152 aliendev_cdk-0.1.33/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc
+-rw-r--r--   0        0        0     1541 2023-04-22 08:42:06.407152 aliendev_cdk-0.1.33/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc
+-rw-r--r--   0        0        0      480 2023-04-22 08:42:06.407152 aliendev_cdk-0.1.33/aliendev_cdk/config/mongo.py
+-rw-r--r--   0        0        0      744 2023-04-22 08:42:06.407152 aliendev_cdk-0.1.33/aliendev_cdk/config/rabbit.py
+-rw-r--r--   0        0        0      689 2023-04-22 08:42:06.407152 aliendev_cdk-0.1.33/aliendev_cdk/main.py
+-rw-r--r--   0        0        0     3431 2023-04-22 08:42:06.407152 aliendev_cdk-0.1.33/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc
+-rw-r--r--   0        0        0     2567 2023-04-22 08:42:06.407152 aliendev_cdk-0.1.33/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc
+-rw-r--r--   0        0        0     2568 2023-04-22 08:42:06.407152 aliendev_cdk-0.1.33/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc
+-rw-r--r--   0        0        0     1151 2023-04-22 08:42:06.407152 aliendev_cdk-0.1.33/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc
+-rw-r--r--   0        0        0     1595 2023-04-22 08:42:06.407152 aliendev_cdk-0.1.33/aliendev_cdk/service/deployService.py
+-rw-r--r--   0        0        0     1237 2023-04-22 08:42:06.407152 aliendev_cdk-0.1.33/aliendev_cdk/service/loginService.py
+-rw-r--r--   0        0        0      288 2023-04-22 08:42:06.411152 aliendev_cdk-0.1.33/aliendev_cdk/service/logoutService.py
+-rw-r--r--   0        0        0     1193 2023-04-22 08:42:06.411152 aliendev_cdk-0.1.33/aliendev_cdk/service/registerService.py
+-rw-r--r--   0        0        0       25 2023-04-22 08:42:06.411152 aliendev_cdk-0.1.33/aliendev_cdk/service/template/README.md
+-rw-r--r--   0        0        0       38 2023-04-22 08:42:06.411152 aliendev_cdk-0.1.33/aliendev_cdk/service/template/helper/test_get.py
+-rw-r--r--   0        0        0      128 2023-04-22 08:42:06.411152 aliendev_cdk-0.1.33/aliendev_cdk/service/template/helper/test_post.py
+-rw-r--r--   0        0        0      368 2023-04-22 08:42:06.411152 aliendev_cdk-0.1.33/aliendev_cdk/service/template/lib/stack.py
+-rw-r--r--   0        0        0     1516 2023-04-22 08:42:06.411152 aliendev_cdk-0.1.33/aliendev_cdk/service/templateService.py
+-rw-r--r--   0        0        0      452 2023-04-22 08:42:06.411152 aliendev_cdk-0.1.33/pyproject.toml
+-rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 aliendev_cdk-0.1.33/PKG-INFO
```

### Comparing `aliendev_cdk-0.1.32/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc` & `aliendev_cdk-0.1.33/aliendev_cdk/config/__pycache__/mongo.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.32/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc` & `aliendev_cdk-0.1.33/aliendev_cdk/config/__pycache__/rabbit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.32/aliendev_cdk/config/rabbit.py` & `aliendev_cdk-0.1.33/aliendev_cdk/config/rabbit.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.32/aliendev_cdk/main.py` & `aliendev_cdk-0.1.33/aliendev_cdk/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import typer
-from aliendev_cdk.service import loginService, registerService, templateService, deployService
+from aliendev_cdk.service import loginService, registerService, templateService, deployService, logoutService
 
 app = typer.Typer()
 
 @app.command("register")
 def register():
     registerService.register()
     
 @app.command("login")
 def login():
     loginService.login()
 
+@app.command("logout")
+def logout():
+    logoutService.logout()
+
 @app.command("init")
 def initTemplate():
     name = input("Application Name: ")
     new_name = name.replace("-","_").replace(" ","_")
     templateService.init(new_name)
 
 @app.command("deploy")
```

### Comparing `aliendev_cdk-0.1.32/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc` & `aliendev_cdk-0.1.33/aliendev_cdk/service/__pycache__/deployService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.32/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc` & `aliendev_cdk-0.1.33/aliendev_cdk/service/__pycache__/loginService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.32/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc` & `aliendev_cdk-0.1.33/aliendev_cdk/service/__pycache__/registerService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.32/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc` & `aliendev_cdk-0.1.33/aliendev_cdk/service/__pycache__/templateService.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.32/aliendev_cdk/service/deployService.py` & `aliendev_cdk-0.1.33/aliendev_cdk/service/deployService.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,17 @@
         self.account_id = ''
     
     def checking_account(self):
         home_folder = os.path.expanduser("~")
         path = f'{home_folder}/.aliendev'
         if not os.path.exists(path):
             os.makedirs(path)    
-            print("folder created")
+            print("please login first 🥹")
         if not os.path.exists(path+"/config.json"):
-            print("please login first")
+            print("please login first 🥹")
         else:
             with open(path+"/config.json",'r') as file:
                 json_file = json.loads(file.read())
                 self.username = json_file.get('username')
                 self.account_id = json_file.get('_id')
     
     def read(self):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aliendev_cdk-0.1.32/aliendev_cdk/service/loginService.py` & `aliendev_cdk-0.1.33/aliendev_cdk/service/loginService.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.32/aliendev_cdk/service/registerService.py` & `aliendev_cdk-0.1.33/aliendev_cdk/service/registerService.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.32/aliendev_cdk/service/templateService.py` & `aliendev_cdk-0.1.33/aliendev_cdk/service/templateService.py`

 * *Files identical despite different names*

### Comparing `aliendev_cdk-0.1.32/PKG-INFO` & `aliendev_cdk-0.1.33/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliendev-cdk
-Version: 0.1.32
+Version: 0.1.33
 Summary: 
 Author: Nasri Adzlani
 Author-email: nasri@jkt1.ebdesk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

