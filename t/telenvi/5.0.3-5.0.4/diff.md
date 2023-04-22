# Comparing `tmp/telenvi-5.0.3.tar.gz` & `tmp/telenvi-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telenvi-5.0.3.tar", last modified: Mon Apr 17 10:40:07 2023, max compression
+gzip compressed data, was "telenvi-5.0.4.tar", last modified: Sat Apr 22 12:30:56 2023, max compression
```

## Comparing `telenvi-5.0.3.tar` & `telenvi-5.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-17 10:40:07.640000 telenvi-5.0.3/
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    35823 2023-04-17 10:40:01.000000 telenvi-5.0.3/LICENSE
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-17 10:40:07.640000 telenvi-5.0.3/PKG-INFO
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      620 2023-04-17 10:40:01.000000 telenvi-5.0.3/README.md
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)       84 2023-04-17 10:40:01.000000 telenvi-5.0.3/pyproject.toml
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      673 2023-04-17 10:40:07.640000 telenvi-5.0.3/setup.cfg
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-17 10:40:07.640000 telenvi-5.0.3/src/
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-17 10:40:07.640000 telenvi-5.0.3/src/telenvi/
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    22386 2023-04-17 10:40:01.000000 telenvi-5.0.3/src/telenvi/GeoIm.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      133 2023-04-17 10:40:01.000000 telenvi-5.0.3/src/telenvi/__init__.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      478 2023-04-17 10:40:01.000000 telenvi-5.0.3/src/telenvi/associations.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    24416 2023-04-17 10:40:01.000000 telenvi-5.0.3/src/telenvi/raster_tools.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     2859 2023-04-17 10:40:01.000000 telenvi-5.0.3/src/telenvi/vector_tools.py
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-17 10:40:07.640000 telenvi-5.0.3/src/telenvi.egg-info/
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-17 10:40:07.000000 telenvi-5.0.3/src/telenvi.egg-info/PKG-INFO
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      311 2023-04-17 10:40:07.000000 telenvi-5.0.3/src/telenvi.egg-info/SOURCES.txt
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        1 2023-04-17 10:40:07.000000 telenvi-5.0.3/src/telenvi.egg-info/dependency_links.txt
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        8 2023-04-17 10:40:07.000000 telenvi-5.0.3/src/telenvi.egg-info/top_level.txt
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:30:56.300000 telenvi-5.0.4/
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    35823 2023-04-22 12:30:51.000000 telenvi-5.0.4/LICENSE
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-22 12:30:56.300000 telenvi-5.0.4/PKG-INFO
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      620 2023-04-22 12:30:51.000000 telenvi-5.0.4/README.md
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)       84 2023-04-22 12:30:51.000000 telenvi-5.0.4/pyproject.toml
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      673 2023-04-22 12:30:56.300000 telenvi-5.0.4/setup.cfg
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:30:56.300000 telenvi-5.0.4/src/
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:30:56.300000 telenvi-5.0.4/src/telenvi/
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    22386 2023-04-22 12:30:51.000000 telenvi-5.0.4/src/telenvi/GeoIm.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      133 2023-04-22 12:30:51.000000 telenvi-5.0.4/src/telenvi/__init__.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      478 2023-04-22 12:30:51.000000 telenvi-5.0.4/src/telenvi/associations.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    26493 2023-04-22 12:30:51.000000 telenvi-5.0.4/src/telenvi/raster_tools.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     2859 2023-04-22 12:30:51.000000 telenvi-5.0.4/src/telenvi/vector_tools.py
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-22 12:30:56.300000 telenvi-5.0.4/src/telenvi.egg-info/
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-22 12:30:56.000000 telenvi-5.0.4/src/telenvi.egg-info/PKG-INFO
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      311 2023-04-22 12:30:56.000000 telenvi-5.0.4/src/telenvi.egg-info/SOURCES.txt
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        1 2023-04-22 12:30:56.000000 telenvi-5.0.4/src/telenvi.egg-info/dependency_links.txt
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        8 2023-04-22 12:30:56.000000 telenvi-5.0.4/src/telenvi.egg-info/top_level.txt
```

### Comparing `telenvi-5.0.3/LICENSE` & `telenvi-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.3/PKG-INFO` & `telenvi-5.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telenvi
-Version: 5.0.3
+Version: 5.0.4
 Summary: Some remote sensing tricks from telenvi master students
 Home-page: https://github.com/pyzak117/telenvi
 Author: Thibaut Duvanel, Julien Pellen
 Author-email: thibaut.duvanel@univ-savoie.fr
 Project-URL: Bug Tracker, https://github.com/pyzak117/telenvi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `telenvi-5.0.3/README.md` & `telenvi-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.3/setup.cfg` & `telenvi-5.0.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = telenvi
-version = 5.0.3
+version = 5.0.4
 author = Thibaut Duvanel, Julien Pellen
 author_email = thibaut.duvanel@univ-savoie.fr
 description = Some remote sensing tricks from telenvi master students
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pyzak117/telenvi
 project_urls =
```

### Comparing `telenvi-5.0.3/src/telenvi/GeoIm.py` & `telenvi-5.0.4/src/telenvi/GeoIm.py`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.3/src/telenvi/raster_tools.py` & `telenvi-5.0.4/src/telenvi/raster_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,22 +9,26 @@
 from telenvi.associations import npdtype_gdalconst, extensions_drivers
 import telenvi.GeoIm as GeoIm
 
 # Standard libraries
 import os
 import json
 import pathlib
+import warnings
 
-# import argparse
+# CLI libraries
+from tqdm import tqdm
 
 # Data libraries
 import numpy as np
+import pandas as pd
 
 # Geo libraries
 import shapely
+from shapely.errors import ShapelyDeprecationWarning
 
 # import richdem as rd
 import geopandas as gpd
 from osgeo import gdal, gdalconst, osr, ogr
 
 """
 # --------------
@@ -690,14 +694,68 @@
     if gdal.Open(outpath) != None:
         print(f"{os.path.basename(outpath)} OK")
         return True
     else:
         print(f"error during {os.path.basename(outpath)} creation")
         return False    
 
+def vectorize(target):
+    target = GeoIm.GeoIm(target)
+
+    # extract raster metadata
+    x_origin, y_origin = getOrigin(target)
+    x_pixel_size, y_pixel_size = getPixelSize(target)
+    nBands, nCols, nRows = getShape(target)
+
+    # Create coordinate arrays
+    x_coords = np.arange(
+        start= x_origin, 
+        stop = x_origin + x_pixel_size * nRows,
+        step = x_pixel_size)
+
+    y_coords = np.arange(
+        start= y_origin, 
+        stop = y_origin + y_pixel_size * nCols,
+        step = y_pixel_size)
+
+    # A 3 dimensionals arrays. We use it like coords[:, posY, posX]
+    coords = np.array(np.meshgrid(x_coords, y_coords))
+
+    # Make a list with each 2D arrays of the images - if multispectral
+    if nBands > 1:
+        values = [target.array[band] for band in range(0,nBands)]
+    else:
+        values = [target.array]
+
+    # Build a 3D array with X and Y coordinates of each pixel + their values
+    combo = np.array(values + [coords[1], coords[0]])
+
+    # Reverse it. Now, combo[posX][poxY] return at least 3 values : b1, b2... bn, coordx, coordy
+    combo = combo.T
+
+    # Build a list of DataFrames, one for each row because pd.DataFrame(array) must be used with 2D array
+    protoVectorLayer = []
+    for row in tqdm(range(nRows)):
+        rowDf = pd.DataFrame(combo[row], columns = [f"b{nBand}" for nBand in range(nBands)] + ['cy  ','cx'])
+
+        # Add geometry column with shapely
+        with warnings.catch_warnings(): # Avoid inunderstandable shapely depreciation warning
+            warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning)
+            rowDf['geometry'] = rowDf.apply(lambda row: shapely.geometry.Point(row.cx, row.cy), axis=1)
+
+        # Drop useless columns
+        rowDf = rowDf.drop(['cx', 'cy'], axis=1)
+
+        protoVectorLayer.append(rowDf)
+
+    # Concat all the row DataFrames into one
+    vectorLayer = gpd.GeoDataFrame(pd.concat(protoVectorLayer, ignore_index=True))
+
+    return vectorLayer
+
 def cropFromIndexes(target, indexes):
 
     # Unpack indexes
     firstCol, firstRow, lastCol, lastRow = indexes
 
     # Get target metadata
     target = getDs(target)
```

### Comparing `telenvi-5.0.3/src/telenvi/vector_tools.py` & `telenvi-5.0.4/src/telenvi/vector_tools.py`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.3/src/telenvi.egg-info/PKG-INFO` & `telenvi-5.0.4/src/telenvi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telenvi
-Version: 5.0.3
+Version: 5.0.4
 Summary: Some remote sensing tricks from telenvi master students
 Home-page: https://github.com/pyzak117/telenvi
 Author: Thibaut Duvanel, Julien Pellen
 Author-email: thibaut.duvanel@univ-savoie.fr
 Project-URL: Bug Tracker, https://github.com/pyzak117/telenvi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

