# Comparing `tmp/easierfile-1.1.0.tar.gz` & `tmp/easierfile-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easierfile-1.1.0.tar", max compression
+gzip compressed data, was "easierfile-2.0.0.tar", max compression
```

## Comparing `easierfile-1.1.0.tar` & `easierfile-2.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       32 2023-04-10 13:57:24.548112 easierfile-1.1.0/easierfile/__init__.py
--rw-r--r--   0        0        0     1700 2023-04-19 05:38:18.190568 easierfile-1.1.0/easierfile/file.py
--rw-r--r--   0        0        0     1092 2023-04-11 00:52:37.919987 easierfile-1.1.0/LICENSE
--rw-r--r--   0        0        0      556 2023-04-19 04:54:06.663354 easierfile-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      934 2023-04-11 01:32:23.623996 easierfile-1.1.0/README.md
--rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 easierfile-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       62 2023-04-21 13:34:36.835394 easierfile-2.0.0/easierfile/__init__.py
+-rw-r--r--   0        0        0     4521 2023-04-22 03:44:40.952818 easierfile-2.0.0/easierfile/file.py
+-rw-r--r--   0        0        0     1092 2023-04-11 00:52:37.919987 easierfile-2.0.0/LICENSE
+-rw-r--r--   0        0        0      563 2023-04-21 13:40:18.443965 easierfile-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      942 2023-04-20 04:53:26.793798 easierfile-2.0.0/README.md
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 easierfile-2.0.0/PKG-INFO
```

### Comparing `easierfile-1.1.0/LICENSE` & `easierfile-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easierfile-1.1.0/pyproject.toml` & `easierfile-2.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "easierfile"
-version = "1.1.0"
-description = "A simple Python package that object-oriented encapsulates Python traditional built-in file operations."
+version = "2.0.0"
+description = "An easier-to-use Python package that object-oriented encapsulates Python traditional built-in file operations."
 license = "MIT"
 authors = ["leoweyr <leoweyr@foxmail.com>"]
 readme = "README.md"
 repository = "https://github.com/leoweyr/Python-Easierfile"
 classifiers = [
-    "Development Status :: 3 - Alpha"
+    "Development Status :: 4 - Beta"
 ]
 packages = [{include = "easierfile"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `easierfile-1.1.0/README.md` & `easierfile-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Easierfile
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/easierfile.svg)](https://pypi.org/project/easierfile/)
 [![Package Status](https://img.shields.io/pypi/status/easierfile.svg)](https://pypi.org/project/easierfile/)
 [![License](https://img.shields.io/pypi/l/easierfile.svg)](https://github.com/leoweyr/Python-Easierfile/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/personalized-badge/easierfile?period=total&units=international_system&left_color=grey&right_color=green&left_text=pypi%20downloads)](https://pepy.tech/project/easierfile)
 
-A simple Python package that object-oriented encapsulates Python traditional built-in file operations. It's also easier than `easygui`. o((>ω< ))o
+An easier-to-use Python package that object-oriented encapsulates Python traditional built-in file operations. It's also easier than `easygui`. o((>ω< ))o
 
 ## ⚖️License
 
 [MIT](https://github.com/leoweyr/Python-Easierfile/blob/main/LICENSE)
 
 ## 📗Documentation
```

### Comparing `easierfile-1.1.0/PKG-INFO` & `easierfile-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: easierfile
-Version: 1.1.0
-Summary: A simple Python package that object-oriented encapsulates Python traditional built-in file operations.
+Version: 2.0.0
+Summary: An easier-to-use Python package that object-oriented encapsulates Python traditional built-in file operations.
 Home-page: https://github.com/leoweyr/Python-Easierfile
 License: MIT
 Author: leoweyr
 Author-email: leoweyr@foxmail.com
 Requires-Python: >=3.7,<4.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,15 +21,15 @@
 # Easierfile
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/easierfile.svg)](https://pypi.org/project/easierfile/)
 [![Package Status](https://img.shields.io/pypi/status/easierfile.svg)](https://pypi.org/project/easierfile/)
 [![License](https://img.shields.io/pypi/l/easierfile.svg)](https://github.com/leoweyr/Python-Easierfile/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/personalized-badge/easierfile?period=total&units=international_system&left_color=grey&right_color=green&left_text=pypi%20downloads)](https://pepy.tech/project/easierfile)
 
-A simple Python package that object-oriented encapsulates Python traditional built-in file operations. It's also easier than `easygui`. o((>ω< ))o
+An easier-to-use Python package that object-oriented encapsulates Python traditional built-in file operations. It's also easier than `easygui`. o((>ω< ))o
 
 ## ⚖️License
 
 [MIT](https://github.com/leoweyr/Python-Easierfile/blob/main/LICENSE)
 
 ## 📗Documentation
```

