# Comparing `tmp/spiel-0.5.0.tar.gz` & `tmp/spiel-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiel-0.5.0.tar", max compression
+gzip compressed data, was "spiel-0.5.1.tar", max compression
```

## Comparing `spiel-0.5.0.tar` & `spiel-0.5.1.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0     1068 2023-02-20 04:36:34.434005 spiel-0.5.0/LICENSE
--rw-r--r--   0        0        0     2631 2023-02-20 04:36:34.434005 spiel-0.5.0/README.md
--rw-r--r--   0        0        0     2405 2023-02-20 04:36:34.438005 spiel-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      437 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/__init__.py
--rw-r--r--   0        0        0       33 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/__main__.py
--rw-r--r--   0        0        0     9461 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/app.py
--rw-r--r--   0        0        0     3455 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/cli.py
--rw-r--r--   0        0        0      548 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/constants.py
--rw-r--r--   0        0        0     3081 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/deck.py
--rw-r--r--   0        0        0        0 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/demo/__init__.py
--rw-r--r--   0        0        0    15522 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/demo/demo.py
--rw-r--r--   0        0        0    54727 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/demo/tree.jpg
--rw-r--r--   0        0        0      125 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/py.typed
--rw-r--r--   0        0        0        0 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/renderables/__init__.py
--rw-r--r--   0        0        0     1337 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/renderables/debug.py
--rw-r--r--   0        0        0     2706 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/renderables/image.py
--rw-r--r--   0        0        0        0 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/screens/__init__.py
--rw-r--r--   0        0        0      776 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/screens/deck.py
--rw-r--r--   0        0        0     1080 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/screens/help.py
--rw-r--r--   0        0        0      171 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/screens/screen.py
--rw-r--r--   0        0        0     1101 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/screens/slide.py
--rw-r--r--   0        0        0     2156 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/screens/transition.py
--rw-r--r--   0        0        0     1656 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/slide.py
--rw-r--r--   0        0        0        0 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/spiel.css
--rw-r--r--   0        0        0        0 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/transitions/__init__.py
--rw-r--r--   0        0        0     2490 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/transitions/protocol.py
--rw-r--r--   0        0        0     1126 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/transitions/swipe.py
--rw-r--r--   0        0        0     3320 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/triggers.py
--rw-r--r--   0        0        0      712 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/utils.py
--rw-r--r--   0        0        0        0 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/widgets/__init__.py
--rw-r--r--   0        0        0     1681 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/widgets/bindings.py
--rw-r--r--   0        0        0     1642 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/widgets/fixed_slide.py
--rw-r--r--   0        0        0     1668 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/widgets/footer.py
--rw-r--r--   0        0        0     2511 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/widgets/minislides.py
--rw-r--r--   0        0        0     1949 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/widgets/slide.py
--rw-r--r--   0        0        0      592 2023-02-20 04:36:34.438005 spiel-0.5.0/spiel/widgets/widget.py
--rw-r--r--   0        0        0     3685 1970-01-01 00:00:00.000000 spiel-0.5.0/setup.py
--rw-r--r--   0        0        0     4145 1970-01-01 00:00:00.000000 spiel-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-21 23:53:12.065111 spiel-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2631 2023-04-21 23:53:12.065111 spiel-0.5.1/README.md
+-rw-r--r--   0        0        0     2405 2023-04-21 23:53:12.069111 spiel-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      437 2023-04-21 23:53:12.069111 spiel-0.5.1/spiel/__init__.py
+-rw-r--r--   0        0        0       33 2023-04-21 23:53:12.069111 spiel-0.5.1/spiel/__main__.py
+-rw-r--r--   0        0        0     9461 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/app.py
+-rw-r--r--   0        0        0     3455 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/cli.py
+-rw-r--r--   0        0        0      548 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/constants.py
+-rw-r--r--   0        0        0     3081 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/deck.py
+-rw-r--r--   0        0        0        0 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/demo/__init__.py
+-rw-r--r--   0        0        0    15522 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/demo/demo.py
+-rw-r--r--   0        0        0    54727 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/demo/tree.jpg
+-rw-r--r--   0        0        0      125 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/py.typed
+-rw-r--r--   0        0        0        0 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/renderables/__init__.py
+-rw-r--r--   0        0        0     1337 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/renderables/debug.py
+-rw-r--r--   0        0        0     2706 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/renderables/image.py
+-rw-r--r--   0        0        0        0 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/screens/__init__.py
+-rw-r--r--   0        0        0      776 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/screens/deck.py
+-rw-r--r--   0        0        0     1080 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/screens/help.py
+-rw-r--r--   0        0        0      171 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/screens/screen.py
+-rw-r--r--   0        0        0     1101 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/screens/slide.py
+-rw-r--r--   0        0        0     2156 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/screens/transition.py
+-rw-r--r--   0        0        0     1656 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/slide.py
+-rw-r--r--   0        0        0        0 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/spiel.css
+-rw-r--r--   0        0        0        0 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/transitions/__init__.py
+-rw-r--r--   0        0        0     2490 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/transitions/protocol.py
+-rw-r--r--   0        0        0     1126 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/transitions/swipe.py
+-rw-r--r--   0        0        0     3320 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/triggers.py
+-rw-r--r--   0        0        0      712 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/widgets/__init__.py
+-rw-r--r--   0        0        0     1681 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/widgets/bindings.py
+-rw-r--r--   0        0        0     1642 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/widgets/fixed_slide.py
+-rw-r--r--   0        0        0     1668 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/widgets/footer.py
+-rw-r--r--   0        0        0     2511 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/widgets/minislides.py
+-rw-r--r--   0        0        0     1949 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/widgets/slide.py
+-rw-r--r--   0        0        0      592 2023-04-21 23:53:12.073111 spiel-0.5.1/spiel/widgets/widget.py
+-rw-r--r--   0        0        0     4145 1970-01-01 00:00:00.000000 spiel-0.5.1/PKG-INFO
```

### Comparing `spiel-0.5.0/LICENSE` & `spiel-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/README.md` & `spiel-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/pyproject.toml` & `spiel-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "spiel"
-version = "0.5.0"
+version = "0.5.1"
 description = "A framework for building and presenting richly-styled presentations in your terminal using Python."
 readme="README.md"
 homepage="https://github.com/JoshKarpel/spiel"
 repository="https://github.com/JoshKarpel/spiel"
 documentation="https://www.spiel.how"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -38,15 +38,15 @@
 include = ["py.typed", "demo/*", "spiel.css"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 rich = ">=13.2"
 typer = ">=0.6"
 pillow = ">=8"
-textual = ">=0.11.0"
+textual = "==0.11.1"
 watchfiles = ">=0.18"
 more-itertools = ">=9"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=3"
 pytest = ">=7"
 pytest-cov = ">=3"
@@ -54,15 +54,15 @@
 pytest-asyncio = ">=0.20"
 pytest-mock = ">=3"
 hypothesis = ">=6"
 mypy = ">=1"
 mkdocs = ">=1.4"
 mkdocs-material = ">=9"
 mkdocstrings = {extras = ["python"], version = ">=0.19.0"}
-textual = {extras = ["dev"], version = ">=0.11.0"}
+textual = {extras = ["dev"], version = "==0.11.1"}
 
 [tool.poetry.scripts]
 spiel = 'spiel.cli:cli'
 
 [tool.black]
 line-length = 100
 include = "\\.pyi?$"
```

### Comparing `spiel-0.5.0/spiel/app.py` & `spiel-0.5.1/spiel/app.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/cli.py` & `spiel-0.5.1/spiel/cli.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/constants.py` & `spiel-0.5.1/spiel/constants.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/deck.py` & `spiel-0.5.1/spiel/deck.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/demo/demo.py` & `spiel-0.5.1/spiel/demo/demo.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/demo/tree.jpg` & `spiel-0.5.1/spiel/demo/tree.jpg`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/renderables/debug.py` & `spiel-0.5.1/spiel/renderables/debug.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/renderables/image.py` & `spiel-0.5.1/spiel/renderables/image.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/screens/deck.py` & `spiel-0.5.1/spiel/screens/deck.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/screens/help.py` & `spiel-0.5.1/spiel/screens/help.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/screens/slide.py` & `spiel-0.5.1/spiel/screens/slide.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/screens/transition.py` & `spiel-0.5.1/spiel/screens/transition.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/slide.py` & `spiel-0.5.1/spiel/slide.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/transitions/protocol.py` & `spiel-0.5.1/spiel/transitions/protocol.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/transitions/swipe.py` & `spiel-0.5.1/spiel/transitions/swipe.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/triggers.py` & `spiel-0.5.1/spiel/triggers.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/utils.py` & `spiel-0.5.1/spiel/utils.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/widgets/bindings.py` & `spiel-0.5.1/spiel/widgets/bindings.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/widgets/fixed_slide.py` & `spiel-0.5.1/spiel/widgets/fixed_slide.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/widgets/footer.py` & `spiel-0.5.1/spiel/widgets/footer.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/widgets/minislides.py` & `spiel-0.5.1/spiel/widgets/minislides.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/widgets/slide.py` & `spiel-0.5.1/spiel/widgets/slide.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/spiel/widgets/widget.py` & `spiel-0.5.1/spiel/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `spiel-0.5.0/setup.py` & `spiel-0.5.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,105 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: spiel
+Version: 0.5.1
+Summary: A framework for building and presenting richly-styled presentations in your terminal using Python.
+Home-page: https://github.com/JoshKarpel/spiel
+License: MIT
+Keywords: presentation,slides,tui,terminal
+Author: JoshKarpel
+Author-email: josh.karpel@gmail.com
+Requires-Python: >=3.10,<4
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Artistic Software
+Classifier: Topic :: Multimedia :: Graphics :: Presentation
+Classifier: Typing :: Typed
+Requires-Dist: more-itertools (>=9)
+Requires-Dist: pillow (>=8)
+Requires-Dist: rich (>=13.2)
+Requires-Dist: textual (==0.11.1)
+Requires-Dist: typer (>=0.6)
+Requires-Dist: watchfiles (>=0.18)
+Project-URL: Documentation, https://www.spiel.how
+Project-URL: Repository, https://github.com/JoshKarpel/spiel
+Description-Content-Type: text/markdown
+
+# Spiel
+
+[![PyPI](https://img.shields.io/pypi/v/spiel)](https://pypi.org/project/spiel)
+[![PyPI - License](https://img.shields.io/pypi/l/spiel)](https://pypi.org/project/spiel)
+[![Docs](https://img.shields.io/badge/docs-exist-brightgreen)](https://www.spiel.how)
+
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/JoshKarpel/spiel/main.svg)](https://results.pre-commit.ci/latest/github/JoshKarpel/spiel/main)
+[![codecov](https://codecov.io/gh/JoshKarpel/spiel/branch/main/graph/badge.svg?token=2sjP4V0AfY)](https://codecov.io/gh/JoshKarpel/spiel)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+[![GitHub issues](https://img.shields.io/github/issues/JoshKarpel/spiel)](https://github.com/JoshKarpel/spiel/issues)
+[![GitHub pull requests](https://img.shields.io/github/issues-pr/JoshKarpel/spiel)](https://github.com/JoshKarpel/spiel/pulls)
+
+[Spiel](https://dictionary.cambridge.org/us/dictionary/english/spiel) is a framework for building and presenting
+[richly-styled](https://github.com/Textualize/rich) presentations in your terminal using Python.
+
+To see what Spiel can do without installing it, you can view the demonstration deck in a container:
+```bash
+$ docker run -it --rm ghcr.io/joshkarpel/spiel
+```
+Alternatively, install Spiel (`pip install spiel`) and run this command to view the demonstration deck:
+```bash
+$ spiel demo present
+```
+
+![The first slide of the demo deck](https://raw.githubusercontent.com/JoshKarpel/spiel/main/docs/assets/demo.svg)
+![The demo deck in "deck view"](https://raw.githubusercontent.com/JoshKarpel/spiel/main/docs/assets/deck.svg)
+
+## Quick Start
+
+If you want to jump right in,
+install Spiel (`pip install spiel`),
+create a file called `deck.py`,
+and copy this code into it:
+```python
+from rich.console import RenderableType
+
+from spiel import Deck, present
+
+deck = Deck(name="Your Deck Name")
+
+
+@deck.slide(title="Slide 1 Title")
+def slide_1() -> RenderableType:
+    return "Your content here!"
+
+
+if __name__ == "__main__":
+    present(__file__)
+```
+
+That is the most basic Spiel presentation you can make.
+To present the deck, run `python deck.py`.
+You should see:
+
+![Barebones slide](https://raw.githubusercontent.com/JoshKarpel/spiel/main/docs/assets/quickstart_basic.svg)
+
+Check out the [Quick Start tutorial](https://www.spiel.how/quickstart) to continue!
 
-packages = \
-['spiel',
- 'spiel.demo',
- 'spiel.renderables',
- 'spiel.screens',
- 'spiel.transitions',
- 'spiel.widgets']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['more-itertools>=9',
- 'pillow>=8',
- 'rich>=13.2',
- 'textual>=0.11.0',
- 'typer>=0.6',
- 'watchfiles>=0.18']
-
-entry_points = \
-{'console_scripts': ['spiel = spiel.cli:cli']}
-
-setup_kwargs = {
-    'name': 'spiel',
-    'version': '0.5.0',
-    'description': 'A framework for building and presenting richly-styled presentations in your terminal using Python.',
-    'long_description': '# Spiel\n\n[![PyPI](https://img.shields.io/pypi/v/spiel)](https://pypi.org/project/spiel)\n[![PyPI - License](https://img.shields.io/pypi/l/spiel)](https://pypi.org/project/spiel)\n[![Docs](https://img.shields.io/badge/docs-exist-brightgreen)](https://www.spiel.how)\n\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/JoshKarpel/spiel/main.svg)](https://results.pre-commit.ci/latest/github/JoshKarpel/spiel/main)\n[![codecov](https://codecov.io/gh/JoshKarpel/spiel/branch/main/graph/badge.svg?token=2sjP4V0AfY)](https://codecov.io/gh/JoshKarpel/spiel)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n[![GitHub issues](https://img.shields.io/github/issues/JoshKarpel/spiel)](https://github.com/JoshKarpel/spiel/issues)\n[![GitHub pull requests](https://img.shields.io/github/issues-pr/JoshKarpel/spiel)](https://github.com/JoshKarpel/spiel/pulls)\n\n[Spiel](https://dictionary.cambridge.org/us/dictionary/english/spiel) is a framework for building and presenting\n[richly-styled](https://github.com/Textualize/rich) presentations in your terminal using Python.\n\nTo see what Spiel can do without installing it, you can view the demonstration deck in a container:\n```bash\n$ docker run -it --rm ghcr.io/joshkarpel/spiel\n```\nAlternatively, install Spiel (`pip install spiel`) and run this command to view the demonstration deck:\n```bash\n$ spiel demo present\n```\n\n![The first slide of the demo deck](https://raw.githubusercontent.com/JoshKarpel/spiel/main/docs/assets/demo.svg)\n![The demo deck in "deck view"](https://raw.githubusercontent.com/JoshKarpel/spiel/main/docs/assets/deck.svg)\n\n## Quick Start\n\nIf you want to jump right in,\ninstall Spiel (`pip install spiel`),\ncreate a file called `deck.py`,\nand copy this code into it:\n```python\nfrom rich.console import RenderableType\n\nfrom spiel import Deck, present\n\ndeck = Deck(name="Your Deck Name")\n\n\n@deck.slide(title="Slide 1 Title")\ndef slide_1() -> RenderableType:\n    return "Your content here!"\n\n\nif __name__ == "__main__":\n    present(__file__)\n```\n\nThat is the most basic Spiel presentation you can make.\nTo present the deck, run `python deck.py`.\nYou should see:\n\n![Barebones slide](https://raw.githubusercontent.com/JoshKarpel/spiel/main/docs/assets/quickstart_basic.svg)\n\nCheck out the [Quick Start tutorial](https://www.spiel.how/quickstart) to continue!\n\n## Documentation\n\nTo learn more about Spiel, take a look at the [documentation](https://www.spiel.how).\n\n## Contributing\n\nIf you\'re interested in contributing to Spiel, check out the [Contributing Guide](https://www.spiel.how/contributing/).\n',
-    'author': 'JoshKarpel',
-    'author_email': 'josh.karpel@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/JoshKarpel/spiel',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4',
-}
+## Documentation
 
+To learn more about Spiel, take a look at the [documentation](https://www.spiel.how).
+
+## Contributing
+
+If you're interested in contributing to Spiel, check out the [Contributing Guide](https://www.spiel.how/contributing/).
 
-setup(**setup_kwargs)
```

