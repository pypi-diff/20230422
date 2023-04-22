# Comparing `tmp/kiutils-1.4.0.tar.gz` & `tmp/kiutils-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiutils-1.4.0.tar", last modified: Mon Mar 27 20:21:27 2023, max compression
+gzip compressed data, was "kiutils-1.4.1.tar", last modified: Sat Apr 22 16:16:26 2023, max compression
```

## Comparing `kiutils-1.4.0.tar` & `kiutils-1.4.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:21:27.615521 kiutils-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-27 20:21:04.000000 kiutils-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-03-27 20:21:27.615521 kiutils-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-03-27 20:21:04.000000 kiutils-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-27 20:21:04.000000 kiutils-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-27 20:21:27.615521 kiutils-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-27 20:21:04.000000 kiutils-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:21:27.611521 kiutils-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:21:27.611521 kiutils-1.4.0/src/kiutils/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/board.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/dru.py
--rw-r--r--   0 runner    (1001) docker     (123)    46972 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/footprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:21:27.615521 kiutils-1.4.0/src/kiutils/items/
--rw-r--r--   0 runner    (1001) docker     (123)    47460 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/items/brditems.py
--rw-r--r--   0 runner    (1001) docker     (123)    42864 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/items/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/items/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/items/fpitems.py
--rw-r--r--   0 runner    (1001) docker     (123)    31527 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/items/gritems.py
--rw-r--r--   0 runner    (1001) docker     (123)    72965 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/items/schitems.py
--rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/items/syitems.py
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/items/zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/libraries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:21:27.615521 kiutils-1.4.0/src/kiutils/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/misc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/schematic.py
--rw-r--r--   0 runner    (1001) docker     (123)    25567 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/symbol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:21:27.615521 kiutils-1.4.0/src/kiutils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/utils/sexpr.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)    38203 2023-03-27 20:21:04.000000 kiutils-1.4.0/src/kiutils/wks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:21:27.611521 kiutils-1.4.0/src/kiutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-03-27 20:21:27.000000 kiutils-1.4.0/src/kiutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-27 20:21:27.000000 kiutils-1.4.0/src/kiutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:21:27.000000 kiutils-1.4.0/src/kiutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-27 20:21:27.000000 kiutils-1.4.0/src/kiutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:21:27.615521 kiutils-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-03-27 20:21:04.000000 kiutils-1.4.0/tests/test_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-03-27 20:21:04.000000 kiutils-1.4.0/tests/test_designrules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-03-27 20:21:04.000000 kiutils-1.4.0/tests/test_footprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-03-27 20:21:04.000000 kiutils-1.4.0/tests/test_libtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-03-27 20:21:04.000000 kiutils-1.4.0/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-03-27 20:21:04.000000 kiutils-1.4.0/tests/test_schematic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-03-27 20:21:04.000000 kiutils-1.4.0/tests/test_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-03-27 20:21:04.000000 kiutils-1.4.0/tests/test_worksheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-03-27 20:21:04.000000 kiutils-1.4.0/tests/testfunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.185885 kiutils-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-22 16:16:01.000000 kiutils-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-22 16:16:26.185885 kiutils-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-22 16:16:01.000000 kiutils-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-22 16:16:01.000000 kiutils-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-22 16:16:26.185885 kiutils-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-22 16:16:01.000000 kiutils-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.181885 kiutils-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.181885 kiutils-1.4.1/src/kiutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/dru.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46972 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/footprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.181885 kiutils-1.4.1/src/kiutils/items/
+-rw-r--r--   0 runner    (1001) docker     (123)    47460 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/brditems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42864 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/fpitems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31527 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/gritems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72965 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/schitems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/syitems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27998 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/libraries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.185885 kiutils-1.4.1/src/kiutils/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/misc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/schematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25567 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/symbol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.185885 kiutils-1.4.1/src/kiutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/utils/sexpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38203 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/wks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.181885 kiutils-1.4.1/src/kiutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-22 16:16:26.000000 kiutils-1.4.1/src/kiutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-22 16:16:26.000000 kiutils-1.4.1/src/kiutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 16:16:26.000000 kiutils-1.4.1/src/kiutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-22 16:16:26.000000 kiutils-1.4.1/src/kiutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.185885 kiutils-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_designrules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_libtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_schematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_worksheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/testfunctions.py
```

### Comparing `kiutils-1.4.0/LICENSE` & `kiutils-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/PKG-INFO` & `kiutils-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiutils
-Version: 1.4.0
+Version: 1.4.1
 Summary: Simple and SCM-friendly KiCad file parser for KiCad 6.0 and up
 Home-page: https://github.com/mvnmgrx/kiutils
 Author: Marvin Mager
 Author-email: 99667992+mvnmgrx@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/mvnmgrx/kiutils/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kiutils-1.4.0/README.md` & `kiutils-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/setup.cfg` & `kiutils-1.4.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kiutils
-version = 1.4.0
+version = 1.4.1
 author = Marvin Mager
 author_email = 99667992+mvnmgrx@users.noreply.github.com
 description = Simple and SCM-friendly KiCad file parser for KiCad 6.0 and up
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mvnmgrx/kiutils
 project_urls =
```

### Comparing `kiutils-1.4.0/src/kiutils/board.py` & `kiutils-1.4.1/src/kiutils/board.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils/dru.py` & `kiutils-1.4.1/src/kiutils/dru.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils/footprint.py` & `kiutils-1.4.1/src/kiutils/footprint.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils/items/brditems.py` & `kiutils-1.4.1/src/kiutils/items/brditems.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils/items/common.py` & `kiutils-1.4.1/src/kiutils/items/common.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils/items/dimensions.py` & `kiutils-1.4.1/src/kiutils/items/dimensions.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils/items/fpitems.py` & `kiutils-1.4.1/src/kiutils/items/fpitems.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils/items/gritems.py` & `kiutils-1.4.1/src/kiutils/items/gritems.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils/items/schitems.py` & `kiutils-1.4.1/src/kiutils/items/schitems.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils/items/syitems.py` & `kiutils-1.4.1/src/kiutils/items/syitems.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils/items/zones.py` & `kiutils-1.4.1/src/kiutils/items/zones.py`

 * *Files 1% similar despite different names*

```diff
@@ -622,21 +622,21 @@
         tstamp = f' (tstamp {self.tstamp})' if self.tstamp is not None else ''
         name = f' (name "{dequote(self.name)}")' if self.name is not None else ''
         contype = f' {self.connectPads}' if self.connectPads is not None else ''
         fat = f' (filled_areas_thickness {self.filledAreasThickness})' if self.filledAreasThickness is not None else ''
         layers, layer_token = '', ''
         for layer in self.layers:
             layers += f' "{dequote(layer)}"'
-
-        if len(self.layers) == 1:
+            
+        if len(self.layers) == 0:
+            raise Exception("Zone: No layers set for this zone")
+        elif len(self.layers) == 1 and self.layers[0] != "F&B.Cu":
             layer_token = f' (layer{layers})'
-        elif len(self.layers) > 1:
-            layer_token = f' (layers{layers})'
         else:
-            raise Exception("Zone: No layers set for this zone")
+            layer_token = f' (layers{layers})'
 
         expression =  f'{indents}(zone{locked} (net {self.net}) (net_name "{dequote(self.netName)}"){layer_token}{tstamp}{name} (hatch {self.hatch.style} {self.hatch.pitch})\n'
         if self.priority is not None:
             expression += f'{indents}  (priority {self.priority})\n'
         expression += f'{indents}  (connect_pads{contype} (clearance {self.clearance}))\n'
         expression += f'{indents}  (min_thickness {self.minThickness}){fat}\n'
         if self.keepoutSettings is not None:
```

### Comparing `kiutils-1.4.0/src/kiutils/libraries.py` & `kiutils-1.4.1/src/kiutils/libraries.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils/schematic.py` & `kiutils-1.4.1/src/kiutils/schematic.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils/symbol.py` & `kiutils-1.4.1/src/kiutils/symbol.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils/utils/sexpr.py` & `kiutils-1.4.1/src/kiutils/utils/sexpr.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils/utils/strings.py` & `kiutils-1.4.1/src/kiutils/utils/strings.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils/wks.py` & `kiutils-1.4.1/src/kiutils/wks.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/src/kiutils.egg-info/PKG-INFO` & `kiutils-1.4.1/src/kiutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiutils
-Version: 1.4.0
+Version: 1.4.1
 Summary: Simple and SCM-friendly KiCad file parser for KiCad 6.0 and up
 Home-page: https://github.com/mvnmgrx/kiutils
 Author: Marvin Mager
 Author-email: 99667992+mvnmgrx@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/mvnmgrx/kiutils/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kiutils-1.4.0/src/kiutils.egg-info/SOURCES.txt` & `kiutils-1.4.1/src/kiutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/tests/test_board.py` & `kiutils-1.4.1/tests/test_board.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/tests/test_designrules.py` & `kiutils-1.4.1/tests/test_designrules.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/tests/test_footprint.py` & `kiutils-1.4.1/tests/test_footprint.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/tests/test_libtable.py` & `kiutils-1.4.1/tests/test_libtable.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/tests/test_misc.py` & `kiutils-1.4.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/tests/test_schematic.py` & `kiutils-1.4.1/tests/test_schematic.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/tests/test_symbol.py` & `kiutils-1.4.1/tests/test_symbol.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/tests/test_worksheets.py` & `kiutils-1.4.1/tests/test_worksheets.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.0/tests/testfunctions.py` & `kiutils-1.4.1/tests/testfunctions.py`

 * *Files identical despite different names*

