# Comparing `tmp/rewards_api-0.0.9.tar.gz` & `tmp/rewards_api-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewards_api-0.0.9.tar", last modified: Sat Apr 22 04:10:41 2023, max compression
+gzip compressed data, was "rewards_api-0.1.0.tar", last modified: Sat Apr 22 15:29:41 2023, max compression
```

## Comparing `rewards_api-0.0.9.tar` & `rewards_api-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 04:10:41.011343 rewards_api-0.0.9/
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-04-22 04:10:41.011343 rewards_api-0.0.9/PKG-INFO
--rw-r--r--   0 anindya   (1000) anindya   (1000)     5582 2023-04-21 05:26:09.000000 rewards_api-0.0.9/README.md
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      623 2023-04-21 14:36:16.000000 rewards_api-0.0.9/pyproject.toml
-drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 04:10:41.011343 rewards_api-0.0.9/rewards_api/
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      228 2023-04-22 00:31:39.000000 rewards_api-0.0.9/rewards_api/__init__.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      239 2023-04-22 00:30:22.000000 rewards_api-0.0.9/rewards_api/cli.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      565 2023-04-22 00:31:16.000000 rewards_api-0.0.9/rewards_api/cli_args.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     1060 2023-04-22 00:47:59.000000 rewards_api-0.0.9/rewards_api/config.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)    10806 2023-04-22 01:08:30.000000 rewards_api-0.0.9/rewards_api/main.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)    11039 2023-04-22 04:08:13.000000 rewards_api-0.0.9/rewards_api/streamer.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)    12496 2023-04-22 04:08:17.000000 rewards_api-0.0.9/rewards_api/utils.py
-drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 04:10:41.011343 rewards_api-0.0.9/rewards_api.egg-info/
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-04-22 04:10:40.000000 rewards_api-0.0.9/rewards_api.egg-info/PKG-INFO
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      399 2023-04-22 04:10:40.000000 rewards_api-0.0.9/rewards_api.egg-info/SOURCES.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)        1 2023-04-22 04:10:40.000000 rewards_api-0.0.9/rewards_api.egg-info/dependency_links.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       63 2023-04-22 04:10:40.000000 rewards_api-0.0.9/rewards_api.egg-info/entry_points.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       99 2023-04-22 04:10:40.000000 rewards_api-0.0.9/rewards_api.egg-info/requires.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       12 2023-04-22 04:10:40.000000 rewards_api-0.0.9/rewards_api.egg-info/top_level.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       38 2023-04-22 04:10:41.011343 rewards_api-0.0.9/setup.cfg
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     1051 2023-04-22 04:10:33.000000 rewards_api-0.0.9/setup.py
+drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 15:29:41.015581 rewards_api-0.1.0/
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-04-22 15:29:41.015581 rewards_api-0.1.0/PKG-INFO
+-rw-r--r--   0 anindya   (1000) anindya   (1000)     5582 2023-04-21 05:26:09.000000 rewards_api-0.1.0/README.md
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      623 2023-04-21 14:36:16.000000 rewards_api-0.1.0/pyproject.toml
+drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 15:29:41.015581 rewards_api-0.1.0/rewards_api/
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      214 2023-04-22 15:13:14.000000 rewards_api-0.1.0/rewards_api/__init__.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      239 2023-04-22 15:14:35.000000 rewards_api-0.1.0/rewards_api/cli.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      565 2023-04-22 00:31:16.000000 rewards_api-0.1.0/rewards_api/cli_args.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     1058 2023-04-22 15:12:26.000000 rewards_api-0.1.0/rewards_api/config.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)    10809 2023-04-22 15:29:07.000000 rewards_api-0.1.0/rewards_api/main.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)    11132 2023-04-22 15:11:49.000000 rewards_api-0.1.0/rewards_api/streamer.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)    12496 2023-04-22 04:08:17.000000 rewards_api-0.1.0/rewards_api/utils.py
+drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 15:29:41.015581 rewards_api-0.1.0/rewards_api.egg-info/
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-04-22 15:29:40.000000 rewards_api-0.1.0/rewards_api.egg-info/PKG-INFO
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      399 2023-04-22 15:29:40.000000 rewards_api-0.1.0/rewards_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)        1 2023-04-22 15:29:40.000000 rewards_api-0.1.0/rewards_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       63 2023-04-22 15:29:40.000000 rewards_api-0.1.0/rewards_api.egg-info/entry_points.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       99 2023-04-22 15:29:40.000000 rewards_api-0.1.0/rewards_api.egg-info/requires.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       12 2023-04-22 15:29:40.000000 rewards_api-0.1.0/rewards_api.egg-info/top_level.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       38 2023-04-22 15:29:41.015581 rewards_api-0.1.0/setup.cfg
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     1054 2023-04-22 15:29:39.000000 rewards_api-0.1.0/setup.py
```

### Comparing `rewards_api-0.0.9/PKG-INFO` & `rewards_api-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewards_api
-Version: 0.0.9
+Version: 0.1.0
 Summary: rewards api cli package for starting the local rewards server
 Home-page: https://github.com/rewards-ai/rewards-api/tree/latest
 Author: rewards.ai
 Author-email: proanindyadeep@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rewards_api-0.0.9/README.md` & `rewards_api-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `rewards_api-0.0.9/pyproject.toml` & `rewards_api-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rewards_api-0.0.9/rewards_api/cli_args.py` & `rewards_api-0.1.0/rewards_api/cli_args.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.0.9/rewards_api/config.py` & `rewards_api-0.1.0/rewards_api/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import os 
 from dataclasses import dataclass 
 from typing import Optional
 from .cli_args import args 
 
 
-
-
 @dataclass(kw_only=True)
 class GlobalConfig:
     DEVICE: str = "cpu"
     IN_FEATURES: int = 5
     TEST_TRIALS: int = 5
     MODEL_NAME: str = "model.pth"
     REWARDS_PARENT_CONFIG_DIR: str = ".rewards_ai"
```

### Comparing `rewards_api-0.0.9/rewards_api/main.py` & `rewards_api-0.1.0/rewards_api/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,21 +333,21 @@
  
     for obj in response.get('Contents', []):
         folder = obj.get('Key', '').split('/')[-2] + '/'
         if folder != folder_name:
             set_of_users.add(folder)
  
     data = []
-    print(list(set_of_users))
+    #print(list(set_of_users))
     for user in list(set_of_users):
         temp = {}
         key_user = "Models/" + user + "user.json"
         key_score = "Models/" + user + "evaluation_metrics.json"
  
-        print(key_user, key_score)
+        #print(key_user, key_score)
  
         result = s3.get_object(Bucket=bucket_name, Key=key_user) 
         text = result["Body"].read().decode()
         text = json.loads(text)
         temp["user"] = text
  
         result = s3.get_object(Bucket=bucket_name, Key=key_score) 
@@ -366,10 +366,10 @@
  
 
 
 
 if __name__ == '__main__':
    host = "127.0.0.1"
    port = 8000
-   debug = True
+   debug = False
    options = None
    app.run(host, port, debug, options)
```

### Comparing `rewards_api-0.0.9/rewards_api/streamer.py` & `rewards_api-0.1.0/rewards_api/streamer.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,14 +243,17 @@
         
         while True:
             _, done, score, pixel_data = agent.evaluate(game)
             game.timeTicking() 
             
             current_time = time.time() 
             if current_time - start_time > elapsed_time:
+                if num_trials == 1:
+                    record = score 
+                    
                 eval_metrics_json['session_id'] = self.session_id
                 eval_metrics_json[mode]['total_elapsed_time'] = elapsed_time
                 eval_metrics_json[mode][str(track_num)] = {
                     "num_trials" : num_trials, 
                     "record" : record 
                 }
```

### Comparing `rewards_api-0.0.9/rewards_api/utils.py` & `rewards_api-0.1.0/rewards_api/utils.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.0.9/rewards_api.egg-info/PKG-INFO` & `rewards_api-0.1.0/rewards_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewards-api
-Version: 0.0.9
+Version: 0.1.0
 Summary: rewards api cli package for starting the local rewards server
 Home-page: https://github.com/rewards-ai/rewards-api/tree/latest
 Author: rewards.ai
 Author-email: proanindyadeep@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rewards_api-0.0.9/setup.py` & `rewards_api-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fhand:
     long_description = fhand.read()
 
 setuptools.setup(
     name="rewards_api",
-    version="0.0.9",
+    version="0.1.0",
     author="rewards.ai",
     author_email="proanindyadeep@gmail.com",
     description="rewards api cli package for starting the local rewards server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rewards-ai/rewards-api/tree/latest",
     
@@ -28,8 +28,10 @@
     packages=setuptools.find_packages(),
     python_requires=">=3.7",
     entry_points={
         "console_scripts": [
             "start-rewards-server = rewards_api.cli:main",
         ]
     }
-)
+)
+
+
```

