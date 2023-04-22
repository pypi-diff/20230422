# Comparing `tmp/pytreeclass-0.3.0.tar.gz` & `tmp/pytreeclass-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.3.0.tar", last modified: Wed Apr 19 23:59:42 2023, max compression
+gzip compressed data, was "pytreeclass-0.3.1.tar", last modified: Sat Apr 22 05:26:51 2023, max compression
```

## Comparing `pytreeclass-0.3.0.tar` & `pytreeclass-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:42.322212 pytreeclass-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29135 2023-04-19 23:59:42.322212 pytreeclass-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28259 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:42.318212 pytreeclass-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:42.318212 pytreeclass-0.3.0/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:42.322212 pytreeclass-0.3.0/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16425 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/pytreeclass/_src/tree_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/pytreeclass/_src/tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/pytreeclass/_src/tree_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31417 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/pytreeclass/_src/tree_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:42.318212 pytreeclass-0.3.0/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29135 2023-04-19 23:59:42.000000 pytreeclass-0.3.0/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-19 23:59:42.000000 pytreeclass-0.3.0/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:59:42.000000 pytreeclass-0.3.0/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:59:42.000000 pytreeclass-0.3.0/pytreeclass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 23:59:42.000000 pytreeclass-0.3.0/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-19 23:59:42.000000 pytreeclass-0.3.0/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:59:42.322212 pytreeclass-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:42.322212 pytreeclass-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14936 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-19 23:59:32.000000 pytreeclass-0.3.0/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:51.105200 pytreeclass-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-04-22 05:26:51.105200 pytreeclass-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:51.101200 pytreeclass-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:51.101200 pytreeclass-0.3.1/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:51.101200 pytreeclass-0.3.1/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16700 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/pytreeclass/_src/tree_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/pytreeclass/_src/tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18188 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/pytreeclass/_src/tree_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30822 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/pytreeclass/_src/tree_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:51.101200 pytreeclass-0.3.1/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-04-22 05:26:51.000000 pytreeclass-0.3.1/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-22 05:26:51.000000 pytreeclass-0.3.1/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 05:26:51.000000 pytreeclass-0.3.1/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 05:26:51.000000 pytreeclass-0.3.1/pytreeclass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-22 05:26:51.000000 pytreeclass-0.3.1/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-22 05:26:51.000000 pytreeclass-0.3.1/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 05:26:51.105200 pytreeclass-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:51.101200 pytreeclass-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17440 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.3.0/LICENSE` & `pytreeclass-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.0/PKG-INFO` & `pytreeclass-0.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: pytreeclass
-Version: 0.3.0
-Summary: JAX compatible dataclass.
-Home-page: https://github.com/ASEM000/pytreeclass
-Author: Mahmoud Asem
-Author-email: asem00@kaist.ac.kr
-License: Apache-2.0
-Keywords: python machine-learning pytorch jax
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!-- <h1 align="center" style="font-family:Monospace" >Py🌲Class</h1> -->
 <h5 align="center">
 <img width="250px" src="https://user-images.githubusercontent.com/48389287/227880173-bf78c02c-d28b-4cf4-95e6-fa49b82a43a1.svg"> <br>
 
 <br>
 
 [**Installation**](#installation)
@@ -32,15 +9,15 @@
 |[**Quick Example**](#quick_example)
 |[**StatefulComputation**](#stateful_computation)
 |[**More**](#more)
 |[**Acknowledgements**](#acknowledgements)
 
 ![Tests](https://github.com/ASEM000/pytreeclass/actions/workflows/tests.yml/badge.svg)
 ![pyver](https://img.shields.io/badge/python-3.8%203.9%203.10%203.11_-red)
-![pyver](https://img.shields.io/badge/jax-0.4+-red)
+![pyver](https://img.shields.io/badge/jax-0.4.7+-red)
 ![codestyle](https://img.shields.io/badge/codestyle-black-black)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ASEM000/PyTreeClass/blob/main/assets/intro.ipynb)
 [![Downloads](https://pepy.tech/badge/pytreeclass)](https://pepy.tech/project/pytreeclass)
 [![codecov](https://codecov.io/gh/ASEM000/pytreeclass/branch/main/graph/badge.svg?token=TZBRMO0UQH)](https://codecov.io/gh/ASEM000/pytreeclass)
 [![Documentation Status](https://readthedocs.org/projects/pytreeclass/badge/?version=latest)](https://pytreeclass.readthedocs.io/en/latest/?badge=latest)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ASEM000/pytreeclass)
 [![DOI](https://zenodo.org/badge/512717921.svg)](https://zenodo.org/badge/latestdoi/512717921)
@@ -76,47 +53,83 @@
 
 ## ⏩ Quick Example <a id="quick_example">
 
 ### 🏗️ Simple Tree example
 
 <div align="center">
 <table>
-<tr><td align="center">Code</td> <td align="center">PyTree representation</td></tr>
+<tr><td align="center"></td> <td align="center"></td></tr>
 <tr>
 <td>
 
 ```python
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
 
+
 class Tree(pytc.TreeClass):
-    a:int = 1
-    b:tuple[float] = (2.,3.)
-    c:jax.Array = jnp.array([4.,5.,6.])
+    a: int = 1
+    b: tuple = (2, 3.)
+    c: jax.Array = jnp.array([4., 5., 6.])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
 
+
 tree = Tree()
-```
+mask = jax.tree_map(lambda x: x > 5, tree)
+tree = tree \
+       .at["a"].set(10) \
+       .at["b"].at[0].set(10) \
+       .at[mask].set(100)
 
-</td>
+print(tree)
+# Tree(a=10, b=(10, 3.0), c=[  4.   5. 100.])
 
-<td>
+print(pytc.tree_diagram(tree))
+# Tree
+# ├── .a=10
+# ├── .b:tuple
+# │   ├── [0]=10
+# │   └── [1]=3.0
+# └── .c=f32[3](μ=36.33, σ=45.02, ∈[4.00,100.00])
 
-```python
-# leaves are parameters
+print(pytc.tree_summary(tree))
+# ┌─────┬──────┬─────┐
+# │Name │Type  │Count│
+# ├─────┼──────┼─────┤
+# │.a   │int   │1    │
+# ├─────┼──────┼─────┤
+# │.b[0]│int   │1    │
+# ├─────┼──────┼─────┤
+# │.b[1]│float │1    │
+# ├─────┼──────┼─────┤
+# │.c   │f32[3]│3    │
+# ├─────┼──────┼─────┤
+# │Σ    │Tree  │6    │
+# └─────┴──────┴─────┘
+
+
+# ** pass it to jax transformations **
+
+# freeze all non-differentiable parameters to make it
+# work with jax trnasformations
+mask = jax.tree_map(pytc.is_nondiff, tree)
+tree = tree.at[mask].apply(pytc.freeze)
 
-Tree
-    ├── a=1
-    ├── b:tuple
-    │   ├── [0]=2.0
-    │   └── [1]=3.0
-    └── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
+@jax.jit
+@jax.grad
+def sum_tree(tree:Tree, x):
+    # unfreeze before calling tree
+    tree = tree.at[...].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)
+    return sum(tree(x))
+
+print(sum_tree(tree, 1.0))
+# Tree(a=#10, b=(#10, 0.0), c=[1. 1. 1.])
 ```
 
 </td>
 
 </tr>
 </table>
 </div>
@@ -140,52 +153,52 @@
 <td>
 
 ```python
 print(pytc.tree_summary(tree, depth=1))
 ┌────┬──────┬─────┐
 │Name│Type  │Count│
 ├────┼──────┼─────┤
-│a   │int   │1    │
+│.a  │int   │1    │
 ├────┼──────┼─────┤
-│b   │tuple │1    │
+│.b  │tuple │1    │
 ├────┼──────┼─────┤
-│c   │f32[3]│3    │
+│.c  │f32[3]│3    │
 ├────┼──────┼─────┤
 │Σ   │Tree  │5    │
 └────┴──────┴─────┘
 ```
 
 </td>
 
 <td>
 
 ```python
 
 print(pytc.tree_diagram(tree, depth=1))
 Tree
-├── a=1
-├── b=(...)
-└── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
+├── .a=1
+├── .b=(...)
+└── .c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
 ```
 
  </td>
 
 <td>
 
 ```python
 print(pytc.tree_mermaid(tree, depth=1))
 ```
 
 ```mermaid
 
 flowchart LR
     id0(<b>Tree</b>)
-    id0 --- id1("</b>a=1</b>")
-    id0 --- id2("</b>b=(...)</b>")
-    id0 --- id3("</b>c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])</b>")
+    id0 --- id1("</b>.a=1</b>")
+    id0 --- id2("</b>.b=(...)</b>")
+    id0 --- id3("</b>.c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])</b>")
 ```
 
 </td>
 
 <td>
 
 ```python
@@ -208,41 +221,41 @@
 
 <tr>
 
 <td>
 
 ```python
 print(pytc.tree_summary(tree, depth=2))
-┌────┬──────┬─────┐
-│Name│Type  │Count│
-├────┼──────┼─────┤
-│a   │int   │1    │
-├────┼──────┼─────┤
-│b[0]│float │1    │
-├────┼──────┼─────┤
-│b[1]│float │1    │
-├────┼──────┼─────┤
-│c   │f32[3]│3    │
-├────┼──────┼─────┤
-│Σ   │Tree  │6    │
-└────┴──────┴─────┘
+┌─────┬──────┬─────┐
+│Name │Type  │Count│
+├─────┼──────┼─────┤
+│.a   │int   │1    │
+├─────┼──────┼─────┤
+│.b[0]│int   │1    │
+├─────┼──────┼─────┤
+│.b[1]│float │1    │
+├─────┼──────┼─────┤
+│.c   │f32[3]│3    │
+├─────┼──────┼─────┤
+│Σ    │Tree  │6    │
+└─────┴──────┴─────┘
 ```
 
 </td>
 
 <td>
 
 ```python
 print(pytc.tree_diagram(tree, depth=2))
 Tree
-├── a=1
-├── b:tuple
+├── .a=1
+├── .b:tuple
 │   ├── [0]=2.0
 │   └── [1]=3.0
-└── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
+└── .c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
 ```
 
 </td>
 
 <td>
 
 ```python
@@ -250,17 +263,17 @@
 ```
 
 ```mermaid
 flowchart LR
     id2 --- id3("</b>[0]=2.0</b>")
     id2 --- id4("</b>[1]=3.0</b>")
     id0(<b>Tree</b>)
-    id0 --- id1("</b>a=1</b>")
-    id0 --- id2("</b>b:tuple</b>")
-    id0 --- id5("</b>c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])</b>")
+    id0 --- id1("</b>.a=1</b>")
+    id0 --- id2("</b>.b:tuple</b>")
+    id0 --- id5("</b>.c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])</b>")
 ```
 
 </td>
 
 <td>
 
 ```python
@@ -414,14 +427,57 @@
 print(tree.at[1].at[0].set(10))
 # Tree(a=1, b=(10, 3.0), c=[4. 5. 6.])
 
 print(tree.at[1].at[0].apply(lambda x: 10))
 # Tree(a=1, b=(10, 3.0), c=[4. 5. 6.])
 ```
 
+### Mix, match , and chain index update
+
+```python
+
+import jax
+import jax.numpy as jnp
+import pytreeclass as pytc
+
+class Tree(pytc.TreeClass):
+    a: int = 1
+    b: str = "b"
+    c: float = 1.0
+    d: bool = True
+    e: tuple = (1, 2, 3)
+    f: jax.Array = jax.numpy.array([1, 2, 3])
+
+tree = Tree()
+
+integer_mask = jax.tree_util.tree_map(lambda x: isinstance(x, int), tree)
+
+tree = (
+    tree
+    .at["a"].set(10)
+    .at["b"].set("B")
+    .at["c"].set(10.0)
+    .at["d"].set(False)
+    .at["e"].at[0].set(10)  # set first element of tuple to 10
+    .at["f"].apply(jnp.sin)  # apply to all elements in array
+    .at[integer_mask].apply(float)  # cast all `int` to `float`
+)
+
+print(tree)
+# Tree(
+#   a=10.0,
+#   b=B,
+#   c=10.0,
+#   d=0.0,
+#   e=(10.0, 2.0, 3.0),
+#   f=[0.841471  0.9092974 0.14112  ]
+# )
+
+```
+
 </details>
 
 <details>
 
 <summary>
 
 ## 📜 Stateful computations<a id="stateful_computation"></a> </summary>
@@ -456,83 +512,14 @@
 print(counter.calls) # 10
 ```
 
 </details>
 
 ## ➕ More<a id="more"></a>
 
-<details><summary>[Advanced] Register custom user-defined classes to work with visualization and indexing tools. </summary>
-
-Similar to [`jax.tree_util.register_pytree_node`](https://jax.readthedocs.io/en/latest/pytrees.html#extending-pytrees), `PyTreeClass` register common data structures and `treeclass` wrapped classes to figure out how to define the names, types, and index of certain leaf along its path.
-
-Here is an example of registering
-
-```python
-
-class Tree:
-    def __init__(self, a, b):
-        self.a = a
-        self.b = b
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(a={self.a}, b={self.b})"
-
-
-# jax flatten rule
-def tree_flatten(tree):
-    return (tree.a, tree.b), None
-
-# jax unflatten rule
-def tree_unflatten(_, children):
-    return Tree(*children)
-
-# PyTreeClass flatten rule
-def pytc_tree_flatten(tree):
-    names = ("a", "b") # or (`None`, `None`) if name is not defined
-    types = (type(tree.a), type(tree.b))
-    indices = (0,1)  # or (`None`, `None`) if index is not defined
-    return [*zip(names, types, indices)]
-
-
-# Register with `jax`
-jax.tree_util.register_pytree_node(Tree, tree_flatten, tree_unflatten)
-
-# Register the `Tree` class trace function to support indexing
-pytc.register_pytree_node_trace(Tree, pytc_tree_flatten)
-
-tree = Tree(1, 2)
-
-# works with jax
-jax.tree_util.tree_leaves(tree)  # [1, 2]
-
-# works with PyTreeClass viz tools
-print(pytc.tree_summary(tree))
-
-# ┌────┬────┬─────┬──────┐
-# │Name│Type│Count│Size  │
-# ├────┼────┼─────┼──────┤
-# │a   │int │1    │28.00B│
-# ├────┼────┼─────┼──────┤
-# │b   │int │1    │28.00B│
-# ├────┼────┼─────┼──────┤
-# │Σ   │Tree│2    │56.00B│
-# └────┴────┴─────┴──────┘
-
-```
-
-After registeration, you can use internal tools like
-
-- `pytc.tree_map_with_trace`
-- `pytc.tree_leaves_with_trace`
-- `pytc.tree_flatten_with_trace`
-
-More details on that soon.
-
-</details>
-
 <details> <summary>Validate or convert inputs using callbacks</summary>
 
 `PyTreeClass` includes `callbacks` in the `field` to apply a sequence of functions on input at setting the attribute stage. The callback is quite useful in several cases, for instance, to ensure a certain input type within a valid range. See example:
 
 ```python
 import jax
 import pytreeclass as pytc
@@ -806,70 +793,70 @@
 ```
 
 </details>
 
 <details><summary>Use PyTreeClass components with other libraries</summary>
 
 ```python
+
 import jax
 import pytreeclass as pytc
 from flax import struct
 
+import jax
+import pytreeclass as pytc
+from flax import struct
+
+# note that flax is registered with `jax.tree_util.register_pytree_with_keys`
+# otherwise for arbitrary objects you need to do the key registration
+
 @struct.dataclass
 class FlaxTree:
     a:int = 1
     b:tuple[float] = (2.,3.)
     c:jax.Array = jax.numpy.array([4.,5.,6.])
 
     def __repr__(self) -> str:
         return pytc.tree_repr(self)
     def __str__(self) -> str:
         return pytc.tree_str(self)
     @property
     def at(self):
         return pytc.tree_indexer(self)
 
-def pytc_flatten_rule(tree):
-    names =("a","b","c")
-    types = map(type, (tree.a, tree.b, tree.c))
-    indices = range(3)  # make it indexable like namedtuple
-    return [*zip(names, types, indices)]
-
-pytc.register_pytree_node_trace(FlaxTree, pytc_flatten_rule)
-
 flax_tree = FlaxTree()
 
 print(f"{flax_tree!r}")
 # FlaxTree(a=1, b=(2.0, 3.0), c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00]))
 
 print(f"{flax_tree!s}")
 # FlaxTree(a=1, b=(2.0, 3.0), c=[4. 5. 6.])
 
 print(pytc.tree_diagram(flax_tree))
 # FlaxTree
-# ├── a=1
-# ├── b:tuple
+# ├── .a=1
+# ├── .b:tuple
 # │   ├── [0]=2.0
 # │   └── [1]=3.0
-# └── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
+# └── .c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
 
 print(pytc.tree_summary(flax_tree))
-# ┌────┬────────┬─────┐
-# │Name│Type    │Count│
-# ├────┼────────┼─────┤
-# │a   │int     │1    │
-# ├────┼────────┼─────┤
-# │b[0]│float   │1    │
-# ├────┼────────┼─────┤
-# │b[1]│float   │1    │
-# ├────┼────────┼─────┤
-# │c   │f32[3]  │3    │
-# ├────┼────────┼─────┤
-# │Σ   │FlaxTree│6    │
-# └────┴────────┴─────┘
+# ┌─────┬────────┬─────┐
+# │Name │Type    │Count│
+# ├─────┼────────┼─────┤
+# │.a   │int     │1    │
+# ├─────┼────────┼─────┤
+# │.b[0]│float   │1    │
+# ├─────┼────────┼─────┤
+# │.b[1]│float   │1    │
+# ├─────┼────────┼─────┤
+# │.c   │f32[3]  │3    │
+# ├─────┼────────┼─────┤
+# │Σ    │FlaxTree│6    │
+# └─────┴────────┴─────┘
 
 flax_tree.at[0].get()
 # FlaxTree(a=1, b=(None, None), c=None)
 
 flax_tree.at["a"].set(10)
 # FlaxTree(a=10, b=(2.0, 3.0), c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00]))
 ```
@@ -884,117 +871,19 @@
 <table>
 
 <tr><td align="center">CPU</td><td align="center">GPU</td></tr>
 
 <tr>
 
 <td><img src='assets/benchmark_cpu.png'></td>
-<td><img src='assets/benchmark_gpu.png'></td>
 
 </tr>
 
 </table>
 
 </details>
 
-<details> 
-<summary>Use tree_map_with_trace</summary>
-
-V0.2 of `PyTreeClass` register common python datatypes and `treeclass` wrapped class to `trace` registry.
-While `jax` uses `jax.tree_util.register_pytree_node` to define `flatten_rule` for leaves, `PyTreeClass` extends on this
-By registering the `flatten_rule` of (1) names, (2) types, (3) indexing
-
-For demonstration , the following figure contains the 4 variants of the same `Tree` instance define
-
-```python
-import jax
-import jax.numpy as jnp
-import pytreeclass as pytc
-
-class Tree(pytc.TreeClass):
-    a:int = 1
-    b:tuple[float] = (2.,3.)
-    c:jax.Array = jnp.array([4.,5.,6.])
-```
-
-![image](assets/tree_figures.png)
-
-1. Value leaves variant.
-2. Name leaves variant.
-3. Type leaves variant.
-4. Indexing leaves variant.
-
-The four variants can be accessed using `pytc.tree_map_with_trace` .
-Similar to `jax.tree_util.tree_map`, `pytc.tree_map_with_trace` accepts the map function, however the first argument must be the `trace` argument.
-Trace is a four item tuple consists of names,types,indices,metadatas path for each leaf.
-For example for the previous tree, the reuslting trace path for each leaf is :
-
-### Named tree variant
-
-```python
->>> name_tree = pytc.tree_map_with_trace(lambda trace,x : trace[0], tree)
->>> print(name_tree)
-Tree(a=(a), b=((b, [0]), (b, [1])), c=(c))
-```
-
-### Typed tree variant
-
-```python
->>> type_tree = pytc.tree_map_with_trace(lambda trace,x : f"{trace[1]!s}", tree)
->>> print(type_tree)
-Tree(
-  a=(<class 'int'>,),
-  b=((<class 'tuple'>, <class 'float'>), (<class 'tuple'>, <class 'float'>)),
-  c=(<class 'jaxlib.xla_extension.ArrayImpl'>,)
-)
-```
-
-### Index tree variant
-
-```python
->>> index_tree = pytc.tree_map_with_trace(lambda trace,x : trace[2], tree)
->>> print(index_tree)
-Tree(a=(0), b=((1, 0), (1, 1)), c=(2))
-```
-
-In essence, each leaf contains information about the name path, type path, and indices path. The rules for custom types can be registered using `pytc.register_pytree_node_trace`
-
-</details>
-
-<details>
-
-<summary> Comparison with dataclass </summary>
-
-<div align="center">
-<table>
-
-<tr><td></td>  <td>PyTreeClass</td>  <td>dataclass</td></tr>
-
-<tr><td align="center">Generated init method</td> <td align="center">✅</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Generated repr method</td> <td align="center">✅</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Generated str method</td> <td align="center">✅</td>  <td align="center"></td></tr>
-<tr><td align="center">Generated hash method</td> <td align="center">✅</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Generated eq method</td> <td align="center">✅✅*</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Support slots</td> <td align="center"></td>  <td align="center">✅</td></tr>
-<tr><td align="center">Keyword-only args</td> <td align="center">✅</td>  <td align="center">✅ 3.10+</td></tr>
-<tr><td align="center">Positional-only args</td> <td align="center">✅</td>  <td align="center"></td></tr>
-<tr><td align="center">Frozen instance</td> <td align="center">✅**</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Match args support</td> <td align="center"></td>  <td align="center">✅</td></tr>
-<tr><td align="center">Support callbacks</td> <td align="center">✅</td>  <td align="center"></td></tr>
-<tr><td align="center">Support alias name</td> <td align="center">✅</td>  <td align="center"></td></tr>
-</table>
-
-</div>
-
-`*` Either compare the whole instance and return `True/False` or treating it leafwise using `treeclass(..., leafwise=True)` and retrurn `Tree(a=True, ....)`
-
-`**` Always frozen. non-frozen is not supported.
-
-`***` `treeclass` decorator is also a bit faster than `dataclasses.dataclass` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ASEM000/PyTreeClass/blob/main/assets/pytc_dc_benchmark.ipynb)
-
-</details>
-
 ## 📙 Acknowledgements<a id="acknowledgements"></a>
 
 - [Farid Talibli (for visualization link generation backend)](https://www.linkedin.com/in/frdt98)
 - [Treex](https://github.com/cgarciae/treex), [Equinox](https://github.com/patrick-kidger/equinox), [tree-math](https://github.com/google/tree-math), [Flax](https://github.com/google/flax), [TensorFlow](https://www.tensorflow.org), [PyTorch](https://pytorch.org)
 - [Lovely JAX](https://github.com/xl0/lovely-jax)
```

### Comparing `pytreeclass-0.3.0/README.md` & `pytreeclass-0.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: pytreeclass
+Version: 0.3.1
+Summary: JAX compatible dataclass.
+Home-page: https://github.com/ASEM000/pytreeclass
+Author: Mahmoud Asem
+Author-email: asem00@kaist.ac.kr
+License: Apache-2.0
+Keywords: python machine-learning pytorch jax
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <!-- <h1 align="center" style="font-family:Monospace" >Py🌲Class</h1> -->
 <h5 align="center">
 <img width="250px" src="https://user-images.githubusercontent.com/48389287/227880173-bf78c02c-d28b-4cf4-95e6-fa49b82a43a1.svg"> <br>
 
 <br>
 
 [**Installation**](#installation)
@@ -9,15 +32,15 @@
 |[**Quick Example**](#quick_example)
 |[**StatefulComputation**](#stateful_computation)
 |[**More**](#more)
 |[**Acknowledgements**](#acknowledgements)
 
 ![Tests](https://github.com/ASEM000/pytreeclass/actions/workflows/tests.yml/badge.svg)
 ![pyver](https://img.shields.io/badge/python-3.8%203.9%203.10%203.11_-red)
-![pyver](https://img.shields.io/badge/jax-0.4+-red)
+![pyver](https://img.shields.io/badge/jax-0.4.7+-red)
 ![codestyle](https://img.shields.io/badge/codestyle-black-black)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ASEM000/PyTreeClass/blob/main/assets/intro.ipynb)
 [![Downloads](https://pepy.tech/badge/pytreeclass)](https://pepy.tech/project/pytreeclass)
 [![codecov](https://codecov.io/gh/ASEM000/pytreeclass/branch/main/graph/badge.svg?token=TZBRMO0UQH)](https://codecov.io/gh/ASEM000/pytreeclass)
 [![Documentation Status](https://readthedocs.org/projects/pytreeclass/badge/?version=latest)](https://pytreeclass.readthedocs.io/en/latest/?badge=latest)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ASEM000/pytreeclass)
 [![DOI](https://zenodo.org/badge/512717921.svg)](https://zenodo.org/badge/latestdoi/512717921)
@@ -53,47 +76,83 @@
 
 ## ⏩ Quick Example <a id="quick_example">
 
 ### 🏗️ Simple Tree example
 
 <div align="center">
 <table>
-<tr><td align="center">Code</td> <td align="center">PyTree representation</td></tr>
+<tr><td align="center"></td> <td align="center"></td></tr>
 <tr>
 <td>
 
 ```python
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
 
+
 class Tree(pytc.TreeClass):
-    a:int = 1
-    b:tuple[float] = (2.,3.)
-    c:jax.Array = jnp.array([4.,5.,6.])
+    a: int = 1
+    b: tuple = (2, 3.)
+    c: jax.Array = jnp.array([4., 5., 6.])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
 
+
 tree = Tree()
-```
+mask = jax.tree_map(lambda x: x > 5, tree)
+tree = tree \
+       .at["a"].set(10) \
+       .at["b"].at[0].set(10) \
+       .at[mask].set(100)
 
-</td>
+print(tree)
+# Tree(a=10, b=(10, 3.0), c=[  4.   5. 100.])
 
-<td>
+print(pytc.tree_diagram(tree))
+# Tree
+# ├── .a=10
+# ├── .b:tuple
+# │   ├── [0]=10
+# │   └── [1]=3.0
+# └── .c=f32[3](μ=36.33, σ=45.02, ∈[4.00,100.00])
 
-```python
-# leaves are parameters
+print(pytc.tree_summary(tree))
+# ┌─────┬──────┬─────┐
+# │Name │Type  │Count│
+# ├─────┼──────┼─────┤
+# │.a   │int   │1    │
+# ├─────┼──────┼─────┤
+# │.b[0]│int   │1    │
+# ├─────┼──────┼─────┤
+# │.b[1]│float │1    │
+# ├─────┼──────┼─────┤
+# │.c   │f32[3]│3    │
+# ├─────┼──────┼─────┤
+# │Σ    │Tree  │6    │
+# └─────┴──────┴─────┘
+
+
+# ** pass it to jax transformations **
+
+# freeze all non-differentiable parameters to make it
+# work with jax trnasformations
+mask = jax.tree_map(pytc.is_nondiff, tree)
+tree = tree.at[mask].apply(pytc.freeze)
 
-Tree
-    ├── a=1
-    ├── b:tuple
-    │   ├── [0]=2.0
-    │   └── [1]=3.0
-    └── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
+@jax.jit
+@jax.grad
+def sum_tree(tree:Tree, x):
+    # unfreeze before calling tree
+    tree = tree.at[...].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)
+    return sum(tree(x))
+
+print(sum_tree(tree, 1.0))
+# Tree(a=#10, b=(#10, 0.0), c=[1. 1. 1.])
 ```
 
 </td>
 
 </tr>
 </table>
 </div>
@@ -117,52 +176,52 @@
 <td>
 
 ```python
 print(pytc.tree_summary(tree, depth=1))
 ┌────┬──────┬─────┐
 │Name│Type  │Count│
 ├────┼──────┼─────┤
-│a   │int   │1    │
+│.a  │int   │1    │
 ├────┼──────┼─────┤
-│b   │tuple │1    │
+│.b  │tuple │1    │
 ├────┼──────┼─────┤
-│c   │f32[3]│3    │
+│.c  │f32[3]│3    │
 ├────┼──────┼─────┤
 │Σ   │Tree  │5    │
 └────┴──────┴─────┘
 ```
 
 </td>
 
 <td>
 
 ```python
 
 print(pytc.tree_diagram(tree, depth=1))
 Tree
-├── a=1
-├── b=(...)
-└── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
+├── .a=1
+├── .b=(...)
+└── .c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
 ```
 
  </td>
 
 <td>
 
 ```python
 print(pytc.tree_mermaid(tree, depth=1))
 ```
 
 ```mermaid
 
 flowchart LR
     id0(<b>Tree</b>)
-    id0 --- id1("</b>a=1</b>")
-    id0 --- id2("</b>b=(...)</b>")
-    id0 --- id3("</b>c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])</b>")
+    id0 --- id1("</b>.a=1</b>")
+    id0 --- id2("</b>.b=(...)</b>")
+    id0 --- id3("</b>.c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])</b>")
 ```
 
 </td>
 
 <td>
 
 ```python
@@ -185,41 +244,41 @@
 
 <tr>
 
 <td>
 
 ```python
 print(pytc.tree_summary(tree, depth=2))
-┌────┬──────┬─────┐
-│Name│Type  │Count│
-├────┼──────┼─────┤
-│a   │int   │1    │
-├────┼──────┼─────┤
-│b[0]│float │1    │
-├────┼──────┼─────┤
-│b[1]│float │1    │
-├────┼──────┼─────┤
-│c   │f32[3]│3    │
-├────┼──────┼─────┤
-│Σ   │Tree  │6    │
-└────┴──────┴─────┘
+┌─────┬──────┬─────┐
+│Name │Type  │Count│
+├─────┼──────┼─────┤
+│.a   │int   │1    │
+├─────┼──────┼─────┤
+│.b[0]│int   │1    │
+├─────┼──────┼─────┤
+│.b[1]│float │1    │
+├─────┼──────┼─────┤
+│.c   │f32[3]│3    │
+├─────┼──────┼─────┤
+│Σ    │Tree  │6    │
+└─────┴──────┴─────┘
 ```
 
 </td>
 
 <td>
 
 ```python
 print(pytc.tree_diagram(tree, depth=2))
 Tree
-├── a=1
-├── b:tuple
+├── .a=1
+├── .b:tuple
 │   ├── [0]=2.0
 │   └── [1]=3.0
-└── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
+└── .c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
 ```
 
 </td>
 
 <td>
 
 ```python
@@ -227,17 +286,17 @@
 ```
 
 ```mermaid
 flowchart LR
     id2 --- id3("</b>[0]=2.0</b>")
     id2 --- id4("</b>[1]=3.0</b>")
     id0(<b>Tree</b>)
-    id0 --- id1("</b>a=1</b>")
-    id0 --- id2("</b>b:tuple</b>")
-    id0 --- id5("</b>c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])</b>")
+    id0 --- id1("</b>.a=1</b>")
+    id0 --- id2("</b>.b:tuple</b>")
+    id0 --- id5("</b>.c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])</b>")
 ```
 
 </td>
 
 <td>
 
 ```python
@@ -391,14 +450,57 @@
 print(tree.at[1].at[0].set(10))
 # Tree(a=1, b=(10, 3.0), c=[4. 5. 6.])
 
 print(tree.at[1].at[0].apply(lambda x: 10))
 # Tree(a=1, b=(10, 3.0), c=[4. 5. 6.])
 ```
 
+### Mix, match , and chain index update
+
+```python
+
+import jax
+import jax.numpy as jnp
+import pytreeclass as pytc
+
+class Tree(pytc.TreeClass):
+    a: int = 1
+    b: str = "b"
+    c: float = 1.0
+    d: bool = True
+    e: tuple = (1, 2, 3)
+    f: jax.Array = jax.numpy.array([1, 2, 3])
+
+tree = Tree()
+
+integer_mask = jax.tree_util.tree_map(lambda x: isinstance(x, int), tree)
+
+tree = (
+    tree
+    .at["a"].set(10)
+    .at["b"].set("B")
+    .at["c"].set(10.0)
+    .at["d"].set(False)
+    .at["e"].at[0].set(10)  # set first element of tuple to 10
+    .at["f"].apply(jnp.sin)  # apply to all elements in array
+    .at[integer_mask].apply(float)  # cast all `int` to `float`
+)
+
+print(tree)
+# Tree(
+#   a=10.0,
+#   b=B,
+#   c=10.0,
+#   d=0.0,
+#   e=(10.0, 2.0, 3.0),
+#   f=[0.841471  0.9092974 0.14112  ]
+# )
+
+```
+
 </details>
 
 <details>
 
 <summary>
 
 ## 📜 Stateful computations<a id="stateful_computation"></a> </summary>
@@ -433,83 +535,14 @@
 print(counter.calls) # 10
 ```
 
 </details>
 
 ## ➕ More<a id="more"></a>
 
-<details><summary>[Advanced] Register custom user-defined classes to work with visualization and indexing tools. </summary>
-
-Similar to [`jax.tree_util.register_pytree_node`](https://jax.readthedocs.io/en/latest/pytrees.html#extending-pytrees), `PyTreeClass` register common data structures and `treeclass` wrapped classes to figure out how to define the names, types, and index of certain leaf along its path.
-
-Here is an example of registering
-
-```python
-
-class Tree:
-    def __init__(self, a, b):
-        self.a = a
-        self.b = b
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(a={self.a}, b={self.b})"
-
-
-# jax flatten rule
-def tree_flatten(tree):
-    return (tree.a, tree.b), None
-
-# jax unflatten rule
-def tree_unflatten(_, children):
-    return Tree(*children)
-
-# PyTreeClass flatten rule
-def pytc_tree_flatten(tree):
-    names = ("a", "b") # or (`None`, `None`) if name is not defined
-    types = (type(tree.a), type(tree.b))
-    indices = (0,1)  # or (`None`, `None`) if index is not defined
-    return [*zip(names, types, indices)]
-
-
-# Register with `jax`
-jax.tree_util.register_pytree_node(Tree, tree_flatten, tree_unflatten)
-
-# Register the `Tree` class trace function to support indexing
-pytc.register_pytree_node_trace(Tree, pytc_tree_flatten)
-
-tree = Tree(1, 2)
-
-# works with jax
-jax.tree_util.tree_leaves(tree)  # [1, 2]
-
-# works with PyTreeClass viz tools
-print(pytc.tree_summary(tree))
-
-# ┌────┬────┬─────┬──────┐
-# │Name│Type│Count│Size  │
-# ├────┼────┼─────┼──────┤
-# │a   │int │1    │28.00B│
-# ├────┼────┼─────┼──────┤
-# │b   │int │1    │28.00B│
-# ├────┼────┼─────┼──────┤
-# │Σ   │Tree│2    │56.00B│
-# └────┴────┴─────┴──────┘
-
-```
-
-After registeration, you can use internal tools like
-
-- `pytc.tree_map_with_trace`
-- `pytc.tree_leaves_with_trace`
-- `pytc.tree_flatten_with_trace`
-
-More details on that soon.
-
-</details>
-
 <details> <summary>Validate or convert inputs using callbacks</summary>
 
 `PyTreeClass` includes `callbacks` in the `field` to apply a sequence of functions on input at setting the attribute stage. The callback is quite useful in several cases, for instance, to ensure a certain input type within a valid range. See example:
 
 ```python
 import jax
 import pytreeclass as pytc
@@ -783,70 +816,70 @@
 ```
 
 </details>
 
 <details><summary>Use PyTreeClass components with other libraries</summary>
 
 ```python
+
 import jax
 import pytreeclass as pytc
 from flax import struct
 
+import jax
+import pytreeclass as pytc
+from flax import struct
+
+# note that flax is registered with `jax.tree_util.register_pytree_with_keys`
+# otherwise for arbitrary objects you need to do the key registration
+
 @struct.dataclass
 class FlaxTree:
     a:int = 1
     b:tuple[float] = (2.,3.)
     c:jax.Array = jax.numpy.array([4.,5.,6.])
 
     def __repr__(self) -> str:
         return pytc.tree_repr(self)
     def __str__(self) -> str:
         return pytc.tree_str(self)
     @property
     def at(self):
         return pytc.tree_indexer(self)
 
-def pytc_flatten_rule(tree):
-    names =("a","b","c")
-    types = map(type, (tree.a, tree.b, tree.c))
-    indices = range(3)  # make it indexable like namedtuple
-    return [*zip(names, types, indices)]
-
-pytc.register_pytree_node_trace(FlaxTree, pytc_flatten_rule)
-
 flax_tree = FlaxTree()
 
 print(f"{flax_tree!r}")
 # FlaxTree(a=1, b=(2.0, 3.0), c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00]))
 
 print(f"{flax_tree!s}")
 # FlaxTree(a=1, b=(2.0, 3.0), c=[4. 5. 6.])
 
 print(pytc.tree_diagram(flax_tree))
 # FlaxTree
-# ├── a=1
-# ├── b:tuple
+# ├── .a=1
+# ├── .b:tuple
 # │   ├── [0]=2.0
 # │   └── [1]=3.0
-# └── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
+# └── .c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
 
 print(pytc.tree_summary(flax_tree))
-# ┌────┬────────┬─────┐
-# │Name│Type    │Count│
-# ├────┼────────┼─────┤
-# │a   │int     │1    │
-# ├────┼────────┼─────┤
-# │b[0]│float   │1    │
-# ├────┼────────┼─────┤
-# │b[1]│float   │1    │
-# ├────┼────────┼─────┤
-# │c   │f32[3]  │3    │
-# ├────┼────────┼─────┤
-# │Σ   │FlaxTree│6    │
-# └────┴────────┴─────┘
+# ┌─────┬────────┬─────┐
+# │Name │Type    │Count│
+# ├─────┼────────┼─────┤
+# │.a   │int     │1    │
+# ├─────┼────────┼─────┤
+# │.b[0]│float   │1    │
+# ├─────┼────────┼─────┤
+# │.b[1]│float   │1    │
+# ├─────┼────────┼─────┤
+# │.c   │f32[3]  │3    │
+# ├─────┼────────┼─────┤
+# │Σ    │FlaxTree│6    │
+# └─────┴────────┴─────┘
 
 flax_tree.at[0].get()
 # FlaxTree(a=1, b=(None, None), c=None)
 
 flax_tree.at["a"].set(10)
 # FlaxTree(a=10, b=(2.0, 3.0), c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00]))
 ```
@@ -861,117 +894,19 @@
 <table>
 
 <tr><td align="center">CPU</td><td align="center">GPU</td></tr>
 
 <tr>
 
 <td><img src='assets/benchmark_cpu.png'></td>
-<td><img src='assets/benchmark_gpu.png'></td>
 
 </tr>
 
 </table>
 
 </details>
 
-<details> 
-<summary>Use tree_map_with_trace</summary>
-
-V0.2 of `PyTreeClass` register common python datatypes and `treeclass` wrapped class to `trace` registry.
-While `jax` uses `jax.tree_util.register_pytree_node` to define `flatten_rule` for leaves, `PyTreeClass` extends on this
-By registering the `flatten_rule` of (1) names, (2) types, (3) indexing
-
-For demonstration , the following figure contains the 4 variants of the same `Tree` instance define
-
-```python
-import jax
-import jax.numpy as jnp
-import pytreeclass as pytc
-
-class Tree(pytc.TreeClass):
-    a:int = 1
-    b:tuple[float] = (2.,3.)
-    c:jax.Array = jnp.array([4.,5.,6.])
-```
-
-![image](assets/tree_figures.png)
-
-1. Value leaves variant.
-2. Name leaves variant.
-3. Type leaves variant.
-4. Indexing leaves variant.
-
-The four variants can be accessed using `pytc.tree_map_with_trace` .
-Similar to `jax.tree_util.tree_map`, `pytc.tree_map_with_trace` accepts the map function, however the first argument must be the `trace` argument.
-Trace is a four item tuple consists of names,types,indices,metadatas path for each leaf.
-For example for the previous tree, the reuslting trace path for each leaf is :
-
-### Named tree variant
-
-```python
->>> name_tree = pytc.tree_map_with_trace(lambda trace,x : trace[0], tree)
->>> print(name_tree)
-Tree(a=(a), b=((b, [0]), (b, [1])), c=(c))
-```
-
-### Typed tree variant
-
-```python
->>> type_tree = pytc.tree_map_with_trace(lambda trace,x : f"{trace[1]!s}", tree)
->>> print(type_tree)
-Tree(
-  a=(<class 'int'>,),
-  b=((<class 'tuple'>, <class 'float'>), (<class 'tuple'>, <class 'float'>)),
-  c=(<class 'jaxlib.xla_extension.ArrayImpl'>,)
-)
-```
-
-### Index tree variant
-
-```python
->>> index_tree = pytc.tree_map_with_trace(lambda trace,x : trace[2], tree)
->>> print(index_tree)
-Tree(a=(0), b=((1, 0), (1, 1)), c=(2))
-```
-
-In essence, each leaf contains information about the name path, type path, and indices path. The rules for custom types can be registered using `pytc.register_pytree_node_trace`
-
-</details>
-
-<details>
-
-<summary> Comparison with dataclass </summary>
-
-<div align="center">
-<table>
-
-<tr><td></td>  <td>PyTreeClass</td>  <td>dataclass</td></tr>
-
-<tr><td align="center">Generated init method</td> <td align="center">✅</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Generated repr method</td> <td align="center">✅</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Generated str method</td> <td align="center">✅</td>  <td align="center"></td></tr>
-<tr><td align="center">Generated hash method</td> <td align="center">✅</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Generated eq method</td> <td align="center">✅✅*</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Support slots</td> <td align="center"></td>  <td align="center">✅</td></tr>
-<tr><td align="center">Keyword-only args</td> <td align="center">✅</td>  <td align="center">✅ 3.10+</td></tr>
-<tr><td align="center">Positional-only args</td> <td align="center">✅</td>  <td align="center"></td></tr>
-<tr><td align="center">Frozen instance</td> <td align="center">✅**</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Match args support</td> <td align="center"></td>  <td align="center">✅</td></tr>
-<tr><td align="center">Support callbacks</td> <td align="center">✅</td>  <td align="center"></td></tr>
-<tr><td align="center">Support alias name</td> <td align="center">✅</td>  <td align="center"></td></tr>
-</table>
-
-</div>
-
-`*` Either compare the whole instance and return `True/False` or treating it leafwise using `treeclass(..., leafwise=True)` and retrurn `Tree(a=True, ....)`
-
-`**` Always frozen. non-frozen is not supported.
-
-`***` `treeclass` decorator is also a bit faster than `dataclasses.dataclass` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ASEM000/PyTreeClass/blob/main/assets/pytc_dc_benchmark.ipynb)
-
-</details>
-
 ## 📙 Acknowledgements<a id="acknowledgements"></a>
 
 - [Farid Talibli (for visualization link generation backend)](https://www.linkedin.com/in/frdt98)
 - [Treex](https://github.com/cgarciae/treex), [Equinox](https://github.com/patrick-kidger/equinox), [tree-math](https://github.com/google/tree-math), [Flax](https://github.com/google/flax), [TensorFlow](https://www.tensorflow.org), [PyTorch](https://pytorch.org)
 - [Lovely JAX](https://github.com/xl0/lovely-jax)
```

### Comparing `pytreeclass-0.3.0/docs/conf.py` & `pytreeclass-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.0/pytreeclass/__init__.py` & `pytreeclass-0.3.1/pytreeclass/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     tree_mermaid,
     tree_repr,
     tree_repr_with_trace,
     tree_str,
     tree_summary,
 )
 from pytreeclass._src.tree_trace import (
-    register_pytree_node_trace,
     tree_flatten_with_trace,
     tree_leaves_with_trace,
     tree_map_with_trace,
 )
 
 __all__ = (
     # general utils
@@ -34,15 +33,14 @@
     "is_nondiff",
     "is_frozen",
     "freeze",
     "unfreeze",
     # masking and indexing utils
     "bcmap",
     "tree_indexer",
-    "register_pytree_node_trace",
     "tree_map_with_trace",
     "tree_leaves_with_trace",
     "tree_flatten_with_trace",
     "tree_repr_with_trace",
 )
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
```

### Comparing `pytreeclass-0.3.0/pytreeclass/_src/tree_decorator.py` & `pytreeclass-0.3.1/pytreeclass/_src/tree_decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from __future__ import annotations
 
 import functools as ft
 import sys
 from abc import ABCMeta
 from collections.abc import MutableMapping, MutableSequence
 from types import FunctionType, MappingProxyType
-from typing import Any, Callable, NamedTuple, Sequence, TypeVar
+from typing import Any, Callable, Hashable, NamedTuple, Sequence, TypeVar
 
-from jax.tree_util import register_pytree_node
+import jax.tree_util as jtu
 from typing_extensions import dataclass_transform
 
 from pytreeclass._src.tree_freeze import tree_hash
 from pytreeclass._src.tree_indexer import (
     _leafwise_transform,
     _mutable_context,
     _mutable_instance_registry,
     is_tree_equal,
     tree_copy,
     tree_indexer,
 )
 from pytreeclass._src.tree_pprint import tree_repr, tree_str
-from pytreeclass._src.tree_trace import register_pytree_node_trace
+from pytreeclass._src.tree_trace import NamedSequenceKey
 
 
 class NOT_SET:
     __repr__ = lambda _: "?"
 
 
-T = TypeVar("T")
+T = TypeVar("T", bound=Hashable)
 PyTree = Any
 
 _NOT_SET = NOT_SET()
 _FIELDS = "_fields"
 _POST_INIT = "__post_init__"
 _MUTABLE_TYPES = (MutableSequence, MutableMapping, set)
 
@@ -107,49 +107,49 @@
         >>> class Employee(pytc.TreeClass):
         ...    # assert employee `name` is str
         ...    name: str = pytc.field(callbacks=[instance_cb_factory(str)])
         ...    # use callback compostion to assert employee `age` is int and positive
         ...    age: int = pytc.field(callbacks=[instance_cb_factory(int), positive_check_callback])
         ...    # use `id` in the constructor for `_id` attribute
         ...    # this is useful for private attributes that are not supposed to be accessed directly
-        ...    # and hide it from the repr, also add extra info for this field
+        ...    # and hide it from the repr
         ...    _id: int = pytc.field(alias="id", repr=False)
 
         >>> tree = Employee(name="Asem", age=10, id=1)
         >>> print(tree)  # _id is not shown
         Employee(name=Asem, age=10)
         >>> assert tree._id == 1  # this is the private attribute
     """
     if not isinstance(alias, (str, type(None))):
         msg = "`alias` must be a string or None, "
         msg += f"got type=`{type(alias).__name__}` instead."
         raise TypeError(msg)
 
     if default is not _NOT_SET and factory is not None:
         msg = "`default` and `factory` are mutually exclusive arguments."
-        msg += f"got default={default} and factory={factory}"
+        msg += f"got {default=} and {factory=}"
         raise ValueError(msg)
 
     if kw_only is True and pos_only is True:
         msg = "`kw_only` and `pos_only` are mutually exclusive arguments."
-        msg += f"got kw_only={kw_only} and pos_only={pos_only}"
+        msg += f"got {kw_only=} and {pos_only=}"
         raise ValueError(msg)
 
     if isinstance(metadata, dict):
         metadata = MappingProxyType(metadata)  # type: ignore
     elif metadata is not None:
         raise TypeError("`metadata` must be a Mapping or None")
 
     if not isinstance(callbacks, Sequence):
         msg = f"`callbacks` must be a Sequence of functions, got {type(callbacks)}"
         raise TypeError(msg)
 
     for index, callback in enumerate(callbacks):
         if not isinstance(callback, Callable):  # type: ignore
-            msg = "`callbacks` must be a Sequence of functions, "
+            msg = "`callbacks` must be a Sequence of zero argument functions, "
             msg += f"got `{type(callbacks).__name__}` at index={index}"
             raise TypeError(msg)
 
     return Field(
         name=None,
         type=None,
         default=default,
@@ -161,26 +161,26 @@
         metadata=metadata,  # type: ignore
         callbacks=callbacks,
         alias=alias,
     )
 
 
 @ft.lru_cache
-def _generate_field_map(klass: type) -> dict[str, Field]:
-    field_map = dict()
+def _generate_field_map(klass: type) -> MappingProxyType[str, Field]:
+    field_map = dict()  # type: dict[str, Field]
 
     if klass is object:
-        return field_map
+        return MappingProxyType(field_map)
 
     for base in reversed(klass.__mro__[1:]):
         field_map.update(_generate_field_map(base))
 
     # TODO: use inspect to get annotations, once we are on minimum python version >3.9
     if "__annotations__" not in vars(klass):
-        return field_map
+        return MappingProxyType(field_map)
 
     for name in (annotation_map := vars(klass)["__annotations__"]):
         value = vars(klass).get(name, _NOT_SET)
         type = annotation_map[name]
 
         if name == "self":
             # while `dataclasses` allows `self` as a field name, its confusing
@@ -209,15 +209,15 @@
             # case: `x: Any`
             field_map[name] = Field(name=name, type=type)
 
         else:
             # case: `x: int = 1`
             field_map[name] = Field(name=name, type=type, default=value)
 
-    return field_map
+    return MappingProxyType(field_map)
 
 
 @ft.lru_cache
 def _generate_init_code(fields: Sequence[Field]) -> str:
     head = body = ""
 
     for field in fields:
@@ -247,15 +247,15 @@
     body = f"def closure(field_map):\n{body}\n\treturn __init__"
     return body.expandtabs(4)
 
 
 def _generate_init_method(klass: type) -> FunctionType:
     field_map = _generate_field_map(klass)
     init_code = _generate_init_code(tuple(field_map.values()))
-    exec(init_code, vars(sys.modules[klass.__module__]), local_namespace := dict())
+    exec(init_code, vars(sys.modules[klass.__module__]), local_namespace := dict())  # type: ignore
     method = local_namespace["closure"](field_map)
     method.__qualname__ = f"{klass.__qualname__}.__init__"
     return method
 
 
 def _setattr(tree: PyTree, key: str, value: Any) -> None:
     if id(tree) not in _mutable_instance_registry:
@@ -275,16 +275,16 @@
 
     elif isinstance(value, TreeClass):
         # auto registers the instance value if it is a registered `treeclass`
         # this behavior is similar to PyTorch behavior in `nn.Module`
         # with instances of `Parameter`/`Module`.
         # the behavior is useful to avoid repetitive code pattern in field definition and
         # and initialization inside init method.
-        kv = {key: Field(type=type(value), init=False, name=key)}
-        vars(tree)[_FIELDS] = MappingProxyType({**field_map, **kv})
+        field = Field(type=type(value), init=False, name=key)
+        vars(tree)[_FIELDS] = MappingProxyType({**field_map, key: field})  # type: ignore
 
     vars(tree)[key] = value  # type: ignore
 
 
 def _delattr(tree, key: str) -> None:
     # delete the attribute under `_mutable_context` context
     # otherwise raise an error
@@ -292,39 +292,14 @@
         msg = f"Cannot delete attribute `{key}` on immutable instance of "
         msg += f"`{type(tree).__name__}`.\n"
         raise AttributeError(msg)
 
     del vars(tree)[key]
 
 
-def _tree_unflatten(klass: type, treedef: Any, leaves: list[Any]):
-    # unflatten rule for `treeclass` to use with `jax.tree_unflatten`
-    tree = object.__new__(klass)
-    vars(tree).update(treedef[1])
-    vars(tree).update(zip(treedef[0], leaves))
-    return tree
-
-
-def _tree_flatten(tree: PyTree):
-    # flatten rule for `treeclass` to use with `jax.tree_flatten`
-    static, dynamic = dict(vars(tree)), dict()
-    for key in static.get(_FIELDS, ()):
-        dynamic[key] = static.pop(key)
-    return list(dynamic.values()), (tuple(dynamic.keys()), static)
-
-
-def _tree_trace(tree: PyTree) -> list[tuple[Any, Any, Any, Any]]:
-    # Trace flatten rule to be used with the `tree_trace` module
-    leaves, (keys, _) = _tree_flatten(tree)
-    names = (f"{key}" for key in keys)
-    types = map(type, leaves)
-    indices = range(len(leaves))
-    return [*zip(names, types, indices)]
-
-
 def _treeclass_transform(klass: type[T]) -> type[T]:
     for key, method in (("__setattr__", _setattr), ("__delattr__", _delattr)):
         if key in vars(klass):
             # the user defined a method that conflicts with the reserved method
             msg = f"Unable to transform the class `{klass.__name__}` "
             msg += f"with resereved `{key}` method defined on the class."
             raise TypeError(msg)
@@ -348,49 +323,70 @@
             setattr(klass, key, method)
 
     return klass
 
 
 def _register_treeclass(klass: type[T]) -> type[T]:
     # handle all registration logic for `treeclass`
-    # TODO: register with jax path registry once jax version >= 0.4.7
-    register_pytree_node_trace(klass, _tree_trace)
-    register_pytree_node(klass, _tree_flatten, ft.partial(_tree_unflatten, klass))
+
+    def tree_unflatten(treedef: Any, leaves: list[Any]) -> T:
+        # unflatten rule for `treeclass` to use with `jax.tree_unflatten`
+        tree = getattr(object, "__new__")(klass)
+        vars(tree).update(treedef[1])
+        vars(tree).update(zip(treedef[0], leaves))
+        return tree
+
+    def tree_flatten(tree: T):
+        # flatten rule for `treeclass` to use with `jax.tree_flatten`
+        static, dynamic = dict(vars(tree)), dict()
+        for key in static.get(_FIELDS, ()):
+            dynamic[key] = static.pop(key)
+        return list(dynamic.values()), (tuple(dynamic.keys()), static)
+
+    def tree_flatten_with_keys(tree: PyTree):
+        # flatten rule for `treeclass` to use with `jax.tree_util.tree_flatten_with_path`
+        static, dynamic = dict(vars(tree)), dict()
+        for key in static.get(_FIELDS, ()):
+            entry = NamedSequenceKey(len(dynamic), key)
+            dynamic[key] = (entry, static.pop(key))
+        return list(dynamic.values()), (tuple(dynamic.keys()), static)
+
+    jtu.register_pytree_with_keys(
+        nodetype=klass,
+        flatten_func=tree_flatten,
+        flatten_with_keys=tree_flatten_with_keys,
+        unflatten_func=tree_unflatten,
+    )
     return klass
 
 
 class TreeClassMeta(ABCMeta):
     def __call__(klass: type[T], *a, **k) -> T:
-        self = klass.__new__(klass, *a, **k)
+        self = getattr(klass, "__new__")(klass, *a, **k)
 
         with _mutable_context(self):
-            vars(self)[_FIELDS] = MappingProxyType(_generate_field_map(klass))
-            klass.__init__(self, *a, **k)
+            setattr(self, _FIELDS, _generate_field_map(klass))
+            getattr(klass, "__init__")(self, *a, **k)
 
             if post_init_func := getattr(klass, _POST_INIT, None):
                 # to simplify the logic, we call the post init method
                 # even if the init method is not code-generated.
                 post_init_func(self)
 
         # handle non-initialized fields
         if len(keys := set(getattr(self, _FIELDS)) - set(vars(self))) > 0:
-            msg = f"Uninitialized fields: ({', '.join(keys)}) "
-            msg += f"in class `{type(self).__name__}`"
+            msg = f"Uninitialized fields: ({', '.join(keys)}) in the instance of `{type(self).__name__}`"
             raise AttributeError(msg)
         return self
 
 
 @dataclass_transform(field_specifiers=(field, Field), frozen_default=True)
 class TreeClass(metaclass=TreeClassMeta):
     """Convert a class to a JAX compatible tree structure.
 
-    Args:
-        klass: class to be converted to a `treeclass`
-        leafwise: Wether to generate leafwise math operations methods. Defaults to `False`.
-
     Example:
         >>> import functools as ft
         >>> import jax
         >>> import pytreeclass as pytc
 
         >>> # Tree leaves are defined by type hinted fields at the class level
         >>> class Tree(pytc.TreeClass):
@@ -409,38 +405,53 @@
         Tree(a=2, b=3.0)
 
         >>> # Advanced indexing is supported using `at` property
         ... class Tree(pytc.TreeClass):
         ...     a:int = 1
         ...     b:float = 2.0
         >>> tree = Tree()
-        >>> tree.at[0].get()
-        Tree(a=1, b=None)
         >>> tree.at["a"].get()
         Tree(a=1, b=None)
+        >>> tree.at[0].get()
+        Tree(a=1, b=None)
 
     Note:
-        Indexing is supported for {`list`, `tuple`, `dict`, `defaultdict`, `OrderedDict`, `namedtuple`}
-        and `treeclass` wrapped classes.
-
-        Extending indexing to other types is possible by registering the type with
-        `pytreeclass.register_pytree_node_trace`
+        ``leafwise=True`` adds the following methods to the class
 
-    Note:
-        `leafwise`=True adds the following methods to the class:
-        .. code-block:: python
-            '__add__', '__and__', '__ceil__', '__divmod__', '__eq__', '__floor__', '__floordiv__',
-            '__ge__', '__gt__', '__invert__', '__le__', '__lshift__', '__lt__',
-            '__matmul__', '__mod__', '__mul__', '__ne__', '__neg__', '__or__', '__pos__',
-            '__pow__', '__radd__', '__rand__', '__rdivmod__', '__reduce__', '__rfloordiv__',
-            '__rlshift__', '__rmatmul__', '__rmod__', '__rmul__', '__ror__', '__round__', '__rpow__',
-            '__rrshift__', '__rshift__', '__rsub__', '__rtruediv__', '__rxor__', '__sub__',
-            '__truediv__', '__trunc__', '__xor__',
+        ==================      ============
+        Method                  Operator
+        ==================      ============
+        ``__add__``              `+`
+        ``__and__``              `&`
+        ``__ceil__``             `math.ceil`
+        ``__divmod__``           `divmod`
+        ``__eq__``               `==`
+        ``__floor__``            math.floor
+        ``__floordiv__``         `//`
+        ``__ge__``               `>=`
+        ``__gt__``               `>`
+        ``__invert__``           `~`
+        ``__le__``               `<=`
+        ``__lshift__``           `<<`
+        ``__lt__``               `<`
+        ``__matmul__``           `@`
+        ``__mod__``              `%`
+        ``__mul__``              `*`
+        ``__ne__``               `!=`
+        ``__neg__``              `-`
+        ``__or__``               `|`
+        ``__pos__``              `+`
+        ``__pow__``              `**`
+        ``__round__``            `round`
+        ``__sub__``              `-`
+        ``__truediv__``          `/`
+        ``__trunc__``            `math.trunc`
+        ``__xor__``              `^`
+        ==================      ============
 
-    Raises:
-        TypeError: if the input is not a class.
     """
 
-    def __init_subclass__(klass: type[T], leafwise: bool = False) -> None:
+    def __init_subclass__(klass: type[T], *a, leafwise: bool = False, **k) -> None:
+        super().__init_subclass__(*a, **k)
         klass = _register_treeclass(klass)
         klass = _leafwise_transform(klass) if leafwise else klass
         klass = _treeclass_transform(klass)
```

### Comparing `pytreeclass-0.3.0/pytreeclass/_src/tree_freeze.py` & `pytreeclass-0.3.1/pytreeclass/_src/tree_freeze.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.0/pytreeclass/_src/tree_indexer.py` & `pytreeclass-0.3.1/pytreeclass/_src/tree_indexer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,91 +1,94 @@
-# this script defines methods used in indexing using `at` property
-# and decorator using to enable masking and math operations
-
 from __future__ import annotations
 
-import copy
 import functools as ft
 import operator as op
 from collections.abc import Callable
 from contextlib import contextmanager
 from math import ceil, floor, trunc
-from typing import Any, NamedTuple, Sequence, TypeVar
+from typing import Any, NamedTuple, TypeVar
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
 
-from pytreeclass._src.tree_trace import tree_map_with_trace
+from pytreeclass._src.tree_pprint import tree_repr_with_trace
+from pytreeclass._src.tree_trace import NamedSequenceKey, TraceType, tree_map_with_trace
 
 T = TypeVar("T")
-PyTree = TypeVar("PyTree")
+PyTree = Any
 EllipsisType = type(Ellipsis)
-TraceType = Any
-
 _no_initializer = object()
 _non_partial = object()
 
+
 # allow methods in mutable context to be called without raising `AttributeError`
 # the instances are registered  during initialization and using `at` property with `__call__
 # this is done by registering the instance id in a set before entering the
 # mutable context and removing it after exiting the context
 _mutable_instance_registry: set[int] = set()
 
 
+def _unpack_entry(entry) -> tuple[Any, ...]:
+    # define rule for indexing matching through `at` property
+    # for example `jax` internals uses `jtu.GetAttrKey` to index an attribute, however
+    # its not ergonomic to use `tree.at[jtu.GetAttrKey("attr")]` to index an attribute
+    # instead `tree.at['attr']` is more ergonomic
+    if isinstance(entry, jtu.GetAttrKey):
+        return (entry.name,)
+    if isinstance(entry, jtu.SequenceKey):
+        return (entry.idx,)
+    if isinstance(entry, (jtu.DictKey, jtu.FlattenedIndexKey)):
+        return (entry.key,)
+    if isinstance(entry, NamedSequenceKey):
+        return (entry.idx, entry.key)
+    return (entry,)
+
+
+def tree_copy(tree: T) -> T:
+    """Return a copy of the tree."""
+    leaves, treedef = jtu.tree_flatten(tree)
+    return jtu.tree_unflatten(treedef, leaves)
+
+
 @contextmanager
 def _mutable_context(tree: PyTree, *, kopy: bool = False):
-    tree = copy.copy(tree) if kopy else tree
+    tree = tree_copy(tree) if kopy else tree
     _mutable_instance_registry.add(id(tree))
     yield tree
     _mutable_instance_registry.discard(id(tree))
 
 
 # tree indexing by boolean PyTree
 
 
 def _get_at_mask(
     tree: PyTree, where: PyTree, is_leaf: Callable[[Any], bool] | None
 ) -> PyTree:
     def leaf_get(leaf: Any, where: Any):
-        # check if where is a boolean leaf inside the `tree_map`
-        # to avoid extrachecks in `tree_map`
-        if isinstance(leaf, (jax.Array, np.ndarray)) and jnp.ndim(leaf) > 0:
-            # return empty array instead of None if condition is not met
-            # not `jittable` as size of array changes
+        if isinstance(where, (jax.Array, np.ndarray)) and where.ndim != 0:
             return leaf[jnp.where(where)]
         return leaf if where else None
 
     return jtu.tree_map(leaf_get, tree, where, is_leaf=is_leaf)
 
 
 def _set_at_mask(
     tree: PyTree,
     where: PyTree,
     set_value: Any,
     is_leaf: Callable[[Any], bool] | None,
 ) -> PyTree:
     def leaf_set(leaf: Any, where: Any, set_value: Any):
-        # check if where is a boolean leaf inside the `tree_map`
-        # to avoid extrachecks in `tree_map`
-        if isinstance(leaf, (jax.Array, np.ndarray)):
-            if jnp.isscalar(set_value):
-                # apply scalar set_value to leaf array if condition is met
-                return jnp.where(where, set_value, leaf)
-            # set_value is not scalar
-            return set_value if jnp.all(where) else leaf
-        # leaf is not an array and set_value, so we apply the set_value to the
-        # leaf if the condition is met
-        return set_value if (where is True) else leaf
-
-    if isinstance(set_value, type(tree)) and (
-        jtu.tree_structure(tree, is_leaf=is_leaf)
-        == jtu.tree_structure(set_value, is_leaf=is_leaf)
-    ):
+        if isinstance(where, (jax.Array, np.ndarray)):
+            return jnp.where(where, set_value, leaf)
+        return set_value if where else leaf
+
+    if jtu.tree_structure(tree) == jtu.tree_structure(set_value):
         # do not broadcast set_value if it is a pytree of same structure
         # for example tree.at[where].set(tree2) will set all tree leaves to tree2 leaves
         # if tree2 is a pytree of same structure as tree
         # instead of making each leaf of tree a copy of tree2
         # is design is similar to `numpy` design `Array.at[...].set(Array)`
         return jtu.tree_map(leaf_set, tree, where, set_value, is_leaf=is_leaf)
 
@@ -98,88 +101,96 @@
 def _apply_at_mask(
     tree: PyTree,
     where: PyTree,
     func: Callable[[Any], Any],
     is_leaf: Callable[[Any], bool] | None,
 ) -> PyTree:
     def leaf_apply(leaf: Any, where: bool):
-        # check if where is a boolean leaf inside the `tree_map`
-        # to avoid extrachecks in `tree_map`
-        value = func(leaf)
-        if isinstance(leaf, (jax.Array, np.ndarray)):
-            try:
-                # leaf is an array with scalar output
-                return jnp.where(where, value, leaf)
-            except TypeError:
-                # set_value is not `scalar` type
-                return value if jnp.all(where) else leaf
-        # leaf is not an array and value is not scalar
-        return value if (where is True) else leaf
+        if isinstance(where, (jax.Array, np.ndarray)):
+            return jnp.where(where, func(leaf), leaf)
+        return func(leaf) if where else leaf
 
     return jtu.tree_map(leaf_apply, tree, where, is_leaf=is_leaf)
 
 
 def _reduce_at_mask(
     tree: PyTree,
     where: PyTree,
     func: Callable[[Any, Any], Any],
     initializer: Any = _no_initializer,
     is_leaf: Callable[[Any], bool] | None = None,
 ) -> Any:
-    tree = tree.at[where].get(is_leaf=is_leaf)
+    tree = tree.at[where].get(is_leaf=is_leaf)  # type: ignore
     if initializer is _no_initializer:
         return jtu.tree_reduce(func, tree)
     return jtu.tree_reduce(func, tree, initializer)
 
 
-def _merge_where(
+def _generate_path_mask(
     tree: PyTree,
-    where: tuple[int | str | PyTree | EllipsisType, ...],
+    where: tuple[int | str, ...],
     is_leaf: Callable[[Any], bool] | None = None,
-):
-    def merge_non_boolean_where(
-        where: tuple[int | str | EllipsisType, ...],
-        trace: Sequence[TraceType],
-        leaf: Any,
-    ):
-        names, _, indices = trace
-        is_array = isinstance(leaf, (jax.Array, np.ndarray))
+) -> PyTree:
+    match = False
+
+    def map_func(path: TraceType, _: Any):
+        keys, _ = path
+
+        if len(where) > len(keys):
+            return False
+
+        for wi, key in zip(where, keys):
+            if wi not in (..., *_unpack_entry(key)):
+                return False
+
+        nonlocal match
 
-        if len(where) > len(indices):
-            return jnp.zeros_like(leaf, dtype=bool) if is_array else False
-        for i, item in enumerate(where):
-            if not (item is ... or indices[i] == item or names[i] == item):
-                return jnp.zeros_like(leaf, dtype=bool) if is_array else False
-        return jnp.ones_like(leaf, dtype=bool) if is_array else True
-
-    def merge_boolean_where(*leaves):
-        def is_leaf_bool(leaf: Any) -> bool:
-            return (
-                leaf.dtype == "bool"
-                if hasattr(leaf, "dtype")
-                else isinstance(leaf, bool)
-            )
+        return (match := True)
 
+    mask = tree_map_with_trace(map_func, tree, is_leaf=is_leaf)
+
+    if not match:
+        msg = f"No match is found for path={where} for tree with trace:\n"
+        msg += f"{tree_repr_with_trace(tree)}"
+        raise LookupError(msg)
+
+    return mask
+
+
+def _combine_maybe_bool_masks(*masks: PyTree) -> PyTree:
+    def is_bool_leaf(leaf: Any) -> bool:
+        if hasattr(leaf, "dtype"):
+            return leaf.dtype == "bool"
+        return isinstance(leaf, bool)
+
+    def map_func(*leaves):
         verdict = True
         for leaf in leaves:
-            if not is_leaf_bool(leaf):
-                msg = f"Expected boolean leaf, found {type(leaf).__name__}."
+            if not is_bool_leaf(leaf):
+                msg = f"Expected boolean, got {leaf=}, of type {type(leaf).__name__}."
                 raise TypeError(msg)
             verdict &= leaf
         return verdict
 
+    return jtu.tree_map(map_func, *masks)
+
+
+def _resolve_where(
+    tree: PyTree,
+    where: tuple[int | str | PyTree | EllipsisType, ...],
+    is_leaf: Callable[[Any], bool] | None = None,
+):
     mask = None
 
-    if non_boolean_where := [i for i in where if isinstance(i, (int, str, type(...)))]:
-        func = ft.partial(merge_non_boolean_where, non_boolean_where)
-        mask = tree_map_with_trace(func, tree, is_leaf=is_leaf)
-
-    if boolean_where := [i for i in where if isinstance(i, type(tree))]:
-        args = (mask, *boolean_where) if mask else boolean_where
-        mask = jtu.tree_map(merge_boolean_where, *args)
+    if path := [i for i in where if isinstance(i, (int, str, type(...)))]:
+        mask = _generate_path_mask(tree, path, is_leaf=is_leaf)
+
+    if maybe_bool_masks := [i for i in where if isinstance(i, type(tree))]:
+        all_masks = [mask, *maybe_bool_masks] if mask else maybe_bool_masks
+        mask = _combine_maybe_bool_masks(*all_masks)
 
     return mask
 
 
 def _recursive_getattr(tree: Any, where: tuple[str, ...]):
     def step(tree: Any, where: tuple[str, ...]):
         if len(where) == 1:
@@ -209,43 +220,43 @@
             ">>> # indexing by attribute name\n"
             ">>> tree.at[`attribute_name`].get()\n\n"
             ">>> # indexing by attribute index\n"
             ">>> tree.at[`attribute_index`].get()"
         )
 
     def get(self, *, is_leaf: Callable[[Any], bool] | None = None) -> PyTree:
-        where = _merge_where(self.tree, self.where, is_leaf)
+        where = _resolve_where(self.tree, self.where, is_leaf)
         return _get_at_mask(self.tree, where, is_leaf)
 
     def set(
         self,
         set_value: Any,
         *,
         is_leaf: Callable[[Any], bool] | None = None,
     ) -> PyTree:
-        where = _merge_where(self.tree, self.where, is_leaf)
+        where = _resolve_where(self.tree, self.where, is_leaf)
         return _set_at_mask(self.tree, where, set_value, is_leaf)
 
     def apply(
         self,
         func: Callable[[Any], Any],
         *,
         is_leaf: Callable[[Any], bool] | None = None,
     ) -> PyTree:
-        where = _merge_where(self.tree, self.where, is_leaf)
+        where = _resolve_where(self.tree, self.where, is_leaf)
         return _apply_at_mask(self.tree, where, func, is_leaf)
 
     def reduce(
         self,
         func: Callable[[Any, Any], Any],
         *,
         initializer: Any = _no_initializer,
         is_leaf: Callable[[Any], bool] | None = None,
     ) -> Any:
-        where = _merge_where(self.tree, self.where, is_leaf)
+        where = _resolve_where(self.tree, self.where, is_leaf)
         return _reduce_at_mask(self.tree, where, func, initializer, is_leaf)
 
     def __getattr__(self, name: str) -> AtIndexer:
         # support nested `.at``
         # for example `.at[A].at[B]` represents model.A.B
         if name == "at":
             # pass the current tree and the current path to the next `.at`
@@ -253,49 +264,39 @@
 
         msg = f"{name} is not a valid attribute of {self}\n"
         msg += f"Did you mean to use .at[{name!r}]?"
         raise AttributeError(msg)
 
     def __call__(self, *a, **k) -> tuple[Any, PyTree]:
         with _mutable_context(self.tree, kopy=True) as tree:
-            value = _recursive_getattr(tree, self.where)(*a, **k)
+            value = _recursive_getattr(tree, self.where)(*a, **k)  # type: ignore
         return value, tree
 
 
 def tree_indexer(tree: PyTree) -> AtIndexer:
     """Adds `.at` indexing abilities to a PyTree.
 
     Example:
-        >>> import jax
+        >>> import jax.tree_util as jtu
         >>> import pytreeclass as pytc
-
-        >>> @jax.tree_util.register_pytree_node_class
+        >>> @jax.tree_util.register_pytree_with_keys_class
         ... class Tree:
-        ...     def __init__(self, a, b):
-        ...         self.a = a
-        ...         self.b = b
-        ...     def tree_flatten(self):
-        ...         return (self.a, self.b), None
-        ...     @classmethod
-        ...     def tree_unflatten(cls, aux_data, children):
-        ...         return cls(*children)
-        ...     @property
-        ...     def at(self):
-        ...         return pytc.tree_indexer(self)
-        ...     def __repr__(self) -> str:
-        ...         return f"{self.__class__.__name__}(a={self.a}, b={self.b})"
-
-        >>> # Register the `Tree` class trace function to support indexing
-        >>> def test_trace_func(tree):
-        ...     names = ("a", "b")
-        ...     types = (type(tree.a), type(tree.b))
-        ...     indices = (None, None) # use None to indicate that the attribute is not indexable
-        ...     return [*zip(names, types, indices)]
-
-        >>> pytc.register_pytree_node_trace(Tree, test_trace_func)
+        ...    def __init__(self, a, b):
+        ...        self.a = a
+        ...        self.b = b
+        ...    def tree_flatten_with_keys(self):
+        ...        return ((jtu.GetAttrKey("a"), self.a), (jtu.GetAttrKey("b"), self.b)), None
+        ...    @classmethod
+        ...    def tree_unflatten(cls, aux_data, children):
+        ...        return cls(*children)
+        ...    @property
+        ...    def at(self):
+        ...        return pytc.tree_indexer(self)
+        ...    def __repr__(self) -> str:
+        ...        return f"{self.__class__.__name__}(a={self.a}, b={self.b})"
 
         >>> Tree(1, 2).at["a"].get()
         Tree(a=1, b=None)
     """
     return AtIndexer(tree=tree, where=())
 
 
@@ -518,12 +519,7 @@
 
     for tree in rest:
         leaves, treedef = jtu.tree_flatten(tree)
         if (treedef != treedef0) or verdict is False:
             return False
         verdict = ft.reduce(op.and_, map(_is_leaf_rhs_equal, leaves0, leaves), verdict)
     return verdict
-
-
-def tree_copy(tree: T) -> T:
-    """Return a copy of the tree."""
-    return jtu.tree_unflatten(*jtu.tree_flatten(tree)[::-1])  # type: ignore
```

### Comparing `pytreeclass-0.3.0/pytreeclass/_src/tree_pprint.py` & `pytreeclass-0.3.1/pytreeclass/_src/tree_pprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import math
 from collections import defaultdict
 from itertools import chain
 from types import FunctionType
 from typing import Any, Callable, Literal
 
 import jax
+import jax.tree_util as jtu
 import numpy as np
 from jax._src.custom_derivatives import custom_jvp
 from jax.util import unzip2
 from jaxlib.xla_extension import PjitFunction
 
 import pytreeclass as pytc
 
@@ -348,35 +349,23 @@
 
         >>> print(pytc.tree_str(tree, depth=2))
         {a:1, b:[2, 3], c:{d:4, e:5}, f:[6 7]}
     """
     return _node_pprint(tree, 0, "str", width, depth).expandtabs(tabwidth)
 
 
-def _resolve_names(trace, width: int) -> str:
-    # given a trace with a tuple of names, we resolve the names
-    # to a single string
-    names, _, indices = trace
-    path = ""
-    for i, (name, index) in enumerate(zip(names, indices)):
-        name = f"[{index}]" if name is None else name
-        path += "" if name.startswith("[") else ("." if i > 0 else "")
-        path += _node_pprint(name, 0, "str", width, float("inf"))
-    return path
-
-
 def _is_trace_leaf_depth_factory(depth: int):
     # generate `is_trace_leaf` function to stop tracing at a certain `depth`
     # in essence, depth is the length of the trace entry
     def is_trace_leaf(trace) -> bool:
         # trace is a tuple of (names, leaves, tracers, aux_data)
         # done like this to ensure 4-tuple unpacking
-        names, _, __ = trace
+        keys, _ = trace
         # stop tracing if depth is reached
-        return False if depth is None else (depth <= len(names))
+        return False if depth is None else (depth <= len(keys))
 
     return is_trace_leaf
 
 
 def tree_indent(
     tree: Any,
     *,
@@ -414,28 +403,28 @@
     seen = set()
 
     for trace, leaf in pytc.tree_leaves_with_trace(
         tree=tree,
         is_leaf=is_leaf,
         is_trace_leaf=_is_trace_leaf_depth_factory(depth),
     ):
-        names, types, indices = trace
+        keys, types = trace
 
-        for j, (name, type_, index) in enumerate(zip(names, types, indices)):
-            if (cur := (names[: j + 1], types[: j + 1], indices[: j + 1])) in seen:
+        for j, (key, type_) in enumerate(zip(keys, types)):
+            if (cur := (keys[: j + 1], types[: j + 1])) in seen:
                 # skip printing the common parent node twice
                 continue
             seen.add(cur)
 
-            name = f"[{index}]" if name is None else name
+            name = str(key)
             fmt += "\n" + "\t" * (j + 1)
             fmt += f"{_node_pprint(name,0,'str',width, depth )}"
             fmt += (
                 f"={_node_pprint(leaf,indent=j+1,kind='repr',width=width, depth=depth-1)}"
-                if j == len(names) - 1
+                if j == len(keys) - 1
                 else f":{type_.__name__}"
             )
     return fmt if tabwidth is None else fmt.expandtabs(tabwidth)
 
 
 def _group_by_depth(input: str) -> dict[int, list[list[int]]]:
     # >>> out = """L2
@@ -538,22 +527,22 @@
         ...     b: tuple = (20,30, A())
 
         >>> print(pytc.tree_diagram(B(), depth=0))
         B
 
         >>> print(pytc.tree_diagram(B(), depth=1))
         B
-        ├── a=10
-        └── b=(...)
+        ├── .a=10
+        └── .b=(...)
 
 
         >>> print(pytc.tree_diagram(B(), depth=2))
         B
-        ├── a=10
-        └── b:tuple
+        ├── .a=10
+        └── .b:tuple
             ├── [0]=20
             ├── [1]=30
             └── [2]=A(x=10, y=(...), z=40)
     """
     indent_repr = tree_indent(
         tree,
         width=width,
@@ -866,20 +855,20 @@
         )
     )
 
     for trace, leaf in zip(traces, leaves):
         count = _calculate_count(leaf)
         COUNT += count
 
-        if trace == ((), (), ()):
+        if trace == ((), ()):
             # avoid printing the leaf trace (which is the root of the tree)
             # twice, once as a leaf and once as the root at the end
             continue
 
-        paths = _resolve_names(trace, width=60)
+        paths = jtu.keystr(trace[0])
         types = _node_type_pprint(leaf, indent=0, kind="str", width=60, depth=depth)
         counts = f"{count:,}"
         ROWS += [[paths, types, counts]]
 
     paths = "Σ"
     types = _node_type_pprint(tree, indent=0, kind="str", width=60, depth=depth)
     counts = f"{COUNT:,}"
@@ -949,22 +938,20 @@
 
     Note:
         This function can be useful for debugging and raising descriptive errors.
     """
 
     def leaf_trace_summary(trace, leaf) -> str:
         # this can be useful in debugging and raising descriptive errors
+
         ROWS = [["Value", tree_repr(leaf)]]
 
-        names = "->".join(trace[0])
+        names = "->".join(str(i) for i in trace[0])
         ROWS += [["Name path", names]]
 
         types = "->".join(i.__name__ for i in trace[1])
         ROWS += [["Type path", types]]
 
-        indices = "->".join(str(i) for i in trace[2])
-        ROWS += [["Index path", indices]]
-
         # make a pretty table for each leaf
         return _table(ROWS, transpose=transpose)
 
     return pytc.tree_map_with_trace(leaf_trace_summary, tree, is_leaf=is_leaf)
```

### Comparing `pytreeclass-0.3.0/pytreeclass.egg-info/PKG-INFO` & `pytreeclass-0.3.1/pytreeclass.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.3.0
+Version: 0.3.1
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,15 +32,15 @@
 |[**Quick Example**](#quick_example)
 |[**StatefulComputation**](#stateful_computation)
 |[**More**](#more)
 |[**Acknowledgements**](#acknowledgements)
 
 ![Tests](https://github.com/ASEM000/pytreeclass/actions/workflows/tests.yml/badge.svg)
 ![pyver](https://img.shields.io/badge/python-3.8%203.9%203.10%203.11_-red)
-![pyver](https://img.shields.io/badge/jax-0.4+-red)
+![pyver](https://img.shields.io/badge/jax-0.4.7+-red)
 ![codestyle](https://img.shields.io/badge/codestyle-black-black)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ASEM000/PyTreeClass/blob/main/assets/intro.ipynb)
 [![Downloads](https://pepy.tech/badge/pytreeclass)](https://pepy.tech/project/pytreeclass)
 [![codecov](https://codecov.io/gh/ASEM000/pytreeclass/branch/main/graph/badge.svg?token=TZBRMO0UQH)](https://codecov.io/gh/ASEM000/pytreeclass)
 [![Documentation Status](https://readthedocs.org/projects/pytreeclass/badge/?version=latest)](https://pytreeclass.readthedocs.io/en/latest/?badge=latest)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ASEM000/pytreeclass)
 [![DOI](https://zenodo.org/badge/512717921.svg)](https://zenodo.org/badge/latestdoi/512717921)
@@ -76,47 +76,83 @@
 
 ## ⏩ Quick Example <a id="quick_example">
 
 ### 🏗️ Simple Tree example
 
 <div align="center">
 <table>
-<tr><td align="center">Code</td> <td align="center">PyTree representation</td></tr>
+<tr><td align="center"></td> <td align="center"></td></tr>
 <tr>
 <td>
 
 ```python
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
 
+
 class Tree(pytc.TreeClass):
-    a:int = 1
-    b:tuple[float] = (2.,3.)
-    c:jax.Array = jnp.array([4.,5.,6.])
+    a: int = 1
+    b: tuple = (2, 3.)
+    c: jax.Array = jnp.array([4., 5., 6.])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
 
+
 tree = Tree()
-```
+mask = jax.tree_map(lambda x: x > 5, tree)
+tree = tree \
+       .at["a"].set(10) \
+       .at["b"].at[0].set(10) \
+       .at[mask].set(100)
 
-</td>
+print(tree)
+# Tree(a=10, b=(10, 3.0), c=[  4.   5. 100.])
 
-<td>
+print(pytc.tree_diagram(tree))
+# Tree
+# ├── .a=10
+# ├── .b:tuple
+# │   ├── [0]=10
+# │   └── [1]=3.0
+# └── .c=f32[3](μ=36.33, σ=45.02, ∈[4.00,100.00])
 
-```python
-# leaves are parameters
+print(pytc.tree_summary(tree))
+# ┌─────┬──────┬─────┐
+# │Name │Type  │Count│
+# ├─────┼──────┼─────┤
+# │.a   │int   │1    │
+# ├─────┼──────┼─────┤
+# │.b[0]│int   │1    │
+# ├─────┼──────┼─────┤
+# │.b[1]│float │1    │
+# ├─────┼──────┼─────┤
+# │.c   │f32[3]│3    │
+# ├─────┼──────┼─────┤
+# │Σ    │Tree  │6    │
+# └─────┴──────┴─────┘
+
+
+# ** pass it to jax transformations **
+
+# freeze all non-differentiable parameters to make it
+# work with jax trnasformations
+mask = jax.tree_map(pytc.is_nondiff, tree)
+tree = tree.at[mask].apply(pytc.freeze)
 
-Tree
-    ├── a=1
-    ├── b:tuple
-    │   ├── [0]=2.0
-    │   └── [1]=3.0
-    └── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
+@jax.jit
+@jax.grad
+def sum_tree(tree:Tree, x):
+    # unfreeze before calling tree
+    tree = tree.at[...].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)
+    return sum(tree(x))
+
+print(sum_tree(tree, 1.0))
+# Tree(a=#10, b=(#10, 0.0), c=[1. 1. 1.])
 ```
 
 </td>
 
 </tr>
 </table>
 </div>
@@ -140,52 +176,52 @@
 <td>
 
 ```python
 print(pytc.tree_summary(tree, depth=1))
 ┌────┬──────┬─────┐
 │Name│Type  │Count│
 ├────┼──────┼─────┤
-│a   │int   │1    │
+│.a  │int   │1    │
 ├────┼──────┼─────┤
-│b   │tuple │1    │
+│.b  │tuple │1    │
 ├────┼──────┼─────┤
-│c   │f32[3]│3    │
+│.c  │f32[3]│3    │
 ├────┼──────┼─────┤
 │Σ   │Tree  │5    │
 └────┴──────┴─────┘
 ```
 
 </td>
 
 <td>
 
 ```python
 
 print(pytc.tree_diagram(tree, depth=1))
 Tree
-├── a=1
-├── b=(...)
-└── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
+├── .a=1
+├── .b=(...)
+└── .c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
 ```
 
  </td>
 
 <td>
 
 ```python
 print(pytc.tree_mermaid(tree, depth=1))
 ```
 
 ```mermaid
 
 flowchart LR
     id0(<b>Tree</b>)
-    id0 --- id1("</b>a=1</b>")
-    id0 --- id2("</b>b=(...)</b>")
-    id0 --- id3("</b>c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])</b>")
+    id0 --- id1("</b>.a=1</b>")
+    id0 --- id2("</b>.b=(...)</b>")
+    id0 --- id3("</b>.c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])</b>")
 ```
 
 </td>
 
 <td>
 
 ```python
@@ -208,41 +244,41 @@
 
 <tr>
 
 <td>
 
 ```python
 print(pytc.tree_summary(tree, depth=2))
-┌────┬──────┬─────┐
-│Name│Type  │Count│
-├────┼──────┼─────┤
-│a   │int   │1    │
-├────┼──────┼─────┤
-│b[0]│float │1    │
-├────┼──────┼─────┤
-│b[1]│float │1    │
-├────┼──────┼─────┤
-│c   │f32[3]│3    │
-├────┼──────┼─────┤
-│Σ   │Tree  │6    │
-└────┴──────┴─────┘
+┌─────┬──────┬─────┐
+│Name │Type  │Count│
+├─────┼──────┼─────┤
+│.a   │int   │1    │
+├─────┼──────┼─────┤
+│.b[0]│int   │1    │
+├─────┼──────┼─────┤
+│.b[1]│float │1    │
+├─────┼──────┼─────┤
+│.c   │f32[3]│3    │
+├─────┼──────┼─────┤
+│Σ    │Tree  │6    │
+└─────┴──────┴─────┘
 ```
 
 </td>
 
 <td>
 
 ```python
 print(pytc.tree_diagram(tree, depth=2))
 Tree
-├── a=1
-├── b:tuple
+├── .a=1
+├── .b:tuple
 │   ├── [0]=2.0
 │   └── [1]=3.0
-└── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
+└── .c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
 ```
 
 </td>
 
 <td>
 
 ```python
@@ -250,17 +286,17 @@
 ```
 
 ```mermaid
 flowchart LR
     id2 --- id3("</b>[0]=2.0</b>")
     id2 --- id4("</b>[1]=3.0</b>")
     id0(<b>Tree</b>)
-    id0 --- id1("</b>a=1</b>")
-    id0 --- id2("</b>b:tuple</b>")
-    id0 --- id5("</b>c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])</b>")
+    id0 --- id1("</b>.a=1</b>")
+    id0 --- id2("</b>.b:tuple</b>")
+    id0 --- id5("</b>.c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])</b>")
 ```
 
 </td>
 
 <td>
 
 ```python
@@ -414,14 +450,57 @@
 print(tree.at[1].at[0].set(10))
 # Tree(a=1, b=(10, 3.0), c=[4. 5. 6.])
 
 print(tree.at[1].at[0].apply(lambda x: 10))
 # Tree(a=1, b=(10, 3.0), c=[4. 5. 6.])
 ```
 
+### Mix, match , and chain index update
+
+```python
+
+import jax
+import jax.numpy as jnp
+import pytreeclass as pytc
+
+class Tree(pytc.TreeClass):
+    a: int = 1
+    b: str = "b"
+    c: float = 1.0
+    d: bool = True
+    e: tuple = (1, 2, 3)
+    f: jax.Array = jax.numpy.array([1, 2, 3])
+
+tree = Tree()
+
+integer_mask = jax.tree_util.tree_map(lambda x: isinstance(x, int), tree)
+
+tree = (
+    tree
+    .at["a"].set(10)
+    .at["b"].set("B")
+    .at["c"].set(10.0)
+    .at["d"].set(False)
+    .at["e"].at[0].set(10)  # set first element of tuple to 10
+    .at["f"].apply(jnp.sin)  # apply to all elements in array
+    .at[integer_mask].apply(float)  # cast all `int` to `float`
+)
+
+print(tree)
+# Tree(
+#   a=10.0,
+#   b=B,
+#   c=10.0,
+#   d=0.0,
+#   e=(10.0, 2.0, 3.0),
+#   f=[0.841471  0.9092974 0.14112  ]
+# )
+
+```
+
 </details>
 
 <details>
 
 <summary>
 
 ## 📜 Stateful computations<a id="stateful_computation"></a> </summary>
@@ -456,83 +535,14 @@
 print(counter.calls) # 10
 ```
 
 </details>
 
 ## ➕ More<a id="more"></a>
 
-<details><summary>[Advanced] Register custom user-defined classes to work with visualization and indexing tools. </summary>
-
-Similar to [`jax.tree_util.register_pytree_node`](https://jax.readthedocs.io/en/latest/pytrees.html#extending-pytrees), `PyTreeClass` register common data structures and `treeclass` wrapped classes to figure out how to define the names, types, and index of certain leaf along its path.
-
-Here is an example of registering
-
-```python
-
-class Tree:
-    def __init__(self, a, b):
-        self.a = a
-        self.b = b
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(a={self.a}, b={self.b})"
-
-
-# jax flatten rule
-def tree_flatten(tree):
-    return (tree.a, tree.b), None
-
-# jax unflatten rule
-def tree_unflatten(_, children):
-    return Tree(*children)
-
-# PyTreeClass flatten rule
-def pytc_tree_flatten(tree):
-    names = ("a", "b") # or (`None`, `None`) if name is not defined
-    types = (type(tree.a), type(tree.b))
-    indices = (0,1)  # or (`None`, `None`) if index is not defined
-    return [*zip(names, types, indices)]
-
-
-# Register with `jax`
-jax.tree_util.register_pytree_node(Tree, tree_flatten, tree_unflatten)
-
-# Register the `Tree` class trace function to support indexing
-pytc.register_pytree_node_trace(Tree, pytc_tree_flatten)
-
-tree = Tree(1, 2)
-
-# works with jax
-jax.tree_util.tree_leaves(tree)  # [1, 2]
-
-# works with PyTreeClass viz tools
-print(pytc.tree_summary(tree))
-
-# ┌────┬────┬─────┬──────┐
-# │Name│Type│Count│Size  │
-# ├────┼────┼─────┼──────┤
-# │a   │int │1    │28.00B│
-# ├────┼────┼─────┼──────┤
-# │b   │int │1    │28.00B│
-# ├────┼────┼─────┼──────┤
-# │Σ   │Tree│2    │56.00B│
-# └────┴────┴─────┴──────┘
-
-```
-
-After registeration, you can use internal tools like
-
-- `pytc.tree_map_with_trace`
-- `pytc.tree_leaves_with_trace`
-- `pytc.tree_flatten_with_trace`
-
-More details on that soon.
-
-</details>
-
 <details> <summary>Validate or convert inputs using callbacks</summary>
 
 `PyTreeClass` includes `callbacks` in the `field` to apply a sequence of functions on input at setting the attribute stage. The callback is quite useful in several cases, for instance, to ensure a certain input type within a valid range. See example:
 
 ```python
 import jax
 import pytreeclass as pytc
@@ -806,70 +816,70 @@
 ```
 
 </details>
 
 <details><summary>Use PyTreeClass components with other libraries</summary>
 
 ```python
+
 import jax
 import pytreeclass as pytc
 from flax import struct
 
+import jax
+import pytreeclass as pytc
+from flax import struct
+
+# note that flax is registered with `jax.tree_util.register_pytree_with_keys`
+# otherwise for arbitrary objects you need to do the key registration
+
 @struct.dataclass
 class FlaxTree:
     a:int = 1
     b:tuple[float] = (2.,3.)
     c:jax.Array = jax.numpy.array([4.,5.,6.])
 
     def __repr__(self) -> str:
         return pytc.tree_repr(self)
     def __str__(self) -> str:
         return pytc.tree_str(self)
     @property
     def at(self):
         return pytc.tree_indexer(self)
 
-def pytc_flatten_rule(tree):
-    names =("a","b","c")
-    types = map(type, (tree.a, tree.b, tree.c))
-    indices = range(3)  # make it indexable like namedtuple
-    return [*zip(names, types, indices)]
-
-pytc.register_pytree_node_trace(FlaxTree, pytc_flatten_rule)
-
 flax_tree = FlaxTree()
 
 print(f"{flax_tree!r}")
 # FlaxTree(a=1, b=(2.0, 3.0), c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00]))
 
 print(f"{flax_tree!s}")
 # FlaxTree(a=1, b=(2.0, 3.0), c=[4. 5. 6.])
 
 print(pytc.tree_diagram(flax_tree))
 # FlaxTree
-# ├── a=1
-# ├── b:tuple
+# ├── .a=1
+# ├── .b:tuple
 # │   ├── [0]=2.0
 # │   └── [1]=3.0
-# └── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
+# └── .c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
 
 print(pytc.tree_summary(flax_tree))
-# ┌────┬────────┬─────┐
-# │Name│Type    │Count│
-# ├────┼────────┼─────┤
-# │a   │int     │1    │
-# ├────┼────────┼─────┤
-# │b[0]│float   │1    │
-# ├────┼────────┼─────┤
-# │b[1]│float   │1    │
-# ├────┼────────┼─────┤
-# │c   │f32[3]  │3    │
-# ├────┼────────┼─────┤
-# │Σ   │FlaxTree│6    │
-# └────┴────────┴─────┘
+# ┌─────┬────────┬─────┐
+# │Name │Type    │Count│
+# ├─────┼────────┼─────┤
+# │.a   │int     │1    │
+# ├─────┼────────┼─────┤
+# │.b[0]│float   │1    │
+# ├─────┼────────┼─────┤
+# │.b[1]│float   │1    │
+# ├─────┼────────┼─────┤
+# │.c   │f32[3]  │3    │
+# ├─────┼────────┼─────┤
+# │Σ    │FlaxTree│6    │
+# └─────┴────────┴─────┘
 
 flax_tree.at[0].get()
 # FlaxTree(a=1, b=(None, None), c=None)
 
 flax_tree.at["a"].set(10)
 # FlaxTree(a=10, b=(2.0, 3.0), c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00]))
 ```
@@ -884,117 +894,19 @@
 <table>
 
 <tr><td align="center">CPU</td><td align="center">GPU</td></tr>
 
 <tr>
 
 <td><img src='assets/benchmark_cpu.png'></td>
-<td><img src='assets/benchmark_gpu.png'></td>
 
 </tr>
 
 </table>
 
 </details>
 
-<details> 
-<summary>Use tree_map_with_trace</summary>
-
-V0.2 of `PyTreeClass` register common python datatypes and `treeclass` wrapped class to `trace` registry.
-While `jax` uses `jax.tree_util.register_pytree_node` to define `flatten_rule` for leaves, `PyTreeClass` extends on this
-By registering the `flatten_rule` of (1) names, (2) types, (3) indexing
-
-For demonstration , the following figure contains the 4 variants of the same `Tree` instance define
-
-```python
-import jax
-import jax.numpy as jnp
-import pytreeclass as pytc
-
-class Tree(pytc.TreeClass):
-    a:int = 1
-    b:tuple[float] = (2.,3.)
-    c:jax.Array = jnp.array([4.,5.,6.])
-```
-
-![image](assets/tree_figures.png)
-
-1. Value leaves variant.
-2. Name leaves variant.
-3. Type leaves variant.
-4. Indexing leaves variant.
-
-The four variants can be accessed using `pytc.tree_map_with_trace` .
-Similar to `jax.tree_util.tree_map`, `pytc.tree_map_with_trace` accepts the map function, however the first argument must be the `trace` argument.
-Trace is a four item tuple consists of names,types,indices,metadatas path for each leaf.
-For example for the previous tree, the reuslting trace path for each leaf is :
-
-### Named tree variant
-
-```python
->>> name_tree = pytc.tree_map_with_trace(lambda trace,x : trace[0], tree)
->>> print(name_tree)
-Tree(a=(a), b=((b, [0]), (b, [1])), c=(c))
-```
-
-### Typed tree variant
-
-```python
->>> type_tree = pytc.tree_map_with_trace(lambda trace,x : f"{trace[1]!s}", tree)
->>> print(type_tree)
-Tree(
-  a=(<class 'int'>,),
-  b=((<class 'tuple'>, <class 'float'>), (<class 'tuple'>, <class 'float'>)),
-  c=(<class 'jaxlib.xla_extension.ArrayImpl'>,)
-)
-```
-
-### Index tree variant
-
-```python
->>> index_tree = pytc.tree_map_with_trace(lambda trace,x : trace[2], tree)
->>> print(index_tree)
-Tree(a=(0), b=((1, 0), (1, 1)), c=(2))
-```
-
-In essence, each leaf contains information about the name path, type path, and indices path. The rules for custom types can be registered using `pytc.register_pytree_node_trace`
-
-</details>
-
-<details>
-
-<summary> Comparison with dataclass </summary>
-
-<div align="center">
-<table>
-
-<tr><td></td>  <td>PyTreeClass</td>  <td>dataclass</td></tr>
-
-<tr><td align="center">Generated init method</td> <td align="center">✅</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Generated repr method</td> <td align="center">✅</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Generated str method</td> <td align="center">✅</td>  <td align="center"></td></tr>
-<tr><td align="center">Generated hash method</td> <td align="center">✅</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Generated eq method</td> <td align="center">✅✅*</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Support slots</td> <td align="center"></td>  <td align="center">✅</td></tr>
-<tr><td align="center">Keyword-only args</td> <td align="center">✅</td>  <td align="center">✅ 3.10+</td></tr>
-<tr><td align="center">Positional-only args</td> <td align="center">✅</td>  <td align="center"></td></tr>
-<tr><td align="center">Frozen instance</td> <td align="center">✅**</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Match args support</td> <td align="center"></td>  <td align="center">✅</td></tr>
-<tr><td align="center">Support callbacks</td> <td align="center">✅</td>  <td align="center"></td></tr>
-<tr><td align="center">Support alias name</td> <td align="center">✅</td>  <td align="center"></td></tr>
-</table>
-
-</div>
-
-`*` Either compare the whole instance and return `True/False` or treating it leafwise using `treeclass(..., leafwise=True)` and retrurn `Tree(a=True, ....)`
-
-`**` Always frozen. non-frozen is not supported.
-
-`***` `treeclass` decorator is also a bit faster than `dataclasses.dataclass` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ASEM000/PyTreeClass/blob/main/assets/pytc_dc_benchmark.ipynb)
-
-</details>
-
 ## 📙 Acknowledgements<a id="acknowledgements"></a>
 
 - [Farid Talibli (for visualization link generation backend)](https://www.linkedin.com/in/frdt98)
 - [Treex](https://github.com/cgarciae/treex), [Equinox](https://github.com/patrick-kidger/equinox), [tree-math](https://github.com/google/tree-math), [Flax](https://github.com/google/flax), [TensorFlow](https://www.tensorflow.org), [PyTorch](https://pytorch.org)
 - [Lovely JAX](https://github.com/xl0/lovely-jax)
```

### Comparing `pytreeclass-0.3.0/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.3.1/pytreeclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.0/setup.py` & `pytreeclass-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     author="Mahmoud Asem",
     description=("JAX compatible dataclass."),
     long_description=open(os.path.join(_CURRENT_DIR, "README.md")).read(),
     long_description_content_type="text/markdown",
     author_email="asem00@kaist.ac.kr",
     keywords="python machine-learning pytorch jax",
     packages=find_namespace_packages(exclude=['examples", "tests","experimental']),
-    install_requires=["jax>=0.4.0"],
+    install_requires=["jax>=0.4.7", "typing-extensions"],
     zip_safe=False,
     python_requires=">=3.8",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
```

### Comparing `pytreeclass-0.3.0/tests/test_indexing.py` & `pytreeclass-0.3.1/tests/test_indexing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from collections import namedtuple
+from typing import Any
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy.testing as npt
 import pytest
 
@@ -650,26 +651,31 @@
 
     t = L2()
 
     with pytest.raises(NotImplementedError):
         t.at[None].set(1)
 
 
-def test_register_pytree_node_trace():
-    with pytest.raises(TypeError):
-        pytc.register_pytree_node_trace(None, None)
-
-    with pytest.raises(ValueError):
-        pytc.register_pytree_node_trace(list, lambda x: x)
-
-
 def test_mixed_not_implemented():
     class T(TreeClass):
         a: tuple[int, ...] = namedtuple("a", ["x", "y"])(1, 2)
 
     t = T()
 
     with pytest.raises(NotImplementedError):
         t.at["a"].at[[1]].get()
 
     with pytest.raises(NotImplementedError):
         t.at[0].at[[1]].get()
+
+
+def test_nested_indexing():
+    class Dict(dict):
+        # test `FlattenedIndexKey`
+        pass
+
+    class Tree(pytc.TreeClass, leafwise=True):
+        a: Any = (1, {"b": Dict({"c": 1})})
+
+    tree = Tree()
+    assert jtu.tree_leaves(tree.at["a"].at[1].at["b"].get())[0] == Dict({"c": 1})
+    assert jtu.tree_leaves(tree.at[0].at[1].at["b"].get())[0] == Dict({"c": 1})
```

### Comparing `pytreeclass-0.3.0/tests/test_nn.py` & `pytreeclass-0.3.1/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.0/tests/test_tree_freeze.py` & `pytreeclass-0.3.1/tests/test_tree_freeze.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,17 +130,22 @@
     jtu.tree_map(pytc.freeze, t)
 
     class Test(pytc.TreeClass, leafwise=True):
         a: int
 
     t = jtu.tree_map(pytc.freeze, (Test(100)))
 
-    assert pytc.is_tree_equal(t.at[...].set(0), t)
-    assert pytc.is_tree_equal(t.at[...].apply(lambda x: x + 1), t)
-    assert pytc.is_tree_equal(t.at[...].reduce(jnp.sin, initializer=0), 0.0)
+    with pytest.raises(LookupError):
+        pytc.is_tree_equal(t.at[...].set(0), t)
+
+    with pytest.raises(LookupError):
+        pytc.is_tree_equal(t.at[...].apply(lambda x: x + 1), t)
+
+    with pytest.raises(LookupError):
+        pytc.is_tree_equal(t.at[...].reduce(jnp.add, initializer=0), t)
 
     class Test(pytc.TreeClass, leafwise=True):
         x: jnp.ndarray
 
         def __init__(self, x):
             self.x = x
```

### Comparing `pytreeclass-0.3.0/tests/test_tree_operator.py` & `pytreeclass-0.3.1/tests/test_tree_operator.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.0/tests/test_tree_pprint.py` & `pytreeclass-0.3.1/tests/test_tree_pprint.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,34 +86,34 @@
         tree_summary(r1, depth=0)
         == "┌────┬─────┬─────┐\n│Name│Type │Count│\n├────┼─────┼─────┤\n│Σ   │Repr1│1    │\n└────┴─────┴─────┘"
     )
 
     assert (
         tree_summary(r1, depth=1)
         # trunk-ignore(flake8/E501)
-        == "┌────┬────────────┬─────┐\n│Name│Type        │Count│\n├────┼────────────┼─────┤\n│a   │int         │1    │\n├────┼────────────┼─────┤\n│b   │str         │1    │\n├────┼────────────┼─────┤\n│c   │float       │1    │\n├────┼────────────┼─────┤\n│d   │str         │1    │\n├────┼────────────┼─────┤\n│e   │list        │1    │\n├────┼────────────┼─────┤\n│f   │set         │1    │\n├────┼────────────┼─────┤\n│g   │dict        │1    │\n├────┼────────────┼─────┤\n│h   │f32[5,1]    │5    │\n├────┼────────────┼─────┤\n│i   │f32[1,6]    │6    │\n├────┼────────────┼─────┤\n│j   │f32[1,1,4,5]│20   │\n├────┼────────────┼─────┤\n│k   │tuple       │1    │\n├────┼────────────┼─────┤\n│l   │a           │1    │\n├────┼────────────┼─────┤\n│m   │f32[5,5]    │25   │\n├────┼────────────┼─────┤\n│n   │bool[]      │1    │\n├────┼────────────┼─────┤\n│o   │c64[2]      │2    │\n├────┼────────────┼─────┤\n│Σ   │Repr1       │68   │\n└────┴────────────┴─────┘"
+        == "┌────┬────────────┬─────┐\n│Name│Type        │Count│\n├────┼────────────┼─────┤\n│.a  │int         │1    │\n├────┼────────────┼─────┤\n│.b  │str         │1    │\n├────┼────────────┼─────┤\n│.c  │float       │1    │\n├────┼────────────┼─────┤\n│.d  │str         │1    │\n├────┼────────────┼─────┤\n│.e  │list        │1    │\n├────┼────────────┼─────┤\n│.f  │set         │1    │\n├────┼────────────┼─────┤\n│.g  │dict        │1    │\n├────┼────────────┼─────┤\n│.h  │f32[5,1]    │5    │\n├────┼────────────┼─────┤\n│.i  │f32[1,6]    │6    │\n├────┼────────────┼─────┤\n│.j  │f32[1,1,4,5]│20   │\n├────┼────────────┼─────┤\n│.k  │tuple       │1    │\n├────┼────────────┼─────┤\n│.l  │a           │1    │\n├────┼────────────┼─────┤\n│.m  │f32[5,5]    │25   │\n├────┼────────────┼─────┤\n│.n  │bool[]      │1    │\n├────┼────────────┼─────┤\n│.o  │c64[2]      │2    │\n├────┼────────────┼─────┤\n│Σ   │Repr1       │68   │\n└────┴────────────┴─────┘"
     )
 
     assert (
         tree_summary(r1, depth=2)
         == tree_summary(r1)
         # trunk-ignore(flake8/E501)
-        == "┌──────┬────────────┬─────┐\n│Name  │Type        │Count│\n├──────┼────────────┼─────┤\n│a     │int         │1    │\n├──────┼────────────┼─────┤\n│b     │str         │1    │\n├──────┼────────────┼─────┤\n│c     │float       │1    │\n├──────┼────────────┼─────┤\n│d     │str         │1    │\n├──────┼────────────┼─────┤\n│e[0]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[1]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[2]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[3]  │int         │1    │\n├──────┼────────────┼─────┤\n│e[4]  │int         │1    │\n├──────┼────────────┼─────┤\n│f     │set         │1    │\n├──────┼────────────┼─────┤\n│g['a']│str         │1    │\n├──────┼────────────┼─────┤\n│g['b']│str         │1    │\n├──────┼────────────┼─────┤\n│g['c']│f32[5,5]    │25   │\n├──────┼────────────┼─────┤\n│h     │f32[5,1]    │5    │\n├──────┼────────────┼─────┤\n│i     │f32[1,6]    │6    │\n├──────┼────────────┼─────┤\n│j     │f32[1,1,4,5]│20   │\n├──────┼────────────┼─────┤\n│k[0]  │int         │1    │\n├──────┼────────────┼─────┤\n│k[1]  │int         │1    │\n├──────┼────────────┼─────┤\n│k[2]  │int         │1    │\n├──────┼────────────┼─────┤\n│l.b   │int         │1    │\n├──────┼────────────┼─────┤\n│l.c   │int         │1    │\n├──────┼────────────┼─────┤\n│m     │f32[5,5]    │25   │\n├──────┼────────────┼─────┤\n│n     │bool[]      │1    │\n├──────┼────────────┼─────┤\n│o     │c64[2]      │2    │\n├──────┼────────────┼─────┤\n│Σ     │Repr1       │101  │\n└──────┴────────────┴─────┘"
+        == "┌───────┬────────────┬─────┐\n│Name   │Type        │Count│\n├───────┼────────────┼─────┤\n│.a     │int         │1    │\n├───────┼────────────┼─────┤\n│.b     │str         │1    │\n├───────┼────────────┼─────┤\n│.c     │float       │1    │\n├───────┼────────────┼─────┤\n│.d     │str         │1    │\n├───────┼────────────┼─────┤\n│.e[0]  │int         │1    │\n├───────┼────────────┼─────┤\n│.e[1]  │int         │1    │\n├───────┼────────────┼─────┤\n│.e[2]  │int         │1    │\n├───────┼────────────┼─────┤\n│.e[3]  │int         │1    │\n├───────┼────────────┼─────┤\n│.e[4]  │int         │1    │\n├───────┼────────────┼─────┤\n│.f     │set         │1    │\n├───────┼────────────┼─────┤\n│.g['a']│str         │1    │\n├───────┼────────────┼─────┤\n│.g['b']│str         │1    │\n├───────┼────────────┼─────┤\n│.g['c']│f32[5,5]    │25   │\n├───────┼────────────┼─────┤\n│.h     │f32[5,1]    │5    │\n├───────┼────────────┼─────┤\n│.i     │f32[1,6]    │6    │\n├───────┼────────────┼─────┤\n│.j     │f32[1,1,4,5]│20   │\n├───────┼────────────┼─────┤\n│.k[0]  │int         │1    │\n├───────┼────────────┼─────┤\n│.k[1]  │int         │1    │\n├───────┼────────────┼─────┤\n│.k[2]  │int         │1    │\n├───────┼────────────┼─────┤\n│.l.b   │int         │1    │\n├───────┼────────────┼─────┤\n│.l.c   │int         │1    │\n├───────┼────────────┼─────┤\n│.m     │f32[5,5]    │25   │\n├───────┼────────────┼─────┤\n│.n     │bool[]      │1    │\n├───────┼────────────┼─────┤\n│.o     │c64[2]      │2    │\n├───────┼────────────┼─────┤\n│Σ      │Repr1       │101  │\n└───────┴────────────┴─────┘"
     )
 
 
 def _tree_to_indent(str):
     return str.replace("├── ", "    ").replace("└── ", "    ").replace("│", " ")
 
 
 def test_tree_diagram():
     assert tree_diagram(r1, depth=0) == tree_indent(r1, depth=0) == "Repr1"
 
     # trunk-ignore(flake8/E501)
-    out = "Repr1\n├── a=1\n├── b='string'\n├── c=1.0\n├── d='aaaaa'\n├── e=[...]\n├── f={...}\n├── g={...}\n├── h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── k=(...)\n├── l=a(...)\n├── m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── n=bool[]\n└── o=c64[2]"
+    out = "Repr1\n├── .a=1\n├── .b='string'\n├── .c=1.0\n├── .d='aaaaa'\n├── .e=[...]\n├── .f={...}\n├── .g={...}\n├── .h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .k=(...)\n├── .l=a(...)\n├── .m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .n=bool[]\n└── .o=c64[2]"
 
     assert tree_diagram(r1, depth=1) == out
     assert tree_indent(r1, depth=1) == _tree_to_indent(out)
 
 
 def test_custom_jax_class():
     @jtu.register_pytree_node_class
@@ -127,39 +127,39 @@
 
         @classmethod
         def tree_unflatten(cls, _, children):
             return cls(*children)
 
     t = Test()
 
-    out = "Test\n├── leaf_0=1\n└── leaf_1=2"
+    out = "Test\n├── .leaf_0=1\n└── .leaf_1=2"
     assert tree_diagram(t) == tree_diagram(t, depth=3) == out
 
     assert tree_indent(t) == tree_indent(t, depth=3) == _tree_to_indent(out)
     assert (
         tree_summary(t)
         == tree_summary(t, depth=4)
         # trunk-ignore(flake8/E501)
-        == "┌──────┬────┬─────┐\n│Name  │Type│Count│\n├──────┼────┼─────┤\n│leaf_0│int │1    │\n├──────┼────┼─────┤\n│leaf_1│int │1    │\n├──────┼────┼─────┤\n│Σ     │Test│2    │\n└──────┴────┴─────┘"
+        == "┌───────┬────┬─────┐\n│Name   │Type│Count│\n├───────┼────┼─────┤\n│.leaf_0│int │1    │\n├───────┼────┼─────┤\n│.leaf_1│int │1    │\n├───────┼────┼─────┤\n│Σ      │Test│2    │\n└───────┴────┴─────┘"
     )
 
     assert tree_repr(Test) == repr(Test)
     assert tree_str(Test) == str(Test)
 
 
 def test_tree_mermaid():
     assert (
         tree_mermaid(r1, depth=1)
         # trunk-ignore(flake8/E501)
-        == 'flowchart LR\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>a=1</b>")\n    id0 --- id2("</b>b=\'string\'</b>")\n    id0 --- id3("</b>c=1.0</b>")\n    id0 --- id4("</b>d=\'aaaaa\'</b>")\n    id0 --- id5("</b>e=[...]</b>")\n    id0 --- id6("</b>f={...}</b>")\n    id0 --- id7("</b>g={...}</b>")\n    id0 --- id8("</b>h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id9("</b>i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id10("</b>j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id11("</b>k=(...)</b>")\n    id0 --- id12("</b>l=a(...)</b>")\n    id0 --- id13("</b>m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id14("</b>n=bool[]</b>")\n    id0 --- id15("</b>o=c64[2]</b>")\n'
+        == 'flowchart LR\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>.a=1</b>")\n    id0 --- id2("</b>.b=\'string\'</b>")\n    id0 --- id3("</b>.c=1.0</b>")\n    id0 --- id4("</b>.d=\'aaaaa\'</b>")\n    id0 --- id5("</b>.e=[...]</b>")\n    id0 --- id6("</b>.f={...}</b>")\n    id0 --- id7("</b>.g={...}</b>")\n    id0 --- id8("</b>.h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id9("</b>.i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id10("</b>.j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id11("</b>.k=(...)</b>")\n    id0 --- id12("</b>.l=a(...)</b>")\n    id0 --- id13("</b>.m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id14("</b>.n=bool[]</b>")\n    id0 --- id15("</b>.o=c64[2]</b>")\n'
     )
     assert (
         tree_mermaid(r1, depth=2)
         # trunk-ignore(flake8/E501)
-        == 'flowchart LR\n    id5 --- id6("</b>[0]=10</b>")\n    id5 --- id7("</b>[1]=10</b>")\n    id5 --- id8("</b>[2]=10</b>")\n    id5 --- id9("</b>[3]=10</b>")\n    id5 --- id10("</b>[4]=10</b>")\n    id12 --- id13("</b>[\'a\']=\'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa\'</b>")\n    id12 --- id14("</b>[\'b\']=\'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb\'</b>")\n    id12 --- id15("</b>[\'c\']=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id19 --- id20("</b>[0]=1</b>")\n    id19 --- id21("</b>[1]=2</b>")\n    id19 --- id22("</b>[2]=3</b>")\n    id23 --- id24("</b>b=1</b>")\n    id23 --- id25("</b>c=2</b>")\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>a=1</b>")\n    id0 --- id2("</b>b=\'string\'</b>")\n    id0 --- id3("</b>c=1.0</b>")\n    id0 --- id4("</b>d=\'aaaaa\'</b>")\n    id0 --- id5("</b>e:list</b>")\n    id0 --- id11("</b>f={1, 2, 3}</b>")\n    id0 --- id12("</b>g:dict</b>")\n    id0 --- id16("</b>h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id17("</b>i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id18("</b>j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id19("</b>k:tuple</b>")\n    id0 --- id23("</b>l:a</b>")\n    id0 --- id26("</b>m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id27("</b>n=bool[]</b>")\n    id0 --- id28("</b>o=c64[2]</b>")\n'
+        == 'flowchart LR\n    id5 --- id6("</b>[0]=10</b>")\n    id5 --- id7("</b>[1]=10</b>")\n    id5 --- id8("</b>[2]=10</b>")\n    id5 --- id9("</b>[3]=10</b>")\n    id5 --- id10("</b>[4]=10</b>")\n    id12 --- id13("</b>[\'a\']=\'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa\'</b>")\n    id12 --- id14("</b>[\'b\']=\'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb\'</b>")\n    id12 --- id15("</b>[\'c\']=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id19 --- id20("</b>[0]=1</b>")\n    id19 --- id21("</b>[1]=2</b>")\n    id19 --- id22("</b>[2]=3</b>")\n    id23 --- id24("</b>.b=1</b>")\n    id23 --- id25("</b>.c=2</b>")\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>.a=1</b>")\n    id0 --- id2("</b>.b=\'string\'</b>")\n    id0 --- id3("</b>.c=1.0</b>")\n    id0 --- id4("</b>.d=\'aaaaa\'</b>")\n    id0 --- id5("</b>.e:list</b>")\n    id0 --- id11("</b>.f={1, 2, 3}</b>")\n    id0 --- id12("</b>.g:dict</b>")\n    id0 --- id16("</b>.h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id17("</b>.i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id18("</b>.j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id19("</b>.k:tuple</b>")\n    id0 --- id23("</b>.l:a</b>")\n    id0 --- id26("</b>.m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id27("</b>.n=bool[]</b>")\n    id0 --- id28("</b>.o=c64[2]</b>")\n'
     )
 
 
 def test_misc():
     x = (1, 2, 3)
     assert tree_repr(x) == tree_str(x) == "(1, 2, 3)"
 
@@ -200,29 +200,29 @@
         e: int = 4
         f: L1 = L1()
         g: L0 = L0()
         h: int = 5
 
     tree = L2()
     # trunk-ignore(flake8/E501)
-    out = "L2\n├── e=4\n├── f:L1\n│   ├── c:L0\n│   │   ├── a=1\n│   │   └── b=2\n│   └── d=3\n├── g:L0\n│   ├── a=1\n│   └── b=2\n└── h=5"
+    out = "L2\n├── .e=4\n├── .f:L1\n│   ├── .c:L0\n│   │   ├── .a=1\n│   │   └── .b=2\n│   └── .d=3\n├── .g:L0\n│   ├── .a=1\n│   └── .b=2\n└── .h=5"
 
     assert (tree_diagram(tree)) == out
 
     assert tree_indent(tree) == _tree_to_indent(out)
 
     class L0(TreeClass):
         a: int = 1
 
     class L1(TreeClass):
         b: L0 = L0()
 
     tree = L1()
 
-    assert tree_diagram(tree) == "L1\n└── b:L0\n    └── a=1"
+    assert tree_diagram(tree) == "L1\n└── .b:L0\n    └── .a=1"
 
 
 def test_invalid_depth():
     with pytest.raises(TypeError):
         tree_diagram(1, depth="a")
     with pytest.raises(TypeError):
         tree_summary(1, depth="a")
@@ -236,15 +236,15 @@
         b: float = 2.0
 
     tree = Test()
 
     assert (
         str(tree_repr_with_trace(tree))
         # trunk-ignore(flake8/E501)
-        == "Test(\n  a=\n    ┌──────────┬───┐\n    │Value     │1  │\n    ├──────────┼───┤\n    │Name path │a  │\n    ├──────────┼───┤\n    │Type path │int│\n    ├──────────┼───┤\n    │Index path│0  │\n    └──────────┴───┘, \n  b=\n    ┌──────────┬─────┐\n    │Value     │2.0  │\n    ├──────────┼─────┤\n    │Name path │b    │\n    ├──────────┼─────┤\n    │Type path │float│\n    ├──────────┼─────┤\n    │Index path│1    │\n    └──────────┴─────┘\n)"
+        == "Test(\n  a=\n    ┌─────────┬───┐\n    │Value    │1  │\n    ├─────────┼───┤\n    │Name path│.a │\n    ├─────────┼───┤\n    │Type path│int│\n    └─────────┴───┘, \n  b=\n    ┌─────────┬─────┐\n    │Value    │2.0  │\n    ├─────────┼─────┤\n    │Name path│.b   │\n    ├─────────┼─────┤\n    │Type path│float│\n    └─────────┴─────┘\n)"
     )
 
     assert (
         str(tree_repr_with_trace(tree, transpose=True))
         # trunk-ignore(flake8/E501)
-        == "Test(\n  a=\n    ┌─────┬─────────┬─────────┬──────────┐\n    │Value│Name path│Type path│Index path│\n    ├─────┼─────────┼─────────┼──────────┤\n    │1    │a        │int      │0         │\n    └─────┴─────────┴─────────┴──────────┘, \n  b=\n    ┌─────┬─────────┬─────────┬──────────┐\n    │Value│Name path│Type path│Index path│\n    ├─────┼─────────┼─────────┼──────────┤\n    │2.0  │b        │float    │1         │\n    └─────┴─────────┴─────────┴──────────┘\n)"
+        == "Test(\n  a=\n    ┌─────┬─────────┬─────────┐\n    │Value│Name path│Type path│\n    ├─────┼─────────┼─────────┤\n    │1    │.a       │int      │\n    └─────┴─────────┴─────────┘, \n  b=\n    ┌─────┬─────────┬─────────┐\n    │Value│Name path│Type path│\n    ├─────┼─────────┼─────────┤\n    │2.0  │.b       │float    │\n    └─────┴─────────┴─────────┘\n)"
     )
```

### Comparing `pytreeclass-0.3.0/tests/test_tree_viz_util.py` & `pytreeclass-0.3.1/tests/test_tree_viz_util.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.0/tests/test_under_jit.py` & `pytreeclass-0.3.1/tests/test_under_jit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import jax
 import jax.tree_util as jtu
 import numpy.testing as npt
-import pytest
 from jax import numpy as jnp
 
 import pytreeclass as pytc
 
 
 def test_jit_freeze():
     class Linear(pytc.TreeClass, leafwise=True):
@@ -122,24 +121,22 @@
     def setter(tree):
         return tree.at[...].set(0)
 
     @jax.jit
     def applier(tree):
         return tree.at[...].apply(lambda _: 0)
 
-    with pytest.raises(jax.errors.ConcretizationTypeError):
-        pytc.is_tree_equal(getter(T0()), T0())
+    # with pytest.raises(jax.errors.ConcretizationTypeError):
+    pytc.is_tree_equal(getter(T0()), T0())
 
     assert pytc.is_tree_equal(T0(0, 0, 0), setter(T0()))
 
     assert pytc.is_tree_equal(T0(0, 0, 0), applier(T0()))
 
-    with pytest.raises(jax.errors.ConcretizationTypeError):
-        pytc.is_tree_equal(getter(T1()), T1())
+    # with pytest.raises(jax.errors.ConcretizationTypeError):
+    pytc.is_tree_equal(getter(T1()), T1())
 
-    assert pytc.is_tree_equal(
-        T1(jnp.array(0), jnp.array(0), jnp.array(0), jnp.array([0, 0, 0])), setter(T1())
-    )
+    assert pytc.is_tree_equal(T1(0, 0, 0, 0), setter(T1()))
 
-    assert pytc.is_tree_equal(T1(0, 0, 0, jnp.array([0, 0, 0])), applier(T1()))
+    assert pytc.is_tree_equal(T1(0, 0, 0, 0), applier(T1()))
 
-    assert jax.jit(pytc.is_tree_equal)(T1(0, 0, 0, jnp.array([0, 0, 0])), applier(T1()))
+    assert jax.jit(pytc.is_tree_equal)(T1(0, 0, 0, 0), applier(T1()))
```

