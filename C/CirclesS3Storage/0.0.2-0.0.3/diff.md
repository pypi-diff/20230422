# Comparing `tmp/CirclesS3Storage-0.0.2.tar.gz` & `tmp/CirclesS3Storage-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CirclesS3Storage-0.0.2.tar", last modified: Sat Apr 22 10:02:16 2023, max compression
+gzip compressed data, was "CirclesS3Storage-0.0.3.tar", last modified: Sat Apr 22 10:06:57 2023, max compression
```

## Comparing `CirclesS3Storage-0.0.2.tar` & `CirclesS3Storage-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:02:16.222052 CirclesS3Storage-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:02:16.222052 CirclesS3Storage-0.0.2/CirclesS3Storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-22 10:02:16.000000 CirclesS3Storage-0.0.2/CirclesS3Storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-22 10:02:16.000000 CirclesS3Storage-0.0.2/CirclesS3Storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 10:02:16.000000 CirclesS3Storage-0.0.2/CirclesS3Storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 10:02:16.000000 CirclesS3Storage-0.0.2/CirclesS3Storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-22 10:02:16.222052 CirclesS3Storage-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:02:16.222052 CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/AWSStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/CirclesStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/FileTypeDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/StorageDB.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/StorageInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 10:02:16.222052 CirclesS3Storage-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:02:16.222052 CirclesS3Storage-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/tests/test_S3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/tests/test_circles_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:06:57.560237 CirclesS3Storage-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:06:57.560237 CirclesS3Storage-0.0.3/CirclesS3Storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-22 10:06:57.000000 CirclesS3Storage-0.0.3/CirclesS3Storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-22 10:06:57.000000 CirclesS3Storage-0.0.3/CirclesS3Storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 10:06:57.000000 CirclesS3Storage-0.0.3/CirclesS3Storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 10:06:57.000000 CirclesS3Storage-0.0.3/CirclesS3Storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-22 10:06:57.560237 CirclesS3Storage-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-22 10:06:30.000000 CirclesS3Storage-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:06:57.560237 CirclesS3Storage-0.0.3/circles_local_aws_s3_storage_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-22 10:06:30.000000 CirclesS3Storage-0.0.3/circles_local_aws_s3_storage_python/AWSStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-22 10:06:30.000000 CirclesS3Storage-0.0.3/circles_local_aws_s3_storage_python/CirclesStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-22 10:06:30.000000 CirclesS3Storage-0.0.3/circles_local_aws_s3_storage_python/FileTypeDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-22 10:06:30.000000 CirclesS3Storage-0.0.3/circles_local_aws_s3_storage_python/StorageDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-22 10:06:30.000000 CirclesS3Storage-0.0.3/circles_local_aws_s3_storage_python/StorageInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 10:06:30.000000 CirclesS3Storage-0.0.3/circles_local_aws_s3_storage_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-22 10:06:30.000000 CirclesS3Storage-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 10:06:57.560237 CirclesS3Storage-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-22 10:06:30.000000 CirclesS3Storage-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:06:57.560237 CirclesS3Storage-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 10:06:30.000000 CirclesS3Storage-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-22 10:06:30.000000 CirclesS3Storage-0.0.3/tests/test_S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-22 10:06:30.000000 CirclesS3Storage-0.0.3/tests/test_circles_storage.py
```

### Comparing `CirclesS3Storage-0.0.2/CirclesS3Storage.egg-info/SOURCES.txt` & `CirclesS3Storage-0.0.3/CirclesS3Storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/AWSStorage.py` & `CirclesS3Storage-0.0.3/circles_local_aws_s3_storage_python/AWSStorage.py`

 * *Files identical despite different names*

### Comparing `CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/CirclesStorage.py` & `CirclesS3Storage-0.0.3/circles_local_aws_s3_storage_python/CirclesStorage.py`

 * *Files identical despite different names*

### Comparing `CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/FileTypeDB.py` & `CirclesS3Storage-0.0.3/circles_local_aws_s3_storage_python/FileTypeDB.py`

 * *Files identical despite different names*

### Comparing `CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/StorageDB.py` & `CirclesS3Storage-0.0.3/circles_local_aws_s3_storage_python/StorageDB.py`

 * *Files identical despite different names*

### Comparing `CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/StorageInterface.py` & `CirclesS3Storage-0.0.3/circles_local_aws_s3_storage_python/StorageInterface.py`

 * *Files identical despite different names*

### Comparing `CirclesS3Storage-0.0.2/setup.py` & `CirclesS3Storage-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='CirclesS3Storage',
-    version='0.0.2',
+    version='0.0.3',
     author="Circles",
     author_email="info@circle.zone",
     description="PyPI Package for Circles S3 functions",
     long_description="This is a package for sharing common S3 function used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/javatechy/dokr",
     packages=setuptools.find_packages(),
```

### Comparing `CirclesS3Storage-0.0.2/tests/test_S3.py` & `CirclesS3Storage-0.0.3/tests/test_S3.py`

 * *Files identical despite different names*

### Comparing `CirclesS3Storage-0.0.2/tests/test_circles_storage.py` & `CirclesS3Storage-0.0.3/tests/test_circles_storage.py`

 * *Files identical despite different names*

