# Comparing `tmp/gokyuzu-0.0.1.tar.gz` & `tmp/gokyuzu-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gokyuzu-0.0.1.tar", last modified: Sat Apr 22 14:49:46 2023, max compression
+gzip compressed data, was "gokyuzu-0.0.3.tar", last modified: Sat Apr 22 15:15:43 2023, max compression
```

## Comparing `gokyuzu-0.0.1.tar` & `gokyuzu-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 14:49:46.873803 gokyuzu-0.0.1/
--rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 12:13:25.000000 gokyuzu-0.0.1/LICENSE
--rw-r--r--   0 kilic      (501) staff       (20)      734 2023-04-22 14:49:46.873699 gokyuzu-0.0.1/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      522 2023-04-22 14:32:54.000000 gokyuzu-0.0.1/README.md
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 14:49:46.872559 gokyuzu-0.0.1/gokyuzu/
--rw-r--r--   0 kilic      (501) staff       (20)      761 2023-04-22 14:14:34.000000 gokyuzu-0.0.1/gokyuzu/BlueskyEndpoints.py
--rw-r--r--   0 kilic      (501) staff       (20)      161 2023-04-22 14:12:10.000000 gokyuzu-0.0.1/gokyuzu/BlueskyHelper.py
--rw-r--r--   0 kilic      (501) staff       (20)     2300 2023-04-22 14:17:06.000000 gokyuzu-0.0.1/gokyuzu/BlueskySession.py
--rw-r--r--   0 kilic      (501) staff       (20)     1723 2023-04-22 14:20:55.000000 gokyuzu-0.0.1/gokyuzu/__init__.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 14:49:46.873224 gokyuzu-0.0.1/gokyuzu.egg-info/
--rw-r--r--   0 kilic      (501) staff       (20)      734 2023-04-22 14:49:46.000000 gokyuzu-0.0.1/gokyuzu.egg-info/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      316 2023-04-22 14:49:46.000000 gokyuzu-0.0.1/gokyuzu.egg-info/SOURCES.txt
--rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-22 14:49:46.000000 gokyuzu-0.0.1/gokyuzu.egg-info/dependency_links.txt
--rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-22 14:49:46.000000 gokyuzu-0.0.1/gokyuzu.egg-info/requires.txt
--rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-22 14:49:46.000000 gokyuzu-0.0.1/gokyuzu.egg-info/top_level.txt
--rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-22 14:49:46.873848 gokyuzu-0.0.1/setup.cfg
--rw-r--r--   0 kilic      (501) staff       (20)      906 2023-04-22 14:31:17.000000 gokyuzu-0.0.1/setup.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 14:49:46.873420 gokyuzu-0.0.1/tests/
--rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 11:38:56.000000 gokyuzu-0.0.1/tests/__init__.py
--rw-r--r--   0 kilic      (501) staff       (20)     1067 2023-04-22 14:33:58.000000 gokyuzu-0.0.1/tests/test_main.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:15:43.692941 gokyuzu-0.0.3/
+-rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 12:13:25.000000 gokyuzu-0.0.3/LICENSE
+-rw-r--r--   0 kilic      (501) staff       (20)     1563 2023-04-22 15:15:43.692814 gokyuzu-0.0.3/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)      787 2023-04-22 15:03:09.000000 gokyuzu-0.0.3/README.md
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:15:43.691710 gokyuzu-0.0.3/gokyuzu/
+-rw-r--r--   0 kilic      (501) staff       (20)      761 2023-04-22 14:14:34.000000 gokyuzu-0.0.3/gokyuzu/BlueskyEndpoints.py
+-rw-r--r--   0 kilic      (501) staff       (20)      161 2023-04-22 14:12:10.000000 gokyuzu-0.0.3/gokyuzu/BlueskyHelper.py
+-rw-r--r--   0 kilic      (501) staff       (20)     2300 2023-04-22 14:17:06.000000 gokyuzu-0.0.3/gokyuzu/BlueskySession.py
+-rw-r--r--   0 kilic      (501) staff       (20)     1723 2023-04-22 14:20:55.000000 gokyuzu-0.0.3/gokyuzu/__init__.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:15:43.692331 gokyuzu-0.0.3/gokyuzu.egg-info/
+-rw-r--r--   0 kilic      (501) staff       (20)     1563 2023-04-22 15:15:43.000000 gokyuzu-0.0.3/gokyuzu.egg-info/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)      331 2023-04-22 15:15:43.000000 gokyuzu-0.0.3/gokyuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-22 15:15:43.000000 gokyuzu-0.0.3/gokyuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-22 15:15:43.000000 gokyuzu-0.0.3/gokyuzu.egg-info/requires.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-22 15:15:43.000000 gokyuzu-0.0.3/gokyuzu.egg-info/top_level.txt
+-rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-22 15:13:44.000000 gokyuzu-0.0.3/pyproject.toml
+-rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-22 15:15:43.692973 gokyuzu-0.0.3/setup.cfg
+-rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-22 15:13:37.000000 gokyuzu-0.0.3/setup.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:15:43.692535 gokyuzu-0.0.3/tests/
+-rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 11:38:56.000000 gokyuzu-0.0.3/tests/__init__.py
+-rw-r--r--   0 kilic      (501) staff       (20)     1067 2023-04-22 14:33:58.000000 gokyuzu-0.0.3/tests/test_main.py
```

### Comparing `gokyuzu-0.0.1/README.md` & `gokyuzu-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -26,8 +26,23 @@
 pip install -r requirements.txt
 ```
 
 ### Running tests
 
 ```bash
 python -m unittest
+```
+
+### Publishing to PyPI
+
+```bash
+# Build for PyPI
+python -m build
+
+# Test PyPI
+python -m twine upload --repository testpypi dist/*
+pip install --index-url https://test.pypi.org/simple/ --no-deps gokyuzu
+
+# PyPI
+python -m twine upload dist/*
+pip install gokyuzu
 ```
```

### Comparing `gokyuzu-0.0.1/gokyuzu/BlueskyEndpoints.py` & `gokyuzu-0.0.3/gokyuzu/BlueskyEndpoints.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-0.0.1/gokyuzu/BlueskySession.py` & `gokyuzu-0.0.3/gokyuzu/BlueskySession.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-0.0.1/gokyuzu/__init__.py` & `gokyuzu-0.0.3/gokyuzu/__init__.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-0.0.1/tests/test_main.py` & `gokyuzu-0.0.3/tests/test_main.py`

 * *Files identical despite different names*

