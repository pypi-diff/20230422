# Comparing `tmp/bioframe-0.4.0.tar.gz` & `tmp/bioframe-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioframe-0.4.0.tar", last modified: Thu Mar 23 22:11:11 2023, max compression
+gzip compressed data, was "bioframe-0.4.1.tar", last modified: Sat Apr 22 15:37:33 2023, max compression
```

## Comparing `bioframe-0.4.0.tar` & `bioframe-0.4.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:11:11.926967 bioframe-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-23 22:10:57.000000 bioframe-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-23 22:10:57.000000 bioframe-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-03-23 22:11:11.926967 bioframe-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-03-23 22:10:57.000000 bioframe-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:11:11.918967 bioframe-0.4.0/bioframe/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:11:11.918967 bioframe-0.4.0/bioframe/core/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25017 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/core/arrops.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/core/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/core/construction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/core/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/core/stringops.py
--rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/extras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:11:11.922967 bioframe-0.4.0/bioframe/io/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:11:11.926967 bioframe-0.4.0/bioframe/io/data/
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/GRCh37.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/ce10.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/ce11.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    70878 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/danRer10.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    66339 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/danRer11.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/dm3.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   161973 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/dm6.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/hg19.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    16501 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/hg38.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/mm10.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/mm39.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/mm9.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/sacCer3.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/t2t-chm13-v1.0.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/t2t-chm13-v1.1.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/data/wuhCor1.seqinfo.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    19560 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/fileops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/io/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    61639 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-03-23 22:10:57.000000 bioframe-0.4.0/bioframe/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:11:11.918967 bioframe-0.4.0/bioframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-03-23 22:11:11.000000 bioframe-0.4.0/bioframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-23 22:11:11.000000 bioframe-0.4.0/bioframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 22:11:11.000000 bioframe-0.4.0/bioframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 22:11:11.000000 bioframe-0.4.0/bioframe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-23 22:11:11.000000 bioframe-0.4.0/bioframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-23 22:11:11.000000 bioframe-0.4.0/bioframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-23 22:11:11.926967 bioframe-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-23 22:10:57.000000 bioframe-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:37:33.015709 bioframe-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-22 15:37:22.000000 bioframe-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-22 15:37:22.000000 bioframe-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-22 15:37:33.015709 bioframe-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-22 15:37:22.000000 bioframe-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:37:33.011709 bioframe-0.4.1/bioframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:37:33.011709 bioframe-0.4.1/bioframe/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25017 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/core/arrops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/core/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/core/construction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/core/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/core/stringops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/extras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:37:33.011709 bioframe-0.4.1/bioframe/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:37:33.015709 bioframe-0.4.1/bioframe/io/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/GRCh37.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/ce10.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/ce11.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    70878 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/danRer10.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    66339 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/danRer11.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/dm3.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   161973 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/dm6.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/hg19.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    16501 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/hg38.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/mm10.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/mm39.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/mm9.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/sacCer3.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/t2t-chm13-v1.0.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/t2t-chm13-v1.1.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/data/wuhCor1.seqinfo.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    19560 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/fileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/io/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61776 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-22 15:37:22.000000 bioframe-0.4.1/bioframe/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:37:33.011709 bioframe-0.4.1/bioframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-22 15:37:32.000000 bioframe-0.4.1/bioframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-22 15:37:32.000000 bioframe-0.4.1/bioframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 15:37:32.000000 bioframe-0.4.1/bioframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 15:37:32.000000 bioframe-0.4.1/bioframe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-22 15:37:32.000000 bioframe-0.4.1/bioframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-22 15:37:32.000000 bioframe-0.4.1/bioframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-22 15:37:33.015709 bioframe-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-22 15:37:22.000000 bioframe-0.4.1/setup.py
```

### Comparing `bioframe-0.4.0/LICENSE` & `bioframe-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/PKG-INFO` & `bioframe-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioframe
-Version: 0.4.0
+Version: 0.4.1
 Summary: Pandas utilities for tab-delimited and other genomic files
 Home-page: https://github.com/open2c/bioframe
 Author: Open2C
 Author-email: nezar@mit.edu
 License: MIT
 Keywords: pandas,dataframe,genomics,epigenomics,bioinformatics,intervals
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bioframe-0.4.0/README.md` & `bioframe-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/core/arrops.py` & `bioframe-0.4.1/bioframe/core/arrops.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/core/checks.py` & `bioframe-0.4.1/bioframe/core/checks.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/core/construction.py` & `bioframe-0.4.1/bioframe/core/construction.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/core/specs.py` & `bioframe-0.4.1/bioframe/core/specs.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/core/stringops.py` & `bioframe-0.4.1/bioframe/core/stringops.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/extras.py` & `bioframe-0.4.1/bioframe/extras.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/data/GRCh37.seqinfo.tsv` & `bioframe-0.4.1/bioframe/io/data/GRCh37.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/data/danRer10.seqinfo.tsv` & `bioframe-0.4.1/bioframe/io/data/danRer10.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/data/danRer11.seqinfo.tsv` & `bioframe-0.4.1/bioframe/io/data/danRer11.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/data/dm3.seqinfo.tsv` & `bioframe-0.4.1/bioframe/io/data/dm3.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/data/dm6.seqinfo.tsv` & `bioframe-0.4.1/bioframe/io/data/dm6.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/data/hg19.seqinfo.tsv` & `bioframe-0.4.1/bioframe/io/data/hg19.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/data/hg38.seqinfo.tsv` & `bioframe-0.4.1/bioframe/io/data/hg38.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/data/mm10.seqinfo.tsv` & `bioframe-0.4.1/bioframe/io/data/mm10.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/data/mm39.seqinfo.tsv` & `bioframe-0.4.1/bioframe/io/data/mm39.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/data/mm9.seqinfo.tsv` & `bioframe-0.4.1/bioframe/io/data/mm9.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/data/sacCer3.seqinfo.tsv` & `bioframe-0.4.1/bioframe/io/data/sacCer3.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/data/t2t-chm13-v1.0.seqinfo.tsv` & `bioframe-0.4.1/bioframe/io/data/t2t-chm13-v1.0.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/data/t2t-chm13-v1.1.seqinfo.tsv` & `bioframe-0.4.1/bioframe/io/data/t2t-chm13-v1.1.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/fileops.py` & `bioframe-0.4.1/bioframe/io/fileops.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/resources.py` & `bioframe-0.4.1/bioframe/io/resources.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/io/schemas.py` & `bioframe-0.4.1/bioframe/io/schemas.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe/ops.py` & `bioframe-0.4.1/bioframe/ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,20 +50,27 @@
     -------
     Boolean array of shape (len(df),)
     """
     ck, sk, ek = _get_default_colnames() if cols is None else cols
     _verify_columns(df, [ck, sk, ek])
 
     chrom, start, end = parse_region(region)
+
     if chrom is None:
         raise ValueError("no chromosome detected, check region input")
-    if (start is not None) and (end is not None):
-        mask = (df[ck] == chrom) & (df[sk] < end) & (df[ek] >= start)
-    else:
+
+    if start is None:
         mask = df[ck] == chrom
+    else:
+        if end is None:
+            end = np.inf
+        mask = (df[ck] == chrom) & (
+            ((df[sk] < end) & (df[ek] > start)) | 
+            ((df[sk] == df[ek]) & (df[sk] == start))  # include points at query start
+        )
     return mask.to_numpy()
 
 
 def select_indices(df, region, cols=None):
     """
     Return integer indices of all genomic intervals that overlap a query range.
```

### Comparing `bioframe-0.4.0/bioframe/vis.py` & `bioframe-0.4.1/bioframe/vis.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/bioframe.egg-info/PKG-INFO` & `bioframe-0.4.1/bioframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioframe
-Version: 0.4.0
+Version: 0.4.1
 Summary: Pandas utilities for tab-delimited and other genomic files
 Home-page: https://github.com/open2c/bioframe
 Author: Open2C
 Author-email: nezar@mit.edu
 License: MIT
 Keywords: pandas,dataframe,genomics,epigenomics,bioinformatics,intervals
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bioframe-0.4.0/bioframe.egg-info/SOURCES.txt` & `bioframe-0.4.1/bioframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioframe-0.4.0/setup.py` & `bioframe-0.4.1/setup.py`

 * *Files identical despite different names*

