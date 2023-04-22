# Comparing `tmp/digitize-1.0.0.tar.gz` & `tmp/digitize-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitize-1.0.0.tar", last modified: Sat Apr 22 12:54:56 2023, max compression
+gzip compressed data, was "digitize-1.0.1.tar", last modified: Sat Apr 22 13:15:43 2023, max compression
```

## Comparing `digitize-1.0.0.tar` & `digitize-1.0.1.tar`

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
+drwxrwxrwx   0        0        0        0 2023-04-22 13:15:43.205885 digitize-1.0.1/
+-rw-rw-rw-   0        0        0      849 2023-04-22 13:15:43.204882 digitize-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-04-22 13:11:41.000000 digitize-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 13:15:43.203884 digitize-1.0.1/digitize.egg-info/
+-rw-rw-rw-   0        0        0      849 2023-04-22 13:15:43.000000 digitize-1.0.1/digitize.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2023-04-22 13:15:43.000000 digitize-1.0.1/digitize.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 13:15:43.000000 digitize-1.0.1/digitize.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 13:15:43.000000 digitize-1.0.1/digitize.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 13:15:43.205885 digitize-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      674 2023-04-22 13:13:50.000000 digitize-1.0.1/setup.py
```

### Comparing `digitize-1.0.0/PKG-INFO` & `digitize-1.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 Metadata-Version: 2.1
 Name: digitize
-Version: 1.0.0
+Version: 1.0.1
 Summary: Break numbers into digits with their names
 Home-page: https://github.com/LimeGeeg/digitize
 Author: LimeGeeg
 Author-email: borovoy06nik@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 #### digitize - open source available library for determining the bit depth of a number with the output of its name
+
+```python
+from pycharge import Exact
+
+var = Exact
+
+print(var.digitize(5000)) # Output: 5,000
+print(var.digitize(51030.4853)) # Output: 51,030.48
+print(var.digitize(51030.4853, True)) # Output: 51,030.48 thousand
+print(var.digitize(51030.4853, True, "ru")) # Output: 51,030.48 С‚С‹СЃ.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `digitize-1.0.0/digitize.egg-info/PKG-INFO` & `digitize-1.0.1/digitize.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 Metadata-Version: 2.1
 Name: digitize
-Version: 1.0.0
+Version: 1.0.1
 Summary: Break numbers into digits with their names
 Home-page: https://github.com/LimeGeeg/digitize
 Author: LimeGeeg
 Author-email: borovoy06nik@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 #### digitize - open source available library for determining the bit depth of a number with the output of its name
+
+```python
+from pycharge import Exact
+
+var = Exact
+
+print(var.digitize(5000)) # Output: 5,000
+print(var.digitize(51030.4853)) # Output: 51,030.48
+print(var.digitize(51030.4853, True)) # Output: 51,030.48 thousand
+print(var.digitize(51030.4853, True, "ru")) # Output: 51,030.48 С‚С‹СЃ.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `digitize-1.0.0/setup.py` & `digitize-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="digitize",
-    version="1.0.0",
+    version="1.0.1",
     author="LimeGeeg",
     author_email="borovoy06nik@gmail.com",
     description="Break numbers into digits with their names",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LimeGeeg/digitize",
     packages=setuptools.find_packages(),
```

