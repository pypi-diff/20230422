# Comparing `tmp/pythesyncer-23.4.16.11.tar.gz` & `tmp/pythesyncer-23.4.22.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pythesyncer-23.4.16.11.tar", last modified: Sun Apr 16 03:04:45 2023, max compression
+gzip compressed data, was "dist/pythesyncer-23.4.22.13.tar", last modified: Sat Apr 22 05:03:12 2023, max compression
```

## Comparing `pythesyncer-23.4.16.11.tar` & `pythesyncer-23.4.22.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-04-16 03:04:45.070639 pythesyncer-23.4.16.11/
--rw-rw-r--   0 tp03      (1000) tp03      (1000)      434 2023-04-16 03:04:45.070639 pythesyncer-23.4.16.11/PKG-INFO
--rw-r--r--   0 tp03      (1000) tp03      (1000)       76 2023-04-14 11:29:59.000000 pythesyncer-23.4.16.11/README.md
-drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-04-16 03:04:45.070639 pythesyncer-23.4.16.11/pythesyncer/
--rw-r--r--   0 tp03      (1000) tp03      (1000)     3448 2023-04-16 03:03:05.000000 pythesyncer-23.4.16.11/pythesyncer/__init__.py
--rw-r--r--   0 tp03      (1000) tp03      (1000)     1469 2023-04-16 02:52:44.000000 pythesyncer-23.4.16.11/pythesyncer/auth.py
-drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-04-16 03:04:45.070639 pythesyncer-23.4.16.11/pythesyncer.egg-info/
--rw-rw-r--   0 tp03      (1000) tp03      (1000)      434 2023-04-16 03:04:44.000000 pythesyncer-23.4.16.11/pythesyncer.egg-info/PKG-INFO
--rw-rw-r--   0 tp03      (1000) tp03      (1000)      274 2023-04-16 03:04:45.000000 pythesyncer-23.4.16.11/pythesyncer.egg-info/SOURCES.txt
--rw-rw-r--   0 tp03      (1000) tp03      (1000)        1 2023-04-16 03:04:44.000000 pythesyncer-23.4.16.11/pythesyncer.egg-info/dependency_links.txt
--rw-rw-r--   0 tp03      (1000) tp03      (1000)       55 2023-04-16 03:04:44.000000 pythesyncer-23.4.16.11/pythesyncer.egg-info/entry_points.txt
--rw-rw-r--   0 tp03      (1000) tp03      (1000)       20 2023-04-16 03:04:44.000000 pythesyncer-23.4.16.11/pythesyncer.egg-info/requires.txt
--rw-rw-r--   0 tp03      (1000) tp03      (1000)       12 2023-04-16 03:04:44.000000 pythesyncer-23.4.16.11/pythesyncer.egg-info/top_level.txt
--rw-rw-r--   0 tp03      (1000) tp03      (1000)       38 2023-04-16 03:04:45.070639 pythesyncer-23.4.16.11/setup.cfg
--rw-r--r--   0 tp03      (1000) tp03      (1000)      864 2023-04-14 11:58:13.000000 pythesyncer-23.4.16.11/setup.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-04-22 05:03:12.103841 pythesyncer-23.4.22.13/
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      434 2023-04-22 05:03:12.099841 pythesyncer-23.4.22.13/PKG-INFO
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       76 2023-04-14 11:29:59.000000 pythesyncer-23.4.22.13/README.md
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-04-22 05:03:12.099841 pythesyncer-23.4.22.13/pythesyncer/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3449 2023-04-22 05:02:08.000000 pythesyncer-23.4.22.13/pythesyncer/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1469 2023-04-16 02:52:44.000000 pythesyncer-23.4.22.13/pythesyncer/auth.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-04-22 05:03:12.099841 pythesyncer-23.4.22.13/pythesyncer.egg-info/
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      434 2023-04-22 05:03:11.000000 pythesyncer-23.4.22.13/pythesyncer.egg-info/PKG-INFO
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      274 2023-04-22 05:03:12.000000 pythesyncer-23.4.22.13/pythesyncer.egg-info/SOURCES.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)        1 2023-04-22 05:03:11.000000 pythesyncer-23.4.22.13/pythesyncer.egg-info/dependency_links.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       55 2023-04-22 05:03:11.000000 pythesyncer-23.4.22.13/pythesyncer.egg-info/entry_points.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       20 2023-04-22 05:03:11.000000 pythesyncer-23.4.22.13/pythesyncer.egg-info/requires.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       12 2023-04-22 05:03:11.000000 pythesyncer-23.4.22.13/pythesyncer.egg-info/top_level.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       38 2023-04-22 05:03:12.103841 pythesyncer-23.4.22.13/setup.cfg
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      864 2023-04-14 11:58:13.000000 pythesyncer-23.4.22.13/setup.py
```

### Comparing `pythesyncer-23.4.16.11/pythesyncer/__init__.py` & `pythesyncer-23.4.22.13/pythesyncer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     file_name=cf.io.basename(obj)
     if os.path.isfile(obj):
         cf.info('Uploading file: {}'.format(obj))
         await asyncformer(upload_file, obj)
 
     elif os.path.isdir(obj):
         cf.info('Uploading dir: {}'.format(obj))
-        zipname = cf.random_string(7)
+        zipname = cf.random_string(16)
         zipfile = zipname+'.7z'
         os.system(
             '7z a -t7z -m0=lzma2 -mx=9 -mfb=64 -md=32m -ms=on {} {}'.
             format(zipfile, obj))
         await asyncformer(upload_file, zipfile)
         os.remove(zipfile)
         cf.info("Upload done: {}".format(zipfile))
```

### Comparing `pythesyncer-23.4.16.11/pythesyncer/auth.py` & `pythesyncer-23.4.22.13/pythesyncer/auth.py`

 * *Files identical despite different names*

### Comparing `pythesyncer-23.4.16.11/setup.py` & `pythesyncer-23.4.22.13/setup.py`

 * *Files identical despite different names*

