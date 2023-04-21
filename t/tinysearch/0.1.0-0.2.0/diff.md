# Comparing `tmp/tinysearch-0.1.0.tar.gz` & `tmp/tinysearch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinysearch-0.1.0.tar", last modified: Fri Apr 21 19:08:18 2023, max compression
+gzip compressed data, was "tinysearch-0.2.0.tar", last modified: Fri Apr 21 20:42:52 2023, max compression
```

## Comparing `tinysearch-0.1.0.tar` & `tinysearch-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-21 19:08:08.833394 tinysearch-0.1.0/LICENSE
--rw-r--r--   0        0        0     1562 2023-04-21 19:08:08.833394 tinysearch-0.1.0/README.md
--rw-r--r--   0        0        0      651 2023-04-21 19:08:18.945639 tinysearch-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 19:08:08.837394 tinysearch-0.1.0/tinysearch/__init__.py
--rw-r--r--   0        0        0     1276 2023-04-21 19:08:08.837394 tinysearch-0.1.0/tinysearch/analyzer.py
--rw-r--r--   0        0        0     1237 2023-04-21 19:08:08.837394 tinysearch-0.1.0/tinysearch/document.py
--rw-r--r--   0        0        0      779 2023-04-21 19:08:08.837394 tinysearch-0.1.0/tinysearch/index.py
--rw-r--r--   0        0        0     2960 2023-04-21 19:08:08.837394 tinysearch-0.1.0/tinysearch/search.py
--rw-r--r--   0        0        0     1824 1970-01-01 00:00:00.000000 tinysearch-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-21 20:42:41.617072 tinysearch-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1562 2023-04-21 20:42:41.617072 tinysearch-0.2.0/README.md
+-rw-r--r--   0        0        0      999 2023-04-21 20:42:52.321223 tinysearch-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 20:42:41.617072 tinysearch-0.2.0/tinysearch/__init__.py
+-rw-r--r--   0        0        0     1276 2023-04-21 20:42:41.617072 tinysearch-0.2.0/tinysearch/analyzer.py
+-rw-r--r--   0        0        0     1302 2023-04-21 20:42:41.617072 tinysearch-0.2.0/tinysearch/document.py
+-rw-r--r--   0        0        0      905 2023-04-21 20:42:41.617072 tinysearch-0.2.0/tinysearch/index.py
+-rw-r--r--   0        0        0     3171 2023-04-21 20:42:41.617072 tinysearch-0.2.0/tinysearch/search.py
+-rw-r--r--   0        0        0     2063 1970-01-01 00:00:00.000000 tinysearch-0.2.0/PKG-INFO
```

### Comparing `tinysearch-0.1.0/LICENSE` & `tinysearch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tinysearch-0.1.0/README.md` & `tinysearch-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tinysearch-0.1.0/pyproject.toml` & `tinysearch-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -16,28 +16,45 @@
     "mkdocs",
 ]
 
 [tool.pdm.scripts]
 test = "pytest test"
 fmt = "black ."
 
+[tool.pdm.version]
+source = "scm"
+
 [project]
 name = "tinysearch"
-version = "0.1.0"
+dynamic = []
 description = "Tiny one-phase search engine"
 authors = [
     { name = "Domagoj Marsic", email = "dmars@protonmail.com" },
 ]
 dependencies = [
     "pystemmer>=2.2.0.1",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
+classifiers = [
+    "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+]
+keywords = [
+    "search",
+    "engine",
+]
+version = "0.2.0"
 
 [project.license]
 text = "Apache-2.0"
 
+[project.urls]
+Homepage = "https://github.com/dmarsic/tinysearch"
+
 [build-system]
 requires = [
     "pdm-backend",
+    "setuptools-git-versioning",
 ]
 build-backend = "pdm.backend"
```

### Comparing `tinysearch-0.1.0/tinysearch/analyzer.py` & `tinysearch-0.2.0/tinysearch/analyzer.py`

 * *Files identical despite different names*

### Comparing `tinysearch-0.1.0/tinysearch/document.py` & `tinysearch-0.2.0/tinysearch/document.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,18 @@
         if original is None:
             raise ValueError(f"Document needs to be text.")
 
         self.original = original
         self.tokens = self.analyze()
 
     def __str__(self):
-        return f'"{self.original}"'
+        return f"Document['{self.original}']"
+
+    def __repr__(self):
+        return self.__str__()
 
     def analyze(self) -> Counter:
         """Parses the original text into a list of tokens."""
         a = Analyzer()
         tokens = a.analyze(self.original)
 
         # Each token (key) has a term frequency (value)
```

### Comparing `tinysearch-0.1.0/tinysearch/index.py` & `tinysearch-0.2.0/tinysearch/index.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,14 +18,20 @@
 from tinysearch.document import Document
 
 
 class Index:
     def __init__(self, docs: List[str]) -> None:
         self.docs = self.process_docs(docs)
 
+    def __str__(self):
+        return f"Index[docs={len(self.docs)}]"
+
+    def __repr__(self):
+        return self.__str__()
+
     def process_docs(self, docs: List[str]) -> List[Document]:
         processed = []
         for doc in docs:
             d = Document(doc)
             d.analyze()
             processed.append(d)
         return processed
```

### Comparing `tinysearch-0.1.0/tinysearch/search.py` & `tinysearch-0.2.0/tinysearch/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,14 +50,17 @@
     def __init__(self):
         self.results = []
         self._matches = []
 
     def __str__(self):
         return str(self.results)
 
+    def __repr__(self):
+        return self.__str__()
+
     def append(self, result: Result) -> None:
         self.results.append(result)
         if result.score > 0.0:
             self._matches.append(result)
 
     @property
     def count(self) -> int:
@@ -74,14 +77,20 @@
             raise ValueError("Query must be text.")
 
         self.index = Index(docs)
         self.query = query
         self.results = Results()
         self.search()
 
+    def __str__(self):
+        return f"Search[query='{self.query}', matches={self.results.count}]"
+
+    def __repr__(self):
+        return self.__str__()
+
     def search(self) -> Results:
         self.score_docs(self.query)
 
     def score_docs(self, query: str):
         for doc in self.index.docs:
             score = self.score_doc(doc, query)
             self.results.append(Result(doc, score))
```

### Comparing `tinysearch-0.1.0/PKG-INFO` & `tinysearch-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 Metadata-Version: 2.1
 Name: tinysearch
-Version: 0.1.0
+Version: 0.2.0
 Summary: Tiny one-phase search engine
+Keywords: search engine
 Author-Email: Domagoj Marsic <dmars@protonmail.com>
 License: Apache-2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Project-URL: Homepage, https://github.com/dmarsic/tinysearch
 Requires-Python: >=3.9
 Requires-Dist: pystemmer>=2.2.0.1
 Description-Content-Type: text/markdown
 
 # TinySearch
 
 TinySearch is a tiny one-phase search engine. It is extremely easy to
```

