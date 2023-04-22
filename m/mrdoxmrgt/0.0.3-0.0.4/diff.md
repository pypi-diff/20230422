# Comparing `tmp/mrdoxmrgt-0.0.3.tar.gz` & `tmp/mrdoxmrgt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrdoxmrgt-0.0.3.tar", last modified: Sat Apr 22 05:17:41 2023, max compression
+gzip compressed data, was "mrdoxmrgt-0.0.4.tar", last modified: Sat Apr 22 05:23:32 2023, max compression
```

## Comparing `mrdoxmrgt-0.0.3.tar` & `mrdoxmrgt-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/
--rw-rw-rw-   0        0        0     1083 2023-04-20 14:15:02.000000 mrdoxmrgt-0.0.3/LICENCE
--rw-rw-rw-   0        0        0      810 2023-04-22 05:17:42.000000 mrdoxmrgt-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-04-20 14:15:34.000000 mrdoxmrgt-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt/
--rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.3/mrdoxmrgt/__init__.py
--rw-rw-rw-   0        0        0     1394 2023-04-22 05:15:38.000000 mrdoxmrgt-0.0.3/mrdoxmrgt/_main_.py
-drwxrwxrwx   0        0        0        0 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/
--rw-rw-rw-   0        0        0      810 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-22 05:17:40.000000 mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 05:17:42.000000 mrdoxmrgt-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1243 2023-04-22 05:15:52.000000 mrdoxmrgt-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/
+-rw-rw-rw-   0        0        0     1083 2023-04-20 14:15:02.000000 mrdoxmrgt-0.0.4/LICENCE
+-rw-rw-rw-   0        0        0      810 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-04-20 14:15:34.000000 mrdoxmrgt-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt/
+drwxrwxrwx   0        0        0        0 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt/GTF/
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.4/mrdoxmrgt/GTF/__init__.py
+-rw-rw-rw-   0        0        0     3115 2023-04-22 05:22:20.000000 mrdoxmrgt-0.0.4/mrdoxmrgt/GTF/install.py
+-rw-rw-rw-   0        0        0     1392 2023-04-22 05:22:14.000000 mrdoxmrgt-0.0.4/mrdoxmrgt/GTF/run.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.4/mrdoxmrgt/__init__.py
+-rw-rw-rw-   0        0        0     1394 2023-04-22 05:15:38.000000 mrdoxmrgt-0.0.4/mrdoxmrgt/_main_.py
+drwxrwxrwx   0        0        0        0 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/
+-rw-rw-rw-   0        0        0      810 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 05:23:32.000000 mrdoxmrgt-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2023-04-22 05:21:34.000000 mrdoxmrgt-0.0.4/setup.py
```

### Comparing `mrdoxmrgt-0.0.3/LICENCE` & `mrdoxmrgt-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.3/PKG-INFO` & `mrdoxmrgt-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/SMS_Forwarder
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.0.3/mrdoxmrgt/_main_.py` & `mrdoxmrgt-0.0.4/mrdoxmrgt/_main_.py`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.3/mrdoxmrgt.egg-info/PKG-INFO` & `mrdoxmrgt-0.0.4/mrdoxmrgt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/SMS_Forwarder
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.0.3/setup.py` & `mrdoxmrgt-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mrdoxmrgt',
     packages=find_packages(),
     include_package_data=True,
-    version="0.0.3",
+    version="0.0.4",
     description='A small example package',
     long_description="A small example package HI",
     long_description_content_type="text/markdown",
     author='MR_GT',
     author_email='friendyt89@gmail.com',
     url='https://github.com/GreyTechno/SMS_Forwarder',
     download_url="https://github.com/GreyTechno/gtf/archive/pypi.zip",
```

