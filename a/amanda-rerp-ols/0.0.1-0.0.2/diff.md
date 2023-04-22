# Comparing `tmp/amanda_rerp_ols-0.0.1.tar.gz` & `tmp/amanda_rerp_ols-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amanda_rerp_ols-0.0.1.tar", last modified: Sat Apr  8 04:10:12 2023, max compression
+gzip compressed data, was "amanda_rerp_ols-0.0.2.tar", last modified: Fri Apr 21 19:58:27 2023, max compression
```

## Comparing `amanda_rerp_ols-0.0.1.tar` & `amanda_rerp_ols-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 amandalin047  (1000) amandalin047  (1000)        0 2023-04-08 04:10:12.330385 amanda_rerp_ols-0.0.1/
--rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)     1088 2023-04-08 02:50:39.000000 amanda_rerp_ols-0.0.1/LICENSE
--rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)     1092 2023-04-08 04:10:12.330385 amanda_rerp_ols-0.0.1/PKG-INFO
--rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)      482 2023-04-08 02:49:54.000000 amanda_rerp_ols-0.0.1/README.md
--rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)      714 2023-04-08 04:09:47.000000 amanda_rerp_ols-0.0.1/pyproject.toml
--rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)       38 2023-04-08 04:10:12.330385 amanda_rerp_ols-0.0.1/setup.cfg
-drwxr-xr-x   0 amandalin047  (1000) amandalin047  (1000)        0 2023-04-08 04:10:12.330385 amanda_rerp_ols-0.0.1/src/
-drwxr-xr-x   0 amandalin047  (1000) amandalin047  (1000)        0 2023-04-08 04:10:12.330385 amanda_rerp_ols-0.0.1/src/amanda_rerp_ols/
--rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)       27 2023-04-08 03:30:55.000000 amanda_rerp_ols-0.0.1/src/amanda_rerp_ols/__init__.py
--rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)     1869 2023-04-08 04:08:28.000000 amanda_rerp_ols-0.0.1/src/amanda_rerp_ols/my_functions.py
-drwxr-xr-x   0 amandalin047  (1000) amandalin047  (1000)        0 2023-04-08 04:10:12.330385 amanda_rerp_ols-0.0.1/src/amanda_rerp_ols.egg-info/
--rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)     1092 2023-04-08 04:10:12.000000 amanda_rerp_ols-0.0.1/src/amanda_rerp_ols.egg-info/PKG-INFO
--rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)      314 2023-04-08 04:10:12.000000 amanda_rerp_ols-0.0.1/src/amanda_rerp_ols.egg-info/SOURCES.txt
--rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)        1 2023-04-08 04:10:12.000000 amanda_rerp_ols-0.0.1/src/amanda_rerp_ols.egg-info/dependency_links.txt
--rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)       11 2023-04-08 04:10:12.000000 amanda_rerp_ols-0.0.1/src/amanda_rerp_ols.egg-info/requires.txt
--rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)       16 2023-04-08 04:10:12.000000 amanda_rerp_ols-0.0.1/src/amanda_rerp_ols.egg-info/top_level.txt
+drwxr-xr-x   0 amandalin047  (1000) amandalin047  (1000)        0 2023-04-21 19:58:27.061502 amanda_rerp_ols-0.0.2/
+-rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)     1074 2023-04-21 19:54:54.000000 amanda_rerp_ols-0.0.2/LICENSE
+-rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)      612 2023-04-21 19:58:27.061502 amanda_rerp_ols-0.0.2/PKG-INFO
+-rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)       68 2023-04-21 19:56:37.000000 amanda_rerp_ols-0.0.2/README.md
+-rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)      656 2023-04-21 19:53:20.000000 amanda_rerp_ols-0.0.2/pyproject.toml
+-rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)       38 2023-04-21 19:58:27.061502 amanda_rerp_ols-0.0.2/setup.cfg
+drwxr-xr-x   0 amandalin047  (1000) amandalin047  (1000)        0 2023-04-21 19:58:27.061502 amanda_rerp_ols-0.0.2/src/
+drwxr-xr-x   0 amandalin047  (1000) amandalin047  (1000)        0 2023-04-21 19:58:27.061502 amanda_rerp_ols-0.0.2/src/amanda_rerp_ols/
+-rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)       27 2023-04-21 19:48:11.000000 amanda_rerp_ols-0.0.2/src/amanda_rerp_ols/__init__.py
+-rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)     1869 2023-04-21 19:48:11.000000 amanda_rerp_ols-0.0.2/src/amanda_rerp_ols/my_functions.py
+drwxr-xr-x   0 amandalin047  (1000) amandalin047  (1000)        0 2023-04-21 19:58:27.061502 amanda_rerp_ols-0.0.2/src/amanda_rerp_ols.egg-info/
+-rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)      612 2023-04-21 19:58:27.000000 amanda_rerp_ols-0.0.2/src/amanda_rerp_ols.egg-info/PKG-INFO
+-rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)      314 2023-04-21 19:58:27.000000 amanda_rerp_ols-0.0.2/src/amanda_rerp_ols.egg-info/SOURCES.txt
+-rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)        1 2023-04-21 19:58:27.000000 amanda_rerp_ols-0.0.2/src/amanda_rerp_ols.egg-info/dependency_links.txt
+-rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)        4 2023-04-21 19:58:27.000000 amanda_rerp_ols-0.0.2/src/amanda_rerp_ols.egg-info/requires.txt
+-rw-r--r--   0 amandalin047  (1000) amandalin047  (1000)       16 2023-04-21 19:58:27.000000 amanda_rerp_ols-0.0.2/src/amanda_rerp_ols.egg-info/top_level.txt
```

### Comparing `amanda_rerp_ols-0.0.1/LICENSE` & `amanda_rerp_ols-0.0.2/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-The MIT License (MIT)
-
-Copyright (c) <year> <copyright holders>
+Copyright (c) 2018 The Python Packaging Authority
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `amanda_rerp_ols-0.0.1/src/amanda_rerp_ols/my_functions.py` & `amanda_rerp_ols-0.0.2/src/amanda_rerp_ols/my_functions.py`

 * *Files identical despite different names*

