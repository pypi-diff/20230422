# Comparing `tmp/cgpt-1.1.29.tar.gz` & `tmp/cgpt-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgpt-1.1.29.tar", last modified: Sat Apr 15 17:48:41 2023, max compression
+gzip compressed data, was "cgpt-1.2.1.tar", last modified: Sat Apr 22 14:10:42 2023, max compression
```

## Comparing `cgpt-1.1.29.tar` & `cgpt-1.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-15 17:48:41.886386 cgpt-1.1.29/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1065 2023-03-17 13:19:22.000000 cgpt-1.1.29/LICENSE
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       15 2023-03-17 13:19:22.000000 cgpt-1.1.29/MANIFEST.in
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1964 2023-04-15 17:48:41.886386 cgpt-1.1.29/PKG-INFO
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1825 2023-04-15 17:47:31.000000 cgpt-1.1.29/README.md
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-15 17:48:41.882386 cgpt-1.1.29/app/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-17 13:58:28.000000 cgpt-1.1.29/app/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     3552 2023-04-15 17:02:26.000000 cgpt-1.1.29/app/base.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-15 17:48:41.882386 cgpt-1.1.29/app/client/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.1.29/app/client/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1419 2023-04-14 13:20:28.000000 cgpt-1.1.29/app/client/main.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-15 17:48:41.882386 cgpt-1.1.29/app/commands/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-14 13:55:23.000000 cgpt-1.1.29/app/commands/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      110 2023-04-15 17:02:26.000000 cgpt-1.1.29/app/commands/main.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      572 2023-04-14 13:20:28.000000 cgpt-1.1.29/app/file_service.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      406 2023-04-12 19:52:50.000000 cgpt-1.1.29/app/main.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1432 2023-04-15 17:02:26.000000 cgpt-1.1.29/app/plugin.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-15 17:48:41.882386 cgpt-1.1.29/app/server/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.1.29/app/server/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1282 2023-04-14 13:20:28.000000 cgpt-1.1.29/app/server/main.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-15 17:48:41.886386 cgpt-1.1.29/app/utils/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.1.29/app/utils/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2740 2023-04-15 17:02:26.000000 cgpt-1.1.29/app/utils/constant.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      137 2023-04-12 19:52:50.000000 cgpt-1.1.29/app/utils/verify_env.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-15 17:48:41.886386 cgpt-1.1.29/cgpt.egg-info/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1964 2023-04-15 17:48:41.000000 cgpt-1.1.29/cgpt.egg-info/PKG-INFO
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      488 2023-04-15 17:48:41.000000 cgpt-1.1.29/cgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        1 2023-04-15 17:48:41.000000 cgpt-1.1.29/cgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       77 2023-04-15 17:48:41.000000 cgpt-1.1.29/cgpt.egg-info/entry_points.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       68 2023-04-15 17:48:41.000000 cgpt-1.1.29/cgpt.egg-info/requires.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        9 2023-04-15 17:48:41.000000 cgpt-1.1.29/cgpt.egg-info/top_level.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      984 2023-04-15 17:02:26.000000 cgpt-1.1.29/cgpt.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       38 2023-04-15 17:48:41.886386 cgpt-1.1.29/setup.cfg
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1133 2023-04-15 17:02:26.000000 cgpt-1.1.29/setup.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 14:10:42.364016 cgpt-1.2.1/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1065 2023-03-17 13:19:22.000000 cgpt-1.2.1/LICENSE
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       15 2023-03-17 13:19:22.000000 cgpt-1.2.1/MANIFEST.in
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2346 2023-04-22 14:10:42.364016 cgpt-1.2.1/PKG-INFO
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2202 2023-04-20 08:44:37.000000 cgpt-1.2.1/README.md
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 14:10:42.360016 cgpt-1.2.1/app/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-17 13:58:28.000000 cgpt-1.2.1/app/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     3550 2023-04-17 18:29:03.000000 cgpt-1.2.1/app/base.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 14:10:42.360016 cgpt-1.2.1/app/client/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.2.1/app/client/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1419 2023-04-14 13:20:28.000000 cgpt-1.2.1/app/client/main.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 14:10:42.360016 cgpt-1.2.1/app/commands/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-14 13:55:23.000000 cgpt-1.2.1/app/commands/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      110 2023-04-15 17:02:26.000000 cgpt-1.2.1/app/commands/main.py
+-rw-r--r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      670 2023-04-17 18:29:03.000000 cgpt-1.2.1/app/create_env.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      406 2023-04-12 19:52:50.000000 cgpt-1.2.1/app/main.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1430 2023-04-17 18:29:03.000000 cgpt-1.2.1/app/plugin.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 14:10:42.360016 cgpt-1.2.1/app/server/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.2.1/app/server/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1631 2023-04-17 18:29:03.000000 cgpt-1.2.1/app/server/main.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 14:10:42.360016 cgpt-1.2.1/app/utils/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.2.1/app/utils/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2771 2023-04-22 14:10:36.000000 cgpt-1.2.1/app/utils/constant.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      135 2023-04-17 18:29:03.000000 cgpt-1.2.1/app/utils/verify_env.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 14:10:42.364016 cgpt-1.2.1/cgpt.egg-info/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2346 2023-04-22 14:10:42.000000 cgpt-1.2.1/cgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      486 2023-04-22 14:10:42.000000 cgpt-1.2.1/cgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        1 2023-04-22 14:10:42.000000 cgpt-1.2.1/cgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       77 2023-04-22 14:10:42.000000 cgpt-1.2.1/cgpt.egg-info/entry_points.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       61 2023-04-22 14:10:42.000000 cgpt-1.2.1/cgpt.egg-info/requires.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        9 2023-04-22 14:10:42.000000 cgpt-1.2.1/cgpt.egg-info/top_level.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      982 2023-04-17 18:29:03.000000 cgpt-1.2.1/cgpt.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       38 2023-04-22 14:10:42.364016 cgpt-1.2.1/setup.cfg
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1114 2023-04-20 07:35:36.000000 cgpt-1.2.1/setup.py
```

### Comparing `cgpt-1.1.29/LICENSE` & `cgpt-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cgpt-1.1.29/PKG-INFO` & `cgpt-1.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 Metadata-Version: 2.1
 Name: cgpt
-Version: 1.1.29
+Version: 1.2.1
 Summary: Use openai chat-gpt on your cli
 Home-page: https://github.com/ainayves/cgpt>
 Author: Aina Yves
 Author-email: randrianaina.yves@gmail.com
 License: MIT
 Description: ![](https://komarev.com/ghpvc/?username=ainayves&color=blueviolet)
         
         ## Use openai chat-gpt on your CLI
         `cgpt` is a Python module that allows you to use Chat-GPT directly in your favorite Terminal.
         
+        ### ⭐ FEATURES
+        
+        - AI conversation exactly the same as in openai website
+        - LAN support (you can use cgpt inside a LAN)
+        - Docker support
+        
         ### REQUIREMENTS
         
         - python >=3.7
         - openai API KEY : 
         
         You need to register on openai to receive your own api key , here : [api_key](https://platform.openai.com/account/api-keys).
         
         ### SETUP
         
         ```
         pip install cgpt
         ```
         
-        ### ⏯️ GET VERSION 
+        ### ⏯️ VERIFY INSTALLATION 
         
         ```
         cgpt-version
         ```
         
         ### 🚀 RUN
         
@@ -52,14 +58,22 @@
         ```
         127.0.0.1	localhost
         127.0.1.1	your-hostanme
         ```
         
         - A `client` can also use his own api_key in the next version.
         
+        ### 🐋 RUN INSIDE DOCKER
+        
+        - To make it easier , use the `docker-compose.yml` file : 
+        
+        ```
+        docker-compose run --rm app
+        ```
+        
         ### GITHUB
         
         - [cgpt](https://github.com/ainayves/cgpt/)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `cgpt-1.1.29/README.md` & `cgpt-1.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 ![python](https://img.shields.io/badge/Python-3.7-blue.svg)
 ![commit activity](https://img.shields.io/github/commit-activity/m/ainayves/cgpt?color=blue)
 [![Build Status](https://img.shields.io/badge/Build%20status-Passing-green)](https://github.com/ainayves/cgpt/actions)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
-<center><h1>🌟 MAKE AI POWERED SEARCH INSIDE YOUR CLI 🌟</h1></center>
+<center><h1>🤖 MAKE AI POWERED SEARCH INSIDE YOUR CLI 💻</h1></center>
+</br>
+
+### ⭐ FEATURES
+
+- [AI conversation exactly the same as in openai website](#description)
+- [LAN support](#link-cgpt-inside-a-local-network)
+- [Docker support](#whale2-build-and-run-with-docker)
+
 </br>
 
 ![cgpt1 1 28 (1)](https://user-images.githubusercontent.com/66997516/232239452-27e5c840-5699-44b8-bb28-da8d2dabc64f.gif)
 
 </br>
 
+### DESCRIPTION
+
 `cgpt` is a Python module that allows you to use Chat-GPT directly in your favorite Terminal.
 
-### ❓ REQUIREMENTS
+### :question: REQUIREMENTS
 
 - python >=3.7
 - openai API KEY : 
 You need to register on openai to receive your own api key , here : [api_key](https://platform.openai.com/account/api-keys).
 
-### 💻 SETUP
+### 🖥️ SETUP
 
 ```
 pip install -r requirements.txt
 ```
 
 ### 🔨 BUILD
 
@@ -36,27 +46,27 @@
 ```
 Then , :
 
 ```
 ./build.sh
 ```
 
-### ⏯️ GET VERSION 
+### ⏯️ VERIFY INSTALLATION 
 
 ```
 cgpt-version
 ```
 
 ### 🚀 RUN
 
 ```
 cgpt
 ```
 
-### 🔗 CGPT INSIDE A LOCAL NETWORK
+### :link: CGPT INSIDE A LOCAL NETWORK
 
 You can use cgpt inside a LAN. 
 
 - You just need one Host (`connected to internet`) to be the server.
 - Other Hosts (`not connected to internet`) can ALWAYS use Chat GPT as `client`. 
 
 NOTES : 
@@ -68,10 +78,18 @@
 ```
 127.0.0.1	localhost
 127.0.1.1	your-hostanme
 ```
 
 - A `client` can also use his own api_key in the next version.
 
+### :whale2: BUILD AND RUN WITH DOCKER
+
+- To make it easier , use the `docker-compose.yml` file : 
+
+```
+docker-compose run --rm app
+```
+
 ### 💚 Feedback
 
 Please feel free to leave feedback in issues/PRs.
```

### Comparing `cgpt-1.1.29/app/base.py` & `cgpt-1.2.1/app/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Dict
 import click, socket
-from app.file_service import file_prompt
+from app.create_env import file_prompt
 from app.plugin import davinci
 from app.utils.constant import (
     init_conversation,
     ASSISTANT,
     MAX_WIDTH,
     color,
     top_left,
```

### Comparing `cgpt-1.1.29/app/client/main.py` & `cgpt-1.2.1/app/client/main.py`

 * *Files identical despite different names*

### Comparing `cgpt-1.1.29/app/file_service.py` & `cgpt-1.2.1/app/create_env.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,22 @@
     API_KEY_ADDED,
     API_KEY_NOT_ADDED,
     STR_OPENAI_API_KEY,
     color,
 )
 
 
-def file_prompt() -> None:
+def file_prompt(output_path=None) -> None:
     api_key = getpass.getpass(GET_API_KEY)
 
+    if output_path is None:
+        output_path = ""
+
     if api_key:
-        fichier = open(".env", "w")
+        fichier = open(output_path + ".env", "w")
         fichier.close()
-        dotenv.set_key(".env", STR_OPENAI_API_KEY, api_key)
+        dotenv.set_key(output_path + ".env", STR_OPENAI_API_KEY, api_key)
 
         click.echo(colored(API_KEY_ADDED, color))
 
     elif api_key == "" or not api_key:
         click.echo(colored(API_KEY_NOT_ADDED, color))
```

### Comparing `cgpt-1.1.29/app/plugin.py` & `cgpt-1.2.1/app/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import os, click
 from termcolor import colored
 from typing import Union, List, Dict
 import openai
-from app.file_service import file_prompt
+from app.create_env import file_prompt
 from dotenv import load_dotenv
 
 load_dotenv()
 from app.utils.constant import (
     AI_COLON,
     CHOICES,
     STR_OPENAI_API_KEY,
```

### Comparing `cgpt-1.1.29/app/server/main.py` & `cgpt-1.2.1/app/server/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,45 +8,58 @@
 print_lock = threading.Lock()
 from app.plugin import davinci
 from app.utils.constant import (
     PORT,
     SERVER_LIVE,
     UTF,
     LIVE,
+    PING,
+    PONG,
     DECONNECTED_HOST,
     init_conversation,
     error_color,
     color,
 )
 
 
 def threaded(c):
     init_conversation_client = init_conversation
     while True:
         try:
             client_data = c.recv(1024).decode()
 
+            if client_data == PING:
+                c.send(PONG.encode(encoding=UTF))
+
             api_response = davinci(client_data, init_conversation_client)
             if api_response is not None:
                 c.send(api_response.encode(encoding=UTF))
             else:
                 continue
 
         except BrokenPipeError:
             continue
 
         except ConnectionResetError:
             click.echo(colored(DECONNECTED_HOST, error_color))
 
 
-def main():
-    adresse_ip = socket.gethostbyname(socket.gethostname())
-    server_socket = socket.create_server((adresse_ip, int(PORT)), reuse_port=False)
-    server_socket.listen()
-    click.echo(colored(f"{SERVER_LIVE} {adresse_ip} ..{LIVE}", color))
+def main(port, ip_address=None):
+    if ip_address is None:
+        auto_detcted_ip = socket.gethostbyname(socket.gethostname())
+        server_socket = socket.create_server(
+            (auto_detcted_ip, int(port)), reuse_port=False
+        )
+        server_socket.listen()
+        click.echo(colored(f"{SERVER_LIVE} {auto_detcted_ip} ..{LIVE}", color))
+
+    else:
+        server_socket = socket.create_server((ip_address, int(port)), reuse_port=False)
+        server_socket.listen()
+
     while True:
         client, _ = server_socket.accept()
         threading.Thread(target=threaded, args=(client,), daemon=True).start()
 
 
 if __name__ == "__main__":
-    main()
+    main(PORT, None)
```

### Comparing `cgpt-1.1.29/app/utils/constant.py` & `cgpt-1.2.1/app/utils/constant.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import platform
+import platform, os
 
-VERSION = "1.1.29"
+VERSION = "1.2.1"
 SUBTITLE = ">>> Make AI powered search inside your CLI"
 os_name = platform.system()
 
 WELCOME = f"""
 
   /$$$$$$   /$$$$$$  /$$$$$$$  /$$$$$$$$    
  /$$__  $$ /$$__  $$| $$__  $$|__  $$__/ v{VERSION}     
@@ -88,7 +88,9 @@
 NOT_CONNECTED = "You are not connected to the internet.."
 TOO_MUCH_REQUEST = "Too many requests"
 CONNECTION_ERROR = "Connection error: "
 ADDRESS_NOT_VALID = f"The IP address is not valid {NO_ENTRY}"
 DECONNECTED_HOST = "A host has disconnected."
 BOLD = "bold"
 PYTHONSTR = "python"
+PING = "PING"
+PONG = "PONG"
```

### Comparing `cgpt-1.1.29/cgpt.egg-info/PKG-INFO` & `cgpt-1.2.1/cgpt.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 Metadata-Version: 2.1
 Name: cgpt
-Version: 1.1.29
+Version: 1.2.1
 Summary: Use openai chat-gpt on your cli
 Home-page: https://github.com/ainayves/cgpt>
 Author: Aina Yves
 Author-email: randrianaina.yves@gmail.com
 License: MIT
 Description: ![](https://komarev.com/ghpvc/?username=ainayves&color=blueviolet)
         
         ## Use openai chat-gpt on your CLI
         `cgpt` is a Python module that allows you to use Chat-GPT directly in your favorite Terminal.
         
+        ### ⭐ FEATURES
+        
+        - AI conversation exactly the same as in openai website
+        - LAN support (you can use cgpt inside a LAN)
+        - Docker support
+        
         ### REQUIREMENTS
         
         - python >=3.7
         - openai API KEY : 
         
         You need to register on openai to receive your own api key , here : [api_key](https://platform.openai.com/account/api-keys).
         
         ### SETUP
         
         ```
         pip install cgpt
         ```
         
-        ### ⏯️ GET VERSION 
+        ### ⏯️ VERIFY INSTALLATION 
         
         ```
         cgpt-version
         ```
         
         ### 🚀 RUN
         
@@ -52,14 +58,22 @@
         ```
         127.0.0.1	localhost
         127.0.1.1	your-hostanme
         ```
         
         - A `client` can also use his own api_key in the next version.
         
+        ### 🐋 RUN INSIDE DOCKER
+        
+        - To make it easier , use the `docker-compose.yml` file : 
+        
+        ```
+        docker-compose run --rm app
+        ```
+        
         ### GITHUB
         
         - [cgpt](https://github.com/ainayves/cgpt/)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `cgpt-1.1.29/cgpt.py` & `cgpt-1.2.1/cgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import click, os, subprocess
 from termcolor import colored
 from app.main import prompt
-from app.file_service import file_prompt
+from app.create_env import file_prompt
 from app.utils.constant import (
     SERVER_PATH,
     CLIENT_PATH,
     CGPT_NETWORK,
     YOU_SERVER,
     OPEN_TERMINAL,
     WELCOME,
```

### Comparing `cgpt-1.1.29/setup.py` & `cgpt-1.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,16 +23,15 @@
     packages=["app", "app.client", "app.server", "app.utils", "app.commands"],
     install_requires=[
         "setuptools",
         "twine",
         "click>=7.1.2",
         "openai",
         "python-dotenv",
-        "termcolor",
-        "pytest",
+        "termcolor"
     ],
     python_requires=">=3.7",
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
     ],
     entry_points={
```

