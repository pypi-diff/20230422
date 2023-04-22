# Comparing `tmp/yzhanurlparser-0.0.1.tar.gz` & `tmp/yzhanurlparser-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yzhanurlparser-0.0.1.tar", last modified: Thu Apr 13 10:49:34 2023, max compression
+gzip compressed data, was "yzhanurlparser-0.0.9.tar", last modified: Sat Apr 22 07:28:29 2023, max compression
```

## Comparing `yzhanurlparser-0.0.1.tar` & `yzhanurlparser-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 10:49:34.536846 yzhanurlparser-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-04-13 06:32:59.000000 yzhanurlparser-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1805 2023-04-13 10:49:34.535846 yzhanurlparser-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1331 2023-04-13 10:36:03.000000 yzhanurlparser-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 10:49:34.536846 yzhanurlparser-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      862 2023-04-13 10:49:16.000000 yzhanurlparser-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 10:49:34.497571 yzhanurlparser-0.0.1/yzhanurlparser/
--rw-rw-rw-   0        0        0      475 2023-04-13 10:36:45.000000 yzhanurlparser-0.0.1/yzhanurlparser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 10:49:34.521918 yzhanurlparser-0.0.1/yzhanurlparser/data/
--rw-rw-rw-   0        0        0  2440842 2023-04-01 12:00:00.000000 yzhanurlparser-0.0.1/yzhanurlparser/data/IP2LOCATION-LITE-DB1.BIN
-drwxrwxrwx   0        0        0        0 2023-04-13 10:49:34.534849 yzhanurlparser-0.0.1/yzhanurlparser/lib/
--rw-rw-rw-   0        0        0        0 2023-04-13 09:55:32.000000 yzhanurlparser-0.0.1/yzhanurlparser/lib/__init__.py
--rw-rw-rw-   0        0        0      635 2023-04-13 09:24:42.000000 yzhanurlparser-0.0.1/yzhanurlparser/lib/ip.py
--rw-rw-rw-   0        0        0      415 2023-04-13 09:43:57.000000 yzhanurlparser-0.0.1/yzhanurlparser/lib/url.py
-drwxrwxrwx   0        0        0        0 2023-04-13 10:49:34.520661 yzhanurlparser-0.0.1/yzhanurlparser.egg-info/
--rw-rw-rw-   0        0        0     1805 2023-04-13 10:49:34.000000 yzhanurlparser-0.0.1/yzhanurlparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-04-13 10:49:34.000000 yzhanurlparser-0.0.1/yzhanurlparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 10:49:34.000000 yzhanurlparser-0.0.1/yzhanurlparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-13 10:49:34.000000 yzhanurlparser-0.0.1/yzhanurlparser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-13 10:49:34.000000 yzhanurlparser-0.0.1/yzhanurlparser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 07:28:29.631184 yzhanurlparser-0.0.9/
+-rw-rw-rw-   0        0        0     1087 2023-04-22 07:04:35.000000 yzhanurlparser-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-04-22 07:27:41.000000 yzhanurlparser-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1805 2023-04-22 07:28:29.630181 yzhanurlparser-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1331 2023-04-22 07:21:23.000000 yzhanurlparser-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-22 07:28:29.631471 yzhanurlparser-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      748 2023-04-22 07:28:27.000000 yzhanurlparser-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 07:28:29.601709 yzhanurlparser-0.0.9/yzhanurlparser/
+-rw-rw-rw-   0        0        0      475 2023-04-22 07:04:35.000000 yzhanurlparser-0.0.9/yzhanurlparser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 07:28:29.620157 yzhanurlparser-0.0.9/yzhanurlparser/data/
+-rw-rw-rw-   0        0        0  2440842 2023-04-22 07:04:35.000000 yzhanurlparser-0.0.9/yzhanurlparser/data/IP2LOCATION-LITE-DB1.BIN
+drwxrwxrwx   0        0        0        0 2023-04-22 07:28:29.629181 yzhanurlparser-0.0.9/yzhanurlparser/lib/
+-rw-rw-rw-   0        0        0        0 2023-04-13 09:55:32.000000 yzhanurlparser-0.0.9/yzhanurlparser/lib/__init__.py
+-rw-rw-rw-   0        0        0      635 2023-04-13 09:24:42.000000 yzhanurlparser-0.0.9/yzhanurlparser/lib/ip.py
+-rw-rw-rw-   0        0        0      415 2023-04-13 09:43:57.000000 yzhanurlparser-0.0.9/yzhanurlparser/lib/url.py
+drwxrwxrwx   0        0        0        0 2023-04-22 07:28:29.618626 yzhanurlparser-0.0.9/yzhanurlparser.egg-info/
+-rw-rw-rw-   0        0        0     1805 2023-04-22 07:28:29.000000 yzhanurlparser-0.0.9/yzhanurlparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-22 07:28:29.000000 yzhanurlparser-0.0.9/yzhanurlparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 07:28:29.000000 yzhanurlparser-0.0.9/yzhanurlparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-22 07:28:29.000000 yzhanurlparser-0.0.9/yzhanurlparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-22 07:28:29.000000 yzhanurlparser-0.0.9/yzhanurlparser.egg-info/top_level.txt
```

### Comparing `yzhanurlparser-0.0.1/LICENSE` & `yzhanurlparser-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yzhanurlparser-0.0.1/PKG-INFO` & `yzhanurlparser-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yzhanurlparser
-Version: 0.0.1
+Version: 0.0.9
 Summary: A python library which could parse URL to ip and country.
 Home-page: https://github.com/mantoufan/yzhanurlparser
 Author: mantoufan
 Author-email: mhjlw@126.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yzhanurlparser-0.0.1/README.md` & `yzhanurlparser-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `yzhanurlparser-0.0.1/setup.py` & `yzhanurlparser-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
-    long_description = fh.read()
+  long_description = fh.read()
 
 setuptools.setup(
-    name = 'yzhanurlparser',
-    version = '0.0.1',
-    author = 'mantoufan',
-    author_email = 'mhjlw@126.com',
-    description = 'A python library which could parse URL to ip and country.',
-    long_description = long_description,
-    long_description_content_type = 'text/markdown',
-    url = 'https://github.com/mantoufan/yzhanurlparser',
-    packages = setuptools.find_packages(),
-    classifiers = [
-      'Programming Language :: Python :: 3',
-      'License :: OSI Approved :: MIT License',
-      'Operating System :: OS Independent',
-    ],
-    python_requires = '>=3.6',
-    install_requires = ['IP2Location'],
-    data_files= [('lib/site-packages/yzhanurlparser/data', ['yzhanurlparser/data/IP2LOCATION-LITE-DB1.BIN'])]
+  name = 'yzhanurlparser',
+  version = '0.0.9',
+  author = 'mantoufan',
+  author_email = 'mhjlw@126.com',
+  description = 'A python library which could parse URL to ip and country.',
+  long_description = long_description,
+  long_description_content_type = 'text/markdown',
+  url = 'https://github.com/mantoufan/yzhanurlparser',
+  packages = setuptools.find_packages(),
+  classifiers = [
+    'Programming Language :: Python :: 3',
+    'License :: OSI Approved :: MIT License',
+    'Operating System :: OS Independent',
+  ],
+  python_requires = '>=3.6',
+  install_requires = ['IP2Location'],
+  include_package_data = True
 )
```

### Comparing `yzhanurlparser-0.0.1/yzhanurlparser/data/IP2LOCATION-LITE-DB1.BIN` & `yzhanurlparser-0.0.9/yzhanurlparser/data/IP2LOCATION-LITE-DB1.BIN`

 * *Files identical despite different names*

### Comparing `yzhanurlparser-0.0.1/yzhanurlparser/lib/ip.py` & `yzhanurlparser-0.0.9/yzhanurlparser/lib/ip.py`

 * *Files identical despite different names*

### Comparing `yzhanurlparser-0.0.1/yzhanurlparser.egg-info/PKG-INFO` & `yzhanurlparser-0.0.9/yzhanurlparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yzhanurlparser
-Version: 0.0.1
+Version: 0.0.9
 Summary: A python library which could parse URL to ip and country.
 Home-page: https://github.com/mantoufan/yzhanurlparser
 Author: mantoufan
 Author-email: mhjlw@126.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

