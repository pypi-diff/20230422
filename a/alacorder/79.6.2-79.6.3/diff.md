# Comparing `tmp/alacorder-79.6.2.tar.gz` & `tmp/alacorder-79.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-79.6.2.tar", max compression
+gzip compressed data, was "alacorder-79.6.3.tar", max compression
```

## Comparing `alacorder-79.6.2.tar` & `alacorder-79.6.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.6.2/LICENSE
--rw-r--r--   0        0        0     9558 2023-04-19 15:07:38.263494 alacorder-79.6.2/README.md
--rw-r--r--   0        0        0      679 2023-04-22 13:52:51.007703 alacorder-79.6.2/pyproject.toml
--rw-r--r--   0        0        0     9208 2023-04-21 18:06:44.921207 alacorder-79.6.2/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb
--rw-r--r--   0        0        0   138382 2023-04-21 18:24:49.412475 alacorder-79.6.2/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.6.2/src/alacorder/.python-version
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.6.2/src/alacorder/__init__.py
--rw-r--r--   0        0        0   139605 2023-04-22 13:52:25.429230 alacorder-79.6.2/src/alacorder/__main__.py
--rw-r--r--   0        0        0   139605 2023-04-22 13:52:12.231450 alacorder-79.6.2/src/alacorder/alac.py
--rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.6.2/src/alacorder/~$E 302 Portfolio.docx
--rw-r--r--   0        0        0    10448 1970-01-01 00:00:00.000000 alacorder-79.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.6.3/LICENSE
+-rw-r--r--   0        0        0     9558 2023-04-19 15:07:38.263494 alacorder-79.6.3/README.md
+-rw-r--r--   0        0        0      679 2023-04-22 19:26:51.205036 alacorder-79.6.3/pyproject.toml
+-rw-r--r--   0        0        0     9208 2023-04-21 18:06:44.921207 alacorder-79.6.3/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb
+-rw-r--r--   0        0        0   138382 2023-04-21 18:24:49.412475 alacorder-79.6.3/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.6.3/src/alacorder/.python-version
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.6.3/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   139811 2023-04-22 19:27:01.673125 alacorder-79.6.3/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   139811 2023-04-22 19:27:06.885178 alacorder-79.6.3/src/alacorder/alac.py
+-rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.6.3/src/alacorder/~$E 302 Portfolio.docx
+-rw-r--r--   0        0        0    10448 1970-01-01 00:00:00.000000 alacorder-79.6.3/PKG-INFO
```

### Comparing `alacorder-79.6.2/LICENSE` & `alacorder-79.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.2/README.md` & `alacorder-79.6.3/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.2/pyproject.toml` & `alacorder-79.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "79.6.2"
+version = "79.6.3"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-79.6.2/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb` & `alacorder-79.6.3/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.2/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-79.6.3/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.2/src/alacorder/__init__.py` & `alacorder-79.6.3/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.2/src/alacorder/__main__.py` & `alacorder-79.6.3/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     tqdm, 
     xlsxwriter, 
     xlsx2csv
 
 """
 
 name = "ALACORDER"
-version = "79.6.2"
+version = "79.6.3"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 if autoload_graphical_user_interface:
     import PySimpleGUI as sg
 
@@ -2576,19 +2576,24 @@
             .then(True)
             .otherwise(False)
             .alias("PermanentDisqConviction"),
             pl.when(pl.col("PERM_DISQ_MATCH") & pl.col("Felony") & pl.col("A_S_C_DISQ"))
             .then(True)
             .otherwise(False)
             .alias("PermanentDisqCharge"),
+            pl.concat_str([
+                pl.col("CaseNumber"),
+                pl.lit("-"),
+                pl.col("Num")
+                ]).alias("CASENONUM")
         ]
     )
-    aggch = charges.groupby("CaseNumber").agg("RAWCITE","RAWDESC")
+    aggch = charges.groupby("CASENONUM").agg("CaseNumber","RAWCITE","RAWDESC")
     aggch = aggch.select([
-        pl.col("CaseNumber"),
+        pl.col("CaseNumber").arr.get(0).alias("CaseNumber"),
         pl.col("RAWDESC").arr.get(0).alias("Description"),
         pl.col("RAWCITE").arr.get(0).alias("Cite")
         ])
     charges = charges.join(aggch, on="CaseNumber")
     charges = charges.select(
         "CaseNumber",
         "Num",
```

### Comparing `alacorder-79.6.2/src/alacorder/alac.py` & `alacorder-79.6.3/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     tqdm, 
     xlsxwriter, 
     xlsx2csv
 
 """
 
 name = "ALACORDER"
-version = "79.6.2"
+version = "79.6.3"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 if autoload_graphical_user_interface:
     import PySimpleGUI as sg
 
@@ -2576,19 +2576,24 @@
             .then(True)
             .otherwise(False)
             .alias("PermanentDisqConviction"),
             pl.when(pl.col("PERM_DISQ_MATCH") & pl.col("Felony") & pl.col("A_S_C_DISQ"))
             .then(True)
             .otherwise(False)
             .alias("PermanentDisqCharge"),
+            pl.concat_str([
+                pl.col("CaseNumber"),
+                pl.lit("-"),
+                pl.col("Num")
+                ]).alias("CASENONUM")
         ]
     )
-    aggch = charges.groupby("CaseNumber").agg("RAWCITE","RAWDESC")
+    aggch = charges.groupby("CASENONUM").agg("CaseNumber","RAWCITE","RAWDESC")
     aggch = aggch.select([
-        pl.col("CaseNumber"),
+        pl.col("CaseNumber").arr.get(0).alias("CaseNumber"),
         pl.col("RAWDESC").arr.get(0).alias("Description"),
         pl.col("RAWCITE").arr.get(0).alias("Cite")
         ])
     charges = charges.join(aggch, on="CaseNumber")
     charges = charges.select(
         "CaseNumber",
         "Num",
```

### Comparing `alacorder-79.6.2/PKG-INFO` & `alacorder-79.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 79.6.2
+Version: 79.6.3
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

