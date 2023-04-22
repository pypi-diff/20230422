# Comparing `tmp/salix-containers-0.3.1.tar.gz` & `tmp/salix-containers-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salix-containers-0.3.1.tar", max compression
+gzip compressed data, was "salix-containers-0.4.0.tar", max compression
```

## Comparing `salix-containers-0.3.1.tar` & `salix-containers-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0      331 2023-04-15 17:31:43.159609 salix-containers-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      153 2023-04-15 17:31:03.289609 salix-containers-0.3.1/salix_containers/__init__.py
--rw-r--r--   0        0        0     1039 2023-04-15 17:31:03.289609 salix-containers-0.3.1/salix_containers/caselessmapping.py
--rw-r--r--   0        0        0     1617 2022-04-16 20:28:31.676860 salix-containers-0.3.1/salix_containers/casttypes.py
--rw-r--r--   0        0        0        0 2023-04-15 16:49:10.619609 salix-containers-0.3.1/salix_containers/tests/__init__.py
--rw-r--r--   0        0        0     3537 2023-04-15 17:31:03.289609 salix-containers-0.3.1/salix_containers/tests/test_caselessmappings.py
--rw-r--r--   0        0        0      561 2023-04-15 17:32:56.424143 salix-containers-0.3.1/setup.py
--rw-r--r--   0        0        0      489 2023-04-15 17:32:56.424292 salix-containers-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      331 2023-04-22 15:28:52.433649 salix-containers-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      153 2023-04-15 17:31:03.289609 salix-containers-0.4.0/salix_containers/__init__.py
+-rw-r--r--   0        0        0     1039 2023-04-15 17:31:03.289609 salix-containers-0.4.0/salix_containers/caselessmapping.py
+-rw-r--r--   0        0        0     1617 2022-04-16 20:28:31.676860 salix-containers-0.4.0/salix_containers/casttypes.py
+-rw-r--r--   0        0        0      452 2023-04-22 14:46:09.483649 salix-containers-0.4.0/salix_containers/empty.py
+-rw-r--r--   0        0        0        0 2023-04-15 16:49:10.619609 salix-containers-0.4.0/salix_containers/tests/__init__.py
+-rw-r--r--   0        0        0     3591 2023-04-22 14:54:07.813649 salix-containers-0.4.0/salix_containers/tests/test_caselessmappings.py
+-rw-r--r--   0        0        0     2669 2023-04-22 14:54:39.073649 salix-containers-0.4.0/salix_containers/tests/test_casttypes.py
+-rw-r--r--   0        0        0     1370 2023-04-22 15:17:50.143649 salix-containers-0.4.0/salix_containers/tests/test_empty.py
+-rw-r--r--   0        0        0      561 2023-04-22 15:30:14.237765 salix-containers-0.4.0/setup.py
+-rw-r--r--   0        0        0      489 2023-04-22 15:30:14.237988 salix-containers-0.4.0/PKG-INFO
```

### Comparing `salix-containers-0.3.1/salix_containers/caselessmapping.py` & `salix-containers-0.4.0/salix_containers/caselessmapping.py`

 * *Files identical despite different names*

### Comparing `salix-containers-0.3.1/salix_containers/casttypes.py` & `salix-containers-0.4.0/salix_containers/casttypes.py`

 * *Files identical despite different names*

### Comparing `salix-containers-0.3.1/salix_containers/tests/test_caselessmappings.py` & `salix-containers-0.4.0/salix_containers/tests/test_caselessmappings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Run via python -m unittest in parent folder
+
+"""
+
 
 from unittest import TestCase
 
 from caselessmapping import CaselessMapping, CaselessMutableMapping
 
 
 class TestCaselessMapping(TestCase):
```

### Comparing `salix-containers-0.3.1/setup.py` & `salix-containers-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['salix_containers', 'salix_containers.tests']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'salix-containers',
-    'version': '0.3.1',
+    'version': '0.4.0',
     'description': 'Occasionally handy container types',
     'long_description': None,
     'author': 'Salix',
     'author_email': 'salix@pilae.net',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

