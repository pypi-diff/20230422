# Comparing `tmp/scidb-bridge-19.11.5.tar.gz` & `tmp/scidb-bridge-19.11.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scidb-bridge-19.11.5.tar", last modified: Tue Jan 31 20:34:22 2023, max compression
+gzip compressed data, was "scidb-bridge-19.11.6.tar", last modified: Sat Apr 22 03:32:42 2023, max compression
```

## Comparing `scidb-bridge-19.11.5.tar` & `scidb-bridge-19.11.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwx------   0 vernica  (21736907) users      (100)        0 2023-01-31 20:34:22.323202 scidb-bridge-19.11.5/
--rw-------   0 vernica  (21736907) users      (100)      689 2023-01-31 17:17:57.000000 scidb-bridge-19.11.5/LICENSE.txt
--rw-------   0 vernica  (21736907) users      (100)     2004 2023-01-31 20:34:22.323202 scidb-bridge-19.11.5/PKG-INFO
--rw-------   0 vernica  (21736907) users      (100)     1101 2023-01-28 18:47:08.000000 scidb-bridge-19.11.5/README.rst
-drwx------   0 vernica  (21736907) users      (100)        0 2023-01-31 20:34:22.322202 scidb-bridge-19.11.5/scidb_bridge.egg-info/
--rw-------   0 vernica  (21736907) users      (100)     2004 2023-01-31 20:34:22.000000 scidb-bridge-19.11.5/scidb_bridge.egg-info/PKG-INFO
--rw-------   0 vernica  (21736907) users      (100)      345 2023-01-31 20:34:22.000000 scidb-bridge-19.11.5/scidb_bridge.egg-info/SOURCES.txt
--rw-------   0 vernica  (21736907) users      (100)        1 2023-01-31 20:34:22.000000 scidb-bridge-19.11.5/scidb_bridge.egg-info/dependency_links.txt
--rw-------   0 vernica  (21736907) users      (100)       55 2023-01-31 20:34:22.000000 scidb-bridge-19.11.5/scidb_bridge.egg-info/requires.txt
--rw-------   0 vernica  (21736907) users      (100)       12 2023-01-31 20:34:22.000000 scidb-bridge-19.11.5/scidb_bridge.egg-info/top_level.txt
-drwx------   0 vernica  (21736907) users      (100)        0 2023-01-31 20:34:22.323202 scidb-bridge-19.11.5/scidbbridge/
--rw-------   0 vernica  (21736907) users      (100)    13642 2023-01-31 18:05:50.000000 scidb-bridge-19.11.5/scidbbridge/__init__.py
--rwx------   0 vernica  (21736907) users      (100)     2948 2023-01-31 17:15:30.000000 scidb-bridge-19.11.5/scidbbridge/bridge-v1to3-fix.py
--rw-------   0 vernica  (21736907) users      (100)     3190 2023-01-31 17:15:30.000000 scidb-bridge-19.11.5/scidbbridge/coord.py
--rw-------   0 vernica  (21736907) users      (100)     8445 2023-01-31 17:15:30.000000 scidb-bridge-19.11.5/scidbbridge/coord_perf.py
--rw-------   0 vernica  (21736907) users      (100)     8508 2023-01-31 17:15:30.000000 scidb-bridge-19.11.5/scidbbridge/driver.py
--rw-------   0 vernica  (21736907) users      (100)       67 2023-01-31 20:34:22.323202 scidb-bridge-19.11.5/setup.cfg
--rw-------   0 vernica  (21736907) users      (100)     2285 2023-01-31 17:16:58.000000 scidb-bridge-19.11.5/setup.py
+drwx------   0 vernica   (1000) vernica   (1000)        0 2023-04-22 03:32:42.574261 scidb-bridge-19.11.6/
+-rw-------   0 vernica   (1000) vernica   (1000)      689 2023-03-14 20:41:57.000000 scidb-bridge-19.11.6/LICENSE.txt
+-rw-------   0 vernica   (1000) vernica   (1000)     2092 2023-04-22 03:32:42.574261 scidb-bridge-19.11.6/PKG-INFO
+-rw-------   0 vernica   (1000) vernica   (1000)     1150 2023-04-22 03:31:13.000000 scidb-bridge-19.11.6/README.rst
+drwx------   0 vernica   (1000) vernica   (1000)        0 2023-04-22 03:32:42.566261 scidb-bridge-19.11.6/scidb_bridge.egg-info/
+-rw-------   0 vernica   (1000) vernica   (1000)     2092 2023-04-22 03:32:42.000000 scidb-bridge-19.11.6/scidb_bridge.egg-info/PKG-INFO
+-rw-------   0 vernica   (1000) vernica   (1000)      345 2023-04-22 03:32:42.000000 scidb-bridge-19.11.6/scidb_bridge.egg-info/SOURCES.txt
+-rw-------   0 vernica   (1000) vernica   (1000)        1 2023-04-22 03:32:42.000000 scidb-bridge-19.11.6/scidb_bridge.egg-info/dependency_links.txt
+-rw-------   0 vernica   (1000) vernica   (1000)       57 2023-04-22 03:32:42.000000 scidb-bridge-19.11.6/scidb_bridge.egg-info/requires.txt
+-rw-------   0 vernica   (1000) vernica   (1000)       12 2023-04-22 03:32:42.000000 scidb-bridge-19.11.6/scidb_bridge.egg-info/top_level.txt
+drwx------   0 vernica   (1000) vernica   (1000)        0 2023-04-22 03:32:42.574261 scidb-bridge-19.11.6/scidbbridge/
+-rw-------   0 vernica   (1000) vernica   (1000)    13642 2023-04-22 03:31:24.000000 scidb-bridge-19.11.6/scidbbridge/__init__.py
+-rwx------   0 vernica   (1000) vernica   (1000)     2948 2023-03-14 20:41:57.000000 scidb-bridge-19.11.6/scidbbridge/bridge-v1to3-fix.py
+-rw-------   0 vernica   (1000) vernica   (1000)     3190 2023-03-05 21:24:26.000000 scidb-bridge-19.11.6/scidbbridge/coord.py
+-rw-------   0 vernica   (1000) vernica   (1000)     8445 2022-05-19 22:22:18.000000 scidb-bridge-19.11.6/scidbbridge/coord_perf.py
+-rw-------   0 vernica   (1000) vernica   (1000)     8508 2023-03-14 20:41:57.000000 scidb-bridge-19.11.6/scidbbridge/driver.py
+-rw-------   0 vernica   (1000) vernica   (1000)       67 2023-04-22 03:32:42.575261 scidb-bridge-19.11.6/setup.cfg
+-rw-------   0 vernica   (1000) vernica   (1000)     2287 2023-03-26 18:22:37.000000 scidb-bridge-19.11.6/setup.py
```

### Comparing `scidb-bridge-19.11.5/LICENSE.txt` & `scidb-bridge-19.11.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scidb-bridge-19.11.5/PKG-INFO` & `scidb-bridge-19.11.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: scidb-bridge
-Version: 19.11.5
+Version: 19.11.6
 Summary: Python library to access externally stored SciDB data
-Download-URL: http://github.com/Paradigm4/bridge
+Home-page: UNKNOWN
 Author: Rares Vernica
 Author-email: rvernica@gmail.com
 License: AGPL-3.0
+Download-URL: http://github.com/Paradigm4/bridge
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -20,28 +22,28 @@
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering
 License-File: LICENSE.txt
 
 SciDB-Bridge: Python Library to access externally stored SciDB data
 ===================================================================
 
-.. image:: https://img.shields.io/badge/SciDB-19.11-blue.svg
-    :target: https://forum.paradigm4.com/t/scidb-release-19-11/2411
+.. image:: https://img.shields.io/badge/SciDB-22.5-blue.svg
+    :target: https://paradigm4.atlassian.net/wiki/spaces/scidb/pages/2828833854/22.5+Release+Notes
 
-.. image:: https://img.shields.io/badge/arrow-3.0.0-blue.svg
-    :target: https://arrow.apache.org/release/3.0.0.html
+.. image:: https://img.shields.io/badge/arrow-11.0.0-blue.svg
+    :target: https://arrow.apache.org/release/11.0.0.html
 
 
 Requirements
 ------------
 
 - Python ``3.5.x``, ``3.6.x``, ``3.7.x``, ``3.8.x``, ``3.9.x``, or ``3.10.x``
 - SciDB ``19.11`` or newer
 - SciDB-Py ``19.11.4`` or newer
-- Apache PyArrow ``3.0.0``
+- Apache PyArrow ``5.0.0`` up to ``11.0.0``
 - Boto3 ``1.14.12`` for Amazon Simple Storage Service (S3) support
 
 
 Installation
 ------------
 
 Install latest release::
@@ -60,7 +62,9 @@
 
 .. code:: bash
 
   pip install pycodestyle
   pycodestyle py_pkg
 
 For Visual Studio Code see `Linting Python in Visual Studio Code <https://code.visualstudio.com/docs/python/linting>`_
+
+
```

### Comparing `scidb-bridge-19.11.5/README.rst` & `scidb-bridge-19.11.6/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 SciDB-Bridge: Python Library to access externally stored SciDB data
 ===================================================================
 
-.. image:: https://img.shields.io/badge/SciDB-19.11-blue.svg
-    :target: https://forum.paradigm4.com/t/scidb-release-19-11/2411
+.. image:: https://img.shields.io/badge/SciDB-22.5-blue.svg
+    :target: https://paradigm4.atlassian.net/wiki/spaces/scidb/pages/2828833854/22.5+Release+Notes
 
-.. image:: https://img.shields.io/badge/arrow-3.0.0-blue.svg
-    :target: https://arrow.apache.org/release/3.0.0.html
+.. image:: https://img.shields.io/badge/arrow-11.0.0-blue.svg
+    :target: https://arrow.apache.org/release/11.0.0.html
 
 
 Requirements
 ------------
 
 - Python ``3.5.x``, ``3.6.x``, ``3.7.x``, ``3.8.x``, ``3.9.x``, or ``3.10.x``
 - SciDB ``19.11`` or newer
 - SciDB-Py ``19.11.4`` or newer
-- Apache PyArrow ``3.0.0``
+- Apache PyArrow ``5.0.0`` up to ``11.0.0``
 - Boto3 ``1.14.12`` for Amazon Simple Storage Service (S3) support
 
 
 Installation
 ------------
 
 Install latest release::
```

### Comparing `scidb-bridge-19.11.5/scidb_bridge.egg-info/PKG-INFO` & `scidb-bridge-19.11.6/scidb_bridge.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: scidb-bridge
-Version: 19.11.5
+Version: 19.11.6
 Summary: Python library to access externally stored SciDB data
-Download-URL: http://github.com/Paradigm4/bridge
+Home-page: UNKNOWN
 Author: Rares Vernica
 Author-email: rvernica@gmail.com
 License: AGPL-3.0
+Download-URL: http://github.com/Paradigm4/bridge
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -20,28 +22,28 @@
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering
 License-File: LICENSE.txt
 
 SciDB-Bridge: Python Library to access externally stored SciDB data
 ===================================================================
 
-.. image:: https://img.shields.io/badge/SciDB-19.11-blue.svg
-    :target: https://forum.paradigm4.com/t/scidb-release-19-11/2411
+.. image:: https://img.shields.io/badge/SciDB-22.5-blue.svg
+    :target: https://paradigm4.atlassian.net/wiki/spaces/scidb/pages/2828833854/22.5+Release+Notes
 
-.. image:: https://img.shields.io/badge/arrow-3.0.0-blue.svg
-    :target: https://arrow.apache.org/release/3.0.0.html
+.. image:: https://img.shields.io/badge/arrow-11.0.0-blue.svg
+    :target: https://arrow.apache.org/release/11.0.0.html
 
 
 Requirements
 ------------
 
 - Python ``3.5.x``, ``3.6.x``, ``3.7.x``, ``3.8.x``, ``3.9.x``, or ``3.10.x``
 - SciDB ``19.11`` or newer
 - SciDB-Py ``19.11.4`` or newer
-- Apache PyArrow ``3.0.0``
+- Apache PyArrow ``5.0.0`` up to ``11.0.0``
 - Boto3 ``1.14.12`` for Amazon Simple Storage Service (S3) support
 
 
 Installation
 ------------
 
 Install latest release::
@@ -60,7 +62,9 @@
 
 .. code:: bash
 
   pip install pycodestyle
   pycodestyle py_pkg
 
 For Visual Studio Code see `Linting Python in Visual Studio Code <https://code.visualstudio.com/docs/python/linting>`_
+
+
```

### Comparing `scidb-bridge-19.11.5/scidbbridge/__init__.py` & `scidb-bridge-19.11.6/scidbbridge/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import pandas
 import pyarrow
 import scidbpy
 
 from .driver import Driver
 from .coord import coord2delta, delta2coord
 
-__version__ = '19.11.5'
+__version__ = '19.11.6'
 
 type_map_pyarrow = dict(
     [(t.__str__(), t) for t in (pyarrow.binary(),
                                 pyarrow.bool_(),
                                 pyarrow.int16(),
                                 pyarrow.int32(),
                                 pyarrow.int64(),
```

### Comparing `scidb-bridge-19.11.5/scidbbridge/bridge-v1to3-fix.py` & `scidb-bridge-19.11.6/scidbbridge/bridge-v1to3-fix.py`

 * *Files identical despite different names*

### Comparing `scidb-bridge-19.11.5/scidbbridge/coord.py` & `scidb-bridge-19.11.6/scidbbridge/coord.py`

 * *Files identical despite different names*

### Comparing `scidb-bridge-19.11.5/scidbbridge/coord_perf.py` & `scidb-bridge-19.11.6/scidbbridge/coord_perf.py`

 * *Files identical despite different names*

### Comparing `scidb-bridge-19.11.5/scidbbridge/driver.py` & `scidb-bridge-19.11.6/scidbbridge/driver.py`

 * *Files identical despite different names*

### Comparing `scidb-bridge-19.11.5/setup.py` & `scidb-bridge-19.11.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     download_url=DOWNLOAD_URL,
     license=LICENSE,
     packages=['scidbbridge'],
     install_requires=[
         'boto3>=1.14.12',
-        'pyarrow>=3.0.0,<5.0.0',
+        'pyarrow>=5.0.0,<=11.0.0',
         'scidb-py>=19.11.5',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU Affero General Public License v3',
```

