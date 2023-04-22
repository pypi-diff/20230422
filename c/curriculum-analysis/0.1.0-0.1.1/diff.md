# Comparing `tmp/curriculum_analysis-0.1.0.tar.gz` & `tmp/curriculum_analysis-0.1.1.tar.gz`

## Comparing `curriculum_analysis-0.1.0.tar` & `curriculum_analysis-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.0/curriculum_analysis/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.0/curriculum_analysis/analysis.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.0/curriculum_analysis/config.cfg.default
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.0/curriculum_analysis/corpus.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.0/curriculum_analysis/csv_exporter.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.0/curriculum_analysis/json_exporter.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.0/curriculum_analysis/keywords.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.0/curriculum_analysis/main.py
--rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.0/curriculum_analysis/txt_parser.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.0/LICENCE
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.0/README.md
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/analysis.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/config.cfg.default
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/corpus.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/csv_exporter.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/json_exporter.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/keywords.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/main.py
+-rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/txt_parser.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/html/index.html
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/html/index.js
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/html/style.css
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/LICENCE
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/PKG-INFO
```

### Comparing `curriculum_analysis-0.1.0/curriculum_analysis/analysis.py` & `curriculum_analysis-0.1.1/curriculum_analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.1.0/curriculum_analysis/corpus.py` & `curriculum_analysis-0.1.1/curriculum_analysis/corpus.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.1.0/curriculum_analysis/csv_exporter.py` & `curriculum_analysis-0.1.1/curriculum_analysis/csv_exporter.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.1.0/curriculum_analysis/json_exporter.py` & `curriculum_analysis-0.1.1/curriculum_analysis/json_exporter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import json
+from pathlib import Path
+from distutils.dir_util import copy_tree
 
 from .analysis import Analysis
 
 class JSONExporter:
     def __init__(self, file, output_path):
         self.file = file
         self.output_path = output_path
@@ -19,8 +21,9 @@
             record = {
                 "code": obj.code,
                 "title": obj.full_title,
                 "data": analysis.results
             }
             result.append(record)
         with self.summary_path.open('w') as summary_file:
-            json.dump(result, summary_file)
+            json.dump(result, summary_file)
+        copy_tree(str(Path(__file__).parent / 'html'), str(self.output_path), update=True)
```

### Comparing `curriculum_analysis-0.1.0/curriculum_analysis/main.py` & `curriculum_analysis-0.1.1/curriculum_analysis/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,24 +28,27 @@
         exit()
 
     # load the config file
     config = ConfigParser()
     config.read(conf_path)
 
     # Load keywords
-    keyword_path = Path(config.get("curriculummAnalysis", "keywords_path")).expanduser()
+    keyword_path = Path(config.get("curriculumAnalysis", "keywords_path")).expanduser()
+    if not keyword_path.exists():
+        default = (Path(__file__).parent / 'keywords.txt').read_text()
+        keyword_path.write_text(default);
+        
     keywords = load_keywords_file(keyword_path)
 
-
     # load the data
     file = file_factory(Path(filename).expanduser())
 
     # Generate an analysis
-    outpath = Path(config.get("curriculummAnalysis", "outpath")).expanduser()
-    format = config.get("curriculummAnalysis", "format")
+    outpath = Path(config.get("curriculumAnalysis", "outpath")).expanduser()
+    format = config.get("curriculumAnalysis", "format")
     exporter = exporters[format](file, outpath)
 
     # Export it
     exporter.export(keywords)
 
 def cli():
     # The parser accepts a filename and an optional configuration file argument
```

### Comparing `curriculum_analysis-0.1.0/curriculum_analysis/txt_parser.py` & `curriculum_analysis-0.1.1/curriculum_analysis/txt_parser.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.1.0/LICENCE` & `curriculum_analysis-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.1.0/README.md` & `curriculum_analysis-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.1.0/pyproject.toml` & `curriculum_analysis-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 include = [
   "curriculum_analysis/config.cfg.default",
+  "curriculum_analysis/html/*",
   "**/*.py",  
 ]
 
 [project]
 name = "curriculum_analysis"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Graeme Stuart", email="gstuart@dmu.ac.uk" },
   { name="Tom Harrison" },
 ]
 description = "A simple tool for analysing DMU module and programme specifications with respect to provided keywords."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `curriculum_analysis-0.1.0/PKG-INFO` & `curriculum_analysis-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curriculum_analysis
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple tool for analysing DMU module and programme specifications with respect to provided keywords.
 Project-URL: Homepage, https://github.com/IESD/curriculumAnalysis
 Project-URL: Bug Tracker, https://github.com/IESD/curriculumAnalysis/issues
 Author: Tom Harrison
 Author-email: Graeme Stuart <gstuart@dmu.ac.uk>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
```

