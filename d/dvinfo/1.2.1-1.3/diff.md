# Comparing `tmp/dvinfo-1.2.1.tar.gz` & `tmp/dvinfo-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvinfo-1.2.1.tar", last modified: Sat Apr 22 07:50:38 2023, max compression
+gzip compressed data, was "dvinfo-1.3.tar", last modified: Sat Apr 22 07:52:14 2023, max compression
```

## Comparing `dvinfo-1.2.1.tar` & `dvinfo-1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 07:50:38.763445 dvinfo-1.2.1/
--rw-rw-rw-   0        0        0      506 2023-04-22 07:50:38.705450 dvinfo-1.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-22 07:50:38.631922 dvinfo-1.2.1/dvinfo.egg-info/
--rw-rw-rw-   0        0        0      506 2023-04-22 07:50:35.000000 dvinfo-1.2.1/dvinfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-04-22 07:50:36.000000 dvinfo-1.2.1/dvinfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 07:50:35.000000 dvinfo-1.2.1/dvinfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-04-22 07:50:35.000000 dvinfo-1.2.1/dvinfo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 07:50:35.000000 dvinfo-1.2.1/dvinfo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 07:50:38.764445 dvinfo-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      882 2023-04-22 07:50:12.000000 dvinfo-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 07:52:14.294914 dvinfo-1.3/
+-rw-rw-rw-   0        0        0      504 2023-04-22 07:52:14.281910 dvinfo-1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-22 07:52:14.256370 dvinfo-1.3/dvinfo.egg-info/
+-rw-rw-rw-   0        0        0      504 2023-04-22 07:52:11.000000 dvinfo-1.3/dvinfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-04-22 07:52:12.000000 dvinfo-1.3/dvinfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 07:52:11.000000 dvinfo-1.3/dvinfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-04-22 07:52:11.000000 dvinfo-1.3/dvinfo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 07:52:11.000000 dvinfo-1.3/dvinfo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 07:52:14.298911 dvinfo-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      880 2023-04-22 07:51:46.000000 dvinfo-1.3/setup.py
```

### Comparing `dvinfo-1.2.1/setup.py` & `dvinfo-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dvinfo",
-    version="1.2.1",
+    version="1.3",
     description="A package for getting system information on Windows and Linux",
     url="https://github.com/0mgRod/deviceinfo",
     author="OmgRod",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

