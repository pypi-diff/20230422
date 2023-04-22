# Comparing `tmp/myodan-tools-0.0.7.tar.gz` & `tmp/myodan-tools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myodan-tools-0.0.7.tar", max compression
+gzip compressed data, was "myodan-tools-0.0.8.tar", max compression
```

## Comparing `myodan-tools-0.0.7.tar` & `myodan-tools-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       14 2023-04-22 09:57:29.778905 myodan-tools-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-04-22 10:23:38.005444 myodan-tools-0.0.7/myodan_tools/__init__.py
--rw-r--r--   0        0        0       52 2023-04-22 10:23:38.005444 myodan-tools-0.0.7/myodan_tools/__main__.py
--rw-r--r--   0        0        0     2199 2023-04-22 10:46:59.132003 myodan-tools-0.0.7/myodan_tools/downloader/__pycache__/mediafire.cpython-310.pyc
--rw-r--r--   0        0        0     2450 2023-04-22 10:46:27.170712 myodan-tools-0.0.7/myodan_tools/downloader/mediafire.py
--rw-r--r--   0        0        0      854 2023-04-22 10:46:59.352002 myodan-tools-0.0.7/myodan_tools/extractor/__pycache__/mrcong.cpython-310.pyc
--rw-r--r--   0        0        0      722 2023-04-22 10:46:25.697396 myodan-tools-0.0.7/myodan_tools/extractor/mrcong.py
--rw-r--r--   0        0        0      747 2023-04-22 10:46:58.556003 myodan-tools-0.0.7/myodan_tools/main.py
--rw-r--r--   0        0        0      697 2023-04-22 10:55:25.823507 myodan-tools-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      982 2023-04-22 10:55:27.833681 myodan-tools-0.0.7/setup.py
--rw-r--r--   0        0        0      665 2023-04-22 10:55:27.834069 myodan-tools-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       14 2023-04-22 09:57:29.778905 myodan-tools-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 10:23:38.005444 myodan-tools-0.0.8/myodan_tools/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-22 10:23:38.005444 myodan-tools-0.0.8/myodan_tools/__main__.py
+-rw-r--r--   0        0        0     2199 2023-04-22 10:46:59.132003 myodan-tools-0.0.8/myodan_tools/downloader/__pycache__/mediafire.cpython-310.pyc
+-rw-r--r--   0        0        0     2450 2023-04-22 10:46:27.170712 myodan-tools-0.0.8/myodan_tools/downloader/mediafire.py
+-rw-r--r--   0        0        0      854 2023-04-22 10:46:59.352002 myodan-tools-0.0.8/myodan_tools/extractor/__pycache__/mrcong.cpython-310.pyc
+-rw-r--r--   0        0        0      722 2023-04-22 10:46:25.697396 myodan-tools-0.0.8/myodan_tools/extractor/mrcong.py
+-rw-r--r--   0        0        0      794 2023-04-22 11:02:32.747090 myodan-tools-0.0.8/myodan_tools/main.py
+-rw-r--r--   0        0        0      697 2023-04-22 11:04:38.342967 myodan-tools-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      982 2023-04-22 11:04:42.133782 myodan-tools-0.0.8/setup.py
+-rw-r--r--   0        0        0      665 2023-04-22 11:04:42.134511 myodan-tools-0.0.8/PKG-INFO
```

### Comparing `myodan-tools-0.0.7/myodan_tools/downloader/__pycache__/mediafire.cpython-310.pyc` & `myodan-tools-0.0.8/myodan_tools/downloader/__pycache__/mediafire.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `myodan-tools-0.0.7/myodan_tools/downloader/mediafire.py` & `myodan-tools-0.0.8/myodan_tools/downloader/mediafire.py`

 * *Files identical despite different names*

### Comparing `myodan-tools-0.0.7/myodan_tools/extractor/__pycache__/mrcong.cpython-310.pyc` & `myodan-tools-0.0.8/myodan_tools/extractor/__pycache__/mrcong.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `myodan-tools-0.0.7/myodan_tools/extractor/mrcong.py` & `myodan-tools-0.0.8/myodan_tools/extractor/mrcong.py`

 * *Files identical despite different names*

### Comparing `myodan-tools-0.0.7/myodan_tools/main.py` & `myodan-tools-0.0.8/myodan_tools/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from urllib.parse import urlparse
 import typer
 
 from .downloader import mediafire
-from .extractor import mrcong
+from .extractor import mrcong as mrcong_extractor
 
 app = typer.Typer()
 
 
-@app.callback()
-def callback(url_str: str):
+@app.command()
+def mrcong(url_str: str):
     url = urlparse(url_str)
 
     download_links = []
 
     if "mrcong.com" in url.netloc:
         if "/tag" in url.path:
-            post_links = mrcong.extract_post_links(url_str)
+            post_links = mrcong_extractor.extract_post_links(url_str)
 
             for post_link in post_links:
-                download_links += mrcong.extract_download_links(
+                download_links += mrcong_extractor.extract_download_links(
                     post_link["href"])
 
         else:
-            download_links += mrcong.extract_download_links(url_str)
+            download_links += mrcong_extractor.extract_download_links(url_str)
 
         for download_link in download_links:
             mediafire.download(download_link["href"], None, quiet=False)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `myodan-tools-0.0.7/pyproject.toml` & `myodan-tools-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "myodan-tools"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = ["Jongho Hong <myodan@pm.me>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 myodan-tools = "myodan_tools.main:app"
```

### Comparing `myodan-tools-0.0.7/setup.py` & `myodan-tools-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'urllib3>=1.26.12,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['myodan-tools = myodan_tools.main:app']}
 
 setup_kwargs = {
     'name': 'myodan-tools',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': '',
     'long_description': '# myodan-tools',
     'author': 'Jongho Hong',
     'author_email': 'myodan@pm.me',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `myodan-tools-0.0.7/PKG-INFO` & `myodan-tools-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myodan-tools
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 Author: Jongho Hong
 Author-email: myodan@pm.me
 Requires-Python: >=3.10.0,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Flask (>=2.2.0,<3.0.0)
```

