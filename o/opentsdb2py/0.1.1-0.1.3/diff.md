# Comparing `tmp/opentsdb2py-0.1.1.tar.gz` & `tmp/opentsdb2py-0.1.3.tar.gz`

## Comparing `opentsdb2py-0.1.1.tar` & `opentsdb2py-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/environment.yml
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/environment_complete.yml
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/.github/workflows/python-package-conda.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/.vscode/launch.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/src/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/src/opentsdb/__init__.py
--rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/src/opentsdb/client.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/src/opentsdb/query.py
--rw-r--r--   0        0        0     8748 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/src/opentsdb/request.py
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/src/opentsdb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/src/tests/__init__py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/src/tests/opentsdb_test.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/LICENSE
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/README.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 opentsdb2py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/environment.yml
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/environment_complete.yml
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/.github/workflows/python-package-conda.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/.vscode/launch.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/src/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/src/opentsdb2py/__init__.py
+-rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/src/opentsdb2py/client.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/src/opentsdb2py/query.py
+-rw-r--r--   0        0        0     8757 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/src/opentsdb2py/request.py
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/src/opentsdb2py/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/tests/__init__py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/tests/opentsdb_test.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/LICENSE
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/README.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 opentsdb2py-0.1.3/PKG-INFO
```

### Comparing `opentsdb2py-0.1.1/environment_complete.yml` & `opentsdb2py-0.1.3/environment_complete.yml`

 * *Files identical despite different names*

### Comparing `opentsdb2py-0.1.1/.github/workflows/python-package-conda.yml` & `opentsdb2py-0.1.3/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `opentsdb2py-0.1.1/.github/workflows/python-publish.yml` & `opentsdb2py-0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `opentsdb2py-0.1.1/.vscode/launch.json` & `opentsdb2py-0.1.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `opentsdb2py-0.1.1/src/opentsdb/client.py` & `opentsdb2py-0.1.3/src/opentsdb2py/client.py`

 * *Files identical despite different names*

### Comparing `opentsdb2py-0.1.1/src/opentsdb/query.py` & `opentsdb2py-0.1.3/src/opentsdb2py/query.py`

 * *Files identical despite different names*

### Comparing `opentsdb2py-0.1.1/src/opentsdb/request.py` & `opentsdb2py-0.1.3/src/opentsdb2py/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from opentsdb.client import Client
-from opentsdb.query import Filter, MetricQueryBuilder, QueryBuilder, TSUIDQueryBuilder
-from opentsdb.utils import Endpoints, Verbs, _builder
+from opentsdb2py.client import Client
+from opentsdb2py.query import Filter, MetricQueryBuilder, QueryBuilder, TSUIDQueryBuilder
+from opentsdb2py.utils import Endpoints, Verbs, _builder
 
 
 import requests
 
 
 import logging
 from typing import Any, List, Tuple
```

### Comparing `opentsdb2py-0.1.1/src/opentsdb/utils.py` & `opentsdb2py-0.1.3/src/opentsdb2py/utils.py`

 * *Files identical despite different names*

### Comparing `opentsdb2py-0.1.1/.gitignore` & `opentsdb2py-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `opentsdb2py-0.1.1/LICENSE` & `opentsdb2py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opentsdb2py-0.1.1/pyproject.toml` & `opentsdb2py-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "opentsdb2py"
-version = "0.1.1"
+version = "0.1.3"
 authors = [
   { name="Niels Westphal", email="opentsdbclient@nielswestphal.de" },
 ]
 description = "A simple OpenTSDB client for Python 3.11+. Warning: This is a work in progress and not ready for production use yet. Breaking changes will be introduced at a regular basis. Feel free to partiscipate in the development by issues or pull requests."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `opentsdb2py-0.1.1/PKG-INFO` & `opentsdb2py-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentsdb2py
-Version: 0.1.1
+Version: 0.1.3
 Summary: A simple OpenTSDB client for Python 3.11+. Warning: This is a work in progress and not ready for production use yet. Breaking changes will be introduced at a regular basis. Feel free to partiscipate in the development by issues or pull requests.
 Project-URL: Homepage, https://github.com/WNiels/OpenTSDBClient
 Project-URL: Bug Tracker, https://github.com/WNiels/OpenTSDBClient/issues
 Author-email: Niels Westphal <opentsdbclient@nielswestphal.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

