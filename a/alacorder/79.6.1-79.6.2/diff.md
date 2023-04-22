# Comparing `tmp/alacorder-79.6.1.tar.gz` & `tmp/alacorder-79.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-79.6.1.tar", max compression
+gzip compressed data, was "alacorder-79.6.2.tar", max compression
```

## Comparing `alacorder-79.6.1.tar` & `alacorder-79.6.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.6.1/LICENSE
--rw-r--r--   0        0        0     9558 2023-04-19 15:07:38.263494 alacorder-79.6.1/README.md
--rw-r--r--   0        0        0      679 2023-04-21 22:16:00.901925 alacorder-79.6.1/pyproject.toml
--rw-r--r--   0        0        0     9208 2023-04-21 18:06:44.921207 alacorder-79.6.1/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb
--rw-r--r--   0        0        0   138382 2023-04-21 18:24:49.412475 alacorder-79.6.1/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.6.1/src/alacorder/.python-version
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.6.1/src/alacorder/__init__.py
--rw-r--r--   0        0        0   139277 2023-04-21 22:15:52.617131 alacorder-79.6.1/src/alacorder/__main__.py
--rw-r--r--   0        0        0   139277 2023-04-21 22:15:32.172949 alacorder-79.6.1/src/alacorder/alac.py
--rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.6.1/src/alacorder/~$E 302 Portfolio.docx
--rw-r--r--   0        0        0    10448 1970-01-01 00:00:00.000000 alacorder-79.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.6.2/LICENSE
+-rw-r--r--   0        0        0     9558 2023-04-19 15:07:38.263494 alacorder-79.6.2/README.md
+-rw-r--r--   0        0        0      679 2023-04-22 13:52:51.007703 alacorder-79.6.2/pyproject.toml
+-rw-r--r--   0        0        0     9208 2023-04-21 18:06:44.921207 alacorder-79.6.2/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb
+-rw-r--r--   0        0        0   138382 2023-04-21 18:24:49.412475 alacorder-79.6.2/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.6.2/src/alacorder/.python-version
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.6.2/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   139605 2023-04-22 13:52:25.429230 alacorder-79.6.2/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   139605 2023-04-22 13:52:12.231450 alacorder-79.6.2/src/alacorder/alac.py
+-rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.6.2/src/alacorder/~$E 302 Portfolio.docx
+-rw-r--r--   0        0        0    10448 1970-01-01 00:00:00.000000 alacorder-79.6.2/PKG-INFO
```

### Comparing `alacorder-79.6.1/LICENSE` & `alacorder-79.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.1/README.md` & `alacorder-79.6.2/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.1/pyproject.toml` & `alacorder-79.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "79.6.1"
+version = "79.6.2"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-79.6.1/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb` & `alacorder-79.6.2/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.1/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-79.6.2/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.1/src/alacorder/__init__.py` & `alacorder-79.6.2/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.1/src/alacorder/__main__.py` & `alacorder-79.6.2/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     tqdm, 
     xlsxwriter, 
     xlsx2csv
 
 """
 
 name = "ALACORDER"
-version = "79.6.1"
+version = "79.6.2"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 if autoload_graphical_user_interface:
     import PySimpleGUI as sg
 
@@ -32,15 +32,15 @@
 from tqdm.auto import tqdm
 import click, fitz, selenium, os, sys, time, glob, re, xlsxwriter, threading, platform
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.chrome.options import Options
 
-pl.Config.set_tbl_rows(10)
+pl.Config.set_tbl_rows(20)
 pl.Config.set_fmt_str_lengths(100)
 pl.Config.set_tbl_width_chars(80)
 pl.Config.set_tbl_formatting("NOTHING")
 pl.Config.set_tbl_hide_column_data_types(True)
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 fname = f"{name} {version}"
@@ -1311,14 +1311,15 @@
     outputs = None if no_write else outputs
     no_write = True if outputs == None else no_write
     found = 0
 
     if debug:
         sys.tracebacklimit = 10
         pl.Config.set_verbose(True)
+        pl.Config.set_tbl_rows(100)
     else:
         sys.tracebacklimit = 1
         pl.Config.set_verbose(False)
 
     # raise overwrite error
     if no_write:
         outputext = "none"
@@ -2439,15 +2440,15 @@
             .str.extract(r"(\d\d/\d\d/\d\d\d\d)", group_index=1)
             .alias("CourtActionDate"),
             pl.col("Charges")
             .str.extract(
                 r"[A-Z0-9]{3}-[A-Z0-9]{3}-[A-Z0-9]{3}\({0,1}[A-Z]{0,1}\){0,1}\.{0,1}\d{0,1}",
                 group_index=0,
             )
-            .alias("Cite"),
+            .alias("RAWCITE"),
             pl.col("Charges")
             .str.extract(
                 r"(BOUND|GUILTY PLEA|WAIVED TO GJ|DISMISSED|TIME LAPSED|NOL PROSS|CONVICTED|INDICTED|DISMISSED|FORFEITURE|TRANSFER|REMANDED|WAIVED|ACQUITTED|WITHDRAWN|PETITION|PRETRIAL|COND\. FORF\.)",
                 group_index=1,
             )
             .alias("CourtAction"),
             pl.col("Charges")
@@ -2476,15 +2477,15 @@
         [
             pl.when(pl.col("Disposition"))
             .then(pl.col("Split").arr.get(1))
             .otherwise(pl.col("Split").arr.get(0).str.slice(9))
             .str.replace(r"-   -", "", literal=True)
             .str.replace("1STS", "1ST", literal=True)
             .str.strip()
-            .alias("Description"),
+            .alias("RAWDESC"),
             pl.when(pl.col("Disposition"))
             .then(pl.col("Split").arr.get(0).str.slice(19))
             .otherwise(pl.col("Split").arr.get(1))
             .str.strip()
             .alias("SEG_2"),
             pl.when(pl.col("Disposition") == True)
             .then(False)
@@ -2504,21 +2505,21 @@
             .alias("TypeDescription"),
             pl.col("SEG_2")
             .str.extract(
                 r"(ALCOHOL|BOND|CONSERVATION|DOCKET|DRUG|GOVERNMENT|HEALTH|MUNICIPAL|OTHER|PERSONAL|PROPERTY|SEX|TRAFFIC)",
                 group_index=1,
             )
             .alias("Category"),
-            pl.col("Description")
+            pl.col("RAWDESC")
             .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP)")
             .is_not()
             .alias("A_S_C_DISQ"),
             pl.col("Code")
             .str.contains(
-                "(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
+                r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
             )
             .alias("CERV_DISQ_MATCH"),
             pl.col("Code")
             .str.contains(
                 r"(RAP1|RAP2|SOD1|SOD2|STSA|SXA1|SXA2|ECHI|SX12|CSSC|FTCS|MURD|MRDI|MURR|FMUR|PMIO|POBM|MIPR|POMA|INCE)"
             )
             .alias("PARDON_DISQ_MATCH"),
@@ -2577,14 +2578,21 @@
             .alias("PermanentDisqConviction"),
             pl.when(pl.col("PERM_DISQ_MATCH") & pl.col("Felony") & pl.col("A_S_C_DISQ"))
             .then(True)
             .otherwise(False)
             .alias("PermanentDisqCharge"),
         ]
     )
+    aggch = charges.groupby("CaseNumber").agg("RAWCITE","RAWDESC")
+    aggch = aggch.select([
+        pl.col("CaseNumber"),
+        pl.col("RAWDESC").arr.get(0).alias("Description"),
+        pl.col("RAWCITE").arr.get(0).alias("Cite")
+        ])
+    charges = charges.join(aggch, on="CaseNumber")
     charges = charges.select(
         "CaseNumber",
         "Num",
         "Code",
         "Cite",
         "Description",
         "TypeDescription",
```

### Comparing `alacorder-79.6.1/src/alacorder/alac.py` & `alacorder-79.6.2/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     tqdm, 
     xlsxwriter, 
     xlsx2csv
 
 """
 
 name = "ALACORDER"
-version = "79.6.1"
+version = "79.6.2"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 if autoload_graphical_user_interface:
     import PySimpleGUI as sg
 
@@ -32,15 +32,15 @@
 from tqdm.auto import tqdm
 import click, fitz, selenium, os, sys, time, glob, re, xlsxwriter, threading, platform
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.chrome.options import Options
 
-pl.Config.set_tbl_rows(10)
+pl.Config.set_tbl_rows(20)
 pl.Config.set_fmt_str_lengths(100)
 pl.Config.set_tbl_width_chars(80)
 pl.Config.set_tbl_formatting("NOTHING")
 pl.Config.set_tbl_hide_column_data_types(True)
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 fname = f"{name} {version}"
@@ -1311,14 +1311,15 @@
     outputs = None if no_write else outputs
     no_write = True if outputs == None else no_write
     found = 0
 
     if debug:
         sys.tracebacklimit = 10
         pl.Config.set_verbose(True)
+        pl.Config.set_tbl_rows(100)
     else:
         sys.tracebacklimit = 1
         pl.Config.set_verbose(False)
 
     # raise overwrite error
     if no_write:
         outputext = "none"
@@ -2439,15 +2440,15 @@
             .str.extract(r"(\d\d/\d\d/\d\d\d\d)", group_index=1)
             .alias("CourtActionDate"),
             pl.col("Charges")
             .str.extract(
                 r"[A-Z0-9]{3}-[A-Z0-9]{3}-[A-Z0-9]{3}\({0,1}[A-Z]{0,1}\){0,1}\.{0,1}\d{0,1}",
                 group_index=0,
             )
-            .alias("Cite"),
+            .alias("RAWCITE"),
             pl.col("Charges")
             .str.extract(
                 r"(BOUND|GUILTY PLEA|WAIVED TO GJ|DISMISSED|TIME LAPSED|NOL PROSS|CONVICTED|INDICTED|DISMISSED|FORFEITURE|TRANSFER|REMANDED|WAIVED|ACQUITTED|WITHDRAWN|PETITION|PRETRIAL|COND\. FORF\.)",
                 group_index=1,
             )
             .alias("CourtAction"),
             pl.col("Charges")
@@ -2476,15 +2477,15 @@
         [
             pl.when(pl.col("Disposition"))
             .then(pl.col("Split").arr.get(1))
             .otherwise(pl.col("Split").arr.get(0).str.slice(9))
             .str.replace(r"-   -", "", literal=True)
             .str.replace("1STS", "1ST", literal=True)
             .str.strip()
-            .alias("Description"),
+            .alias("RAWDESC"),
             pl.when(pl.col("Disposition"))
             .then(pl.col("Split").arr.get(0).str.slice(19))
             .otherwise(pl.col("Split").arr.get(1))
             .str.strip()
             .alias("SEG_2"),
             pl.when(pl.col("Disposition") == True)
             .then(False)
@@ -2504,21 +2505,21 @@
             .alias("TypeDescription"),
             pl.col("SEG_2")
             .str.extract(
                 r"(ALCOHOL|BOND|CONSERVATION|DOCKET|DRUG|GOVERNMENT|HEALTH|MUNICIPAL|OTHER|PERSONAL|PROPERTY|SEX|TRAFFIC)",
                 group_index=1,
             )
             .alias("Category"),
-            pl.col("Description")
+            pl.col("RAWDESC")
             .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP)")
             .is_not()
             .alias("A_S_C_DISQ"),
             pl.col("Code")
             .str.contains(
-                "(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
+                r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
             )
             .alias("CERV_DISQ_MATCH"),
             pl.col("Code")
             .str.contains(
                 r"(RAP1|RAP2|SOD1|SOD2|STSA|SXA1|SXA2|ECHI|SX12|CSSC|FTCS|MURD|MRDI|MURR|FMUR|PMIO|POBM|MIPR|POMA|INCE)"
             )
             .alias("PARDON_DISQ_MATCH"),
@@ -2577,14 +2578,21 @@
             .alias("PermanentDisqConviction"),
             pl.when(pl.col("PERM_DISQ_MATCH") & pl.col("Felony") & pl.col("A_S_C_DISQ"))
             .then(True)
             .otherwise(False)
             .alias("PermanentDisqCharge"),
         ]
     )
+    aggch = charges.groupby("CaseNumber").agg("RAWCITE","RAWDESC")
+    aggch = aggch.select([
+        pl.col("CaseNumber"),
+        pl.col("RAWDESC").arr.get(0).alias("Description"),
+        pl.col("RAWCITE").arr.get(0).alias("Cite")
+        ])
+    charges = charges.join(aggch, on="CaseNumber")
     charges = charges.select(
         "CaseNumber",
         "Num",
         "Code",
         "Cite",
         "Description",
         "TypeDescription",
```

### Comparing `alacorder-79.6.1/PKG-INFO` & `alacorder-79.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 79.6.1
+Version: 79.6.2
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

