# Comparing `tmp/cleanvision-0.2.0.tar.gz` & `tmp/cleanvision-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sanjana/cleanlab_home/cleanvision/dist/.tmp-pef1lbg3/cleanvision-0.2.0.tar", last modified: Tue Apr 11 03:03:25 2023, max compression
+gzip compressed data, was "cleanvision-0.2.1.tar", last modified: Sat Apr 22 00:33:32 2023, max compression
```

## Comparing `cleanvision-0.2.0.tar` & `cleanvision-0.2.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/
--rw-r--r--   0 sanjana    (501) staff       (20)     5373 2023-04-10 14:40:45.000000 cleanvision-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 sanjana    (501) staff       (20)     2989 2023-04-11 02:44:57.000000 cleanvision-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 sanjana    (501) staff       (20)     3901 2023-04-10 14:40:45.000000 cleanvision-0.2.0/DEVELOPMENT.md
--rw-r--r--   0 sanjana    (501) staff       (20)    34523 2023-04-10 14:40:45.000000 cleanvision-0.2.0/LICENSE
--rw-r--r--   0 sanjana    (501) staff       (20)       58 2023-04-10 14:40:45.000000 cleanvision-0.2.0/MANIFEST.in
--rw-r--r--   0 sanjana    (501) staff       (20)    49935 2023-04-11 03:03:25.000000 cleanvision-0.2.0/PKG-INFO
--rw-r--r--   0 sanjana    (501) staff       (20)     8719 2023-04-11 02:44:57.000000 cleanvision-0.2.0/README.md
--rw-r--r--   0 sanjana    (501) staff       (20)     1747 2023-04-11 02:44:57.000000 cleanvision-0.2.0/pyproject.toml
--rw-r--r--   0 sanjana    (501) staff       (20)       38 2023-04-11 03:03:25.000000 cleanvision-0.2.0/setup.cfg
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision/
--rw-r--r--   0 sanjana    (501) staff       (20)        0 2023-04-10 14:40:45.000000 cleanvision-0.2.0/src/cleanvision/__init__.py
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision/dataset/
--rw-r--r--   0 sanjana    (501) staff       (20)        0 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/dataset/__init__.py
--rw-r--r--   0 sanjana    (501) staff       (20)      978 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/dataset/base_dataset.py
--rw-r--r--   0 sanjana    (501) staff       (20)     1044 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/dataset/folder_dataset.py
--rw-r--r--   0 sanjana    (501) staff       (20)     1076 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/dataset/hf_dataset.py
--rw-r--r--   0 sanjana    (501) staff       (20)     1019 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/dataset/torch_dataset.py
--rw-r--r--   0 sanjana    (501) staff       (20)     1184 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/dataset/utils.py
--rw-r--r--   0 sanjana    (501) staff       (20)    27008 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/imagelab.py
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision/issue_managers/
--rw-r--r--   0 sanjana    (501) staff       (20)     2069 2023-04-10 14:40:45.000000 cleanvision-0.2.0/src/cleanvision/issue_managers/__init__.py
--rw-r--r--   0 sanjana    (501) staff       (20)     8447 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/issue_managers/duplicate_issue_manager.py
--rw-r--r--   0 sanjana    (501) staff       (20)    10509 2023-04-10 14:40:45.000000 cleanvision-0.2.0/src/cleanvision/issue_managers/image_property.py
--rw-r--r--   0 sanjana    (501) staff       (20)    12346 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/issue_managers/image_property_issue_manager.py
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision/utils/
--rw-r--r--   0 sanjana    (501) staff       (20)        0 2023-04-10 14:40:45.000000 cleanvision-0.2.0/src/cleanvision/utils/__init__.py
--rw-r--r--   0 sanjana    (501) staff       (20)     2155 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/utils/base_issue_manager.py
--rw-r--r--   0 sanjana    (501) staff       (20)      668 2023-04-10 14:40:45.000000 cleanvision-0.2.0/src/cleanvision/utils/constants.py
--rw-r--r--   0 sanjana    (501) staff       (20)     3349 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/utils/utils.py
--rw-r--r--   0 sanjana    (501) staff       (20)     1955 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/utils/viz_manager.py
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision.egg-info/
--rw-r--r--   0 sanjana    (501) staff       (20)    49935 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision.egg-info/PKG-INFO
--rw-r--r--   0 sanjana    (501) staff       (20)     1172 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision.egg-info/SOURCES.txt
--rw-r--r--   0 sanjana    (501) staff       (20)        1 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision.egg-info/dependency_links.txt
--rw-r--r--   0 sanjana    (501) staff       (20)      164 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision.egg-info/requires.txt
--rw-r--r--   0 sanjana    (501) staff       (20)       12 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision.egg-info/top_level.txt
-drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/tests/
--rw-r--r--   0 sanjana    (501) staff       (20)     1969 2023-04-11 02:44:57.000000 cleanvision-0.2.0/tests/test_dataset.py
--rw-r--r--   0 sanjana    (501) staff       (20)     8473 2023-04-10 14:40:45.000000 cleanvision-0.2.0/tests/test_duplicate_issue_manager.py
--rw-r--r--   0 sanjana    (501) staff       (20)     4297 2023-04-10 14:40:45.000000 cleanvision-0.2.0/tests/test_image_property_helpers.py
--rw-r--r--   0 sanjana    (501) staff       (20)     3594 2023-04-10 14:40:45.000000 cleanvision-0.2.0/tests/test_image_property_issue_manager.py
--rw-r--r--   0 sanjana    (501) staff       (20)     7528 2023-04-11 02:44:57.000000 cleanvision-0.2.0/tests/test_run.py
--rw-r--r--   0 sanjana    (501) staff       (20)      529 2023-04-10 14:40:45.000000 cleanvision-0.2.0/tests/test_utils.py
--rw-r--r--   0 sanjana    (501) staff       (20)     1064 2023-04-11 02:44:57.000000 cleanvision-0.2.0/tests/test_viz_manager.py
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.783344 cleanvision-0.2.1/
+-rw-r--r--   0 sanjana    (501) staff       (20)     5373 2023-04-10 14:40:45.000000 cleanvision-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 sanjana    (501) staff       (20)     2989 2023-04-11 02:44:57.000000 cleanvision-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 sanjana    (501) staff       (20)     3901 2023-04-10 14:40:45.000000 cleanvision-0.2.1/DEVELOPMENT.md
+-rw-r--r--   0 sanjana    (501) staff       (20)    34523 2023-04-10 14:40:45.000000 cleanvision-0.2.1/LICENSE
+-rw-r--r--   0 sanjana    (501) staff       (20)       58 2023-04-10 14:40:45.000000 cleanvision-0.2.1/MANIFEST.in
+-rw-r--r--   0 sanjana    (501) staff       (20)    49948 2023-04-22 00:33:32.782331 cleanvision-0.2.1/PKG-INFO
+-rw-r--r--   0 sanjana    (501) staff       (20)     8732 2023-04-21 23:53:01.000000 cleanvision-0.2.1/README.md
+-rw-r--r--   0 sanjana    (501) staff       (20)     1747 2023-04-17 23:09:29.000000 cleanvision-0.2.1/pyproject.toml
+-rw-r--r--   0 sanjana    (501) staff       (20)       38 2023-04-22 00:33:32.783490 cleanvision-0.2.1/setup.cfg
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.756636 cleanvision-0.2.1/src/
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.763038 cleanvision-0.2.1/src/cleanvision/
+-rw-r--r--   0 sanjana    (501) staff       (20)      166 2023-04-19 16:30:00.000000 cleanvision-0.2.1/src/cleanvision/__init__.py
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.769802 cleanvision-0.2.1/src/cleanvision/dataset/
+-rw-r--r--   0 sanjana    (501) staff       (20)        0 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/dataset/__init__.py
+-rw-r--r--   0 sanjana    (501) staff       (20)      978 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/dataset/base_dataset.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     1044 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/dataset/folder_dataset.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     1076 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/dataset/hf_dataset.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     1019 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/dataset/torch_dataset.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     1184 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/dataset/utils.py
+-rw-r--r--   0 sanjana    (501) staff       (20)    27295 2023-04-13 20:37:40.000000 cleanvision-0.2.1/src/cleanvision/imagelab.py
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.773065 cleanvision-0.2.1/src/cleanvision/issue_managers/
+-rw-r--r--   0 sanjana    (501) staff       (20)     2069 2023-04-10 14:40:45.000000 cleanvision-0.2.1/src/cleanvision/issue_managers/__init__.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     8399 2023-04-13 20:37:40.000000 cleanvision-0.2.1/src/cleanvision/issue_managers/duplicate_issue_manager.py
+-rw-r--r--   0 sanjana    (501) staff       (20)    10509 2023-04-10 14:40:45.000000 cleanvision-0.2.1/src/cleanvision/issue_managers/image_property.py
+-rw-r--r--   0 sanjana    (501) staff       (20)    12286 2023-04-13 20:37:40.000000 cleanvision-0.2.1/src/cleanvision/issue_managers/image_property_issue_manager.py
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.776538 cleanvision-0.2.1/src/cleanvision/utils/
+-rw-r--r--   0 sanjana    (501) staff       (20)        0 2023-04-10 14:40:45.000000 cleanvision-0.2.1/src/cleanvision/utils/__init__.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     2155 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/utils/base_issue_manager.py
+-rw-r--r--   0 sanjana    (501) staff       (20)      668 2023-04-10 14:40:45.000000 cleanvision-0.2.1/src/cleanvision/utils/constants.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     3349 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/utils/utils.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     1955 2023-04-11 02:44:57.000000 cleanvision-0.2.1/src/cleanvision/utils/viz_manager.py
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.765972 cleanvision-0.2.1/src/cleanvision.egg-info/
+-rw-r--r--   0 sanjana    (501) staff       (20)    49948 2023-04-22 00:33:32.000000 cleanvision-0.2.1/src/cleanvision.egg-info/PKG-INFO
+-rw-r--r--   0 sanjana    (501) staff       (20)     1172 2023-04-22 00:33:32.000000 cleanvision-0.2.1/src/cleanvision.egg-info/SOURCES.txt
+-rw-r--r--   0 sanjana    (501) staff       (20)        1 2023-04-22 00:33:32.000000 cleanvision-0.2.1/src/cleanvision.egg-info/dependency_links.txt
+-rw-r--r--   0 sanjana    (501) staff       (20)      164 2023-04-22 00:33:32.000000 cleanvision-0.2.1/src/cleanvision.egg-info/requires.txt
+-rw-r--r--   0 sanjana    (501) staff       (20)       12 2023-04-22 00:33:32.000000 cleanvision-0.2.1/src/cleanvision.egg-info/top_level.txt
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-22 00:33:32.781672 cleanvision-0.2.1/tests/
+-rw-r--r--   0 sanjana    (501) staff       (20)     1969 2023-04-11 02:44:57.000000 cleanvision-0.2.1/tests/test_dataset.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     8473 2023-04-10 14:40:45.000000 cleanvision-0.2.1/tests/test_duplicate_issue_manager.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     4297 2023-04-10 14:40:45.000000 cleanvision-0.2.1/tests/test_image_property_helpers.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     3594 2023-04-10 14:40:45.000000 cleanvision-0.2.1/tests/test_image_property_issue_manager.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     7541 2023-04-21 23:53:01.000000 cleanvision-0.2.1/tests/test_run.py
+-rw-r--r--   0 sanjana    (501) staff       (20)      529 2023-04-10 14:40:45.000000 cleanvision-0.2.1/tests/test_utils.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     1064 2023-04-11 02:44:57.000000 cleanvision-0.2.1/tests/test_viz_manager.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cleanvision-0.2.0/CODE_OF_CONDUCT.md` & `cleanvision-0.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/CONTRIBUTING.md` & `cleanvision-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/DEVELOPMENT.md` & `cleanvision-0.2.1/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/LICENSE` & `cleanvision-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/PKG-INFO` & `cleanvision-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanvision
-Version: 0.2.0
+Version: 0.2.1
 Summary: Find issues in image datasets
 Author-email: "Cleanlab Inc." <team@cleanlab.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -749,15 +749,15 @@
 
 
 ## More resources on how to use CleanVision
 
 - [Tutorial notebook](https://github.com/cleanlab/cleanvision-examples/blob/main/tutorial.ipynb)
 - [Notebook for running CleanVision on a HuggingFace Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/huggingface_dataset.ipynb)
 - [Notebook for running CleanVision on a Torchvision Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/torchvision_dataset.ipynb)
-- [Example script](https://github.com/cleanlab/cleanvision/blob/main/examples/run.py) that can be run with: `python examples/run.py --path <FOLDER_WITH_IMAGES>`
+- [Example script](https://github.com/cleanlab/cleanvision/blob/main/docs/source/tutorials/run.py) that can be run with: `python examples/run.py --path <FOLDER_WITH_IMAGES>`
 - [Additional example notebooks](https://github.com/cleanlab/cleanvision-examples)
 - [Documentation](https://cleanvision.readthedocs.io/)
 - [Blog Post](https://cleanlab.ai/blog/cleanvision/)
 
 ## *Clean* your data for better Computer *Vision*
 
 The quality of machine learning models hinges on the quality of the data used to train them, but it is hard to manually identify all of the low-quality data in a big dataset. CleanVision helps you automatically identify common types of data issues lurking in image datasets.
```

### Comparing `cleanvision-0.2.0/README.md` & `cleanvision-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 
 ## More resources on how to use CleanVision
 
 - [Tutorial notebook](https://github.com/cleanlab/cleanvision-examples/blob/main/tutorial.ipynb)
 - [Notebook for running CleanVision on a HuggingFace Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/huggingface_dataset.ipynb)
 - [Notebook for running CleanVision on a Torchvision Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/torchvision_dataset.ipynb)
-- [Example script](https://github.com/cleanlab/cleanvision/blob/main/examples/run.py) that can be run with: `python examples/run.py --path <FOLDER_WITH_IMAGES>`
+- [Example script](https://github.com/cleanlab/cleanvision/blob/main/docs/source/tutorials/run.py) that can be run with: `python examples/run.py --path <FOLDER_WITH_IMAGES>`
 - [Additional example notebooks](https://github.com/cleanlab/cleanvision-examples)
 - [Documentation](https://cleanvision.readthedocs.io/)
 - [Blog Post](https://cleanlab.ai/blog/cleanvision/)
 
 ## *Clean* your data for better Computer *Vision*
 
 The quality of machine learning models hinges on the quality of the data used to train them, but it is hard to manually identify all of the low-quality data in a big dataset. CleanVision helps you automatically identify common types of data issues lurking in image datasets.
```

### Comparing `cleanvision-0.2.0/pyproject.toml` & `cleanvision-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cleanvision"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name = "Cleanlab Inc.", email = "team@cleanlab.ai" },
 ]
 description = "Find issues in image datasets"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["computer_vision", "cv", "image_data", "issue_detection", "data_quality", "image_quality", "machine_learning", "data_cleaning", "image_deduplication"]
```

### Comparing `cleanvision-0.2.0/src/cleanvision/dataset/base_dataset.py` & `cleanvision-0.2.1/src/cleanvision/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/src/cleanvision/dataset/folder_dataset.py` & `cleanvision-0.2.1/src/cleanvision/dataset/folder_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/src/cleanvision/dataset/hf_dataset.py` & `cleanvision-0.2.1/src/cleanvision/dataset/hf_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/src/cleanvision/dataset/torch_dataset.py` & `cleanvision-0.2.1/src/cleanvision/dataset/torch_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/src/cleanvision/dataset/utils.py` & `cleanvision-0.2.1/src/cleanvision/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/src/cleanvision/imagelab.py` & `cleanvision-0.2.1/src/cleanvision/imagelab.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import List, Dict, Any, Optional, Tuple, TypeVar, Type
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 from PIL import Image
 
+from cleanvision.dataset.torch_dataset import TorchDataset
 from cleanvision.dataset.utils import build_dataset
 from cleanvision.issue_managers import (
     IssueType,
     IssueManagerFactory,
     ISSUE_MANAGER_REGISTRY,
 )
 from cleanvision.utils.base_issue_manager import IssueManager
@@ -28,14 +29,15 @@
     SETS,
 )
 from cleanvision.utils.utils import (
     deep_update_dict,
     get_is_issue_colname,
     get_score_colname,
     update_df,
+    get_max_n_jobs,
 )
 from cleanvision.utils.viz_manager import VizManager
 
 if TYPE_CHECKING:  # pragma: no cover
     import datasets
     from torchvision.datasets.vision import VisionDataset
 
@@ -256,14 +258,20 @@
             set(self._issue_types).union(set(to_compute_issues_with_params.keys()))
         )
 
         # set issue managers
         issue_type_groups = self._get_issue_type_groups(to_compute_issues_with_params)
         self._set_issue_managers(issue_type_groups)
 
+        # set number of jobs for parallelizing computation
+        if n_jobs is None:
+            n_jobs = get_max_n_jobs()
+            if isinstance(self._dataset, TorchDataset):
+                n_jobs = 1
+
         # find issues
         for issue_type_group, params in issue_type_groups.items():
             issue_manager = self._issue_managers[issue_type_group]
             issue_manager.find_issues(
                 params=params,
                 dataset=self._dataset,
                 imagelab_info=self.info,
```

### Comparing `cleanvision-0.2.0/src/cleanvision/issue_managers/__init__.py` & `cleanvision-0.2.1/src/cleanvision/issue_managers/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/src/cleanvision/issue_managers/duplicate_issue_manager.py` & `cleanvision-0.2.1/src/cleanvision/issue_managers/duplicate_issue_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from PIL import Image
 from tqdm import tqdm
 
 from cleanvision.dataset.base_dataset import Dataset
 from cleanvision.issue_managers import register_issue_manager, IssueType
 from cleanvision.utils.base_issue_manager import IssueManager
 from cleanvision.utils.constants import SETS, DUPLICATE, MAX_PROCS
-from cleanvision.utils.utils import get_max_n_jobs, get_is_issue_colname
+from cleanvision.utils.utils import get_is_issue_colname
 
 
 def get_hash(image: Image, params: Dict[str, Any]) -> str:
     hash_type, hash_size = params["hash_type"], params.get("hash_size", None)
     if hash_type == "md5":
         pixels = np.asarray(image)
         return hashlib.md5(pixels.tobytes()).hexdigest()
@@ -102,26 +102,24 @@
         n_jobs: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         super().find_issues(**kwargs)
         assert params is not None
         assert imagelab_info is not None
         assert dataset is not None
+        assert n_jobs is not None
 
         self.issue_types = list(params.keys())
         self.update_params(params)
 
         to_compute = self._get_issue_types_to_compute(self.issue_types, imagelab_info)
         issue_type_hash_mapping: Dict[str, Any] = {
             issue_type: {} for issue_type in to_compute
         }
 
-        if n_jobs is None:
-            n_jobs = get_max_n_jobs()
-
         results: List[Dict[str, Union[str, int]]] = []
         if n_jobs == 1:
             for idx in tqdm(dataset.index):
                 results.append(compute_hash(idx, dataset, to_compute, self.params))
         else:
             args = [
                 {
```

### Comparing `cleanvision-0.2.0/src/cleanvision/issue_managers/image_property.py` & `cleanvision-0.2.1/src/cleanvision/issue_managers/image_property.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/src/cleanvision/issue_managers/image_property_issue_manager.py` & `cleanvision-0.2.1/src/cleanvision/issue_managers/image_property_issue_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from cleanvision.utils.base_issue_manager import IssueManager
 from cleanvision.utils.constants import (
     IMAGE_PROPERTY,
     MAX_PROCS,
     IMAGE_PROPERTY_ISSUE_TYPES_LIST,
 )
 from cleanvision.utils.utils import (
-    get_max_n_jobs,
     get_is_issue_colname,
     update_df,
     get_score_colname,
 )
 
 
 def compute_scores(
@@ -122,14 +121,15 @@
         n_jobs: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         super().find_issues(**kwargs)
         assert params is not None
         assert imagelab_info is not None
         assert dataset is not None
+        assert n_jobs is not None
 
         self.issue_types = list(params.keys())
         self.issues = pd.DataFrame(index=dataset.index)
         additional_set = self._get_additional_to_compute_set(self.issue_types)
         self.issue_types = self.issue_types + additional_set
 
         self.update_params(params)
@@ -139,17 +139,14 @@
 
         defer_set = self._get_defer_set(self.issue_types, agg_computations)
 
         to_be_computed = list(set(self.issue_types).difference(defer_set))
 
         new_computations = pd.DataFrame(index=dataset.index)
         if to_be_computed:
-            if n_jobs is None:
-                n_jobs = get_max_n_jobs()
-
             results: List[Dict[str, Union[int, float, str]]] = []
             if n_jobs == 1:
                 for idx in tqdm(dataset.index):
                     results.append(
                         compute_scores(
                             idx, dataset, to_be_computed, self.image_properties
                         )
```

### Comparing `cleanvision-0.2.0/src/cleanvision/utils/base_issue_manager.py` & `cleanvision-0.2.1/src/cleanvision/utils/base_issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/src/cleanvision/utils/constants.py` & `cleanvision-0.2.1/src/cleanvision/utils/constants.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/src/cleanvision/utils/utils.py` & `cleanvision-0.2.1/src/cleanvision/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/src/cleanvision/utils/viz_manager.py` & `cleanvision-0.2.1/src/cleanvision/utils/viz_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/src/cleanvision.egg-info/PKG-INFO` & `cleanvision-0.2.1/src/cleanvision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanvision
-Version: 0.2.0
+Version: 0.2.1
 Summary: Find issues in image datasets
 Author-email: "Cleanlab Inc." <team@cleanlab.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -749,15 +749,15 @@
 
 
 ## More resources on how to use CleanVision
 
 - [Tutorial notebook](https://github.com/cleanlab/cleanvision-examples/blob/main/tutorial.ipynb)
 - [Notebook for running CleanVision on a HuggingFace Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/huggingface_dataset.ipynb)
 - [Notebook for running CleanVision on a Torchvision Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/torchvision_dataset.ipynb)
-- [Example script](https://github.com/cleanlab/cleanvision/blob/main/examples/run.py) that can be run with: `python examples/run.py --path <FOLDER_WITH_IMAGES>`
+- [Example script](https://github.com/cleanlab/cleanvision/blob/main/docs/source/tutorials/run.py) that can be run with: `python examples/run.py --path <FOLDER_WITH_IMAGES>`
 - [Additional example notebooks](https://github.com/cleanlab/cleanvision-examples)
 - [Documentation](https://cleanvision.readthedocs.io/)
 - [Blog Post](https://cleanlab.ai/blog/cleanvision/)
 
 ## *Clean* your data for better Computer *Vision*
 
 The quality of machine learning models hinges on the quality of the data used to train them, but it is hard to manually identify all of the low-quality data in a big dataset. CleanVision helps you automatically identify common types of data issues lurking in image datasets.
```

### Comparing `cleanvision-0.2.0/src/cleanvision.egg-info/SOURCES.txt` & `cleanvision-0.2.1/src/cleanvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/tests/test_dataset.py` & `cleanvision-0.2.1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/tests/test_duplicate_issue_manager.py` & `cleanvision-0.2.1/tests/test_duplicate_issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/tests/test_image_property_helpers.py` & `cleanvision-0.2.1/tests/test_image_property_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/tests/test_image_property_issue_manager.py` & `cleanvision-0.2.1/tests/test_image_property_issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/tests/test_run.py` & `cleanvision-0.2.1/tests/test_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from cleanvision.dataset.folder_dataset import FolderDataset
 from cleanvision.imagelab import Imagelab
 from cleanvision.issue_managers.image_property import BrightnessProperty
 from cleanvision.issue_managers.image_property_issue_manager import (
     compute_scores_wrapper,
 )
-from examples.custom_issue_manager import CustomIssueManager
+from docs.source.tutorials.custom_issue_manager import CustomIssueManager
 
 
 @pytest.mark.usefixtures("set_plt_show")
 def test_example1(capsys, generate_local_dataset):
     imagelab = Imagelab(data_path=generate_local_dataset)  # initialize imagelab
     imagelab.list_default_issue_types()  # list default checks
```

### Comparing `cleanvision-0.2.0/tests/test_utils.py` & `cleanvision-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.2.0/tests/test_viz_manager.py` & `cleanvision-0.2.1/tests/test_viz_manager.py`

 * *Files identical despite different names*

