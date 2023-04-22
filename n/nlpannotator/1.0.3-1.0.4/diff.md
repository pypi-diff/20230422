# Comparing `tmp/nlpannotator-1.0.3.tar.gz` & `tmp/nlpannotator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpannotator-1.0.3.tar", last modified: Tue Nov 15 13:02:28 2022, max compression
+gzip compressed data, was "nlpannotator-1.0.4.tar", last modified: Sat Apr 22 11:38:14 2023, max compression
```

## Comparing `nlpannotator-1.0.3.tar` & `nlpannotator-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 iulusoy   (1001) iulusoy   (1001)        0 2022-11-15 13:02:28.371317 nlpannotator-1.0.3/
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)     1060 2022-11-14 09:53:40.000000 nlpannotator-1.0.3/LICENSE
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)     7480 2022-11-15 13:02:28.371317 nlpannotator-1.0.3/PKG-INFO
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)     7064 2022-11-15 12:34:49.000000 nlpannotator-1.0.3/README.md
-drwxrwxr-x   0 iulusoy   (1001) iulusoy   (1001)        0 2022-11-15 13:02:28.371317 nlpannotator-1.0.3/nlpannotator/
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)      191 2022-11-14 09:53:40.000000 nlpannotator-1.0.3/nlpannotator/__init__.py
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)    21124 2022-11-14 09:53:40.000000 nlpannotator-1.0.3/nlpannotator/base.py
-drwxrwxr-x   0 iulusoy   (1001) iulusoy   (1001)        0 2022-11-15 13:02:28.371317 nlpannotator-1.0.3/nlpannotator/data/
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)     1230 2022-11-14 09:53:40.000000 nlpannotator-1.0.3/nlpannotator/data/attribute_names.json
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)     2154 2022-11-14 09:53:40.000000 nlpannotator-1.0.3/nlpannotator/data/input.json
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)    13687 2022-11-14 09:53:40.000000 nlpannotator-1.0.3/nlpannotator/data/input_schema.json
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)     7414 2022-11-15 12:34:49.000000 nlpannotator-1.0.3/nlpannotator/main.py
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)     2671 2022-11-15 10:14:27.000000 nlpannotator-1.0.3/nlpannotator/mflair.py
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)     2701 2022-11-14 09:53:40.000000 nlpannotator-1.0.3/nlpannotator/msomajo.py
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)     5474 2022-11-14 09:53:40.000000 nlpannotator-1.0.3/nlpannotator/mspacy.py
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)     5734 2022-11-14 09:53:40.000000 nlpannotator-1.0.3/nlpannotator/mstanza.py
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)     2536 2022-11-14 09:53:40.000000 nlpannotator-1.0.3/nlpannotator/mtreetagger.py
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)    12379 2022-11-14 09:53:40.000000 nlpannotator-1.0.3/nlpannotator/pipe.py
-drwxrwxr-x   0 iulusoy   (1001) iulusoy   (1001)        0 2022-11-15 13:02:28.371317 nlpannotator-1.0.3/nlpannotator.egg-info/
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)     7480 2022-11-15 13:02:28.000000 nlpannotator-1.0.3/nlpannotator.egg-info/PKG-INFO
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)      573 2022-11-15 13:02:28.000000 nlpannotator-1.0.3/nlpannotator.egg-info/SOURCES.txt
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)        1 2022-11-15 13:02:28.000000 nlpannotator-1.0.3/nlpannotator.egg-info/dependency_links.txt
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)       59 2022-11-15 13:02:28.000000 nlpannotator-1.0.3/nlpannotator.egg-info/entry_points.txt
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)       99 2022-11-15 13:02:28.000000 nlpannotator-1.0.3/nlpannotator.egg-info/requires.txt
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)       13 2022-11-15 13:02:28.000000 nlpannotator-1.0.3/nlpannotator.egg-info/top_level.txt
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)      937 2022-11-15 12:34:49.000000 nlpannotator-1.0.3/pyproject.toml
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)       38 2022-11-15 13:02:28.371317 nlpannotator-1.0.3/setup.cfg
--rw-rw-r--   0 iulusoy   (1001) iulusoy   (1001)       69 2022-11-14 09:53:40.000000 nlpannotator-1.0.3/setup.py
+drwxrwxr-x   0 inga      (1001) inga      (1001)        0 2023-04-22 11:38:14.462515 nlpannotator-1.0.4/
+-rw-rw-r--   0 inga      (1001) inga      (1001)     1060 2021-09-15 09:10:48.000000 nlpannotator-1.0.4/LICENSE
+-rw-rw-r--   0 inga      (1001) inga      (1001)     7504 2023-04-22 11:38:14.462515 nlpannotator-1.0.4/PKG-INFO
+-rw-rw-r--   0 inga      (1001) inga      (1001)     7088 2023-04-21 12:28:41.000000 nlpannotator-1.0.4/README.md
+drwxrwxr-x   0 inga      (1001) inga      (1001)        0 2023-04-22 11:38:14.458516 nlpannotator-1.0.4/nlpannotator/
+-rw-rw-r--   0 inga      (1001) inga      (1001)      191 2022-07-08 09:57:21.000000 nlpannotator-1.0.4/nlpannotator/__init__.py
+-rw-rw-r--   0 inga      (1001) inga      (1001)    21124 2022-09-02 18:43:35.000000 nlpannotator-1.0.4/nlpannotator/base.py
+drwxrwxr-x   0 inga      (1001) inga      (1001)        0 2023-04-22 11:38:14.462515 nlpannotator-1.0.4/nlpannotator/data/
+-rw-rw-r--   0 inga      (1001) inga      (1001)     1230 2022-07-08 09:57:21.000000 nlpannotator-1.0.4/nlpannotator/data/attribute_names.json
+-rw-rw-r--   0 inga      (1001) inga      (1001)     2154 2022-09-02 18:43:35.000000 nlpannotator-1.0.4/nlpannotator/data/input.json
+-rw-rw-r--   0 inga      (1001) inga      (1001)    13687 2022-09-02 18:43:35.000000 nlpannotator-1.0.4/nlpannotator/data/input_schema.json
+-rw-rw-r--   0 inga      (1001) inga      (1001)     7414 2022-11-18 19:17:27.000000 nlpannotator-1.0.4/nlpannotator/main.py
+-rw-rw-r--   0 inga      (1001) inga      (1001)     2671 2022-07-08 09:57:21.000000 nlpannotator-1.0.4/nlpannotator/mflair.py
+-rw-rw-r--   0 inga      (1001) inga      (1001)     2701 2022-07-08 09:57:21.000000 nlpannotator-1.0.4/nlpannotator/msomajo.py
+-rw-rw-r--   0 inga      (1001) inga      (1001)     5891 2023-04-21 13:12:47.000000 nlpannotator-1.0.4/nlpannotator/mspacy.py
+-rw-rw-r--   0 inga      (1001) inga      (1001)     5734 2022-07-08 09:57:21.000000 nlpannotator-1.0.4/nlpannotator/mstanza.py
+-rw-rw-r--   0 inga      (1001) inga      (1001)     2536 2022-07-08 09:57:21.000000 nlpannotator-1.0.4/nlpannotator/mtreetagger.py
+-rw-rw-r--   0 inga      (1001) inga      (1001)    12379 2022-07-08 09:57:21.000000 nlpannotator-1.0.4/nlpannotator/pipe.py
+drwxrwxr-x   0 inga      (1001) inga      (1001)        0 2023-04-22 11:38:14.462515 nlpannotator-1.0.4/nlpannotator.egg-info/
+-rw-rw-r--   0 inga      (1001) inga      (1001)     7504 2023-04-22 11:38:14.000000 nlpannotator-1.0.4/nlpannotator.egg-info/PKG-INFO
+-rw-rw-r--   0 inga      (1001) inga      (1001)      573 2023-04-22 11:38:14.000000 nlpannotator-1.0.4/nlpannotator.egg-info/SOURCES.txt
+-rw-rw-r--   0 inga      (1001) inga      (1001)        1 2023-04-22 11:38:14.000000 nlpannotator-1.0.4/nlpannotator.egg-info/dependency_links.txt
+-rw-rw-r--   0 inga      (1001) inga      (1001)       59 2023-04-22 11:38:14.000000 nlpannotator-1.0.4/nlpannotator.egg-info/entry_points.txt
+-rw-rw-r--   0 inga      (1001) inga      (1001)      107 2023-04-22 11:38:14.000000 nlpannotator-1.0.4/nlpannotator.egg-info/requires.txt
+-rw-rw-r--   0 inga      (1001) inga      (1001)       13 2023-04-22 11:38:14.000000 nlpannotator-1.0.4/nlpannotator.egg-info/top_level.txt
+-rw-rw-r--   0 inga      (1001) inga      (1001)      946 2023-04-22 11:37:56.000000 nlpannotator-1.0.4/pyproject.toml
+-rw-rw-r--   0 inga      (1001) inga      (1001)       38 2023-04-22 11:38:14.462515 nlpannotator-1.0.4/setup.cfg
+-rw-rw-r--   0 inga      (1001) inga      (1001)       69 2023-04-22 11:36:16.000000 nlpannotator-1.0.4/setup.py
```

### Comparing `nlpannotator-1.0.3/LICENSE` & `nlpannotator-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nlpannotator-1.0.3/PKG-INFO` & `nlpannotator-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nlpannotator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Annotator combining different NLP pipelines
 Maintainer-email: Inga Ulusoy <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Automated annotation of natural languages using selected toolchains
 
 ![Version](https://img.shields.io/pypi/v/nlpannotator)
 ![License: MIT](https://img.shields.io/github/license/ssciwr/argumentation-management)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/ssciwr/argumentation-management/CI)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ssciwr/argumentation-management/ci.yml?branch=main)
 ![codecov](https://img.shields.io/codecov/c/github/ssciwr/argumentation-management)
 ![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=ssciwr_argumentation-management&metric=alert_status)
 ![Language](https://img.shields.io/github/languages/top/ssciwr/argumentation-management)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/6698/badge)](https://bestpractices.coreinfrastructure.org/projects/6698)
 
 *This project just had its first version release and is still under development.*
```

### Comparing `nlpannotator-1.0.3/README.md` & `nlpannotator-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Automated annotation of natural languages using selected toolchains
 
 ![Version](https://img.shields.io/pypi/v/nlpannotator)
 ![License: MIT](https://img.shields.io/github/license/ssciwr/argumentation-management)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/ssciwr/argumentation-management/CI)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ssciwr/argumentation-management/ci.yml?branch=main)
 ![codecov](https://img.shields.io/codecov/c/github/ssciwr/argumentation-management)
 ![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=ssciwr_argumentation-management&metric=alert_status)
 ![Language](https://img.shields.io/github/languages/top/ssciwr/argumentation-management)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/6698/badge)](https://bestpractices.coreinfrastructure.org/projects/6698)
 
 *This project just had its first version release and is still under development.*
```

### Comparing `nlpannotator-1.0.3/nlpannotator/base.py` & `nlpannotator-1.0.4/nlpannotator/base.py`

 * *Files identical despite different names*

### Comparing `nlpannotator-1.0.3/nlpannotator/data/attribute_names.json` & `nlpannotator-1.0.4/nlpannotator/data/attribute_names.json`

 * *Files identical despite different names*

### Comparing `nlpannotator-1.0.3/nlpannotator/data/input.json` & `nlpannotator-1.0.4/nlpannotator/data/input.json`

 * *Files identical despite different names*

### Comparing `nlpannotator-1.0.3/nlpannotator/data/input_schema.json` & `nlpannotator-1.0.4/nlpannotator/data/input_schema.json`

 * *Files identical despite different names*

### Comparing `nlpannotator-1.0.3/nlpannotator/main.py` & `nlpannotator-1.0.4/nlpannotator/main.py`

 * *Files identical despite different names*

### Comparing `nlpannotator-1.0.3/nlpannotator/mflair.py` & `nlpannotator-1.0.4/nlpannotator/mflair.py`

 * *Files identical despite different names*

### Comparing `nlpannotator-1.0.3/nlpannotator/msomajo.py` & `nlpannotator-1.0.4/nlpannotator/msomajo.py`

 * *Files identical despite different names*

### Comparing `nlpannotator-1.0.3/nlpannotator/mspacy.py` & `nlpannotator-1.0.4/nlpannotator/mspacy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import spacy as sp
 import nlpannotator.base as be
+import warnings
 
 
 class MySpacy:
     """Base class for spaCy module.
 
     Args:
         subdict[dict]: Dict containing the setup for the spaCy run.
@@ -24,17 +25,25 @@
         self._load_pipe()
 
     def _load_pipe(self):
         try:
             self.nlp = sp.load(self.model, config=self.config)
 
         except OSError:
-            raise OSError("Could not find {} in standard directory.".format(self.model))
-
-        print(">>>")
+            warnings.warn("Could not find {} in standard directory.".format(self.model))
+            warnings.warn("Attempting to download the model...")
+            try:
+                sp.cli.download(self.model)
+                self.nlp = sp.load(self.model, config=self.config)
+            except SystemExit:
+                raise ValueError(
+                    "Could not download model {} - please check your model name!".format(
+                        self.model
+                    )
+                )
 
         # find which processors are available in model
         components = [component[0] for component in self.nlp.components]
 
         # go through the requested processors
         for component in self.jobs:
             # check if the keywords requested correspond to available components in pipeline
```

### Comparing `nlpannotator-1.0.3/nlpannotator/mstanza.py` & `nlpannotator-1.0.4/nlpannotator/mstanza.py`

 * *Files identical despite different names*

### Comparing `nlpannotator-1.0.3/nlpannotator/mtreetagger.py` & `nlpannotator-1.0.4/nlpannotator/mtreetagger.py`

 * *Files identical despite different names*

### Comparing `nlpannotator-1.0.3/nlpannotator/pipe.py` & `nlpannotator-1.0.4/nlpannotator/pipe.py`

 * *Files identical despite different names*

### Comparing `nlpannotator-1.0.3/nlpannotator.egg-info/PKG-INFO` & `nlpannotator-1.0.4/nlpannotator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nlpannotator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Annotator combining different NLP pipelines
 Maintainer-email: Inga Ulusoy <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Automated annotation of natural languages using selected toolchains
 
 ![Version](https://img.shields.io/pypi/v/nlpannotator)
 ![License: MIT](https://img.shields.io/github/license/ssciwr/argumentation-management)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/ssciwr/argumentation-management/CI)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ssciwr/argumentation-management/ci.yml?branch=main)
 ![codecov](https://img.shields.io/codecov/c/github/ssciwr/argumentation-management)
 ![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=ssciwr_argumentation-management&metric=alert_status)
 ![Language](https://img.shields.io/github/languages/top/ssciwr/argumentation-management)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/6698/badge)](https://bestpractices.coreinfrastructure.org/projects/6698)
 
 *This project just had its first version release and is still under development.*
```

### Comparing `nlpannotator-1.0.3/nlpannotator.egg-info/SOURCES.txt` & `nlpannotator-1.0.4/nlpannotator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlpannotator-1.0.3/pyproject.toml` & `nlpannotator-1.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 requires = [
     "setuptools>=61",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nlpannotator"
-version = "1.0.3"
+version = "1.0.4"
 description = "Annotator combining different NLP pipelines"
 readme = "README.md"
 maintainers = [
     { name = "Inga Ulusoy", email = "ssc@iwr.uni-heidelberg.de" },
 ]
 requires-python = ">=3.7, <4"
 license = { text = "MIT" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
     "spacy <3.5.0, >=3.4.0",
-    "stanza",
-    "flair",
-    "SoMaJo >=2.0",
+    "stanza <=1.4.0",
+    "flair <=0.11",
+    "SoMaJo",
     "treetaggerwrapper",
     "jsonschema",
     "importlib-resources >=5.8",
 ]
 
 [tool.setuptools.package-data]
-# Include any *.jsno files found in the "data" subdirectory of "nlpannotator"
+# Include any *.json files found in the "data" subdirectory of "nlpannotator"
 "nlpannotator.data" = ["*.json"]
 
 [project.scripts]
 nlpannotator_run = "nlpannotator.main:run"
 
 [tool.setuptools]
 packages = ["nlpannotator"]
```

