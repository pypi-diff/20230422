# Comparing `tmp/scidb-strm-19.3.0.tar.gz` & `tmp/scidb-strm-19.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scidb-strm-19.3.0.tar", last modified: Mon Jul  8 05:30:51 2019, max compression
+gzip compressed data, was "dist/scidb-strm-19.3.1.tar", last modified: Mon Jun 22 04:32:30 2020, max compression
```

## Comparing `scidb-strm-19.3.0.tar` & `scidb-strm-19.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwx------   0 rares     (1000) rares     (1000)        0 2019-07-08 05:30:51.000000 scidb-strm-19.3.0/
--rw-------   0 rares     (1000) rares     (1000)     5770 2019-07-08 05:30:51.000000 scidb-strm-19.3.0/PKG-INFO
--rw-------   0 rares     (1000) rares     (1000)     3892 2018-02-16 02:30:28.000000 scidb-strm-19.3.0/README.rst
-drwx------   0 rares     (1000) rares     (1000)        0 2019-07-08 05:30:51.000000 scidb-strm-19.3.0/scidb_strm.egg-info/
--rw-------   0 rares     (1000) rares     (1000)     5770 2019-07-08 05:30:51.000000 scidb-strm-19.3.0/scidb_strm.egg-info/PKG-INFO
--rw-------   0 rares     (1000) rares     (1000)      220 2019-07-08 05:30:51.000000 scidb-strm-19.3.0/scidb_strm.egg-info/SOURCES.txt
--rw-------   0 rares     (1000) rares     (1000)        1 2019-07-08 05:30:51.000000 scidb-strm-19.3.0/scidb_strm.egg-info/dependency_links.txt
--rw-------   0 rares     (1000) rares     (1000)      120 2019-07-08 05:30:51.000000 scidb-strm-19.3.0/scidb_strm.egg-info/requires.txt
--rw-------   0 rares     (1000) rares     (1000)       10 2019-07-08 05:30:51.000000 scidb-strm-19.3.0/scidb_strm.egg-info/top_level.txt
-drwx------   0 rares     (1000) rares     (1000)        0 2019-07-08 05:30:51.000000 scidb-strm-19.3.0/scidbstrm/
--rw-------   0 rares     (1000) rares     (1000)     2336 2019-07-08 05:30:13.000000 scidb-strm-19.3.0/scidbstrm/__init__.py
--rw-rw-r--   0 rares     (1000) rares     (1000)       67 2019-07-08 05:30:51.000000 scidb-strm-19.3.0/setup.cfg
--rw-------   0 rares     (1000) rares     (1000)     1451 2019-07-08 04:40:15.000000 scidb-strm-19.3.0/setup.py
+drwx------   0 vernica   (1000) vernica   (1000)        0 2020-06-22 04:32:30.157603 scidb-strm-19.3.1/
+-rw-------   0 vernica   (1000) vernica   (1000)     6596 2020-06-22 04:32:30.157603 scidb-strm-19.3.1/PKG-INFO
+-rw-------   0 vernica   (1000) vernica   (1000)     4526 2020-05-27 02:47:05.000000 scidb-strm-19.3.1/README.rst
+drwx------   0 vernica   (1000) vernica   (1000)        0 2020-06-22 04:32:30.157603 scidb-strm-19.3.1/scidb_strm.egg-info/
+-rw-------   0 vernica   (1000) vernica   (1000)     6596 2020-06-22 04:32:30.000000 scidb-strm-19.3.1/scidb_strm.egg-info/PKG-INFO
+-rw-------   0 vernica   (1000) vernica   (1000)      220 2020-06-22 04:32:30.000000 scidb-strm-19.3.1/scidb_strm.egg-info/SOURCES.txt
+-rw-------   0 vernica   (1000) vernica   (1000)        1 2020-06-22 04:32:30.000000 scidb-strm-19.3.1/scidb_strm.egg-info/dependency_links.txt
+-rw-------   0 vernica   (1000) vernica   (1000)      128 2020-06-22 04:32:30.000000 scidb-strm-19.3.1/scidb_strm.egg-info/requires.txt
+-rw-------   0 vernica   (1000) vernica   (1000)       10 2020-06-22 04:32:30.000000 scidb-strm-19.3.1/scidb_strm.egg-info/top_level.txt
+drwx------   0 vernica   (1000) vernica   (1000)        0 2020-06-22 04:32:30.157603 scidb-strm-19.3.1/scidbstrm/
+-rw-------   0 vernica   (1000) vernica   (1000)     2336 2020-06-22 04:32:23.000000 scidb-strm-19.3.1/scidbstrm/__init__.py
+-rw-------   0 vernica   (1000) vernica   (1000)       67 2020-06-22 04:32:30.158603 scidb-strm-19.3.1/setup.cfg
+-rw-------   0 vernica   (1000) vernica   (1000)     1459 2020-06-22 04:31:00.000000 scidb-strm-19.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scidb-strm-19.3.0/PKG-INFO` & `scidb-strm-19.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scidb-strm
-Version: 19.3.0
+Version: 19.3.1
 Summary: Python library for SciDB streaming
 Home-page: UNKNOWN
 Author: Rares Vernica
 Author-email: rvernica@gmail.com
 License: AGPL-3.0
 Download-URL: http://github.com/Paradigm4/Stream
 Description: SciDB-Strm: Python Library for SciDB Streaming
@@ -20,14 +20,15 @@
         Python ``2.7.x``, ``3.4.x``, ``3.5.x``, ``3.6.x`` or newer.
         
         Required Python packages::
         
           dill
           feather-format
           pandas
+          pyarrow
         
         Note
         ^^^^
         
         Apache Arrow versions older than ``0.8.0`` contain a bug which might
         affect Stream users. The bug manifests on chunks of more than ``128``
         records with null-able values. For more details, see the full bug
@@ -132,14 +133,37 @@
         
           /opt/scidb/18.1/DB-scidb/0/0/scidb-stderr.log
           /opt/scidb/18.1/DB-scidb/0/1/scidb-stderr.log
         
         If using SciDB ``18.1`` installed in the default location and
         configured with one server and two instances.
         
+        
+        ImportError: No module named
+        ----------------------------
+        
+        When trying to de-serialize a Python function uploaded to SciDB using
+        ``pack_func``, one might encounter::
+        
+          ImportError: No module named ...
+        
+        This error is because ``dill``, the Python serialization library,
+        links the function to the module in which it is defined. This can be
+        resolved in two ways:
+        
+        1. Make the named module available on all the SciDB instances
+        2. If the module is small, the recursive ``dill`` mode can be
+           used. Replace::
+        
+             foo_pack = scidbstrm.pack_func(foo)
+        
+           with::
+        
+             foo_pack = numpy.array([dill.dumps(foo, 0, recurse=True)])
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `scidb-strm-19.3.0/README.rst` & `scidb-strm-19.3.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 Python ``2.7.x``, ``3.4.x``, ``3.5.x``, ``3.6.x`` or newer.
 
 Required Python packages::
 
   dill
   feather-format
   pandas
+  pyarrow
 
 Note
 ^^^^
 
 Apache Arrow versions older than ``0.8.0`` contain a bug which might
 affect Stream users. The bug manifests on chunks of more than ``128``
 records with null-able values. For more details, see the full bug
@@ -122,7 +123,30 @@
 instance, for example::
 
   /opt/scidb/18.1/DB-scidb/0/0/scidb-stderr.log
   /opt/scidb/18.1/DB-scidb/0/1/scidb-stderr.log
 
 If using SciDB ``18.1`` installed in the default location and
 configured with one server and two instances.
+
+
+ImportError: No module named
+----------------------------
+
+When trying to de-serialize a Python function uploaded to SciDB using
+``pack_func``, one might encounter::
+
+  ImportError: No module named ...
+
+This error is because ``dill``, the Python serialization library,
+links the function to the module in which it is defined. This can be
+resolved in two ways:
+
+1. Make the named module available on all the SciDB instances
+2. If the module is small, the recursive ``dill`` mode can be
+   used. Replace::
+
+     foo_pack = scidbstrm.pack_func(foo)
+
+   with::
+
+     foo_pack = numpy.array([dill.dumps(foo, 0, recurse=True)])
```

### Comparing `scidb-strm-19.3.0/scidb_strm.egg-info/PKG-INFO` & `scidb-strm-19.3.1/scidb_strm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scidb-strm
-Version: 19.3.0
+Version: 19.3.1
 Summary: Python library for SciDB streaming
 Home-page: UNKNOWN
 Author: Rares Vernica
 Author-email: rvernica@gmail.com
 License: AGPL-3.0
 Download-URL: http://github.com/Paradigm4/Stream
 Description: SciDB-Strm: Python Library for SciDB Streaming
@@ -20,14 +20,15 @@
         Python ``2.7.x``, ``3.4.x``, ``3.5.x``, ``3.6.x`` or newer.
         
         Required Python packages::
         
           dill
           feather-format
           pandas
+          pyarrow
         
         Note
         ^^^^
         
         Apache Arrow versions older than ``0.8.0`` contain a bug which might
         affect Stream users. The bug manifests on chunks of more than ``128``
         records with null-able values. For more details, see the full bug
@@ -132,14 +133,37 @@
         
           /opt/scidb/18.1/DB-scidb/0/0/scidb-stderr.log
           /opt/scidb/18.1/DB-scidb/0/1/scidb-stderr.log
         
         If using SciDB ``18.1`` installed in the default location and
         configured with one server and two instances.
         
+        
+        ImportError: No module named
+        ----------------------------
+        
+        When trying to de-serialize a Python function uploaded to SciDB using
+        ``pack_func``, one might encounter::
+        
+          ImportError: No module named ...
+        
+        This error is because ``dill``, the Python serialization library,
+        links the function to the module in which it is defined. This can be
+        resolved in two ways:
+        
+        1. Make the named module available on all the SciDB instances
+        2. If the module is small, the recursive ``dill`` mode can be
+           used. Replace::
+        
+             foo_pack = scidbstrm.pack_func(foo)
+        
+           with::
+        
+             foo_pack = numpy.array([dill.dumps(foo, 0, recurse=True)])
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `scidb-strm-19.3.0/scidbstrm/__init__.py` & `scidb-strm-19.3.1/scidbstrm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 except KeyError:
     import os
     os.environ.setdefault('PATH', '')
     import numpy
     import pandas
 
 
-__version__ = '19.3.0'
+__version__ = '19.3.1'
 
 
 python_map = ("'" +
               'python{major} -uc '.format(major=sys.version_info.major) +
               '"import scidbstrm; scidbstrm.map(scidbstrm.read_func())"' +
               "'")
```

### Comparing `scidb-strm-19.3.0/setup.py` & `scidb-strm-19.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     author_email=AUTHOR_EMAIL,
     download_url=DOWNLOAD_URL,
     license=LICENSE,
     packages=['scidbstrm'],
     install_requires=[
         'dill',
         'feather-format',
-        'pandas',
+        'pandas>=0.20.0',
         'pyarrow==0.9.0;python_version<"3.5"',
         'pyarrow>=0.9.0,<0.14.0;python_version>="3.5"',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
```

