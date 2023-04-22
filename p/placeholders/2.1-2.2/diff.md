# Comparing `tmp/placeholders-2.1.tar.gz` & `tmp/placeholders-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "placeholders-2.1.tar", last modified: Sat Apr 22 13:20:47 2023, max compression
+gzip compressed data, was "placeholders-2.2.tar", last modified: Sat Apr 22 13:40:30 2023, max compression
```

## Comparing `placeholders-2.1.tar` & `placeholders-2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:20:47.711733 placeholders-2.1/
--rw-r--r--   0 austinbrown   (501) staff       (20)     1074 2023-04-22 12:00:08.000000 placeholders-2.1/LICENSE
--rw-r--r--   0 austinbrown   (501) staff       (20)        0 2023-04-22 12:00:25.000000 placeholders-2.1/MANIFEST.in
--rw-r--r--   0 austinbrown   (501) staff       (20)     1356 2023-04-22 13:20:47.711383 placeholders-2.1/PKG-INFO
--rw-r--r--   0 austinbrown   (501) staff       (20)     1016 2023-04-22 12:59:04.000000 placeholders-2.1/README.md
-drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:20:47.701770 placeholders-2.1/placeholders/
--rw-r--r--   0 austinbrown   (501) staff       (20)        0 2023-04-22 11:33:55.000000 placeholders-2.1/placeholders/__init__.py
--rw-r--r--   0 austinbrown   (501) staff       (20)      976 2023-04-22 13:03:08.000000 placeholders-2.1/placeholders/controls.py
--rw-r--r--   0 austinbrown   (501) staff       (20)     2118 2023-04-22 11:45:07.000000 placeholders-2.1/placeholders/tools.py
-drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:20:47.703812 placeholders-2.1/placeholders.egg-info/
--rw-r--r--   0 austinbrown   (501) staff       (20)     1356 2023-04-22 13:20:47.000000 placeholders-2.1/placeholders.egg-info/PKG-INFO
--rw-r--r--   0 austinbrown   (501) staff       (20)      310 2023-04-22 13:20:47.000000 placeholders-2.1/placeholders.egg-info/SOURCES.txt
--rw-r--r--   0 austinbrown   (501) staff       (20)        1 2023-04-22 13:20:47.000000 placeholders-2.1/placeholders.egg-info/dependency_links.txt
--rw-r--r--   0 austinbrown   (501) staff       (20)      478 2023-04-22 13:20:47.000000 placeholders-2.1/placeholders.egg-info/requires.txt
--rw-r--r--   0 austinbrown   (501) staff       (20)       13 2023-04-22 13:20:47.000000 placeholders-2.1/placeholders.egg-info/top_level.txt
-drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:20:47.704090 placeholders-2.1/scripts/
--rwxr-xr-x   0 austinbrown   (501) staff       (20)     1101 2023-04-22 13:00:19.000000 placeholders-2.1/scripts/placeholders
--rw-r--r--   0 austinbrown   (501) staff       (20)       38 2023-04-22 13:20:47.711813 placeholders-2.1/setup.cfg
--rw-r--r--   0 austinbrown   (501) staff       (20)     1441 2023-04-22 13:20:25.000000 placeholders-2.1/setup.py
+drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:40:30.920204 placeholders-2.2/
+-rw-r--r--   0 austinbrown   (501) staff       (20)     1074 2023-04-22 12:00:08.000000 placeholders-2.2/LICENSE
+-rw-r--r--   0 austinbrown   (501) staff       (20)        0 2023-04-22 12:00:25.000000 placeholders-2.2/MANIFEST.in
+-rw-r--r--   0 austinbrown   (501) staff       (20)     1356 2023-04-22 13:40:30.920061 placeholders-2.2/PKG-INFO
+-rw-r--r--   0 austinbrown   (501) staff       (20)     1016 2023-04-22 12:59:04.000000 placeholders-2.2/README.md
+drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:40:30.918686 placeholders-2.2/placeholders/
+-rw-r--r--   0 austinbrown   (501) staff       (20)        0 2023-04-22 11:33:55.000000 placeholders-2.2/placeholders/__init__.py
+-rw-r--r--   0 austinbrown   (501) staff       (20)      976 2023-04-22 13:03:08.000000 placeholders-2.2/placeholders/controls.py
+-rw-r--r--   0 austinbrown   (501) staff       (20)     2118 2023-04-22 11:45:07.000000 placeholders-2.2/placeholders/tools.py
+drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:40:30.919525 placeholders-2.2/placeholders.egg-info/
+-rw-r--r--   0 austinbrown   (501) staff       (20)     1356 2023-04-22 13:40:30.000000 placeholders-2.2/placeholders.egg-info/PKG-INFO
+-rw-r--r--   0 austinbrown   (501) staff       (20)      310 2023-04-22 13:40:30.000000 placeholders-2.2/placeholders.egg-info/SOURCES.txt
+-rw-r--r--   0 austinbrown   (501) staff       (20)        1 2023-04-22 13:40:30.000000 placeholders-2.2/placeholders.egg-info/dependency_links.txt
+-rw-r--r--   0 austinbrown   (501) staff       (20)       30 2023-04-22 13:40:30.000000 placeholders-2.2/placeholders.egg-info/requires.txt
+-rw-r--r--   0 austinbrown   (501) staff       (20)       13 2023-04-22 13:40:30.000000 placeholders-2.2/placeholders.egg-info/top_level.txt
+drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:40:30.919648 placeholders-2.2/scripts/
+-rwxr-xr-x   0 austinbrown   (501) staff       (20)     1101 2023-04-22 13:00:19.000000 placeholders-2.2/scripts/placeholders
+-rw-r--r--   0 austinbrown   (501) staff       (20)       38 2023-04-22 13:40:30.920247 placeholders-2.2/setup.cfg
+-rw-r--r--   0 austinbrown   (501) staff       (20)      719 2023-04-22 13:38:59.000000 placeholders-2.2/setup.py
```

### Comparing `placeholders-2.1/LICENSE` & `placeholders-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `placeholders-2.1/PKG-INFO` & `placeholders-2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: placeholders
-Version: 2.1
+Version: 2.2
 Summary: Create placeholder images by embedding keywords into regular jpg images.
 Home-page: https://github.com/austinbrown34/placeholders
 Author: Austin Brown
 Author-email: austinbrown34@gmail.com
 Keywords: image,exif,jpg
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `placeholders-2.1/README.md` & `placeholders-2.2/README.md`

 * *Files identical despite different names*

### Comparing `placeholders-2.1/placeholders/controls.py` & `placeholders-2.2/placeholders/controls.py`

 * *Files identical despite different names*

### Comparing `placeholders-2.1/placeholders/tools.py` & `placeholders-2.2/placeholders/tools.py`

 * *Files identical despite different names*

### Comparing `placeholders-2.1/placeholders.egg-info/PKG-INFO` & `placeholders-2.2/placeholders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: placeholders
-Version: 2.1
+Version: 2.2
 Summary: Create placeholder images by embedding keywords into regular jpg images.
 Home-page: https://github.com/austinbrown34/placeholders
 Author: Austin Brown
 Author-email: austinbrown34@gmail.com
 Keywords: image,exif,jpg
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `placeholders-2.1/scripts/placeholders` & `placeholders-2.2/scripts/placeholders`

 * *Files identical despite different names*

