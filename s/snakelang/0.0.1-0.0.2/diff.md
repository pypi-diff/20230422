# Comparing `tmp/snakelang-0.0.1.tar.gz` & `tmp/snakelang-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakelang-0.0.1.tar", last modified: Fri Apr 21 22:35:15 2023, max compression
+gzip compressed data, was "snakelang-0.0.2.tar", last modified: Fri Apr 21 22:38:30 2023, max compression
```

## Comparing `snakelang-0.0.1.tar` & `snakelang-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-21 22:35:15.401428 snakelang-0.0.1/
--rw-r--r--   0 emery      (504) staff       (20)      468 2023-04-21 22:35:15.401318 snakelang-0.0.1/PKG-INFO
--rw-r--r--   0 emery      (504) staff       (20)      615 2023-04-21 22:32:28.000000 snakelang-0.0.1/pyproject.toml
--rw-r--r--   0 emery      (504) staff       (20)       38 2023-04-21 22:35:15.401457 snakelang-0.0.1/setup.cfg
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-21 22:35:15.400574 snakelang-0.0.1/snakelang/
--rw-r--r--   0 emery      (504) staff       (20)       56 2023-04-21 22:32:38.000000 snakelang-0.0.1/snakelang/__init__.py
--rw-r--r--   0 emery      (504) staff       (20)     3938 2023-04-21 22:32:38.000000 snakelang-0.0.1/snakelang/snakelang_module.py
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-21 22:35:15.401082 snakelang-0.0.1/snakelang.egg-info/
--rw-r--r--   0 emery      (504) staff       (20)      468 2023-04-21 22:35:15.000000 snakelang-0.0.1/snakelang.egg-info/PKG-INFO
--rw-r--r--   0 emery      (504) staff       (20)      247 2023-04-21 22:35:15.000000 snakelang-0.0.1/snakelang.egg-info/SOURCES.txt
--rw-r--r--   0 emery      (504) staff       (20)        1 2023-04-21 22:35:15.000000 snakelang-0.0.1/snakelang.egg-info/dependency_links.txt
--rw-r--r--   0 emery      (504) staff       (20)       28 2023-04-21 22:35:15.000000 snakelang-0.0.1/snakelang.egg-info/requires.txt
--rw-r--r--   0 emery      (504) staff       (20)       10 2023-04-21 22:35:15.000000 snakelang-0.0.1/snakelang.egg-info/top_level.txt
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-21 22:35:15.401183 snakelang-0.0.1/test/
--rw-r--r--   0 emery      (504) staff       (20)      159 2023-04-21 22:34:26.000000 snakelang-0.0.1/test/test-fib.py
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-21 22:38:30.675780 snakelang-0.0.2/
+-rw-r--r--   0 emery      (504) staff       (20)      468 2023-04-21 22:38:30.675679 snakelang-0.0.2/PKG-INFO
+-rw-r--r--   0 emery      (504) staff       (20)      615 2023-04-21 22:38:04.000000 snakelang-0.0.2/pyproject.toml
+-rw-r--r--   0 emery      (504) staff       (20)       38 2023-04-21 22:38:30.675808 snakelang-0.0.2/setup.cfg
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-21 22:38:30.674960 snakelang-0.0.2/snakelang/
+-rw-r--r--   0 emery      (504) staff       (20)       56 2023-04-21 22:32:38.000000 snakelang-0.0.2/snakelang/__init__.py
+-rw-r--r--   0 emery      (504) staff       (20)     3940 2023-04-21 22:37:47.000000 snakelang-0.0.2/snakelang/snakelang_module.py
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-21 22:38:30.675465 snakelang-0.0.2/snakelang.egg-info/
+-rw-r--r--   0 emery      (504) staff       (20)      468 2023-04-21 22:38:30.000000 snakelang-0.0.2/snakelang.egg-info/PKG-INFO
+-rw-r--r--   0 emery      (504) staff       (20)      247 2023-04-21 22:38:30.000000 snakelang-0.0.2/snakelang.egg-info/SOURCES.txt
+-rw-r--r--   0 emery      (504) staff       (20)        1 2023-04-21 22:38:30.000000 snakelang-0.0.2/snakelang.egg-info/dependency_links.txt
+-rw-r--r--   0 emery      (504) staff       (20)       28 2023-04-21 22:38:30.000000 snakelang-0.0.2/snakelang.egg-info/requires.txt
+-rw-r--r--   0 emery      (504) staff       (20)       10 2023-04-21 22:38:30.000000 snakelang-0.0.2/snakelang.egg-info/top_level.txt
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-21 22:38:30.675559 snakelang-0.0.2/test/
+-rw-r--r--   0 emery      (504) staff       (20)      159 2023-04-21 22:34:26.000000 snakelang-0.0.2/test/test-fib.py
```

### Comparing `snakelang-0.0.1/pyproject.toml` & `snakelang-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snakelang"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Emery Berger", email="emery.berger@gmail.com" },
 ]
 dependencies = ["openai>=0.27.0", "click>=8.1.3"]
 description = "TBD."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `snakelang-0.0.1/snakelang/snakelang_module.py` & `snakelang-0.0.2/snakelang/snakelang_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             {string}
 
             The function should have the following argument types and return type:
             
             Arguments: {arg_types}
             Return type: {return_type}
             """
-            print(prompt)
+            # print(prompt)
             # See if we already have code for that prompt.
             function_def = cdb.get_code(prompt)
             if not function_def:
                 result = complete(prompt)
                 # print(result)
                 #try:
                 the_json = json.loads(result)
```

