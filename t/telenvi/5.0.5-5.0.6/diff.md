# Comparing `tmp/telenvi-5.0.5.tar.gz` & `tmp/telenvi-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telenvi-5.0.5.tar", last modified: Sat Apr 22 12:36:45 2023, max compression
+gzip compressed data, was "telenvi-5.0.6.tar", last modified: Sat Apr 22 13:32:44 2023, max compression
```

## Comparing `telenvi-5.0.5.tar` & `telenvi-5.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:36:45.480000 telenvi-5.0.5/
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    35823 2023-04-22 12:36:40.000000 telenvi-5.0.5/LICENSE
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-22 12:36:45.480000 telenvi-5.0.5/PKG-INFO
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      620 2023-04-22 12:36:40.000000 telenvi-5.0.5/README.md
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)       84 2023-04-22 12:36:40.000000 telenvi-5.0.5/pyproject.toml
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      673 2023-04-22 12:36:45.480000 telenvi-5.0.5/setup.cfg
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:36:45.470000 telenvi-5.0.5/src/
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:36:45.480000 telenvi-5.0.5/src/telenvi/
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    22386 2023-04-22 12:36:40.000000 telenvi-5.0.5/src/telenvi/GeoIm.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      133 2023-04-22 12:36:40.000000 telenvi-5.0.5/src/telenvi/__init__.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      478 2023-04-22 12:36:40.000000 telenvi-5.0.5/src/telenvi/associations.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    26495 2023-04-22 12:36:40.000000 telenvi-5.0.5/src/telenvi/raster_tools.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     2859 2023-04-22 12:36:40.000000 telenvi-5.0.5/src/telenvi/vector_tools.py
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:36:45.480000 telenvi-5.0.5/src/telenvi.egg-info/
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-22 12:36:45.000000 telenvi-5.0.5/src/telenvi.egg-info/PKG-INFO
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      311 2023-04-22 12:36:45.000000 telenvi-5.0.5/src/telenvi.egg-info/SOURCES.txt
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        1 2023-04-22 12:36:45.000000 telenvi-5.0.5/src/telenvi.egg-info/dependency_links.txt
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        8 2023-04-22 12:36:45.000000 telenvi-5.0.5/src/telenvi.egg-info/top_level.txt
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 13:32:44.720000 telenvi-5.0.6/
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    35823 2023-04-22 13:32:39.000000 telenvi-5.0.6/LICENSE
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-22 13:32:44.720000 telenvi-5.0.6/PKG-INFO
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      620 2023-04-22 13:32:39.000000 telenvi-5.0.6/README.md
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)       84 2023-04-22 13:32:39.000000 telenvi-5.0.6/pyproject.toml
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      673 2023-04-22 13:32:44.720000 telenvi-5.0.6/setup.cfg
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 13:32:44.720000 telenvi-5.0.6/src/
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 13:32:44.720000 telenvi-5.0.6/src/telenvi/
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    22386 2023-04-22 13:32:39.000000 telenvi-5.0.6/src/telenvi/GeoIm.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      133 2023-04-22 13:32:39.000000 telenvi-5.0.6/src/telenvi/__init__.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      478 2023-04-22 13:32:39.000000 telenvi-5.0.6/src/telenvi/associations.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    26495 2023-04-22 13:32:39.000000 telenvi-5.0.6/src/telenvi/raster_tools.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     2859 2023-04-22 13:32:39.000000 telenvi-5.0.6/src/telenvi/vector_tools.py
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 13:32:44.720000 telenvi-5.0.6/src/telenvi.egg-info/
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-22 13:32:44.000000 telenvi-5.0.6/src/telenvi.egg-info/PKG-INFO
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      311 2023-04-22 13:32:44.000000 telenvi-5.0.6/src/telenvi.egg-info/SOURCES.txt
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        1 2023-04-22 13:32:44.000000 telenvi-5.0.6/src/telenvi.egg-info/dependency_links.txt
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        8 2023-04-22 13:32:44.000000 telenvi-5.0.6/src/telenvi.egg-info/top_level.txt
```

### Comparing `telenvi-5.0.5/LICENSE` & `telenvi-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.5/PKG-INFO` & `telenvi-5.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telenvi
-Version: 5.0.5
+Version: 5.0.6
 Summary: Some remote sensing tricks from telenvi master students
 Home-page: https://github.com/pyzak117/telenvi
 Author: Thibaut Duvanel, Julien Pellen
 Author-email: thibaut.duvanel@univ-savoie.fr
 Project-URL: Bug Tracker, https://github.com/pyzak117/telenvi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `telenvi-5.0.5/README.md` & `telenvi-5.0.6/README.md`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.5/setup.cfg` & `telenvi-5.0.6/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = telenvi
-version = 5.0.5
+version = 5.0.6
 author = Thibaut Duvanel, Julien Pellen
 author_email = thibaut.duvanel@univ-savoie.fr
 description = Some remote sensing tricks from telenvi master students
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pyzak117/telenvi
 project_urls =
```

### Comparing `telenvi-5.0.5/src/telenvi/GeoIm.py` & `telenvi-5.0.6/src/telenvi/GeoIm.py`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.5/src/telenvi/raster_tools.py` & `telenvi-5.0.6/src/telenvi/raster_tools.py`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.5/src/telenvi/vector_tools.py` & `telenvi-5.0.6/src/telenvi/vector_tools.py`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.5/src/telenvi.egg-info/PKG-INFO` & `telenvi-5.0.6/src/telenvi.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telenvi
-Version: 5.0.5
+Version: 5.0.6
 Summary: Some remote sensing tricks from telenvi master students
 Home-page: https://github.com/pyzak117/telenvi
 Author: Thibaut Duvanel, Julien Pellen
 Author-email: thibaut.duvanel@univ-savoie.fr
 Project-URL: Bug Tracker, https://github.com/pyzak117/telenvi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

