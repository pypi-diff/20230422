# Comparing `tmp/secure_package_template-0.7.0.tar.gz` & `tmp/secure_package_template-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Apr 22 19:15:07 2023, max compression
+gzip compressed data, last modified: Sat Apr 22 19:46:26 2023, max compression
```

## Comparing `secure_package_template-0.7.0.tar` & `secure_package_template-0.7.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1756 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0       63 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/src/secure_package_template/__init__.py
--rw-r--r--   0        0        0       22 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/src/secure_package_template/_version.py
--rw-r--r--   0        0        0        0 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/src/secure_package_template/py.typed
--rw-r--r--   0        0        0     3079 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/.gitignore
--rw-r--r--   0        0        0     1147 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/LICENSE
--rw-r--r--   0        0        0    15497 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/README.md
--rw-r--r--   0        0        0      895 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    17109 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1934 2023-04-22 19:46:26.000000 secure_package_template-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0       63 2023-04-22 19:46:26.000000 secure_package_template-0.7.1/src/secure_package_template/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-22 19:46:26.000000 secure_package_template-0.7.1/src/secure_package_template/_version.py
+-rw-r--r--   0        0        0        0 2023-04-22 19:46:26.000000 secure_package_template-0.7.1/src/secure_package_template/py.typed
+-rw-r--r--   0        0        0     3079 2023-04-22 19:46:26.000000 secure_package_template-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1147 2023-04-22 19:46:26.000000 secure_package_template-0.7.1/LICENSE
+-rw-r--r--   0        0        0    15497 2023-04-22 19:46:26.000000 secure_package_template-0.7.1/README.md
+-rw-r--r--   0        0        0      895 2023-04-22 19:46:26.000000 secure_package_template-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    17109 2023-04-22 19:46:26.000000 secure_package_template-0.7.1/PKG-INFO
```

### Comparing `secure_package_template-0.7.0/CHANGELOG.md` & `secure_package_template-0.7.1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # Changelog
 <!-- scriv-insert-here -->
 
+<a id='changelog-0.7.1'></a>
+## 0.7.1 (2023-04-22)
+
+### Changed
+
+- Changed the `build.outputs.hashes` state to use `$GITHUB_OUTPUT` instead of deprecated `::set-output` method.
+
 <a id='changelog-0.7.0'></a>
 ## 0.7.0 (2023-04-22)
 
 ### Added
 
 - Added instructions on how to configure a Trusted Publisher.
```

### Comparing `secure_package_template-0.7.0/.gitignore` & `secure_package_template-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `secure_package_template-0.7.0/LICENSE` & `secure_package_template-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `secure_package_template-0.7.0/README.md` & `secure_package_template-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `secure_package_template-0.7.0/pyproject.toml` & `secure_package_template-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `secure_package_template-0.7.0/PKG-INFO` & `secure_package_template-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure_package_template
-Version: 0.7.0
+Version: 0.7.1
 Summary: Template for a Python package with a secure project host and package repository configuration.
 Project-URL: Source, https://github.com/sethmlarson/secure-python-package-template
 Author-email: Seth Michael Larson <sethmichaellarson@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or distribute this software, either in source code form or as a compiled binary, for any purpose, commercial or non-commercial, and by any means.
```

