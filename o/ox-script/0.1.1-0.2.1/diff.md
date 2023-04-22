# Comparing `tmp/ox-script-0.1.1.tar.gz` & `tmp/ox-script-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ox-script-0.1.1.tar", last modified: Sat Apr 22 17:34:46 2023, max compression
+gzip compressed data, was "dist/ox-script-0.2.1.tar", last modified: Sat Apr 22 17:42:56 2023, max compression
```

## Comparing `ox-script-0.1.1.tar` & `ox-script-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 17:34:46.000000 ox-script-0.1.1/
--rw-r--r--   0 jarvislu   (501) staff       (20)      725 2023-04-22 17:34:46.000000 ox-script-0.1.1/PKG-INFO
--rw-r--r--   0 jarvislu   (501) staff       (20)       23 2023-04-22 17:20:19.000000 ox-script-0.1.1/__init__.py
--rw-------   0 jarvislu   (501) staff       (20)    38368 2023-04-22 17:09:09.000000 ox-script-0.1.1/pskfunc.py
--rw-r--r--   0 jarvislu   (501) staff       (20)       13 2023-04-22 17:32:02.000000 ox-script-0.1.1/MANIFEST.in
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 17:34:46.000000 ox-script-0.1.1/ox_script.egg-info/
--rw-r--r--   0 jarvislu   (501) staff       (20)      725 2023-04-22 17:34:46.000000 ox-script-0.1.1/ox_script.egg-info/PKG-INFO
--rw-r--r--   0 jarvislu   (501) staff       (20)      207 2023-04-22 17:34:46.000000 ox-script-0.1.1/ox_script.egg-info/SOURCES.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)       29 2023-04-22 17:34:46.000000 ox-script-0.1.1/ox_script.egg-info/requires.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)        1 2023-04-22 17:34:46.000000 ox-script-0.1.1/ox_script.egg-info/top_level.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)        1 2023-04-22 17:34:46.000000 ox-script-0.1.1/ox_script.egg-info/dependency_links.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)      903 2023-04-22 17:34:27.000000 ox-script-0.1.1/setup.py
--rw-r--r--   0 jarvislu   (501) staff       (20)       38 2023-04-22 17:34:46.000000 ox-script-0.1.1/setup.cfg
+drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 17:42:56.000000 ox-script-0.2.1/
+-rw-r--r--   0 jarvislu   (501) staff       (20)      725 2023-04-22 17:42:56.000000 ox-script-0.2.1/PKG-INFO
+-rw-r--r--   0 jarvislu   (501) staff       (20)       23 2023-04-22 17:20:19.000000 ox-script-0.2.1/__init__.py
+-rw-------   0 jarvislu   (501) staff       (20)    38368 2023-04-22 17:09:09.000000 ox-script-0.2.1/pskfunc.py
+-rw-r--r--   0 jarvislu   (501) staff       (20)       13 2023-04-22 17:32:02.000000 ox-script-0.2.1/MANIFEST.in
+drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 17:42:56.000000 ox-script-0.2.1/ox_script.egg-info/
+-rw-r--r--   0 jarvislu   (501) staff       (20)      725 2023-04-22 17:42:56.000000 ox-script-0.2.1/ox_script.egg-info/PKG-INFO
+-rw-r--r--   0 jarvislu   (501) staff       (20)      207 2023-04-22 17:42:56.000000 ox-script-0.2.1/ox_script.egg-info/SOURCES.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)       16 2023-04-22 17:42:56.000000 ox-script-0.2.1/ox_script.egg-info/requires.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)        1 2023-04-22 17:42:56.000000 ox-script-0.2.1/ox_script.egg-info/top_level.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)        1 2023-04-22 17:42:56.000000 ox-script-0.2.1/ox_script.egg-info/dependency_links.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)      857 2023-04-22 17:42:53.000000 ox-script-0.2.1/setup.py
+-rw-r--r--   0 jarvislu   (501) staff       (20)       38 2023-04-22 17:42:56.000000 ox-script-0.2.1/setup.cfg
```

### Comparing `ox-script-0.1.1/PKG-INFO` & `ox-script-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: ox-script
-Version: 0.1.1
+Version: 0.2.1
 Summary: The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
 Most printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your ide of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. 
 Home-page: https://github.com/POSTEK-OX-Script
 Author: Jarvis Lu
 Author-email: jarvis.lu@postekus.com
 License: MIT
 Description: UNKNOWN
```

### Comparing `ox-script-0.1.1/pskfunc.py` & `ox-script-0.2.1/pskfunc.py`

 * *Files identical despite different names*

### Comparing `ox-script-0.1.1/ox_script.egg-info/PKG-INFO` & `ox-script-0.2.1/ox_script.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: ox-script
-Version: 0.1.1
+Version: 0.2.1
 Summary: The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
 Most printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your ide of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. 
 Home-page: https://github.com/POSTEK-OX-Script
 Author: Jarvis Lu
 Author-email: jarvis.lu@postekus.com
 License: MIT
 Description: UNKNOWN
```

### Comparing `ox-script-0.1.1/setup.py` & `ox-script-0.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ox-script',
-    version='0.1.1',
+    version='0.2.1',
     author='Jarvis Lu',
     author_email='jarvis.lu@postekus.com',
     packages=find_packages(),
     license="MIT",
     description="The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.\nMost printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your ide of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. ",
     url="https://github.com/POSTEK-OX-Script",
     install_requires=[
-        "re",
         "pandas",
         "openpyxl",
-        "string",
-        "os",
     ],
 )
```

