# Comparing `tmp/dfsjson-1.1.0.tar.gz` & `tmp/dfsjson-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfsjson-1.1.0.tar", max compression
+gzip compressed data, was "dfsjson-1.1.1.tar", max compression
```

## Comparing `dfsjson-1.1.0.tar` & `dfsjson-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-04-21 10:30:21.167494 dfsjson-1.1.0/LICENSE
--rw-r--r--   0        0        0      971 2023-04-21 11:40:08.885748 dfsjson-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-21 10:14:31.990972 dfsjson-1.1.0/dfsjson/__init__.py
--rw-r--r--   0        0        0       28 2023-04-21 13:40:54.294586 dfsjson-1.1.0/dfsjson/src/__init__.py
--rw-r--r--   0        0        0     3344 2023-04-22 09:35:38.005165 dfsjson-1.1.0/dfsjson/src/dfsjson.py
--rw-r--r--   0        0        0      499 2023-04-22 09:45:05.082993 dfsjson-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 dfsjson-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-21 10:30:21.167494 dfsjson-1.1.1/LICENSE
+-rw-r--r--   0        0        0      972 2023-04-22 09:47:28.532993 dfsjson-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 10:14:31.990972 dfsjson-1.1.1/dfsjson/__init__.py
+-rw-r--r--   0        0        0       28 2023-04-21 13:40:54.294586 dfsjson-1.1.1/dfsjson/src/__init__.py
+-rw-r--r--   0        0        0     3344 2023-04-22 09:35:38.005165 dfsjson-1.1.1/dfsjson/src/dfsjson.py
+-rw-r--r--   0        0        0      499 2023-04-22 09:48:10.937282 dfsjson-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 dfsjson-1.1.1/PKG-INFO
```

### Comparing `dfsjson-1.1.0/LICENSE` & `dfsjson-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dfsjson-1.1.0/README.md` & `dfsjson-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DFS JSON
-A Depth First Search powered JSON encoding library. For the remaining operations (dump, dumps), it uses standard python JSON library.
+A Depth First Search powered JSON decoding library. For the remaining operations (dump, dumps), it uses standard python JSON library.
 
 # Installation
 ```
 pip install dfsjson
 ```
 
 # Usage
@@ -28,8 +28,8 @@
 ### Hey I know this. Why not have you used Breadth First Search?
 Technically you are correct but keep in mind that Breadth First Search keeps the previous states in its list which 
 scales with number of iterations you are making and it can be a huge strain on the memory.
 
 However, Depth First search requires only O(log(n)) memory complexity in which we can search a lot more possibilities.
 
 # Contribution
-Please don't hesitate to create issues and pull requests since this is developed overnight.
+Please don't hesitate to create issues and pull requests since this is developed overnight.
```

### Comparing `dfsjson-1.1.0/dfsjson/src/dfsjson.py` & `dfsjson-1.1.1/dfsjson/src/dfsjson.py`

 * *Files identical despite different names*

### Comparing `dfsjson-1.1.0/PKG-INFO` & `dfsjson-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: dfsjson
-Version: 1.1.0
+Version: 1.1.1
 Summary: A robust JSON encoder that fixes errors by utilizing DFS algorithm.
 Home-page: https://github.com/AutomaticHourglass/dfsjson
 Keywords: JSON,JSON Serialize,DFS,Error correcting JSON
 Author: Unsal Gokdag
 Author-email: unsal.gokdag@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # DFS JSON
-A Depth First Search powered JSON encoding library. For the remaining operations (dump, dumps), it uses standard python JSON library.
+A Depth First Search powered JSON decoding library. For the remaining operations (dump, dumps), it uses standard python JSON library.
 
 # Installation
 ```
 pip install dfsjson
 ```
 
 # Usage
@@ -45,7 +45,8 @@
 Technically you are correct but keep in mind that Breadth First Search keeps the previous states in its list which 
 scales with number of iterations you are making and it can be a huge strain on the memory.
 
 However, Depth First search requires only O(log(n)) memory complexity in which we can search a lot more possibilities.
 
 # Contribution
 Please don't hesitate to create issues and pull requests since this is developed overnight.
+
```

