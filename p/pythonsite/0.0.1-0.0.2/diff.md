# Comparing `tmp/pythonsite-0.0.1.tar.gz` & `tmp/pythonsite-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsite-0.0.1.tar", last modified: Sat Apr 22 04:28:38 2023, max compression
+gzip compressed data, was "pythonsite-0.0.2.tar", last modified: Sat Apr 22 04:31:35 2023, max compression
```

## Comparing `pythonsite-0.0.1.tar` & `pythonsite-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-22 04:28:38.145701 pythonsite-0.0.1/
--rw-r--r--   0 kali      (1000) kali      (1000)     1073 2023-04-15 11:08:56.000000 pythonsite-0.0.1/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)      505 2023-04-22 04:28:38.145701 pythonsite-0.0.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      117 2023-04-22 04:04:17.000000 pythonsite-0.0.1/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)      461 2023-04-22 04:22:51.000000 pythonsite-0.0.1/pyproject.toml
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-22 04:28:38.145701 pythonsite-0.0.1/setup.cfg
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-22 04:28:38.141701 pythonsite-0.0.1/src/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-22 04:28:38.145701 pythonsite-0.0.1/src/pythonsite/
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-22 04:28:14.000000 pythonsite-0.0.1/src/pythonsite/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       82 2023-04-22 04:01:27.000000 pythonsite-0.0.1/src/pythonsite/elements.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-22 04:28:38.145701 pythonsite-0.0.1/src/pythonsite.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      505 2023-04-22 04:28:38.000000 pythonsite-0.0.1/src/pythonsite.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      238 2023-04-22 04:28:38.000000 pythonsite-0.0.1/src/pythonsite.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-22 04:28:38.000000 pythonsite-0.0.1/src/pythonsite.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       11 2023-04-22 04:28:38.000000 pythonsite-0.0.1/src/pythonsite.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-22 04:31:35.255410 pythonsite-0.0.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1073 2023-04-15 11:08:56.000000 pythonsite-0.0.2/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)      510 2023-04-22 04:31:35.255410 pythonsite-0.0.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      122 2023-04-22 04:31:04.000000 pythonsite-0.0.2/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)      461 2023-04-22 04:31:13.000000 pythonsite-0.0.2/pyproject.toml
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-22 04:31:35.255410 pythonsite-0.0.2/setup.cfg
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-22 04:31:35.251410 pythonsite-0.0.2/src/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-22 04:31:35.255410 pythonsite-0.0.2/src/pythonsite/
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-22 04:28:14.000000 pythonsite-0.0.2/src/pythonsite/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       82 2023-04-22 04:01:27.000000 pythonsite-0.0.2/src/pythonsite/elements.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-22 04:31:35.255410 pythonsite-0.0.2/src/pythonsite.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)      510 2023-04-22 04:31:35.000000 pythonsite-0.0.2/src/pythonsite.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      238 2023-04-22 04:31:35.000000 pythonsite-0.0.2/src/pythonsite.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-22 04:31:35.000000 pythonsite-0.0.2/src/pythonsite.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       11 2023-04-22 04:31:35.000000 pythonsite-0.0.2/src/pythonsite.egg-info/top_level.txt
```

### Comparing `pythonsite-0.0.1/LICENSE` & `pythonsite-0.0.2/LICENSE`

 * *Files identical despite different names*

