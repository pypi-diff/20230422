# Comparing `tmp/unwanted_content_detector-0.1.1.tar.gz` & `tmp/unwanted_content_detector-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unwanted_content_detector-0.1.1.tar", max compression
+gzip compressed data, was "unwanted_content_detector-0.1.2.tar", max compression
```

## Comparing `unwanted_content_detector-0.1.1.tar` & `unwanted_content_detector-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0     1331 2023-04-22 20:35:33.710968 unwanted_content_detector-0.1.1/README.md
--rw-r--r--   0        0        0      619 2023-04-22 20:40:32.844302 unwanted_content_detector-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       31 2023-04-13 21:09:25.299508 unwanted_content_detector-0.1.1/unwanted_content_detector/__init__.py
--rw-r--r--   0        0        0      497 2023-04-13 21:09:25.299899 unwanted_content_detector-0.1.1/unwanted_content_detector/detector.py
--rw-r--r--   0        0        0      161 2023-04-02 10:45:59.495528 unwanted_content_detector-0.1.1/unwanted_content_detector/entities.py
--rw-r--r--   0        0        0     1405 2023-04-21 18:36:13.070815 unwanted_content_detector-0.1.1/unwanted_content_detector/evaluator/evaluator.py
--rw-r--r--   0        0        0        0 2023-04-01 11:49:01.792441 unwanted_content_detector-0.1.1/unwanted_content_detector/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 21:09:25.300529 unwanted_content_detector-0.1.1/unwanted_content_detector/models/distilbert_finetuned/__init__.py
--rw-r--r--   0        0        0      926 2023-04-22 20:25:08.130551 unwanted_content_detector-0.1.1/unwanted_content_detector/models/distilbert_finetuned/inference.py
--rw-r--r--   0        0        0     3805 2023-04-22 20:06:52.551673 unwanted_content_detector-0.1.1/unwanted_content_detector/models/distilbert_finetuned/train.py
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 unwanted_content_detector-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1331 2023-04-22 20:35:33.710968 unwanted_content_detector-0.1.2/README.md
+-rw-r--r--   0        0        0      619 2023-04-22 20:44:21.335867 unwanted_content_detector-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-04-13 21:09:25.299508 unwanted_content_detector-0.1.2/unwanted_content_detector/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 20:42:32.601085 unwanted_content_detector-0.1.2/unwanted_content_detector/data/__init__.py
+-rw-r--r--   0        0        0    11062 2023-04-13 21:09:25.299076 unwanted_content_detector-0.1.2/unwanted_content_detector/data/data.csv
+-rw-r--r--   0        0        0      490 2023-04-01 11:23:42.326632 unwanted_content_detector-0.1.2/unwanted_content_detector/data/generative_prompts.txt
+-rw-r--r--   0        0        0      183 2023-04-22 20:43:32.978787 unwanted_content_detector-0.1.2/unwanted_content_detector/data/loader.py
+-rw-r--r--   0        0        0      497 2023-04-13 21:09:25.299899 unwanted_content_detector-0.1.2/unwanted_content_detector/detector.py
+-rw-r--r--   0        0        0      161 2023-04-02 10:45:59.495528 unwanted_content_detector-0.1.2/unwanted_content_detector/entities.py
+-rw-r--r--   0        0        0     1337 2023-04-22 20:42:36.005969 unwanted_content_detector-0.1.2/unwanted_content_detector/evaluator/evaluator.py
+-rw-r--r--   0        0        0        0 2023-04-01 11:49:01.792441 unwanted_content_detector-0.1.2/unwanted_content_detector/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 21:09:25.300529 unwanted_content_detector-0.1.2/unwanted_content_detector/models/distilbert_finetuned/__init__.py
+-rw-r--r--   0        0        0      926 2023-04-22 20:25:08.130551 unwanted_content_detector-0.1.2/unwanted_content_detector/models/distilbert_finetuned/inference.py
+-rw-r--r--   0        0        0     3831 2023-04-22 20:42:36.003090 unwanted_content_detector-0.1.2/unwanted_content_detector/models/distilbert_finetuned/train.py
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 unwanted_content_detector-0.1.2/PKG-INFO
```

### Comparing `unwanted_content_detector-0.1.1/README.md` & `unwanted_content_detector-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.1/pyproject.toml` & `unwanted_content_detector-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unwanted-content-detector"
-version = "0.1.1"
+version = "0.1.2"
 description = "A library to detect undesired, unbranded, or harmful content"
 authors = ["Jean Carlo Machado <jean.machado@getyourguide.com>"]
 license = "Apache"
 readme = "README.md"
 packages = [{include = "unwanted_content_detector"}]
 
 [tool.poetry.dependencies]
```

### Comparing `unwanted_content_detector-0.1.1/unwanted_content_detector/evaluator/evaluator.py` & `unwanted_content_detector-0.1.2/unwanted_content_detector/evaluator/evaluator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
 
-from data.loader import load_data
+from unwanted_content_detector.data.loader import load_data
 from unwanted_content_detector.entities import Label
 
 
 def random_guess(_):
     return random.choice([Label.UNWANTED_CONTENT.value, Label.SAFE_CONTENT.value])
 
 
@@ -19,15 +19,14 @@
         return self.evaluate_function(inference.infer)
 
     def evaluate_random(self):
         self.evaluate_function(random_guess)
 
     def evaluate_function(self, fn):
         """ Evaluates the entire dataset in a given model """
-        from unwanted_content_detector.models.distilbert_finetuned.inference import Inference
         data = load_data()
 
         Y = data.iloc[:, -1:]
         X = data.iloc[:, 0:]
 
         total = len(Y)
         print(f"Total items: {total}")
```

### Comparing `unwanted_content_detector-0.1.1/unwanted_content_detector/models/distilbert_finetuned/inference.py` & `unwanted_content_detector-0.1.2/unwanted_content_detector/models/distilbert_finetuned/inference.py`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.1/unwanted_content_detector/models/distilbert_finetuned/train.py` & `unwanted_content_detector-0.1.2/unwanted_content_detector/models/distilbert_finetuned/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import os
 
-from data.loader import load_data
+from unwanted_content_detector.data.loader import load_data
 from unwanted_content_detector.evaluator.evaluator import Evaluator
 
 MODEL_NAME = "detector_distilbert_01"
 SPLIT_SIZE = 0.4
 ID_2_LABEL = {0: "SAFE_CONTENT", 1: "UNWANTED_CONTENT"}
 LABEL_2_ID = {"UNWANTED_CONTENT": 0, "SAFE_CONTENT": 1}
```

### Comparing `unwanted_content_detector-0.1.1/PKG-INFO` & `unwanted_content_detector-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unwanted-content-detector
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library to detect undesired, unbranded, or harmful content
 License: Apache
 Author: Jean Carlo Machado
 Author-email: jean.machado@getyourguide.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

