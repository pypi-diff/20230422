# Comparing `tmp/scSAMP-0.1.1.tar.gz` & `tmp/scSAMP-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scSAMP-0.1.1.tar", last modified: Sat Apr 22 07:05:36 2023, max compression
+gzip compressed data, was "scSAMP-0.1.2.tar", last modified: Sat Apr 22 07:37:51 2023, max compression
```

## Comparing `scSAMP-0.1.1.tar` & `scSAMP-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:05:36.817927 scSAMP-0.1.1/
--rw-r--r--   0 tianpei    (501) staff       (20)     1081 2023-04-21 10:55:20.000000 scSAMP-0.1.1/LICENSE
--rw-r--r--   0 tianpei    (501) staff       (20)      659 2023-04-22 07:05:36.817498 scSAMP-0.1.1/PKG-INFO
--rw-r--r--   0 tianpei    (501) staff       (20)      383 2023-04-21 05:56:39.000000 scSAMP-0.1.1/README.md
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:05:36.805256 scSAMP-0.1.1/docs/
--rw-r--r--   0 tianpei    (501) staff       (20)        0 2023-04-04 02:37:34.000000 scSAMP-0.1.1/docs/__init__.py
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:05:36.807218 scSAMP-0.1.1/scSAMP/
--rw-r--r--   0 tianpei    (501) staff       (20)       97 2023-04-22 07:01:57.000000 scSAMP-0.1.1/scSAMP/__init__.py
--rw-r--r--   0 tianpei    (501) staff       (20)     1675 2023-04-04 06:15:14.000000 scSAMP-0.1.1/scSAMP/_config.py
--rw-r--r--   0 tianpei    (501) staff       (20)     1175 2023-04-22 07:01:57.000000 scSAMP-0.1.1/scSAMP/_decorator.py
--rw-r--r--   0 tianpei    (501) staff       (20)     4040 2023-04-22 07:01:57.000000 scSAMP-0.1.1/scSAMP/_utils.py
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:05:36.811167 scSAMP-0.1.1/scSAMP/evaluation/
--rw-r--r--   0 tianpei    (501) staff       (20)       80 2023-04-22 07:01:57.000000 scSAMP-0.1.1/scSAMP/evaluation/__init__.py
--rw-r--r--   0 tianpei    (501) staff       (20)     5852 2023-04-22 07:01:57.000000 scSAMP-0.1.1/scSAMP/evaluation/_batch.py
--rw-r--r--   0 tianpei    (501) staff       (20)     1509 2023-04-22 06:18:17.000000 scSAMP-0.1.1/scSAMP/evaluation/_score.py
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:05:36.812422 scSAMP-0.1.1/scSAMP/evaluation/model/
--rw-r--r--   0 tianpei    (501) staff       (20)       32 2023-04-22 07:01:57.000000 scSAMP-0.1.1/scSAMP/evaluation/model/__init__.py
--rw-r--r--   0 tianpei    (501) staff       (20)    13735 2023-04-22 06:18:17.000000 scSAMP-0.1.1/scSAMP/evaluation/model/_actinn.py
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:05:36.816262 scSAMP-0.1.1/scSAMP/processing/
--rw-r--r--   0 tianpei    (501) staff       (20)      152 2023-04-22 07:01:57.000000 scSAMP-0.1.1/scSAMP/processing/__init__.py
--rw-r--r--   0 tianpei    (501) staff       (20)     1154 2023-04-04 05:32:09.000000 scSAMP-0.1.1/scSAMP/processing/_balance.py
--rw-r--r--   0 tianpei    (501) staff       (20)     3423 2023-04-04 05:27:17.000000 scSAMP-0.1.1/scSAMP/processing/_factors.py
--rw-r--r--   0 tianpei    (501) staff       (20)     7836 2023-04-22 06:18:17.000000 scSAMP-0.1.1/scSAMP/processing/_preprocessing.py
--rw-r--r--   0 tianpei    (501) staff       (20)    12469 2023-04-22 07:01:57.000000 scSAMP-0.1.1/scSAMP/processing/_sampler.py
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:05:36.809489 scSAMP-0.1.1/scSAMP.egg-info/
--rw-r--r--   0 tianpei    (501) staff       (20)      659 2023-04-22 07:05:36.000000 scSAMP-0.1.1/scSAMP.egg-info/PKG-INFO
--rw-r--r--   0 tianpei    (501) staff       (20)      593 2023-04-22 07:05:36.000000 scSAMP-0.1.1/scSAMP.egg-info/SOURCES.txt
--rw-r--r--   0 tianpei    (501) staff       (20)        1 2023-04-22 07:05:36.000000 scSAMP-0.1.1/scSAMP.egg-info/dependency_links.txt
--rw-r--r--   0 tianpei    (501) staff       (20)       88 2023-04-22 07:05:36.000000 scSAMP-0.1.1/scSAMP.egg-info/requires.txt
--rw-r--r--   0 tianpei    (501) staff       (20)       12 2023-04-22 07:05:36.000000 scSAMP-0.1.1/scSAMP.egg-info/top_level.txt
--rw-r--r--   0 tianpei    (501) staff       (20)       38 2023-04-22 07:05:36.818056 scSAMP-0.1.1/setup.cfg
--rw-r--r--   0 tianpei    (501) staff       (20)     3879 2023-04-22 07:04:05.000000 scSAMP-0.1.1/setup.py
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:05:36.817017 scSAMP-0.1.1/test/
--rw-r--r--   0 tianpei    (501) staff       (20)        0 2023-04-22 06:48:47.000000 scSAMP-0.1.1/test/test.py
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:37:51.855841 scSAMP-0.1.2/
+-rw-r--r--   0 tianpei    (501) staff       (20)     1081 2023-04-21 10:55:20.000000 scSAMP-0.1.2/LICENSE
+-rw-r--r--   0 tianpei    (501) staff       (20)      658 2023-04-22 07:37:51.855481 scSAMP-0.1.2/PKG-INFO
+-rw-r--r--   0 tianpei    (501) staff       (20)      423 2023-04-22 07:09:56.000000 scSAMP-0.1.2/README.md
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:37:51.840373 scSAMP-0.1.2/docs/
+-rw-r--r--   0 tianpei    (501) staff       (20)        0 2023-04-04 02:37:34.000000 scSAMP-0.1.2/docs/__init__.py
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:37:51.843336 scSAMP-0.1.2/scSAMP/
+-rw-r--r--   0 tianpei    (501) staff       (20)       97 2023-04-22 07:01:57.000000 scSAMP-0.1.2/scSAMP/__init__.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     1675 2023-04-04 06:15:14.000000 scSAMP-0.1.2/scSAMP/_config.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     1175 2023-04-22 07:01:57.000000 scSAMP-0.1.2/scSAMP/_decorator.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     4040 2023-04-22 07:01:57.000000 scSAMP-0.1.2/scSAMP/_utils.py
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:37:51.848178 scSAMP-0.1.2/scSAMP/evaluation/
+-rw-r--r--   0 tianpei    (501) staff       (20)       80 2023-04-22 07:01:57.000000 scSAMP-0.1.2/scSAMP/evaluation/__init__.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     5852 2023-04-22 07:01:57.000000 scSAMP-0.1.2/scSAMP/evaluation/_batch.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     1509 2023-04-22 06:18:17.000000 scSAMP-0.1.2/scSAMP/evaluation/_score.py
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:37:51.850064 scSAMP-0.1.2/scSAMP/evaluation/model/
+-rw-r--r--   0 tianpei    (501) staff       (20)       32 2023-04-22 07:01:57.000000 scSAMP-0.1.2/scSAMP/evaluation/model/__init__.py
+-rw-r--r--   0 tianpei    (501) staff       (20)    13735 2023-04-22 06:18:17.000000 scSAMP-0.1.2/scSAMP/evaluation/model/_actinn.py
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:37:51.853793 scSAMP-0.1.2/scSAMP/processing/
+-rw-r--r--   0 tianpei    (501) staff       (20)      152 2023-04-22 07:01:57.000000 scSAMP-0.1.2/scSAMP/processing/__init__.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     1154 2023-04-04 05:32:09.000000 scSAMP-0.1.2/scSAMP/processing/_balance.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     3423 2023-04-04 05:27:17.000000 scSAMP-0.1.2/scSAMP/processing/_factors.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     7836 2023-04-22 06:18:17.000000 scSAMP-0.1.2/scSAMP/processing/_preprocessing.py
+-rw-r--r--   0 tianpei    (501) staff       (20)    12469 2023-04-22 07:01:57.000000 scSAMP-0.1.2/scSAMP/processing/_sampler.py
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:37:51.845291 scSAMP-0.1.2/scSAMP.egg-info/
+-rw-r--r--   0 tianpei    (501) staff       (20)      658 2023-04-22 07:37:51.000000 scSAMP-0.1.2/scSAMP.egg-info/PKG-INFO
+-rw-r--r--   0 tianpei    (501) staff       (20)      593 2023-04-22 07:37:51.000000 scSAMP-0.1.2/scSAMP.egg-info/SOURCES.txt
+-rw-r--r--   0 tianpei    (501) staff       (20)        1 2023-04-22 07:37:51.000000 scSAMP-0.1.2/scSAMP.egg-info/dependency_links.txt
+-rw-r--r--   0 tianpei    (501) staff       (20)       88 2023-04-22 07:37:51.000000 scSAMP-0.1.2/scSAMP.egg-info/requires.txt
+-rw-r--r--   0 tianpei    (501) staff       (20)       12 2023-04-22 07:37:51.000000 scSAMP-0.1.2/scSAMP.egg-info/top_level.txt
+-rw-r--r--   0 tianpei    (501) staff       (20)       38 2023-04-22 07:37:51.855957 scSAMP-0.1.2/setup.cfg
+-rw-r--r--   0 tianpei    (501) staff       (20)     3878 2023-04-22 07:32:43.000000 scSAMP-0.1.2/setup.py
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 07:37:51.854558 scSAMP-0.1.2/test/
+-rw-r--r--   0 tianpei    (501) staff       (20)       22 2023-04-22 07:08:49.000000 scSAMP-0.1.2/test/test.py
```

### Comparing `scSAMP-0.1.1/LICENSE` & `scSAMP-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.1/PKG-INFO` & `scSAMP-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: scSAMP
-Version: 0.1.1
+Version: 0.1.2
 Summary: scRNA-seq data sampling toolkit.
 Home-page: https://github.com/Tptrix29/scSAMP
 Author: Pei Tian
 Author-email: 1953776@tongji.edu.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.10.0
+Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 scRNA-seq data sampling toolkit.
```

### Comparing `scSAMP-0.1.1/scSAMP/_config.py` & `scSAMP-0.1.2/scSAMP/_config.py`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.1/scSAMP/_decorator.py` & `scSAMP-0.1.2/scSAMP/_decorator.py`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.1/scSAMP/_utils.py` & `scSAMP-0.1.2/scSAMP/_utils.py`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.1/scSAMP/evaluation/_batch.py` & `scSAMP-0.1.2/scSAMP/evaluation/_batch.py`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.1/scSAMP/evaluation/_score.py` & `scSAMP-0.1.2/scSAMP/evaluation/_score.py`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.1/scSAMP/evaluation/model/_actinn.py` & `scSAMP-0.1.2/scSAMP/evaluation/model/_actinn.py`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.1/scSAMP/processing/_balance.py` & `scSAMP-0.1.2/scSAMP/processing/_balance.py`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.1/scSAMP/processing/_factors.py` & `scSAMP-0.1.2/scSAMP/processing/_factors.py`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.1/scSAMP/processing/_preprocessing.py` & `scSAMP-0.1.2/scSAMP/processing/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.1/scSAMP/processing/_sampler.py` & `scSAMP-0.1.2/scSAMP/processing/_sampler.py`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.1/scSAMP.egg-info/PKG-INFO` & `scSAMP-0.1.2/scSAMP.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: scSAMP
-Version: 0.1.1
+Version: 0.1.2
 Summary: scRNA-seq data sampling toolkit.
 Home-page: https://github.com/Tptrix29/scSAMP
 Author: Pei Tian
 Author-email: 1953776@tongji.edu.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.10.0
+Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 scRNA-seq data sampling toolkit.
```

### Comparing `scSAMP-0.1.1/scSAMP.egg-info/SOURCES.txt` & `scSAMP-0.1.2/scSAMP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.1/setup.py` & `scSAMP-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 # Package meta-data.
 NAME = 'scSAMP'
 DESCRIPTION = 'scRNA-seq data sampling toolkit.'
 URL = 'https://github.com/Tptrix29/scSAMP'
 EMAIL = '1953776@tongji.edu.cn'
 AUTHOR = 'Pei Tian'
-REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.1.1'
+REQUIRES_PYTHON = '>=3.6.0'
+VERSION = '0.1.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "numpy", "pandas", "matplotlib", "scikit-learn",
     "pyreadr", "anndata", "tensorflow", "imbalanced-learn", "scanpy"
 ]
```

