# Comparing `tmp/docbuild-0.1.102.tar.gz` & `tmp/docbuild-0.1.103.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docbuild-0.1.102.tar", last modified: Sat Apr 22 16:47:32 2023, max compression
+gzip compressed data, was "docbuild-0.1.103.tar", last modified: Sat Apr 22 17:26:39 2023, max compression
```

## Comparing `docbuild-0.1.102.tar` & `docbuild-0.1.103.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-22 16:47:32.063263 docbuild-0.1.102/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-22 16:47:32.063109 docbuild-0.1.102/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.102/README.md
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-22 16:47:32.059982 docbuild-0.1.102/docbuild/
--rw-r--r--   0 moran      (501) staff       (20)       63 2023-04-22 16:47:10.000000 docbuild-0.1.102/docbuild/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      439 2023-04-20 11:04:19.000000 docbuild-0.1.102/docbuild/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.102/docbuild/graph.py
--rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.102/docbuild/hocr_parser.py
--rw-r--r--   0 moran      (501) staff       (20)     7030 2023-04-22 09:34:19.000000 docbuild-0.1.102/docbuild/page_creator.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-22 16:47:32.061845 docbuild-0.1.102/docbuild/paragraph_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.102/docbuild/paragraph_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.102/docbuild/paragraph_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-20 11:03:50.000000 docbuild-0.1.102/docbuild/paragraph_detection/paragraph_extractor.py
--rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.102/docbuild/paragraph_detection/paragraph_sorter.py
--rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.102/docbuild/paragraph_detection/two_columns.py
--rw-r--r--   0 moran      (501) staff       (20)     4293 2023-04-22 13:58:04.000000 docbuild-0.1.102/docbuild/textract_parser.py
--rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.102/docbuild/utils.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-22 16:47:32.062766 docbuild-0.1.102/docbuild/visual_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.102/docbuild/visual_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)    12466 2023-04-19 14:32:23.000000 docbuild-0.1.102/docbuild/visual_detection/bordered_table_extraction.py
--rw-r--r--   0 moran      (501) staff       (20)      193 2023-04-22 15:58:54.000000 docbuild-0.1.102/docbuild/visual_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)    16321 2023-04-22 16:45:50.000000 docbuild-0.1.102/docbuild/visual_detection/vis_line_detection.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-22 16:47:32.060914 docbuild-0.1.102/docbuild.egg-info/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-22 16:47:32.000000 docbuild-0.1.102/docbuild.egg-info/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)      741 2023-04-22 16:47:32.000000 docbuild-0.1.102/docbuild.egg-info/SOURCES.txt
--rw-r--r--   0 moran      (501) staff       (20)        1 2023-04-22 16:47:32.000000 docbuild-0.1.102/docbuild.egg-info/dependency_links.txt
--rw-r--r--   0 moran      (501) staff       (20)       83 2023-04-22 16:47:32.000000 docbuild-0.1.102/docbuild.egg-info/requires.txt
--rw-r--r--   0 moran      (501) staff       (20)        9 2023-04-22 16:47:32.000000 docbuild-0.1.102/docbuild.egg-info/top_level.txt
--rw-r--r--   0 moran      (501) staff       (20)       38 2023-04-22 16:47:32.063299 docbuild-0.1.102/setup.cfg
--rw-r--r--   0 moran      (501) staff       (20)      832 2023-04-22 16:47:13.000000 docbuild-0.1.102/setup.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-22 17:26:39.981466 docbuild-0.1.103/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-22 17:26:39.981288 docbuild-0.1.103/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.103/README.md
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-22 17:26:39.976140 docbuild-0.1.103/docbuild/
+-rw-r--r--   0 moran      (501) staff       (20)       63 2023-04-22 17:26:35.000000 docbuild-0.1.103/docbuild/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      439 2023-04-20 11:04:19.000000 docbuild-0.1.103/docbuild/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.103/docbuild/graph.py
+-rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.103/docbuild/hocr_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)     7042 2023-04-22 17:26:00.000000 docbuild-0.1.103/docbuild/page_creator.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-22 17:26:39.979514 docbuild-0.1.103/docbuild/paragraph_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.103/docbuild/paragraph_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.103/docbuild/paragraph_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-20 11:03:50.000000 docbuild-0.1.103/docbuild/paragraph_detection/paragraph_extractor.py
+-rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.103/docbuild/paragraph_detection/paragraph_sorter.py
+-rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.103/docbuild/paragraph_detection/two_columns.py
+-rw-r--r--   0 moran      (501) staff       (20)     4293 2023-04-22 13:58:04.000000 docbuild-0.1.103/docbuild/textract_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.103/docbuild/utils.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-22 17:26:39.980857 docbuild-0.1.103/docbuild/visual_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.103/docbuild/visual_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)    12466 2023-04-19 14:32:23.000000 docbuild-0.1.103/docbuild/visual_detection/bordered_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)      193 2023-04-22 15:58:54.000000 docbuild-0.1.103/docbuild/visual_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)    16317 2023-04-22 17:26:25.000000 docbuild-0.1.103/docbuild/visual_detection/vis_line_detection.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-22 17:26:39.978106 docbuild-0.1.103/docbuild.egg-info/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-22 17:26:39.000000 docbuild-0.1.103/docbuild.egg-info/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)      741 2023-04-22 17:26:39.000000 docbuild-0.1.103/docbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 moran      (501) staff       (20)        1 2023-04-22 17:26:39.000000 docbuild-0.1.103/docbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 moran      (501) staff       (20)       83 2023-04-22 17:26:39.000000 docbuild-0.1.103/docbuild.egg-info/requires.txt
+-rw-r--r--   0 moran      (501) staff       (20)        9 2023-04-22 17:26:39.000000 docbuild-0.1.103/docbuild.egg-info/top_level.txt
+-rw-r--r--   0 moran      (501) staff       (20)       38 2023-04-22 17:26:39.981555 docbuild-0.1.103/setup.cfg
+-rw-r--r--   0 moran      (501) staff       (20)      832 2023-04-22 17:26:29.000000 docbuild-0.1.103/setup.py
```

### Comparing `docbuild-0.1.102/PKG-INFO` & `docbuild-0.1.103/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.102
+Version: 0.1.103
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.102/docbuild/graph.py` & `docbuild-0.1.103/docbuild/graph.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.102/docbuild/hocr_parser.py` & `docbuild-0.1.103/docbuild/hocr_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.102/docbuild/page_creator.py` & `docbuild-0.1.103/docbuild/page_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             hor_threshold = avg_word_size_hor
             vis_line_detector = VisLineDetector(
                 image_path=self.image_path, words=words
             )
             hor_lines, ver_lines = vis_line_detector.detect_lines(
                 hor_threshold, ver_threshold, image_length_threshold
             )
-
+            
             table_detector = BorderedTableExtractor(
                 words,
                 hor_lines,
                 ver_lines,
                 hor_threshold,
                 ver_threshold,
             )
```

### Comparing `docbuild-0.1.102/docbuild/paragraph_detection/paragraph_extractor.py` & `docbuild-0.1.103/docbuild/paragraph_detection/paragraph_extractor.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.102/docbuild/paragraph_detection/paragraph_sorter.py` & `docbuild-0.1.103/docbuild/paragraph_detection/paragraph_sorter.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.102/docbuild/paragraph_detection/two_columns.py` & `docbuild-0.1.103/docbuild/paragraph_detection/two_columns.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.102/docbuild/textract_parser.py` & `docbuild-0.1.103/docbuild/textract_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.102/docbuild/utils.py` & `docbuild-0.1.103/docbuild/utils.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.102/docbuild/visual_detection/bordered_table_extraction.py` & `docbuild-0.1.103/docbuild/visual_detection/bordered_table_extraction.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.102/docbuild/visual_detection/vis_line_detection.py` & `docbuild-0.1.103/docbuild/visual_detection/vis_line_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         )
 
     def get_lines(self, orientation: VisLineOrientation) -> list[VisLine]:
         filter_func = VisLineOpenCV.is_hor_line if orientation == VisLineOrientation.HORIZONTAL\
          else VisLineOpenCV.is_ver_line
         openCV_lines = self.get_openCV_lines()
         if openCV_lines is None:
-            return [], []
+            return []
         openCV_filtered_lines = [line for line in openCV_lines if filter_func(line)]
         vis_lines = [
             self.convert_to_vis_line(line, orientation=orientation)
             for line in openCV_filtered_lines
         ]
         return vis_lines
```

### Comparing `docbuild-0.1.102/docbuild.egg-info/PKG-INFO` & `docbuild-0.1.103/docbuild.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.102
+Version: 0.1.103
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.102/docbuild.egg-info/SOURCES.txt` & `docbuild-0.1.103/docbuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.102/setup.py` & `docbuild-0.1.103/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name="docbuild",
-    version="0.1.102",
+    version="0.1.103",
     description="A package for building a document from a textract response, for more information see the docstruct package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Moran Nechushtan, Serah Tapia, Shlomo Agishtein",
     author_email="moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com",
     url="https://github.com/smrt-co/docbuild",
     packages=setuptools.find_packages(),
```

