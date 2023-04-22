# Comparing `tmp/firepup650-1.0.4.tar.gz` & `tmp/firepup650-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firepup650-1.0.4.tar", last modified: Fri Apr 21 14:43:26 2023, max compression
+gzip compressed data, was "firepup650-1.0.5.tar", last modified: Sat Apr 22 02:21:15 2023, max compression
```

## Comparing `firepup650-1.0.4.tar` & `firepup650-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 14:43:26.836159 firepup650-1.0.4/
--rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 firepup650-1.0.4/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1274 2023-04-21 14:43:26.836159 firepup650-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      327 2023-04-21 14:41:13.000000 firepup650-1.0.4/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-04-21 14:24:26.000000 firepup650-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)      895 2023-04-21 14:43:26.836159 firepup650-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 14:43:26.832159 firepup650-1.0.4/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 14:43:26.836159 firepup650-1.0.4/src/firepup650/
--rw-r--r--   0 runner    (1000) runner    (1000)     3382 2023-04-21 14:40:17.000000 firepup650-1.0.4/src/firepup650/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 14:43:26.836159 firepup650-1.0.4/src/firepup650.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1274 2023-04-21 14:43:26.000000 firepup650-1.0.4/src/firepup650.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      221 2023-04-21 14:43:26.000000 firepup650-1.0.4/src/firepup650.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-21 14:43:26.000000 firepup650-1.0.4/src/firepup650.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-04-21 14:43:26.000000 firepup650-1.0.4/src/firepup650.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-22 02:21:15.327068 firepup650-1.0.5/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 firepup650-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1384 2023-04-22 02:21:15.327068 firepup650-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      421 2023-04-22 02:17:46.000000 firepup650-1.0.5/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2023-04-22 02:18:06.000000 firepup650-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)      895 2023-04-22 02:21:15.327068 firepup650-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-22 02:21:15.319068 firepup650-1.0.5/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-22 02:21:15.319068 firepup650-1.0.5/src/firepup650/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3382 2023-04-21 14:40:17.000000 firepup650-1.0.5/src/firepup650/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-22 02:21:15.327068 firepup650-1.0.5/src/firepup650.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1384 2023-04-22 02:21:14.000000 firepup650-1.0.5/src/firepup650.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      221 2023-04-22 02:21:15.000000 firepup650-1.0.5/src/firepup650.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-22 02:21:14.000000 firepup650-1.0.5/src/firepup650.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-04-22 02:21:14.000000 firepup650-1.0.5/src/firepup650.egg-info/top_level.txt
```

### Comparing `firepup650-1.0.4/LICENSE` & `firepup650-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `firepup650-1.0.4/PKG-INFO` & `firepup650-1.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: firepup650
-Version: 1.0.4
+Version: 1.0.5
 Summary: Package containing various shorthand things I use, and a few imports I almost always use
 Home-page: https://github.com/F1repup650/firepup650-PYPI
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/F1repup650/firepup650-PYPI/issues
 Project-URL: replit, https://replit.com/@Firepup650/firepup650-PYPI-Package
 Description: # Firepup650
         Package containing various shorthand things I use, and a few imports I almost always use
         #### Change log:
+        ###### v.1.0.5:
+        Hopefully, fixes an issue where the package doesn't install it's dependencies
         ###### v.1.0.4:
         Subscript errors
         ###### v.1.0.3:
         Dependant errors
         ###### v.1.0.2:
         Random shorthand (litterally)
         ###### v.1.0.1:
```

### Comparing `firepup650-1.0.4/setup.cfg` & `firepup650-1.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = firepup650
-version = 1.0.4
+version = 1.0.5
 author = Firepup650
 author_email = firepyp650@gmail.com
 description = Package containing various shorthand things I use, and a few imports I almost always use
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/F1repup650/firepup650-PYPI
 project_urls =
```

### Comparing `firepup650-1.0.4/src/firepup650/__init__.py` & `firepup650-1.0.5/src/firepup650/__init__.py`

 * *Files identical despite different names*

### Comparing `firepup650-1.0.4/src/firepup650.egg-info/PKG-INFO` & `firepup650-1.0.5/src/firepup650.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: firepup650
-Version: 1.0.4
+Version: 1.0.5
 Summary: Package containing various shorthand things I use, and a few imports I almost always use
 Home-page: https://github.com/F1repup650/firepup650-PYPI
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/F1repup650/firepup650-PYPI/issues
 Project-URL: replit, https://replit.com/@Firepup650/firepup650-PYPI-Package
 Description: # Firepup650
         Package containing various shorthand things I use, and a few imports I almost always use
         #### Change log:
+        ###### v.1.0.5:
+        Hopefully, fixes an issue where the package doesn't install it's dependencies
         ###### v.1.0.4:
         Subscript errors
         ###### v.1.0.3:
         Dependant errors
         ###### v.1.0.2:
         Random shorthand (litterally)
         ###### v.1.0.1:
```

