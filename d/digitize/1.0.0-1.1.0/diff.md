# Comparing `tmp/digitize-1.0.0.tar.gz` & `tmp/digitize-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitize-1.0.0.tar", last modified: Sat Apr 22 12:54:56 2023, max compression
+gzip compressed data, was "digitize-1.1.0.tar", last modified: Sat Apr 22 13:21:47 2023, max compression
```

## Comparing `digitize-1.0.0.tar` & `digitize-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 12:54:56.794870 digitize-1.0.0/
--rw-rw-rw-   0        0        0      546 2023-04-22 12:54:56.794870 digitize-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-04-22 12:52:57.000000 digitize-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 12:54:56.793875 digitize-1.0.0/digitize.egg-info/
--rw-rw-rw-   0        0        0      546 2023-04-22 12:54:56.000000 digitize-1.0.0/digitize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2023-04-22 12:54:56.000000 digitize-1.0.0/digitize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 12:54:56.000000 digitize-1.0.0/digitize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 12:54:56.000000 digitize-1.0.0/digitize.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 12:54:56.795870 digitize-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      674 2023-04-22 12:54:24.000000 digitize-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:21:47.035670 digitize-1.1.0/
+-rw-rw-rw-   0        0        0      780 2023-04-22 13:21:47.034161 digitize-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-04-22 13:20:27.000000 digitize-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 13:21:47.034161 digitize-1.1.0/digitize.egg-info/
+-rw-rw-rw-   0        0        0      780 2023-04-22 13:21:46.000000 digitize-1.1.0/digitize.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2023-04-22 13:21:46.000000 digitize-1.1.0/digitize.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 13:21:46.000000 digitize-1.1.0/digitize.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 13:21:46.000000 digitize-1.1.0/digitize.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 13:21:47.035670 digitize-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      674 2023-04-22 13:21:36.000000 digitize-1.1.0/setup.py
```

### Comparing `digitize-1.0.0/setup.py` & `digitize-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="digitize",
-    version="1.0.0",
+    version="1.1.0",
     author="LimeGeeg",
     author_email="borovoy06nik@gmail.com",
     description="Break numbers into digits with their names",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LimeGeeg/digitize",
     packages=setuptools.find_packages(),
```

