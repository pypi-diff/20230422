# Comparing `tmp/binooculars-0.0.1.tar.gz` & `tmp/binooculars-0.0.2.tar.gz`

## Comparing `binooculars-0.0.1.tar` & `binooculars-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 binooculars-0.0.1/Cargo.toml
--rw-r--r--   0      502       20      946 2023-04-14 08:20:03.000000 binooculars-0.0.1/.github/workflows/python.yml
--rw-r--r--   0      502       20      692 2023-04-17 08:38:36.000000 binooculars-0.0.1/.github/workflows/rust.yml
--rw-r--r--   0      502       20      685 2023-04-01 12:28:12.000000 binooculars-0.0.1/.gitignore
--rw-r--r--   0      502       20      398 2023-04-17 12:28:30.000000 binooculars-0.0.1/.readthedocs.yaml
--rw-r--r--   0      502       20      872 2023-04-17 08:36:59.000000 binooculars-0.0.1/CHANGELOG.md
--rw-r--r--   0      502       20      347 2023-04-17 07:50:52.000000 binooculars-0.0.1/Pipfile
--rw-r--r--   0      502       20    91556 2023-04-17 11:43:26.000000 binooculars-0.0.1/Pipfile.lock
--rw-r--r--   0      502       20      753 2023-04-17 07:50:52.000000 binooculars-0.0.1/README.md
--rw-r--r--   0      502       20      638 2023-04-22 13:37:14.000000 binooculars-0.0.1/docs/Makefile
--rw-r--r--   0      502       20      804 2023-04-22 13:37:14.000000 binooculars-0.0.1/docs/make.bat
--rw-r--r--   0      502       20      959 2023-04-22 13:57:34.000000 binooculars-0.0.1/docs/source/conf.py
--rw-r--r--   0      502       20      394 2023-04-22 13:48:43.000000 binooculars-0.0.1/docs/source/index.rst
--rw-r--r--   0      502       20      168 2023-04-22 13:43:05.000000 binooculars-0.0.1/docs/source/modules/cluster.rst
--rw-r--r--   0      502       20      165 2023-04-22 13:43:19.000000 binooculars-0.0.1/docs/source/modules/linear.rst
--rw-r--r--   0      502       20      868 2023-04-22 14:19:52.000000 binooculars-0.0.1/pyproject.toml
--rw-r--r--   0      502       20      230 2023-04-17 11:29:29.000000 binooculars-0.0.1/python/binoculars/__init__.py
--rw-r--r--   0      502       20       49 2023-04-17 08:03:08.000000 binooculars-0.0.1/python/binoculars/cluster/__init__.py
--rw-r--r--   0      502       20     3403 2023-04-17 12:50:31.000000 binooculars-0.0.1/python/binoculars/cluster/cluster.py
--rw-r--r--   0      502       20      110 2023-04-17 08:05:14.000000 binooculars-0.0.1/python/binoculars/linear/__init__.py
--rw-r--r--   0      502       20     4016 2023-04-17 15:01:06.000000 binooculars-0.0.1/python/binoculars/linear/linear.py
--rw-r--r--   0      502       20      171 2023-04-17 07:50:52.000000 binooculars-0.0.1/src/cluster/dist.rs
--rw-r--r--   0      502       20     3572 2023-04-17 07:50:52.000000 binooculars-0.0.1/src/cluster/kmeans.rs
--rw-r--r--   0      502       20      572 2023-04-17 11:12:47.000000 binooculars-0.0.1/src/lib.rs
--rw-r--r--   0      502       20     5552 2023-04-14 08:20:03.000000 binooculars-0.0.1/src/linear/regression.rs
--rw-r--r--   0      502       20      985 2023-04-14 08:20:03.000000 binooculars-0.0.1/src/linear/utils.rs
--rw-r--r--   0      502       20    13687 2023-04-22 14:20:07.000000 binooculars-0.0.1/Cargo.lock
--rw-r--r--   0        0        0     1208 1970-01-01 00:00:00.000000 binooculars-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 binooculars-0.0.2/Cargo.toml
+-rw-r--r--   0      502       20      946 2023-04-14 08:20:03.000000 binooculars-0.0.2/.github/workflows/python.yml
+-rw-r--r--   0      502       20      692 2023-04-17 08:38:36.000000 binooculars-0.0.2/.github/workflows/rust.yml
+-rw-r--r--   0      502       20      685 2023-04-01 12:28:12.000000 binooculars-0.0.2/.gitignore
+-rw-r--r--   0      502       20      398 2023-04-17 12:28:30.000000 binooculars-0.0.2/.readthedocs.yaml
+-rw-r--r--   0      502       20      872 2023-04-17 08:36:59.000000 binooculars-0.0.2/CHANGELOG.md
+-rw-r--r--   0      502       20      347 2023-04-17 07:50:52.000000 binooculars-0.0.2/Pipfile
+-rw-r--r--   0      502       20    91556 2023-04-17 11:43:26.000000 binooculars-0.0.2/Pipfile.lock
+-rw-r--r--   0      502       20      753 2023-04-17 07:50:52.000000 binooculars-0.0.2/README.md
+-rw-r--r--   0      502       20      638 2023-04-22 13:37:14.000000 binooculars-0.0.2/docs/Makefile
+-rw-r--r--   0      502       20      804 2023-04-22 13:37:14.000000 binooculars-0.0.2/docs/make.bat
+-rw-r--r--   0      502       20      959 2023-04-22 13:57:34.000000 binooculars-0.0.2/docs/source/conf.py
+-rw-r--r--   0      502       20      394 2023-04-22 13:48:43.000000 binooculars-0.0.2/docs/source/index.rst
+-rw-r--r--   0      502       20      168 2023-04-22 13:43:05.000000 binooculars-0.0.2/docs/source/modules/cluster.rst
+-rw-r--r--   0      502       20      165 2023-04-22 13:43:19.000000 binooculars-0.0.2/docs/source/modules/linear.rst
+-rw-r--r--   0      502       20      868 2023-04-22 14:28:45.000000 binooculars-0.0.2/pyproject.toml
+-rw-r--r--   0      502       20      235 2023-04-22 14:27:16.000000 binooculars-0.0.2/python/binooculars/__init__.py
+-rw-r--r--   0      502       20       49 2023-04-17 08:03:08.000000 binooculars-0.0.2/python/binooculars/cluster/__init__.py
+-rw-r--r--   0      502       20     3404 2023-04-22 14:25:59.000000 binooculars-0.0.2/python/binooculars/cluster/cluster.py
+-rw-r--r--   0      502       20      110 2023-04-17 08:05:14.000000 binooculars-0.0.2/python/binooculars/linear/__init__.py
+-rw-r--r--   0      502       20     4017 2023-04-22 14:27:00.000000 binooculars-0.0.2/python/binooculars/linear/linear.py
+-rw-r--r--   0      502       20      171 2023-04-17 07:50:52.000000 binooculars-0.0.2/src/cluster/dist.rs
+-rw-r--r--   0      502       20     3572 2023-04-17 07:50:52.000000 binooculars-0.0.2/src/cluster/kmeans.rs
+-rw-r--r--   0      502       20      573 2023-04-22 14:25:46.000000 binooculars-0.0.2/src/lib.rs
+-rw-r--r--   0      502       20     5552 2023-04-14 08:20:03.000000 binooculars-0.0.2/src/linear/regression.rs
+-rw-r--r--   0      502       20      985 2023-04-14 08:20:03.000000 binooculars-0.0.2/src/linear/utils.rs
+-rw-r--r--   0      502       20    13687 2023-04-22 14:20:07.000000 binooculars-0.0.2/Cargo.lock
+-rw-r--r--   0        0        0     1208 1970-01-01 00:00:00.000000 binooculars-0.0.2/PKG-INFO
```

### Comparing `binooculars-0.0.1/.github/workflows/python.yml` & `binooculars-0.0.2/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `binooculars-0.0.1/.github/workflows/rust.yml` & `binooculars-0.0.2/.github/workflows/rust.yml`

 * *Files identical despite different names*

### Comparing `binooculars-0.0.1/.gitignore` & `binooculars-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `binooculars-0.0.1/CHANGELOG.md` & `binooculars-0.0.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `binooculars-0.0.1/Pipfile.lock` & `binooculars-0.0.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `binooculars-0.0.1/README.md` & `binooculars-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `binooculars-0.0.1/docs/Makefile` & `binooculars-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `binooculars-0.0.1/docs/make.bat` & `binooculars-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `binooculars-0.0.1/docs/source/conf.py` & `binooculars-0.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `binooculars-0.0.1/pyproject.toml` & `binooculars-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15", "setuptools", "wheel", "setuptools-rust"]
 build-backend = "maturin"
 
 [project]
 name = "binooculars"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Benedek Harsanyi"},
 ]
 description = "A tiny, yet blazingly fast machine learning library written in Rust with Python interface."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `binooculars-0.0.1/python/binoculars/cluster/cluster.py` & `binooculars-0.0.2/python/binooculars/cluster/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module for kmeans."""
 
 from __future__ import annotations
 
-from binoculars import KMeansRust
+from binooculars import KMeansRust
 
 
 class KMeans:
     """KMeans clustering with Rust backend.
 
     K-means tries to find the centroids of the clusters by minimizing the
     the within-cluster sum-of-squares criterion. The algorithm can be stated
```

### Comparing `binooculars-0.0.1/python/binoculars/linear/linear.py` & `binooculars-0.0.2/python/binooculars/linear/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module for linear regression."""
 
 from __future__ import annotations
 
-from binoculars import LinearRegressionRust, LogisticRegressionRust
+from binooculars import LinearRegressionRust, LogisticRegressionRust
 
 
 class LinearRegression:
     """Least squares linear regression with Rust backend."""
 
     def __init__(self) -> None:
         self._rustobj = LinearRegressionRust()
```

### Comparing `binooculars-0.0.1/src/cluster/kmeans.rs` & `binooculars-0.0.2/src/cluster/kmeans.rs`

 * *Files identical despite different names*

### Comparing `binooculars-0.0.1/src/lib.rs` & `binooculars-0.0.2/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,14 @@
     mod dist;
     pub mod kmeans;
     pub use crate::cluster::kmeans::KMeansRust;
 }
 
 /// This module is implemented in Rust.
 #[pymodule]
-#[pyo3(name = "binoculars")]
+#[pyo3(name = "binooculars")]
 fn my_extension(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<linear::LinearRegressionRust>()?;
     m.add_class::<linear::LogisticRegressionRust>()?;
     m.add_class::<cluster::KMeansRust>()?;
     Ok(())
 }
```

### Comparing `binooculars-0.0.1/src/linear/regression.rs` & `binooculars-0.0.2/src/linear/regression.rs`

 * *Files identical despite different names*

### Comparing `binooculars-0.0.1/src/linear/utils.rs` & `binooculars-0.0.2/src/linear/utils.rs`

 * *Files identical despite different names*

### Comparing `binooculars-0.0.1/Cargo.lock` & `binooculars-0.0.2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `binooculars-0.0.1/PKG-INFO` & `binooculars-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binooculars
-Version: 0.0.1
+Version: 0.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: A tiny, yet blazingly fast machine learning library written in Rust with Python interface.
 Author: Benedek Harsanyi
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

