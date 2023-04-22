# Comparing `tmp/intecomm-eligibility-0.1.4.tar.gz` & `tmp/intecomm-eligibility-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intecomm-eligibility-0.1.4.tar", last modified: Fri Mar 31 01:26:00 2023, max compression
+gzip compressed data, was "intecomm-eligibility-0.1.5.tar", last modified: Sat Apr 22 18:15:04 2023, max compression
```

## Comparing `intecomm-eligibility-0.1.4.tar` & `intecomm-eligibility-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:26:00.136171 intecomm-eligibility-0.1.4/
--rw-r--r--   0 erikvw     (501) staff       (20)       64 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.4/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.4/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:26:00.129552 intecomm-eligibility-0.1.4/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:26:00.132614 intecomm-eligibility-0.1.4/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1652 2023-03-31 01:25:52.000000 intecomm-eligibility-0.1.4/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-29 06:14:51.000000 intecomm-eligibility-0.1.4/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-03-31 01:25:52.000000 intecomm-eligibility-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.4/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)      243 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.4/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       29 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.4/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-17 17:46:50.000000 intecomm-eligibility-0.1.4/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.4/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1773 2023-03-31 01:26:00.136260 intecomm-eligibility-0.1.4/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      905 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.4/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.4/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:26:00.134621 intecomm-eligibility-0.1.4/intecomm_eligibility/
--rw-r--r--   0 erikvw     (501) staff       (20)       46 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.4/intecomm_eligibility/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.4/intecomm_eligibility/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7349 2023-01-25 03:01:05.000000 intecomm-eligibility-0.1.4/intecomm_eligibility/eligibility.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:26:00.135819 intecomm-eligibility-0.1.4/intecomm_eligibility/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.4/intecomm_eligibility/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17256 2022-11-29 06:14:51.000000 intecomm-eligibility-0.1.4/intecomm_eligibility/tests/test_eligibility.py
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.4/intecomm_eligibility/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 01:26:00.135539 intecomm-eligibility-0.1.4/intecomm_eligibility.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1773 2023-03-31 01:26:00.000000 intecomm-eligibility-0.1.4/intecomm_eligibility.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      626 2023-03-31 01:26:00.000000 intecomm-eligibility-0.1.4/intecomm_eligibility.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-03-31 01:26:00.000000 intecomm-eligibility-0.1.4/intecomm_eligibility.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-17 23:17:15.000000 intecomm-eligibility-0.1.4/intecomm_eligibility.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       21 2023-03-31 01:26:00.000000 intecomm-eligibility-0.1.4/intecomm_eligibility.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1707 2023-03-31 01:25:52.000000 intecomm-eligibility-0.1.4/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     3245 2022-11-30 02:57:08.000000 intecomm-eligibility-0.1.4/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-03-31 01:26:00.136556 intecomm-eligibility-0.1.4/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:15:04.884570 intecomm-eligibility-0.1.5/
+-rw-r--r--   0 erikvw     (501) staff       (20)       64 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.5/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.5/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:15:04.879145 intecomm-eligibility-0.1.5/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:15:04.882378 intecomm-eligibility-0.1.5/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1652 2023-03-31 01:25:52.000000 intecomm-eligibility-0.1.5/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-29 06:14:51.000000 intecomm-eligibility-0.1.5/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-04-22 18:14:57.000000 intecomm-eligibility-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.5/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)      243 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.5/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       29 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.5/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-17 17:46:50.000000 intecomm-eligibility-0.1.5/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.5/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1773 2023-04-22 18:15:04.884650 intecomm-eligibility-0.1.5/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      905 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.5/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.5/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:15:04.883202 intecomm-eligibility-0.1.5/intecomm_eligibility/
+-rw-r--r--   0 erikvw     (501) staff       (20)       46 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.5/intecomm_eligibility/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.5/intecomm_eligibility/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7349 2023-01-25 03:01:05.000000 intecomm-eligibility-0.1.5/intecomm_eligibility/eligibility.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:15:04.884162 intecomm-eligibility-0.1.5/intecomm_eligibility/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.5/intecomm_eligibility/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17256 2022-11-29 06:14:51.000000 intecomm-eligibility-0.1.5/intecomm_eligibility/tests/test_eligibility.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-17 23:17:07.000000 intecomm-eligibility-0.1.5/intecomm_eligibility/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:15:04.883939 intecomm-eligibility-0.1.5/intecomm_eligibility.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1773 2023-04-22 18:15:04.000000 intecomm-eligibility-0.1.5/intecomm_eligibility.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      626 2023-04-22 18:15:04.000000 intecomm-eligibility-0.1.5/intecomm_eligibility.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-04-22 18:15:04.000000 intecomm-eligibility-0.1.5/intecomm_eligibility.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-17 23:17:15.000000 intecomm-eligibility-0.1.5/intecomm_eligibility.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       21 2023-04-22 18:15:04.000000 intecomm-eligibility-0.1.5/intecomm_eligibility.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1707 2023-03-31 01:25:52.000000 intecomm-eligibility-0.1.5/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     3245 2022-11-30 02:57:08.000000 intecomm-eligibility-0.1.5/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-04-22 18:15:04.884957 intecomm-eligibility-0.1.5/setup.cfg
```

### Comparing `intecomm-eligibility-0.1.4/.github/workflows/build.yml` & `intecomm-eligibility-0.1.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `intecomm-eligibility-0.1.4/.gitignore` & `intecomm-eligibility-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `intecomm-eligibility-0.1.4/.pre-commit-config.yaml` & `intecomm-eligibility-0.1.5/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ---
 exclude: tests/etc/user-*
 
 repos:
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3.10
 
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
@@ -37,13 +37,18 @@
       - id: fix-byte-order-marker
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
+  - repo: https://github.com/rstcheck/rstcheck
+    rev: v6.1.2
+    hooks:
+      - id: rstcheck
+
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.29.0
+    rev: v1.30.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `intecomm-eligibility-0.1.4/LICENSE` & `intecomm-eligibility-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `intecomm-eligibility-0.1.4/PKG-INFO` & `intecomm-eligibility-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-eligibility
-Version: 0.1.4
+Version: 0.1.5
 Summary: INTECOMM EDC eligibility
 Home-page: https://github.com/intecomm-trial/intecomm-eligibility
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC eligibility,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `intecomm-eligibility-0.1.4/README.rst` & `intecomm-eligibility-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `intecomm-eligibility-0.1.4/intecomm_eligibility/eligibility.py` & `intecomm-eligibility-0.1.5/intecomm_eligibility/eligibility.py`

 * *Files identical despite different names*

### Comparing `intecomm-eligibility-0.1.4/intecomm_eligibility/tests/test_eligibility.py` & `intecomm-eligibility-0.1.5/intecomm_eligibility/tests/test_eligibility.py`

 * *Files identical despite different names*

### Comparing `intecomm-eligibility-0.1.4/intecomm_eligibility.egg-info/PKG-INFO` & `intecomm-eligibility-0.1.5/intecomm_eligibility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-eligibility
-Version: 0.1.4
+Version: 0.1.5
 Summary: INTECOMM EDC eligibility
 Home-page: https://github.com/intecomm-trial/intecomm-eligibility
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC eligibility,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `intecomm-eligibility-0.1.4/intecomm_eligibility.egg-info/SOURCES.txt` & `intecomm-eligibility-0.1.5/intecomm_eligibility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intecomm-eligibility-0.1.4/pyproject.toml` & `intecomm-eligibility-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `intecomm-eligibility-0.1.4/runtests.py` & `intecomm-eligibility-0.1.5/runtests.py`

 * *Files identical despite different names*

### Comparing `intecomm-eligibility-0.1.4/setup.cfg` & `intecomm-eligibility-0.1.5/setup.cfg`

 * *Files identical despite different names*

