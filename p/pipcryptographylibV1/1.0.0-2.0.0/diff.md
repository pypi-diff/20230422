# Comparing `tmp/pipcryptographylibV1-1.0.0.tar.gz` & `tmp/pipcryptographylibV1-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcryptographylibV1-1.0.0.tar", last modified: Fri Apr 21 16:58:55 2023, max compression
+gzip compressed data, was "pipcryptographylibV1-2.0.0.tar", last modified: Sat Apr 22 00:27:20 2023, max compression
```

## Comparing `pipcryptographylibV1-1.0.0.tar` & `pipcryptographylibV1-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:58:55.604296 pipcryptographylibV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      328 2023-04-21 16:58:55.604296 pipcryptographylibV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:58:55.604296 pipcryptographylibV1-1.0.0/pipcryptographylibV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-21 16:58:55.000000 pipcryptographylibV1-1.0.0/pipcryptographylibV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:58:55.604296 pipcryptographylibV1-1.0.0/pipcryptographylibV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      328 2023-04-21 16:58:55.000000 pipcryptographylibV1-1.0.0/pipcryptographylibV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2023-04-21 16:58:55.000000 pipcryptographylibV1-1.0.0/pipcryptographylibV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 16:58:55.000000 pipcryptographylibV1-1.0.0/pipcryptographylibV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-21 16:58:55.000000 pipcryptographylibV1-1.0.0/pipcryptographylibV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 16:58:55.604296 pipcryptographylibV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      541 2023-04-21 16:58:54.000000 pipcryptographylibV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 00:27:20.081591 pipcryptographylibV1-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-04-22 00:27:20.081591 pipcryptographylibV1-2.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 00:27:20.081591 pipcryptographylibV1-2.0.0/pipcryptographylibV1/
+-rw-r--r--   0 root         (0) root         (0)    70957 2023-04-22 00:27:19.000000 pipcryptographylibV1-2.0.0/pipcryptographylibV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 00:27:20.081591 pipcryptographylibV1-2.0.0/pipcryptographylibV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-04-22 00:27:20.000000 pipcryptographylibV1-2.0.0/pipcryptographylibV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-04-22 00:27:20.000000 pipcryptographylibV1-2.0.0/pipcryptographylibV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 00:27:20.000000 pipcryptographylibV1-2.0.0/pipcryptographylibV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-22 00:27:20.000000 pipcryptographylibV1-2.0.0/pipcryptographylibV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 00:27:20.081591 pipcryptographylibV1-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      638 2023-04-22 00:27:19.000000 pipcryptographylibV1-2.0.0/setup.py
```

### Comparing `pipcryptographylibV1-1.0.0/setup.py` & `pipcryptographylibV1-2.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
-DESCRIPTION = "Hello World"
-LONG_DESCRIPTION = "Hello World"
+VERSION = '2.0.0'
+DESCRIPTION = "A Modern Python Package to Handle color and hex in Python."
+LONG_DESCRIPTION = "A Modern Python Package to Handle color and hex in Python."
 
 # Setting up
 setup(
     name="pipcryptographylibV1",
     version=VERSION,
-    author="NHJonas",
+    author="knwnLegend",
     author_email="nick.faltermeier@gmx.de",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python'],
```

