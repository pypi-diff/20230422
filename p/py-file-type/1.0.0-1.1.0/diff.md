# Comparing `tmp/py_file_type-1.0.0.tar.gz` & `tmp/py_file_type-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_file_type-1.0.0.tar", last modified: Sat Apr 22 19:46:42 2023, max compression
+gzip compressed data, was "py_file_type-1.1.0.tar", last modified: Sat Apr 22 19:57:14 2023, max compression
```

## Comparing `py_file_type-1.0.0.tar` & `py_file_type-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 19:46:42.910518 py_file_type-1.0.0/
--rw-rw-rw-   0        0        0     1553 2023-04-22 19:46:42.909518 py_file_type-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      808 2023-04-22 19:40:14.000000 py_file_type-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 19:46:42.889518 py_file_type-1.0.0/py_file_type/
--rw-rw-rw-   0        0        0       44 2023-04-22 19:13:45.000000 py_file_type-1.0.0/py_file_type/__init__.py
--rw-rw-rw-   0        0        0     8316 2023-04-22 19:12:40.000000 py_file_type-1.0.0/py_file_type/compat.py
--rw-rw-rw-   0        0        0     1168 2023-04-22 19:12:40.000000 py_file_type-1.0.0/py_file_type/loader.py
--rw-rw-rw-   0        0        0     9840 2023-04-22 19:13:45.000000 py_file_type-1.0.0/py_file_type/magic.py
-drwxrwxrwx   0        0        0        0 2023-04-22 19:46:42.908517 py_file_type-1.0.0/py_file_type.egg-info/
--rw-rw-rw-   0        0        0     1553 2023-04-22 19:46:42.000000 py_file_type-1.0.0/py_file_type.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-04-22 19:46:42.000000 py_file_type-1.0.0/py_file_type.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 19:46:42.000000 py_file_type-1.0.0/py_file_type.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-22 19:46:42.000000 py_file_type-1.0.0/py_file_type.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 19:46:42.910518 py_file_type-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-04-22 19:46:26.000000 py_file_type-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 19:57:14.168851 py_file_type-1.1.0/
+-rw-rw-rw-   0        0        0     1553 2023-04-22 19:57:14.167834 py_file_type-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      808 2023-04-22 19:40:14.000000 py_file_type-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 19:57:14.139835 py_file_type-1.1.0/py_file_type/
+-rw-rw-rw-   0        0        0       44 2023-04-22 19:13:45.000000 py_file_type-1.1.0/py_file_type/__init__.py
+-rw-rw-rw-   0        0        0     8316 2023-04-22 19:12:40.000000 py_file_type-1.1.0/py_file_type/compat.py
+drwxrwxrwx   0        0        0        0 2023-04-22 19:57:14.158834 py_file_type-1.1.0/py_file_type/libmagic/
+-rw-rw-rw-   0        0        0   347136 2023-04-22 19:13:45.000000 py_file_type-1.1.0/py_file_type/libmagic/libmagic.dll
+-rw-rw-rw-   0        0        0  4917824 2023-04-22 19:13:45.000000 py_file_type-1.1.0/py_file_type/libmagic/magic.mgc
+-rw-rw-rw-   0        0        0     1168 2023-04-22 19:12:40.000000 py_file_type-1.1.0/py_file_type/loader.py
+-rw-rw-rw-   0        0        0     9840 2023-04-22 19:13:45.000000 py_file_type-1.1.0/py_file_type/magic.py
+drwxrwxrwx   0        0        0        0 2023-04-22 19:57:14.154835 py_file_type-1.1.0/py_file_type.egg-info/
+-rw-rw-rw-   0        0        0     1553 2023-04-22 19:57:14.000000 py_file_type-1.1.0/py_file_type.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-04-22 19:57:14.000000 py_file_type-1.1.0/py_file_type.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 19:57:14.000000 py_file_type-1.1.0/py_file_type.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-22 19:57:14.000000 py_file_type-1.1.0/py_file_type.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 19:57:14.169834 py_file_type-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1485 2023-04-22 19:57:11.000000 py_file_type-1.1.0/setup.py
```

### Comparing `py_file_type-1.0.0/PKG-INFO` & `py_file_type-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_file_type
-Version: 1.0.0
+Version: 1.1.0
 Summary: Wrapper for python-magic that includes necessary bin files.
 Home-page: https://github.com/riad-azz/py-file-type
 Author: riad-azz
 Author-email: riadh.azzoun@hotmail.com
 License: MIT License
 Project-URL: Source, https://github.com/riad-azz/py-file-type
 Keywords: python-magic wrapper,python-magic-bin,python-magic binaries,libmagic
```

### Comparing `py_file_type-1.0.0/README.md` & `py_file_type-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `py_file_type-1.0.0/py_file_type/compat.py` & `py_file_type-1.1.0/py_file_type/compat.py`

 * *Files identical despite different names*

### Comparing `py_file_type-1.0.0/py_file_type/loader.py` & `py_file_type-1.1.0/py_file_type/loader.py`

 * *Files identical despite different names*

### Comparing `py_file_type-1.0.0/py_file_type/magic.py` & `py_file_type-1.1.0/py_file_type/magic.py`

 * *Files identical despite different names*

### Comparing `py_file_type-1.0.0/py_file_type.egg-info/PKG-INFO` & `py_file_type-1.1.0/py_file_type.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-file-type
-Version: 1.0.0
+Version: 1.1.0
 Summary: Wrapper for python-magic that includes necessary bin files.
 Home-page: https://github.com/riad-azz/py-file-type
 Author: riad-azz
 Author-email: riadh.azzoun@hotmail.com
 License: MIT License
 Project-URL: Source, https://github.com/riad-azz/py-file-type
 Keywords: python-magic wrapper,python-magic-bin,python-magic binaries,libmagic
```

### Comparing `py_file_type-1.0.0/setup.py` & `py_file_type-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,27 +10,28 @@
 
 
 long_description = open('README.md').read()
 long_description_content_type = 'text/markdown'
 
 setup(
     name='py_file_type',
-    version='1.0.0',
+    version='1.1.0',
     author='riad-azz',
     author_email='riadh.azzoun@hotmail.com',
     description='Wrapper for python-magic that includes necessary bin files.',
     long_description=long_description,
     long_description_content_type=long_description_content_type,
     url='https://github.com/riad-azz/py-file-type',
     project_urls={
         "Source": "https://github.com/riad-azz/py-file-type",
     },
     packages=find_packages(exclude=["docs", "tests"]),
     license="MIT License",
     keywords=["python-magic wrapper", "python-magic-bin", "python-magic binaries", "libmagic"],
+    data_files=[('py_file_type', ['./py_file_type/libmagic/libmagic.dll', './py_file_type/libmagic/magic.mgc'])],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

