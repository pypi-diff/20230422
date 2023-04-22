# Comparing `tmp/mrdoxmrgt-0.0.4.tar.gz` & `tmp/mrdoxmrgt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrdoxmrgt-0.0.4.tar", last modified: Sat Apr 22 05:23:32 2023, max compression
+gzip compressed data, was "mrdoxmrgt-0.0.5.tar", last modified: Sat Apr 22 05:29:37 2023, max compression
```

## Comparing `mrdoxmrgt-0.0.4.tar` & `mrdoxmrgt-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/
--rw-rw-rw-   0        0        0     1083 2023-04-20 14:15:02.000000 mrdoxmrgt-0.0.4/LICENCE
--rw-rw-rw-   0        0        0      810 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-04-20 14:15:34.000000 mrdoxmrgt-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt/
-drwxrwxrwx   0        0        0        0 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt/GTF/
--rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.4/mrdoxmrgt/GTF/__init__.py
--rw-rw-rw-   0        0        0     3115 2023-04-22 05:22:20.000000 mrdoxmrgt-0.0.4/mrdoxmrgt/GTF/install.py
--rw-rw-rw-   0        0        0     1392 2023-04-22 05:22:14.000000 mrdoxmrgt-0.0.4/mrdoxmrgt/GTF/run.py
--rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.4/mrdoxmrgt/__init__.py
--rw-rw-rw-   0        0        0     1394 2023-04-22 05:15:38.000000 mrdoxmrgt-0.0.4/mrdoxmrgt/_main_.py
-drwxrwxrwx   0        0        0        0 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/
--rw-rw-rw-   0        0        0      810 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1243 2023-04-22 05:21:34.000000 mrdoxmrgt-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 05:29:38.000000 mrdoxmrgt-0.0.5/
+-rw-rw-rw-   0        0        0     1083 2023-04-20 14:15:02.000000 mrdoxmrgt-0.0.5/LICENCE
+-rw-rw-rw-   0        0        0      810 2023-04-22 05:29:38.000000 mrdoxmrgt-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-04-20 14:15:34.000000 mrdoxmrgt-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 05:29:38.000000 mrdoxmrgt-0.0.5/mrdoxmrgt/
+drwxrwxrwx   0        0        0        0 2023-04-22 05:29:38.000000 mrdoxmrgt-0.0.5/mrdoxmrgt/GTF/
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.5/mrdoxmrgt/GTF/__init__.py
+-rw-rw-rw-   0        0        0     3115 2023-04-22 05:22:20.000000 mrdoxmrgt-0.0.5/mrdoxmrgt/GTF/install.py
+-rw-rw-rw-   0        0        0     1392 2023-04-22 05:22:14.000000 mrdoxmrgt-0.0.5/mrdoxmrgt/GTF/run.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.5/mrdoxmrgt/__init__.py
+-rw-rw-rw-   0        0        0     1396 2023-04-22 05:28:48.000000 mrdoxmrgt-0.0.5/mrdoxmrgt/_main_.py
+drwxrwxrwx   0        0        0        0 2023-04-22 05:29:38.000000 mrdoxmrgt-0.0.5/mrdoxmrgt.egg-info/
+-rw-rw-rw-   0        0        0      810 2023-04-22 05:29:38.000000 mrdoxmrgt-0.0.5/mrdoxmrgt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-04-22 05:29:38.000000 mrdoxmrgt-0.0.5/mrdoxmrgt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 05:29:38.000000 mrdoxmrgt-0.0.5/mrdoxmrgt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-22 05:29:38.000000 mrdoxmrgt-0.0.5/mrdoxmrgt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-22 05:29:38.000000 mrdoxmrgt-0.0.5/mrdoxmrgt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-22 05:29:38.000000 mrdoxmrgt-0.0.5/mrdoxmrgt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 05:29:38.000000 mrdoxmrgt-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2023-04-22 05:29:02.000000 mrdoxmrgt-0.0.5/setup.py
```

### Comparing `mrdoxmrgt-0.0.4/LICENCE` & `mrdoxmrgt-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.4/PKG-INFO` & `mrdoxmrgt-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/SMS_Forwarder
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.0.4/mrdoxmrgt/GTF/install.py` & `mrdoxmrgt-0.0.5/mrdoxmrgt/GTF/install.py`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.4/mrdoxmrgt/GTF/run.py` & `mrdoxmrgt-0.0.5/mrdoxmrgt/GTF/run.py`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.4/mrdoxmrgt/_main_.py` & `mrdoxmrgt-0.0.5/mrdoxmrgt/_main_.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python
 # -*- coding: UTF-8 -*-
 
 import sys
 
-from GTF import install
-from GTF import run
+from .GTF import install
+from .GTF import run
 
 
 
 def main():
     try: command = sys.argv[1]
     except: command = False
     try: arguments = sys.argv[2]
```

### Comparing `mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/PKG-INFO` & `mrdoxmrgt-0.0.5/mrdoxmrgt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/SMS_Forwarder
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.0.4/setup.py` & `mrdoxmrgt-0.0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mrdoxmrgt',
     packages=find_packages(),
     include_package_data=True,
-    version="0.0.4",
+    version="0.0.5",
     description='A small example package',
     long_description="A small example package HI",
     long_description_content_type="text/markdown",
     author='MR_GT',
     author_email='friendyt89@gmail.com',
     url='https://github.com/GreyTechno/SMS_Forwarder',
     download_url="https://github.com/GreyTechno/gtf/archive/pypi.zip",
```

