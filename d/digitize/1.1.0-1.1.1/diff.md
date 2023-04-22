# Comparing `tmp/digitize-1.1.0.tar.gz` & `tmp/digitize-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitize-1.1.0.tar", last modified: Sat Apr 22 13:21:47 2023, max compression
+gzip compressed data, was "digitize-1.1.1.tar", last modified: Sat Apr 22 14:00:12 2023, max compression
```

## Comparing `digitize-1.1.0.tar` & `digitize-1.1.1.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 13:21:47.035670 digitize-1.1.0/
--rw-rw-rw-   0        0        0      780 2023-04-22 13:21:47.034161 digitize-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-04-22 13:20:27.000000 digitize-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 13:21:47.034161 digitize-1.1.0/digitize.egg-info/
--rw-rw-rw-   0        0        0      780 2023-04-22 13:21:46.000000 digitize-1.1.0/digitize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2023-04-22 13:21:46.000000 digitize-1.1.0/digitize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 13:21:46.000000 digitize-1.1.0/digitize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 13:21:46.000000 digitize-1.1.0/digitize.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 13:21:47.035670 digitize-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      674 2023-04-22 13:21:36.000000 digitize-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:00:12.038908 digitize-1.1.1/
+-rw-rw-rw-   0        0        0      780 2023-04-22 14:00:12.038908 digitize-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-04-22 13:20:27.000000 digitize-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 14:00:12.021910 digitize-1.1.1/digitize/
+-rw-rw-rw-   0        0        0       28 2023-04-22 13:37:24.000000 digitize-1.1.1/digitize/__init__.py
+-rw-rw-rw-   0        0        0     3933 2023-04-22 13:14:47.000000 digitize-1.1.1/digitize/get_exact.py
+-rw-rw-rw-   0        0        0      121 2023-04-22 13:14:54.000000 digitize-1.1.1/digitize/test_example.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:00:12.036912 digitize-1.1.1/digitize.egg-info/
+-rw-rw-rw-   0        0        0      780 2023-04-22 14:00:11.000000 digitize-1.1.1/digitize.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-04-22 14:00:11.000000 digitize-1.1.1/digitize.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 14:00:11.000000 digitize-1.1.1/digitize.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-22 14:00:11.000000 digitize-1.1.1/digitize.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 14:00:12.038908 digitize-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      660 2023-04-22 13:58:51.000000 digitize-1.1.1/setup.py
```

### Comparing `digitize-1.1.0/PKG-INFO` & `digitize-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitize
-Version: 1.1.0
+Version: 1.1.1
 Summary: Break numbers into digits with their names
 Home-page: https://github.com/LimeGeeg/digitize
 Author: LimeGeeg
 Author-email: borovoy06nik@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `digitize-1.1.0/digitize.egg-info/PKG-INFO` & `digitize-1.1.1/digitize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitize
-Version: 1.1.0
+Version: 1.1.1
 Summary: Break numbers into digits with their names
 Home-page: https://github.com/LimeGeeg/digitize
 Author: LimeGeeg
 Author-email: borovoy06nik@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `digitize-1.1.0/setup.py` & `digitize-1.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="digitize",
-    version="1.1.0",
+    version="1.1.1",
     author="LimeGeeg",
     author_email="borovoy06nik@gmail.com",
     description="Break numbers into digits with their names",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LimeGeeg/digitize",
-    packages=setuptools.find_packages(),
+    packages=["digitize"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

