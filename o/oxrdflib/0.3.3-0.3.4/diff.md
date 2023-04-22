# Comparing `tmp/oxrdflib-0.3.3.tar.gz` & `tmp/oxrdflib-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxrdflib-0.3.3.tar", last modified: Mon Mar 20 18:00:38 2023, max compression
+gzip compressed data, was "oxrdflib-0.3.4.tar", last modified: Sat Apr 22 05:32:22 2023, max compression
```

## Comparing `oxrdflib-0.3.3.tar` & `oxrdflib-0.3.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:00:38.071156 oxrdflib-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:00:38.071156 oxrdflib-0.3.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:00:38.071156 oxrdflib-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-03-20 18:00:38.071156 oxrdflib-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:00:38.071156 oxrdflib-0.3.3/oxrdflib/
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/oxrdflib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/oxrdflib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:00:38.071156 oxrdflib-0.3.3/oxrdflib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-03-20 18:00:38.000000 oxrdflib-0.3.3/oxrdflib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-20 18:00:38.000000 oxrdflib-0.3.3/oxrdflib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 18:00:38.000000 oxrdflib-0.3.3/oxrdflib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-20 18:00:38.000000 oxrdflib-0.3.3/oxrdflib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-20 18:00:38.000000 oxrdflib-0.3.3/oxrdflib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-20 18:00:38.000000 oxrdflib-0.3.3/oxrdflib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 18:00:38.071156 oxrdflib-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:00:38.071156 oxrdflib-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/tests/test_graph_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/tests/test_sparql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-03-20 18:00:29.000000 oxrdflib-0.3.3/tests/test_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/oxrdflib/
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/oxrdflib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/oxrdflib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/oxrdflib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-22 05:32:22.000000 oxrdflib-0.3.4/oxrdflib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-22 05:32:22.000000 oxrdflib-0.3.4/oxrdflib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 05:32:22.000000 oxrdflib-0.3.4/oxrdflib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-22 05:32:22.000000 oxrdflib-0.3.4/oxrdflib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-22 05:32:22.000000 oxrdflib-0.3.4/oxrdflib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-22 05:32:22.000000 oxrdflib-0.3.4/oxrdflib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/tests/test_graph_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/tests/test_sparql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/tests/test_store.py
```

### Comparing `oxrdflib-0.3.3/.github/workflows/build.yml` & `oxrdflib-0.3.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.3/.pre-commit-config.yaml` & `oxrdflib-0.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.3/CHANGELOG.md` & `oxrdflib-0.3.4/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## [0.3.4] - 2023-04-22
+
+### Changed
+- Fixes support of rdflib `Query` object in `Store.query`.
+
+
 ## [0.3.3] - 2023-03-20
 
 ### Added
 - Implements directly `Store.addN` method.
 - Allows to Allows to inject the `pyoxigraph.Store` object directly into `OxigraphStore`.
 
 ### Changed
```

### Comparing `oxrdflib-0.3.3/LICENSE.md` & `oxrdflib-0.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.3/PKG-INFO` & `oxrdflib-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxrdflib
-Version: 0.3.3
+Version: 0.3.4
 Summary: rdflib stores based on pyoxigraph
 Author-email: Tpt <thomas@pellissier-tanon.fr>
 License: BSD-3-Clause
 Project-URL: Changelog, https://github.com/oxigraph/oxrdflib/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/oxigraph/oxrdflib/blob/main/README.md
 Project-URL: Homepage, https://github.com/oxigraph/oxrdflib
 Project-URL: Source, https://github.com/oxigraph/oxrdflib
```

### Comparing `oxrdflib-0.3.3/README.md` & `oxrdflib-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.3/oxrdflib/__init__.py` & `oxrdflib-0.3.4/oxrdflib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         self,
         query: Union[Query, str],
         initNs: Mapping[str, Any],  # noqa: N803
         initBindings: Mapping[str, Identifier],  # noqa: N803
         queryGraph: str,  # noqa: N803
         **kwargs: Any,
     ) -> "Result":
-        if isinstance(queryGraph, Query) or kwargs:
+        if isinstance(query, Query) or kwargs:
             raise NotImplementedError
         init_ns = dict(self._namespace_for_prefix, **initNs)
         query = "".join(f"PREFIX {prefix}: <{namespace}>\n" for prefix, namespace in init_ns.items()) + query
         if initBindings:
             query += "\nVALUES ( {} ) {{ ({}) }}".format(
                 " ".join(f"?{k}" for k in initBindings), " ".join(v.n3() for v in initBindings.values())
             )
```

### Comparing `oxrdflib-0.3.3/oxrdflib.egg-info/PKG-INFO` & `oxrdflib-0.3.4/oxrdflib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxrdflib
-Version: 0.3.3
+Version: 0.3.4
 Summary: rdflib stores based on pyoxigraph
 Author-email: Tpt <thomas@pellissier-tanon.fr>
 License: BSD-3-Clause
 Project-URL: Changelog, https://github.com/oxigraph/oxrdflib/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/oxigraph/oxrdflib/blob/main/README.md
 Project-URL: Homepage, https://github.com/oxigraph/oxrdflib
 Project-URL: Source, https://github.com/oxigraph/oxrdflib
```

### Comparing `oxrdflib-0.3.3/pyproject.toml` & `oxrdflib-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.3/tests/test_dataset.py` & `oxrdflib-0.3.4/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.3/tests/test_graph.py` & `oxrdflib-0.3.4/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.3/tests/test_graph_context.py` & `oxrdflib-0.3.4/tests/test_graph_context.py`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.3/tests/test_sparql.py` & `oxrdflib-0.3.4/tests/test_sparql.py`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.3/tests/test_store.py` & `oxrdflib-0.3.4/tests/test_store.py`

 * *Files identical despite different names*

