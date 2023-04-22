# Comparing `tmp/vmt-0.0.0b3.tar.gz` & `tmp/vmt-0.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmt-0.0.0b3.tar", last modified: Fri Apr 14 00:50:16 2023, max compression
+gzip compressed data, was "vmt-0.0.0b4.tar", last modified: Sat Apr 22 06:00:30 2023, max compression
```

## Comparing `vmt-0.0.0b3.tar` & `vmt-0.0.0b4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:50:16.003606 vmt-0.0.0b3/
--rw-r--r--   0 anon      (1000) wheel      (998)    34742 2022-07-14 19:37:15.000000 vmt-0.0.0b3/LICENSE
--rw-r--r--   0 anon      (1000) wheel      (998)    10185 2023-04-14 00:50:16.003606 vmt-0.0.0b3/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)     9847 2022-09-22 03:13:29.000000 vmt-0.0.0b3/README.md
--rw-r--r--   0 anon      (1000) wheel      (998)      570 2023-04-14 00:49:38.000000 vmt-0.0.0b3/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-14 00:50:16.003606 vmt-0.0.0b3/setup.cfg
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:50:16.000273 vmt-0.0.0b3/src/
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:50:16.000273 vmt-0.0.0b3/src/vmt/
--rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 vmt-0.0.0b3/src/vmt/__init__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1628 2022-09-22 02:48:23.000000 vmt-0.0.0b3/src/vmt/__main__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     6218 2022-09-22 02:48:23.000000 vmt-0.0.0b3/src/vmt/build.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     6315 2022-09-22 02:48:23.000000 vmt-0.0.0b3/src/vmt/config.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 vmt-0.0.0b3/src/vmt/initial_setup.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     3371 2022-09-22 02:48:23.000000 vmt-0.0.0b3/src/vmt/media.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     4987 2022-07-11 05:05:28.000000 vmt-0.0.0b3/src/vmt/options.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1615 2023-04-14 00:28:04.000000 vmt-0.0.0b3/src/vmt/prompts.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2250 2022-09-22 02:48:23.000000 vmt-0.0.0b3/src/vmt/search.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1070 2022-10-09 04:34:45.000000 vmt-0.0.0b3/src/vmt/system.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2091 2022-09-22 02:48:23.000000 vmt-0.0.0b3/src/vmt/utils.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:50:16.003606 vmt-0.0.0b3/src/vmt.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)    10185 2023-04-14 00:50:15.000000 vmt-0.0.0b3/src/vmt.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      428 2023-04-14 00:50:15.000000 vmt-0.0.0b3/src/vmt.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-14 00:50:15.000000 vmt-0.0.0b3/src/vmt.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       42 2023-04-14 00:50:15.000000 vmt-0.0.0b3/src/vmt.egg-info/entry_points.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       37 2023-04-14 00:50:15.000000 vmt-0.0.0b3/src/vmt.egg-info/requires.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        4 2023-04-14 00:50:15.000000 vmt-0.0.0b3/src/vmt.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-22 06:00:30.879650 vmt-0.0.0b4/
+-rw-r--r--   0 anon      (1000) wheel      (998)    34742 2022-07-14 19:37:15.000000 vmt-0.0.0b4/LICENSE
+-rw-r--r--   0 anon      (1000) wheel      (998)    10185 2023-04-22 06:00:30.879650 vmt-0.0.0b4/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)     9847 2022-09-22 03:13:29.000000 vmt-0.0.0b4/README.md
+-rw-r--r--   0 anon      (1000) wheel      (998)      570 2023-04-22 05:54:45.000000 vmt-0.0.0b4/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-22 06:00:30.879650 vmt-0.0.0b4/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-22 06:00:30.876316 vmt-0.0.0b4/src/
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-22 06:00:30.879650 vmt-0.0.0b4/src/vmt/
+-rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 vmt-0.0.0b4/src/vmt/__init__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1628 2022-09-22 02:48:23.000000 vmt-0.0.0b4/src/vmt/__main__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     6218 2022-09-22 02:48:23.000000 vmt-0.0.0b4/src/vmt/build.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     6315 2022-09-22 02:48:23.000000 vmt-0.0.0b4/src/vmt/config.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 vmt-0.0.0b4/src/vmt/initial_setup.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     3371 2022-09-22 02:48:23.000000 vmt-0.0.0b4/src/vmt/media.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     4987 2022-07-11 05:05:28.000000 vmt-0.0.0b4/src/vmt/options.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1669 2023-04-22 05:55:06.000000 vmt-0.0.0b4/src/vmt/prompts.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2250 2022-09-22 02:48:23.000000 vmt-0.0.0b4/src/vmt/search.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1070 2022-10-09 04:34:45.000000 vmt-0.0.0b4/src/vmt/system.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2091 2022-09-22 02:48:23.000000 vmt-0.0.0b4/src/vmt/utils.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-22 06:00:30.879650 vmt-0.0.0b4/src/vmt.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)    10185 2023-04-22 06:00:30.000000 vmt-0.0.0b4/src/vmt.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      428 2023-04-22 06:00:30.000000 vmt-0.0.0b4/src/vmt.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-22 06:00:30.000000 vmt-0.0.0b4/src/vmt.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       42 2023-04-22 06:00:30.000000 vmt-0.0.0b4/src/vmt.egg-info/entry_points.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       37 2023-04-22 06:00:30.000000 vmt-0.0.0b4/src/vmt.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        4 2023-04-22 06:00:30.000000 vmt-0.0.0b4/src/vmt.egg-info/top_level.txt
```

### Comparing `vmt-0.0.0b3/LICENSE` & `vmt-0.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b3/PKG-INFO` & `vmt-0.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmt
-Version: 0.0.0b3
+Version: 0.0.0b4
 Summary: Video Media Tracker. Local, and simple method for watching and tracking a video media library.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/vmt
 Keywords: mpv
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `vmt-0.0.0b3/README.md` & `vmt-0.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b3/pyproject.toml` & `vmt-0.0.0b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vmt"
-version = "0.0.0.b3"
+version = "0.0.0.b4"
 description = "Video Media Tracker. Local, and simple method for watching and tracking a video media library."
 readme = "README.md"
 license = { text = "GNU General Public License v3 (GPLv3)" }
 keywords = [ "mpv" ]
 dependencies = [
     "python-magic",
     "loadconf",
```

### Comparing `vmt-0.0.0b3/src/vmt/__main__.py` & `vmt-0.0.0b4/src/vmt/__main__.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b3/src/vmt/build.py` & `vmt-0.0.0b4/src/vmt/build.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b3/src/vmt/config.py` & `vmt-0.0.0b4/src/vmt/config.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b3/src/vmt/media.py` & `vmt-0.0.0b4/src/vmt/media.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b3/src/vmt/options.py` & `vmt-0.0.0b4/src/vmt/options.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b3/src/vmt/prompts.py` & `vmt-0.0.0b4/src/vmt/prompts.py`

 * *Files 20% similar despite different names*

```diff
@@ -60,8 +60,11 @@
 
     choice = p.ask(
         options=options,
         prompt=prompt,
         additional_args=cmd_args,
     )
 
-    return choice[0]
+    try:
+        return choice[0]
+    except IndexError:
+        return []
```

### Comparing `vmt-0.0.0b3/src/vmt/search.py` & `vmt-0.0.0b4/src/vmt/search.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b3/src/vmt/system.py` & `vmt-0.0.0b4/src/vmt/system.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b3/src/vmt/utils.py` & `vmt-0.0.0b4/src/vmt/utils.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b3/src/vmt.egg-info/PKG-INFO` & `vmt-0.0.0b4/src/vmt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmt
-Version: 0.0.0b3
+Version: 0.0.0b4
 Summary: Video Media Tracker. Local, and simple method for watching and tracking a video media library.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/vmt
 Keywords: mpv
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

