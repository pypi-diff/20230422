# Comparing `tmp/docbuild-0.1.101.tar.gz` & `tmp/docbuild-0.1.102.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docbuild-0.1.101.tar", last modified: Thu Apr 20 11:06:47 2023, max compression
+gzip compressed data, was "docbuild-0.1.102.tar", last modified: Sat Apr 22 16:47:32 2023, max compression
```

## Comparing `docbuild-0.1.101.tar` & `docbuild-0.1.102.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-20 11:06:47.017799 docbuild-0.1.101/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-20 11:06:47.017466 docbuild-0.1.101/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.101/README.md
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-20 11:06:47.011799 docbuild-0.1.101/docbuild/
--rw-r--r--   0 moran      (501) staff       (20)       63 2023-04-20 11:06:41.000000 docbuild-0.1.101/docbuild/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      439 2023-04-20 11:04:19.000000 docbuild-0.1.101/docbuild/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.101/docbuild/graph.py
--rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.101/docbuild/hocr_parser.py
--rw-r--r--   0 moran      (501) staff       (20)     7030 2023-04-20 11:06:00.000000 docbuild-0.1.101/docbuild/page_creator.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-20 11:06:47.014684 docbuild-0.1.101/docbuild/paragraph_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.101/docbuild/paragraph_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.101/docbuild/paragraph_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-20 11:03:50.000000 docbuild-0.1.101/docbuild/paragraph_detection/paragraph_extractor.py
--rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.101/docbuild/paragraph_detection/paragraph_sorter.py
--rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.101/docbuild/paragraph_detection/two_columns.py
--rw-r--r--   0 moran      (501) staff       (20)     4293 2023-04-19 06:25:19.000000 docbuild-0.1.101/docbuild/textract_parser.py
--rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.101/docbuild/utils.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-20 11:06:47.016699 docbuild-0.1.101/docbuild/visual_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.101/docbuild/visual_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)    12466 2023-04-19 14:32:23.000000 docbuild-0.1.101/docbuild/visual_detection/bordered_table_extraction.py
--rw-r--r--   0 moran      (501) staff       (20)      158 2023-04-19 09:10:38.000000 docbuild-0.1.101/docbuild/visual_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)    16376 2023-04-19 09:12:11.000000 docbuild-0.1.101/docbuild/visual_detection/vis_line_detection.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-20 11:06:47.013171 docbuild-0.1.101/docbuild.egg-info/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-20 11:06:46.000000 docbuild-0.1.101/docbuild.egg-info/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)      741 2023-04-20 11:06:46.000000 docbuild-0.1.101/docbuild.egg-info/SOURCES.txt
--rw-r--r--   0 moran      (501) staff       (20)        1 2023-04-20 11:06:46.000000 docbuild-0.1.101/docbuild.egg-info/dependency_links.txt
--rw-r--r--   0 moran      (501) staff       (20)       83 2023-04-20 11:06:46.000000 docbuild-0.1.101/docbuild.egg-info/requires.txt
--rw-r--r--   0 moran      (501) staff       (20)        9 2023-04-20 11:06:46.000000 docbuild-0.1.101/docbuild.egg-info/top_level.txt
--rw-r--r--   0 moran      (501) staff       (20)       38 2023-04-20 11:06:47.017860 docbuild-0.1.101/setup.cfg
--rw-r--r--   0 moran      (501) staff       (20)      832 2023-04-20 11:06:30.000000 docbuild-0.1.101/setup.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-22 16:47:32.063263 docbuild-0.1.102/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-22 16:47:32.063109 docbuild-0.1.102/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.102/README.md
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-22 16:47:32.059982 docbuild-0.1.102/docbuild/
+-rw-r--r--   0 moran      (501) staff       (20)       63 2023-04-22 16:47:10.000000 docbuild-0.1.102/docbuild/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      439 2023-04-20 11:04:19.000000 docbuild-0.1.102/docbuild/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.102/docbuild/graph.py
+-rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.102/docbuild/hocr_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)     7030 2023-04-22 09:34:19.000000 docbuild-0.1.102/docbuild/page_creator.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-22 16:47:32.061845 docbuild-0.1.102/docbuild/paragraph_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.102/docbuild/paragraph_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.102/docbuild/paragraph_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-20 11:03:50.000000 docbuild-0.1.102/docbuild/paragraph_detection/paragraph_extractor.py
+-rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.102/docbuild/paragraph_detection/paragraph_sorter.py
+-rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.102/docbuild/paragraph_detection/two_columns.py
+-rw-r--r--   0 moran      (501) staff       (20)     4293 2023-04-22 13:58:04.000000 docbuild-0.1.102/docbuild/textract_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.102/docbuild/utils.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-22 16:47:32.062766 docbuild-0.1.102/docbuild/visual_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.102/docbuild/visual_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)    12466 2023-04-19 14:32:23.000000 docbuild-0.1.102/docbuild/visual_detection/bordered_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)      193 2023-04-22 15:58:54.000000 docbuild-0.1.102/docbuild/visual_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)    16321 2023-04-22 16:45:50.000000 docbuild-0.1.102/docbuild/visual_detection/vis_line_detection.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-22 16:47:32.060914 docbuild-0.1.102/docbuild.egg-info/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-22 16:47:32.000000 docbuild-0.1.102/docbuild.egg-info/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)      741 2023-04-22 16:47:32.000000 docbuild-0.1.102/docbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 moran      (501) staff       (20)        1 2023-04-22 16:47:32.000000 docbuild-0.1.102/docbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 moran      (501) staff       (20)       83 2023-04-22 16:47:32.000000 docbuild-0.1.102/docbuild.egg-info/requires.txt
+-rw-r--r--   0 moran      (501) staff       (20)        9 2023-04-22 16:47:32.000000 docbuild-0.1.102/docbuild.egg-info/top_level.txt
+-rw-r--r--   0 moran      (501) staff       (20)       38 2023-04-22 16:47:32.063299 docbuild-0.1.102/setup.cfg
+-rw-r--r--   0 moran      (501) staff       (20)      832 2023-04-22 16:47:13.000000 docbuild-0.1.102/setup.py
```

### Comparing `docbuild-0.1.101/PKG-INFO` & `docbuild-0.1.102/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.101
+Version: 0.1.102
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.101/docbuild/graph.py` & `docbuild-0.1.102/docbuild/graph.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.101/docbuild/hocr_parser.py` & `docbuild-0.1.102/docbuild/hocr_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.101/docbuild/page_creator.py` & `docbuild-0.1.102/docbuild/page_creator.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.101/docbuild/paragraph_detection/paragraph_extractor.py` & `docbuild-0.1.102/docbuild/paragraph_detection/paragraph_extractor.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.101/docbuild/paragraph_detection/paragraph_sorter.py` & `docbuild-0.1.102/docbuild/paragraph_detection/paragraph_sorter.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.101/docbuild/paragraph_detection/two_columns.py` & `docbuild-0.1.102/docbuild/paragraph_detection/two_columns.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.101/docbuild/textract_parser.py` & `docbuild-0.1.102/docbuild/textract_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.101/docbuild/utils.py` & `docbuild-0.1.102/docbuild/utils.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.101/docbuild/visual_detection/bordered_table_extraction.py` & `docbuild-0.1.102/docbuild/visual_detection/bordered_table_extraction.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.101/docbuild/visual_detection/vis_line_detection.py` & `docbuild-0.1.102/docbuild/visual_detection/vis_line_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from ..graph import Node, Graph
 from docstruct import Word, Drawer, SpatialGrid
 from .constants import (
     ANGLE_DEGREE_THRESHOLD,
     NUM_SAMPLED_POINTS_ON_LINE,
     NUM_SAMPLED_POINTS_ON_ORTHOGONAL_LINE,
     SPATIAL_GRID_SIZE,
+    KERNEL_HEIGHT,
+    KERNEL_WIDTH,
 )
 
 
 @attr.s(auto_attribs=True)
 class HorVerVisLines:
     hor_lines: list[VisLine]
     ver_lines: list[VisLine]
@@ -82,14 +84,17 @@
         x0 = x0 / self.image_width
         x1 = x1 / self.image_width
         y0 = 1 - y0 / self.image_height
         y1 = 1 - y1 / self.image_height
         return x0, y0, x1, y1
 
     def get_line_width(self, line: dict, orientation: VisLineOrientation):
+        return 10
+
+    def get_line_width_not_in_use(self, line: dict, orientation: VisLineOrientation):
         x0, y0, x1, y1 = line
         points = sample_points_on_line(x0, y0, x1, y1, NUM_SAMPLED_POINTS_ON_LINE)
         widths = []
         for point in points:
             # TODO think of a max_length
             max_length = 15
             orthogonal_line = get_line(
@@ -128,33 +133,26 @@
             axis=axis,
             orientation=orientation,
             start=start,
             end=end,
             width=normalized_line_width,
         )
 
-    def get_lines(self):
+    def get_lines(self, orientation: VisLineOrientation) -> list[VisLine]:
+        filter_func = VisLineOpenCV.is_hor_line if orientation == VisLineOrientation.HORIZONTAL\
+         else VisLineOpenCV.is_ver_line
         openCV_lines = self.get_openCV_lines()
         if openCV_lines is None:
             return [], []
-        openCV_hor_lines = [
-            line for line in openCV_lines if VisLineOpenCV.is_hor_line(line)
-        ]
-        openCV_ver_lines = [
-            line for line in openCV_lines if VisLineOpenCV.is_ver_line(line)
-        ]
-        vis_hor_lines = [
-            self.convert_to_vis_line(line, orientation=VisLineOrientation.HORIZONTAL)
-            for line in openCV_hor_lines
-        ]
-        vis_ver_lines = [
-            self.convert_to_vis_line(line, orientation=VisLineOrientation.VERTICAL)
-            for line in openCV_ver_lines
+        openCV_filtered_lines = [line for line in openCV_lines if filter_func(line)]
+        vis_lines = [
+            self.convert_to_vis_line(line, orientation=orientation)
+            for line in openCV_filtered_lines
         ]
-        return vis_hor_lines, vis_ver_lines
+        return vis_lines
 
 
 class VisLineRemover:
     def __init__(self, lines: list[VisLine], words: list[Word]):
         self.lines = lines
         self.words = words
         self.spatial_grid = self.get_spatial_grid(lines, words)
@@ -391,43 +389,41 @@
         debug_dir: str = None,
     ):
         self.image = cv2.imread(image_path)
         self.image_height, self.image_width = self.image.shape[:2]
         self.words = words
         self.debug = debug
         self.debug_dir = debug_dir
+        self.hor_kernel = np.ones((KERNEL_WIDTH, KERNEL_HEIGHT), np.uint8) / (KERNEL_WIDTH  * KERNEL_HEIGHT)
+        self.ver_kernel = np.ones((KERNEL_HEIGHT, KERNEL_WIDTH), np.uint8) / (KERNEL_WIDTH  * KERNEL_HEIGHT)
+        
         if debug:
             self.opencv_drawer = Drawer(image_path)
             self.remover_drawer = Drawer(image_path)
             self.merge_drawer = Drawer(image_path)
             self.extension_drawer = Drawer(image_path)
 
     def detect_lines(
         self, hor_threshold: int, ver_threshold: int, image_length_threshold: int
     ) -> HorVerVisLines:
-        hor_image = self.hor_preprocess(self.image)
-        ver_image = self.ver_preprocess(self.image)
-
-        gray_hor_image = cv2.cvtColor(hor_image, cv2.COLOR_BGR2GRAY)
-        gray_ver_image = cv2.cvtColor(ver_image, cv2.COLOR_BGR2GRAY)
-
+        gray_image = cv2.cvtColor(self.image, cv2.COLOR_BGR2GRAY)
+        gray_hor_image = self.hor_preprocess(gray_image)
+        gray_ver_image = self.ver_preprocess(gray_image)
+        
         hor_line_detector = VisLineOpenCV(gray_hor_image, image_length_threshold)
-
-        hor_lines, _ = hor_line_detector.get_lines()
+        hor_lines = hor_line_detector.get_lines(VisLineOrientation.HORIZONTAL)
         ver_line_detector = VisLineOpenCV(gray_ver_image, image_length_threshold)
-        _, ver_lines = ver_line_detector.get_lines()
+        ver_lines = ver_line_detector.get_lines(VisLineOrientation.VERTICAL)
 
         if self.debug:
             self.opencv_drawer.draw_vis_lines(hor_lines + ver_lines, random_color=True)
             self.opencv_drawer.save(os.path.join(self.debug_dir, "opencv_lines.jpg"))
 
         line_remover = VisLineRemover(lines=hor_lines + ver_lines, words=self.words)
 
-        # self.remover_drawer.draw_spatial_grid(line_remover.spatial_grid, VisLine)
-        # self.remover_drawer.show()
         hor_lines, ver_lines = line_remover.remove_lines()
         if self.debug:
             self.remover_drawer.draw_vis_lines(hor_lines + ver_lines, random_color=True)
             self.remover_drawer.save(os.path.join(self.folder, "remover_lines.jpg"))
 
         hor_line_merger = VisLineMerger(hor_lines, hor_threshold)
         merged_hor_lines = hor_line_merger.merge_lines()
@@ -444,19 +440,15 @@
         line_extension.extend_lines()
         line_extension = VisLineExtension(merged_ver_lines, ver_threshold)
 
         hor_ver_vis_lines = HorVerVisLines(merged_hor_lines, merged_ver_lines)
         return hor_ver_vis_lines
 
     def hor_preprocess(self, image: np.ndarray) -> np.ndarray:
-        """Horizontal blur"""
-        kernel = np.ones((3, 7), np.float32) / 21
-        image = cv2.filter2D(image, -1, kernel)
+        image = cv2.filter2D(image, -1, self.hor_kernel)
         return image
 
     def ver_preprocess(self, image: np.ndarray) -> np.ndarray:
-        """Vertical blur"""
-        kernel = np.ones((7, 3), np.float32) / 21
-        image = cv2.filter2D(image, -1, kernel)
+        image = cv2.filter2D(image, -1, self.ver_kernel)
         return image
```

### Comparing `docbuild-0.1.101/docbuild.egg-info/PKG-INFO` & `docbuild-0.1.102/docbuild.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.101
+Version: 0.1.102
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.101/docbuild.egg-info/SOURCES.txt` & `docbuild-0.1.102/docbuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.101/setup.py` & `docbuild-0.1.102/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name="docbuild",
-    version="0.1.101",
+    version="0.1.102",
     description="A package for building a document from a textract response, for more information see the docstruct package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Moran Nechushtan, Serah Tapia, Shlomo Agishtein",
     author_email="moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com",
     url="https://github.com/smrt-co/docbuild",
     packages=setuptools.find_packages(),
```

