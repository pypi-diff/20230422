# Comparing `tmp/mrdoxmrgt-0.0.7.tar.gz` & `tmp/mrdoxmrgt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrdoxmrgt-0.0.7.tar", last modified: Sat Apr 22 06:29:41 2023, max compression
+gzip compressed data, was "mrdoxmrgt-0.0.8.tar", last modified: Sat Apr 22 06:35:08 2023, max compression
```

## Comparing `mrdoxmrgt-0.0.7.tar` & `mrdoxmrgt-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 06:29:42.000000 mrdoxmrgt-0.0.7/
--rw-rw-rw-   0        0        0     1083 2023-04-20 14:15:02.000000 mrdoxmrgt-0.0.7/LICENCE
--rw-rw-rw-   0        0        0      810 2023-04-22 06:29:42.000000 mrdoxmrgt-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-04-20 14:15:34.000000 mrdoxmrgt-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 06:29:42.000000 mrdoxmrgt-0.0.7/mrdoxmrgt/
-drwxrwxrwx   0        0        0        0 2023-04-22 06:29:42.000000 mrdoxmrgt-0.0.7/mrdoxmrgt/GTF/
--rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.7/mrdoxmrgt/GTF/__init__.py
--rw-rw-rw-   0        0        0     3192 2023-04-22 06:26:56.000000 mrdoxmrgt-0.0.7/mrdoxmrgt/GTF/install.py
--rw-rw-rw-   0        0        0     1392 2023-04-22 05:22:14.000000 mrdoxmrgt-0.0.7/mrdoxmrgt/GTF/run.py
--rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.7/mrdoxmrgt/__init__.py
--rw-rw-rw-   0        0        0     2576 2023-04-22 06:28:24.000000 mrdoxmrgt-0.0.7/mrdoxmrgt/_main_.py
-drwxrwxrwx   0        0        0        0 2023-04-22 06:29:42.000000 mrdoxmrgt-0.0.7/mrdoxmrgt.egg-info/
--rw-rw-rw-   0        0        0      810 2023-04-22 06:29:42.000000 mrdoxmrgt-0.0.7/mrdoxmrgt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-04-22 06:29:42.000000 mrdoxmrgt-0.0.7/mrdoxmrgt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 06:29:42.000000 mrdoxmrgt-0.0.7/mrdoxmrgt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-22 06:29:42.000000 mrdoxmrgt-0.0.7/mrdoxmrgt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-22 06:29:42.000000 mrdoxmrgt-0.0.7/mrdoxmrgt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-22 06:29:42.000000 mrdoxmrgt-0.0.7/mrdoxmrgt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 06:29:42.000000 mrdoxmrgt-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1243 2023-04-22 06:28:32.000000 mrdoxmrgt-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/
+-rw-rw-rw-   0        0        0     1083 2023-04-20 14:15:02.000000 mrdoxmrgt-0.0.8/LICENCE
+-rw-rw-rw-   0        0        0      810 2023-04-22 06:35:10.000000 mrdoxmrgt-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-04-20 14:15:34.000000 mrdoxmrgt-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt/
+drwxrwxrwx   0        0        0        0 2023-04-22 06:35:10.000000 mrdoxmrgt-0.0.8/mrdoxmrgt/GTF/
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.8/mrdoxmrgt/GTF/__init__.py
+-rw-rw-rw-   0        0        0     3192 2023-04-22 06:26:56.000000 mrdoxmrgt-0.0.8/mrdoxmrgt/GTF/install.py
+-rw-rw-rw-   0        0        0     1392 2023-04-22 05:22:14.000000 mrdoxmrgt-0.0.8/mrdoxmrgt/GTF/run.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.8/mrdoxmrgt/__init__.py
+-rw-rw-rw-   0        0        0     2542 2023-04-22 06:34:40.000000 mrdoxmrgt-0.0.8/mrdoxmrgt/_main_.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/
+-rw-rw-rw-   0        0        0      810 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-22 06:35:08.000000 mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 06:35:10.000000 mrdoxmrgt-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2023-04-22 06:34:46.000000 mrdoxmrgt-0.0.8/setup.py
```

### Comparing `mrdoxmrgt-0.0.7/LICENCE` & `mrdoxmrgt-0.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.7/PKG-INFO` & `mrdoxmrgt-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/SMS_Forwarder
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.0.7/mrdoxmrgt/GTF/install.py` & `mrdoxmrgt-0.0.8/mrdoxmrgt/GTF/install.py`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.7/mrdoxmrgt/GTF/run.py` & `mrdoxmrgt-0.0.8/mrdoxmrgt/GTF/run.py`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.7/mrdoxmrgt/_main_.py` & `mrdoxmrgt-0.0.8/mrdoxmrgt/_main_.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,15 @@
 
 
 
 
 
 
 def main():
-    try: version = requests.get("https://raw.githubusercontent.com/GreyTechno/gtf/main/.info").json()["version"]
-    except: version = __VERSION__
-    if (__VERSION__ != version): Release()
+    
 
     try: command = sys.argv[1]
     except: command = False
 
     try: arguments = sys.argv[2]
     except: arguments = ""
 
@@ -78,8 +76,10 @@
             run.Run(arguments)
         # elif (command == "list") or (command == "-list") or (command == "--list"): print("list")
         # elif (command == "about") or (command == "-about") or (command == "--about"): pass
         # elif (command == "show") or (command == "-show") or (command == "--show"): pass
         # elif (command == "help") or (command == "-help") or (command == "--help"): pass
         else: print(f"ERROR : Command not found '{command}'\nShow help 'gtf -h'")
 if __name__ == "__main__":
+    version = requests.get("https://raw.githubusercontent.com/GreyTechno/gtf/main/.info").json()["version"]
+    if (__VERSION__ != version): Release()
     main()
```

### Comparing `mrdoxmrgt-0.0.7/mrdoxmrgt.egg-info/PKG-INFO` & `mrdoxmrgt-0.0.8/mrdoxmrgt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/SMS_Forwarder
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.0.7/setup.py` & `mrdoxmrgt-0.0.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mrdoxmrgt',
     packages=find_packages(),
     include_package_data=True,
-    version="0.0.7",
+    version="0.0.8",
     description='A small example package',
     long_description="A small example package HI",
     long_description_content_type="text/markdown",
     author='MR_GT',
     author_email='friendyt89@gmail.com',
     url='https://github.com/GreyTechno/SMS_Forwarder',
     download_url="https://github.com/GreyTechno/gtf/archive/pypi.zip",
```

