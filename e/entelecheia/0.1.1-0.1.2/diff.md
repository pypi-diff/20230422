# Comparing `tmp/entelecheia-0.1.1.tar.gz` & `tmp/entelecheia-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entelecheia-0.1.1.tar", max compression
+gzip compressed data, was "entelecheia-0.1.2.tar", max compression
```

## Comparing `entelecheia-0.1.1.tar` & `entelecheia-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1071 2023-04-22 06:02:40.716920 entelecheia-0.1.1/LICENSE
--rw-r--r--   0        0        0     1016 2023-04-22 06:02:40.716920 entelecheia-0.1.1/README.md
--rw-r--r--   0        0        0     3130 2023-04-22 06:03:09.186931 entelecheia-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      179 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/__cli__.py
--rw-r--r--   0        0        0      822 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/__init__.py
--rw-r--r--   0        0        0       22 2023-04-22 06:03:09.122927 entelecheia-0.1.1/src/entelecheia/_version.py
--rw-r--r--   0        0        0        0 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/__init__.py
--rw-r--r--   0        0        0      321 2023-04-22 06:03:09.122927 entelecheia-0.1.1/src/entelecheia/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/conf/task/__init__.yaml
--rw-r--r--   0        0        0        0 2023-04-22 06:02:40.716920 entelecheia-0.1.1/src/entelecheia/py.typed
--rw-r--r--   0        0        0     1707 1970-01-01 00:00:00.000000 entelecheia-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-22 06:08:17.011046 entelecheia-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1016 2023-04-22 06:08:17.011046 entelecheia-0.1.2/README.md
+-rw-r--r--   0        0        0     3130 2023-04-22 06:08:51.544231 entelecheia-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      179 2023-04-22 06:08:17.011046 entelecheia-0.1.2/src/entelecheia/__cli__.py
+-rw-r--r--   0        0        0      820 2023-04-22 06:08:17.011046 entelecheia-0.1.2/src/entelecheia/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-22 06:08:51.480229 entelecheia-0.1.2/src/entelecheia/_version.py
+-rw-r--r--   0        0        0        0 2023-04-22 06:08:17.011046 entelecheia-0.1.2/src/entelecheia/conf/__init__.py
+-rw-r--r--   0        0        0      321 2023-04-22 06:08:51.480229 entelecheia-0.1.2/src/entelecheia/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-22 06:08:17.011046 entelecheia-0.1.2/src/entelecheia/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-22 06:08:17.011046 entelecheia-0.1.2/src/entelecheia/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-22 06:08:17.011046 entelecheia-0.1.2/src/entelecheia/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-22 06:08:17.011046 entelecheia-0.1.2/src/entelecheia/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-22 06:08:17.015046 entelecheia-0.1.2/src/entelecheia/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-22 06:08:17.015046 entelecheia-0.1.2/src/entelecheia/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-22 06:08:17.015046 entelecheia-0.1.2/src/entelecheia/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-22 06:08:17.015046 entelecheia-0.1.2/src/entelecheia/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-22 06:08:17.015046 entelecheia-0.1.2/src/entelecheia/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-22 06:08:17.015046 entelecheia-0.1.2/src/entelecheia/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-22 06:08:17.015046 entelecheia-0.1.2/src/entelecheia/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-22 06:08:17.015046 entelecheia-0.1.2/src/entelecheia/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-22 06:08:17.015046 entelecheia-0.1.2/src/entelecheia/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-04-22 06:08:17.015046 entelecheia-0.1.2/src/entelecheia/conf/task/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-04-22 06:08:17.015046 entelecheia-0.1.2/src/entelecheia/py.typed
+-rw-r--r--   0        0        0     1707 1970-01-01 00:00:00.000000 entelecheia-0.1.2/PKG-INFO
```

### Comparing `entelecheia-0.1.1/LICENSE` & `entelecheia-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.1/README.md` & `entelecheia-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.1/pyproject.toml` & `entelecheia-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "entelecheia"
-version = "0.1.1"
+version = "0.1.2"
 description = "ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”)."
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.me"
 readme = "README.md"
 packages = [{ include = "entelecheia", from = "src" }]
```

### Comparing `entelecheia-0.1.1/src/entelecheia/__init__.py` & `entelecheia-0.1.2/src/entelecheia/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 # Extract package information
 about.name = about_data.get("name", "package name")
 about.authors = about_data.get("authors", ["Author name"])
 about.description = about_data.get("description", "package description")
 about.homepage = about_data.get("homepage", "https://package.homepage")
 about.license = about_data.get("license", "MIT")
 about.version = __version__
-global_config.hyfi_package_config_path = "pkg://hyfi_template.conf"
+global_config.hyfi_package_config_path = "pkg://entelecheia.conf"
 
 
 def get_version() -> str:
     """This is the cli function of the package"""
     return __version__
```

### Comparing `entelecheia-0.1.1/src/entelecheia/conf/dotenv/__init__.yaml` & `entelecheia-0.1.2/src/entelecheia/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.1/src/entelecheia/conf/hydra/help/help.yaml` & `entelecheia-0.1.2/src/entelecheia/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.1/src/entelecheia/conf/mode/__init__.yaml` & `entelecheia-0.1.2/src/entelecheia/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.1/src/entelecheia/conf/path/__default__.yaml` & `entelecheia-0.1.2/src/entelecheia/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.1/src/entelecheia/conf/path/__init__.yaml` & `entelecheia-0.1.2/src/entelecheia/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.1/PKG-INFO` & `entelecheia-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entelecheia
-Version: 0.1.1
+Version: 0.1.2
 Summary: ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”).
 Home-page: https://entelecheia.me
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

