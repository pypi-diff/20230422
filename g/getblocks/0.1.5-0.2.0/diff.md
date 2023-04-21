# Comparing `tmp/getblocks-0.1.5.tar.gz` & `tmp/getblocks-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getblocks-0.1.5.tar", last modified: Wed Feb 22 00:42:50 2023, max compression
+gzip compressed data, was "getblocks-0.2.0.tar", last modified: Fri Apr 21 22:01:34 2023, max compression
```

## Comparing `getblocks-0.1.5.tar` & `getblocks-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 00:42:50.492735 getblocks-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-22 00:42:34.000000 getblocks-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-02-22 00:42:50.492735 getblocks-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-22 00:42:34.000000 getblocks-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 00:42:50.488735 getblocks-0.1.5/getblocks/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-22 00:42:34.000000 getblocks-0.1.5/getblocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-22 00:42:34.000000 getblocks-0.1.5/getblocks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-02-22 00:42:34.000000 getblocks-0.1.5/getblocks/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 00:42:50.492735 getblocks-0.1.5/getblocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-02-22 00:42:50.000000 getblocks-0.1.5/getblocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-22 00:42:50.000000 getblocks-0.1.5/getblocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 00:42:50.000000 getblocks-0.1.5/getblocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-22 00:42:50.000000 getblocks-0.1.5/getblocks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 00:42:50.000000 getblocks-0.1.5/getblocks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-22 00:42:50.000000 getblocks-0.1.5/getblocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 00:42:50.000000 getblocks-0.1.5/getblocks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 00:42:50.492735 getblocks-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-22 00:42:34.000000 getblocks-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:01:34.433871 getblocks-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 22:01:20.000000 getblocks-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-21 22:01:34.433871 getblocks-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-21 22:01:20.000000 getblocks-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:01:34.433871 getblocks-0.2.0/getblocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 22:01:20.000000 getblocks-0.2.0/getblocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-21 22:01:20.000000 getblocks-0.2.0/getblocks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-21 22:01:20.000000 getblocks-0.2.0/getblocks/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:01:34.433871 getblocks-0.2.0/getblocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-21 22:01:34.000000 getblocks-0.2.0/getblocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-21 22:01:34.000000 getblocks-0.2.0/getblocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 22:01:34.000000 getblocks-0.2.0/getblocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 22:01:34.000000 getblocks-0.2.0/getblocks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 22:01:34.000000 getblocks-0.2.0/getblocks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 22:01:34.000000 getblocks-0.2.0/getblocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 22:01:34.000000 getblocks-0.2.0/getblocks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 22:01:34.433871 getblocks-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-21 22:01:20.000000 getblocks-0.2.0/setup.py
```

### Comparing `getblocks-0.1.5/LICENSE` & `getblocks-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `getblocks-0.1.5/PKG-INFO` & `getblocks-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 0.1.5
+Version: 0.2.0
 Summary: Down to the sector detail!
 Home-page: https://github.com/jblukach/getblocks
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # getblocks
 
+### Installation
+
+```
+curl https://sh.rustup.rs -sSf | sh -s -- -y
+source "$HOME/.cargo/env"
+pip3 install getblocks --upgrade
+```
+
+### Captured Data
+
 0. ami
 1. path
 2. file
 3. size
 4. md5
 5. sha256
 6. b3
```

### Comparing `getblocks-0.1.5/getblocks/cli.py` & `getblocks-0.2.0/getblocks/cli.py`

 * *Files identical despite different names*

### Comparing `getblocks-0.1.5/getblocks.egg-info/PKG-INFO` & `getblocks-0.2.0/getblocks.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 0.1.5
+Version: 0.2.0
 Summary: Down to the sector detail!
 Home-page: https://github.com/jblukach/getblocks
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # getblocks
 
+### Installation
+
+```
+curl https://sh.rustup.rs -sSf | sh -s -- -y
+source "$HOME/.cargo/env"
+pip3 install getblocks --upgrade
+```
+
+### Captured Data
+
 0. ami
 1. path
 2. file
 3. size
 4. md5
 5. sha256
 6. b3
```

### Comparing `getblocks-0.1.5/setup.py` & `getblocks-0.2.0/setup.py`

 * *Files identical despite different names*

