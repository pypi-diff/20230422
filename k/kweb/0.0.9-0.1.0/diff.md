# Comparing `tmp/kweb-0.0.9.tar.gz` & `tmp/kweb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kweb-0.0.9.tar", last modified: Sun Feb  5 01:59:50 2023, max compression
+gzip compressed data, was "kweb-0.1.0.tar", last modified: Sat Apr 22 14:01:28 2023, max compression
```

## Comparing `kweb-0.0.9.tar` & `kweb-0.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:59:50.181913 kweb-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-05 01:59:30.000000 kweb-0.0.9/.bumpversion.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:59:50.181913 kweb-0.0.9/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-05 01:59:30.000000 kweb-0.0.9/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-05 01:59:30.000000 kweb-0.0.9/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:59:50.181913 kweb-0.0.9/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-05 01:59:30.000000 kweb-0.0.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:59:50.181913 kweb-0.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-02-05 01:59:30.000000 kweb-0.0.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-02-05 01:59:30.000000 kweb-0.0.9/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-02-05 01:59:30.000000 kweb-0.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-02-05 01:59:30.000000 kweb-0.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-05 01:59:30.000000 kweb-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-05 01:59:30.000000 kweb-0.0.9/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-02-05 01:59:50.181913 kweb-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-02-05 01:59:30.000000 kweb-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:59:50.181913 kweb-0.0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-05 01:59:30.000000 kweb-0.0.9/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-05 01:59:30.000000 kweb-0.0.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-02-05 01:59:30.000000 kweb-0.0.9/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:59:50.177913 kweb-0.0.9/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:59:50.181913 kweb-0.0.9/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-02-05 01:59:30.000000 kweb-0.0.9/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-02-05 01:59:30.000000 kweb-0.0.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-05 01:59:30.000000 kweb-0.0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-02-05 01:59:30.000000 kweb-0.0.9/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-05 01:59:30.000000 kweb-0.0.9/docs/markdown.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-05 01:59:30.000000 kweb-0.0.9/docs/rst.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-02-05 01:59:30.000000 kweb-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-05 01:59:50.181913 kweb-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:59:50.177913 kweb-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:59:50.181913 kweb-0.0.9/src/kweb/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-05 01:59:30.000000 kweb-0.0.9/src/kweb/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-05 01:59:30.000000 kweb-0.0.9/src/kweb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:59:50.181913 kweb-0.0.9/src/kweb/gds_files/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-05 01:59:30.000000 kweb-0.0.9/src/kweb/gds_files/wg.gds
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-02-05 01:59:30.000000 kweb-0.0.9/src/kweb/main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6777 2023-02-05 01:59:30.000000 kweb-0.0.9/src/kweb/server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      580 2023-02-05 01:59:30.000000 kweb-0.0.9/src/kweb/server_jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:59:50.181913 kweb-0.0.9/src/kweb/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-02-05 01:59:30.000000 kweb-0.0.9/src/kweb/static/client.css
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-02-05 01:59:30.000000 kweb-0.0.9/src/kweb/static/client.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:59:50.181913 kweb-0.0.9/src/kweb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-02-05 01:59:30.000000 kweb-0.0.9/src/kweb/templates/client.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:59:50.181913 kweb-0.0.9/src/kweb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-02-05 01:59:50.000000 kweb-0.0.9/src/kweb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-05 01:59:50.000000 kweb-0.0.9/src/kweb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-05 01:59:50.000000 kweb-0.0.9/src/kweb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-05 01:59:50.000000 kweb-0.0.9/src/kweb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-05 01:59:50.000000 kweb-0.0.9/src/kweb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:59:50.181913 kweb-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-05 01:59:30.000000 kweb-0.0.9/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.666090 kweb-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-22 14:01:11.000000 kweb-0.1.0/.bumpversion.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.662090 kweb-0.1.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-22 14:01:11.000000 kweb-0.1.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-22 14:01:11.000000 kweb-0.1.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.662090 kweb-0.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-22 14:01:11.000000 kweb-0.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.662090 kweb-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-22 14:01:11.000000 kweb-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-22 14:01:11.000000 kweb-0.1.0/.github/workflows/test_code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-22 14:01:11.000000 kweb-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-22 14:01:11.000000 kweb-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-22 14:01:11.000000 kweb-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-22 14:01:11.000000 kweb-0.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-22 14:01:28.666090 kweb-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-22 14:01:11.000000 kweb-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.662090 kweb-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.658090 kweb-0.1.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.662090 kweb-0.1.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/markdown.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/rst.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-22 14:01:11.000000 kweb-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 14:01:28.666090 kweb-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.662090 kweb-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.662090 kweb-0.1.0/src/kweb/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.666090 kweb-0.1.0/src/kweb/gds_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/gds_files/wg.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7188 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1321 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/server_jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.666090 kweb-0.1.0/src/kweb/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/static/client.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/static/client.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.666090 kweb-0.1.0/src/kweb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/templates/client.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.666090 kweb-0.1.0/src/kweb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-22 14:01:28.000000 kweb-0.1.0/src/kweb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-22 14:01:28.000000 kweb-0.1.0/src/kweb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 14:01:28.000000 kweb-0.1.0/src/kweb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-22 14:01:28.000000 kweb-0.1.0/src/kweb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-22 14:01:28.000000 kweb-0.1.0/src/kweb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.666090 kweb-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-22 14:01:11.000000 kweb-0.1.0/tests/test_sample.py
```

### Comparing `kweb-0.0.9/.github/workflows/release.yml` & `kweb-0.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `kweb-0.0.9/.github/workflows/test_code.yml` & `kweb-0.1.0/.github/workflows/test_code.yml`

 * *Files identical despite different names*

### Comparing `kweb-0.0.9/.gitignore` & `kweb-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kweb-0.0.9/.pre-commit-config.yaml` & `kweb-0.1.0/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "5191f112dfd133e97acba8c2162c37d8613cf54b"
+    rev: "v4.4.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
@@ -12,65 +12,65 @@
       - id: mixed-line-ending
       - id: name-tests-test
         args: ["--pytest-test-first"]
       - id: requirements-txt-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/hakancelik96/unimport
-    rev: 33ead41ee30f1d323a9c2fcfd0114297efbbc4d5
+    rev: 0.14.1
     hooks:
       - id: unimport
         args: [--remove, --include-star-import]
   - repo: https://github.com/pycqa/isort
-    rev: "06d8ef58a15751eda085547cc2095a6dea098f3b"
+    rev: "5.12.0"
     hooks:
       - id: isort
         files: "kweb/.*"
         args: ["--profile", "black", "--filter-files"]
 
   - repo: https://github.com/psf/black
-    rev: "196b1f349eb2baa9bbbc483226874cc01fb7567d"
+    rev: "23.1.0"
     hooks:
       - id: black
 
   # - repo: https://github.com/pycqa/flake8
   #   rev: "647996c743f9e77368ce46cc74abe98549dd4c3a"
   #   hooks:
   #     - id: flake8
 
   - repo: https://github.com/kynan/nbstripout
-    rev: 1185a8d25bb45ada13f64d9591c14d81d69206bc
+    rev: 0.6.1
     hooks:
       - id: nbstripout
         files: ".ipynb"
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: 97ed6fb3cf2e650d4f762ba231c3f04c41797710
+    rev: v3.3.1
     hooks:
       - id: pyupgrade
         args: [--py310-plus, --keep-runtime-typing]
 
   # - repo: https://github.com/codespell-project/codespell
   #   rev: 3841ffe24aba604a5d16439c8216b018a7ec649a
   #   hooks:
   #     - id: codespell
   #       args: ["-L TE,TE/TM,te,ba,FPR,fpr_spacing,ro,donot"]
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: 953faa6870f6663ac0121ab4a800f1ce76bca31f
+    rev: v0.9.0.2
     hooks:
       - id: shellcheck
 
   # - repo: https://github.com/pre-commit/pygrep-hooks
   #   rev: 7b4409161486c6956bb3206ce96db5d56731b1b9 # Use the ref you want to point at
   #   hooks:
   #     - id: python-use-type-annotations
 
   - repo: https://github.com/PyCQA/bandit
-    rev: 91c4d979550888c8d190898279bfdb0af732791e
+    rev: 1.7.4
     hooks:
       - id: bandit
         args: [--exit-zero]
         # ignore all tests, not just tests data
         exclude: ^tests/
   # - repo: https://github.com/pre-commit/mirrors-mypy
   #   rev: "v0.991"
@@ -133,10 +133,10 @@
   #       additional_dependencies: [jupytext, black] # optional, only if you're using Jupytext
   #     - id: nbqa-pyupgrade
   #       args: ["--py37-plus"]
   #     # - id: nbqa-flake8
   #     # - id: nbqa-isort
   #     #   args: ["--float-to-top"]
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.231"
+    rev: "v0.0.253"
     hooks:
       - id: ruff
```

### Comparing `kweb-0.0.9/LICENSE` & `kweb-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kweb-0.0.9/PKG-INFO` & `kweb-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: kweb
-Version: 0.0.9
+Version: 0.1.0
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: docs
+Provides-Extra: ipy
 License-File: LICENSE
 
-# kweb 0.0.9
+# kweb 0.1.0
 
 KLayout Web Viewer ![demo](https://i.imgur.com/HPvePvX.png)
 
 Based on https://github.com/klayoutmatthias/canvas2canvas
 
 ## Run
```

### Comparing `kweb-0.0.9/docs/Makefile` & `kweb-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kweb-0.0.9/docs/conf.py` & `kweb-0.1.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project = "kweb"
-version = "0.0.9"
+version = "0.1.0"
 copyright = "2022"
 # copyright = "2020, gdsfactory"
 # author = "gdsfactory"
 
 # html_theme = "furo"
 # html_theme = "sphinx_rtd_theme"
 html_theme = "sphinx_book_theme"
```

### Comparing `kweb-0.0.9/docs/make.bat` & `kweb-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kweb-0.0.9/pyproject.toml` & `kweb-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	"Programming Language :: Python :: 3.7",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"Operating System :: OS Independent",
 ]
-version = "0.0.9"
+version = "0.1.0"
 authors = [
     {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 dependencies = [
   "klayout >= 0.28.3",
   "fastapi",
   "uvicorn[standard]",
@@ -39,14 +39,19 @@
     "sphinx-copybutton",
     "sphinx-markdown-tables==0.0.17",
     "myst-parser",
     "matplotlib",
     "nbsphinx",
     "autodoc_pydantic"
     ]
+ipy = [
+    "ipython",
+    "ipywidgets",
+    "ipyevents",
+]
 
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.black]
 line-length = 88  # Specify the line length
```

### Comparing `kweb-0.0.9/src/kweb/static/client.css` & `kweb-0.1.0/src/kweb/static/client.css`

 * *Files identical despite different names*

### Comparing `kweb-0.0.9/src/kweb/static/client.js` & `kweb-0.1.0/src/kweb/static/client.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,15 @@
 //  TODO: shouldn't be explicit here ..
 // let url = 'ws://localhost:8765/ws';
 
 ws_url = ws_url.replace("http://", "ws://");
 ws_url = ws_url.replace("https://", "wss://");
-let url = ws_url + '/ws';
+let url = ws_url + '/ws?' + "gds_file=" + gds_file + "&layer_props=" + layer_props;
 console.log(url);
+console.log(layer_props);
 
 var canvas = document.getElementById("layout_canvas");
 var context = canvas.getContext("2d");
 
 var message = document.getElementById("message");
 
 let socket = new WebSocket(url);
```

### Comparing `kweb-0.0.9/src/kweb.egg-info/PKG-INFO` & `kweb-0.1.0/src/kweb.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: kweb
-Version: 0.0.9
+Version: 0.1.0
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: docs
+Provides-Extra: ipy
 License-File: LICENSE
 
-# kweb 0.0.9
+# kweb 0.1.0
 
 KLayout Web Viewer ![demo](https://i.imgur.com/HPvePvX.png)
 
 Based on https://github.com/klayoutmatthias/canvas2canvas
 
 ## Run
```

### Comparing `kweb-0.0.9/src/kweb.egg-info/SOURCES.txt` & `kweb-0.1.0/src/kweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

