# Comparing `tmp/ypmp_example-0.1.1.tar.gz` & `tmp/ypmp_example-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypmp_example-0.1.1.tar", max compression
+gzip compressed data, was "ypmp_example-0.2.0.tar", max compression
```

## Comparing `ypmp_example-0.1.1.tar` & `ypmp_example-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1649 2023-04-22 15:46:26.081781 ypmp_example-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       51 2023-04-22 15:46:00.236734 ypmp_example-0.1.1/ypmp_example/__init__.py
--rw-r--r--   0        0        0       49 2023-04-22 15:46:00.236734 ypmp_example-0.1.1/ypmp_example/functions.py
--rw-r--r--   0        0        0        0 2023-04-22 15:46:00.236734 ypmp_example-0.1.1/ypmp_example/py.typed
--rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 ypmp_example-0.1.1/setup.py
--rw-r--r--   0        0        0      368 1970-01-01 00:00:00.000000 ypmp_example-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1649 2023-04-22 15:51:51.943526 ypmp_example-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-04-22 15:51:31.955654 ypmp_example-0.2.0/ypmp_example/__init__.py
+-rw-r--r--   0        0        0       49 2023-04-22 15:51:31.955654 ypmp_example-0.2.0/ypmp_example/functions.py
+-rw-r--r--   0        0        0        0 2023-04-22 15:51:31.955654 ypmp_example-0.2.0/ypmp_example/py.typed
+-rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 ypmp_example-0.2.0/setup.py
+-rw-r--r--   0        0        0      368 1970-01-01 00:00:00.000000 ypmp_example-0.2.0/PKG-INFO
```

### Comparing `ypmp_example-0.1.1/pyproject.toml` & `ypmp_example-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 profile = "black"
 py_version = 310
 
 [tool.poetry]
 authors = ["ovsds <ovsds@yandex-team.ru>"]
 description = "Example package for YP 24"
 name = "ypmp-example"
-version = "0.1.1"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 
 [tool.poetry.dev-dependencies]
 black = "22.10.0"
 isort = "5.10.1"
```

### Comparing `ypmp_example-0.1.1/setup.py` & `ypmp_example-0.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['ypmp_example']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'ypmp-example',
-    'version': '0.1.1',
+    'version': '0.2.0',
     'description': 'Example package for YP 24',
     'long_description': 'None',
     'author': 'ovsds',
     'author_email': 'ovsds@yandex-team.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

