# Comparing `tmp/dvinfo-0.1.tar.gz` & `tmp/dvinfo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvinfo-0.1.tar", last modified: Sat Apr 22 07:17:49 2023, max compression
+gzip compressed data, was "dvinfo-0.1.1.tar", last modified: Sat Apr 22 07:21:10 2023, max compression
```

## Comparing `dvinfo-0.1.tar` & `dvinfo-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 07:17:48.988659 dvinfo-0.1/
--rw-rw-rw-   0        0        0      708 2023-04-22 07:17:48.918659 dvinfo-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-22 07:17:48.814666 dvinfo-0.1/dvinfo.egg-info/
--rw-rw-rw-   0        0        0      708 2023-04-22 07:17:46.000000 dvinfo-0.1/dvinfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-04-22 07:17:47.000000 dvinfo-0.1/dvinfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 07:17:46.000000 dvinfo-0.1/dvinfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-22 07:17:46.000000 dvinfo-0.1/dvinfo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 07:17:46.000000 dvinfo-0.1/dvinfo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 07:17:48.990654 dvinfo-0.1/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-04-22 07:16:59.000000 dvinfo-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 07:21:10.125755 dvinfo-0.1.1/
+-rw-rw-rw-   0        0        0      710 2023-04-22 07:21:10.094757 dvinfo-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-22 07:21:10.050758 dvinfo-0.1.1/dvinfo.egg-info/
+-rw-rw-rw-   0        0        0      710 2023-04-22 07:21:07.000000 dvinfo-0.1.1/dvinfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-04-22 07:21:08.000000 dvinfo-0.1.1/dvinfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 07:21:07.000000 dvinfo-0.1.1/dvinfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-22 07:21:07.000000 dvinfo-0.1.1/dvinfo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 07:21:07.000000 dvinfo-0.1.1/dvinfo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 07:21:10.126751 dvinfo-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      936 2023-04-22 07:20:33.000000 dvinfo-0.1.1/setup.py
```

### Comparing `dvinfo-0.1/PKG-INFO` & `dvinfo-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvinfo
-Version: 0.1
+Version: 0.1.1
 Summary: A package for getting system information on Windows and Linux
 Home-page: https://github.com/0mgRod/deviceinfo
 Author: OmgRod
 Keywords: system info
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dvinfo-0.1/dvinfo.egg-info/PKG-INFO` & `dvinfo-0.1.1/dvinfo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvinfo
-Version: 0.1
+Version: 0.1.1
 Summary: A package for getting system information on Windows and Linux
 Home-page: https://github.com/0mgRod/deviceinfo
 Author: OmgRod
 Keywords: system info
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dvinfo-0.1/setup.py` & `dvinfo-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dvinfo",
-    version="0.1",
+    version="0.1.1",
     description="A package for getting system information on Windows and Linux",
     url="https://github.com/0mgRod/deviceinfo",
     author="OmgRod",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

