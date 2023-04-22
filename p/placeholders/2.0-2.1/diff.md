# Comparing `tmp/placeholders-2.0.tar.gz` & `tmp/placeholders-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "placeholders-2.0.tar", last modified: Sat Apr 22 13:00:28 2023, max compression
+gzip compressed data, was "placeholders-2.1.tar", last modified: Sat Apr 22 13:20:47 2023, max compression
```

## Comparing `placeholders-2.0.tar` & `placeholders-2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:00:28.240896 placeholders-2.0/
--rw-r--r--   0 austinbrown   (501) staff       (20)     1074 2023-04-22 12:00:08.000000 placeholders-2.0/LICENSE
--rw-r--r--   0 austinbrown   (501) staff       (20)        0 2023-04-22 12:00:25.000000 placeholders-2.0/MANIFEST.in
--rw-r--r--   0 austinbrown   (501) staff       (20)     1356 2023-04-22 13:00:28.240748 placeholders-2.0/PKG-INFO
--rw-r--r--   0 austinbrown   (501) staff       (20)     1016 2023-04-22 12:59:04.000000 placeholders-2.0/README.md
-drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:00:28.239392 placeholders-2.0/placeholders/
--rw-r--r--   0 austinbrown   (501) staff       (20)        0 2023-04-22 11:33:55.000000 placeholders-2.0/placeholders/__init__.py
--rw-r--r--   0 austinbrown   (501) staff       (20)      833 2023-04-22 12:34:40.000000 placeholders-2.0/placeholders/controls.py
--rw-r--r--   0 austinbrown   (501) staff       (20)     2118 2023-04-22 11:45:07.000000 placeholders-2.0/placeholders/tools.py
-drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:00:28.240320 placeholders-2.0/placeholders.egg-info/
--rw-r--r--   0 austinbrown   (501) staff       (20)     1356 2023-04-22 13:00:28.000000 placeholders-2.0/placeholders.egg-info/PKG-INFO
--rw-r--r--   0 austinbrown   (501) staff       (20)      310 2023-04-22 13:00:28.000000 placeholders-2.0/placeholders.egg-info/SOURCES.txt
--rw-r--r--   0 austinbrown   (501) staff       (20)        1 2023-04-22 13:00:28.000000 placeholders-2.0/placeholders.egg-info/dependency_links.txt
--rw-r--r--   0 austinbrown   (501) staff       (20)       14 2023-04-22 13:00:28.000000 placeholders-2.0/placeholders.egg-info/requires.txt
--rw-r--r--   0 austinbrown   (501) staff       (20)       13 2023-04-22 13:00:28.000000 placeholders-2.0/placeholders.egg-info/top_level.txt
-drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:00:28.240532 placeholders-2.0/scripts/
--rwxr-xr-x   0 austinbrown   (501) staff       (20)     1101 2023-04-22 13:00:19.000000 placeholders-2.0/scripts/placeholders
--rw-r--r--   0 austinbrown   (501) staff       (20)       38 2023-04-22 13:00:28.240949 placeholders-2.0/setup.cfg
--rw-r--r--   0 austinbrown   (501) staff       (20)      681 2023-04-22 12:20:02.000000 placeholders-2.0/setup.py
+drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:20:47.711733 placeholders-2.1/
+-rw-r--r--   0 austinbrown   (501) staff       (20)     1074 2023-04-22 12:00:08.000000 placeholders-2.1/LICENSE
+-rw-r--r--   0 austinbrown   (501) staff       (20)        0 2023-04-22 12:00:25.000000 placeholders-2.1/MANIFEST.in
+-rw-r--r--   0 austinbrown   (501) staff       (20)     1356 2023-04-22 13:20:47.711383 placeholders-2.1/PKG-INFO
+-rw-r--r--   0 austinbrown   (501) staff       (20)     1016 2023-04-22 12:59:04.000000 placeholders-2.1/README.md
+drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:20:47.701770 placeholders-2.1/placeholders/
+-rw-r--r--   0 austinbrown   (501) staff       (20)        0 2023-04-22 11:33:55.000000 placeholders-2.1/placeholders/__init__.py
+-rw-r--r--   0 austinbrown   (501) staff       (20)      976 2023-04-22 13:03:08.000000 placeholders-2.1/placeholders/controls.py
+-rw-r--r--   0 austinbrown   (501) staff       (20)     2118 2023-04-22 11:45:07.000000 placeholders-2.1/placeholders/tools.py
+drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:20:47.703812 placeholders-2.1/placeholders.egg-info/
+-rw-r--r--   0 austinbrown   (501) staff       (20)     1356 2023-04-22 13:20:47.000000 placeholders-2.1/placeholders.egg-info/PKG-INFO
+-rw-r--r--   0 austinbrown   (501) staff       (20)      310 2023-04-22 13:20:47.000000 placeholders-2.1/placeholders.egg-info/SOURCES.txt
+-rw-r--r--   0 austinbrown   (501) staff       (20)        1 2023-04-22 13:20:47.000000 placeholders-2.1/placeholders.egg-info/dependency_links.txt
+-rw-r--r--   0 austinbrown   (501) staff       (20)      478 2023-04-22 13:20:47.000000 placeholders-2.1/placeholders.egg-info/requires.txt
+-rw-r--r--   0 austinbrown   (501) staff       (20)       13 2023-04-22 13:20:47.000000 placeholders-2.1/placeholders.egg-info/top_level.txt
+drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:20:47.704090 placeholders-2.1/scripts/
+-rwxr-xr-x   0 austinbrown   (501) staff       (20)     1101 2023-04-22 13:00:19.000000 placeholders-2.1/scripts/placeholders
+-rw-r--r--   0 austinbrown   (501) staff       (20)       38 2023-04-22 13:20:47.711813 placeholders-2.1/setup.cfg
+-rw-r--r--   0 austinbrown   (501) staff       (20)     1441 2023-04-22 13:20:25.000000 placeholders-2.1/setup.py
```

### Comparing `placeholders-2.0/LICENSE` & `placeholders-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `placeholders-2.0/PKG-INFO` & `placeholders-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: placeholders
-Version: 2.0
+Version: 2.1
 Summary: Create placeholder images by embedding keywords into regular jpg images.
 Home-page: https://github.com/austinbrown34/placeholders
 Author: Austin Brown
 Author-email: austinbrown34@gmail.com
 Keywords: image,exif,jpg
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `placeholders-2.0/README.md` & `placeholders-2.1/README.md`

 * *Files identical despite different names*

### Comparing `placeholders-2.0/placeholders/controls.py` & `placeholders-2.1/placeholders/controls.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,16 +7,20 @@
 warnings.filterwarnings("ignore")
 
 def set_tags(f):
     def_file = open(f)
     definitions = yaml.safe_load(def_file)
     def_file.close()
     for file, tag in definitions.items():
+        if os.path.isabs(file):
+            full_path = file
+        else:
+            full_path = os.path.join(os.path.dirname(f), file)
         pt.set_image_tag(
-            file,
+            full_path,
             tag
         )    
             
     print("Complete!")
     return
 
 def set_tag(f, t):
```

### Comparing `placeholders-2.0/placeholders/tools.py` & `placeholders-2.1/placeholders/tools.py`

 * *Files identical despite different names*

### Comparing `placeholders-2.0/placeholders.egg-info/PKG-INFO` & `placeholders-2.1/placeholders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: placeholders
-Version: 2.0
+Version: 2.1
 Summary: Create placeholder images by embedding keywords into regular jpg images.
 Home-page: https://github.com/austinbrown34/placeholders
 Author: Austin Brown
 Author-email: austinbrown34@gmail.com
 Keywords: image,exif,jpg
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `placeholders-2.0/scripts/placeholders` & `placeholders-2.1/scripts/placeholders`

 * *Files identical despite different names*

