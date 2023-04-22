# Comparing `tmp/smartsheet-pydantic-1.0.1.tar.gz` & `tmp/smartsheet-pydantic-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartsheet-pydantic-1.0.1.tar", last modified: Sat Apr 22 16:46:03 2023, max compression
+gzip compressed data, was "smartsheet-pydantic-1.1.0.tar", last modified: Sat Apr 22 21:38:20 2023, max compression
```

## Comparing `smartsheet-pydantic-1.0.1.tar` & `smartsheet-pydantic-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-22 16:46:03.694806 smartsheet-pydantic-1.0.1/
--rw-r--r--   0 tak       (1000) tak       (1000)     1091 2023-04-22 15:28:56.000000 smartsheet-pydantic-1.0.1/LICENSE
--rw-r--r--   0 tak       (1000) tak       (1000)       53 2023-04-22 15:28:20.000000 smartsheet-pydantic-1.0.1/MANIFEST.in
--rw-r--r--   0 tak       (1000) tak       (1000)     1811 2023-04-22 16:46:03.694806 smartsheet-pydantic-1.0.1/PKG-INFO
--rw-r--r--   0 tak       (1000) tak       (1000)      162 2023-04-22 14:53:39.000000 smartsheet-pydantic-1.0.1/README.md
--rw-r--r--   0 tak       (1000) tak       (1000)      811 2023-04-22 16:45:20.000000 smartsheet-pydantic-1.0.1/pyproject.toml
--rw-r--r--   0 tak       (1000) tak       (1000)       38 2023-04-22 16:46:03.694806 smartsheet-pydantic-1.0.1/setup.cfg
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-22 16:46:03.694806 smartsheet-pydantic-1.0.1/src/
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-22 16:46:03.694806 smartsheet-pydantic-1.0.1/src/smartsheet_pydantic/
--rw-r--r--   0 tak       (1000) tak       (1000)        0 2023-04-22 14:53:46.000000 smartsheet-pydantic-1.0.1/src/smartsheet_pydantic/__init__.py
--rw-r--r--   0 tak       (1000) tak       (1000)     6732 2023-04-22 16:41:51.000000 smartsheet-pydantic-1.0.1/src/smartsheet_pydantic/controller.py
--rw-r--r--   0 tak       (1000) tak       (1000)      493 2023-04-22 14:53:20.000000 smartsheet-pydantic-1.0.1/src/smartsheet_pydantic/debug_logger.py
--rw-r--r--   0 tak       (1000) tak       (1000)     2816 2023-04-22 15:44:48.000000 smartsheet-pydantic-1.0.1/src/smartsheet_pydantic/filters.py
--rw-r--r--   0 tak       (1000) tak       (1000)     8452 2023-04-22 15:43:30.000000 smartsheet-pydantic-1.0.1/src/smartsheet_pydantic/smartmodels.py
--rw-r--r--   0 tak       (1000) tak       (1000)     1145 2023-04-22 15:43:35.000000 smartsheet-pydantic-1.0.1/src/smartsheet_pydantic/sources.py
--rw-r--r--   0 tak       (1000) tak       (1000)     2327 2023-04-22 15:45:13.000000 smartsheet-pydantic-1.0.1/src/smartsheet_pydantic/transformer.py
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-22 16:46:03.694806 smartsheet-pydantic-1.0.1/src/smartsheet_pydantic.egg-info/
--rw-r--r--   0 tak       (1000) tak       (1000)     1811 2023-04-22 16:46:03.000000 smartsheet-pydantic-1.0.1/src/smartsheet_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 tak       (1000) tak       (1000)      634 2023-04-22 16:46:03.000000 smartsheet-pydantic-1.0.1/src/smartsheet_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 tak       (1000) tak       (1000)        1 2023-04-22 16:46:03.000000 smartsheet-pydantic-1.0.1/src/smartsheet_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 tak       (1000) tak       (1000)      102 2023-04-22 16:46:03.000000 smartsheet-pydantic-1.0.1/src/smartsheet_pydantic.egg-info/requires.txt
--rw-r--r--   0 tak       (1000) tak       (1000)       20 2023-04-22 16:46:03.000000 smartsheet-pydantic-1.0.1/src/smartsheet_pydantic.egg-info/top_level.txt
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-22 16:46:03.694806 smartsheet-pydantic-1.0.1/tests/
--rw-r--r--   0 tak       (1000) tak       (1000)     3924 2023-04-22 16:43:42.000000 smartsheet-pydantic-1.0.1/tests/test_controller.py
--rw-r--r--   0 tak       (1000) tak       (1000)     3527 2023-04-22 16:01:06.000000 smartsheet-pydantic-1.0.1/tests/test_filters.py
--rw-r--r--   0 tak       (1000) tak       (1000)     2231 2023-04-22 16:01:26.000000 smartsheet-pydantic-1.0.1/tests/test_smartmodel.py
--rw-r--r--   0 tak       (1000) tak       (1000)      877 2023-04-22 16:06:21.000000 smartsheet-pydantic-1.0.1/tests/test_sources.py
+drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-22 21:38:20.593078 smartsheet-pydantic-1.1.0/
+-rw-r--r--   0 tak       (1000) tak       (1000)     1091 2023-04-22 15:28:56.000000 smartsheet-pydantic-1.1.0/LICENSE
+-rw-r--r--   0 tak       (1000) tak       (1000)       53 2023-04-22 15:28:20.000000 smartsheet-pydantic-1.1.0/MANIFEST.in
+-rw-r--r--   0 tak       (1000) tak       (1000)     1811 2023-04-22 21:38:20.593078 smartsheet-pydantic-1.1.0/PKG-INFO
+-rw-r--r--   0 tak       (1000) tak       (1000)      162 2023-04-22 14:53:39.000000 smartsheet-pydantic-1.1.0/README.md
+-rw-r--r--   0 tak       (1000) tak       (1000)      811 2023-04-22 21:38:07.000000 smartsheet-pydantic-1.1.0/pyproject.toml
+-rw-r--r--   0 tak       (1000) tak       (1000)       38 2023-04-22 21:38:20.593078 smartsheet-pydantic-1.1.0/setup.cfg
+drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-22 21:38:20.583078 smartsheet-pydantic-1.1.0/src/
+drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-22 21:38:20.583078 smartsheet-pydantic-1.1.0/src/smartsheet_pydantic/
+-rw-r--r--   0 tak       (1000) tak       (1000)        0 2023-04-22 14:53:46.000000 smartsheet-pydantic-1.1.0/src/smartsheet_pydantic/__init__.py
+-rw-r--r--   0 tak       (1000) tak       (1000)     6732 2023-04-22 16:41:51.000000 smartsheet-pydantic-1.1.0/src/smartsheet_pydantic/controller.py
+-rw-r--r--   0 tak       (1000) tak       (1000)      493 2023-04-22 14:53:20.000000 smartsheet-pydantic-1.1.0/src/smartsheet_pydantic/debug_logger.py
+-rw-r--r--   0 tak       (1000) tak       (1000)     2816 2023-04-22 15:44:48.000000 smartsheet-pydantic-1.1.0/src/smartsheet_pydantic/filters.py
+-rw-r--r--   0 tak       (1000) tak       (1000)    12396 2023-04-22 21:35:20.000000 smartsheet-pydantic-1.1.0/src/smartsheet_pydantic/smartmodels.py
+-rw-r--r--   0 tak       (1000) tak       (1000)     1145 2023-04-22 15:43:35.000000 smartsheet-pydantic-1.1.0/src/smartsheet_pydantic/sources.py
+-rw-r--r--   0 tak       (1000) tak       (1000)     2327 2023-04-22 15:45:13.000000 smartsheet-pydantic-1.1.0/src/smartsheet_pydantic/transformer.py
+drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-22 21:38:20.593078 smartsheet-pydantic-1.1.0/src/smartsheet_pydantic.egg-info/
+-rw-r--r--   0 tak       (1000) tak       (1000)     1811 2023-04-22 21:38:20.000000 smartsheet-pydantic-1.1.0/src/smartsheet_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 tak       (1000) tak       (1000)      634 2023-04-22 21:38:20.000000 smartsheet-pydantic-1.1.0/src/smartsheet_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 tak       (1000) tak       (1000)        1 2023-04-22 21:38:20.000000 smartsheet-pydantic-1.1.0/src/smartsheet_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 tak       (1000) tak       (1000)      102 2023-04-22 21:38:20.000000 smartsheet-pydantic-1.1.0/src/smartsheet_pydantic.egg-info/requires.txt
+-rw-r--r--   0 tak       (1000) tak       (1000)       20 2023-04-22 21:38:20.000000 smartsheet-pydantic-1.1.0/src/smartsheet_pydantic.egg-info/top_level.txt
+drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-22 21:38:20.593078 smartsheet-pydantic-1.1.0/tests/
+-rw-r--r--   0 tak       (1000) tak       (1000)     3924 2023-04-22 16:43:42.000000 smartsheet-pydantic-1.1.0/tests/test_controller.py
+-rw-r--r--   0 tak       (1000) tak       (1000)     3527 2023-04-22 16:01:06.000000 smartsheet-pydantic-1.1.0/tests/test_filters.py
+-rw-r--r--   0 tak       (1000) tak       (1000)    13872 2023-04-22 21:13:24.000000 smartsheet-pydantic-1.1.0/tests/test_smartmodel.py
+-rw-r--r--   0 tak       (1000) tak       (1000)      877 2023-04-22 16:06:21.000000 smartsheet-pydantic-1.1.0/tests/test_sources.py
```

### Comparing `smartsheet-pydantic-1.0.1/LICENSE` & `smartsheet-pydantic-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.0.1/PKG-INFO` & `smartsheet-pydantic-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsheet-pydantic
-Version: 1.0.1
+Version: 1.1.0
 Summary: Smartsheet Python SDK and Pydantic Wrapper
 Author: Takahiro Watanabe
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `smartsheet-pydantic-1.0.1/pyproject.toml` & `smartsheet-pydantic-1.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=67.7.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "smartsheet-pydantic"
-version = "1.0.1"
+version = "1.1.0"
 description = "Smartsheet Python SDK and Pydantic Wrapper"
 readme = "README.md"
 authors = [{ name = "Takahiro Watanabe" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `smartsheet-pydantic-1.0.1/src/smartsheet_pydantic/controller.py` & `smartsheet-pydantic-1.1.0/src/smartsheet_pydantic/controller.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.0.1/src/smartsheet_pydantic/filters.py` & `smartsheet-pydantic-1.1.0/src/smartsheet_pydantic/filters.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.0.1/src/smartsheet_pydantic/sources.py` & `smartsheet-pydantic-1.1.0/src/smartsheet_pydantic/sources.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.0.1/src/smartsheet_pydantic/transformer.py` & `smartsheet-pydantic-1.1.0/src/smartsheet_pydantic/transformer.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.0.1/src/smartsheet_pydantic.egg-info/PKG-INFO` & `smartsheet-pydantic-1.1.0/src/smartsheet_pydantic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsheet-pydantic
-Version: 1.0.1
+Version: 1.1.0
 Summary: Smartsheet Python SDK and Pydantic Wrapper
 Author: Takahiro Watanabe
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `smartsheet-pydantic-1.0.1/src/smartsheet_pydantic.egg-info/SOURCES.txt` & `smartsheet-pydantic-1.1.0/src/smartsheet_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.0.1/tests/test_controller.py` & `smartsheet-pydantic-1.1.0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.0.1/tests/test_filters.py` & `smartsheet-pydantic-1.1.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.0.1/tests/test_sources.py` & `smartsheet-pydantic-1.1.0/tests/test_sources.py`

 * *Files identical despite different names*

