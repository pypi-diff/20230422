# Comparing `tmp/unwanted_content_detector-0.1.2.tar.gz` & `tmp/unwanted_content_detector-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unwanted_content_detector-0.1.2.tar", max compression
+gzip compressed data, was "unwanted_content_detector-0.1.3.tar", max compression
```

## Comparing `unwanted_content_detector-0.1.2.tar` & `unwanted_content_detector-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1331 2023-04-22 20:35:33.710968 unwanted_content_detector-0.1.2/README.md
--rw-r--r--   0        0        0      619 2023-04-22 20:44:21.335867 unwanted_content_detector-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       31 2023-04-13 21:09:25.299508 unwanted_content_detector-0.1.2/unwanted_content_detector/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 20:42:32.601085 unwanted_content_detector-0.1.2/unwanted_content_detector/data/__init__.py
--rw-r--r--   0        0        0    11062 2023-04-13 21:09:25.299076 unwanted_content_detector-0.1.2/unwanted_content_detector/data/data.csv
--rw-r--r--   0        0        0      490 2023-04-01 11:23:42.326632 unwanted_content_detector-0.1.2/unwanted_content_detector/data/generative_prompts.txt
--rw-r--r--   0        0        0      183 2023-04-22 20:43:32.978787 unwanted_content_detector-0.1.2/unwanted_content_detector/data/loader.py
--rw-r--r--   0        0        0      497 2023-04-13 21:09:25.299899 unwanted_content_detector-0.1.2/unwanted_content_detector/detector.py
--rw-r--r--   0        0        0      161 2023-04-02 10:45:59.495528 unwanted_content_detector-0.1.2/unwanted_content_detector/entities.py
--rw-r--r--   0        0        0     1337 2023-04-22 20:42:36.005969 unwanted_content_detector-0.1.2/unwanted_content_detector/evaluator/evaluator.py
--rw-r--r--   0        0        0        0 2023-04-01 11:49:01.792441 unwanted_content_detector-0.1.2/unwanted_content_detector/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 21:09:25.300529 unwanted_content_detector-0.1.2/unwanted_content_detector/models/distilbert_finetuned/__init__.py
--rw-r--r--   0        0        0      926 2023-04-22 20:25:08.130551 unwanted_content_detector-0.1.2/unwanted_content_detector/models/distilbert_finetuned/inference.py
--rw-r--r--   0        0        0     3831 2023-04-22 20:42:36.003090 unwanted_content_detector-0.1.2/unwanted_content_detector/models/distilbert_finetuned/train.py
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 unwanted_content_detector-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1341 2023-04-22 20:45:16.811744 unwanted_content_detector-0.1.3/README.md
+-rw-r--r--   0        0        0      639 2023-04-22 20:48:44.575023 unwanted_content_detector-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-04-13 21:09:25.299508 unwanted_content_detector-0.1.3/unwanted_content_detector/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 20:42:32.601085 unwanted_content_detector-0.1.3/unwanted_content_detector/data/__init__.py
+-rw-r--r--   0        0        0    11062 2023-04-13 21:09:25.299076 unwanted_content_detector-0.1.3/unwanted_content_detector/data/data.csv
+-rw-r--r--   0        0        0      490 2023-04-01 11:23:42.326632 unwanted_content_detector-0.1.3/unwanted_content_detector/data/generative_prompts.txt
+-rw-r--r--   0        0        0      183 2023-04-22 20:43:32.978787 unwanted_content_detector-0.1.3/unwanted_content_detector/data/loader.py
+-rw-r--r--   0        0        0      497 2023-04-13 21:09:25.299899 unwanted_content_detector-0.1.3/unwanted_content_detector/detector.py
+-rw-r--r--   0        0        0      161 2023-04-02 10:45:59.495528 unwanted_content_detector-0.1.3/unwanted_content_detector/entities.py
+-rw-r--r--   0        0        0     1337 2023-04-22 20:42:36.005969 unwanted_content_detector-0.1.3/unwanted_content_detector/evaluator/evaluator.py
+-rw-r--r--   0        0        0        0 2023-04-01 11:49:01.792441 unwanted_content_detector-0.1.3/unwanted_content_detector/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 21:09:25.300529 unwanted_content_detector-0.1.3/unwanted_content_detector/models/distilbert_finetuned/__init__.py
+-rw-r--r--   0        0        0      926 2023-04-22 20:25:08.130551 unwanted_content_detector-0.1.3/unwanted_content_detector/models/distilbert_finetuned/inference.py
+-rw-r--r--   0        0        0     3831 2023-04-22 20:42:36.003090 unwanted_content_detector-0.1.3/unwanted_content_detector/models/distilbert_finetuned/train.py
+-rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 unwanted_content_detector-0.1.3/PKG-INFO
```

### Comparing `unwanted_content_detector-0.1.2/README.md` & `unwanted_content_detector-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## Usage
 
 In python:
 
 
 ```sh
-pip install unwanted-content-detector
+pip install unwanted-content-detector --upgrade
 ```
 
 With Pandas
 
 ```py
 import pandas as pd
 from unwanted_content_detector import Detector
```

### Comparing `unwanted_content_detector-0.1.2/pyproject.toml` & `unwanted_content_detector-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "unwanted-content-detector"
-version = "0.1.2"
+version = "0.1.3"
 description = "A library to detect undesired, unbranded, or harmful content"
 authors = ["Jean Carlo Machado <jean.machado@getyourguide.com>"]
 license = "Apache"
 readme = "README.md"
 packages = [{include = "unwanted_content_detector"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fire = "^0.5.0"
 pandas = "^2.0.0"
 transformers = "^4.28.0"
+evaluate = "^0.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `unwanted_content_detector-0.1.2/unwanted_content_detector/data/data.csv` & `unwanted_content_detector-0.1.3/unwanted_content_detector/data/data.csv`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.2/unwanted_content_detector/evaluator/evaluator.py` & `unwanted_content_detector-0.1.3/unwanted_content_detector/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.2/unwanted_content_detector/models/distilbert_finetuned/inference.py` & `unwanted_content_detector-0.1.3/unwanted_content_detector/models/distilbert_finetuned/inference.py`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.2/unwanted_content_detector/models/distilbert_finetuned/train.py` & `unwanted_content_detector-0.1.3/unwanted_content_detector/models/distilbert_finetuned/train.py`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.2/PKG-INFO` & `unwanted_content_detector-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: unwanted-content-detector
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library to detect undesired, unbranded, or harmful content
 License: Apache
 Author: Jean Carlo Machado
 Author-email: jean.machado@getyourguide.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: evaluate (>=0.4.0,<0.5.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: transformers (>=4.28.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Unwanted Content Detector
 
@@ -22,15 +23,15 @@
 
 ## Usage
 
 In python:
 
 
 ```sh
-pip install unwanted-content-detector
+pip install unwanted-content-detector --upgrade
 ```
 
 With Pandas
 
 ```py
 import pandas as pd
 from unwanted_content_detector import Detector
```

