# Comparing `tmp/cc-pathlib-0.0.8.tar.gz` & `tmp/cc-pathlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cc-pathlib-0.0.8.tar", last modified: Tue May 12 19:59:04 2020, max compression
+gzip compressed data, was "dist/cc-pathlib-0.0.9.tar", last modified: Mon Dec  7 15:59:39 2020, max compression
```

## Comparing `cc-pathlib-0.0.8.tar` & `cc-pathlib-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yoochan   (1000) yoochan   (1000)        0 2020-05-12 19:59:04.000000 cc-pathlib-0.0.8/
--rw-r--r--   0 yoochan   (1000) yoochan   (1000)     2970 2020-05-12 19:59:04.000000 cc-pathlib-0.0.8/PKG-INFO
--rw-r--r--   0 yoochan   (1000) yoochan   (1000)     2063 2019-06-30 16:20:16.000000 cc-pathlib-0.0.8/README.md
-drwxr-xr-x   0 yoochan   (1000) yoochan   (1000)        0 2020-05-12 19:59:04.000000 cc-pathlib-0.0.8/package/
-drwxr-xr-x   0 yoochan   (1000) yoochan   (1000)        0 2020-05-12 19:59:04.000000 cc-pathlib-0.0.8/package/cc_pathlib/
--rw-r--r--   0 yoochan   (1000) yoochan   (1000)       57 2020-05-12 19:54:43.000000 cc-pathlib-0.0.8/package/cc_pathlib/__init__.py
-drwxr-xr-x   0 yoochan   (1000) yoochan   (1000)        0 2020-05-12 19:59:04.000000 cc-pathlib-0.0.8/package/cc_pathlib/filter/
--rw-rw-r--   0 yoochan   (1000) yoochan   (1000)       23 2019-06-30 14:40:03.000000 cc-pathlib-0.0.8/package/cc_pathlib/filter/__init__.py
--rw-r--r--   0 yoochan   (1000) yoochan   (1000)      944 2020-05-12 19:54:43.000000 cc-pathlib-0.0.8/package/cc_pathlib/filter/cc_json.py
--rw-r--r--   0 yoochan   (1000) yoochan   (1000)      189 2020-05-12 19:54:43.000000 cc-pathlib-0.0.8/package/cc_pathlib/filter/cc_pickle.py
--rw-rw-r--   0 yoochan   (1000) yoochan   (1000)      626 2019-06-30 14:19:53.000000 cc-pathlib-0.0.8/package/cc_pathlib/filter/tsv.py
--rw-r--r--   0 yoochan   (1000) yoochan   (1000)     7709 2020-05-12 19:54:43.000000 cc-pathlib-0.0.8/package/cc_pathlib/path.py
-drwxr-xr-x   0 yoochan   (1000) yoochan   (1000)        0 2020-05-12 19:59:04.000000 cc-pathlib-0.0.8/package/cc_pathlib.egg-info/
--rw-rw-r--   0 yoochan   (1000) yoochan   (1000)     2970 2020-05-12 19:59:04.000000 cc-pathlib-0.0.8/package/cc_pathlib.egg-info/PKG-INFO
--rw-rw-r--   0 yoochan   (1000) yoochan   (1000)      432 2020-05-12 19:59:04.000000 cc-pathlib-0.0.8/package/cc_pathlib.egg-info/SOURCES.txt
--rw-rw-r--   0 yoochan   (1000) yoochan   (1000)        1 2020-05-12 19:59:04.000000 cc-pathlib-0.0.8/package/cc_pathlib.egg-info/dependency_links.txt
--rw-rw-r--   0 yoochan   (1000) yoochan   (1000)        7 2020-05-12 19:59:04.000000 cc-pathlib-0.0.8/package/cc_pathlib.egg-info/requires.txt
--rw-rw-r--   0 yoochan   (1000) yoochan   (1000)       11 2020-05-12 19:59:04.000000 cc-pathlib-0.0.8/package/cc_pathlib.egg-info/top_level.txt
--rw-r--r--   0 yoochan   (1000) yoochan   (1000)       38 2020-05-12 19:59:04.000000 cc-pathlib-0.0.8/setup.cfg
--rw-r--r--   0 yoochan   (1000) yoochan   (1000)      882 2020-05-12 19:57:13.000000 cc-pathlib-0.0.8/setup.py
+drwxrwxr-x   0 chassagne  (1000) chassagne  (1000)        0 2020-12-07 15:59:39.784577 cc-pathlib-0.0.9/
+-rw-rw-r--   0 chassagne  (1000) chassagne  (1000)     2970 2020-12-07 15:59:39.784577 cc-pathlib-0.0.9/PKG-INFO
+-rw-rw-r--   0 chassagne  (1000) chassagne  (1000)     2063 2020-11-27 09:25:59.000000 cc-pathlib-0.0.9/README.md
+drwxrwxr-x   0 chassagne  (1000) chassagne  (1000)        0 2020-12-07 15:59:39.784577 cc-pathlib-0.0.9/package/
+drwxrwxr-x   0 chassagne  (1000) chassagne  (1000)        0 2020-12-07 15:59:39.784577 cc-pathlib-0.0.9/package/cc_pathlib/
+-rw-rw-r--   0 chassagne  (1000) chassagne  (1000)       57 2020-11-27 09:25:59.000000 cc-pathlib-0.0.9/package/cc_pathlib/__init__.py
+drwxrwxr-x   0 chassagne  (1000) chassagne  (1000)        0 2020-12-07 15:59:39.784577 cc-pathlib-0.0.9/package/cc_pathlib/filter/
+-rw-rw-r--   0 chassagne  (1000) chassagne  (1000)       23 2020-11-27 09:25:59.000000 cc-pathlib-0.0.9/package/cc_pathlib/filter/__init__.py
+-rw-rw-r--   0 chassagne  (1000) chassagne  (1000)      944 2020-11-27 09:25:59.000000 cc-pathlib-0.0.9/package/cc_pathlib/filter/cc_json.py
+-rw-rw-r--   0 chassagne  (1000) chassagne  (1000)      189 2020-11-27 09:25:59.000000 cc-pathlib-0.0.9/package/cc_pathlib/filter/cc_pickle.py
+-rw-rw-r--   0 chassagne  (1000) chassagne  (1000)      626 2020-11-27 09:25:59.000000 cc-pathlib-0.0.9/package/cc_pathlib/filter/tsv.py
+-rw-rw-r--   0 chassagne  (1000) chassagne  (1000)     7708 2020-12-07 15:49:48.000000 cc-pathlib-0.0.9/package/cc_pathlib/path.py
+drwxrwxr-x   0 chassagne  (1000) chassagne  (1000)        0 2020-12-07 15:59:39.784577 cc-pathlib-0.0.9/package/cc_pathlib.egg-info/
+-rw-rw-r--   0 chassagne  (1000) chassagne  (1000)     2970 2020-12-07 15:59:39.000000 cc-pathlib-0.0.9/package/cc_pathlib.egg-info/PKG-INFO
+-rw-rw-r--   0 chassagne  (1000) chassagne  (1000)      432 2020-12-07 15:59:39.000000 cc-pathlib-0.0.9/package/cc_pathlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 chassagne  (1000) chassagne  (1000)        1 2020-12-07 15:59:39.000000 cc-pathlib-0.0.9/package/cc_pathlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 chassagne  (1000) chassagne  (1000)        7 2020-12-07 15:59:39.000000 cc-pathlib-0.0.9/package/cc_pathlib.egg-info/requires.txt
+-rw-rw-r--   0 chassagne  (1000) chassagne  (1000)       11 2020-12-07 15:59:39.000000 cc-pathlib-0.0.9/package/cc_pathlib.egg-info/top_level.txt
+-rw-rw-r--   0 chassagne  (1000) chassagne  (1000)       38 2020-12-07 15:59:39.784577 cc-pathlib-0.0.9/setup.cfg
+-rw-rw-r--   0 chassagne  (1000) chassagne  (1000)      882 2020-12-07 15:57:02.000000 cc-pathlib-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cc-pathlib-0.0.8/PKG-INFO` & `cc-pathlib-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cc-pathlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: supercharged implementation of pathlib.Path()
 Home-page: https://bitbucket.org/yoochan/pypi-ccpathlib
-Author: Yoochan
+Author: yoochan
 Author-email: yota.news@gmail.com
 License: UNKNOWN
 Description: # In short
         
         This libray propose to extend the capabilities of pathlib.
         The Path class provided here is a sub-class of the original pathlib.Path class.
         
@@ -47,9 +47,9 @@
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cc-pathlib-0.0.8/README.md` & `cc-pathlib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cc-pathlib-0.0.8/package/cc_pathlib/filter/cc_json.py` & `cc-pathlib-0.0.9/package/cc_pathlib/filter/cc_json.py`

 * *Files identical despite different names*

### Comparing `cc-pathlib-0.0.8/package/cc_pathlib/filter/tsv.py` & `cc-pathlib-0.0.9/package/cc_pathlib/filter/tsv.py`

 * *Files identical despite different names*

### Comparing `cc-pathlib-0.0.8/package/cc_pathlib/path.py` & `cc-pathlib-0.0.9/package/cc_pathlib/path.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 #!/usr/bin/env python3
 
-import bz2
 import datetime
 import lzma
 import gzip
 import pathlib
 import subprocess
 import socket
 import sys
 
 try :
 	import brotli
 except :
 	pass
+	
+try :
+	import bz2
+except :
+	pass
 
 import cc_pathlib.filter.cc_json
 import cc_pathlib.filter.cc_pickle
 import cc_pathlib.filter.tsv
 
 class Path(type(pathlib.Path())) :
 
@@ -216,16 +220,15 @@
 		if self.is_file() :
 			os.link(str(self), str(target))
 		else :
 			raise ValueError("hardlink source must be a file")
 
 	@property
 	def fname(self) :
-		s = ''.join(self.suffixes)
-		return self.name[:-len(s)]
+		return self.name.split('.')[0]
 
 	@property
 	def fsuffix(self) :
 		s = ''.join(self.suffixes)
 		return self.name[-len(s):]
 
 	def run(self, * cmd_lst, timeout=None, blocking=True, bg_task=False, quiet=False) :
```

### Comparing `cc-pathlib-0.0.8/package/cc_pathlib.egg-info/PKG-INFO` & `cc-pathlib-0.0.9/package/cc_pathlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cc-pathlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: supercharged implementation of pathlib.Path()
 Home-page: https://bitbucket.org/yoochan/pypi-ccpathlib
-Author: Yoochan
+Author: yoochan
 Author-email: yota.news@gmail.com
 License: UNKNOWN
 Description: # In short
         
         This libray propose to extend the capabilities of pathlib.
         The Path class provided here is a sub-class of the original pathlib.Path class.
         
@@ -47,9 +47,9 @@
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cc-pathlib-0.0.8/setup.py` & `cc-pathlib-0.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import setuptools
 
 from pathlib import Path
 
 setuptools.setup(
     name="cc-pathlib",
-    version="0.0.8",
-    author="Yoochan",
+    version="0.0.9",
+    author="yoochan",
     author_email="yota.news@gmail.com",
     description="supercharged implementation of pathlib.Path()",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://bitbucket.org/yoochan/pypi-ccpathlib",
     packages=setuptools.find_packages(where="package"),
     package_dir={
@@ -23,9 +23,9 @@
     classifiers=[
         "Programming Language :: Python :: 3",
 		"Development Status :: 4 - Beta",
         "License :: OSI Approved :: BSD License",
 		"License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
 )
```

