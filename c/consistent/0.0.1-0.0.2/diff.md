# Comparing `tmp/consistent-0.0.1.tar.gz` & `tmp/consistent-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consistent-0.0.1.tar", last modified: Sat Apr 22 10:06:45 2023, max compression
+gzip compressed data, was "consistent-0.0.2.tar", last modified: Sat Apr 22 10:39:30 2023, max compression
```

## Comparing `consistent-0.0.1.tar` & `consistent-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:06:45.870262 consistent-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-04-19 15:06:29.000000 consistent-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1703 2023-04-22 10:06:45.870262 consistent-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-22 09:22:37.000000 consistent-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:06:45.850262 consistent-0.0.1/consisTent/
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-22 09:22:37.000000 consistent-0.0.1/consisTent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:06:45.860262 consistent-0.0.1/consisTent/cache/
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-22 09:22:37.000000 consistent-0.0.1/consisTent/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)      277 2023-04-22 09:22:37.000000 consistent-0.0.1/consisTent/cache/base_cache.py
--rw-r--r--   0 root         (0) root         (0)     1150 2023-04-22 09:22:37.000000 consistent-0.0.1/consisTent/cache/chroma_cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:06:45.860262 consistent-0.0.1/consisTent/validators/
--rw-r--r--   0 root         (0) root         (0)       98 2023-04-22 09:22:37.000000 consistent-0.0.1/consisTent/validators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-04-22 09:22:37.000000 consistent-0.0.1/consisTent/validators/base_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:06:45.870262 consistent-0.0.1/consisTent/validators/semantic_validators/
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-22 09:22:37.000000 consistent-0.0.1/consisTent/validators/semantic_validators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1157 2023-04-22 09:22:37.000000 consistent-0.0.1/consisTent/validators/semantic_validators/consistency_validator.py
--rw-r--r--   0 root         (0) root         (0)     2667 2023-04-22 09:22:37.000000 consistent-0.0.1/consisTent/validators/semantic_validators/openai_validator.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-04-22 09:22:37.000000 consistent-0.0.1/consisTent/validators/syntactic_validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:06:45.870262 consistent-0.0.1/consistent.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1703 2023-04-22 10:06:45.000000 consistent-0.0.1/consistent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      620 2023-04-22 10:06:45.000000 consistent-0.0.1/consistent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 10:06:45.000000 consistent-0.0.1/consistent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      124 2023-04-22 10:06:45.000000 consistent-0.0.1/consistent.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-22 10:06:45.000000 consistent-0.0.1/consistent.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1151 2023-04-22 10:04:00.000000 consistent-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 10:06:45.870262 consistent-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:39:30.032233 consistent-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-22 10:39:18.000000 consistent-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-22 10:39:30.032233 consistent-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-22 10:39:18.000000 consistent-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:39:30.028232 consistent-0.0.2/consisTent/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:39:30.028232 consistent-0.0.2/consisTent/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/cache/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/cache/chroma_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:39:30.028232 consistent-0.0.2/consisTent/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/validators/base_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:39:30.028232 consistent-0.0.2/consisTent/validators/semantic_validators/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/validators/semantic_validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/validators/semantic_validators/consistency_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/validators/semantic_validators/openai_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/validators/syntactic_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:39:30.032233 consistent-0.0.2/consistent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-22 10:39:30.000000 consistent-0.0.2/consistent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-22 10:39:30.000000 consistent-0.0.2/consistent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 10:39:30.000000 consistent-0.0.2/consistent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-22 10:39:30.000000 consistent-0.0.2/consistent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 10:39:30.000000 consistent-0.0.2/consistent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-22 10:39:18.000000 consistent-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 10:39:30.032233 consistent-0.0.2/setup.cfg
```

### Comparing `consistent-0.0.1/LICENSE` & `consistent-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `consistent-0.0.1/PKG-INFO` & `consistent-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consistent
-Version: 0.0.1
+Version: 0.0.2
 Summary: Make sure AI model outputs are consistent
 License: MIT License
         
         Copyright (c) 2023 drorIvry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `consistent-0.0.1/consisTent/cache/chroma_cache.py` & `consistent-0.0.2/consisTent/cache/chroma_cache.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.1/consisTent/validators/semantic_validators/consistency_validator.py` & `consistent-0.0.2/consisTent/validators/semantic_validators/consistency_validator.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.1/consisTent/validators/semantic_validators/openai_validator.py` & `consistent-0.0.2/consisTent/validators/semantic_validators/openai_validator.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.1/consisTent/validators/syntactic_validators.py` & `consistent-0.0.2/consisTent/validators/syntactic_validators.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.1/consistent.egg-info/PKG-INFO` & `consistent-0.0.2/consistent.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consistent
-Version: 0.0.1
+Version: 0.0.2
 Summary: Make sure AI model outputs are consistent
 License: MIT License
         
         Copyright (c) 2023 drorIvry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `consistent-0.0.1/consistent.egg-info/SOURCES.txt` & `consistent-0.0.2/consistent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `consistent-0.0.1/pyproject.toml` & `consistent-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "consistent"
-version = "0.0.1"
+version = "0.0.2"
 description = "Make sure AI model outputs are consistent"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -28,17 +28,17 @@
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest", "pre-commit", "pyflakes"]
 
 [project.urls]
 Homepage = "https://github.com/drorivry/consistent"
 
 
 [tool.bumpver]
-current_version = "0.0.1"
+current_version = "0.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"src/reader/__init__.py" = ["{version}"]
+"consistent/__init__.py" = ["{version}"]
```

