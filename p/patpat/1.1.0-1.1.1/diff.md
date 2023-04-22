# Comparing `tmp/patpat-1.1.0.tar.gz` & `tmp/patpat-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patpat-1.1.0.tar", last modified: Sat Dec  3 13:53:19 2022, max compression
+gzip compressed data, was "patpat-1.1.1.tar", last modified: Sat Apr 22 09:53:07 2023, max compression
```

## Comparing `patpat-1.1.0.tar` & `patpat-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-12-03 13:53:19.964662 patpat-1.1.0/
--rw-rw-rw-   0        0        0    11543 2022-10-13 07:30:37.000000 patpat-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2356 2022-12-03 13:53:19.949009 patpat-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1759 2022-11-28 12:02:38.000000 patpat-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-12-03 13:53:19.933401 patpat-1.1.0/patpat/
--rw-rw-rw-   0        0        0       14 2022-11-24 13:43:12.000000 patpat-1.1.0/patpat/__init__.py
--rw-rw-rw-   0        0        0    13055 2022-12-03 12:19:07.000000 patpat-1.1.0/patpat/checker.py
--rw-rw-rw-   0        0        0    15778 2022-12-03 12:33:22.000000 patpat-1.1.0/patpat/hub.py
--rw-rw-rw-   0        0        0     2826 2022-11-28 11:41:38.000000 patpat-1.1.0/patpat/logger.py
--rw-rw-rw-   0        0        0    30997 2022-12-03 13:40:55.000000 patpat-1.1.0/patpat/mapper.py
--rw-rw-rw-   0        0        0    17772 2022-11-29 09:39:47.000000 patpat-1.1.0/patpat/querier.py
--rw-rw-rw-   0        0        0    41496 2022-12-03 11:18:44.000000 patpat-1.1.0/patpat/retriever.py
--rw-rw-rw-   0        0        0     9716 2022-12-01 12:34:08.000000 patpat-1.1.0/patpat/utility.py
-drwxrwxrwx   0        0        0        0 2022-12-03 13:53:19.949009 patpat-1.1.0/patpat.egg-info/
--rw-rw-rw-   0        0        0     2356 2022-12-03 13:53:19.000000 patpat-1.1.0/patpat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2022-12-03 13:53:19.000000 patpat-1.1.0/patpat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-03 13:53:19.000000 patpat-1.1.0/patpat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2022-12-03 13:53:19.000000 patpat-1.1.0/patpat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-12-03 13:53:19.000000 patpat-1.1.0/patpat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      797 2022-12-03 13:43:58.000000 patpat-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-03 13:53:19.964662 patpat-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-22 09:53:07.881251 patpat-1.1.1/
+-rw-rw-rw-   0        0        0    11543 2022-10-13 07:30:37.000000 patpat-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2423 2023-04-22 09:53:07.881251 patpat-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1826 2023-04-22 09:49:43.000000 patpat-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 09:53:07.850039 patpat-1.1.1/patpat/
+-rw-rw-rw-   0        0        0       14 2022-11-24 13:43:12.000000 patpat-1.1.1/patpat/__init__.py
+-rw-rw-rw-   0        0        0    13060 2023-04-22 09:26:05.000000 patpat-1.1.1/patpat/checker.py
+-rw-rw-rw-   0        0        0    15778 2022-12-03 12:33:22.000000 patpat-1.1.1/patpat/hub.py
+-rw-rw-rw-   0        0        0     2826 2022-11-28 11:41:38.000000 patpat-1.1.1/patpat/logger.py
+-rw-rw-rw-   0        0        0    30997 2022-12-03 13:40:55.000000 patpat-1.1.1/patpat/mapper.py
+-rw-rw-rw-   0        0        0    17772 2022-11-29 09:39:47.000000 patpat-1.1.1/patpat/querier.py
+-rw-rw-rw-   0        0        0    41496 2023-04-22 09:32:20.000000 patpat-1.1.1/patpat/retriever.py
+-rw-rw-rw-   0        0        0     9716 2022-12-01 12:34:08.000000 patpat-1.1.1/patpat/utility.py
+drwxrwxrwx   0        0        0        0 2023-04-22 09:53:07.881251 patpat-1.1.1/patpat.egg-info/
+-rw-rw-rw-   0        0        0     2423 2023-04-22 09:53:07.000000 patpat-1.1.1/patpat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-04-22 09:53:07.000000 patpat-1.1.1/patpat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 09:53:07.000000 patpat-1.1.1/patpat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-22 09:53:07.000000 patpat-1.1.1/patpat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-22 09:53:07.000000 patpat-1.1.1/patpat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      797 2023-04-22 09:48:18.000000 patpat-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-22 09:53:07.881251 patpat-1.1.1/setup.cfg
```

### Comparing `patpat-1.1.0/LICENSE` & `patpat-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `patpat-1.1.0/PKG-INFO` & `patpat-1.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: patpat
-Version: 1.1.0
+Version: 1.1.1
 Summary: Patpat is public proteomics dataset search framework that only requires protein identifiers to be passed in to search for relevant datasets.
 Author-email: Weiheng Liao <weiheng_liao@outlook.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/henry-leo/Patpat
 Project-URL: Bug Tracker, https://github.com/henry-leo/Patpat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# Update
+
+1. Fixed a bug for checking connection with iProX
+
+
 # Patpat
 
 Patpat is public proteomics dataset search framework that
 only requires protein identifiers to be passed in to search for relevant datasets
 
 ## Base Usage
```

### Comparing `patpat-1.1.0/README.md` & `patpat-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Update
+
+1. Fixed a bug for checking connection with iProX
+
+
 # Patpat
 
 Patpat is public proteomics dataset search framework that
 only requires protein identifiers to be passed in to search for relevant datasets
 
 ## Base Usage
```

### Comparing `patpat-1.1.0/patpat/checker.py` & `patpat-1.1.1/patpat/checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         t = project_retriever
         flag = False
         message = []
 
         print(f"\nCheck the connectivity of the iProX Project API")
         for _ in tqdm.tqdm(range(self.times)):
             try:
-                c = requests.get(t.api, params=t.example)
+                c = requests.get("/".join([t.api, t.example]))
             except requests.exceptions.RequestException as e:
                 message.extend([e])
                 continue
             else:
                 if c.ok:
                     flag = True
                     break
```

### Comparing `patpat-1.1.0/patpat/hub.py` & `patpat-1.1.1/patpat/hub.py`

 * *Files identical despite different names*

### Comparing `patpat-1.1.0/patpat/logger.py` & `patpat-1.1.1/patpat/logger.py`

 * *Files identical despite different names*

### Comparing `patpat-1.1.0/patpat/mapper.py` & `patpat-1.1.1/patpat/mapper.py`

 * *Files identical despite different names*

### Comparing `patpat-1.1.0/patpat/querier.py` & `patpat-1.1.1/patpat/querier.py`

 * *Files identical despite different names*

### Comparing `patpat-1.1.0/patpat/retriever.py` & `patpat-1.1.1/patpat/retriever.py`

 * *Files 0% similar despite different names*

```diff
@@ -615,15 +615,15 @@
 class IProXProteinRetriever(GenericIProXRetriever):
     """Used to collect protein information in iProX database. 用于收集iProX数据库中的蛋白质信息。"""
 
     def __init__(self):
         super().__init__()
         self.response = dict()
         self.api = 'https://www.iprox.cn/proxi/psms'
-        self.example = 'E9PV96'
+        self.example = 'P60709'
 
     @property
     def request_word(self):
         return self._request_word
 
     @request_word.setter
     def request_word(self, request_word):
```

### Comparing `patpat-1.1.0/patpat/utility.py` & `patpat-1.1.1/patpat/utility.py`

 * *Files identical despite different names*

### Comparing `patpat-1.1.0/patpat.egg-info/PKG-INFO` & `patpat-1.1.1/patpat.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: patpat
-Version: 1.1.0
+Version: 1.1.1
 Summary: Patpat is public proteomics dataset search framework that only requires protein identifiers to be passed in to search for relevant datasets.
 Author-email: Weiheng Liao <weiheng_liao@outlook.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/henry-leo/Patpat
 Project-URL: Bug Tracker, https://github.com/henry-leo/Patpat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# Update
+
+1. Fixed a bug for checking connection with iProX
+
+
 # Patpat
 
 Patpat is public proteomics dataset search framework that
 only requires protein identifiers to be passed in to search for relevant datasets
 
 ## Base Usage
```

### Comparing `patpat-1.1.0/pyproject.toml` & `patpat-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "patpat"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
     { name = "Weiheng Liao", email = "weiheng_liao@outlook.com" },
 ]
 description = "Patpat is public proteomics dataset search framework that only requires protein identifiers to be passed in to search for relevant datasets."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

