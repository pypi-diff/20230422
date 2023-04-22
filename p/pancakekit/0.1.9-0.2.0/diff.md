# Comparing `tmp/pancakekit-0.1.9.tar.gz` & `tmp/pancakekit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pancakekit-0.1.9.tar", last modified: Wed Mar  8 13:55:35 2023, max compression
+gzip compressed data, was "pancakekit-0.2.0.tar", last modified: Sat Apr 22 14:51:43 2023, max compression
```

## Comparing `pancakekit-0.1.9.tar` & `pancakekit-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-03-08 13:55:35.760665 pancakekit-0.1.9/
--rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2022-12-09 15:15:03.000000 pancakekit-0.1.9/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       77 2022-12-09 19:43:44.000000 pancakekit-0.1.9/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)     1924 2023-03-08 13:55:35.760731 pancakekit-0.1.9/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)     9017 2022-12-13 16:59:16.000000 pancakekit-0.1.9/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)      940 2022-12-13 17:09:19.000000 pancakekit-0.1.9/README_pypi.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2022-12-09 18:59:58.000000 pancakekit-0.1.9/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)     1105 2023-03-08 13:55:35.761013 pancakekit-0.1.9/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 pancakekit-0.1.9/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-03-08 13:55:35.751208 pancakekit-0.1.9/src/
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-03-08 13:55:35.754163 pancakekit-0.1.9/src/pancakekit/
--rw-r--r--   0 shuntaro   (501) staff       (20)      430 2022-12-13 13:08:50.000000 pancakekit-0.1.9/src/pancakekit/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)      416 2022-12-09 11:01:03.000000 pancakekit-0.1.9/src/pancakekit/__main__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)       21 2022-12-10 02:52:48.000000 pancakekit-0.1.9/src/pancakekit/_version.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-03-08 13:55:35.755977 pancakekit-0.1.9/src/pancakekit/basecomponent/
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:20:37.000000 pancakekit-0.1.9/src/pancakekit/basecomponent/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     1604 2022-12-03 16:28:54.000000 pancakekit-0.1.9/src/pancakekit/basecomponent/navigation.py
--rw-r--r--   0 shuntaro   (501) staff       (20)    55156 2023-03-08 13:54:03.000000 pancakekit-0.1.9/src/pancakekit/pancakekit.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-03-08 13:55:35.751474 pancakekit-0.1.9/src/pancakekit/static/
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-03-08 13:55:35.756861 pancakekit-0.1.9/src/pancakekit/static/css/
--rw-r--r--   0 shuntaro   (501) staff       (20)     3656 2021-08-28 08:52:02.000000 pancakekit-0.1.9/src/pancakekit/static/css/pancake.css
--rw-r--r--   0 shuntaro   (501) staff       (20)    23661 2021-06-15 06:07:03.000000 pancakekit-0.1.9/src/pancakekit/static/css/w3.css
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-03-08 13:55:35.758048 pancakekit-0.1.9/src/pancakekit/static/js/
--rw-r--r--   0 shuntaro   (501) staff       (20)     1881 2021-08-28 08:54:41.000000 pancakekit-0.1.9/src/pancakekit/static/js/draggable.js
--rw-r--r--   0 shuntaro   (501) staff       (20)    10104 2022-12-06 07:15:07.000000 pancakekit-0.1.9/src/pancakekit/static/js/main.js
--rw-r--r--   0 shuntaro   (501) staff       (20)     1222 2022-12-05 05:58:32.000000 pancakekit-0.1.9/src/pancakekit/static/js/run_script.js
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-03-08 13:55:35.759859 pancakekit-0.1.9/src/pancakekit/toppings/
--rw-r--r--   0 shuntaro   (501) staff       (20)      237 2022-12-11 12:23:12.000000 pancakekit-0.1.9/src/pancakekit/toppings/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     4158 2022-12-13 16:19:22.000000 pancakekit-0.1.9/src/pancakekit/toppings/automatic.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     9480 2022-12-21 13:47:42.000000 pancakekit-0.1.9/src/pancakekit/toppings/basic.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     3075 2022-12-11 12:18:30.000000 pancakekit-0.1.9/src/pancakekit/toppings/image.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     2877 2022-12-11 12:23:04.000000 pancakekit-0.1.9/src/pancakekit/toppings/nparray.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     2793 2022-12-12 03:15:55.000000 pancakekit-0.1.9/src/pancakekit/toppings/table.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-03-08 13:55:35.760430 pancakekit-0.1.9/src/pancakekit/utils/
--rw-r--r--   0 shuntaro   (501) staff       (20)      358 2022-12-12 02:27:44.000000 pancakekit-0.1.9/src/pancakekit/utils/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     3404 2022-12-12 02:27:13.000000 pancakekit-0.1.9/src/pancakekit/utils/utils.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-03-08 13:55:35.755605 pancakekit-0.1.9/src/pancakekit.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)     1924 2023-03-08 13:55:35.000000 pancakekit-0.1.9/src/pancakekit.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      916 2023-03-08 13:55:35.000000 pancakekit-0.1.9/src/pancakekit.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-03-08 13:55:35.000000 pancakekit-0.1.9/src/pancakekit.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       35 2023-03-08 13:55:35.000000 pancakekit-0.1.9/src/pancakekit.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       11 2023-03-08 13:55:35.000000 pancakekit-0.1.9/src/pancakekit.egg-info/top_level.txt
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-04-22 14:51:43.416935 pancakekit-0.2.0/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2022-12-09 15:15:03.000000 pancakekit-0.2.0/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       77 2022-12-09 19:43:44.000000 pancakekit-0.2.0/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2054 2023-04-22 14:51:43.417003 pancakekit-0.2.0/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)     9146 2023-04-22 14:49:51.000000 pancakekit-0.2.0/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1070 2023-04-22 14:50:00.000000 pancakekit-0.2.0/README_pypi.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2022-12-09 18:59:58.000000 pancakekit-0.2.0/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1105 2023-04-22 14:51:43.417354 pancakekit-0.2.0/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 pancakekit-0.2.0/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-04-22 14:51:43.408146 pancakekit-0.2.0/src/
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-04-22 14:51:43.410689 pancakekit-0.2.0/src/pancakekit/
+-rw-r--r--   0 shuntaro   (501) staff       (20)      430 2022-12-13 13:08:50.000000 pancakekit-0.2.0/src/pancakekit/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)      992 2023-04-22 14:38:40.000000 pancakekit-0.2.0/src/pancakekit/__main__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)       21 2022-12-10 02:52:48.000000 pancakekit-0.2.0/src/pancakekit/_version.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-04-22 14:51:43.412353 pancakekit-0.2.0/src/pancakekit/basecomponent/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:20:37.000000 pancakekit-0.2.0/src/pancakekit/basecomponent/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1604 2022-12-03 16:28:54.000000 pancakekit-0.2.0/src/pancakekit/basecomponent/navigation.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)    55156 2023-03-08 13:54:03.000000 pancakekit-0.2.0/src/pancakekit/pancakekit.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-04-22 14:51:43.408420 pancakekit-0.2.0/src/pancakekit/static/
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-04-22 14:51:43.413094 pancakekit-0.2.0/src/pancakekit/static/css/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     3656 2021-08-28 08:52:02.000000 pancakekit-0.2.0/src/pancakekit/static/css/pancake.css
+-rw-r--r--   0 shuntaro   (501) staff       (20)    23661 2021-06-15 06:07:03.000000 pancakekit-0.2.0/src/pancakekit/static/css/w3.css
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-04-22 14:51:43.414436 pancakekit-0.2.0/src/pancakekit/static/js/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1881 2021-08-28 08:54:41.000000 pancakekit-0.2.0/src/pancakekit/static/js/draggable.js
+-rw-r--r--   0 shuntaro   (501) staff       (20)    10104 2022-12-06 07:15:07.000000 pancakekit-0.2.0/src/pancakekit/static/js/main.js
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1222 2022-12-05 05:58:32.000000 pancakekit-0.2.0/src/pancakekit/static/js/run_script.js
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-04-22 14:51:43.416076 pancakekit-0.2.0/src/pancakekit/toppings/
+-rw-r--r--   0 shuntaro   (501) staff       (20)      237 2022-12-11 12:23:12.000000 pancakekit-0.2.0/src/pancakekit/toppings/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     4158 2022-12-13 16:19:22.000000 pancakekit-0.2.0/src/pancakekit/toppings/automatic.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     9480 2022-12-21 13:47:42.000000 pancakekit-0.2.0/src/pancakekit/toppings/basic.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     3075 2022-12-11 12:18:30.000000 pancakekit-0.2.0/src/pancakekit/toppings/image.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2877 2022-12-11 12:23:04.000000 pancakekit-0.2.0/src/pancakekit/toppings/nparray.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2793 2022-12-12 03:15:55.000000 pancakekit-0.2.0/src/pancakekit/toppings/table.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-04-22 14:51:43.416686 pancakekit-0.2.0/src/pancakekit/utils/
+-rw-r--r--   0 shuntaro   (501) staff       (20)      358 2022-12-12 02:27:44.000000 pancakekit-0.2.0/src/pancakekit/utils/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     3404 2022-12-12 02:27:13.000000 pancakekit-0.2.0/src/pancakekit/utils/utils.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-04-22 14:51:43.411946 pancakekit-0.2.0/src/pancakekit.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2054 2023-04-22 14:51:43.000000 pancakekit-0.2.0/src/pancakekit.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      916 2023-04-22 14:51:43.000000 pancakekit-0.2.0/src/pancakekit.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-04-22 14:51:43.000000 pancakekit-0.2.0/src/pancakekit.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       35 2023-04-22 14:51:43.000000 pancakekit-0.2.0/src/pancakekit.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       11 2023-04-22 14:51:43.000000 pancakekit-0.2.0/src/pancakekit.egg-info/top_level.txt
```

### Comparing `pancakekit-0.1.9/LICENSE.txt` & `pancakekit-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pancakekit-0.1.9/PKG-INFO` & `pancakekit-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pancakekit
-Version: 0.1.9
+Version: 0.2.0
 Summary: Handy graphical user interface library for daily use
 Home-page: https://github.com/chocolate-icecream/pancakekit
 Author: chocolate-icecream
 Project-URL: Bug Tracker, https://github.com/chocolate-icecream/pancakekit/issues
 Keywords: gui
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -41,9 +41,17 @@
 cake = Pancake()	# Step 1: Make a Pancake instance.
 cake.add(fibonacci)	# Step 2: Add your function to the pancake.
 cake.serve()		# Step 3: Serve the cake.
 ```
 
 When you open `http://127.0.0.1:8000/` in a web browser, you will find an input box for entering `n` and a button that invokes `fibonacci()`.
 
+## Adding an interface to your exisiting python script in an instant
+
+```shell
+pip -m pancakekit __YOUR_SCRIPT_FILE_NAME__
+```
+
+
+
 For more details: https://github.com/chocolate-icecream/pancakekit
```

### Comparing `pancakekit-0.1.9/README.md` & `pancakekit-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 cake = Pancake()	# Step 1: Make a Pancake instance.
 cake.add(fibonacci)	# Step 2: Add your function to the pancake.
 cake.serve()		# Step 3: Serve the cake.
 ```
 
 When you open `http://127.0.0.1:8000/` in a web browser, you will find an input box for entering `n` and a button that invokes `fibonacci()`.
 
+### Adding an interface to your exisiting python script in an instant
+
+```shell
+pip -m pancakekit __YOUR_SCRIPT_FILE_NAME__
+```
+
 ### Adding toppings
 
 In Pancake Kit, a Pancake instance corresponds to a single web page. Each UI component is added to the pancake as a Topping instance. 
 
 #### Value
 
 ```python
```

### Comparing `pancakekit-0.1.9/setup.cfg` & `pancakekit-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pancakekit
-version = 0.1.9
+version = 0.2.0
 author = chocolate-icecream
 description = Handy graphical user interface library for daily use
 long_description = file: README_pypi.md
 long_description_content_type = text/markdown
 url = https://github.com/chocolate-icecream/pancakekit
 project_urls = 
 	Bug Tracker = https://github.com/chocolate-icecream/pancakekit/issues
```

### Comparing `pancakekit-0.1.9/src/pancakekit/basecomponent/navigation.py` & `pancakekit-0.2.0/src/pancakekit/basecomponent/navigation.py`

 * *Files identical despite different names*

### Comparing `pancakekit-0.1.9/src/pancakekit/pancakekit.py` & `pancakekit-0.2.0/src/pancakekit/pancakekit.py`

 * *Files identical despite different names*

### Comparing `pancakekit-0.1.9/src/pancakekit/static/css/pancake.css` & `pancakekit-0.2.0/src/pancakekit/static/css/pancake.css`

 * *Files identical despite different names*

### Comparing `pancakekit-0.1.9/src/pancakekit/static/css/w3.css` & `pancakekit-0.2.0/src/pancakekit/static/css/w3.css`

 * *Files identical despite different names*

### Comparing `pancakekit-0.1.9/src/pancakekit/static/js/draggable.js` & `pancakekit-0.2.0/src/pancakekit/static/js/draggable.js`

 * *Files identical despite different names*

### Comparing `pancakekit-0.1.9/src/pancakekit/static/js/main.js` & `pancakekit-0.2.0/src/pancakekit/static/js/main.js`

 * *Files identical despite different names*

### Comparing `pancakekit-0.1.9/src/pancakekit/static/js/run_script.js` & `pancakekit-0.2.0/src/pancakekit/static/js/run_script.js`

 * *Files identical despite different names*

### Comparing `pancakekit-0.1.9/src/pancakekit/toppings/automatic.py` & `pancakekit-0.2.0/src/pancakekit/toppings/automatic.py`

 * *Files identical despite different names*

### Comparing `pancakekit-0.1.9/src/pancakekit/toppings/basic.py` & `pancakekit-0.2.0/src/pancakekit/toppings/basic.py`

 * *Files identical despite different names*

### Comparing `pancakekit-0.1.9/src/pancakekit/toppings/image.py` & `pancakekit-0.2.0/src/pancakekit/toppings/image.py`

 * *Files identical despite different names*

### Comparing `pancakekit-0.1.9/src/pancakekit/toppings/nparray.py` & `pancakekit-0.2.0/src/pancakekit/toppings/nparray.py`

 * *Files identical despite different names*

### Comparing `pancakekit-0.1.9/src/pancakekit/toppings/table.py` & `pancakekit-0.2.0/src/pancakekit/toppings/table.py`

 * *Files identical despite different names*

### Comparing `pancakekit-0.1.9/src/pancakekit/utils/utils.py` & `pancakekit-0.2.0/src/pancakekit/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pancakekit-0.1.9/src/pancakekit.egg-info/PKG-INFO` & `pancakekit-0.2.0/src/pancakekit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pancakekit
-Version: 0.1.9
+Version: 0.2.0
 Summary: Handy graphical user interface library for daily use
 Home-page: https://github.com/chocolate-icecream/pancakekit
 Author: chocolate-icecream
 Project-URL: Bug Tracker, https://github.com/chocolate-icecream/pancakekit/issues
 Keywords: gui
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -41,9 +41,17 @@
 cake = Pancake()	# Step 1: Make a Pancake instance.
 cake.add(fibonacci)	# Step 2: Add your function to the pancake.
 cake.serve()		# Step 3: Serve the cake.
 ```
 
 When you open `http://127.0.0.1:8000/` in a web browser, you will find an input box for entering `n` and a button that invokes `fibonacci()`.
 
+## Adding an interface to your exisiting python script in an instant
+
+```shell
+pip -m pancakekit __YOUR_SCRIPT_FILE_NAME__
+```
+
+
+
 For more details: https://github.com/chocolate-icecream/pancakekit
```

### Comparing `pancakekit-0.1.9/src/pancakekit.egg-info/SOURCES.txt` & `pancakekit-0.2.0/src/pancakekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

