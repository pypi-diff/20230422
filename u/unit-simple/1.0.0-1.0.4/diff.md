# Comparing `tmp/unit_simple-1.0.0.tar.gz` & `tmp/unit_simple-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unit_simple-1.0.0.tar", last modified: Thu Apr 20 22:43:12 2023, max compression
+gzip compressed data, was "unit_simple-1.0.4.tar", last modified: Sat Apr 22 15:05:19 2023, max compression
```

## Comparing `unit_simple-1.0.0.tar` & `unit_simple-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2023-04-20 22:43:12.720753 unit_simple-1.0.0/
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     2780 2023-04-20 22:43:12.720753 unit_simple-1.0.0/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     2404 2023-04-20 21:06:08.000000 unit_simple-1.0.0/README.md
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      531 2023-04-20 22:43:04.000000 unit_simple-1.0.0/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       38 2023-04-20 22:43:12.720753 unit_simple-1.0.0/setup.cfg
-drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2023-04-20 22:43:12.720753 unit_simple-1.0.0/unit_simple.egg-info/
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     2780 2023-04-20 22:43:12.000000 unit_simple-1.0.0/unit_simple.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      179 2023-04-20 22:43:12.000000 unit_simple-1.0.0/unit_simple.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)        1 2023-04-20 22:43:12.000000 unit_simple-1.0.0/unit_simple.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       12 2023-04-20 22:43:12.000000 unit_simple-1.0.0/unit_simple.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     6115 2023-03-31 20:37:02.000000 unit_simple-1.0.0/unit_simple.py
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2023-04-22 15:05:19.328425 unit_simple-1.0.4/
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     2820 2023-04-22 15:05:19.328425 unit_simple-1.0.4/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     2404 2023-04-20 21:06:08.000000 unit_simple-1.0.4/README.md
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      571 2023-04-22 15:05:11.000000 unit_simple-1.0.4/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       38 2023-04-22 15:05:19.328425 unit_simple-1.0.4/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       69 2023-04-22 13:04:43.000000 unit_simple-1.0.4/setup.py
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2023-04-22 15:05:19.328425 unit_simple-1.0.4/unit_simple.egg-info/
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     2820 2023-04-22 15:05:19.000000 unit_simple-1.0.4/unit_simple.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      188 2023-04-22 15:05:19.000000 unit_simple-1.0.4/unit_simple.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)        1 2023-04-22 15:05:19.000000 unit_simple-1.0.4/unit_simple.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       12 2023-04-22 15:05:19.000000 unit_simple-1.0.4/unit_simple.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     6115 2023-03-31 20:37:02.000000 unit_simple-1.0.4/unit_simple.py
```

### Comparing `unit_simple-1.0.0/PKG-INFO` & `unit_simple-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: unit_simple
-Version: 1.0.0
-Summary: A small example package
+Version: 1.0.4
+Summary: A simple measurement unit API to handle basic unit conversions.
 Author-email: Samuel Andrés <samuel.andres@yahoo.fr>
 Project-URL: Homepage, https://github.com/SamuelAndresPascal/cosmoloj-py
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `unit_simple-1.0.0/README.md` & `unit_simple-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `unit_simple-1.0.0/unit_simple.egg-info/PKG-INFO` & `unit_simple-1.0.4/unit_simple.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: unit-simple
-Version: 1.0.0
-Summary: A small example package
+Version: 1.0.4
+Summary: A simple measurement unit API to handle basic unit conversions.
 Author-email: Samuel Andrés <samuel.andres@yahoo.fr>
 Project-URL: Homepage, https://github.com/SamuelAndresPascal/cosmoloj-py
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `unit_simple-1.0.0/unit_simple.py` & `unit_simple-1.0.4/unit_simple.py`

 * *Files identical despite different names*

