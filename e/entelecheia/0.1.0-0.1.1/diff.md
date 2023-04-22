# Comparing `tmp/entelecheia-0.1.0.tar.gz` & `tmp/entelecheia-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entelecheia-0.1.0.tar", max compression
+gzip compressed data, was "entelecheia-0.1.1.tar", max compression
```

## Comparing `entelecheia-0.1.0.tar` & `entelecheia-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1071 2023-04-22 00:30:25.983561 entelecheia-0.1.0/LICENSE
--rw-r--r--   0        0        0     1016 2023-04-22 00:30:25.983561 entelecheia-0.1.0/README.md
--rw-r--r--   0        0        0     3105 2023-04-22 00:30:53.528144 entelecheia-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      179 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/__cli__.py
--rw-r--r--   0        0        0      880 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/__init__.py
--rw-r--r--   0        0        0       22 2023-04-22 00:30:53.476143 entelecheia-0.1.0/src/entelecheia/_version.py
--rw-r--r--   0        0        0        0 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/conf/task/__init__.yaml
--rw-r--r--   0        0        0      312 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/project.toml
--rw-r--r--   0        0        0        0 2023-04-22 00:30:25.983561 entelecheia-0.1.0/src/entelecheia/py.typed
--rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 entelecheia-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-22 06:02:40.716920 entelecheia-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1016 2023-04-22 06:02:40.716920 entelecheia-0.1.1/README.md
+-rw-r--r--   0        0        0     3130 2023-04-22 06:03:09.186931 entelecheia-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      179 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/__cli__.py
+-rw-r--r--   0        0        0      822 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-22 06:03:09.122927 entelecheia-0.1.1/src/entelecheia/_version.py
+-rw-r--r--   0        0        0        0 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/__init__.py
+-rw-r--r--   0        0        0      321 2023-04-22 06:03:09.122927 entelecheia-0.1.1/src/entelecheia/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/task/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/py.typed
+-rw-r--r--   0        0        0     1707 1970-01-01 00:00:00.000000 entelecheia-0.1.1/PKG-INFO
```

### Comparing `entelecheia-0.1.0/LICENSE` & `entelecheia-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.0/README.md` & `entelecheia-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.0/pyproject.toml` & `entelecheia-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "entelecheia"
-version = "0.1.0"
+version = "0.1.1"
 description = "ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”)."
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.me"
 readme = "README.md"
 packages = [{ include = "entelecheia", from = "src" }]
 
 [tool.poetry.scripts]
 entelecheia = 'entelecheia.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.2.11"
-toml = "^0.10.2"
+hyfi = "^0.2.13"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 setuptools-scm = "^7.1.0"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
@@ -82,21 +81,21 @@
 write_to_template = '__version__ = "{version}"'
 tag_regex = '^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$'
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/entelecheia/_version.py:__version__"
+version_pattern = 'src/entelecheia/conf/about/__init__.yaml:version: "{version}"'
 version_source = "tag"
 commit_version_number = true # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
-pre_commit_command = "make scm-version"
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
 build_command = "poetry build --no-cache"
 hvcs = "github" # hosting version control system, gitlab is also supported
 
 [build-system]
```

### Comparing `entelecheia-0.1.0/src/entelecheia/conf/dotenv/__init__.yaml` & `entelecheia-0.1.1/src/entelecheia/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.0/src/entelecheia/conf/hydra/help/help.yaml` & `entelecheia-0.1.1/src/entelecheia/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.0/src/entelecheia/conf/mode/__init__.yaml` & `entelecheia-0.1.1/src/entelecheia/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.0/src/entelecheia/conf/path/__default__.yaml` & `entelecheia-0.1.1/src/entelecheia/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.0/src/entelecheia/conf/path/__init__.yaml` & `entelecheia-0.1.1/src/entelecheia/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.0/PKG-INFO` & `entelecheia-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: entelecheia
-Version: 0.1.0
+Version: 0.1.1
 Summary: ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”).
 Home-page: https://entelecheia.me
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.2.11,<0.3.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: hyfi (>=0.2.13,<0.3.0)
 Description-Content-Type: text/markdown
 
 # ἐντελέχεια 【en.te.lé.kʰeː.a】
 [![home-img]][home-url]
 [![course-img]][course-url]
 [![lecture-img]][lecture-url]
 [![research-img]][research-url]
```

