# Comparing `tmp/metagentools-0.0.5.tar.gz` & `tmp/metagentools-0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metagentools-0.0.5.tar", last modified: Sat Apr 22 07:55:37 2023, max compression
+gzip compressed data, was "metagentools-0.0.dev2.tar", last modified: Fri Jan 27 14:02:02 2023, max compression
```

## Comparing `metagentools-0.0.5.tar` & `metagentools-0.0.dev2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-04-22 07:55:37.613190 metagentools-0.0.5/
--rw-rw-r--   0 vtec      (1000) vtec      (1000)    11337 2022-09-05 16:31:43.000000 metagentools-0.0.5/LICENSE
--rw-rw-r--   0 vtec      (1000) vtec      (1000)      111 2022-09-05 16:31:43.000000 metagentools-0.0.5/MANIFEST.in
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2269 2023-04-22 07:55:37.613190 metagentools-0.0.5/PKG-INFO
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1517 2023-04-22 07:49:55.000000 metagentools-0.0.5/README.md
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-04-22 07:55:37.613190 metagentools-0.0.5/legacy/
--rw-r--r--   0 vtec      (1000) vtec      (1000)        0 2022-10-07 01:34:07.000000 metagentools-0.0.5/legacy/__init__.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)      897 2022-10-07 01:34:07.000000 metagentools-0.0.5/legacy/analyze_final_report.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     5981 2022-10-07 01:34:07.000000 metagentools-0.0.5/legacy/analyze_using_bayes_autocpt.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1980 2022-10-29 06:12:30.000000 metagentools-0.0.5/legacy/architecture.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2491 2022-10-07 01:34:07.000000 metagentools-0.0.5/legacy/datasets.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2311 2022-10-07 01:34:07.000000 metagentools-0.0.5/legacy/evaluation_on_simulated_150mers.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1566 2022-10-07 01:34:07.000000 metagentools-0.0.5/legacy/evaluation_on_simulated_50mers.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1654 2022-10-07 01:34:07.000000 metagentools-0.0.5/legacy/evaluation_on_simulated_HIV.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)      805 2022-10-07 01:34:07.000000 metagentools-0.0.5/legacy/generate_report.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1565 2022-10-07 01:34:07.000000 metagentools-0.0.5/legacy/predict_100mers.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)      858 2022-10-07 01:34:07.000000 metagentools-0.0.5/legacy/predict_50mers.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1629 2022-10-07 01:34:07.000000 metagentools-0.0.5/legacy/predict_on_realdata.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     8642 2022-10-07 01:34:07.000000 metagentools-0.0.5/legacy/preprocessing.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1999 2022-10-07 01:34:07.000000 metagentools-0.0.5/legacy/training_model.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     6489 2022-10-07 01:34:07.000000 metagentools-0.0.5/legacy/utils.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)      851 2022-10-07 01:34:07.000000 metagentools-0.0.5/legacy/voting.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)    12176 2022-10-29 06:12:30.000000 metagentools-0.0.5/legacy/wandb.py
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-04-22 07:55:37.613190 metagentools-0.0.5/metagentools/
--rw-r--r--   0 vtec      (1000) vtec      (1000)       22 2023-04-22 07:46:09.000000 metagentools-0.0.5/metagentools/__init__.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)    16014 2023-04-22 07:49:55.000000 metagentools-0.0.5/metagentools/_modidx.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     7767 2023-04-22 07:49:55.000000 metagentools-0.0.5/metagentools/art.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     3372 2023-04-22 07:46:09.000000 metagentools-0.0.5/metagentools/bio.py
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-04-22 07:55:37.613190 metagentools-0.0.5/metagentools/cnn_virus/
--rw-r--r--   0 vtec      (1000) vtec      (1000)        0 2023-04-22 07:46:09.000000 metagentools-0.0.5/metagentools/cnn_virus/__init__.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2284 2023-04-22 07:46:09.000000 metagentools-0.0.5/metagentools/cnn_virus/architecture.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)    19458 2023-04-22 07:49:55.000000 metagentools-0.0.5/metagentools/cnn_virus/data.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1712 2023-04-22 07:46:09.000000 metagentools-0.0.5/metagentools/cnn_virus/utils.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)    10023 2023-04-22 07:49:55.000000 metagentools-0.0.5/metagentools/core.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)    10884 2023-04-22 07:46:09.000000 metagentools-0.0.5/metagentools/wandb.py
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-04-22 07:55:37.613190 metagentools-0.0.5/metagentools.egg-info/
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2269 2023-04-22 07:55:37.000000 metagentools-0.0.5/metagentools.egg-info/PKG-INFO
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1029 2023-04-22 07:55:37.000000 metagentools-0.0.5/metagentools.egg-info/SOURCES.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2023-04-22 07:55:37.000000 metagentools-0.0.5/metagentools.egg-info/dependency_links.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)       46 2023-04-22 07:55:37.000000 metagentools-0.0.5/metagentools.egg-info/entry_points.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2022-10-29 12:01:44.000000 metagentools-0.0.5/metagentools.egg-info/not-zip-safe
--rw-r--r--   0 vtec      (1000) vtec      (1000)       64 2023-04-22 07:55:37.000000 metagentools-0.0.5/metagentools.egg-info/requires.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)       20 2023-04-22 07:55:37.000000 metagentools-0.0.5/metagentools.egg-info/top_level.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)      927 2023-02-04 14:46:19.000000 metagentools-0.0.5/settings.ini
--rw-r--r--   0 vtec      (1000) vtec      (1000)       38 2023-04-22 07:55:37.613190 metagentools-0.0.5/setup.cfg
--rw-rw-r--   0 vtec      (1000) vtec      (1000)     2541 2022-09-05 16:31:43.000000 metagentools-0.0.5/setup.py
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-01-27 14:02:02.607491 metagentools-0.0.dev2/
+-rw-rw-r--   0 vtec      (1000) vtec      (1000)    11337 2022-09-05 16:31:43.000000 metagentools-0.0.dev2/LICENSE
+-rw-rw-r--   0 vtec      (1000) vtec      (1000)      111 2022-09-05 16:31:43.000000 metagentools-0.0.dev2/MANIFEST.in
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1391 2023-01-27 14:02:02.607491 metagentools-0.0.dev2/PKG-INFO
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      735 2023-01-17 09:05:10.000000 metagentools-0.0.dev2/README.md
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-01-27 14:02:02.607491 metagentools-0.0.dev2/legacy/
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        0 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/__init__.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      897 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/analyze_final_report.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     5981 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/analyze_using_bayes_autocpt.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1980 2022-10-29 06:12:30.000000 metagentools-0.0.dev2/legacy/architecture.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     2491 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/datasets.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     2311 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/evaluation_on_simulated_150mers.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1566 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/evaluation_on_simulated_50mers.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1654 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/evaluation_on_simulated_HIV.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      805 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/generate_report.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1565 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/predict_100mers.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      858 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/predict_50mers.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1629 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/predict_on_realdata.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     8642 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/preprocessing.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1999 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/training_model.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     6489 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/utils.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      851 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/voting.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)    12176 2022-10-29 06:12:30.000000 metagentools-0.0.dev2/legacy/wandb.py
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-01-27 14:02:02.607491 metagentools-0.0.dev2/metagentools/
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        0 2023-01-27 13:05:49.000000 metagentools-0.0.dev2/metagentools/__init__.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     5845 2023-01-27 13:32:29.000000 metagentools-0.0.dev2/metagentools/_modidx.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     7429 2023-01-27 13:05:49.000000 metagentools-0.0.dev2/metagentools/art.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     2750 2023-01-27 13:07:20.000000 metagentools-0.0.dev2/metagentools/bio.py
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-01-27 14:02:02.607491 metagentools-0.0.dev2/metagentools/cnn_virus/
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        0 2023-01-27 13:05:49.000000 metagentools-0.0.dev2/metagentools/cnn_virus/__init__.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     2284 2023-01-27 13:05:49.000000 metagentools-0.0.dev2/metagentools/cnn_virus/architecture.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     2802 2023-01-27 13:05:49.000000 metagentools-0.0.dev2/metagentools/cnn_virus/data.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1712 2023-01-27 13:05:49.000000 metagentools-0.0.dev2/metagentools/cnn_virus/utils.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      201 2023-01-27 13:07:20.000000 metagentools-0.0.dev2/metagentools/core.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)    10884 2023-01-27 13:05:49.000000 metagentools-0.0.dev2/metagentools/wandb.py
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-01-27 14:02:02.607491 metagentools-0.0.dev2/metagentools.egg-info/
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1391 2023-01-27 14:02:02.000000 metagentools-0.0.dev2/metagentools.egg-info/PKG-INFO
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1029 2023-01-27 14:02:02.000000 metagentools-0.0.dev2/metagentools.egg-info/SOURCES.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2023-01-27 14:02:02.000000 metagentools-0.0.dev2/metagentools.egg-info/dependency_links.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       46 2023-01-27 14:02:02.000000 metagentools-0.0.dev2/metagentools.egg-info/entry_points.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2022-10-29 12:01:44.000000 metagentools-0.0.dev2/metagentools.egg-info/not-zip-safe
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       64 2023-01-27 14:02:02.000000 metagentools-0.0.dev2/metagentools.egg-info/requires.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       20 2023-01-27 14:02:02.000000 metagentools-0.0.dev2/metagentools.egg-info/top_level.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1005 2023-01-27 14:01:46.000000 metagentools-0.0.dev2/settings.ini
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       38 2023-01-27 14:02:02.607491 metagentools-0.0.dev2/setup.cfg
+-rw-rw-r--   0 vtec      (1000) vtec      (1000)     2541 2022-09-05 16:31:43.000000 metagentools-0.0.dev2/setup.py
```

### Comparing `metagentools-0.0.5/LICENSE` & `metagentools-0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/analyze_final_report.py` & `metagentools-0.0.dev2/legacy/analyze_final_report.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/analyze_using_bayes_autocpt.py` & `metagentools-0.0.dev2/legacy/analyze_using_bayes_autocpt.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/architecture.py` & `metagentools-0.0.dev2/legacy/architecture.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/datasets.py` & `metagentools-0.0.dev2/legacy/datasets.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/evaluation_on_simulated_150mers.py` & `metagentools-0.0.dev2/legacy/evaluation_on_simulated_150mers.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/evaluation_on_simulated_50mers.py` & `metagentools-0.0.dev2/legacy/evaluation_on_simulated_50mers.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/evaluation_on_simulated_HIV.py` & `metagentools-0.0.dev2/legacy/evaluation_on_simulated_HIV.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/generate_report.py` & `metagentools-0.0.dev2/legacy/generate_report.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/predict_100mers.py` & `metagentools-0.0.dev2/legacy/predict_100mers.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/predict_50mers.py` & `metagentools-0.0.dev2/legacy/predict_50mers.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/predict_on_realdata.py` & `metagentools-0.0.dev2/legacy/predict_on_realdata.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/preprocessing.py` & `metagentools-0.0.dev2/legacy/preprocessing.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/training_model.py` & `metagentools-0.0.dev2/legacy/training_model.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/utils.py` & `metagentools-0.0.dev2/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/voting.py` & `metagentools-0.0.dev2/legacy/voting.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/legacy/wandb.py` & `metagentools-0.0.dev2/legacy/wandb.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/metagentools/art.py` & `metagentools-0.0.dev2/metagentools/art.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,19 @@
 from fastcore.utils import run, join_path_file
 from pathlib import Path
 from typing import Tuple, List, Optional
 
 # %% ../nbs-dev/02_art.ipynb 6
 # Private Utility functions to export ==============================================
 
-def _run(args:List[str], shell:bool=False, print_output=True):
+def _run(args: List[str], shell: bool=False):
     """Wrapper subprocess.run and prints the output"""
     p = subprocess.run(args=args, stdout=subprocess.PIPE, shell=shell)
-    if print_output:
-        print('return code: ',p.returncode, '\n')
-        print(str(p.stdout, 'utf-8'))
+    print('return code: ',p.returncode, '\n')
+    print(str(p.stdout, 'utf-8'))
 
 def _validate_path(p:str|Path) -> Path:
     """checks that path is a string or a Path, and returns a Path"""
     if isinstance(p, str): 
         p = Path(p)
     elif not isinstance(p, Path): 
         raise TypeError(f"a path must be a string or a Path, not a {type(p)}")
@@ -42,27 +41,24 @@
         'HS25': 'HiSeq 2500 (125bp, 150bp)', 'HSXn': 'HiSeqX PCR free (150bp)', 'HSXt': 'HiSeqX TruSeq (150bp)',
         'MinS': 'MiniSeq TruSeq (50bp)', 'MSv1': 'MiSeq v1 (250bp)', 'MSv3': 'MiSeq v3 (250bp)',
         'NS50': 'NextSeq500 v2 (75bp)'
         }
 
     def __init__(
         self, 
-        path2app: str|Path,            # full path to art_illumina application on the system
-        input_dir: str|Path,           # full path to dir where input files are
-        output_dir: str|Path=None,     # full path to dir where to save output files, if different from input_dir
-        app_in_system_path:bool=False, # whether `art_illumina` is in the system path or not
+        path2app: str|Path,           # path to the art_illumina application on the system
+        input_dir: str|Path,          # path to dir where input files are
+        output_dir: str|Path=None     # path to dir where to save output files, if different from input_dir
         ):
         """Initialize the art_illumina instance"""
 
         # Validate and save paths
-        path2app = _validate_path(path2app)
-        if app_in_system_path:
-            self.app_cmd = 'art_illumina'
-        elif path2app.is_file():
-            self.app_cmd = str(path2app.absolute())
+        path2app = _validate_path(path2app)        
+        if path2app.is_file():
+            self.app = path2app
         else:
             raise ValueError(f"{path2app.name} is not a file, please check the path to the application")
 
         input_dir = _validate_path(input_dir)
         if input_dir.is_dir():
             self.input_dir = input_dir
         else:
@@ -73,41 +69,39 @@
         else:
             output_dir = _validate_path(output_dir)
             if output_dir.is_dir():
                 self.output_dir = output_dir
             else:
                 raise ValueError(f"{input_dir.name} is not a directory, please check the path")
 
-        print(f"Ready to operate with art: {self.app_cmd}")
+        print(f"Ready to operate with art: {self.app.absolute()}")
         print(f"Input files from : {self.input_dir.absolute()}")
         print(f"Output files to :  {self.output_dir.absolute()}")
 
     def sim_reads(
         self,
         input_file: str,          # name of the fasta file to use as input
         output_seed: str,         # seed to use for the output files
         sim_type: str='single',   # type of read simmulation: 'single' or 'paired'
         read_length: int=150,     # length of the read in bp
         fold: int=10,             # fold
         mean_read: int=None,      # mean length of the read for paired reads
         std_read: int=None,       # std of the read length, for paired reads
         ss: str='HS25',           # quality profile to use for simulation,
-        overwrite: bool=False,    # overwrite existing output files if true, raise error if false 
-        print_output:bool=True    # if True, prints art ilumina's CLI output
+        overwrite: bool=False     # overwrite existing output files if true, raise error if false 
         ):
         """Simulates reads with art_illumina. Output files saved in a separate directory"""
 
         # validate input file and save in instance
         path2inputfile = self.input_dir / input_file
         if path2inputfile.is_file(): 
             self.last_input_file = path2inputfile
         else:
             raise ValueError(f"{input_file} is not a file in {self.input_dir}")
 
-        
         # validate output seed and save in instance
         if not overwrite and len(list(self.output_dir.glob(f"{output_seed}*"))) > 0: 
             raise ValueError(f"Existing output directory starting with {output_seed}")
         else:
             self.last_output_seed = output_seed
             self.last_read_output_dir = self.output_dir/self.last_output_seed
             os.makedirs(self.last_read_output_dir, exist_ok=True)
@@ -126,16 +120,17 @@
                 params = f"-ss {ss} -p -l {read_length} -f {fold} -m {mean_read} -s {std_read}"
         else:
             raise RuntimeError(f"{sim_type} in not a type or is not implemented yet")
 
         p2in = self.last_input_file.absolute()
         p2out = (self.output_dir / self.last_output_seed / self.last_output_seed).absolute()
 
-        cmd = f"{self.app_cmd} -i {p2in} {params} -o {p2out}"
-        _run(args=shlex.split(cmd), print_output=print_output)
+        cmd = f"{self.app.absolute()} -i {p2in} {params} -o {p2out}"
+
+        _run(args=shlex.split(cmd))
 
     def get_last_output_files(self):
         """Returns the path to all output files from last simulation"""
         return [f for f in self.last_read_output_dir.iterdir()]
 
     def list_last_output_files(self):
         """Prints a list of the last simulation's output files"""
```

### Comparing `metagentools-0.0.5/metagentools/cnn_virus/architecture.py` & `metagentools-0.0.dev2/metagentools/cnn_virus/architecture.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/metagentools/cnn_virus/utils.py` & `metagentools-0.0.dev2/metagentools/cnn_virus/utils.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/metagentools/wandb.py` & `metagentools-0.0.dev2/metagentools/wandb.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/metagentools.egg-info/SOURCES.txt` & `metagentools-0.0.dev2/metagentools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.5/setup.py` & `metagentools-0.0.dev2/setup.py`

 * *Files identical despite different names*

