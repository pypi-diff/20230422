# Comparing `tmp/aemcmc-nightly-0.0.8.dev20230420.tar.gz` & `tmp/aemcmc-nightly-0.0.8.dev20230421.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aemcmc-nightly-0.0.8.dev20230420.tar", last modified: Thu Apr 20 00:56:49 2023, max compression
+gzip compressed data, was "aemcmc-nightly-0.0.8.dev20230421.tar", last modified: Fri Apr 21 00:57:08 2023, max compression
```

## Comparing `aemcmc-nightly-0.0.8.dev20230420.tar` & `aemcmc-nightly-0.0.8.dev20230421.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:56:49.423674 aemcmc-nightly-0.0.8.dev20230420/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-20 00:56:49.423674 aemcmc-nightly-0.0.8.dev20230420/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:56:49.423674 aemcmc-nightly-0.0.8.dev20230420/aemcmc/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-20 00:56:49.423674 aemcmc-nightly-0.0.8.dev20230420/aemcmc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc/conjugates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc/ffbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24238 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc/gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:56:49.423674 aemcmc-nightly-0.0.8.dev20230420/aemcmc_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-20 00:56:49.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-20 00:56:49.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:56:49.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:56:49.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 00:56:49.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 00:56:49.000000 aemcmc-nightly-0.0.8.dev20230420/aemcmc_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-20 00:56:49.423674 aemcmc-nightly-0.0.8.dev20230420/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:56:49.423674 aemcmc-nightly-0.0.8.dev20230420/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/tests/test_conjugates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/tests/test_dists.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/tests/test_ffbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/tests/test_gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/tests/test_nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-04-20 00:56:38.000000 aemcmc-nightly-0.0.8.dev20230420/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:57:08.958845 aemcmc-nightly-0.0.8.dev20230421/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-21 00:57:08.958845 aemcmc-nightly-0.0.8.dev20230421/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:57:08.958845 aemcmc-nightly-0.0.8.dev20230421/aemcmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-21 00:57:08.958845 aemcmc-nightly-0.0.8.dev20230421/aemcmc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc/conjugates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc/ffbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24238 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc/gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:57:08.954846 aemcmc-nightly-0.0.8.dev20230421/aemcmc_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-21 00:57:08.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-21 00:57:08.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:57:08.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:57:08.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-21 00:57:08.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 00:57:08.000000 aemcmc-nightly-0.0.8.dev20230421/aemcmc_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-21 00:57:08.958845 aemcmc-nightly-0.0.8.dev20230421/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:57:08.958845 aemcmc-nightly-0.0.8.dev20230421/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/tests/test_conjugates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/tests/test_dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/tests/test_ffbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/tests/test_gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/tests/test_nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-04-21 00:56:46.000000 aemcmc-nightly-0.0.8.dev20230421/versioneer.py
```

### Comparing `aemcmc-nightly-0.0.8.dev20230420/LICENSE` & `aemcmc-nightly-0.0.8.dev20230421/LICENSE`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/PKG-INFO` & `aemcmc-nightly-0.0.8.dev20230421/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aemcmc-nightly
-Version: 0.0.8.dev20230420
+Version: 0.0.8.dev20230421
 Summary: Miscellaneous MCMC samplers written in Aesara
 Home-page: http://github.com/aesara-devs/aemcmc
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: math,probability,numerical,symbolic,MCMC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aemcmc-nightly-0.0.8.dev20230420/README.md` & `aemcmc-nightly-0.0.8.dev20230421/README.md`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/aemcmc/basic.py` & `aemcmc-nightly-0.0.8.dev20230421/aemcmc/basic.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/aemcmc/conjugates.py` & `aemcmc-nightly-0.0.8.dev20230421/aemcmc/conjugates.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/aemcmc/dists.py` & `aemcmc-nightly-0.0.8.dev20230421/aemcmc/dists.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/aemcmc/ffbs.py` & `aemcmc-nightly-0.0.8.dev20230421/aemcmc/ffbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/aemcmc/gibbs.py` & `aemcmc-nightly-0.0.8.dev20230421/aemcmc/gibbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/aemcmc/nuts.py` & `aemcmc-nightly-0.0.8.dev20230421/aemcmc/nuts.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/aemcmc/rewriting.py` & `aemcmc-nightly-0.0.8.dev20230421/aemcmc/rewriting.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/aemcmc/sample.py` & `aemcmc-nightly-0.0.8.dev20230421/aemcmc/sample.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/aemcmc/transforms.py` & `aemcmc-nightly-0.0.8.dev20230421/aemcmc/transforms.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/aemcmc/types.py` & `aemcmc-nightly-0.0.8.dev20230421/aemcmc/types.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/aemcmc/utils.py` & `aemcmc-nightly-0.0.8.dev20230421/aemcmc/utils.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/aemcmc_nightly.egg-info/PKG-INFO` & `aemcmc-nightly-0.0.8.dev20230421/aemcmc_nightly.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aemcmc-nightly
-Version: 0.0.8.dev20230420
+Version: 0.0.8.dev20230421
 Summary: Miscellaneous MCMC samplers written in Aesara
 Home-page: http://github.com/aesara-devs/aemcmc
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: math,probability,numerical,symbolic,MCMC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aemcmc-nightly-0.0.8.dev20230420/aemcmc_nightly.egg-info/SOURCES.txt` & `aemcmc-nightly-0.0.8.dev20230421/aemcmc_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/setup.cfg` & `aemcmc-nightly-0.0.8.dev20230421/setup.cfg`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/setup.py` & `aemcmc-nightly-0.0.8.dev20230421/setup.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/tests/test_basic.py` & `aemcmc-nightly-0.0.8.dev20230421/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/tests/test_conjugates.py` & `aemcmc-nightly-0.0.8.dev20230421/tests/test_conjugates.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/tests/test_dists.py` & `aemcmc-nightly-0.0.8.dev20230421/tests/test_dists.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/tests/test_ffbs.py` & `aemcmc-nightly-0.0.8.dev20230421/tests/test_ffbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/tests/test_gibbs.py` & `aemcmc-nightly-0.0.8.dev20230421/tests/test_gibbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/tests/test_nuts.py` & `aemcmc-nightly-0.0.8.dev20230421/tests/test_nuts.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/tests/test_rewriting.py` & `aemcmc-nightly-0.0.8.dev20230421/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/tests/test_sample.py` & `aemcmc-nightly-0.0.8.dev20230421/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/tests/test_transforms.py` & `aemcmc-nightly-0.0.8.dev20230421/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/tests/test_utils.py` & `aemcmc-nightly-0.0.8.dev20230421/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230420/versioneer.py` & `aemcmc-nightly-0.0.8.dev20230421/versioneer.py`

 * *Files identical despite different names*

