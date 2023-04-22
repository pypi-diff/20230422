# Comparing `tmp/dvinfo-0.1.2.tar.gz` & `tmp/dvinfo-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvinfo-0.1.2.tar", last modified: Sat Apr 22 07:25:15 2023, max compression
+gzip compressed data, was "dvinfo-0.2.tar", last modified: Sat Apr 22 07:34:41 2023, max compression
```

## Comparing `dvinfo-0.1.2.tar` & `dvinfo-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 07:25:15.381818 dvinfo-0.1.2/
--rw-rw-rw-   0        0        0      710 2023-04-22 07:25:15.377812 dvinfo-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-22 07:25:15.286286 dvinfo-0.1.2/dvinfo.egg-info/
--rw-rw-rw-   0        0        0      710 2023-04-22 07:25:11.000000 dvinfo-0.1.2/dvinfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-04-22 07:25:12.000000 dvinfo-0.1.2/dvinfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 07:25:11.000000 dvinfo-0.1.2/dvinfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-22 07:25:11.000000 dvinfo-0.1.2/dvinfo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 07:25:11.000000 dvinfo-0.1.2/dvinfo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 07:25:15.383818 dvinfo-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      916 2023-04-22 07:24:38.000000 dvinfo-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 07:34:41.188676 dvinfo-0.2/
+-rw-rw-rw-   0        0        0      708 2023-04-22 07:34:41.183655 dvinfo-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-22 07:34:41.174577 dvinfo-0.2/dvinfo.egg-info/
+-rw-rw-rw-   0        0        0      708 2023-04-22 07:34:37.000000 dvinfo-0.2/dvinfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-04-22 07:34:39.000000 dvinfo-0.2/dvinfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 07:34:37.000000 dvinfo-0.2/dvinfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-22 07:34:37.000000 dvinfo-0.2/dvinfo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 07:34:38.000000 dvinfo-0.2/dvinfo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 07:34:41.189658 dvinfo-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      914 2023-04-22 07:34:10.000000 dvinfo-0.2/setup.py
```

### Comparing `dvinfo-0.1.2/PKG-INFO` & `dvinfo-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvinfo
-Version: 0.1.2
+Version: 0.2
 Summary: A package for getting system information on Windows and Linux
 Home-page: https://github.com/0mgRod/deviceinfo
 Author: OmgRod
 Keywords: system info
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dvinfo-0.1.2/dvinfo.egg-info/PKG-INFO` & `dvinfo-0.2/dvinfo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvinfo
-Version: 0.1.2
+Version: 0.2
 Summary: A package for getting system information on Windows and Linux
 Home-page: https://github.com/0mgRod/deviceinfo
 Author: OmgRod
 Keywords: system info
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dvinfo-0.1.2/setup.py` & `dvinfo-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dvinfo",
-    version="0.1.2",
+    version="0.2",
     description="A package for getting system information on Windows and Linux",
     url="https://github.com/0mgRod/deviceinfo",
     author="OmgRod",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

