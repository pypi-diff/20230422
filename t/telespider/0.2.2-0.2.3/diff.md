# Comparing `tmp/telespider-0.2.2.tar.gz` & `tmp/telespider-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telespider-0.2.2.tar", max compression
+gzip compressed data, was "telespider-0.2.3.tar", max compression
```

## Comparing `telespider-0.2.2.tar` & `telespider-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2023-04-20 08:10:29.039624 telespider-0.2.2/LICENSE
--rw-r--r--   0        0        0      934 2023-04-22 08:18:34.032173 telespider-0.2.2/README.md
--rw-r--r--   0        0        0      592 2023-04-22 09:21:28.359840 telespider-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-22 09:11:54.244843 telespider-0.2.2/telespider/__init__.py
--rw-r--r--   0        0        0     2662 2023-04-22 09:20:41.573975 telespider-0.2.2/telespider/__main__.py
--rw-r--r--   0        0        0     1701 2023-04-22 09:20:55.313815 telespider-0.2.2/telespider/app.py
--rw-r--r--   0        0        0      606 2023-04-22 09:18:16.420398 telespider-0.2.2/telespider/config.py
--rw-r--r--   0        0        0      152 2023-04-19 17:18:45.959480 telespider-0.2.2/telespider/console.py
--rw-r--r--   0        0        0       69 2023-04-22 08:06:36.213270 telespider-0.2.2/telespider/scrapper/__init__.py
--rw-r--r--   0        0        0     2095 2023-04-22 08:36:14.647055 telespider-0.2.2/telespider/scrapper/channel.py
--rw-r--r--   0        0        0     5475 2023-04-22 09:20:55.193817 telespider-0.2.2/telespider/scrapper/scrapper.py
--rw-r--r--   0        0        0      361 2023-04-22 08:47:20.048014 telespider-0.2.2/telespider/scrapper/types.py
--rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 telespider-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-20 08:10:29.039624 telespider-0.2.3/LICENSE
+-rw-r--r--   0        0        0      934 2023-04-22 08:18:34.032173 telespider-0.2.3/README.md
+-rw-r--r--   0        0        0      592 2023-04-22 09:28:37.068328 telespider-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-22 09:11:54.244843 telespider-0.2.3/telespider/__init__.py
+-rw-r--r--   0        0        0     2662 2023-04-22 09:20:41.573975 telespider-0.2.3/telespider/__main__.py
+-rw-r--r--   0        0        0     1701 2023-04-22 09:20:55.313815 telespider-0.2.3/telespider/app.py
+-rw-r--r--   0        0        0      605 2023-04-22 09:28:07.946481 telespider-0.2.3/telespider/config.py
+-rw-r--r--   0        0        0      201 2023-04-22 09:27:51.193158 telespider-0.2.3/telespider/console.py
+-rw-r--r--   0        0        0       69 2023-04-22 08:06:36.213270 telespider-0.2.3/telespider/scrapper/__init__.py
+-rw-r--r--   0        0        0     2095 2023-04-22 08:36:14.647055 telespider-0.2.3/telespider/scrapper/channel.py
+-rw-r--r--   0        0        0     5475 2023-04-22 09:20:55.193817 telespider-0.2.3/telespider/scrapper/scrapper.py
+-rw-r--r--   0        0        0      361 2023-04-22 08:47:20.048014 telespider-0.2.3/telespider/scrapper/types.py
+-rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 telespider-0.2.3/PKG-INFO
```

### Comparing `telespider-0.2.2/LICENSE` & `telespider-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `telespider-0.2.2/README.md` & `telespider-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `telespider-0.2.2/pyproject.toml` & `telespider-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telespider"
-version = "0.2.2"
+version = "0.2.3"
 description = "recursively parsing tg channels"
 authors = ["andrewsap <andrewsapw@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `telespider-0.2.2/telespider/__main__.py` & `telespider-0.2.3/telespider/__main__.py`

 * *Files identical despite different names*

### Comparing `telespider-0.2.2/telespider/app.py` & `telespider-0.2.3/telespider/app.py`

 * *Files identical despite different names*

### Comparing `telespider-0.2.2/telespider/config.py` & `telespider-0.2.3/telespider/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     API_HASH: Optional[str] = None
     API_ID: Optional[str] = None
 
     ENTRYPOINT_CHANNELS: str = ""  # comma separated list of channels
     MAX_PER_CHANNEL: int = 100  # maximum number of messages to parse per channel
 
     AUTO_EXPLORE_CHANNELS: bool = True
-    SILENT: bool = False
+    SILENT: bool = True
 
     # parse .env
     class Config:
         env_file = ROOT_DIR.parent / ".env"
 
 
 settings = Settings()
```

### Comparing `telespider-0.2.2/telespider/scrapper/channel.py` & `telespider-0.2.3/telespider/scrapper/channel.py`

 * *Files identical despite different names*

### Comparing `telespider-0.2.2/telespider/scrapper/scrapper.py` & `telespider-0.2.3/telespider/scrapper/scrapper.py`

 * *Files identical despite different names*

### Comparing `telespider-0.2.2/PKG-INFO` & `telespider-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telespider
-Version: 0.2.2
+Version: 0.2.3
 Summary: recursively parsing tg channels
 License: MIT
 Author: andrewsap
 Author-email: andrewsapw@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

