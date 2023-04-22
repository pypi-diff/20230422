# Comparing `tmp/dfsjson-1.0.9.tar.gz` & `tmp/dfsjson-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfsjson-1.0.9.tar", max compression
+gzip compressed data, was "dfsjson-1.1.0.tar", max compression
```

## Comparing `dfsjson-1.0.9.tar` & `dfsjson-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-04-21 10:30:21.167494 dfsjson-1.0.9/LICENSE
--rw-r--r--   0        0        0      971 2023-04-21 11:40:08.885748 dfsjson-1.0.9/README.md
--rw-r--r--   0        0        0        0 2023-04-21 10:14:31.990972 dfsjson-1.0.9/dfsjson/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 08:29:19.085236 dfsjson-1.0.9/dfsjson/src/__init__.py
--rw-r--r--   0        0        0     3113 2023-04-21 10:52:57.284569 dfsjson-1.0.9/dfsjson/src/dfsjson.py
--rw-r--r--   0        0        0      499 2023-04-21 13:02:41.664411 dfsjson-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 dfsjson-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-21 10:30:21.167494 dfsjson-1.1.0/LICENSE
+-rw-r--r--   0        0        0      971 2023-04-21 11:40:08.885748 dfsjson-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 10:14:31.990972 dfsjson-1.1.0/dfsjson/__init__.py
+-rw-r--r--   0        0        0       28 2023-04-21 13:40:54.294586 dfsjson-1.1.0/dfsjson/src/__init__.py
+-rw-r--r--   0        0        0     3344 2023-04-22 09:35:38.005165 dfsjson-1.1.0/dfsjson/src/dfsjson.py
+-rw-r--r--   0        0        0      499 2023-04-22 09:45:05.082993 dfsjson-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 dfsjson-1.1.0/PKG-INFO
```

### Comparing `dfsjson-1.0.9/LICENSE` & `dfsjson-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dfsjson-1.0.9/README.md` & `dfsjson-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dfsjson-1.0.9/dfsjson/src/dfsjson.py` & `dfsjson-1.1.0/dfsjson/src/dfsjson.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-import re
+from __future__ import annotations
+
 import json
+import re
 
 
 class DFSJson:
     def __init__(self, max_depth=100, max_diff=5):
         self.max_depth = max_depth
         self.max_diff = max_diff
-        self.search_pattern = r'([\[\]\$\(\)\{\}\,\"\'])'
-        self.replace_characters = """}{"]\',+"""
+        self.search_pattern = r'([\[\]\(\)\{\}\,\"\'])'
+        self.replace_characters = """\"\',+ }{()]"""
         return
 
     @staticmethod
     def dump(*args):
         return json.dump(*args)
 
     @staticmethod
@@ -22,53 +24,63 @@
         string = f.read()
         return self.loads(string)
 
     def loads(self, string):
         try:
             return json.loads(string)
         except json.JSONDecodeError:
-            string = string.replace("'", '"') # most basic error is using ' instead of "
+            # most basic error is using ' instead of "
+            string = string.replace("'", '"')
             fixed_json, fitness = self.dfs(string, self.max_depth)
             return json.loads(fixed_json)
 
     @staticmethod
     def fitness(string):
         try:
             json.loads(string)
             return int(1e8)  # No error
         except json.JSONDecodeError as e:
             return e.pos
 
     @staticmethod
     def mutate(string, index, replacement, flag='insert'):
         if flag == 'insert':
-            return string[:index] + replacement + string[index:]  # insert character
+            # insert character
+            return string[:index] + replacement + string[index:]
         elif flag == 'replace':
-            return string[:index] + replacement + string[index + 1:]  # replace character
+            # replace character
+            return string[:index] + replacement + string[index + 1:]
         else:
             return ValueError
 
     @staticmethod
     def level_diff(string):
-        diff1 = abs(len(re.findall(r'{', string)) - len(re.findall(r'}', string)))
-        diff2 = abs(len(re.findall(r'\[', string)) - len(re.findall(r'\]', string)))
+        diff1 = abs(
+            len(re.findall(r'{', string)) - len(re.findall(r'}', string)),
+        )
+        diff2 = abs(
+            len(re.findall(r'\[', string)) - len(re.findall(r'\]', string)),
+        )
         return max(diff1, diff2)
 
     def dfs(self, string, max_depth=10, cur_fitness=None, visited=None):
         if visited is None:
             visited = set()
         if cur_fitness is None:
             cur_fitness = self.fitness(string)
         if max_depth < 0:
             return string, 0
         if cur_fitness == int(1e8):
             return string, cur_fitness
         best_fitness = cur_fitness
         best_string = string
-        indexes = [cur_fitness] + [r.span()[0] for r in re.finditer(self.search_pattern, string)]
+        indexes = [cur_fitness] + [
+            r.span()[0]
+            for r in re.finditer(self.search_pattern, string)
+        ]
         diff = -self.max_diff
 
         for index in indexes:
             for m in self.replace_characters:
                 for mutate_type in ['insert', 'replace']:
                     new_string = self.mutate(string, index, m, mutate_type)
                     diff = self.level_diff(new_string)
@@ -80,10 +92,15 @@
                     if new_fitness > best_fitness + 1:
                         best_fitness = new_fitness
                         best_string = new_string
                         if best_fitness == int(1e8) and diff == 0:
                             break
 
         if best_fitness < int(1e8) and diff != 0:
-            return self.dfs(best_string, max_depth - 1, best_fitness, visited.copy().union({best_string}))
+            return self.dfs(
+                best_string,
+                max_depth - 1,
+                best_fitness,
+                visited.copy().union({best_string}),
+            )
         else:
             return best_string, best_fitness
```

### Comparing `dfsjson-1.0.9/PKG-INFO` & `dfsjson-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: dfsjson
-Version: 1.0.9
+Version: 1.1.0
 Summary: A robust JSON encoder that fixes errors by utilizing DFS algorithm.
 Home-page: https://github.com/AutomaticHourglass/dfsjson
 Keywords: JSON,JSON Serialize,DFS,Error correcting JSON
 Author: Unsal Gokdag
 Author-email: unsal.gokdag@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # DFS JSON
```

