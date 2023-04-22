# Comparing `tmp/osrs-lib-0.1.0.tar.gz` & `tmp/osrs-lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osrs-lib-0.1.0.tar", last modified: Thu Feb 23 03:43:24 2023, max compression
+gzip compressed data, was "osrs-lib-0.1.1.tar", last modified: Sat Apr 22 21:08:37 2023, max compression
```

## Comparing `osrs-lib-0.1.0.tar` & `osrs-lib-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-02-23 03:43:24.889291 osrs-lib-0.1.0/
--rw-r--r--   0 peter     (1000) peter     (1000)    11357 2023-02-22 21:55:07.000000 osrs-lib-0.1.0/LICENSE
--rw-r--r--   0 peter     (1000) peter     (1000)      469 2023-02-23 03:43:24.889291 osrs-lib-0.1.0/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     1249 2023-02-23 03:26:10.000000 osrs-lib-0.1.0/README.md
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-02-23 03:43:24.889291 osrs-lib-0.1.0/osrs-lib/
--rw-r--r--   0 peter     (1000) peter     (1000)      794 2023-02-23 03:38:15.000000 osrs-lib-0.1.0/osrs-lib/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      887 2023-02-23 03:26:08.000000 osrs-lib-0.1.0/osrs-lib/errors.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4465 2023-02-23 03:32:58.000000 osrs-lib-0.1.0/osrs-lib/hiscores.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1217 2023-02-22 21:55:36.000000 osrs-lib-0.1.0/osrs-lib/utils.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-02-23 03:43:24.889291 osrs-lib-0.1.0/osrs_lib.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)      469 2023-02-23 03:43:24.000000 osrs-lib-0.1.0/osrs_lib.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      264 2023-02-23 03:43:24.000000 osrs-lib-0.1.0/osrs_lib.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-02-23 03:43:24.000000 osrs-lib-0.1.0/osrs_lib.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       20 2023-02-23 03:43:24.000000 osrs-lib-0.1.0/osrs_lib.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        9 2023-02-23 03:43:24.000000 osrs-lib-0.1.0/osrs_lib.egg-info/top_level.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-02-23 03:43:24.889291 osrs-lib-0.1.0/setup.cfg
--rw-r--r--   0 peter     (1000) peter     (1000)      671 2023-02-23 03:43:10.000000 osrs-lib-0.1.0/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 21:08:37.841650 osrs-lib-0.1.1/
+-rw-r--r--   0 peter     (1000) peter     (1000)    11357 2023-02-22 21:55:07.000000 osrs-lib-0.1.1/LICENSE
+-rw-r--r--   0 peter     (1000) peter     (1000)      509 2023-04-22 21:08:37.841650 osrs-lib-0.1.1/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     1249 2023-02-23 03:26:10.000000 osrs-lib-0.1.1/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 21:08:37.841650 osrs-lib-0.1.1/osrs_lib/
+-rw-r--r--   0 peter     (1000) peter     (1000)      794 2023-02-23 03:38:15.000000 osrs-lib-0.1.1/osrs_lib/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      887 2023-02-23 03:26:08.000000 osrs-lib-0.1.1/osrs_lib/errors.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4465 2023-04-22 21:02:59.000000 osrs-lib-0.1.1/osrs_lib/hiscores.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1217 2023-02-22 21:55:36.000000 osrs-lib-0.1.1/osrs_lib/utils.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 21:08:37.841650 osrs-lib-0.1.1/osrs_lib.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)      509 2023-04-22 21:08:37.000000 osrs-lib-0.1.1/osrs_lib.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      264 2023-04-22 21:08:37.000000 osrs-lib-0.1.1/osrs_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-22 21:08:37.000000 osrs-lib-0.1.1/osrs_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       20 2023-04-22 21:08:37.000000 osrs-lib-0.1.1/osrs_lib.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        9 2023-04-22 21:08:37.000000 osrs-lib-0.1.1/osrs_lib.egg-info/top_level.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-04-22 21:08:37.841650 osrs-lib-0.1.1/setup.cfg
+-rw-r--r--   0 peter     (1000) peter     (1000)      722 2023-04-22 21:08:35.000000 osrs-lib-0.1.1/setup.py
```

### Comparing `osrs-lib-0.1.0/LICENSE` & `osrs-lib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `osrs-lib-0.1.0/README.md` & `osrs-lib-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `osrs-lib-0.1.0/osrs-lib/__init__.py` & `osrs-lib-0.1.1/osrs_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `osrs-lib-0.1.0/osrs-lib/errors.py` & `osrs-lib-0.1.1/osrs_lib/errors.py`

 * *Files identical despite different names*

### Comparing `osrs-lib-0.1.0/osrs-lib/hiscores.py` & `osrs-lib-0.1.1/osrs_lib/hiscores.py`

 * *Files identical despite different names*

### Comparing `osrs-lib-0.1.0/osrs-lib/utils.py` & `osrs-lib-0.1.1/osrs_lib/utils.py`

 * *Files identical despite different names*

### Comparing `osrs-lib-0.1.0/setup.py` & `osrs-lib-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup
 
 setup(
     name='osrs-lib',
-    version='0.1.0',
+    version='0.1.1',
     description='An OSRS library',
     url='https://github.com/shumatepf/osrs-lib',
     author='shumatepf',
     author_email='shumatepfs@gmail.com',
     license='Apache 2.0',
-    packages=['osrs-lib'],
+    packages=['osrs_lib'],
     install_requires=['bs4',
                       'asyncio',
                       'aiohttp',
                       ],
+    long_description_content_type='text/markdown',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 3.11',
     ],
```

