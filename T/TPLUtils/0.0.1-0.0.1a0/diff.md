# Comparing `tmp/TPLUtils-0.0.1.tar.gz` & `tmp/TPLUtils-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TPLUtils-0.0.1.tar", last modified: Fri Apr 21 23:24:29 2023, max compression
+gzip compressed data, was "TPLUtils-0.0.1a0.tar", last modified: Fri Apr 21 23:30:07 2023, max compression
```

## Comparing `TPLUtils-0.0.1.tar` & `TPLUtils-0.0.1a0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:24:29.740484 TPLUtils-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-21 23:24:29.740484 TPLUtils-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-21 23:24:18.000000 TPLUtils-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:24:29.740484 TPLUtils-0.0.1/TPLUtils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-21 23:24:29.000000 TPLUtils-0.0.1/TPLUtils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-21 23:24:29.000000 TPLUtils-0.0.1/TPLUtils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 23:24:29.000000 TPLUtils-0.0.1/TPLUtils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-21 23:24:29.000000 TPLUtils-0.0.1/TPLUtils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-21 23:24:29.000000 TPLUtils-0.0.1/TPLUtils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 23:24:29.740484 TPLUtils-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-21 23:24:18.000000 TPLUtils-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:24:29.740484 TPLUtils-0.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 23:24:18.000000 TPLUtils-0.0.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:24:29.740484 TPLUtils-0.0.1/src/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 23:24:18.000000 TPLUtils-0.0.1/src/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-21 23:24:18.000000 TPLUtils-0.0.1/src/db/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-21 23:24:18.000000 TPLUtils-0.0.1/src/db/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:24:29.740484 TPLUtils-0.0.1/src/utility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 23:24:18.000000 TPLUtils-0.0.1/src/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-21 23:24:18.000000 TPLUtils-0.0.1/src/utility/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:30:07.032249 TPLUtils-0.0.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-21 23:30:07.032249 TPLUtils-0.0.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-21 23:29:55.000000 TPLUtils-0.0.1a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 23:30:07.032249 TPLUtils-0.0.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-21 23:29:55.000000 TPLUtils-0.0.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:30:07.032249 TPLUtils-0.0.1a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:30:07.032249 TPLUtils-0.0.1a0/src/TPLUtils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-21 23:30:06.000000 TPLUtils-0.0.1a0/src/TPLUtils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-21 23:30:07.000000 TPLUtils-0.0.1a0/src/TPLUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 23:30:06.000000 TPLUtils-0.0.1a0/src/TPLUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-21 23:30:06.000000 TPLUtils-0.0.1a0/src/TPLUtils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 23:30:06.000000 TPLUtils-0.0.1a0/src/TPLUtils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:30:07.032249 TPLUtils-0.0.1a0/src/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 23:29:55.000000 TPLUtils-0.0.1a0/src/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-21 23:29:55.000000 TPLUtils-0.0.1a0/src/db/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-21 23:29:55.000000 TPLUtils-0.0.1a0/src/db/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:30:07.032249 TPLUtils-0.0.1a0/src/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 23:29:55.000000 TPLUtils-0.0.1a0/src/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-21 23:29:55.000000 TPLUtils-0.0.1a0/src/utility/logging.py
```

### Comparing `TPLUtils-0.0.1/src/db/config.py` & `TPLUtils-0.0.1a0/src/db/config.py`

 * *Files identical despite different names*

### Comparing `TPLUtils-0.0.1/src/db/user.py` & `TPLUtils-0.0.1a0/src/db/user.py`

 * *Files identical despite different names*

