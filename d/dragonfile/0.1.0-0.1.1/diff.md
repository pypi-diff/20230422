# Comparing `tmp/dragonfile-0.1.0.tar.gz` & `tmp/dragonfile-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragonfile-0.1.0.tar", last modified: Mon Apr 17 14:35:13 2023, max compression
+gzip compressed data, was "dragonfile-0.1.1.tar", last modified: Sat Apr 22 03:16:33 2023, max compression
```

## Comparing `dragonfile-0.1.0.tar` & `dragonfile-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 14:35:13.151864 dragonfile-0.1.0/
--rw-rw-rw-   0        0        0      748 2023-04-17 14:35:13.151864 dragonfile-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 14:35:13.125852 dragonfile-0.1.0/dragonfile/
--rw-rw-rw-   0        0        0      373 2023-04-17 14:27:46.000000 dragonfile-0.1.0/dragonfile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:35:13.148849 dragonfile-0.1.0/dragonfile.egg-info/
--rw-rw-rw-   0        0        0      748 2023-04-17 14:35:12.000000 dragonfile-0.1.0/dragonfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-04-17 14:35:12.000000 dragonfile-0.1.0/dragonfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 14:35:12.000000 dragonfile-0.1.0/dragonfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-17 14:35:12.000000 dragonfile-0.1.0/dragonfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 14:35:13.152850 dragonfile-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      864 2023-04-17 14:30:19.000000 dragonfile-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:35:13.149847 dragonfile-0.1.0/tests/
--rw-rw-rw-   0        0        0      844 2023-04-17 14:27:50.000000 dragonfile-0.1.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 03:16:33.290106 dragonfile-0.1.1/
+-rw-rw-rw-   0        0        0     1086 2023-04-20 21:04:35.000000 dragonfile-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      771 2023-04-22 03:16:33.288107 dragonfile-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2091 2023-04-22 02:49:35.000000 dragonfile-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 03:16:33.169181 dragonfile-0.1.1/dragonfile/
+-rw-rw-rw-   0        0        0     4025 2023-04-22 02:38:24.000000 dragonfile-0.1.1/dragonfile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 03:16:33.263122 dragonfile-0.1.1/dragonfile.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-04-22 03:16:32.000000 dragonfile-0.1.1/dragonfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-22 03:16:32.000000 dragonfile-0.1.1/dragonfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 03:16:32.000000 dragonfile-0.1.1/dragonfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-22 03:16:32.000000 dragonfile-0.1.1/dragonfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 03:16:33.292106 dragonfile-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      864 2023-04-22 03:05:21.000000 dragonfile-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 03:16:33.281111 dragonfile-0.1.1/tests/
+-rw-rw-rw-   0        0        0      472 2023-04-22 02:39:36.000000 dragonfile-0.1.1/tests/__init__.py
```

### Comparing `dragonfile-0.1.0/PKG-INFO` & `dragonfile-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: dragonfile
-Version: 0.1.0
+Version: 0.1.1
 Summary: Read CSV - Versão Test
 Author: Gabriel Arantd Felipe
 Author-email: grantd.ctt@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+License-File: LICENSE
```

### Comparing `dragonfile-0.1.0/dragonfile.egg-info/PKG-INFO` & `dragonfile-0.1.1/dragonfile.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: dragonfile
-Version: 0.1.0
+Version: 0.1.1
 Summary: Read CSV - Versão Test
 Author: Gabriel Arantd Felipe
 Author-email: grantd.ctt@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+License-File: LICENSE
```

### Comparing `dragonfile-0.1.0/setup.py` & `dragonfile-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dragonfile',
-    version='0.1.0',
+    version='0.1.1',
     description='Read CSV - Versão Test',
     author='Gabriel Arantd Felipe',
     author_email='grantd.ctt@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

