# Comparing `tmp/rewards_api-0.0.3.tar.gz` & `tmp/rewards_api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewards_api-0.0.3.tar", last modified: Fri Apr 21 15:05:39 2023, max compression
+gzip compressed data, was "rewards_api-0.0.4.tar", last modified: Sat Apr 22 00:39:54 2023, max compression
```

## Comparing `rewards_api-0.0.3.tar` & `rewards_api-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-21 15:05:39.525786 rewards_api-0.0.3/
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-04-21 15:05:39.525786 rewards_api-0.0.3/PKG-INFO
--rw-r--r--   0 anindya   (1000) anindya   (1000)     5582 2023-04-21 05:26:09.000000 rewards_api-0.0.3/README.md
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      623 2023-04-21 14:36:16.000000 rewards_api-0.0.3/pyproject.toml
-drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-21 15:05:39.525786 rewards_api-0.0.3/rewards_api/
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      213 2023-04-21 14:55:00.000000 rewards_api-0.0.3/rewards_api/__init__.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      634 2023-04-21 14:40:51.000000 rewards_api-0.0.3/rewards_api/cli.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      883 2023-04-21 05:27:10.000000 rewards_api-0.0.3/rewards_api/config.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     8116 2023-04-21 14:00:28.000000 rewards_api-0.0.3/rewards_api/main.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     9791 2023-04-21 07:15:50.000000 rewards_api-0.0.3/rewards_api/streamer.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)    13941 2023-04-21 14:00:47.000000 rewards_api-0.0.3/rewards_api/utils.py
-drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-21 15:05:39.525786 rewards_api-0.0.3/rewards_api.egg-info/
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-04-21 15:05:39.000000 rewards_api-0.0.3/rewards_api.egg-info/PKG-INFO
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      375 2023-04-21 15:05:39.000000 rewards_api-0.0.3/rewards_api.egg-info/SOURCES.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)        1 2023-04-21 15:05:39.000000 rewards_api-0.0.3/rewards_api.egg-info/dependency_links.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       63 2023-04-21 15:05:39.000000 rewards_api-0.0.3/rewards_api.egg-info/entry_points.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       80 2023-04-21 15:05:39.000000 rewards_api-0.0.3/rewards_api.egg-info/requires.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       12 2023-04-21 15:05:39.000000 rewards_api-0.0.3/rewards_api.egg-info/top_level.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       38 2023-04-21 15:05:39.525786 rewards_api-0.0.3/setup.cfg
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     1017 2023-04-21 15:05:37.000000 rewards_api-0.0.3/setup.py
+drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 00:39:54.832357 rewards_api-0.0.4/
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-04-22 00:39:54.832357 rewards_api-0.0.4/PKG-INFO
+-rw-r--r--   0 anindya   (1000) anindya   (1000)     5582 2023-04-21 05:26:09.000000 rewards_api-0.0.4/README.md
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      623 2023-04-21 14:36:16.000000 rewards_api-0.0.4/pyproject.toml
+drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 00:39:54.832357 rewards_api-0.0.4/rewards_api/
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      228 2023-04-22 00:31:39.000000 rewards_api-0.0.4/rewards_api/__init__.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      239 2023-04-22 00:30:22.000000 rewards_api-0.0.4/rewards_api/cli.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      565 2023-04-22 00:31:16.000000 rewards_api-0.0.4/rewards_api/cli_args.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     1149 2023-04-22 00:31:30.000000 rewards_api-0.0.4/rewards_api/config.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     8717 2023-04-21 20:56:06.000000 rewards_api-0.0.4/rewards_api/main.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     9791 2023-04-21 07:15:50.000000 rewards_api-0.0.4/rewards_api/streamer.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)    12490 2023-04-21 20:39:52.000000 rewards_api-0.0.4/rewards_api/utils.py
+drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 00:39:54.832357 rewards_api-0.0.4/rewards_api.egg-info/
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-04-22 00:39:54.000000 rewards_api-0.0.4/rewards_api.egg-info/PKG-INFO
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      399 2023-04-22 00:39:54.000000 rewards_api-0.0.4/rewards_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)        1 2023-04-22 00:39:54.000000 rewards_api-0.0.4/rewards_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       63 2023-04-22 00:39:54.000000 rewards_api-0.0.4/rewards_api.egg-info/entry_points.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       86 2023-04-22 00:39:54.000000 rewards_api-0.0.4/rewards_api.egg-info/requires.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       12 2023-04-22 00:39:54.000000 rewards_api-0.0.4/rewards_api.egg-info/top_level.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       38 2023-04-22 00:39:54.832357 rewards_api-0.0.4/setup.cfg
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     1035 2023-04-22 00:34:10.000000 rewards_api-0.0.4/setup.py
```

### Comparing `rewards_api-0.0.3/PKG-INFO` & `rewards_api-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewards_api
-Version: 0.0.3
+Version: 0.0.4
 Summary: rewards api cli package for starting the local rewards server
 Home-page: https://github.com/rewards-ai/rewards-api/tree/latest
 Author: rewards.ai
 Author-email: proanindyadeep@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rewards_api-0.0.3/README.md` & `rewards_api-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rewards_api-0.0.3/pyproject.toml` & `rewards_api-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rewards_api-0.0.3/rewards_api/cli.py` & `rewards_api-0.0.4/rewards_api/cli_args.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-import argparse 
-from .main import app 
+import argparse
 
-def main():
-    parser = argparse.ArgumentParser(
+
+parser = argparse.ArgumentParser(
         description="rewards-api v0.0.1 package to launch the rewards backend server"
     )
     
-    parser.add_argument(
-        "--url", "-u", type=str, default="127.0.0.1", 
-        help = "The host connection url."
-    )
-    
-    parser.add_argument(
-        "--port", "-p", type=int, default=8000, 
-        help = "The port to connect to"
-    )
-    
-    args = parser.parse_args() 
-    debug = True 
-    app.run(
-        host = args.url, 
-        port = args.port, 
-        debug = debug
-    )
-    
+parser.add_argument(
+    "metrics", type=str, default="", 
+    help="The file path of the metrics which is located inside the reacts's repo under src/assets/temp.json"
+)
+
+parser.add_argument(
+    "--url", "-u", type=str, default="127.0.0.1", 
+    help = "The host connection url."
+)
+
+parser.add_argument(
+    "--port", "-p", type=int, default=8000, 
+    help = "The port to connect to"
+)
 
-if __name__ == "__main__":
-    main() 
+args = parser.parse_args()
```

### Comparing `rewards_api-0.0.3/rewards_api/config.py` & `rewards_api-0.0.4/rewards_api/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 import os 
 from dataclasses import dataclass 
 from typing import Optional
+from .cli_args import args 
+
+
+
+env_file = open(".env", "r").read()
+aws_access, aws_secret_access = [env_file.split("\n")[i].split("=")[1] for i in range(2)]
 
 @dataclass(kw_only=True)
 class GlobalConfig:
     DEVICE: str = "cpu"
     IN_FEATURES: int = 5
     TEST_TRIALS: int = 5
     MODEL_NAME: str = "model.pth"
@@ -15,10 +21,13 @@
     TRAINING_METRICS_JSON_NAME : str = "training_metrics.json"
     EVALUATION_METRICS_JSON_NAME : str = "evaluation_metrics.json"
     MODEL_HISTORY_JSON_NAME : str = "model_history.json"
 
     EVALUATION_TOTAL_TIME_FOR_TRAINING_PATH : int = 30
     EVALUATION_TOTAL_TIME_FOR_EVALUATION_PATH : int = 60
     
-    STREAMING_TEMP_JSON_PATH: str = "/home/anindya/workspace/RewardsHQ/RewardsSuit/training-platform/src/assets/temp.json"
+    AWS_SECRET_KEY : str = aws_access
+    AWS_SECRET_ACCESS_KEY : str = aws_secret_access
+    
+    STREAMING_TEMP_JSON_PATH: str = args.metrics #"/home/anindya/workspace/RewardsHQ/RewardsSuit/training-platform/src/assets/temp.json"
 
 CONFIG = GlobalConfig().__dict__.copy()
```

### Comparing `rewards_api-0.0.3/rewards_api/main.py` & `rewards_api-0.0.4/rewards_api/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,19 +153,23 @@
     ---
     parameters:
     
     - request (Request): Incoming request headers 
     - body (EnvironmentConfigurations): Request body
     """
     body = request.json
+    reward_function = body["reward_function"]
+    
+    # validate the reward function here TODO 
+    
     utils.add_inside_session(
         session_id=body["session_id"], config_name = "training_params",
         learning_algorithm = body["learning_algorithm"], 
         enable_wandb = body["enable_wandb"] == 1, 
-        reward_function = body["reward_function"]
+        reward_function = reward_function
     )
     
     return {
         'status' : 200, 
         'response' : 'ok'
     } 
 
@@ -245,14 +249,15 @@
     
     return Response(
         rewards_streamer.train(), 
         mimetype = "multipart/x-mixed-replace; boundary=frame"
     )
 
 
+# Needs to be integrated with react 
 @app.route('/api/v1/evaluate/', methods = ['POST'])
 def evaluate_stream():
     body = request.json 
     session_id = body['session_id']
     mode = body['mode']
     track_num = int(body['track_num']) 
     rewards_streamer = RewardsStreamer(
@@ -264,20 +269,38 @@
             mode = mode, 
             track_num = track_num
         ), 
         mimetype = "multipart/x-mixed-replace; boundary=frame"
     )
 
 
-# Will be deprecated soon 
-@app.route('/api/v1/stop')
-def stop():
-    # global stop_streaming 
-    # stop_streaming = True 
-    return {"status": 204}
+@app.route('/api/v1/final_eval_score', methods = ['GET'])
+def get_final_evaluation_score_before_push():
+    session_id = request.args.get('session_id')
+    final_score = utils.calculate_evaluation_metric(session_id=session_id)
+    return {
+        'status' : 200, 
+        'score' : final_score
+    }
+
+
+@app.route('/api/v1/push_model', methods=["POST"])
+def push_model():
+    data = request.json
+    status = utils.push_model_to_s3(data)
+    if status:
+        return {
+            "status": 200
+        }
+    else:
+        return {
+            "status" : 500, 
+            "message" : "internal server error"
+        }
+
 
 if __name__ == '__main__':
    host = "127.0.0.1"
    port = 8000
    debug = True
    options = None
    app.run(host, port, debug, options)
```

### Comparing `rewards_api-0.0.3/rewards_api/streamer.py` & `rewards_api-0.0.4/rewards_api/streamer.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.0.3/rewards_api/utils.py` & `rewards_api-0.0.4/rewards_api/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os 
-import cv2  
-import json 
-import pygame 
+import json
+import boto3 
 import shutil 
 import numpy as np 
 from datetime import datetime 
 from typing import Optional, Any, Dict, Union 
 
 from .config import CONFIG 
 
@@ -71,21 +70,33 @@
             'plot_scores' : [], 
             'plot_mean_scores' : []
         }
         
         # NOTE: This is very much specific to the rewards Car Environment 
         session_evaluation_metrics = {
             'training' : {
-                "1" : {}, # this will contain the trials results 
-                "2" : {}, 
-                "3" : {}
+                "1" : {
+                    "num_trials" : 1, 
+                    "record" : 0
+                    }, # this will contain the trials results 
+                "2" : {
+                    "num_trials" : 1, 
+                    "record" : 0
+                    },
+                "3" : {
+                    "num_trials" : 1, 
+                    "record" : 0
+                    }
             }, 
             
             'evaluation': {
-                "1" : {}
+                "1" : {
+                    "num_trials" : 1, 
+                    "record" : 0
+                    }
             }
         }
         
         with open(os.path.join(session_dir, CONFIG['TRAINING_METRICS_JSON_NAME']), "w") as json_file:
             json.dump(session_training_metrics, json_file)
         print(f"=> Created session_training_metrics.json for session: {session_name}")
         
@@ -298,112 +309,52 @@
 
 def convert_str_func_to_exec(str_function: str, function_name: str):
     globals_dict = {}
     exec(str_function, globals_dict)
     new_func = globals_dict[function_name]
     return new_func
 
-def generate(session_id, model_name : Optional[str] = None):
-    r = get_session_files(session_id)
-    print(session_id)
-    print("check" ,session_id)
-    record = 0
-    done = False
-    #enableStreaming()
-    
-    # environment parameters 
-    env_world = int(r["env_params"]["environment_world"])
-    mode = "training"
-    car_speed = r["env_params"]["car_speed"]
-    
-    # agent parameters
-    layer_config = eval(r["agent_params"]["model_configuration"])
-    if type(layer_config) == str:
-        layer_config = eval(layer_config)
-    
-    # training parameters 
-    
-    lr = r["agent_params"]["learning_rate"]
-    loss = r["agent_params"]["loss_fn"]
-    optimizer = r["agent_params"]["optimizer"]
-    gamma = r["agent_params"]["gamma"] / 100 # have to change it later
-    epsilon = r["agent_params"]['epsilon']
-    num_episodes = r["agent_params"]["num_episodes"]
-    reward_function = r["training_params"]["reward_function"]
-    
-    checkpoint_folder_path = os.path.join(
-        get_home_path(),
-        CONFIG["REWARDS_PARENT_CONFIG_DIR"], 
-        f"{session_id}/{CONFIG['REWARDS_CONFIG_MODEL_FOLDER_NAME']}/"
-    )
-    
-    screen_size = (800, 700)
-    model = LinearQNet(layer_config)
-    env_config = CarConfig(
-        car_fps = car_speed,
-        render_mode = "rgb_array",
-        render_fps=car_speed, 
-        screen_size=screen_size, 
-    )
-    
-    game = CarGame(
-        mode = mode, 
-        track_num = env_world, 
-        reward_function=convert_str_func_to_exec(
-            reward_function, function_name="reward_function"
-        ), 
-        config = env_config
+
+# rewards_metric_calculator 
+
+def calculate_evaluation_metric(session_id, session_root_dir: Optional[str] = None):
+    session_root_dir = (
+        os.path.join(get_home_path(), ".rewards_ai")
+        if session_root_dir is None
+        else session_root_dir
     )
+
+    evaluation_metric_json_path = os.path.join(session_root_dir, session_id, CONFIG['EVALUATION_METRICS_JSON_NAME'])
+    evaluation_metrics = json.load(open(evaluation_metric_json_path, "r"))
     
-    model_name = CONFIG['MODEL_NAME'] if model_name is None else model_name 
-    agent = QTrainer(
-        lr = lr, 
-        gamma = gamma, 
-        epsilon = epsilon, 
-        model = model, 
-        loss = loss, 
-        optimizer = optimizer, 
-        checkpoint_folder_path = checkpoint_folder_path, 
-        model_name = model_name 
-    )
+    final_score = 0.0 
+    for i in range(3):
+        final_score += (evaluation_metrics['training'][str(i)]['record'] / evaluation_metrics['training'][str(i)]['num_trials'])
     
-    plot_scores, plot_mean_scores = [], []
-    total_score, record = 0, 0
+    final_score +=  (evaluation_metrics['evaluation']["1"]['record'] / evaluation_metrics['evaluation']["1"]['num_trials'])
+    return final_score
+
+
+# Pushing models to S3 
+
+def push_model_to_s3(data):
+    session_id = data["session_id"]
+    user = data["user"]
     
-    while True:
-        if agent.n_games == num_episodes:
-            pygame.quit() 
-            return {
-                "status" : 204
-            }
-            
-        _, done, score, pixel_data = agent.train_step(game)
-        game.timeTicking() 
+    try:
+        s3 = boto3.client(
+            's3',
+            aws_access_key_id=CONFIG['AWS_SECRET_KEY'],
+            aws_secret_access_key=CONFIG['AWS_SECRET_ACCESS_KEY']
+        )
         
-        if done:
-            game.initialize()
-            agent.n_games += 1 
-            agent.train_long_memory() 
-            
-            if score > record:
-                record = score 
-                agent.model.save(
-                    checkpoint_folder_path, 
-                    model_name, 
-                    device = CONFIG['DEVICE'], 
-                )
-            print('Game', agent.n_games, 'Score', score, 'Record:', record)
-            plot_scores.append(score)
-            total_score += score 
-            mean_score = total_score / agent.n_games
-            plot_mean_scores.append(mean_score)
-            
-            update_graphing_file(
-                session_id=session_id, 
-                data = {"plot_scores": plot_scores, "plot_mean_scores": plot_mean_scores}
-            )
-        img = np.fliplr(pixel_data)
-        img = np.rot90(img)
-        img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-        img = cv2.imencode(".png", img)[1]
-        yield (b'--frame\r\n' b'Content-Type: image/jpeg\r\n\r\n' + bytearray(img) + b'\r\n')
-        
+        def uploadDirectory(path, bucketname):
+            for root, dirs, files in os.walk(path):
+                for file in files:
+                    s3.upload_file(os.path.join(root,file), bucketname, "Models/" + user + "/" + file)
+                    
+        path = os.path.join(os.path.join(get_home_path(), ".rewards_ai"), session_id)
+        uploadDirectory(path, "clash-of-models")
+        return True 
+    except:
+        return False 
+
```

### Comparing `rewards_api-0.0.3/rewards_api.egg-info/PKG-INFO` & `rewards_api-0.0.4/rewards_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewards-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: rewards api cli package for starting the local rewards server
 Home-page: https://github.com/rewards-ai/rewards-api/tree/latest
 Author: rewards.ai
 Author-email: proanindyadeep@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rewards_api-0.0.3/setup.py` & `rewards_api-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fhand:
     long_description = fhand.read()
 
 setuptools.setup(
     name="rewards_api",
-    version="0.0.3",
+    version="0.0.4",
     author="rewards.ai",
     author_email="proanindyadeep@gmail.com",
     description="rewards api cli package for starting the local rewards server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rewards-ai/rewards-api/tree/latest",
     
@@ -18,15 +18,16 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "rewards-envs", 
         "rewards-experimental", 
         "torch", "opencv-python", 
-        "flask", "flask_cors", "flasgger"
+        "flask", "flask_cors", "flasgger", 
+        "boto3"
         ],
     packages=setuptools.find_packages(),
     python_requires=">=3.7",
     entry_points={
         "console_scripts": [
             "start-rewards-server = rewards_api.cli:main",
         ]
```

