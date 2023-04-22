# Comparing `tmp/networkx_robustness-0.0.3.tar.gz` & `tmp/networkx_robustness-0.0.4.tar.gz`

## Comparing `networkx_robustness-0.0.3.tar` & `networkx_robustness-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 networkx_robustness-0.0.3/src/networkx_robustness/__init__.py
--rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 networkx_robustness-0.0.3/src/networkx_robustness/networkx_robustness.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 networkx_robustness-0.0.3/LICENSE
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 networkx_robustness-0.0.3/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 networkx_robustness-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 networkx_robustness-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 networkx_robustness-0.0.4/src/networkx_robustness/__init__.py
+-rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 networkx_robustness-0.0.4/src/networkx_robustness/networkx_robustness.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 networkx_robustness-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 networkx_robustness-0.0.4/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 networkx_robustness-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 networkx_robustness-0.0.4/PKG-INFO
```

### Comparing `networkx_robustness-0.0.3/src/networkx_robustness/networkx_robustness.py` & `networkx_robustness-0.0.4/src/networkx_robustness/networkx_robustness.py`

 * *Files identical despite different names*

### Comparing `networkx_robustness-0.0.3/LICENSE` & `networkx_robustness-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `networkx_robustness-0.0.3/README.md` & `networkx_robustness-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,29 @@
 
 The package can be installed using the pip package manager and requires Python 3.7 or greater.
 
 ```bash
 pip install networkx-robustness
 ```
 
+## Example
+
+An example of importing and using the package is shown below
+
+```python
+import networkx as nx
+from networkx_robustness import networkx_robustness
+
+#Random NetworkX graph with 100 nodes
+G = nx.gnp_random_graph(100, 0.5)
+
+#Simulate a random attack on 20 nodes
+initial, frac, apl = networkx_robustness.simulate_random_attack(G, attack_fraction=0.2)
+```
+
 ## Simulating random attacks
 
 ```python
 initial, frac, apl = simulate_random_attack(G=None, attack_fraction=0.1, weight=None)
     """
     Simulate random attack on a network
     :param G: networkx graph
```

### Comparing `networkx_robustness-0.0.3/pyproject.toml` & `networkx_robustness-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "networkx_robustness"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Tejas Santanam", email="santanam.tejas@gmail.com" },
 ]
 description = "A package for simulating network attacks on NetworkX graphs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `networkx_robustness-0.0.3/PKG-INFO` & `networkx_robustness-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networkx_robustness
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for simulating network attacks on NetworkX graphs
 Project-URL: Homepage, https://github.com/tsantanam/networkx-robustness
 Project-URL: Bug Tracker, https://github.com/tsantanam/networkx-robustness/issues
 Author-email: Tejas Santanam <santanam.tejas@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,29 @@
 
 The package can be installed using the pip package manager and requires Python 3.7 or greater.
 
 ```bash
 pip install networkx-robustness
 ```
 
+## Example
+
+An example of importing and using the package is shown below
+
+```python
+import networkx as nx
+from networkx_robustness import networkx_robustness
+
+#Random NetworkX graph with 100 nodes
+G = nx.gnp_random_graph(100, 0.5)
+
+#Simulate a random attack on 20 nodes
+initial, frac, apl = networkx_robustness.simulate_random_attack(G, attack_fraction=0.2)
+```
+
 ## Simulating random attacks
 
 ```python
 initial, frac, apl = simulate_random_attack(G=None, attack_fraction=0.1, weight=None)
     """
     Simulate random attack on a network
     :param G: networkx graph
```

