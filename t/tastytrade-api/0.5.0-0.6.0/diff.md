# Comparing `tmp/tastytrade-api-0.5.0.tar.gz` & `tmp/tastytrade-api-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-api-0.5.0.tar", last modified: Sun Apr 16 14:01:56 2023, max compression
+gzip compressed data, was "tastytrade-api-0.6.0.tar", last modified: Sat Apr 22 09:30:21 2023, max compression
```

## Comparing `tastytrade-api-0.5.0.tar` & `tastytrade-api-0.6.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:01:56.949888 tastytrade-api-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 14:01:35.000000 tastytrade-api-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-16 14:01:56.949888 tastytrade-api-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-16 14:01:35.000000 tastytrade-api-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 14:01:56.949888 tastytrade-api-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-16 14:01:35.000000 tastytrade-api-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:01:56.945888 tastytrade-api-0.5.0/tastytrade_api/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 14:01:35.000000 tastytrade-api-0.5.0/tastytrade_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:01:56.949888 tastytrade-api-0.5.0/tastytrade_api/account/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 14:01:35.000000 tastytrade-api-0.5.0/tastytrade_api/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-16 14:01:35.000000 tastytrade-api-0.5.0/tastytrade_api/account/account_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-16 14:01:35.000000 tastytrade-api-0.5.0/tastytrade_api/account/balances_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-16 14:01:35.000000 tastytrade-api-0.5.0/tastytrade_api/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:01:56.949888 tastytrade-api-0.5.0/tastytrade_api/market_data/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 14:01:35.000000 tastytrade-api-0.5.0/tastytrade_api/market_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16855 2023-04-16 14:01:35.000000 tastytrade-api-0.5.0/tastytrade_api/market_data/instruments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:01:56.949888 tastytrade-api-0.5.0/tastytrade_api/streamer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 14:01:35.000000 tastytrade-api-0.5.0/tastytrade_api/streamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-16 14:01:35.000000 tastytrade-api-0.5.0/tastytrade_api/streamer/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-16 14:01:35.000000 tastytrade-api-0.5.0/tastytrade_api/symbology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:01:56.945888 tastytrade-api-0.5.0/tastytrade_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-16 14:01:56.000000 tastytrade-api-0.5.0/tastytrade_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-16 14:01:56.000000 tastytrade-api-0.5.0/tastytrade_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 14:01:56.000000 tastytrade-api-0.5.0/tastytrade_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 14:01:56.000000 tastytrade-api-0.5.0/tastytrade_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-16 14:01:56.000000 tastytrade-api-0.5.0/tastytrade_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:01:56.949888 tastytrade-api-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 14:01:35.000000 tastytrade-api-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-16 14:01:35.000000 tastytrade-api-0.5.0/tests/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:30:21.722963 tastytrade-api-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-22 09:30:21.722963 tastytrade-api-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 09:30:21.722963 tastytrade-api-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:30:21.718963 tastytrade-api-0.6.0/tastytrade_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/tastytrade_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:30:21.718963 tastytrade-api-0.6.0/tastytrade_api/account/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/tastytrade_api/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/tastytrade_api/account/account_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/tastytrade_api/account/balances_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/tastytrade_api/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:30:21.718963 tastytrade-api-0.6.0/tastytrade_api/market_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/tastytrade_api/market_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16855 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/tastytrade_api/market_data/instruments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:30:21.722963 tastytrade-api-0.6.0/tastytrade_api/streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/tastytrade_api/streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/tastytrade_api/streamer/dx_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/tastytrade_api/streamer/dxfeed_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/tastytrade_api/streamer/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/tastytrade_api/symbology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:30:21.718963 tastytrade-api-0.6.0/tastytrade_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-22 09:30:21.000000 tastytrade-api-0.6.0/tastytrade_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-22 09:30:21.000000 tastytrade-api-0.6.0/tastytrade_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:30:21.000000 tastytrade-api-0.6.0/tastytrade_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-22 09:30:21.000000 tastytrade-api-0.6.0/tastytrade_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-22 09:30:21.000000 tastytrade-api-0.6.0/tastytrade_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:30:21.722963 tastytrade-api-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-22 09:30:01.000000 tastytrade-api-0.6.0/tests/test_authentication.py
```

### Comparing `tastytrade-api-0.5.0/PKG-INFO` & `tastytrade-api-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-api
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python client for the Tastytrade API
 Home-page: https://github.com/peter-oroszvari/tastytrade-api
 Author: Peter Oroszvari
 Author-email: peter@oroszvari.hu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tastytrade-api-0.5.0/README.md` & `tastytrade-api-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.5.0/setup.py` & `tastytrade-api-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tastytrade-api",
-    version="0.5.0",
+    version="0.6.0",
     author="Peter Oroszvari",
     author_email="peter@oroszvari.hu",
     description="A Python client for the Tastytrade API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/peter-oroszvari/tastytrade-api",
     packages=find_packages(),
```

### Comparing `tastytrade-api-0.5.0/tastytrade_api/account/account_handler.py` & `tastytrade-api-0.6.0/tastytrade_api/account/account_handler.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.5.0/tastytrade_api/account/balances_positions.py` & `tastytrade-api-0.6.0/tastytrade_api/account/balances_positions.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.5.0/tastytrade_api/authentication.py` & `tastytrade-api-0.6.0/tastytrade_api/authentication.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.5.0/tastytrade_api/market_data/instruments.py` & `tastytrade-api-0.6.0/tastytrade_api/market_data/instruments.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.5.0/tastytrade_api/streamer/streamer.py` & `tastytrade-api-0.6.0/tastytrade_api/streamer/streamer.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.5.0/tastytrade_api/symbology.py` & `tastytrade-api-0.6.0/tastytrade_api/symbology.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.5.0/tastytrade_api.egg-info/PKG-INFO` & `tastytrade-api-0.6.0/tastytrade_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-api
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python client for the Tastytrade API
 Home-page: https://github.com/peter-oroszvari/tastytrade-api
 Author: Peter Oroszvari
 Author-email: peter@oroszvari.hu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tastytrade-api-0.5.0/tastytrade_api.egg-info/SOURCES.txt` & `tastytrade-api-0.6.0/tastytrade_api.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,10 +11,12 @@
 tastytrade_api.egg-info/top_level.txt
 tastytrade_api/account/__init__.py
 tastytrade_api/account/account_handler.py
 tastytrade_api/account/balances_positions.py
 tastytrade_api/market_data/__init__.py
 tastytrade_api/market_data/instruments.py
 tastytrade_api/streamer/__init__.py
+tastytrade_api/streamer/dx_mapping.py
+tastytrade_api/streamer/dxfeed_handler.py
 tastytrade_api/streamer/streamer.py
 tests/__init__.py
 tests/test_authentication.py
```

### Comparing `tastytrade-api-0.5.0/tests/test_authentication.py` & `tastytrade-api-0.6.0/tests/test_authentication.py`

 * *Files identical despite different names*

