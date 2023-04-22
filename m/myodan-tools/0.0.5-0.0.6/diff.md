# Comparing `tmp/myodan-tools-0.0.5.tar.gz` & `tmp/myodan-tools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myodan-tools-0.0.5.tar", max compression
+gzip compressed data, was "myodan-tools-0.0.6.tar", max compression
```

## Comparing `myodan-tools-0.0.5.tar` & `myodan-tools-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       14 2023-04-22 09:57:29.778905 myodan-tools-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-04-22 10:23:38.005444 myodan-tools-0.0.5/myodan_tools/__init__.py
--rw-r--r--   0        0        0       52 2023-04-22 10:23:38.005444 myodan-tools-0.0.5/myodan_tools/__main__.py
--rw-r--r--   0        0        0     2199 2023-04-22 10:46:59.132003 myodan-tools-0.0.5/myodan_tools/downloader/__pycache__/mediafire.cpython-310.pyc
--rw-r--r--   0        0        0     2450 2023-04-22 10:46:27.170712 myodan-tools-0.0.5/myodan_tools/downloader/mediafire.py
--rw-r--r--   0        0        0      854 2023-04-22 10:46:59.352002 myodan-tools-0.0.5/myodan_tools/extractor/__pycache__/mrcong.cpython-310.pyc
--rw-r--r--   0        0        0      722 2023-04-22 10:46:25.697396 myodan-tools-0.0.5/myodan_tools/extractor/mrcong.py
--rw-r--r--   0        0        0      747 2023-04-22 10:46:58.556003 myodan-tools-0.0.5/myodan_tools/main.py
--rw-r--r--   0        0        0      729 2023-04-22 10:47:22.059980 myodan-tools-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1026 2023-04-22 10:47:29.133992 myodan-tools-0.0.5/setup.py
--rw-r--r--   0        0        0      737 2023-04-22 10:47:29.134423 myodan-tools-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       14 2023-04-22 09:57:29.778905 myodan-tools-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 10:23:38.005444 myodan-tools-0.0.6/myodan_tools/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-22 10:23:38.005444 myodan-tools-0.0.6/myodan_tools/__main__.py
+-rw-r--r--   0        0        0     2199 2023-04-22 10:46:59.132003 myodan-tools-0.0.6/myodan_tools/downloader/__pycache__/mediafire.cpython-310.pyc
+-rw-r--r--   0        0        0     2450 2023-04-22 10:46:27.170712 myodan-tools-0.0.6/myodan_tools/downloader/mediafire.py
+-rw-r--r--   0        0        0      854 2023-04-22 10:46:59.352002 myodan-tools-0.0.6/myodan_tools/extractor/__pycache__/mrcong.cpython-310.pyc
+-rw-r--r--   0        0        0      722 2023-04-22 10:46:25.697396 myodan-tools-0.0.6/myodan_tools/extractor/mrcong.py
+-rw-r--r--   0        0        0      747 2023-04-22 10:46:58.556003 myodan-tools-0.0.6/myodan_tools/main.py
+-rw-r--r--   0        0        0      729 2023-04-22 10:48:34.643909 myodan-tools-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1026 2023-04-22 10:48:37.960954 myodan-tools-0.0.6/setup.py
+-rw-r--r--   0        0        0      737 2023-04-22 10:48:37.963678 myodan-tools-0.0.6/PKG-INFO
```

### Comparing `myodan-tools-0.0.5/myodan_tools/downloader/__pycache__/mediafire.cpython-310.pyc` & `myodan-tools-0.0.6/myodan_tools/downloader/__pycache__/mediafire.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `myodan-tools-0.0.5/myodan_tools/downloader/mediafire.py` & `myodan-tools-0.0.6/myodan_tools/downloader/mediafire.py`

 * *Files identical despite different names*

### Comparing `myodan-tools-0.0.5/myodan_tools/extractor/__pycache__/mrcong.cpython-310.pyc` & `myodan-tools-0.0.6/myodan_tools/extractor/__pycache__/mrcong.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `myodan-tools-0.0.5/myodan_tools/extractor/mrcong.py` & `myodan-tools-0.0.6/myodan_tools/extractor/mrcong.py`

 * *Files identical despite different names*

### Comparing `myodan-tools-0.0.5/myodan_tools/main.py` & `myodan-tools-0.0.6/myodan_tools/main.py`

 * *Files identical despite different names*

### Comparing `myodan-tools-0.0.5/pyproject.toml` & `myodan-tools-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "myodan-tools"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["Jongho Hong <myodan@pm.me>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
-myodan-tools = "myodan-tools.main:app"
+myodan-tools = "myodan_tools.main:app"
 
 [tool.poetry.dependencies]
 python = ">=3.10.0,<3.11"
 numpy = "^1.22.2"
 replit = "^3.2.4"
 Flask = "^2.2.0"
 urllib3 = "^1.26.12"
```

### Comparing `myodan-tools-0.0.5/setup.py` & `myodan-tools-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,19 +17,19 @@
  'replit>=3.2.4,<4.0.0',
  'requests>=2.28.2,<3.0.0',
  'six>=1.16.0,<2.0.0',
  'typer[all]>=0.7.0,<0.8.0',
  'urllib3>=1.26.12,<2.0.0']
 
 entry_points = \
-{'console_scripts': ['myodan-tools = myodan-tools.main:app']}
+{'console_scripts': ['myodan-tools = myodan_tools.main:app']}
 
 setup_kwargs = {
     'name': 'myodan-tools',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': '',
     'long_description': '# myodan-tools',
     'author': 'Jongho Hong',
     'author_email': 'myodan@pm.me',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `myodan-tools-0.0.5/PKG-INFO` & `myodan-tools-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myodan-tools
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Author: Jongho Hong
 Author-email: myodan@pm.me
 Requires-Python: >=3.10.0,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Flask (>=2.2.0,<3.0.0)
```

