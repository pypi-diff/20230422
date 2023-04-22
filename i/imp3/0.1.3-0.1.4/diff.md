# Comparing `tmp/imp3-0.1.3.tar.gz` & `tmp/imp3-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imp3-0.1.3.tar", last modified: Sat Apr 22 12:50:02 2023, max compression
+gzip compressed data, was "imp3-0.1.4.tar", last modified: Sat Apr 22 13:39:26 2023, max compression
```

## Comparing `imp3-0.1.3.tar` & `imp3-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:50:02.643622 imp3-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-22 12:49:26.000000 imp3-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-22 12:50:02.643622 imp3-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-22 12:49:26.000000 imp3-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:50:02.639621 imp3-0.1.3/imp3/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 12:49:26.000000 imp3-0.1.3/imp3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23896 2023-04-22 12:49:26.000000 imp3-0.1.3/imp3/app.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:49:26.000000 imp3-0.1.3/imp3/cleaning_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-22 12:49:26.000000 imp3-0.1.3/imp3/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:50:02.643622 imp3-0.1.3/imp3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-22 12:50:02.000000 imp3-0.1.3/imp3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-22 12:50:02.000000 imp3-0.1.3/imp3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 12:50:02.000000 imp3-0.1.3/imp3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 12:50:02.000000 imp3-0.1.3/imp3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 12:50:02.000000 imp3-0.1.3/imp3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-22 12:50:02.000000 imp3-0.1.3/imp3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 12:50:02.000000 imp3-0.1.3/imp3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 12:50:02.643622 imp3-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-22 12:49:26.000000 imp3-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:50:02.643622 imp3-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:49:26.000000 imp3-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-22 12:49:26.000000 imp3-0.1.3/tests/unit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:39:26.496518 imp3-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-22 13:38:53.000000 imp3-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-22 13:39:26.492518 imp3-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-22 13:38:53.000000 imp3-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:39:26.492518 imp3-0.1.4/imp3/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 13:38:53.000000 imp3-0.1.4/imp3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23896 2023-04-22 13:38:53.000000 imp3-0.1.4/imp3/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 13:38:53.000000 imp3-0.1.4/imp3/cleaning_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-22 13:38:53.000000 imp3-0.1.4/imp3/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:39:26.492518 imp3-0.1.4/imp3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-22 13:39:26.000000 imp3-0.1.4/imp3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-22 13:39:26.000000 imp3-0.1.4/imp3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 13:39:26.000000 imp3-0.1.4/imp3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 13:39:26.000000 imp3-0.1.4/imp3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 13:39:26.000000 imp3-0.1.4/imp3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-22 13:39:26.000000 imp3-0.1.4/imp3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 13:39:26.000000 imp3-0.1.4/imp3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 13:39:26.496518 imp3-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-22 13:38:53.000000 imp3-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:39:26.492518 imp3-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 13:38:53.000000 imp3-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-22 13:38:53.000000 imp3-0.1.4/tests/unit_test.py
```

### Comparing `imp3-0.1.3/LICENSE` & `imp3-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `imp3-0.1.3/PKG-INFO` & `imp3-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imp3
-Version: 0.1.3
+Version: 0.1.4
 Summary: Interactive tool for image pre-processing and automated pipeline creation
 Home-page: https://github.com/bokey007/imp3
 Author: Sudhir Arvind Deshmukh
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # imp3 (Image pre-preocessing pipeline) :
@@ -27,16 +27,15 @@
 
 ```bash
 imp3.run --port 8080
 ```
 Above command can be used to specify the port on which you want to run the app.
 
 ## UI
-add video 
-![alt text](https://github.com/bokey007/imp3/blob/main/media/demo.gif)
+![](https://github.com/bokey007/imp3/blob/main/media/demo.png)
 
 # Following is the list of currently supported operations:
 
 ## 0. Resize input image
 
 ## 1. map the image to different color spaces
     Folowwing methods are available:
```

### Comparing `imp3-0.1.3/README.md` & `imp3-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 
 ```bash
 imp3.run --port 8080
 ```
 Above command can be used to specify the port on which you want to run the app.
 
 ## UI
-add video 
-![alt text](https://github.com/bokey007/imp3/blob/main/media/demo.gif)
+![](https://github.com/bokey007/imp3/blob/main/media/demo.png)
 
 # Following is the list of currently supported operations:
 
 ## 0. Resize input image
 
 ## 1. map the image to different color spaces
     Folowwing methods are available:
```

### Comparing `imp3-0.1.3/imp3/app.py` & `imp3-0.1.4/imp3/app.py`

 * *Files identical despite different names*

### Comparing `imp3-0.1.3/imp3/run.py` & `imp3-0.1.4/imp3/run.py`

 * *Files identical despite different names*

### Comparing `imp3-0.1.3/imp3.egg-info/PKG-INFO` & `imp3-0.1.4/imp3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imp3
-Version: 0.1.3
+Version: 0.1.4
 Summary: Interactive tool for image pre-processing and automated pipeline creation
 Home-page: https://github.com/bokey007/imp3
 Author: Sudhir Arvind Deshmukh
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # imp3 (Image pre-preocessing pipeline) :
@@ -27,16 +27,15 @@
 
 ```bash
 imp3.run --port 8080
 ```
 Above command can be used to specify the port on which you want to run the app.
 
 ## UI
-add video 
-![alt text](https://github.com/bokey007/imp3/blob/main/media/demo.gif)
+![](https://github.com/bokey007/imp3/blob/main/media/demo.png)
 
 # Following is the list of currently supported operations:
 
 ## 0. Resize input image
 
 ## 1. map the image to different color spaces
     Folowwing methods are available:
```

### Comparing `imp3-0.1.3/setup.py` & `imp3-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #     install_requires = f.read().splitlines()
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='imp3',
-    version='0.1.3',
+    version='0.1.4',
     author='Sudhir Arvind Deshmukh',
     description='Interactive tool for image pre-processing and automated pipeline creation',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/bokey007/imp3',
     packages=find_packages(),
     install_requires=[
```

