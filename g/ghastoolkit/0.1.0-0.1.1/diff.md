# Comparing `tmp/ghastoolkit-0.1.0.tar.gz` & `tmp/ghastoolkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.1.0.tar", last modified: Fri Apr 21 23:08:49 2023, max compression
+gzip compressed data, was "ghastoolkit-0.1.1.tar", last modified: Sat Apr 22 00:30:38 2023, max compression
```

## Comparing `ghastoolkit-0.1.0.tar` & `ghastoolkit-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxrwxr-x   0 geekmasher  (1000) geekmasher  (1000)        0 2023-04-21 23:08:49.531077 ghastoolkit-0.1.0/
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     1069 2023-04-21 21:33:13.000000 ghastoolkit-0.1.0/LICENSE
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)      540 2023-04-21 23:08:49.531077 ghastoolkit-0.1.0/PKG-INFO
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)       47 2023-04-21 13:48:52.000000 ghastoolkit-0.1.0/README.md
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)      567 2023-04-21 21:32:29.000000 ghastoolkit-0.1.0/pyproject.toml
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)       38 2023-04-21 23:08:49.531077 ghastoolkit-0.1.0/setup.cfg
-drwxrwxr-x   0 geekmasher  (1000) geekmasher  (1000)        0 2023-04-21 23:08:49.531077 ghastoolkit-0.1.0/src/
-drwxrwxr-x   0 geekmasher  (1000) geekmasher  (1000)        0 2023-04-21 23:08:49.531077 ghastoolkit-0.1.0/src/ghastoolkit/
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)      359 2023-04-21 19:18:54.000000 ghastoolkit-0.1.0/src/ghastoolkit/__init__.py
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     2380 2023-04-21 23:06:17.000000 ghastoolkit-0.1.0/src/ghastoolkit/__main__.py
-drwxrwxr-x   0 geekmasher  (1000) geekmasher  (1000)        0 2023-04-21 23:08:49.531077 ghastoolkit-0.1.0/src/ghastoolkit/codeql/
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)       96 2023-04-21 22:24:13.000000 ghastoolkit-0.1.0/src/ghastoolkit/codeql/__init__.py
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)      268 2023-04-21 16:23:49.000000 ghastoolkit-0.1.0/src/ghastoolkit/codeql/consts.py
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     6119 2023-04-21 22:08:21.000000 ghastoolkit-0.1.0/src/ghastoolkit/codeql/databases.py
-drwxrwxr-x   0 geekmasher  (1000) geekmasher  (1000)        0 2023-04-21 23:08:49.531077 ghastoolkit-0.1.0/src/ghastoolkit/octokit/
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)        1 2023-04-21 15:14:50.000000 ghastoolkit-0.1.0/src/ghastoolkit/octokit/__init__.py
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     2013 2023-04-21 20:48:15.000000 ghastoolkit-0.1.0/src/ghastoolkit/octokit/codescanning.py
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     2923 2023-04-21 22:24:13.000000 ghastoolkit-0.1.0/src/ghastoolkit/octokit/dependencygraph.py
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     2370 2023-04-21 19:14:05.000000 ghastoolkit-0.1.0/src/ghastoolkit/octokit/github.py
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     4314 2023-04-21 20:48:12.000000 ghastoolkit-0.1.0/src/ghastoolkit/octokit/octokit.py
-drwxrwxr-x   0 geekmasher  (1000) geekmasher  (1000)        0 2023-04-21 23:08:49.531077 ghastoolkit-0.1.0/src/ghastoolkit.egg-info/
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)      540 2023-04-21 23:08:49.000000 ghastoolkit-0.1.0/src/ghastoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)      581 2023-04-21 23:08:49.000000 ghastoolkit-0.1.0/src/ghastoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)        1 2023-04-21 23:08:49.000000 ghastoolkit-0.1.0/src/ghastoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)       12 2023-04-21 23:08:49.000000 ghastoolkit-0.1.0/src/ghastoolkit.egg-info/top_level.txt
-drwxrwxr-x   0 geekmasher  (1000) geekmasher  (1000)        0 2023-04-21 23:08:49.531077 ghastoolkit-0.1.0/tests/
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)      627 2023-04-21 22:26:33.000000 ghastoolkit-0.1.0/tests/test_codeqldb.py
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)      564 2023-04-21 22:24:13.000000 ghastoolkit-0.1.0/tests/test_octokit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/octokit/octokit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-22 00:30:38.000000 ghastoolkit-0.1.1/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-22 00:30:38.000000 ghastoolkit-0.1.1/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:30:38.000000 ghastoolkit-0.1.1/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-22 00:30:38.000000 ghastoolkit-0.1.1/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/tests/test_octokit.py
```

### Comparing `ghastoolkit-0.1.0/LICENSE` & `ghastoolkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.0/PKG-INFO` & `ghastoolkit-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMaher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMaher/ghastoolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ghastoolkit-0.1.0/pyproject.toml` & `ghastoolkit-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.1.0/src/ghastoolkit/__main__.py` & `ghastoolkit-0.1.1/src/ghastoolkit/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 import json
 import os
 import logging
 import argparse
 
 from ghastoolkit import __name__ as name
-from ghastoolkit.codeql import CodeQLDatabase
-from ghastoolkit.codeql.databases import CodeQLDatabaseList
-from ghastoolkit.octokit import dependencygraph
 from ghastoolkit.octokit.github import GitHub
 from ghastoolkit.octokit.codescanning import CodeScanning
 from ghastoolkit.octokit.dependencygraph import (
-    Dependencies,
     DependencyGraph,
-    Dependency,
 )
 
 # Arguments
 parser = argparse.ArgumentParser(name)
 parser.add_argument("--debug", action="store_true")
 
 parser.add_argument("mode", choices=["codescanning", "codeql", "dependencygraph"])
```

### Comparing `ghastoolkit-0.1.0/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.1.1/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.0/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.1.1/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.0/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.1.1/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.0/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.1.1/src/ghastoolkit/octokit/github.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,18 +23,21 @@
         if self.reference:
             return f"{self.owner}/{self.repo}@{self.reference}"
         return f"{self.owner}/{self.repo}"
 
     @staticmethod
     def parseRepository(name: str) -> "Repository":
         ref = None
+        branch = None
         if "@" in name:
-            name, ref = name.split("@", 1)
+            name, branch = name.split("@", 1)
+            ref = f"refs/heads/{branch}"
+
         owner, repo = name.split("/", 1)
-        return Repository(owner, repo, ref)
+        return Repository(owner, repo, reference=ref, branch=branch)
 
 
 class GitHub:
     repository: Optional[Repository] = None
     token: Optional[str] = None
 
     # URLs
```

### Comparing `ghastoolkit-0.1.0/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.1.1/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.0/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.1.1/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMaher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMaher/ghastoolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ghastoolkit-0.1.0/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.1.1/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,8 +12,10 @@
 src/ghastoolkit/codeql/databases.py
 src/ghastoolkit/octokit/__init__.py
 src/ghastoolkit/octokit/codescanning.py
 src/ghastoolkit/octokit/dependencygraph.py
 src/ghastoolkit/octokit/github.py
 src/ghastoolkit/octokit/octokit.py
 tests/test_codeqldb.py
+tests/test_depgraph.py
+tests/test_github.py
 tests/test_octokit.py
```

### Comparing `ghastoolkit-0.1.0/tests/test_codeqldb.py` & `ghastoolkit-0.1.1/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.0/tests/test_octokit.py` & `ghastoolkit-0.1.1/tests/test_octokit.py`

 * *Files identical despite different names*

