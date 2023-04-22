# Comparing `tmp/mrdoxmrgt-0.0.2.tar.gz` & `tmp/mrdoxmrgt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrdoxmrgt-0.0.2.tar", last modified: Fri Apr 21 18:41:43 2023, max compression
+gzip compressed data, was "mrdoxmrgt-0.0.3.tar", last modified: Sat Apr 22 05:17:41 2023, max compression
```

## Comparing `mrdoxmrgt-0.0.2.tar` & `mrdoxmrgt-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/
--rw-rw-rw-   0        0        0     1083 2023-04-20 14:15:02.000000 mrdoxmrgt-0.0.2/LICENCE
--rw-rw-rw-   0        0        0      810 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-04-20 14:15:34.000000 mrdoxmrgt-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt/
--rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.2/mrdoxmrgt/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-04-21 18:03:58.000000 mrdoxmrgt-0.0.2/mrdoxmrgt/_main_.py
--rw-rw-rw-   0        0        0     3069 2023-04-21 18:06:14.000000 mrdoxmrgt-0.0.2/mrdoxmrgt/install.py
--rw-rw-rw-   0        0        0     1346 2023-04-21 18:03:38.000000 mrdoxmrgt-0.0.2/mrdoxmrgt/run.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/
--rw-rw-rw-   0        0        0      810 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1243 2023-04-21 18:41:22.000000 mrdoxmrgt-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/
+-rw-rw-rw-   0        0        0     1083 2023-04-20 14:15:02.000000 mrdoxmrgt-0.0.3/LICENCE
+-rw-rw-rw-   0        0        0      810 2023-04-22 05:17:42.000000 mrdoxmrgt-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-04-20 14:15:34.000000 mrdoxmrgt-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt/
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.3/mrdoxmrgt/__init__.py
+-rw-rw-rw-   0        0        0     1394 2023-04-22 05:15:38.000000 mrdoxmrgt-0.0.3/mrdoxmrgt/_main_.py
+drwxrwxrwx   0        0        0        0 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/
+-rw-rw-rw-   0        0        0      810 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 05:17:42.000000 mrdoxmrgt-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2023-04-22 05:15:52.000000 mrdoxmrgt-0.0.3/setup.py
```

### Comparing `mrdoxmrgt-0.0.2/LICENCE` & `mrdoxmrgt-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.2/PKG-INFO` & `mrdoxmrgt-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/SMS_Forwarder
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.0.2/mrdoxmrgt/_main_.py` & `mrdoxmrgt-0.0.3/mrdoxmrgt/_main_.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 #!/usr/bin/python
 # -*- coding: UTF-8 -*-
 
-import install
-import run
-
-
-
+import sys
 
+from GTF import install
+from GTF import run
 
-import sys
 
 
 def main():
     try: command = sys.argv[1]
     except: command = False
     try: arguments = sys.argv[2]
     except: arguments = ""
```

### Comparing `mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/PKG-INFO` & `mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/SMS_Forwarder
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.0.2/setup.py` & `mrdoxmrgt-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mrdoxmrgt',
     packages=find_packages(),
     include_package_data=True,
-    version="0.0.2",
+    version="0.0.3",
     description='A small example package',
     long_description="A small example package HI",
     long_description_content_type="text/markdown",
     author='MR_GT',
     author_email='friendyt89@gmail.com',
     url='https://github.com/GreyTechno/SMS_Forwarder',
     download_url="https://github.com/GreyTechno/gtf/archive/pypi.zip",
```

