# Comparing `tmp/telenvi-5.0.4.tar.gz` & `tmp/telenvi-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telenvi-5.0.4.tar", last modified: Sat Apr 22 12:30:56 2023, max compression
+gzip compressed data, was "telenvi-5.0.5.tar", last modified: Sat Apr 22 12:36:45 2023, max compression
```

## Comparing `telenvi-5.0.4.tar` & `telenvi-5.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:30:56.300000 telenvi-5.0.4/
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    35823 2023-04-22 12:30:51.000000 telenvi-5.0.4/LICENSE
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-22 12:30:56.300000 telenvi-5.0.4/PKG-INFO
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      620 2023-04-22 12:30:51.000000 telenvi-5.0.4/README.md
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)       84 2023-04-22 12:30:51.000000 telenvi-5.0.4/pyproject.toml
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      673 2023-04-22 12:30:56.300000 telenvi-5.0.4/setup.cfg
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:30:56.300000 telenvi-5.0.4/src/
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:30:56.300000 telenvi-5.0.4/src/telenvi/
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    22386 2023-04-22 12:30:51.000000 telenvi-5.0.4/src/telenvi/GeoIm.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      133 2023-04-22 12:30:51.000000 telenvi-5.0.4/src/telenvi/__init__.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      478 2023-04-22 12:30:51.000000 telenvi-5.0.4/src/telenvi/associations.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    26493 2023-04-22 12:30:51.000000 telenvi-5.0.4/src/telenvi/raster_tools.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     2859 2023-04-22 12:30:51.000000 telenvi-5.0.4/src/telenvi/vector_tools.py
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:30:56.300000 telenvi-5.0.4/src/telenvi.egg-info/
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-22 12:30:56.000000 telenvi-5.0.4/src/telenvi.egg-info/PKG-INFO
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      311 2023-04-22 12:30:56.000000 telenvi-5.0.4/src/telenvi.egg-info/SOURCES.txt
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        1 2023-04-22 12:30:56.000000 telenvi-5.0.4/src/telenvi.egg-info/dependency_links.txt
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        8 2023-04-22 12:30:56.000000 telenvi-5.0.4/src/telenvi.egg-info/top_level.txt
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:36:45.480000 telenvi-5.0.5/
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    35823 2023-04-22 12:36:40.000000 telenvi-5.0.5/LICENSE
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-22 12:36:45.480000 telenvi-5.0.5/PKG-INFO
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      620 2023-04-22 12:36:40.000000 telenvi-5.0.5/README.md
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)       84 2023-04-22 12:36:40.000000 telenvi-5.0.5/pyproject.toml
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      673 2023-04-22 12:36:45.480000 telenvi-5.0.5/setup.cfg
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:36:45.470000 telenvi-5.0.5/src/
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:36:45.480000 telenvi-5.0.5/src/telenvi/
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    22386 2023-04-22 12:36:40.000000 telenvi-5.0.5/src/telenvi/GeoIm.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      133 2023-04-22 12:36:40.000000 telenvi-5.0.5/src/telenvi/__init__.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      478 2023-04-22 12:36:40.000000 telenvi-5.0.5/src/telenvi/associations.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    26495 2023-04-22 12:36:40.000000 telenvi-5.0.5/src/telenvi/raster_tools.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     2859 2023-04-22 12:36:40.000000 telenvi-5.0.5/src/telenvi/vector_tools.py
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:36:45.480000 telenvi-5.0.5/src/telenvi.egg-info/
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-22 12:36:45.000000 telenvi-5.0.5/src/telenvi.egg-info/PKG-INFO
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      311 2023-04-22 12:36:45.000000 telenvi-5.0.5/src/telenvi.egg-info/SOURCES.txt
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        1 2023-04-22 12:36:45.000000 telenvi-5.0.5/src/telenvi.egg-info/dependency_links.txt
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        8 2023-04-22 12:36:45.000000 telenvi-5.0.5/src/telenvi.egg-info/top_level.txt
```

### Comparing `telenvi-5.0.4/LICENSE` & `telenvi-5.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.4/PKG-INFO` & `telenvi-5.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telenvi
-Version: 5.0.4
+Version: 5.0.5
 Summary: Some remote sensing tricks from telenvi master students
 Home-page: https://github.com/pyzak117/telenvi
 Author: Thibaut Duvanel, Julien Pellen
 Author-email: thibaut.duvanel@univ-savoie.fr
 Project-URL: Bug Tracker, https://github.com/pyzak117/telenvi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `telenvi-5.0.4/README.md` & `telenvi-5.0.5/README.md`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.4/setup.cfg` & `telenvi-5.0.5/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = telenvi
-version = 5.0.4
+version = 5.0.5
 author = Thibaut Duvanel, Julien Pellen
 author_email = thibaut.duvanel@univ-savoie.fr
 description = Some remote sensing tricks from telenvi master students
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pyzak117/telenvi
 project_urls =
```

### Comparing `telenvi-5.0.4/src/telenvi/GeoIm.py` & `telenvi-5.0.5/src/telenvi/GeoIm.py`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.4/src/telenvi/raster_tools.py` & `telenvi-5.0.5/src/telenvi/raster_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -727,19 +727,19 @@
         values = [target.array]
 
     # Build a 3D array with X and Y coordinates of each pixel + their values
     combo = np.array(values + [coords[1], coords[0]])
 
     # Reverse it. Now, combo[posX][poxY] return at least 3 values : b1, b2... bn, coordx, coordy
     combo = combo.T
-
+    
     # Build a list of DataFrames, one for each row because pd.DataFrame(array) must be used with 2D array
     protoVectorLayer = []
     for row in tqdm(range(nRows)):
-        rowDf = pd.DataFrame(combo[row], columns = [f"b{nBand}" for nBand in range(nBands)] + ['cy  ','cx'])
+        rowDf = pd.DataFrame(combo[row], columns = [f"b{nBand}" for nBand in range(nBands)] + ['cy','cx'])
 
         # Add geometry column with shapely
         with warnings.catch_warnings(): # Avoid inunderstandable shapely depreciation warning
             warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning)
             rowDf['geometry'] = rowDf.apply(lambda row: shapely.geometry.Point(row.cx, row.cy), axis=1)
 
         # Drop useless columns
```

### Comparing `telenvi-5.0.4/src/telenvi/vector_tools.py` & `telenvi-5.0.5/src/telenvi/vector_tools.py`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.4/src/telenvi.egg-info/PKG-INFO` & `telenvi-5.0.5/src/telenvi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telenvi
-Version: 5.0.4
+Version: 5.0.5
 Summary: Some remote sensing tricks from telenvi master students
 Home-page: https://github.com/pyzak117/telenvi
 Author: Thibaut Duvanel, Julien Pellen
 Author-email: thibaut.duvanel@univ-savoie.fr
 Project-URL: Bug Tracker, https://github.com/pyzak117/telenvi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

