# Comparing `tmp/pyeasee-0.7.51.tar.gz` & `tmp/pyeasee-0.7.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeasee-0.7.51.tar", last modified: Thu Apr  6 21:35:25 2023, max compression
+gzip compressed data, was "pyeasee-0.7.52.tar", last modified: Sat Apr 22 20:13:58 2023, max compression
```

## Comparing `pyeasee-0.7.51.tar` & `pyeasee-0.7.52.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2023-04-06 21:35:25.435674 pyeasee-0.7.51/
--rw-rw-r--   0 olal      (1000) olal      (1000)     3319 2023-04-06 21:35:25.435674 pyeasee-0.7.51/PKG-INFO
--rw-rw-r--   0 olal      (1000) olal      (1000)     2299 2022-10-12 21:10:32.000000 pyeasee-0.7.51/README.md
-drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2023-04-06 21:35:25.431674 pyeasee-0.7.51/pyeasee/
--rw-rw-r--   0 olal      (1000) olal      (1000)      185 2022-12-18 22:29:13.000000 pyeasee-0.7.51/pyeasee/__init__.py
--rw-rw-r--   0 olal      (1000) olal      (1000)    13505 2023-04-06 21:27:23.000000 pyeasee-0.7.51/pyeasee/__main__.py
--rw-rw-r--   0 olal      (1000) olal      (1000)    19443 2023-04-06 21:27:23.000000 pyeasee-0.7.51/pyeasee/charger.py
--rw-rw-r--   0 olal      (1000) olal      (1000)    29599 2023-04-06 21:27:23.000000 pyeasee-0.7.51/pyeasee/const.py
--rw-rw-r--   0 olal      (1000) olal      (1000)    16783 2023-04-06 21:28:11.000000 pyeasee-0.7.51/pyeasee/easee.py
--rw-rw-r--   0 olal      (1000) olal      (1000)      776 2022-12-17 23:49:14.000000 pyeasee-0.7.51/pyeasee/exceptions.py
--rw-rw-r--   0 olal      (1000) olal      (1000)     8707 2023-04-06 21:27:23.000000 pyeasee-0.7.51/pyeasee/site.py
--rw-rw-r--   0 olal      (1000) olal      (1000)     2130 2022-12-18 22:29:13.000000 pyeasee-0.7.51/pyeasee/utils.py
-drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2023-04-06 21:35:25.435674 pyeasee-0.7.51/pyeasee.egg-info/
--rw-rw-r--   0 olal      (1000) olal      (1000)     3319 2023-04-06 21:35:24.000000 pyeasee-0.7.51/pyeasee.egg-info/PKG-INFO
--rw-rw-r--   0 olal      (1000) olal      (1000)      364 2023-04-06 21:35:24.000000 pyeasee-0.7.51/pyeasee.egg-info/SOURCES.txt
--rw-rw-r--   0 olal      (1000) olal      (1000)        1 2023-04-06 21:35:24.000000 pyeasee-0.7.51/pyeasee.egg-info/dependency_links.txt
--rw-rw-r--   0 olal      (1000) olal      (1000)       51 2023-04-06 21:35:24.000000 pyeasee-0.7.51/pyeasee.egg-info/entry_points.txt
--rw-rw-r--   0 olal      (1000) olal      (1000)       27 2023-04-06 21:35:24.000000 pyeasee-0.7.51/pyeasee.egg-info/requires.txt
--rw-rw-r--   0 olal      (1000) olal      (1000)        8 2023-04-06 21:35:24.000000 pyeasee-0.7.51/pyeasee.egg-info/top_level.txt
--rw-rw-r--   0 olal      (1000) olal      (1000)      169 2023-04-06 21:35:25.435674 pyeasee-0.7.51/setup.cfg
--rw-rw-r--   0 olal      (1000) olal      (1000)      805 2023-04-06 21:28:11.000000 pyeasee-0.7.51/setup.py
+drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2023-04-22 20:13:58.413156 pyeasee-0.7.52/
+-rw-rw-r--   0 olal      (1000) olal      (1000)     3319 2023-04-22 20:13:58.413156 pyeasee-0.7.52/PKG-INFO
+-rw-rw-r--   0 olal      (1000) olal      (1000)     2299 2022-10-12 21:10:32.000000 pyeasee-0.7.52/README.md
+drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2023-04-22 20:13:58.409156 pyeasee-0.7.52/pyeasee/
+-rw-rw-r--   0 olal      (1000) olal      (1000)      185 2022-12-18 22:29:13.000000 pyeasee-0.7.52/pyeasee/__init__.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)    13505 2023-04-06 21:27:23.000000 pyeasee-0.7.52/pyeasee/__main__.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)    19443 2023-04-06 21:27:23.000000 pyeasee-0.7.52/pyeasee/charger.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)    29599 2023-04-06 21:27:23.000000 pyeasee-0.7.52/pyeasee/const.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)    16785 2023-04-22 20:11:43.000000 pyeasee-0.7.52/pyeasee/easee.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)      776 2022-12-17 23:49:14.000000 pyeasee-0.7.52/pyeasee/exceptions.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)     8707 2023-04-06 21:27:23.000000 pyeasee-0.7.52/pyeasee/site.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)     2130 2022-12-18 22:29:13.000000 pyeasee-0.7.52/pyeasee/utils.py
+drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2023-04-22 20:13:58.413156 pyeasee-0.7.52/pyeasee.egg-info/
+-rw-rw-r--   0 olal      (1000) olal      (1000)     3319 2023-04-22 20:13:52.000000 pyeasee-0.7.52/pyeasee.egg-info/PKG-INFO
+-rw-rw-r--   0 olal      (1000) olal      (1000)      364 2023-04-22 20:13:53.000000 pyeasee-0.7.52/pyeasee.egg-info/SOURCES.txt
+-rw-rw-r--   0 olal      (1000) olal      (1000)        1 2023-04-22 20:13:52.000000 pyeasee-0.7.52/pyeasee.egg-info/dependency_links.txt
+-rw-rw-r--   0 olal      (1000) olal      (1000)       51 2023-04-22 20:13:52.000000 pyeasee-0.7.52/pyeasee.egg-info/entry_points.txt
+-rw-rw-r--   0 olal      (1000) olal      (1000)       27 2023-04-22 20:13:52.000000 pyeasee-0.7.52/pyeasee.egg-info/requires.txt
+-rw-rw-r--   0 olal      (1000) olal      (1000)        8 2023-04-22 20:13:52.000000 pyeasee-0.7.52/pyeasee.egg-info/top_level.txt
+-rw-rw-r--   0 olal      (1000) olal      (1000)      169 2023-04-22 20:13:58.413156 pyeasee-0.7.52/setup.cfg
+-rw-rw-r--   0 olal      (1000) olal      (1000)      805 2023-04-22 20:11:43.000000 pyeasee-0.7.52/setup.py
```

### Comparing `pyeasee-0.7.51/PKG-INFO` & `pyeasee-0.7.52/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeasee
-Version: 0.7.51
+Version: 0.7.52
 Summary: Easee EV charger API library
 Home-page: https://github.com/fondberg/pyeasee
 Author: Niklas Fondberg
 Author-email: niklas.fondberg@gmail.com
 License: MIT
 Description: ![Maintenance](https://img.shields.io/maintenance/yes/2022.svg) ![Easee library](https://github.com/fondberg/easee/workflows/Easee%20library/badge.svg)
```

### Comparing `pyeasee-0.7.51/README.md` & `pyeasee-0.7.52/README.md`

 * *Files identical despite different names*

### Comparing `pyeasee-0.7.51/pyeasee/__main__.py` & `pyeasee-0.7.52/pyeasee/__main__.py`

 * *Files identical despite different names*

### Comparing `pyeasee-0.7.51/pyeasee/charger.py` & `pyeasee-0.7.52/pyeasee/charger.py`

 * *Files identical despite different names*

### Comparing `pyeasee-0.7.51/pyeasee/const.py` & `pyeasee-0.7.52/pyeasee/const.py`

 * *Files identical despite different names*

### Comparing `pyeasee-0.7.51/pyeasee/easee.py` & `pyeasee-0.7.52/pyeasee/easee.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     NotFoundException,
     ServerFailureException,
     TooManyRequestsException,
 )
 from .site import Site, SiteState
 from .utils import convert_stream_data
 
-__VERSION__ = "0.7.51"
+__VERSION__ = "0.7.52"
 
 _LOGGER = logging.getLogger(__name__)
 
 SR_MIN_BACKOFF = 0
 SR_MAX_BACKOFF = 300
 SR_INC_BACKOFF = 30
 
@@ -78,15 +78,15 @@
         self.username = username
         self.password = password
         self.external_session = True if session else False
 
         _LOGGER.info("Easee python library version: %s", __VERSION__)
 
         self.base = ["https://api.easee.cloud", "https://api.easee.com"]
-        self.sr_base = "https://api.easee.cloud/hubs/chargers"
+        self.sr_base = "https://streams.easee.com/hubs/chargers"
         self.token = {}
         self.headers = {
             "User-Agent": f"pyeasee/{__VERSION__} REST client",
             "Accept": "application/json",
             "Content-Type": "application/json;charset=UTF-8",
         }
         self.minimal_headers = self.headers
```

### Comparing `pyeasee-0.7.51/pyeasee/exceptions.py` & `pyeasee-0.7.52/pyeasee/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyeasee-0.7.51/pyeasee/site.py` & `pyeasee-0.7.52/pyeasee/site.py`

 * *Files identical despite different names*

### Comparing `pyeasee-0.7.51/pyeasee/utils.py` & `pyeasee-0.7.52/pyeasee/utils.py`

 * *Files identical despite different names*

### Comparing `pyeasee-0.7.51/pyeasee.egg-info/PKG-INFO` & `pyeasee-0.7.52/pyeasee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeasee
-Version: 0.7.51
+Version: 0.7.52
 Summary: Easee EV charger API library
 Home-page: https://github.com/fondberg/pyeasee
 Author: Niklas Fondberg
 Author-email: niklas.fondberg@gmail.com
 License: MIT
 Description: ![Maintenance](https://img.shields.io/maintenance/yes/2022.svg) ![Easee library](https://github.com/fondberg/easee/workflows/Easee%20library/badge.svg)
```

### Comparing `pyeasee-0.7.51/setup.py` & `pyeasee-0.7.52/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os.path
 from setuptools import setup
 
 # This call to setup() does all the work
 setup(
     name="pyeasee",
-    version="0.7.51",
+    version="0.7.52",
     description="Easee EV charger API library",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/fondberg/pyeasee",
     author="Niklas Fondberg",
     author_email="niklas.fondberg@gmail.com",
     license="MIT",
```

