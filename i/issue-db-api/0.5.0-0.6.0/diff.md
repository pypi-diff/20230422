# Comparing `tmp/issue_db_api-0.5.0.tar.gz` & `tmp/issue_db_api-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.5.0.tar", last modified: Sat Apr 22 09:17:31 2023, max compression
+gzip compressed data, was "issue_db_api-0.6.0.tar", last modified: Sat Apr 22 10:25:28 2023, max compression
```

## Comparing `issue_db_api-0.5.0.tar` & `issue_db_api-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 09:17:31.863943 issue_db_api-0.5.0/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.5.0/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-22 09:17:31.863943 issue_db_api-0.5.0/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 09:17:31.859943 issue_db_api-0.5.0/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      469 2023-04-22 09:16:52.000000 issue_db_api-0.5.0/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 10:30:30.000000 issue_db_api-0.5.0/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8096 2023-04-22 09:15:44.000000 issue_db_api-0.5.0/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 09:17:31.863943 issue_db_api-0.5.0/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    41564 2023-04-21 11:09:36.000000 issue_db_api-0.5.0/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3780 2023-04-22 08:55:43.000000 issue_db_api-0.5.0/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    36013 2023-04-22 09:15:44.000000 issue_db_api-0.5.0/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-22 09:10:35.000000 issue_db_api-0.5.0/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3710 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6312 2023-04-22 09:15:44.000000 issue_db_api-0.5.0/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 09:17:31.863943 issue_db_api-0.5.0/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-22 09:10:31.000000 issue_db_api-0.5.0/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 09:17:31.859943 issue_db_api-0.5.0/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-22 09:17:31.000000 issue_db_api-0.5.0/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-04-22 09:17:31.000000 issue_db_api-0.5.0/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-22 09:17:31.000000 issue_db_api-0.5.0/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.5.0/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-04-22 09:17:31.000000 issue_db_api-0.5.0/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-04-22 09:16:52.000000 issue_db_api-0.5.0/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-04-22 09:17:31.863943 issue_db_api-0.5.0/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 10:25:28.607392 issue_db_api-0.6.0/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.6.0/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-22 10:25:28.607392 issue_db_api-0.6.0/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 10:25:28.603392 issue_db_api-0.6.0/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      469 2023-04-22 10:24:52.000000 issue_db_api-0.6.0/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 10:30:30.000000 issue_db_api-0.6.0/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8096 2023-04-22 09:15:44.000000 issue_db_api-0.6.0/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 10:25:28.607392 issue_db_api-0.6.0/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    41564 2023-04-21 11:09:36.000000 issue_db_api-0.6.0/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3780 2023-04-22 08:55:43.000000 issue_db_api-0.6.0/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    36247 2023-04-22 10:20:48.000000 issue_db_api-0.6.0/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-22 09:10:35.000000 issue_db_api-0.6.0/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3710 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6312 2023-04-22 09:15:44.000000 issue_db_api-0.6.0/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 10:25:28.607392 issue_db_api-0.6.0/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-22 09:10:31.000000 issue_db_api-0.6.0/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 10:25:28.603392 issue_db_api-0.6.0/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-22 10:25:28.000000 issue_db_api-0.6.0/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-04-22 10:25:28.000000 issue_db_api-0.6.0/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-22 10:25:28.000000 issue_db_api-0.6.0/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.6.0/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-04-22 10:25:28.000000 issue_db_api-0.6.0/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-04-22 10:24:52.000000 issue_db_api-0.6.0/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-04-22 10:25:28.607392 issue_db_api-0.6.0/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/setup.py
```

### Comparing `issue_db_api-0.5.0/LICENSE` & `issue_db_api-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/PKG-INFO` & `issue_db_api-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.5.0
+Version: 0.6.0
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.5.0/issue_db_api/issue_api.pyi` & `issue_db_api-0.6.0/issue_db_api/issue_api.pyi`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/issue_db_api/src/api_core.rs` & `issue_db_api-0.6.0/issue_db_api/src/api_core.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/issue_db_api/src/comments.rs` & `issue_db_api-0.6.0/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/issue_db_api/src/config.rs` & `issue_db_api-0.6.0/issue_db_api/src/config.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/issue_db_api/src/embedding.rs` & `issue_db_api-0.6.0/issue_db_api/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/issue_db_api/src/errors.rs` & `issue_db_api-0.6.0/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/issue_db_api/src/issues.rs` & `issue_db_api-0.6.0/issue_db_api/src/issues.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/issue_db_api/src/labels.rs` & `issue_db_api-0.6.0/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/issue_db_api/src/lib.rs` & `issue_db_api-0.6.0/issue_db_api/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -405,14 +405,21 @@
         fn tag(&self, name: String) -> PyResult<Self> {
             Ok(Self{query: Some(self.add_tag(name, QueryCMP::Eq)?)})
         }
 
         fn not_tag(&self, name: String) -> PyResult<Self> {
             Ok(Self{query: Some(self.add_tag(name, QueryCMP::Ne)?)})
         }
+
+        fn to_json(&self, py: Python<'_>) -> PyResult<PyObject> {
+            match self.query {
+                None => Ok(py.None()),
+                Some(ref q) => Ok(json_to_py(py, q.clone().into_json()))
+            }
+        }
     }
 
     #[pyclass(name="Label")]
     #[allow(unused)]
     #[derive(Debug, Copy, Clone)]
     #[derive(Eq, PartialEq, Hash)]
     struct PyLabel {
```

### Comparing `issue_db_api-0.5.0/issue_db_api/src/models.rs` & `issue_db_api-0.6.0/issue_db_api/src/models.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/issue_db_api/src/query.rs` & `issue_db_api-0.6.0/issue_db_api/src/query.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/issue_db_api/src/repository.rs` & `issue_db_api-0.6.0/issue_db_api/src/repository.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.6.0/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/issue_db_api/src/tags.rs` & `issue_db_api-0.6.0/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/issue_db_api/src/util.rs` & `issue_db_api-0.6.0/issue_db_api/src/util.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.6.0/issue_db_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.5.0
+Version: 0.6.0
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.5.0/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.6.0/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.5.0/pyproject.toml` & `issue_db_api-0.6.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```

