# Comparing `tmp/ml_botting_core-1.0.2.tar.gz` & `tmp/ml_botting_core-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_botting_core-1.0.2.tar", last modified: Thu Apr 20 00:13:16 2023, max compression
+gzip compressed data, was "ml_botting_core-1.0.3.tar", last modified: Sat Apr 22 00:54:35 2023, max compression
```

## Comparing `ml_botting_core-1.0.2.tar` & `ml_botting_core-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.475421 ml_botting_core-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.475421 ml_botting_core-1.0.2/src/ml_botting_core/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/src/ml_botting_core/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/classification/universal_classifier_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/src/ml_botting_core/model_management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/model_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/model_management/download_models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/model_management/load_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/model_management/model_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/src/ml_botting_core/prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/prediction/prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/src/ml_botting_core/regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/regression/universal_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/src/ml_botting_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-20 00:13:16.000000 ml_botting_core-1.0.2/src/ml_botting_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-20 00:13:16.000000 ml_botting_core-1.0.2/src/ml_botting_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:13:16.000000 ml_botting_core-1.0.2/src/ml_botting_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 00:13:16.000000 ml_botting_core-1.0.2/src/ml_botting_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/tests/test_universal_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.609975 ml_botting_core-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/src/ml_botting_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/src/ml_botting_core/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/classification/universal_classifier_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/src/ml_botting_core/model_management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/model_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/model_management/download_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/model_management/load_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/model_management/model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/src/ml_botting_core/prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/prediction/prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/src/ml_botting_core/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/src/ml_botting_core/regression/universal_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/src/ml_botting_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-22 00:54:35.000000 ml_botting_core-1.0.3/src/ml_botting_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-22 00:54:35.000000 ml_botting_core-1.0.3/src/ml_botting_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:54:35.000000 ml_botting_core-1.0.3/src/ml_botting_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 00:54:35.000000 ml_botting_core-1.0.3/src/ml_botting_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:54:35.613975 ml_botting_core-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-22 00:53:12.000000 ml_botting_core-1.0.3/tests/test_universal_predictor.py
```

### Comparing `ml_botting_core-1.0.2/LICENSE` & `ml_botting_core-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.2/PKG-INFO` & `ml_botting_core-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_botting_core
-Version: 1.0.2
+Version: 1.0.3
 Summary: Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 Home-page: https://github.com/darkmatter2222/ml_botting_core
 Author: Ryan Susman
 Author-email: ryansusman@gmail.com
 Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -54,54 +54,62 @@
 {
    "public_models":[
       {
          "game":"eve_online",
          "model_name":"game_state",
          "download_latest":1,
          "download_latest_from":"https://storage.googleapis.com/eve_online_models/",
-         "model_root_directory":"O:\\eve_live_models\\game_state"
+         "model_root_directory":"O:\\eve_live_models\\game_state",
+         "model_log_directory":"O:\\eve_live_logs\\game_state",
+         "save_images":0
       }
    ]
 }
 ```
 
 
 ### Implementation 
 ```python
 from ml_botting_core import universal_predictor
 
 up_config = json.load(open(r'ml_botting_core_config.json'))
 up = universal_predictor(config=up_config)
-up.load_models()
 
 img = Image.open('some_image.png')
 state_result = up.predict(img, 'game_state')
 ```
 
 ### state_result
 ```json
 {
-   "argmax_index":0,
-   "value_at_argmax":0.76277816,
-   "class":"char_select",
+   "epoc_time":"1682138565007.508",
+   "argmax_index":2,
+   "value_at_argmax":"1.0",
+   "class":"jump_though_first",
    "classes":[
-      "char_select",
-      "connection_lost",
-      "in_flight",
-      "in_hanger"
+      "dock_now",
+      "invalid",
+      "jump_though_first",
+      "jump_through_second",
+      "no_action",
+      "warp_to_dock_3",
+      "warp_to_dock_4"
    ],
    "scores":[
-      0.7627781629562378,
-      0.004260888323187828,
-      3.3299270398856606e-06,
-      0.23295757174491882
+      1.2750345662162804e-15,
+      1.4581948495906438e-11,
+      1.0,
+      5.21881417175057e-17,
+      1.4712418422554443e-18,
+      1.2777047215389858e-12,
+      6.730089694497203e-17
    ],
-   "id": UUID("57a29474-de52-11ed-a215-2cf05d9fe8eb"),
+   "id":"98ad373b-e0a6-11ed-9b27-2cf05d9fe8eb",
    "image_saved":0,
-   "model_name":"game_state"
+   "model_name":"nav_options"
 }
 ```
```

### Comparing `ml_botting_core-1.0.2/README.md` & `ml_botting_core-1.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -39,54 +39,62 @@
 {
    "public_models":[
       {
          "game":"eve_online",
          "model_name":"game_state",
          "download_latest":1,
          "download_latest_from":"https://storage.googleapis.com/eve_online_models/",
-         "model_root_directory":"O:\\eve_live_models\\game_state"
+         "model_root_directory":"O:\\eve_live_models\\game_state",
+         "model_log_directory":"O:\\eve_live_logs\\game_state",
+         "save_images":0
       }
    ]
 }
 ```
 
 
 ### Implementation 
 ```python
 from ml_botting_core import universal_predictor
 
 up_config = json.load(open(r'ml_botting_core_config.json'))
 up = universal_predictor(config=up_config)
-up.load_models()
 
 img = Image.open('some_image.png')
 state_result = up.predict(img, 'game_state')
 ```
 
 ### state_result
 ```json
 {
-   "argmax_index":0,
-   "value_at_argmax":0.76277816,
-   "class":"char_select",
+   "epoc_time":"1682138565007.508",
+   "argmax_index":2,
+   "value_at_argmax":"1.0",
+   "class":"jump_though_first",
    "classes":[
-      "char_select",
-      "connection_lost",
-      "in_flight",
-      "in_hanger"
+      "dock_now",
+      "invalid",
+      "jump_though_first",
+      "jump_through_second",
+      "no_action",
+      "warp_to_dock_3",
+      "warp_to_dock_4"
    ],
    "scores":[
-      0.7627781629562378,
-      0.004260888323187828,
-      3.3299270398856606e-06,
-      0.23295757174491882
+      1.2750345662162804e-15,
+      1.4581948495906438e-11,
+      1.0,
+      5.21881417175057e-17,
+      1.4712418422554443e-18,
+      1.2777047215389858e-12,
+      6.730089694497203e-17
    ],
-   "id": UUID("57a29474-de52-11ed-a215-2cf05d9fe8eb"),
+   "id":"98ad373b-e0a6-11ed-9b27-2cf05d9fe8eb",
    "image_saved":0,
-   "model_name":"game_state"
+   "model_name":"nav_options"
 }
 ```
```

### Comparing `ml_botting_core-1.0.2/setup.cfg` & `ml_botting_core-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ml_botting_core
-version = 1.0.2
+version = 1.0.3
 author = Ryan Susman
 author_email = ryansusman@gmail.com
 description = Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/darkmatter2222/ml_botting_core
 project_urls =
```

### Comparing `ml_botting_core-1.0.2/src/ml_botting_core/base.py` & `ml_botting_core-1.0.3/src/ml_botting_core/base.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.2/src/ml_botting_core/classification/universal_classifier_trainer.py` & `ml_botting_core-1.0.3/src/ml_botting_core/classification/universal_classifier_trainer.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.2/src/ml_botting_core/model_management/download_models.py` & `ml_botting_core-1.0.3/src/ml_botting_core/model_management/download_models.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.2/src/ml_botting_core/model_management/model_manager.py` & `ml_botting_core-1.0.3/src/ml_botting_core/model_management/model_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,35 @@
 import json
 import os
+import errno
 
 import tensorflow as tf
 from loguru import logger
 
 from .download_models import download_model, sync_model
 
 
+def mkdir_p(path):
+    try:
+        os.makedirs(path)
+    except OSError as exc:  # Python >2.5
+        if exc.errno == errno.EEXIST and os.path.isdir(path):
+            pass
+        else:
+            raise
+
+
+def construct_dirs(config_record):
+    if not os.path.isdir(config_record['model_root_directory']):
+        mkdir_p(config_record['model_root_directory'])
+
+    if not os.path.isdir(config_record['model_log_directory']):
+        mkdir_p(config_record['model_log_directory'])
+
+
 def get_local_file_locations(config_record):
     meta_file = f"{config_record['model_root_directory']}\\{config_record['model_name']}_meta.json"
     model_file = f"{config_record['model_root_directory']}\\{config_record['model_name']}_model.h5"
     gcp_file = f"{config_record['model_root_directory']}\\{config_record['model_name']}_gcp.json"
 
     meta_file_exist = os.path.isfile(meta_file)
     model_file_exist = os.path.isfile(model_file)
@@ -18,14 +37,15 @@
 
     return meta_file, model_file, gcp_file, meta_file_exist, model_file_exist, gcp_file_exist
 
 
 def process_model_config(config):
     if 'public_models' in config:
         for config_record in config['public_models']:
+            construct_dirs(config_record)
             ingest_public_model(config_record)
             logger.info(f"PreProcessed public_models {config_record['model_name']}")
             pass
     # TODO, Build This
     if 'private_models' in config:
         for config_record in config['private_models']:
             ingest_private_model(config_record)
@@ -55,14 +75,15 @@
 
     if not meta_file_exist or not model_file_exist or not gcp_file_exist:
         error = 'Attempted to load models that are not downloaded'
         logger.error(error)
         raise Exception(error)
 
     classifier = {
+        'config_record': config_record,
         'model': tf.keras.models.load_model(model_file),
         'meta': json.loads(open(meta_file, 'r').read()),
         'gcp': json.loads(open(gcp_file, 'r').read()),
     }
 
     return classifier
```

### Comparing `ml_botting_core-1.0.2/src/ml_botting_core.egg-info/PKG-INFO` & `ml_botting_core-1.0.3/src/ml_botting_core.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-botting-core
-Version: 1.0.2
+Version: 1.0.3
 Summary: Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 Home-page: https://github.com/darkmatter2222/ml_botting_core
 Author: Ryan Susman
 Author-email: ryansusman@gmail.com
 Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -54,54 +54,62 @@
 {
    "public_models":[
       {
          "game":"eve_online",
          "model_name":"game_state",
          "download_latest":1,
          "download_latest_from":"https://storage.googleapis.com/eve_online_models/",
-         "model_root_directory":"O:\\eve_live_models\\game_state"
+         "model_root_directory":"O:\\eve_live_models\\game_state",
+         "model_log_directory":"O:\\eve_live_logs\\game_state",
+         "save_images":0
       }
    ]
 }
 ```
 
 
 ### Implementation 
 ```python
 from ml_botting_core import universal_predictor
 
 up_config = json.load(open(r'ml_botting_core_config.json'))
 up = universal_predictor(config=up_config)
-up.load_models()
 
 img = Image.open('some_image.png')
 state_result = up.predict(img, 'game_state')
 ```
 
 ### state_result
 ```json
 {
-   "argmax_index":0,
-   "value_at_argmax":0.76277816,
-   "class":"char_select",
+   "epoc_time":"1682138565007.508",
+   "argmax_index":2,
+   "value_at_argmax":"1.0",
+   "class":"jump_though_first",
    "classes":[
-      "char_select",
-      "connection_lost",
-      "in_flight",
-      "in_hanger"
+      "dock_now",
+      "invalid",
+      "jump_though_first",
+      "jump_through_second",
+      "no_action",
+      "warp_to_dock_3",
+      "warp_to_dock_4"
    ],
    "scores":[
-      0.7627781629562378,
-      0.004260888323187828,
-      3.3299270398856606e-06,
-      0.23295757174491882
+      1.2750345662162804e-15,
+      1.4581948495906438e-11,
+      1.0,
+      5.21881417175057e-17,
+      1.4712418422554443e-18,
+      1.2777047215389858e-12,
+      6.730089694497203e-17
    ],
-   "id": UUID("57a29474-de52-11ed-a215-2cf05d9fe8eb"),
+   "id":"98ad373b-e0a6-11ed-9b27-2cf05d9fe8eb",
    "image_saved":0,
-   "model_name":"game_state"
+   "model_name":"nav_options"
 }
 ```
```

### Comparing `ml_botting_core-1.0.2/src/ml_botting_core.egg-info/SOURCES.txt` & `ml_botting_core-1.0.3/src/ml_botting_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

