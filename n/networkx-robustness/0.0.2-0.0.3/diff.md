# Comparing `tmp/networkx_robustness-0.0.2.tar.gz` & `tmp/networkx_robustness-0.0.3.tar.gz`

## Comparing `networkx_robustness-0.0.2.tar` & `networkx_robustness-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 networkx_robustness-0.0.2/src/networkx_robustness/__init__.py
--rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 networkx_robustness-0.0.2/src/networkx_robustness/networkx_robustness.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 networkx_robustness-0.0.2/LICENSE
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 networkx_robustness-0.0.2/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 networkx_robustness-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 networkx_robustness-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 networkx_robustness-0.0.3/src/networkx_robustness/__init__.py
+-rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 networkx_robustness-0.0.3/src/networkx_robustness/networkx_robustness.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 networkx_robustness-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 networkx_robustness-0.0.3/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 networkx_robustness-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 networkx_robustness-0.0.3/PKG-INFO
```

### Comparing `networkx_robustness-0.0.2/src/networkx_robustness/networkx_robustness.py` & `networkx_robustness-0.0.3/src/networkx_robustness/networkx_robustness.py`

 * *Files identical despite different names*

### Comparing `networkx_robustness-0.0.2/LICENSE` & `networkx_robustness-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `networkx_robustness-0.0.2/README.md` & `networkx_robustness-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# networkx_robustness
+# networkx-robustness
 
 A package for simulating network attacks on NetworkX graphs. The current supported attacks include random attacks and targeted attacks on nodes with the highest degree centrality, betweenness centrality, closeness centrality, and eigenvector centrality. Attack functions return the initial fraction of nodes in the giant component, a list of the fraction of nodes in the giant component after each node removal, and a list of the average path length in the giant component after each node removal.
 
 ## Installation
 
 The package can be installed using the pip package manager and requires Python 3.7 or greater.
 
 ```bash
-pip install networkx_robustness
+pip install networkx-robustness
 ```
 
 ## Simulating random attacks
 
 ```python
 initial, frac, apl = simulate_random_attack(G=None, attack_fraction=0.1, weight=None)
     """
```

### Comparing `networkx_robustness-0.0.2/pyproject.toml` & `networkx_robustness-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "networkx_robustness"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Tejas Santanam", email="santanam.tejas@gmail.com" },
 ]
 description = "A package for simulating network attacks on NetworkX graphs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `networkx_robustness-0.0.2/PKG-INFO` & `networkx_robustness-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: networkx_robustness
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for simulating network attacks on NetworkX graphs
 Project-URL: Homepage, https://github.com/tsantanam/networkx-robustness
 Project-URL: Bug Tracker, https://github.com/tsantanam/networkx-robustness/issues
 Author-email: Tejas Santanam <santanam.tejas@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# networkx_robustness
+# networkx-robustness
 
 A package for simulating network attacks on NetworkX graphs. The current supported attacks include random attacks and targeted attacks on nodes with the highest degree centrality, betweenness centrality, closeness centrality, and eigenvector centrality. Attack functions return the initial fraction of nodes in the giant component, a list of the fraction of nodes in the giant component after each node removal, and a list of the average path length in the giant component after each node removal.
 
 ## Installation
 
 The package can be installed using the pip package manager and requires Python 3.7 or greater.
 
 ```bash
-pip install networkx_robustness
+pip install networkx-robustness
 ```
 
 ## Simulating random attacks
 
 ```python
 initial, frac, apl = simulate_random_attack(G=None, attack_fraction=0.1, weight=None)
     """
```

