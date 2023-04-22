# Comparing `tmp/jupyter-cache-0.6.0.tar.gz` & `tmp/jupyter-cache-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-cache-0.6.0.tar", last modified: Fri Apr 21 12:50:18 2023, max compression
+gzip compressed data, was "jupyter-cache-0.6.1.tar", last modified: Sat Apr 22 15:38:04 2023, max compression
```

## Comparing `jupyter-cache-0.6.0.tar` & `jupyter-cache-0.6.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      529 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2175 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1886 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/.gitignore
--rw-r--r--   0        0        0      821 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      193 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/.readthedocs.yml
--rw-r--r--   0        0        0     5581 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/LICENSE
--rw-r--r--   0        0        0     3552 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/README.md
--rw-r--r--   0        0        0      162 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/codecov.yml
--rw-r--r--   0        0        0      309 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/jupyter_cache/__init__.py
--rw-r--r--   0        0        0    11366 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/jupyter_cache/base.py
--rw-r--r--   0        0        0        0 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/jupyter_cache/cache/__init__.py
--rw-r--r--   0        0        0    15069 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/jupyter_cache/cache/db.py
--rw-r--r--   0        0        0    19736 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/jupyter_cache/cache/main.py
--rw-r--r--   0        0        0     1294 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/jupyter_cache/cli/__init__.py
--rw-r--r--   0        0        0     1188 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/jupyter_cache/cli/arguments.py
--rw-r--r--   0        0        0      182 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/cli/commands/__init__.py
--rw-r--r--   0        0        0     6373 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/cli/commands/cmd_cache.py
--rw-r--r--   0        0        0      392 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/cli/commands/cmd_main.py
--rw-r--r--   0        0        0     6516 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/cli/commands/cmd_notebook.py
--rw-r--r--   0        0        0     2539 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/cli/commands/cmd_project.py
--rw-r--r--   0        0        0     4301 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/cli/options.py
--rw-r--r--   0        0        0      530 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/cli/utils.py
--rw-r--r--   0        0        0     1466 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/entry_points.py
--rw-r--r--   0        0        0       87 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/executors/__init__.py
--rw-r--r--   0        0        0     3977 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/executors/base.py
--rw-r--r--   0        0        0     8363 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/executors/basic.py
--rw-r--r--   0        0        0     3649 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/executors/utils.py
--rw-r--r--   0        0        0     1286 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/readers.py
--rw-r--r--   0        0        0     3988 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/utils.py
--rw-r--r--   0        0        0     2773 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1205 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/tox.ini
--rw-r--r--   0        0        0     5805 1970-01-01 00:00:00.000000 jupyter-cache-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      529 2023-04-22 15:38:00.585209 jupyter-cache-0.6.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2175 2023-04-22 15:38:00.585209 jupyter-cache-0.6.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1886 2023-04-22 15:38:00.585209 jupyter-cache-0.6.1/.gitignore
+-rw-r--r--   0        0        0      821 2023-04-22 15:38:00.585209 jupyter-cache-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      193 2023-04-22 15:38:00.585209 jupyter-cache-0.6.1/.readthedocs.yml
+-rw-r--r--   0        0        0     5796 2023-04-22 15:38:00.585209 jupyter-cache-0.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-04-22 15:38:00.585209 jupyter-cache-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3552 2023-04-22 15:38:00.585209 jupyter-cache-0.6.1/README.md
+-rw-r--r--   0        0        0      162 2023-04-22 15:38:00.585209 jupyter-cache-0.6.1/codecov.yml
+-rw-r--r--   0        0        0      309 2023-04-22 15:38:00.585209 jupyter-cache-0.6.1/jupyter_cache/__init__.py
+-rw-r--r--   0        0        0    11366 2023-04-22 15:38:00.585209 jupyter-cache-0.6.1/jupyter_cache/base.py
+-rw-r--r--   0        0        0        0 2023-04-22 15:38:00.585209 jupyter-cache-0.6.1/jupyter_cache/cache/__init__.py
+-rw-r--r--   0        0        0    15231 2023-04-22 15:38:00.585209 jupyter-cache-0.6.1/jupyter_cache/cache/db.py
+-rw-r--r--   0        0        0    19736 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/cache/main.py
+-rw-r--r--   0        0        0     1294 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/cli/__init__.py
+-rw-r--r--   0        0        0     1188 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/cli/arguments.py
+-rw-r--r--   0        0        0      182 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6373 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/cli/commands/cmd_cache.py
+-rw-r--r--   0        0        0      392 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/cli/commands/cmd_main.py
+-rw-r--r--   0        0        0     6516 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/cli/commands/cmd_notebook.py
+-rw-r--r--   0        0        0     2539 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/cli/commands/cmd_project.py
+-rw-r--r--   0        0        0     4301 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/cli/options.py
+-rw-r--r--   0        0        0      530 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/cli/utils.py
+-rw-r--r--   0        0        0     1466 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/entry_points.py
+-rw-r--r--   0        0        0       87 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/executors/__init__.py
+-rw-r--r--   0        0        0     3977 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/executors/base.py
+-rw-r--r--   0        0        0     8363 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/executors/basic.py
+-rw-r--r--   0        0        0     3649 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/executors/utils.py
+-rw-r--r--   0        0        0     1286 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/readers.py
+-rw-r--r--   0        0        0     3988 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/jupyter_cache/utils.py
+-rw-r--r--   0        0        0     2773 2023-04-22 15:38:00.589209 jupyter-cache-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1205 2023-04-22 15:38:00.593209 jupyter-cache-0.6.1/tox.ini
+-rw-r--r--   0        0        0     5805 1970-01-01 00:00:00.000000 jupyter-cache-0.6.1/PKG-INFO
```

### Comparing `jupyter-cache-0.6.0/.github/dependabot.yml` & `jupyter-cache-0.6.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/.github/workflows/tests.yml` & `jupyter-cache-0.6.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/.gitignore` & `jupyter-cache-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/.pre-commit-config.yaml` & `jupyter-cache-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/CHANGELOG.md` & `jupyter-cache-0.6.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # CHANGELOG
 
+## v0.6.1 2023-04-22
+
+A patch release to fix compatibility with sqlalchemy <1.4.
+
+- FIX: compatibility with SQLAlchemy < 1.4.0 [#105](https://github.com/executablebooks/jupyter-cache/pull/105) @DimitriPapadopoulos
+
 ## v0.6.0 2023-04-21
 
 This is a minor release to improve our packaging infrastructure and to support several new versions of dependencies.
 
 ### Breaking changes
 
 - ‼️ BREAKING: Drop Python 3.7, add Python 3.11, unpin myst-nb in docs [#96](https://github.com/executablebooks/jupyter-cache/pull/96) ([@choldgraf](https://github.com/choldgraf))
```

### Comparing `jupyter-cache-0.6.0/LICENSE` & `jupyter-cache-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/README.md` & `jupyter-cache-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/jupyter_cache/base.py` & `jupyter-cache-0.6.1/jupyter_cache/base.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/jupyter_cache/cache/db.py` & `jupyter-cache-0.6.1/jupyter_cache/cache/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,21 @@
 import os
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 from sqlalchemy import JSON, Column, DateTime, Integer, String, Text
 from sqlalchemy.engine import Engine, create_engine
 from sqlalchemy.exc import IntegrityError, OperationalError
-from sqlalchemy.orm import declarative_base, sessionmaker, validates
+
+try:
+    from sqlalchemy.orm import declarative_base  # sqlalchemy >= 1.4.0
+except ImportError:
+    from sqlalchemy.ext.declarative import declarative_base  # sqlalchemy < 1.4.0
+
+from sqlalchemy.orm import sessionmaker, validates
 from sqlalchemy.sql.expression import desc
 
 from jupyter_cache import __version__
 from jupyter_cache.utils import shorten_path
 
 OrmBase = declarative_base()
 DB_NAME = "global.db"
```

### Comparing `jupyter-cache-0.6.0/jupyter_cache/cache/main.py` & `jupyter-cache-0.6.1/jupyter_cache/cache/main.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/jupyter_cache/cli/__init__.py` & `jupyter-cache-0.6.1/jupyter_cache/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/jupyter_cache/cli/arguments.py` & `jupyter-cache-0.6.1/jupyter_cache/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/jupyter_cache/cli/commands/cmd_cache.py` & `jupyter-cache-0.6.1/jupyter_cache/cli/commands/cmd_cache.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/jupyter_cache/cli/commands/cmd_notebook.py` & `jupyter-cache-0.6.1/jupyter_cache/cli/commands/cmd_notebook.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/jupyter_cache/cli/commands/cmd_project.py` & `jupyter-cache-0.6.1/jupyter_cache/cli/commands/cmd_project.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/jupyter_cache/cli/options.py` & `jupyter-cache-0.6.1/jupyter_cache/cli/options.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/jupyter_cache/cli/utils.py` & `jupyter-cache-0.6.1/jupyter_cache/cli/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/jupyter_cache/entry_points.py` & `jupyter-cache-0.6.1/jupyter_cache/entry_points.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/jupyter_cache/executors/base.py` & `jupyter-cache-0.6.1/jupyter_cache/executors/base.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/jupyter_cache/executors/basic.py` & `jupyter-cache-0.6.1/jupyter_cache/executors/basic.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/jupyter_cache/executors/utils.py` & `jupyter-cache-0.6.1/jupyter_cache/executors/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/jupyter_cache/readers.py` & `jupyter-cache-0.6.1/jupyter_cache/readers.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/jupyter_cache/utils.py` & `jupyter-cache-0.6.1/jupyter_cache/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/pyproject.toml` & `jupyter-cache-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/tox.ini` & `jupyter-cache-0.6.1/tox.ini`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.6.0/PKG-INFO` & `jupyter-cache-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-cache
-Version: 0.6.0
+Version: 0.6.1
 Summary: A defined interface for working with a cache of jupyter notebooks.
 Keywords: sphinx extension material design web components
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
```

