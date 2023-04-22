# Comparing `tmp/chinese_whispers-0.8.1rc1.tar.gz` & `tmp/chinese_whispers-0.8.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chinese_whispers-0.8.1rc1.tar", last modified: Sat Dec 10 00:18:23 2022, max compression
+gzip compressed data, was "chinese_whispers-0.8.2rc1.tar", last modified: Sat Apr 22 13:10:31 2023, max compression
```

## Comparing `chinese_whispers-0.8.1rc1.tar` & `chinese_whispers-0.8.2rc1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 00:18:23.340557 chinese_whispers-0.8.1rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2022-12-10 00:17:35.000000 chinese_whispers-0.8.1rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2022-12-10 00:18:23.340557 chinese_whispers-0.8.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2022-12-10 00:17:35.000000 chinese_whispers-0.8.1rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 00:18:23.340557 chinese_whispers-0.8.1rc1/chinese_whispers/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2022-12-10 00:17:35.000000 chinese_whispers-0.8.1rc1/chinese_whispers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1226 2022-12-10 00:17:35.000000 chinese_whispers-0.8.1rc1/chinese_whispers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2022-12-10 00:17:35.000000 chinese_whispers-0.8.1rc1/chinese_whispers/chinese_whispers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2022-12-10 00:17:35.000000 chinese_whispers-0.8.1rc1/chinese_whispers/test_chinese_whispers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 00:18:23.340557 chinese_whispers-0.8.1rc1/chinese_whispers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2022-12-10 00:18:23.000000 chinese_whispers-0.8.1rc1/chinese_whispers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2022-12-10 00:18:23.000000 chinese_whispers-0.8.1rc1/chinese_whispers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-10 00:18:23.000000 chinese_whispers-0.8.1rc1/chinese_whispers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-10 00:18:23.000000 chinese_whispers-0.8.1rc1/chinese_whispers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-10 00:18:23.000000 chinese_whispers-0.8.1rc1/chinese_whispers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-10 00:18:23.000000 chinese_whispers-0.8.1rc1/chinese_whispers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-10 00:17:44.000000 chinese_whispers-0.8.1rc1/chinese_whispers.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2022-12-10 00:17:35.000000 chinese_whispers-0.8.1rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-10 00:18:23.340557 chinese_whispers-0.8.1rc1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2022-12-10 00:17:35.000000 chinese_whispers-0.8.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:10:31.915820 chinese_whispers-0.8.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-22 13:09:37.000000 chinese_whispers-0.8.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-22 13:10:31.915820 chinese_whispers-0.8.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-22 13:09:37.000000 chinese_whispers-0.8.2rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:10:31.911820 chinese_whispers-0.8.2rc1/chinese_whispers/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-22 13:09:37.000000 chinese_whispers-0.8.2rc1/chinese_whispers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1226 2023-04-22 13:09:37.000000 chinese_whispers-0.8.2rc1/chinese_whispers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-22 13:09:37.000000 chinese_whispers-0.8.2rc1/chinese_whispers/chinese_whispers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-22 13:09:37.000000 chinese_whispers-0.8.2rc1/chinese_whispers/test_chinese_whispers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:10:31.915820 chinese_whispers-0.8.2rc1/chinese_whispers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-22 13:10:31.000000 chinese_whispers-0.8.2rc1/chinese_whispers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-22 13:10:31.000000 chinese_whispers-0.8.2rc1/chinese_whispers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 13:10:31.000000 chinese_whispers-0.8.2rc1/chinese_whispers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-22 13:10:31.000000 chinese_whispers-0.8.2rc1/chinese_whispers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-22 13:10:31.000000 chinese_whispers-0.8.2rc1/chinese_whispers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-22 13:10:31.000000 chinese_whispers-0.8.2rc1/chinese_whispers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 13:09:47.000000 chinese_whispers-0.8.2rc1/chinese_whispers.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-22 13:09:37.000000 chinese_whispers-0.8.2rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 13:10:31.915820 chinese_whispers-0.8.2rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-04-22 13:09:37.000000 chinese_whispers-0.8.2rc1/setup.py
```

### Comparing `chinese_whispers-0.8.1rc1/LICENSE` & `chinese_whispers-0.8.2rc1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018-2022 Dmitry Ustalov
+Copyright (c) 2018-2023 Dmitry Ustalov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `chinese_whispers-0.8.1rc1/PKG-INFO` & `chinese_whispers-0.8.2rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chinese_whispers
-Version: 0.8.1rc1
+Version: 0.8.2rc1
 Summary: An implementation of the Chinese Whispers clustering algorithm.
 Author: Dmitry Ustalov
 License: MIT
 Project-URL: Homepage, https://github.com/nlpub/chinese-whispers-python
 Keywords: graph clustering,unsupervised learning,chinese whispers,cluster analysis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,28 +12,31 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Typing :: Typed
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Chinese Whispers for Python
 
 This is an implementation of the [Chinese Whispers](https://doi.org/10.3115/1654758.1654774) clustering algorithm in Python. Since this library is based on [NetworkX](https://networkx.github.io/), it is simple to use.
 
-[![Unit Tests][github_tests_badge]][github_tests_link] [![Read the Docs][rtfd_badge]][rtfd_link] [![PyPI Version][pypi_badge]][pypi_link]
+[![Unit Tests][github_tests_badge]][github_tests_link] [![Read the Docs][rtfd_badge]][rtfd_link] [![PyPI Version][pypi_badge]][pypi_link] [![Conda Version][conda_badge]][conda_link]
 
 [github_tests_badge]: https://github.com/nlpub/chinese-whispers-python/workflows/Unit%20Tests/badge.svg?branch=master
 [github_tests_link]: https://github.com/nlpub/chinese-whispers-python/actions?query=workflow%3A%22Unit+Tests%22
 [rtfd_badge]: https://readthedocs.org/projects/chinese-whispers/badge/
 [rtfd_link]: https://chinese-whispers.readthedocs.io/
 [pypi_badge]: https://badge.fury.io/py/chinese-whispers.svg
 [pypi_link]: https://pypi.python.org/pypi/chinese-whispers
+[conda_badge]: https://img.shields.io/conda/vn/conda-forge/chinese-whispers.svg
+[conda_link]: https://anaconda.org/conda-forge/chinese-whispers
 
 Given a NetworkX graph `G`, this library can [cluster](https://en.wikipedia.org/wiki/Cluster_analysis) it using the following code:
 
 ```python
 from chinese_whispers import chinese_whispers
 chinese_whispers(G, weighting='top', iterations=20)
 ```
@@ -75,8 +78,8 @@
   issn      = {0891-2017},
   language  = {english},
 }
 ```
 
 ## Copyright
 
-Copyright (c) 2018&ndash;2022 [Dmitry Ustalov](https://github.com/dustalov). See [LICENSE](LICENSE) for details.
+Copyright (c) 2018&ndash;2023 [Dmitry Ustalov](https://github.com/dustalov). See [LICENSE](LICENSE) for details.
```

### Comparing `chinese_whispers-0.8.1rc1/README.md` & `chinese_whispers-0.8.2rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # Chinese Whispers for Python
 
 This is an implementation of the [Chinese Whispers](https://doi.org/10.3115/1654758.1654774) clustering algorithm in Python. Since this library is based on [NetworkX](https://networkx.github.io/), it is simple to use.
 
-[![Unit Tests][github_tests_badge]][github_tests_link] [![Read the Docs][rtfd_badge]][rtfd_link] [![PyPI Version][pypi_badge]][pypi_link]
+[![Unit Tests][github_tests_badge]][github_tests_link] [![Read the Docs][rtfd_badge]][rtfd_link] [![PyPI Version][pypi_badge]][pypi_link] [![Conda Version][conda_badge]][conda_link]
 
 [github_tests_badge]: https://github.com/nlpub/chinese-whispers-python/workflows/Unit%20Tests/badge.svg?branch=master
 [github_tests_link]: https://github.com/nlpub/chinese-whispers-python/actions?query=workflow%3A%22Unit+Tests%22
 [rtfd_badge]: https://readthedocs.org/projects/chinese-whispers/badge/
 [rtfd_link]: https://chinese-whispers.readthedocs.io/
 [pypi_badge]: https://badge.fury.io/py/chinese-whispers.svg
 [pypi_link]: https://pypi.python.org/pypi/chinese-whispers
+[conda_badge]: https://img.shields.io/conda/vn/conda-forge/chinese-whispers.svg
+[conda_link]: https://anaconda.org/conda-forge/chinese-whispers
 
 Given a NetworkX graph `G`, this library can [cluster](https://en.wikipedia.org/wiki/Cluster_analysis) it using the following code:
 
 ```python
 from chinese_whispers import chinese_whispers
 chinese_whispers(G, weighting='top', iterations=20)
 ```
@@ -55,8 +57,8 @@
   issn      = {0891-2017},
   language  = {english},
 }
 ```
 
 ## Copyright
 
-Copyright (c) 2018&ndash;2022 [Dmitry Ustalov](https://github.com/dustalov). See [LICENSE](LICENSE) for details.
+Copyright (c) 2018&ndash;2023 [Dmitry Ustalov](https://github.com/dustalov). See [LICENSE](LICENSE) for details.
```

### Comparing `chinese_whispers-0.8.1rc1/chinese_whispers/__init__.py` & `chinese_whispers-0.8.2rc1/chinese_whispers/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.8.1rc1'
+__version__ = '0.8.2.pre1'
 __author__ = 'Dmitry Ustalov'
 __credits__ = ['Alexander Panchenko', 'Alexander Chambers', 'Frederik Wille']
 __license__ = 'MIT'
 
 from .chinese_whispers import (
     WEIGHTING,
     top_weighting,
```

### Comparing `chinese_whispers-0.8.1rc1/chinese_whispers/__main__.py` & `chinese_whispers-0.8.2rc1/chinese_whispers/__main__.py`

 * *Files identical despite different names*

### Comparing `chinese_whispers-0.8.1rc1/chinese_whispers/chinese_whispers.py` & `chinese_whispers-0.8.2rc1/chinese_whispers/chinese_whispers.py`

 * *Files identical despite different names*

### Comparing `chinese_whispers-0.8.1rc1/chinese_whispers/test_chinese_whispers.py` & `chinese_whispers-0.8.2rc1/chinese_whispers/test_chinese_whispers.py`

 * *Files identical despite different names*

### Comparing `chinese_whispers-0.8.1rc1/chinese_whispers.egg-info/PKG-INFO` & `chinese_whispers-0.8.2rc1/chinese_whispers.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chinese-whispers
-Version: 0.8.1rc1
+Version: 0.8.2rc1
 Summary: An implementation of the Chinese Whispers clustering algorithm.
 Author: Dmitry Ustalov
 License: MIT
 Project-URL: Homepage, https://github.com/nlpub/chinese-whispers-python
 Keywords: graph clustering,unsupervised learning,chinese whispers,cluster analysis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,28 +12,31 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Typing :: Typed
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Chinese Whispers for Python
 
 This is an implementation of the [Chinese Whispers](https://doi.org/10.3115/1654758.1654774) clustering algorithm in Python. Since this library is based on [NetworkX](https://networkx.github.io/), it is simple to use.
 
-[![Unit Tests][github_tests_badge]][github_tests_link] [![Read the Docs][rtfd_badge]][rtfd_link] [![PyPI Version][pypi_badge]][pypi_link]
+[![Unit Tests][github_tests_badge]][github_tests_link] [![Read the Docs][rtfd_badge]][rtfd_link] [![PyPI Version][pypi_badge]][pypi_link] [![Conda Version][conda_badge]][conda_link]
 
 [github_tests_badge]: https://github.com/nlpub/chinese-whispers-python/workflows/Unit%20Tests/badge.svg?branch=master
 [github_tests_link]: https://github.com/nlpub/chinese-whispers-python/actions?query=workflow%3A%22Unit+Tests%22
 [rtfd_badge]: https://readthedocs.org/projects/chinese-whispers/badge/
 [rtfd_link]: https://chinese-whispers.readthedocs.io/
 [pypi_badge]: https://badge.fury.io/py/chinese-whispers.svg
 [pypi_link]: https://pypi.python.org/pypi/chinese-whispers
+[conda_badge]: https://img.shields.io/conda/vn/conda-forge/chinese-whispers.svg
+[conda_link]: https://anaconda.org/conda-forge/chinese-whispers
 
 Given a NetworkX graph `G`, this library can [cluster](https://en.wikipedia.org/wiki/Cluster_analysis) it using the following code:
 
 ```python
 from chinese_whispers import chinese_whispers
 chinese_whispers(G, weighting='top', iterations=20)
 ```
@@ -75,8 +78,8 @@
   issn      = {0891-2017},
   language  = {english},
 }
 ```
 
 ## Copyright
 
-Copyright (c) 2018&ndash;2022 [Dmitry Ustalov](https://github.com/dustalov). See [LICENSE](LICENSE) for details.
+Copyright (c) 2018&ndash;2023 [Dmitry Ustalov](https://github.com/dustalov). See [LICENSE](LICENSE) for details.
```

### Comparing `chinese_whispers-0.8.1rc1/pyproject.toml` & `chinese_whispers-0.8.2rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,27 @@
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Typing :: Typed",
 ]
 license = {text = "MIT"}
 description = "An implementation of the Chinese Whispers clustering algorithm."
 keywords = ["graph clustering", "unsupervised learning", "chinese whispers", "cluster analysis"]
 requires-python = "~=3.7"
-dependencies = ["networkx >= 2.1,<3.0"]
+dependencies = ["networkx >= 2.1,< 4.0"]
 dynamic = ["version"]
 
+[project.optional-dependencies]
+dev = [
+    "mypy",
+    "notebook",
+    "matplotlib",
+    "flake8",
+    "twine",
+    "build"
+]
+
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
 Homepage = "https://github.com/nlpub/chinese-whispers-python"
```

