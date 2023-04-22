# Comparing `tmp/rewards_api-0.0.8.tar.gz` & `tmp/rewards_api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewards_api-0.0.8.tar", last modified: Sat Apr 22 01:29:08 2023, max compression
+gzip compressed data, was "rewards_api-0.0.9.tar", last modified: Sat Apr 22 04:10:41 2023, max compression
```

## Comparing `rewards_api-0.0.8.tar` & `rewards_api-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 01:29:08.097250 rewards_api-0.0.8/
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-04-22 01:29:08.097250 rewards_api-0.0.8/PKG-INFO
--rw-r--r--   0 anindya   (1000) anindya   (1000)     5582 2023-04-21 05:26:09.000000 rewards_api-0.0.8/README.md
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      623 2023-04-21 14:36:16.000000 rewards_api-0.0.8/pyproject.toml
-drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 01:29:08.097250 rewards_api-0.0.8/rewards_api/
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      228 2023-04-22 00:31:39.000000 rewards_api-0.0.8/rewards_api/__init__.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      239 2023-04-22 00:30:22.000000 rewards_api-0.0.8/rewards_api/cli.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      565 2023-04-22 00:31:16.000000 rewards_api-0.0.8/rewards_api/cli_args.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     1060 2023-04-22 00:47:59.000000 rewards_api-0.0.8/rewards_api/config.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)    10806 2023-04-22 01:08:30.000000 rewards_api-0.0.8/rewards_api/main.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)    11031 2023-04-22 01:06:11.000000 rewards_api-0.0.8/rewards_api/streamer.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)    12490 2023-04-21 20:39:52.000000 rewards_api-0.0.8/rewards_api/utils.py
-drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 01:29:08.097250 rewards_api-0.0.8/rewards_api.egg-info/
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-04-22 01:29:08.000000 rewards_api-0.0.8/rewards_api.egg-info/PKG-INFO
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      399 2023-04-22 01:29:08.000000 rewards_api-0.0.8/rewards_api.egg-info/SOURCES.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)        1 2023-04-22 01:29:08.000000 rewards_api-0.0.8/rewards_api.egg-info/dependency_links.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       63 2023-04-22 01:29:08.000000 rewards_api-0.0.8/rewards_api.egg-info/entry_points.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       99 2023-04-22 01:29:08.000000 rewards_api-0.0.8/rewards_api.egg-info/requires.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       12 2023-04-22 01:29:08.000000 rewards_api-0.0.8/rewards_api.egg-info/top_level.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       38 2023-04-22 01:29:08.097250 rewards_api-0.0.8/setup.cfg
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     1051 2023-04-22 01:29:05.000000 rewards_api-0.0.8/setup.py
+drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 04:10:41.011343 rewards_api-0.0.9/
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-04-22 04:10:41.011343 rewards_api-0.0.9/PKG-INFO
+-rw-r--r--   0 anindya   (1000) anindya   (1000)     5582 2023-04-21 05:26:09.000000 rewards_api-0.0.9/README.md
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      623 2023-04-21 14:36:16.000000 rewards_api-0.0.9/pyproject.toml
+drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 04:10:41.011343 rewards_api-0.0.9/rewards_api/
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      228 2023-04-22 00:31:39.000000 rewards_api-0.0.9/rewards_api/__init__.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      239 2023-04-22 00:30:22.000000 rewards_api-0.0.9/rewards_api/cli.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      565 2023-04-22 00:31:16.000000 rewards_api-0.0.9/rewards_api/cli_args.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     1060 2023-04-22 00:47:59.000000 rewards_api-0.0.9/rewards_api/config.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)    10806 2023-04-22 01:08:30.000000 rewards_api-0.0.9/rewards_api/main.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)    11039 2023-04-22 04:08:13.000000 rewards_api-0.0.9/rewards_api/streamer.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)    12496 2023-04-22 04:08:17.000000 rewards_api-0.0.9/rewards_api/utils.py
+drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 04:10:41.011343 rewards_api-0.0.9/rewards_api.egg-info/
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-04-22 04:10:40.000000 rewards_api-0.0.9/rewards_api.egg-info/PKG-INFO
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      399 2023-04-22 04:10:40.000000 rewards_api-0.0.9/rewards_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)        1 2023-04-22 04:10:40.000000 rewards_api-0.0.9/rewards_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       63 2023-04-22 04:10:40.000000 rewards_api-0.0.9/rewards_api.egg-info/entry_points.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       99 2023-04-22 04:10:40.000000 rewards_api-0.0.9/rewards_api.egg-info/requires.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       12 2023-04-22 04:10:40.000000 rewards_api-0.0.9/rewards_api.egg-info/top_level.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       38 2023-04-22 04:10:41.011343 rewards_api-0.0.9/setup.cfg
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     1051 2023-04-22 04:10:33.000000 rewards_api-0.0.9/setup.py
```

### Comparing `rewards_api-0.0.8/PKG-INFO` & `rewards_api-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewards_api
-Version: 0.0.8
+Version: 0.0.9
 Summary: rewards api cli package for starting the local rewards server
 Home-page: https://github.com/rewards-ai/rewards-api/tree/latest
 Author: rewards.ai
 Author-email: proanindyadeep@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rewards_api-0.0.8/README.md` & `rewards_api-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rewards_api-0.0.8/pyproject.toml` & `rewards_api-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rewards_api-0.0.8/rewards_api/cli_args.py` & `rewards_api-0.0.9/rewards_api/cli_args.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.0.8/rewards_api/config.py` & `rewards_api-0.0.9/rewards_api/config.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.0.8/rewards_api/main.py` & `rewards_api-0.0.9/rewards_api/main.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.0.8/rewards_api/streamer.py` & `rewards_api-0.0.9/rewards_api/streamer.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,18 +156,18 @@
                     
                 print('=> Session:', self.session_id, 'Game', agent.n_games, 'Score', score, 'Record:', record)
                 plot_scores.append(score)
                 total_score += score 
                 mean_score = total_score / agent.n_games
                 plot_mean_scores.append(mean_score)
                 
-                update_graphing_file(
-                    session_id = self.session_id, 
-                    data = {"plot_scores": plot_scores, "plot_mean_scores": plot_mean_scores}
-                )
+                # update_graphing_file(
+                #     session_id = self.session_id, 
+                #     data = {"plot_scores": plot_scores, "plot_mean_scores": plot_mean_scores}
+                # )
                 
                 # writing the latest changes after every done. So that closing will not loose
                 # latest information 
                 
                 self._write_model_json(
                     record=record, 
                     plot_scores=plot_scores,
```

### Comparing `rewards_api-0.0.8/rewards_api/utils.py` & `rewards_api-0.0.9/rewards_api/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 from rewards_envs import CarConfig, CarGame
 
 
 def get_home_path():
     # get the home directory using os
     return os.path.expanduser("~")
 
-def update_graphing_file(session_id: str, data: dict, dir: Optional[str] = None, name: Optional[str] = None) -> None:
-    f = open(CONFIG['STREAMING_TEMP_JSON_PATH'], "w")
-    f.write(json.dumps(data))
+# def update_graphing_file(session_id: str, data: dict, dir: Optional[str] = None, name: Optional[str] = None) -> None:
+#     f = open(CONFIG['STREAMING_TEMP_JSON_PATH'], "w")
+#     f.write(json.dumps(data))
     
 
 def create_folder_struct(dir: Optional[str] = None, name: Optional[str] = None) -> None:
     """Creates a root folder to store all the session configuration
 
     Args:
         dir (Optional[str], optional): _description_. Defaults to None.
```

### Comparing `rewards_api-0.0.8/rewards_api.egg-info/PKG-INFO` & `rewards_api-0.0.9/rewards_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewards-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: rewards api cli package for starting the local rewards server
 Home-page: https://github.com/rewards-ai/rewards-api/tree/latest
 Author: rewards.ai
 Author-email: proanindyadeep@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rewards_api-0.0.8/setup.py` & `rewards_api-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fhand:
     long_description = fhand.read()
 
 setuptools.setup(
     name="rewards_api",
-    version="0.0.8",
+    version="0.0.9",
     author="rewards.ai",
     author_email="proanindyadeep@gmail.com",
     description="rewards api cli package for starting the local rewards server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rewards-ai/rewards-api/tree/latest",
```

