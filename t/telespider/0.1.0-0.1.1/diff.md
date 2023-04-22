# Comparing `tmp/telespider-0.1.0.tar.gz` & `tmp/telespider-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telespider-0.1.0.tar", max compression
+gzip compressed data, was "telespider-0.1.1.tar", max compression
```

## Comparing `telespider-0.1.0.tar` & `telespider-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2023-04-20 08:10:29.039624 telespider-0.1.0/LICENSE
--rw-r--r--   0        0        0     1025 2023-04-20 08:07:36.639629 telespider-0.1.0/README.md
--rw-r--r--   0        0        0      592 2023-04-17 17:57:51.124471 telespider-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       26 2023-04-17 17:49:13.844485 telespider-0.1.0/telespider/__init__.py
--rw-r--r--   0        0        0     2392 2023-04-22 08:11:49.578255 telespider-0.1.0/telespider/__main__.py
--rw-r--r--   0        0        0      287 2023-04-17 17:57:56.434471 telespider-0.1.0/telespider/app.py
--rw-r--r--   0        0        0      538 2023-04-19 16:12:02.069745 telespider-0.1.0/telespider/config.py
--rw-r--r--   0        0        0      152 2023-04-19 17:18:45.959480 telespider-0.1.0/telespider/console.py
--rw-r--r--   0        0        0       69 2023-04-22 08:06:36.213270 telespider-0.1.0/telespider/scrapper/__init__.py
--rw-r--r--   0        0        0     2065 2023-04-22 08:01:16.056546 telespider-0.1.0/telespider/scrapper/channel.py
--rw-r--r--   0        0        0     4886 2023-04-22 08:10:51.262527 telespider-0.1.0/telespider/scrapper/scrapper.py
--rw-r--r--   0        0        0      358 2023-04-22 08:10:51.262527 telespider-0.1.0/telespider/scrapper/types.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 telespider-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-20 08:10:29.039624 telespider-0.1.1/LICENSE
+-rw-r--r--   0        0        0      934 2023-04-22 08:18:34.032173 telespider-0.1.1/README.md
+-rw-r--r--   0        0        0      592 2023-04-22 08:19:38.407063 telespider-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-04-17 17:49:13.844485 telespider-0.1.1/telespider/__init__.py
+-rw-r--r--   0        0        0     2392 2023-04-22 08:11:49.578255 telespider-0.1.1/telespider/__main__.py
+-rw-r--r--   0        0        0      287 2023-04-17 17:57:56.434471 telespider-0.1.1/telespider/app.py
+-rw-r--r--   0        0        0      538 2023-04-19 16:12:02.069745 telespider-0.1.1/telespider/config.py
+-rw-r--r--   0        0        0      152 2023-04-19 17:18:45.959480 telespider-0.1.1/telespider/console.py
+-rw-r--r--   0        0        0       69 2023-04-22 08:06:36.213270 telespider-0.1.1/telespider/scrapper/__init__.py
+-rw-r--r--   0        0        0     2065 2023-04-22 08:01:16.056546 telespider-0.1.1/telespider/scrapper/channel.py
+-rw-r--r--   0        0        0     4886 2023-04-22 08:10:51.262527 telespider-0.1.1/telespider/scrapper/scrapper.py
+-rw-r--r--   0        0        0      358 2023-04-22 08:10:51.262527 telespider-0.1.1/telespider/scrapper/types.py
+-rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 telespider-0.1.1/PKG-INFO
```

### Comparing `telespider-0.1.0/LICENSE` & `telespider-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telespider-0.1.0/pyproject.toml` & `telespider-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telespider"
-version = "0.1.0"
+version = "0.1.1"
 description = "recursively parsing tg channels"
 authors = ["andrewsap <andrewsapw@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `telespider-0.1.0/telespider/__main__.py` & `telespider-0.1.1/telespider/__main__.py`

 * *Files identical despite different names*

### Comparing `telespider-0.1.0/telespider/config.py` & `telespider-0.1.1/telespider/config.py`

 * *Files identical despite different names*

### Comparing `telespider-0.1.0/telespider/scrapper/channel.py` & `telespider-0.1.1/telespider/scrapper/channel.py`

 * *Files identical despite different names*

### Comparing `telespider-0.1.0/telespider/scrapper/scrapper.py` & `telespider-0.1.1/telespider/scrapper/scrapper.py`

 * *Files identical despite different names*

### Comparing `telespider-0.1.0/PKG-INFO` & `telespider-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telespider
-Version: 0.1.0
+Version: 0.1.1
 Summary: recursively parsing tg channels
 License: MIT
 Author: andrewsap
 Author-email: andrewsapw@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,29 +14,28 @@
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyrogram (>=2.0.103,<3.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: tgcrypto (>=1.2.5,<2.0.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Description-Content-Type: text/markdown
 
-# :spider_web: Telegram scrapper
+# 🕸️ Telegram scrapper
 
 Simple package (+ CLI) for scrapping Telegram channel
 
 # Features
 
-:heavy_check_mark: auto explore new channels  
-:heavy_check_mark: search text  
-:heavy_check_mark: search mentions  
+✔️ auto explore new channels  
+✔️ search text  
+✔️ search mentions  
 
 # Usage
 
 ```console
-$ git clone https://github.com/andrewsapw/telespider.git
-$ poetry install
+$ pip install telespider
 $ tspider search -w "stonks" -n 100 # search word `stonks`
 $ tspider search -u "andrewsap" -n 100 # search mentions of user `andrewsap`
 ```
 
 # Configuration
 
 App uses this environment variables:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

