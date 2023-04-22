# Comparing `tmp/pygismeteo_base-4.4.0.tar.gz` & `tmp/pygismeteo_base-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygismeteo_base-4.4.0.tar", max compression
+gzip compressed data, was "pygismeteo_base-4.4.1.tar", max compression
```

## Comparing `pygismeteo_base-4.4.0.tar` & `pygismeteo_base-4.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1065 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.0/LICENSE
--rw-r--r--   0        0        0      553 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.0/README.md
--rw-r--r--   0        0        0       86 2023-04-21 20:36:29.353649 pygismeteo_base-4.4.0/pygismeteo_base/__init__.py
--rw-r--r--   0        0        0       92 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.0/pygismeteo_base/constants.py
--rw-r--r--   0        0        0      925 2023-04-21 19:11:10.073668 pygismeteo_base-4.4.0/pygismeteo_base/current.py
--rw-r--r--   0        0        0      392 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.0/pygismeteo_base/endpoint.py
--rw-r--r--   0        0        0      901 2023-04-21 19:29:03.763651 pygismeteo_base-4.4.0/pygismeteo_base/http.py
--rw-r--r--   0        0        0      309 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.0/pygismeteo_base/models/__init__.py
--rw-r--r--   0        0        0     1812 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.0/pygismeteo_base/models/current.py
--rw-r--r--   0        0        0      759 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.0/pygismeteo_base/models/search_by_coordinates.py
--rw-r--r--   0        0        0      673 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.0/pygismeteo_base/models/search_by_ip.py
--rw-r--r--   0        0        0      783 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.0/pygismeteo_base/models/search_by_query.py
--rw-r--r--   0        0        0     2908 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.0/pygismeteo_base/models/step24.py
--rw-r--r--   0        0        0     1786 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.0/pygismeteo_base/models/step3.py
--rw-r--r--   0        0        0     1803 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.0/pygismeteo_base/models/step6.py
--rw-r--r--   0        0        0        0 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.0/pygismeteo_base/py.typed
--rw-r--r--   0        0        0     1223 2023-04-22 07:03:15.526346 pygismeteo_base-4.4.0/pygismeteo_base/search.py
--rw-r--r--   0        0        0        0 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.0/pygismeteo_base/step_n/__init__.py
--rw-r--r--   0        0        0     1452 2023-04-21 19:55:58.533667 pygismeteo_base-4.4.0/pygismeteo_base/step_n/abc.py
--rw-r--r--   0        0        0     1609 2023-04-21 19:56:30.993669 pygismeteo_base-4.4.0/pygismeteo_base/step_n/mixins.py
--rw-r--r--   0        0        0     1308 2023-04-21 19:55:05.883666 pygismeteo_base-4.4.0/pygismeteo_base/types.py
--rw-r--r--   0        0        0      400 2023-04-21 18:50:04.713658 pygismeteo_base-4.4.0/pygismeteo_base/typing_compat.py
--rw-r--r--   0        0        0      914 2023-04-22 07:03:10.606346 pygismeteo_base-4.4.0/pygismeteo_base/validators.py
--rw-r--r--   0        0        0     2706 2023-04-22 07:04:48.776337 pygismeteo_base-4.4.0/pyproject.toml
--rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 pygismeteo_base-4.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/LICENSE
+-rw-r--r--   0        0        0      553 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/README.md
+-rw-r--r--   0        0        0       86 2023-04-21 20:36:29.353649 pygismeteo_base-4.4.1/pygismeteo_base/__init__.py
+-rw-r--r--   0        0        0       92 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/constants.py
+-rw-r--r--   0        0        0      925 2023-04-21 19:11:10.073668 pygismeteo_base-4.4.1/pygismeteo_base/current.py
+-rw-r--r--   0        0        0      392 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/endpoint.py
+-rw-r--r--   0        0        0      901 2023-04-21 19:29:03.763651 pygismeteo_base-4.4.1/pygismeteo_base/http.py
+-rw-r--r--   0        0        0      366 2023-04-22 18:01:28.729243 pygismeteo_base-4.4.1/pygismeteo_base/models/__init__.py
+-rw-r--r--   0        0        0     1812 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/models/current.py
+-rw-r--r--   0        0        0      759 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/models/search_by_coordinates.py
+-rw-r--r--   0        0        0      673 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/models/search_by_ip.py
+-rw-r--r--   0        0        0      783 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/models/search_by_query.py
+-rw-r--r--   0        0        0     2908 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/models/step24.py
+-rw-r--r--   0        0        0     1786 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/models/step3.py
+-rw-r--r--   0        0        0     1803 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/models/step6.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/py.typed
+-rw-r--r--   0        0        0     1223 2023-04-22 07:03:15.526346 pygismeteo_base-4.4.1/pygismeteo_base/search.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/step_n/__init__.py
+-rw-r--r--   0        0        0     1452 2023-04-21 19:55:58.533667 pygismeteo_base-4.4.1/pygismeteo_base/step_n/abc.py
+-rw-r--r--   0        0        0     1609 2023-04-21 19:56:30.993669 pygismeteo_base-4.4.1/pygismeteo_base/step_n/mixins.py
+-rw-r--r--   0        0        0     1816 2023-04-22 18:10:34.669234 pygismeteo_base-4.4.1/pygismeteo_base/types.py
+-rw-r--r--   0        0        0      400 2023-04-21 18:50:04.713658 pygismeteo_base-4.4.1/pygismeteo_base/typing_compat.py
+-rw-r--r--   0        0        0      914 2023-04-22 07:03:10.606346 pygismeteo_base-4.4.1/pygismeteo_base/validators.py
+-rw-r--r--   0        0        0     2706 2023-04-22 18:11:26.199232 pygismeteo_base-4.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 pygismeteo_base-4.4.1/PKG-INFO
```

### Comparing `pygismeteo_base-4.4.0/LICENSE` & `pygismeteo_base-4.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.0/README.md` & `pygismeteo_base-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.0/pygismeteo_base/current.py` & `pygismeteo_base-4.4.1/pygismeteo_base/current.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.0/pygismeteo_base/http.py` & `pygismeteo_base-4.4.1/pygismeteo_base/http.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.0/pygismeteo_base/models/current.py` & `pygismeteo_base-4.4.1/pygismeteo_base/models/current.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.0/pygismeteo_base/models/search_by_coordinates.py` & `pygismeteo_base-4.4.1/pygismeteo_base/models/search_by_coordinates.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.0/pygismeteo_base/models/search_by_ip.py` & `pygismeteo_base-4.4.1/pygismeteo_base/models/search_by_ip.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.0/pygismeteo_base/models/search_by_query.py` & `pygismeteo_base-4.4.1/pygismeteo_base/models/search_by_query.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.0/pygismeteo_base/models/step24.py` & `pygismeteo_base-4.4.1/pygismeteo_base/models/step24.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.0/pygismeteo_base/models/step3.py` & `pygismeteo_base-4.4.1/pygismeteo_base/models/step3.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.0/pygismeteo_base/models/step6.py` & `pygismeteo_base-4.4.1/pygismeteo_base/models/step6.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.0/pygismeteo_base/search.py` & `pygismeteo_base-4.4.1/pygismeteo_base/search.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.0/pygismeteo_base/step_n/abc.py` & `pygismeteo_base-4.4.1/pygismeteo_base/step_n/abc.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.0/pygismeteo_base/step_n/mixins.py` & `pygismeteo_base-4.4.1/pygismeteo_base/step_n/mixins.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.0/pygismeteo_base/validators.py` & `pygismeteo_base-4.4.1/pygismeteo_base/validators.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.0/pyproject.toml` & `pygismeteo_base-4.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygismeteo-base"
-version = "4.4.0"
+version = "4.4.1"
 description = "Base for pygismeteo and aiopygismeteo"
 authors = ["monosans <hsyqixco@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/monosans/pygismeteo-base"
 classifiers = [
     "Environment :: Web Environment",
```

### Comparing `pygismeteo_base-4.4.0/PKG-INFO` & `pygismeteo_base-4.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygismeteo-base
-Version: 4.4.0
+Version: 4.4.1
 Summary: Base for pygismeteo and aiopygismeteo
 Home-page: https://github.com/monosans/pygismeteo-base
 License: MIT
 Author: monosans
 Author-email: hsyqixco@protonmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Web Environment
```

