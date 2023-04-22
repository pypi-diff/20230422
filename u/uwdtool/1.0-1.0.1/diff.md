# Comparing `tmp/uwdtool-1.0.tar.gz` & `tmp/uwdtool-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwdtool-1.0.tar", max compression
+gzip compressed data, was "uwdtool-1.0.1.tar", max compression
```

## Comparing `uwdtool-1.0.tar` & `uwdtool-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2510 2023-04-22 03:28:37.833937 uwdtool-1.0/README.md
--rw-r--r--   0        0        0      365 2023-04-22 03:31:00.434212 uwdtool-1.0/pyproject.toml
--rw-r--r--   0        0        0     7457 2023-04-22 03:21:43.645395 uwdtool-1.0/uwdtool/UWDTool.py
--rw-r--r--   0        0        0        0 2023-04-22 03:25:18.701618 uwdtool-1.0/uwdtool/__init__.py
--rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 uwdtool-1.0/PKG-INFO
+-rw-r--r--   0        0        0     2288 2023-04-22 03:36:42.542973 uwdtool-1.0.1/README.md
+-rw-r--r--   0        0        0      367 2023-04-22 03:44:07.836084 uwdtool-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7459 2023-04-22 03:44:15.172103 uwdtool-1.0.1/uwdtool/UWDTool.py
+-rw-r--r--   0        0        0        0 2023-04-22 03:25:18.701618 uwdtool-1.0.1/uwdtool/__init__.py
+-rw-r--r--   0        0        0     2820 1970-01-01 00:00:00.000000 uwdtool-1.0.1/PKG-INFO
```

### Comparing `uwdtool-1.0/uwdtool/UWDTool.py` & `uwdtool-1.0.1/uwdtool/UWDTool.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import struct
 import os
 import hashlib
 from glob import glob
 from pathlib import Path
 
 
-UWDT_VERSION = "1.0"
+UWDT_VERSION = "1.0.1"
 HELP_STR = f"""UWDTool v{UWDT_VERSION}"""
 
 
 class UWDTException(Exception):
     def __init__(self, msg):
         self.msg = msg
```

