# Comparing `tmp/cgpt-1.2.1.tar.gz` & `tmp/cgpt-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgpt-1.2.1.tar", last modified: Sat Apr 22 14:10:42 2023, max compression
+gzip compressed data, was "cgpt-1.2.2.tar", last modified: Sat Apr 22 15:07:39 2023, max compression
```

## Comparing `cgpt-1.2.1.tar` & `cgpt-1.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 14:10:42.364016 cgpt-1.2.1/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1065 2023-03-17 13:19:22.000000 cgpt-1.2.1/LICENSE
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       15 2023-03-17 13:19:22.000000 cgpt-1.2.1/MANIFEST.in
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2346 2023-04-22 14:10:42.364016 cgpt-1.2.1/PKG-INFO
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2202 2023-04-20 08:44:37.000000 cgpt-1.2.1/README.md
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 14:10:42.360016 cgpt-1.2.1/app/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-17 13:58:28.000000 cgpt-1.2.1/app/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     3550 2023-04-17 18:29:03.000000 cgpt-1.2.1/app/base.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 14:10:42.360016 cgpt-1.2.1/app/client/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.2.1/app/client/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1419 2023-04-14 13:20:28.000000 cgpt-1.2.1/app/client/main.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 14:10:42.360016 cgpt-1.2.1/app/commands/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-14 13:55:23.000000 cgpt-1.2.1/app/commands/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      110 2023-04-15 17:02:26.000000 cgpt-1.2.1/app/commands/main.py
--rw-r--r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      670 2023-04-17 18:29:03.000000 cgpt-1.2.1/app/create_env.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      406 2023-04-12 19:52:50.000000 cgpt-1.2.1/app/main.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1430 2023-04-17 18:29:03.000000 cgpt-1.2.1/app/plugin.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 14:10:42.360016 cgpt-1.2.1/app/server/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.2.1/app/server/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1631 2023-04-17 18:29:03.000000 cgpt-1.2.1/app/server/main.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 14:10:42.360016 cgpt-1.2.1/app/utils/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.2.1/app/utils/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2771 2023-04-22 14:10:36.000000 cgpt-1.2.1/app/utils/constant.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      135 2023-04-17 18:29:03.000000 cgpt-1.2.1/app/utils/verify_env.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 14:10:42.364016 cgpt-1.2.1/cgpt.egg-info/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2346 2023-04-22 14:10:42.000000 cgpt-1.2.1/cgpt.egg-info/PKG-INFO
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      486 2023-04-22 14:10:42.000000 cgpt-1.2.1/cgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        1 2023-04-22 14:10:42.000000 cgpt-1.2.1/cgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       77 2023-04-22 14:10:42.000000 cgpt-1.2.1/cgpt.egg-info/entry_points.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       61 2023-04-22 14:10:42.000000 cgpt-1.2.1/cgpt.egg-info/requires.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        9 2023-04-22 14:10:42.000000 cgpt-1.2.1/cgpt.egg-info/top_level.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      982 2023-04-17 18:29:03.000000 cgpt-1.2.1/cgpt.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       38 2023-04-22 14:10:42.364016 cgpt-1.2.1/setup.cfg
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1114 2023-04-20 07:35:36.000000 cgpt-1.2.1/setup.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 15:07:39.784039 cgpt-1.2.2/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1065 2023-03-17 13:19:22.000000 cgpt-1.2.2/LICENSE
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       15 2023-03-17 13:19:22.000000 cgpt-1.2.2/MANIFEST.in
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2141 2023-04-22 15:07:39.784039 cgpt-1.2.2/PKG-INFO
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2202 2023-04-22 14:56:41.000000 cgpt-1.2.2/README.md
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 15:07:39.780039 cgpt-1.2.2/app/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-17 13:58:28.000000 cgpt-1.2.2/app/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     3550 2023-04-17 18:29:03.000000 cgpt-1.2.2/app/base.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 15:07:39.780039 cgpt-1.2.2/app/client/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.2.2/app/client/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1419 2023-04-14 13:20:28.000000 cgpt-1.2.2/app/client/main.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 15:07:39.780039 cgpt-1.2.2/app/commands/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-14 13:55:23.000000 cgpt-1.2.2/app/commands/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      110 2023-04-15 17:02:26.000000 cgpt-1.2.2/app/commands/main.py
+-rw-r--r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      670 2023-04-17 18:29:03.000000 cgpt-1.2.2/app/create_env.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      406 2023-04-12 19:52:50.000000 cgpt-1.2.2/app/main.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1430 2023-04-17 18:29:03.000000 cgpt-1.2.2/app/plugin.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 15:07:39.784039 cgpt-1.2.2/app/server/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.2.2/app/server/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1631 2023-04-17 18:29:03.000000 cgpt-1.2.2/app/server/main.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 15:07:39.784039 cgpt-1.2.2/app/utils/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.2.2/app/utils/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2767 2023-04-22 15:07:03.000000 cgpt-1.2.2/app/utils/constant.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      135 2023-04-17 18:29:03.000000 cgpt-1.2.2/app/utils/verify_env.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-22 15:07:39.784039 cgpt-1.2.2/cgpt.egg-info/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2141 2023-04-22 15:07:39.000000 cgpt-1.2.2/cgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      486 2023-04-22 15:07:39.000000 cgpt-1.2.2/cgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        1 2023-04-22 15:07:39.000000 cgpt-1.2.2/cgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       77 2023-04-22 15:07:39.000000 cgpt-1.2.2/cgpt.egg-info/entry_points.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       61 2023-04-22 15:07:39.000000 cgpt-1.2.2/cgpt.egg-info/requires.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        9 2023-04-22 15:07:39.000000 cgpt-1.2.2/cgpt.egg-info/top_level.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      982 2023-04-17 18:29:03.000000 cgpt-1.2.2/cgpt.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       38 2023-04-22 15:07:39.788039 cgpt-1.2.2/setup.cfg
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1114 2023-04-22 14:56:41.000000 cgpt-1.2.2/setup.py
```

### Comparing `cgpt-1.2.1/LICENSE` & `cgpt-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cgpt-1.2.1/PKG-INFO` & `cgpt-1.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: cgpt
-Version: 1.2.1
+Version: 1.2.2
 Summary: Use openai chat-gpt on your cli
 Home-page: https://github.com/ainayves/cgpt>
 Author: Aina Yves
 Author-email: randrianaina.yves@gmail.com
 License: MIT
 Description: ![](https://komarev.com/ghpvc/?username=ainayves&color=blueviolet)
         
         ## Use openai chat-gpt on your CLI
         `cgpt` is a Python module that allows you to use Chat-GPT directly in your favorite Terminal.
         
         ### ⭐ FEATURES
         
         - AI conversation exactly the same as in openai website
         - LAN support (you can use cgpt inside a LAN)
-        - Docker support
         
         ### REQUIREMENTS
         
         - python >=3.7
         - openai API KEY : 
         
         You need to register on openai to receive your own api key , here : [api_key](https://platform.openai.com/account/api-keys).
@@ -58,21 +57,14 @@
         ```
         127.0.0.1	localhost
         127.0.1.1	your-hostanme
         ```
         
         - A `client` can also use his own api_key in the next version.
         
-        ### 🐋 RUN INSIDE DOCKER
-        
-        - To make it easier , use the `docker-compose.yml` file : 
-        
-        ```
-        docker-compose run --rm app
-        ```
         
         ### GITHUB
         
         - [cgpt](https://github.com/ainayves/cgpt/)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cgpt-1.2.1/README.md` & `cgpt-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cgpt-1.2.1/app/base.py` & `cgpt-1.2.2/app/base.py`

 * *Files identical despite different names*

### Comparing `cgpt-1.2.1/app/client/main.py` & `cgpt-1.2.2/app/client/main.py`

 * *Files identical despite different names*

### Comparing `cgpt-1.2.1/app/create_env.py` & `cgpt-1.2.2/app/create_env.py`

 * *Files identical despite different names*

### Comparing `cgpt-1.2.1/app/plugin.py` & `cgpt-1.2.2/app/plugin.py`

 * *Files identical despite different names*

### Comparing `cgpt-1.2.1/app/server/main.py` & `cgpt-1.2.2/app/server/main.py`

 * *Files identical despite different names*

### Comparing `cgpt-1.2.1/app/utils/constant.py` & `cgpt-1.2.2/app/utils/constant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import platform, os
+import platform
 
-VERSION = "1.2.1"
+VERSION = "1.2.2"
 SUBTITLE = ">>> Make AI powered search inside your CLI"
 os_name = platform.system()
 
 WELCOME = f"""
 
   /$$$$$$   /$$$$$$  /$$$$$$$  /$$$$$$$$    
  /$$__  $$ /$$__  $$| $$__  $$|__  $$__/ v{VERSION}
```

### Comparing `cgpt-1.2.1/cgpt.egg-info/PKG-INFO` & `cgpt-1.2.2/cgpt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: cgpt
-Version: 1.2.1
+Version: 1.2.2
 Summary: Use openai chat-gpt on your cli
 Home-page: https://github.com/ainayves/cgpt>
 Author: Aina Yves
 Author-email: randrianaina.yves@gmail.com
 License: MIT
 Description: ![](https://komarev.com/ghpvc/?username=ainayves&color=blueviolet)
         
         ## Use openai chat-gpt on your CLI
         `cgpt` is a Python module that allows you to use Chat-GPT directly in your favorite Terminal.
         
         ### ⭐ FEATURES
         
         - AI conversation exactly the same as in openai website
         - LAN support (you can use cgpt inside a LAN)
-        - Docker support
         
         ### REQUIREMENTS
         
         - python >=3.7
         - openai API KEY : 
         
         You need to register on openai to receive your own api key , here : [api_key](https://platform.openai.com/account/api-keys).
@@ -58,21 +57,14 @@
         ```
         127.0.0.1	localhost
         127.0.1.1	your-hostanme
         ```
         
         - A `client` can also use his own api_key in the next version.
         
-        ### 🐋 RUN INSIDE DOCKER
-        
-        - To make it easier , use the `docker-compose.yml` file : 
-        
-        ```
-        docker-compose run --rm app
-        ```
         
         ### GITHUB
         
         - [cgpt](https://github.com/ainayves/cgpt/)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cgpt-1.2.1/cgpt.py` & `cgpt-1.2.2/cgpt.py`

 * *Files identical despite different names*

### Comparing `cgpt-1.2.1/setup.py` & `cgpt-1.2.2/setup.py`

 * *Files identical despite different names*

