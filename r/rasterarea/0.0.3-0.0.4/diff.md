# Comparing `tmp/rasterarea-0.0.3.tar.gz` & `tmp/rasterarea-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasterarea-0.0.3.tar", last modified: Sat Apr 15 03:47:27 2023, max compression
+gzip compressed data, was "rasterarea-0.0.4.tar", last modified: Sat Apr 22 03:44:13 2023, max compression
```

## Comparing `rasterarea-0.0.3.tar` & `rasterarea-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:47:27.216307 rasterarea-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-15 03:47:18.000000 rasterarea-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-15 03:47:18.000000 rasterarea-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-15 03:47:27.216307 rasterarea-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 03:47:18.000000 rasterarea-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:47:27.216307 rasterarea-0.0.3/rasterarea/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-15 03:47:18.000000 rasterarea-0.0.3/rasterarea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-15 03:47:18.000000 rasterarea-0.0.3/rasterarea/foliummap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-15 03:47:18.000000 rasterarea-0.0.3/rasterarea/ipyleafletmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-15 03:47:18.000000 rasterarea-0.0.3/rasterarea/rasterarea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:47:27.216307 rasterarea-0.0.3/rasterarea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-15 03:47:27.000000 rasterarea-0.0.3/rasterarea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-15 03:47:27.000000 rasterarea-0.0.3/rasterarea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-15 03:47:27.000000 rasterarea-0.0.3/rasterarea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 03:47:27.000000 rasterarea-0.0.3/rasterarea.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-15 03:47:27.000000 rasterarea-0.0.3/rasterarea.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 03:47:27.000000 rasterarea-0.0.3/rasterarea.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-15 03:47:18.000000 rasterarea-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-15 03:47:27.216307 rasterarea-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-15 03:47:18.000000 rasterarea-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:44:13.895546 rasterarea-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-22 03:43:57.000000 rasterarea-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-22 03:43:57.000000 rasterarea-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-22 03:44:13.895546 rasterarea-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-22 03:43:57.000000 rasterarea-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:44:13.895546 rasterarea-0.0.4/rasterarea/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-22 03:43:57.000000 rasterarea-0.0.4/rasterarea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-22 03:43:57.000000 rasterarea-0.0.4/rasterarea/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-04-22 03:43:57.000000 rasterarea-0.0.4/rasterarea/ipyleafletmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-04-22 03:43:57.000000 rasterarea-0.0.4/rasterarea/rasterarea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:44:13.895546 rasterarea-0.0.4/rasterarea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-22 03:44:13.000000 rasterarea-0.0.4/rasterarea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-22 03:44:13.000000 rasterarea-0.0.4/rasterarea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-22 03:44:13.000000 rasterarea-0.0.4/rasterarea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 03:44:13.000000 rasterarea-0.0.4/rasterarea.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-22 03:44:13.000000 rasterarea-0.0.4/rasterarea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 03:44:13.000000 rasterarea-0.0.4/rasterarea.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-22 03:43:57.000000 rasterarea-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-22 03:44:13.895546 rasterarea-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-22 03:43:57.000000 rasterarea-0.0.4/setup.py
```

### Comparing `rasterarea-0.0.3/LICENSE` & `rasterarea-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rasterarea-0.0.3/PKG-INFO` & `rasterarea-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasterarea
-Version: 0.0.3
+Version: 0.0.4
 Summary: This package provides a more accurate way to claculate the area of rasters.
 Home-page: https://github.com/Feng96/rasterarea
 Author: Yinan Feng
 Author-email: 1041267458@qq.com
 License: MIT license
 Keywords: rasterarea
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rasterarea-0.0.3/README.md` & `rasterarea-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rasterarea-0.0.3/rasterarea/foliummap.py` & `rasterarea-0.0.4/rasterarea/foliummap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import folium
-
 class Map(folium.Map):
-    """Create a folium map object.
+    """ Create a folium map object.
 
     Args:
-        folium (_type_): _description_
-    """    
-    def __init__(self, center=[20, 0], zoom=2, **kwargs) -> None:
-        """Initializes the map object.
+        folium: Creates a map in Folium 
+    """
+    def __init__(self, center=[20,0], zoom=2, **kwargs) -> None:
+        """
 
         Args:
-            center (list, optional): The map center. Defaults to [20, 0].
-            zoom (int, optional): The zoom level. Defaults to 2.
+            center (list, optional): The Map Center. Defaults to [20,0].
+            zoom (int, optional): Sets the zoom level of the map. Defaults to 2.
         """
         super().__init__(location=center, zoom_start=zoom, **kwargs)
 
-
     def add_tile_layer(self, url, name, attribution = "", **kwargs):
         """Adds a tile layer to the map.
 
         Args:
             url (str): The URL of the tile layer.
             name (str): The name of the tile layer
             attribution (str, optional): The attribution of the tile layer. Defaults to **
@@ -28,15 +26,15 @@
             tiles= url,
             name = name,
             attr = attribution,
             **kwargs
         )
         self.add_child(tile_layer)
 
-     def add_basemap(self, basemap, **kwargs):
+    def add_basemap(self, basemap, **kwargs):   
         """Adds a basemap to the map
 
         Args:
             basemap: The basemap to add
 
         Raises:
             ValueError: Incorrect Basemap
```

### Comparing `rasterarea-0.0.3/rasterarea/ipyleafletmap.py` & `rasterarea-0.0.4/rasterarea/ipyleafletmap.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import ipyleaflet
-
+from ipyleaflet import WidgetControl
+import ipywidgets as widgets
 class Map(ipyleaflet.Map):
     
     def __init__(self, center=[20, 0], zoom=2, **kwargs) -> None:
 
         if "scroll_wheel_zoom" not in kwargs:
             kwargs["scroll_wheel_zoom"] = True
 
@@ -197,7 +198,20 @@
         tile = r["tiles"][0]
 
         self.add_tile_layer(url=tile, name=name, **kwargs)
 
         if fit_bounds:
             bbox = [[bounds[1], bounds[0]], [bounds[3], bounds[2]]]
             self.fit_bounds(bbox)
+
+    def add_image(self, url, width, height, position = 'bottomright',**kwargs):
+        """Add an image to the map.
+
+        Args:
+            url (str): The URL of the image.
+            width (int): The width of the image.
+            height (int): The height of the image.
+            position (str, optional): The position of the image. Defaults to 'bottomright'.
+        """
+        widget = widgets.HTML(value = f'<img src="{url}" width="{width}" height="{height}">')
+        control = WidgetControl(widget=widget, position=position)
+        self.add(control)
```

### Comparing `rasterarea-0.0.3/rasterarea/rasterarea.py` & `rasterarea-0.0.4/rasterarea/rasterarea.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Main module."""
 
 import math
+import pandas as pd
 
 def area_of_pixel(center_lat,pixel_size=1, coordinatesp = 'WGS84', **kwargs):
     """_summary_
 
     Args:
         center_lat (_type_): _description_
         pixel_size (int, optional): _description_. Defaults to 1.
@@ -189,15 +190,15 @@
     import rasterio
 
     with rasterio.open(geotiff_path) as src:
         shape = src.shape
 
     return shape
 
-def point_cloud_arrary(filepath, no_data=0, band=1, **kwargs):
+def point_cloud_arrary(filepath, no_data=-99999, band=1, **kwargs):
     """_summary_
 
     Args:
         filepath (_type_): _description_
         no_data (int, optional): _description_. Defaults to 0.
         band (int, optional): _description_. Defaults to 1.
 
@@ -205,15 +206,15 @@
         _type_: _description_
     """
     import lidario as lio
     translator = lio.Translator("geotiff", "np")
     point_cloud = translator.translate(input_values=filepath, no_data=no_data, band=band)
     return point_cloud
     
-def pixel_area_array(point_cloud_arrary, pixel_size=1, coordinatesp = 'WGS84', **kwargs):
+def pixel_area_array(point_cloud_arrary, pixel_size=1, coordinatesp = 'WGS84', toTable = False, **kwargs):
     """_summary_
 
     Args:
         filepath (_type_): _description_
         no_data (int, optional): _description_. Defaults to 0.
         band (int, optional): _description_. Defaults to 1.
 
@@ -268,8 +269,15 @@
         zp_a = 1 + c*math.sin(math.radians(center_lat+pixel_size/2))
         area_a = math.pi * b**2 * (math.log(zp_a/zm_a) / (2*c) + math.sin(math.radians(center_lat+pixel_size/2)) / (zp_a*zm_a))
         zm_b = 1 - c*math.sin(math.radians(center_lat-pixel_size/2))
         zp_b = 1 + c*math.sin(math.radians(center_lat-pixel_size/2))
         area_b = math.pi * b**2 * (math.log(zp_b/zm_b) / (2*c) + math.sin(math.radians(center_lat-pixel_size/2)) / (zp_b*zm_b))
         area = (1 / 360 * (area_a - area_b))
         raster_area[i][2] = area
-    return raster_area
+    
+    if toTable == True:
+        raster_area = pd.DataFrame(raster_area)
+        raster_area.rename(columns={0:'center_lon',1:'center_lat',2:'pixel_area'},inplace=True)
+    else:
+        pass
+    
+    return raster_area
```

### Comparing `rasterarea-0.0.3/rasterarea.egg-info/PKG-INFO` & `rasterarea-0.0.4/rasterarea.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasterarea
-Version: 0.0.3
+Version: 0.0.4
 Summary: This package provides a more accurate way to claculate the area of rasters.
 Home-page: https://github.com/Feng96/rasterarea
 Author: Yinan Feng
 Author-email: 1041267458@qq.com
 License: MIT license
 Keywords: rasterarea
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rasterarea-0.0.3/setup.py` & `rasterarea-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='rasterarea',
     name='rasterarea',
     packages=find_packages(include=['rasterarea', 'rasterarea.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Feng96/rasterarea',
-    version='0.0.3',
+    version='0.0.4',
     zip_safe=False,
 )
```

