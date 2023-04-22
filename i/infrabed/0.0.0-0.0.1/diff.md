# Comparing `tmp/infrabed-0.0.0.tar.gz` & `tmp/infrabed-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrabed-0.0.0.tar", last modified: Sat Apr 22 20:48:40 2023, max compression
+gzip compressed data, was "infrabed-0.0.1.tar", last modified: Sat Apr 22 21:10:51 2023, max compression
```

## Comparing `infrabed-0.0.0.tar` & `infrabed-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-22 20:48:40.956434 infrabed-0.0.0/
--rw-rw-r--   0 yamen     (1000) yamen     (1000)     1119 2023-04-22 20:48:40.956434 infrabed-0.0.0/PKG-INFO
-drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-22 20:48:40.956434 infrabed-0.0.0/infrabed.egg-info/
--rw-rw-r--   0 yamen     (1000) yamen     (1000)     1119 2023-04-22 20:48:40.000000 infrabed-0.0.0/infrabed.egg-info/PKG-INFO
--rw-rw-r--   0 yamen     (1000) yamen     (1000)      167 2023-04-22 20:48:40.000000 infrabed-0.0.0/infrabed.egg-info/SOURCES.txt
--rw-rw-r--   0 yamen     (1000) yamen     (1000)        1 2023-04-22 20:48:40.000000 infrabed-0.0.0/infrabed.egg-info/dependency_links.txt
--rw-rw-r--   0 yamen     (1000) yamen     (1000)       34 2023-04-22 20:48:40.000000 infrabed-0.0.0/infrabed.egg-info/requires.txt
--rw-rw-r--   0 yamen     (1000) yamen     (1000)        1 2023-04-22 20:48:40.000000 infrabed-0.0.0/infrabed.egg-info/top_level.txt
--rw-rw-r--   0 yamen     (1000) yamen     (1000)       38 2023-04-22 20:48:40.956434 infrabed-0.0.0/setup.cfg
--rw-rw-r--   0 yamen     (1000) yamen     (1000)     1407 2023-04-22 20:42:26.000000 infrabed-0.0.0/setup.py
+drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-22 21:10:51.881182 infrabed-0.0.1/
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)     1053 2023-04-22 21:10:51.881182 infrabed-0.0.1/PKG-INFO
+drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-22 21:10:51.881182 infrabed-0.0.1/infrabed.egg-info/
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)     1053 2023-04-22 21:10:51.000000 infrabed-0.0.1/infrabed.egg-info/PKG-INFO
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)      167 2023-04-22 21:10:51.000000 infrabed-0.0.1/infrabed.egg-info/SOURCES.txt
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)        1 2023-04-22 21:10:51.000000 infrabed-0.0.1/infrabed.egg-info/dependency_links.txt
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)       29 2023-04-22 21:10:51.000000 infrabed-0.0.1/infrabed.egg-info/requires.txt
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)        1 2023-04-22 21:10:51.000000 infrabed-0.0.1/infrabed.egg-info/top_level.txt
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)       38 2023-04-22 21:10:51.881182 infrabed-0.0.1/setup.cfg
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)     1399 2023-04-22 21:10:08.000000 infrabed-0.0.1/setup.py
```

### Comparing `infrabed-0.0.0/PKG-INFO` & `infrabed-0.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: infrabed
-Version: 0.0.0
+Version: 0.0.1
 Summary: Python library designed to simplify client-side interaction with deep learning models that perform embedding calculations.
-Home-page: UNKNOWN
 Author: DepDiko
 Author-email: <yamen.habib@depdiko.com>
-License: UNKNOWN
-Description: With this library, users can easily interface with APIs that provide embedding services, allowing them to quickly generate high-quality embeddings for a wide range of natural language processing (NLP) tasks. Whether you need to perform sentiment analysis, semantic similarity matching, or any other task that requires the use of embeddings, Embedding Client makes it easy to access the power of deep learning models from within your Python environment.
 Keywords: python,embedding,deep learning
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+
+With this library, users can easily interface with APIs that provide embedding services, allowing them to quickly generate high-quality embeddings for a wide range of natural language processing (NLP) tasks. Whether you need to perform sentiment analysis, semantic similarity matching, or any other task that requires the use of embeddings, Embedding Client makes it easy to access the power of deep learning models from within your Python environment.
```

### Comparing `infrabed-0.0.0/infrabed.egg-info/PKG-INFO` & `infrabed-0.0.1/infrabed.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: infrabed
-Version: 0.0.0
+Version: 0.0.1
 Summary: Python library designed to simplify client-side interaction with deep learning models that perform embedding calculations.
-Home-page: UNKNOWN
 Author: DepDiko
 Author-email: <yamen.habib@depdiko.com>
-License: UNKNOWN
-Description: With this library, users can easily interface with APIs that provide embedding services, allowing them to quickly generate high-quality embeddings for a wide range of natural language processing (NLP) tasks. Whether you need to perform sentiment analysis, semantic similarity matching, or any other task that requires the use of embeddings, Embedding Client makes it easy to access the power of deep learning models from within your Python environment.
 Keywords: python,embedding,deep learning
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+
+With this library, users can easily interface with APIs that provide embedding services, allowing them to quickly generate high-quality embeddings for a wide range of natural language processing (NLP) tasks. Whether you need to perform sentiment analysis, semantic similarity matching, or any other task that requires the use of embeddings, Embedding Client makes it easy to access the power of deep learning models from within your Python environment.
```

### Comparing `infrabed-0.0.0/setup.py` & `infrabed-0.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
 
-VERSION = '0.0.0'
+VERSION = '0.0.1'
 DESCRIPTION = 'Python library designed to simplify client-side interaction with deep learning models that perform embedding calculations.'
 LONG_DESCRIPTION = 'With this library, users can easily interface with APIs that provide embedding services, allowing them to quickly generate high-quality embeddings for a wide range of natural language processing (NLP) tasks. Whether you need to perform sentiment analysis, semantic similarity matching, or any other task that requires the use of embeddings, Embedding Client makes it easy to access the power of deep learning models from within your Python environment.'
 
 # Setting up
 setup(
     name="infrabed",
     version=VERSION,
     author="DepDiko",
     author_email="<yamen.habib@depdiko.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['requests', 'base64',  'hashlib', 'hmac', 'json'],
+    install_requires=['requests', 'base64',  'hashlib', 'hmac'],
     keywords=['python', 'embedding', 'deep learning'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

