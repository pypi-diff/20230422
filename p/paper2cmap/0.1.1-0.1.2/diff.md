# Comparing `tmp/paper2cmap-0.1.1.tar.gz` & `tmp/paper2cmap-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper2cmap-0.1.1.tar", last modified: Sat Apr 22 08:40:39 2023, max compression
+gzip compressed data, was "paper2cmap-0.1.2.tar", last modified: Sat Apr 22 08:52:41 2023, max compression
```

## Comparing `paper2cmap-0.1.1.tar` & `paper2cmap-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:40:39.475427 paper2cmap-0.1.1/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1065 2023-04-21 13:31:25.000000 paper2cmap-0.1.1/LICENSE
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       41 2023-04-22 02:05:11.000000 paper2cmap-0.1.1/MANIFEST.in
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5465 2023-04-22 08:40:39.475427 paper2cmap-0.1.1/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3686 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/README.md
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:40:39.467427 paper2cmap-0.1.1/paper2cmap/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      179 2023-04-22 08:39:53.000000 paper2cmap-0.1.1/paper2cmap/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5243 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/paper2cmap/cmapgpt.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2368 2023-04-21 16:55:29.000000 paper2cmap-0.1.1/paper2cmap/llm.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      409 2023-04-21 11:49:55.000000 paper2cmap-0.1.1/paper2cmap/logger.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:40:39.471427 paper2cmap-0.1.1/paper2cmap/metas/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1157 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/paper2cmap/metas/generate_examples.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)        8 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/paper2cmap/metas/merge_and_prune_examples.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2798 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/paper2cmap/metas/prompts.yaml
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5449 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/paper2cmap/paper2cmap.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3700 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/paper2cmap/paper_reader.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:40:39.471427 paper2cmap-0.1.1/paper2cmap.egg-info/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5465 2023-04-22 08:40:39.000000 paper2cmap-0.1.1/paper2cmap.egg-info/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      540 2023-04-22 08:40:39.000000 paper2cmap-0.1.1/paper2cmap.egg-info/SOURCES.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)        1 2023-04-22 08:40:39.000000 paper2cmap-0.1.1/paper2cmap.egg-info/dependency_links.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       53 2023-04-22 08:40:39.000000 paper2cmap-0.1.1/paper2cmap.egg-info/requires.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       11 2023-04-22 08:40:39.000000 paper2cmap-0.1.1/paper2cmap.egg-info/top_level.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      816 2023-04-22 08:39:43.000000 paper2cmap-0.1.1/pyproject.toml
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-22 08:40:39.475427 paper2cmap-0.1.1/setup.cfg
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:40:39.475427 paper2cmap-0.1.1/tests/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1979 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/tests/test_cmapgpt.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      400 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/tests/test_paper2cmap.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      474 2023-04-22 08:39:00.000000 paper2cmap-0.1.1/tests/test_paper_reader.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:52:41.781001 paper2cmap-0.1.2/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1065 2023-04-21 13:31:25.000000 paper2cmap-0.1.2/LICENSE
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       41 2023-04-22 02:05:11.000000 paper2cmap-0.1.2/MANIFEST.in
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5465 2023-04-22 08:52:41.781001 paper2cmap-0.1.2/PKG-INFO
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3686 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/README.md
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:52:41.773001 paper2cmap-0.1.2/paper2cmap/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      179 2023-04-22 08:52:16.000000 paper2cmap-0.1.2/paper2cmap/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5243 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/paper2cmap/cmapgpt.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2368 2023-04-21 16:55:29.000000 paper2cmap-0.1.2/paper2cmap/llm.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      409 2023-04-21 11:49:55.000000 paper2cmap-0.1.2/paper2cmap/logger.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:52:41.777001 paper2cmap-0.1.2/paper2cmap/metas/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1157 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/paper2cmap/metas/generate_examples.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)        8 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/paper2cmap/metas/merge_and_prune_examples.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2798 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/paper2cmap/metas/prompts.yaml
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5485 2023-04-22 08:51:30.000000 paper2cmap-0.1.2/paper2cmap/paper2cmap.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3700 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/paper2cmap/paper_reader.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:52:41.777001 paper2cmap-0.1.2/paper2cmap.egg-info/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5465 2023-04-22 08:52:41.000000 paper2cmap-0.1.2/paper2cmap.egg-info/PKG-INFO
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      540 2023-04-22 08:52:41.000000 paper2cmap-0.1.2/paper2cmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)        1 2023-04-22 08:52:41.000000 paper2cmap-0.1.2/paper2cmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       53 2023-04-22 08:52:41.000000 paper2cmap-0.1.2/paper2cmap.egg-info/requires.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       11 2023-04-22 08:52:41.000000 paper2cmap-0.1.2/paper2cmap.egg-info/top_level.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      816 2023-04-22 08:51:54.000000 paper2cmap-0.1.2/pyproject.toml
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-22 08:52:41.781001 paper2cmap-0.1.2/setup.cfg
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-22 08:52:41.781001 paper2cmap-0.1.2/tests/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1979 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/tests/test_cmapgpt.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      400 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/tests/test_paper2cmap.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      474 2023-04-22 08:39:00.000000 paper2cmap-0.1.2/tests/test_paper_reader.py
```

### Comparing `paper2cmap-0.1.1/LICENSE` & `paper2cmap-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `paper2cmap-0.1.1/PKG-INFO` & `paper2cmap-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper2cmap
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package that automatically generates a concept map for a PDF document using LLM.
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `paper2cmap-0.1.1/README.md` & `paper2cmap-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `paper2cmap-0.1.1/paper2cmap/cmapgpt.py` & `paper2cmap-0.1.2/paper2cmap/cmapgpt.py`

 * *Files identical despite different names*

### Comparing `paper2cmap-0.1.1/paper2cmap/llm.py` & `paper2cmap-0.1.2/paper2cmap/llm.py`

 * *Files identical despite different names*

### Comparing `paper2cmap-0.1.1/paper2cmap/metas/generate_examples.json` & `paper2cmap-0.1.2/paper2cmap/metas/generate_examples.json`

 * *Files identical despite different names*

### Comparing `paper2cmap-0.1.1/paper2cmap/metas/prompts.yaml` & `paper2cmap-0.1.2/paper2cmap/metas/prompts.yaml`

 * *Files identical despite different names*

### Comparing `paper2cmap-0.1.1/paper2cmap/paper2cmap.py` & `paper2cmap-0.1.2/paper2cmap/paper2cmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Dict, List
 import colorlog
 
 from paper2cmap import LLMManager, CMapGPT, PaperReader, logger
 
 
 class Paper2CMap():
```

### Comparing `paper2cmap-0.1.1/paper2cmap/paper_reader.py` & `paper2cmap-0.1.2/paper2cmap/paper_reader.py`

 * *Files identical despite different names*

### Comparing `paper2cmap-0.1.1/paper2cmap.egg-info/PKG-INFO` & `paper2cmap-0.1.2/paper2cmap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper2cmap
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package that automatically generates a concept map for a PDF document using LLM.
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `paper2cmap-0.1.1/paper2cmap.egg-info/SOURCES.txt` & `paper2cmap-0.1.2/paper2cmap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paper2cmap-0.1.1/pyproject.toml` & `paper2cmap-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "paper2cmap"
-version = "0.1.1"
+version = "0.1.2"
 description = "A package that automatically generates a concept map for a PDF document using LLM."
 readme = "README.md"
 authors = [{ name = "weitian", email = "weitian.bnu@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `paper2cmap-0.1.1/tests/test_cmapgpt.py` & `paper2cmap-0.1.2/tests/test_cmapgpt.py`

 * *Files identical despite different names*

