# Comparing `tmp/issue_db_api-0.4.1.tar.gz` & `tmp/issue_db_api-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.4.1.tar", last modified: Fri Apr 21 11:12:36 2023, max compression
+gzip compressed data, was "issue_db_api-0.5.0.tar", last modified: Sat Apr 22 09:17:31 2023, max compression
```

## Comparing `issue_db_api-0.4.1.tar` & `issue_db_api-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-21 11:12:36.358591 issue_db_api-0.4.1/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.4.1/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.4.1/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.4.1/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-21 11:12:36.358591 issue_db_api-0.4.1/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.4.1/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-21 11:12:36.354591 issue_db_api-0.4.1/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      469 2023-04-21 11:12:15.000000 issue_db_api-0.4.1/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 10:30:30.000000 issue_db_api-0.4.1/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     7843 2023-04-20 12:01:48.000000 issue_db_api-0.4.1/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-21 11:12:36.358591 issue_db_api-0.4.1/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    41564 2023-04-21 11:09:36.000000 issue_db_api-0.4.1/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.4.1/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.4.1/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3773 2023-04-20 11:59:24.000000 issue_db_api-0.4.1/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.4.1/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.4.1/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.4.1/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    35430 2023-04-20 12:01:48.000000 issue_db_api-0.4.1/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-20 10:10:15.000000 issue_db_api-0.4.1/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3710 2023-04-20 08:15:34.000000 issue_db_api-0.4.1/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5906 2023-04-20 12:00:30.000000 issue_db_api-0.4.1/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-21 11:12:36.358591 issue_db_api-0.4.1/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.4.1/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.4.1/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.4.1/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-20 08:15:34.000000 issue_db_api-0.4.1/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-21 11:12:36.354591 issue_db_api-0.4.1/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-21 11:12:36.000000 issue_db_api-0.4.1/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-04-21 11:12:36.000000 issue_db_api-0.4.1/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-21 11:12:36.000000 issue_db_api-0.4.1/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.4.1/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-04-21 11:12:36.000000 issue_db_api-0.4.1/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-04-21 11:12:15.000000 issue_db_api-0.4.1/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-04-21 11:12:36.358591 issue_db_api-0.4.1/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.4.1/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 09:17:31.863943 issue_db_api-0.5.0/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.5.0/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-22 09:17:31.863943 issue_db_api-0.5.0/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 09:17:31.859943 issue_db_api-0.5.0/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      469 2023-04-22 09:16:52.000000 issue_db_api-0.5.0/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 10:30:30.000000 issue_db_api-0.5.0/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8096 2023-04-22 09:15:44.000000 issue_db_api-0.5.0/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 09:17:31.863943 issue_db_api-0.5.0/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    41564 2023-04-21 11:09:36.000000 issue_db_api-0.5.0/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3780 2023-04-22 08:55:43.000000 issue_db_api-0.5.0/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    36013 2023-04-22 09:15:44.000000 issue_db_api-0.5.0/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-22 09:10:35.000000 issue_db_api-0.5.0/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3710 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6312 2023-04-22 09:15:44.000000 issue_db_api-0.5.0/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 09:17:31.863943 issue_db_api-0.5.0/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-22 09:10:31.000000 issue_db_api-0.5.0/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 09:17:31.859943 issue_db_api-0.5.0/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-22 09:17:31.000000 issue_db_api-0.5.0/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-04-22 09:17:31.000000 issue_db_api-0.5.0/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-22 09:17:31.000000 issue_db_api-0.5.0/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.5.0/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-04-22 09:17:31.000000 issue_db_api-0.5.0/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-04-22 09:16:52.000000 issue_db_api-0.5.0/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-04-22 09:17:31.863943 issue_db_api-0.5.0/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.5.0/setup.py
```

### Comparing `issue_db_api-0.4.1/LICENSE` & `issue_db_api-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.4.1/PKG-INFO` & `issue_db_api-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.4.1
+Version: 0.5.0
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.4.1/issue_db_api/issue_api.pyi` & `issue_db_api-0.5.0/issue_db_api/issue_api.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -36,27 +36,33 @@
 
     def get_embedding_by_id(self, id: str) -> Embedding:
         ...
 
     def create_embedding(self, name: str, config: dict[str, typing.Any]) -> Embedding:
         ...
 
+    def delete_embedding(self, embedding: Embedding):
+        ...
+
     def find_issues_by_key(self, *args: tuple[str, str]) -> list[Issue]:
         ...
 
     @property
     def models(self) -> list[Model]:
         ...
 
     def get_model_by_id(self, id: str) -> Model:
         ...
 
     def add_model(self, name: str, config: dict[str, typing.Any]) -> Model:
         ...
 
+    def delete_model_config(self, model: Model):
+        ...
+
 
 class Repo:
     def __repr__(self) -> str:
         ...
 
     @property
     def name(self) -> str:
@@ -132,14 +138,18 @@
     def __eq__(self, other) -> bool | NotImplemented:
         ...
 
     def __hash__(self) -> int:
         ...
 
     @property
+    def identifier(self) -> str:
+        ...
+
+    @property
     def manual_label(self) -> Label:
         ...
 
     @manual_label.setter
     def manual_label(self, value: Label):
         ...
 
@@ -161,15 +171,15 @@
         ...
 
     @is_in_review.setter
     def is_in_review(self, value: bool):
         ...
 
     @property
-    def labelling_comments(self) -> list[str]:
+    def labelling_comments(self) -> list[Comment]:
         ...
 
     def add_labelling_comment(self, text: str):
         ...
 
     def remove_labelling_comment(self, comment: Comment):
         ...
@@ -303,14 +313,18 @@
     def __repr__(self) -> str:
         ...
 
     def __eq__(self, other) -> bool | NotImplemented:
         ...
 
     @property
+    def identifier(self) -> str:
+        ...
+
+    @property
     def name(self) -> str:
         ...
 
     @name.setter
     def name(self, name: str):
         ...
```

### Comparing `issue_db_api-0.4.1/issue_db_api/src/api_core.rs` & `issue_db_api-0.5.0/issue_db_api/src/api_core.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.4.1/issue_db_api/src/comments.rs` & `issue_db_api-0.5.0/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.4.1/issue_db_api/src/config.rs` & `issue_db_api-0.5.0/issue_db_api/src/config.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.4.1/issue_db_api/src/embedding.rs` & `issue_db_api-0.5.0/issue_db_api/src/embedding.rs`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             has_file: self.has_file,
             update_policy: config_handling
         }
     }
 }
 
 #[allow(unused)]
-#[derive(Debug)]
+#[derive(Debug, Clone)]
 pub struct Embedding {
     api: Arc<IssueAPI>,
     id: String,
     name: String ,
     config: HashMap<String, Value>,
     has_file: bool,
     update_policy: ConfigHandlingPolicy
```

### Comparing `issue_db_api-0.4.1/issue_db_api/src/errors.rs` & `issue_db_api-0.5.0/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.4.1/issue_db_api/src/issues.rs` & `issue_db_api-0.5.0/issue_db_api/src/issues.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.4.1/issue_db_api/src/labels.rs` & `issue_db_api-0.5.0/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.4.1/issue_db_api/src/lib.rs` & `issue_db_api-0.5.0/issue_db_api/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,18 @@
                 let config = c.into_iter().collect();
                 Ok(PyEmbedding{inner: api2py_error(self.repo.create_embedding(name, config))?})
             } else {
                 Err(PyTypeError::new_err("Top-level JSON must be an object"))
             }
         }
 
+        fn delete_embedding(&self, embedding: &PyEmbedding) -> PyResult<()> {
+            api2py_error(self.repo.delete_embedding(embedding.inner.clone()))
+        }
+
         #[pyo3(signature=(*args, attributes=vec![], load_labels=false))]
         fn find_issues_by_key(&self,
                               args: &PyTuple,
                               attributes: Vec<String>,
                               load_labels: bool) -> PyResult<Vec<PyIssue>> {
             let keys = args.extract::<Vec<(String, String)>>()?;
             let settings = IssueLoadingSettings::new(
@@ -296,14 +300,19 @@
             let mut converted = HashMap::with_capacity(config.len());
             for (k, v) in config {
                 converted.insert(k, py_to_json(v)?);
             }
             let model = api2py_error(self.repo.add_model(name, converted))?;
             Ok(PyModel{inner: model})
         }
+
+        fn delete_model_config(&self, model: &PyModel) -> PyResult<()> {
+            api2py_error(self.repo.delete_model_config_by_id(model.inner.identifier()))
+
+        }
     }
 
     #[pyclass(name="IssueRepo")]
     struct PyRepo {
         inner: IssueRepo
     }
 
@@ -495,14 +504,19 @@
         fn __hash__(&self) -> PyResult<u64> {
             let mut s = std::collections::hash_map::DefaultHasher::new();
             self.issue.hash(&mut s);
             Ok(s.finish())
         }
 
         #[getter]
+        fn identifier(&self) -> PyResult<String> {
+            Ok(self.issue.ident().clone())
+        }
+
+        #[getter]
         fn manual_label(&self) -> PyResult<Option<PyLabel>> {
             let obj = api2py_error(self.issue.get_manual_label())?
                 .map(|label| PyLabel{inner: label});
             Ok(obj)
         }
 
         #[setter]
@@ -787,14 +801,19 @@
                 CompareOp::Eq => (self.inner == other.inner).into_py(py),
                 CompareOp::Ne => (self.inner != other.inner).into_py(py),
                 _ => py.NotImplemented(),
             }
         }
 
         #[getter]
+        fn identifier(&self) -> PyResult<String> {
+            Ok(self.inner.identifier())
+        }
+
+        #[getter]
         fn name(&self) -> PyResult<String> {
             api2py_error(self.inner.name())
         }
 
         #[setter]
         fn set_name(&mut self, name: String) -> PyResult<()> {
             api2py_error(self.inner.update_name(name))
```

### Comparing `issue_db_api-0.4.1/issue_db_api/src/models.rs` & `issue_db_api-0.5.0/issue_db_api/src/models.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.4.1/issue_db_api/src/query.rs` & `issue_db_api-0.5.0/issue_db_api/src/query.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.4.1/issue_db_api/src/repository.rs` & `issue_db_api-0.5.0/issue_db_api/src/repository.rs`

 * *Files 5% similar despite different names*

```diff
@@ -128,14 +128,18 @@
             config,
             false,
             self.config_handling
         );
         Ok(embedding)
     }
 
+    pub fn delete_embedding(&self, embedding: Embedding) -> APIResult<()> {
+        self.api.delete_embedding(embedding.identifier())
+    }
+
     pub fn models(&self) -> APIResult<Vec<Model>> {
         let models = self.api.get_all_models()?;
         let converted = models
             .into_iter()
             .map(|m|
                 Model::new(self.api.clone(),
                            m.model_id,
@@ -165,14 +169,22 @@
             id,
             name,
             Some(config),
             self.config_handling
         );
         Ok(m)
     }
+
+    pub fn delete_model_config(&self, model: Model) -> APIResult<()> {
+        self.api.delete_model_config(model.identifier())
+    }
+
+    pub(crate) fn delete_model_config_by_id(&self, id: String) -> APIResult<()> {
+        self.api.delete_model_config(id)
+    }
 }
 
 
 pub struct IssueRepo {
     name: String,
     api: Arc<IssueAPI>
 }
```

### Comparing `issue_db_api-0.4.1/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.5.0/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.4.1/issue_db_api/src/tags.rs` & `issue_db_api-0.5.0/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.4.1/issue_db_api/src/util.rs` & `issue_db_api-0.5.0/issue_db_api/src/util.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.4.1/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.5.0/issue_db_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.4.1
+Version: 0.5.0
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.4.1/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.5.0/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.4.1/pyproject.toml` & `issue_db_api-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.4.1"
+version = "0.5.0"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```

