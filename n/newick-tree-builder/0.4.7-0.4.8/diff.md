# Comparing `tmp/newick-tree-builder-0.4.7.tar.gz` & `tmp/newick-tree-builder-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newick-tree-builder-0.4.7.tar", last modified: Tue Apr 18 12:13:17 2023, max compression
+gzip compressed data, was "newick-tree-builder-0.4.8.tar", last modified: Sat Apr 22 16:31:45 2023, max compression
```

## Comparing `newick-tree-builder-0.4.7.tar` & `newick-tree-builder-0.4.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-18 12:13:17.735896 newick-tree-builder-0.4.7/
--rw-r--r--   0 ba        (1000) ba        (1000)      783 2023-04-18 12:13:17.735896 newick-tree-builder-0.4.7/PKG-INFO
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-18 12:13:17.735896 newick-tree-builder-0.4.7/newick/
--rw-r--r--   0 ba        (1000) ba        (1000)        0 2023-04-07 17:41:00.000000 newick-tree-builder-0.4.7/newick/__init__.py
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-18 12:13:17.735896 newick-tree-builder-0.4.7/newick/backend/
--rw-r--r--   0 ba        (1000) ba        (1000)       34 2023-04-08 12:27:05.000000 newick-tree-builder-0.4.7/newick/backend/__init__.py
--rw-r--r--   0 ba        (1000) ba        (1000)     1103 2023-04-14 13:08:53.000000 newick-tree-builder-0.4.7/newick/backend/nhx_util.py
--rw-r--r--   0 ba        (1000) ba        (1000)    24871 2023-04-14 14:57:02.000000 newick-tree-builder-0.4.7/newick/backend/node.py
--rw-r--r--   0 ba        (1000) ba        (1000)     2255 2023-04-14 10:06:26.000000 newick-tree-builder-0.4.7/newick/backend/path.py
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-18 12:13:17.735896 newick-tree-builder-0.4.7/newick/backend/test/
--rw-r--r--   0 ba        (1000) ba        (1000)       32 2023-04-14 12:45:25.000000 newick-tree-builder-0.4.7/newick/backend/test/__init__.py
--rw-r--r--   0 ba        (1000) ba        (1000)      619 2023-04-14 13:09:59.000000 newick-tree-builder-0.4.7/newick/backend/test/test_nhx_util.py
--rw-r--r--   0 ba        (1000) ba        (1000)     3576 2023-04-14 09:39:53.000000 newick-tree-builder-0.4.7/newick/backend/test/test_node.py
--rw-r--r--   0 ba        (1000) ba        (1000)      833 2023-04-14 10:08:13.000000 newick-tree-builder-0.4.7/newick/backend/test/test_path.py
--rw-r--r--   0 ba        (1000) ba        (1000)     1884 2023-04-14 10:45:15.000000 newick-tree-builder-0.4.7/newick/backend/test/test_tree.py
--rw-r--r--   0 ba        (1000) ba        (1000)    13188 2023-04-18 12:00:05.000000 newick-tree-builder-0.4.7/newick/backend/tree.py
--rw-r--r--   0 ba        (1000) ba        (1000)      252 2023-04-08 12:32:42.000000 newick-tree-builder-0.4.7/newick/backend/util_funcs.py
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-18 12:13:17.735896 newick-tree-builder-0.4.7/newick/frontend/
--rw-r--r--   0 ba        (1000) ba        (1000)        0 2023-04-11 18:09:04.000000 newick-tree-builder-0.4.7/newick/frontend/__init__.py
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-18 12:13:17.735896 newick-tree-builder-0.4.7/newick/frontend/test/
--rw-r--r--   0 ba        (1000) ba        (1000)       32 2023-04-14 12:45:30.000000 newick-tree-builder-0.4.7/newick/frontend/test/__init__.py
--rw-r--r--   0 ba        (1000) ba        (1000)     2865 2023-04-14 14:22:50.000000 newick-tree-builder-0.4.7/newick/frontend/test/test_very_basic.py
--rw-r--r--   0 ba        (1000) ba        (1000)     2704 2023-04-18 11:58:22.000000 newick-tree-builder-0.4.7/newick/frontend/very_basic.py
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-18 12:13:17.735896 newick-tree-builder-0.4.7/newick_tree_builder.egg-info/
--rw-r--r--   0 ba        (1000) ba        (1000)      783 2023-04-18 12:13:17.000000 newick-tree-builder-0.4.7/newick_tree_builder.egg-info/PKG-INFO
--rw-r--r--   0 ba        (1000) ba        (1000)      698 2023-04-18 12:13:17.000000 newick-tree-builder-0.4.7/newick_tree_builder.egg-info/SOURCES.txt
--rw-r--r--   0 ba        (1000) ba        (1000)        1 2023-04-18 12:13:17.000000 newick-tree-builder-0.4.7/newick_tree_builder.egg-info/dependency_links.txt
--rw-r--r--   0 ba        (1000) ba        (1000)       24 2023-04-18 12:13:17.000000 newick-tree-builder-0.4.7/newick_tree_builder.egg-info/requires.txt
--rw-r--r--   0 ba        (1000) ba        (1000)        7 2023-04-18 12:13:17.000000 newick-tree-builder-0.4.7/newick_tree_builder.egg-info/top_level.txt
--rw-r--r--   0 ba        (1000) ba        (1000)     1060 2023-04-18 12:12:41.000000 newick-tree-builder-0.4.7/pyproject.toml
--rw-r--r--   0 ba        (1000) ba        (1000)       38 2023-04-18 12:13:17.735896 newick-tree-builder-0.4.7/setup.cfg
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-22 16:31:45.364426 newick-tree-builder-0.4.8/
+-rw-r--r--   0 ba        (1000) ba        (1000)      783 2023-04-22 16:31:45.364426 newick-tree-builder-0.4.8/PKG-INFO
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-22 16:31:45.364426 newick-tree-builder-0.4.8/newick/
+-rw-r--r--   0 ba        (1000) ba        (1000)        0 2023-04-07 17:41:00.000000 newick-tree-builder-0.4.8/newick/__init__.py
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-22 16:31:45.364426 newick-tree-builder-0.4.8/newick/backend/
+-rw-r--r--   0 ba        (1000) ba        (1000)       34 2023-04-08 12:27:05.000000 newick-tree-builder-0.4.8/newick/backend/__init__.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     1103 2023-04-14 13:08:53.000000 newick-tree-builder-0.4.8/newick/backend/nhx_util.py
+-rw-r--r--   0 ba        (1000) ba        (1000)    24871 2023-04-14 14:57:02.000000 newick-tree-builder-0.4.8/newick/backend/node.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     2255 2023-04-14 10:06:26.000000 newick-tree-builder-0.4.8/newick/backend/path.py
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-22 16:31:45.364426 newick-tree-builder-0.4.8/newick/backend/test/
+-rw-r--r--   0 ba        (1000) ba        (1000)       32 2023-04-14 12:45:25.000000 newick-tree-builder-0.4.8/newick/backend/test/__init__.py
+-rw-r--r--   0 ba        (1000) ba        (1000)      619 2023-04-14 13:09:59.000000 newick-tree-builder-0.4.8/newick/backend/test/test_nhx_util.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     3576 2023-04-14 09:39:53.000000 newick-tree-builder-0.4.8/newick/backend/test/test_node.py
+-rw-r--r--   0 ba        (1000) ba        (1000)      833 2023-04-14 10:08:13.000000 newick-tree-builder-0.4.8/newick/backend/test/test_path.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     1884 2023-04-14 10:45:15.000000 newick-tree-builder-0.4.8/newick/backend/test/test_tree.py
+-rw-r--r--   0 ba        (1000) ba        (1000)    13487 2023-04-22 16:21:44.000000 newick-tree-builder-0.4.8/newick/backend/tree.py
+-rw-r--r--   0 ba        (1000) ba        (1000)      252 2023-04-08 12:32:42.000000 newick-tree-builder-0.4.8/newick/backend/util_funcs.py
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-22 16:31:45.364426 newick-tree-builder-0.4.8/newick/frontend/
+-rw-r--r--   0 ba        (1000) ba        (1000)        0 2023-04-11 18:09:04.000000 newick-tree-builder-0.4.8/newick/frontend/__init__.py
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-22 16:31:45.364426 newick-tree-builder-0.4.8/newick/frontend/test/
+-rw-r--r--   0 ba        (1000) ba        (1000)       32 2023-04-14 12:45:30.000000 newick-tree-builder-0.4.8/newick/frontend/test/__init__.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     2865 2023-04-22 16:29:19.000000 newick-tree-builder-0.4.8/newick/frontend/test/test_very_basic.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     2698 2023-04-22 16:29:17.000000 newick-tree-builder-0.4.8/newick/frontend/very_basic.py
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-22 16:31:45.364426 newick-tree-builder-0.4.8/newick_tree_builder.egg-info/
+-rw-r--r--   0 ba        (1000) ba        (1000)      783 2023-04-22 16:31:45.000000 newick-tree-builder-0.4.8/newick_tree_builder.egg-info/PKG-INFO
+-rw-r--r--   0 ba        (1000) ba        (1000)      698 2023-04-22 16:31:45.000000 newick-tree-builder-0.4.8/newick_tree_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 ba        (1000) ba        (1000)        1 2023-04-22 16:31:45.000000 newick-tree-builder-0.4.8/newick_tree_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 ba        (1000) ba        (1000)       24 2023-04-22 16:31:45.000000 newick-tree-builder-0.4.8/newick_tree_builder.egg-info/requires.txt
+-rw-r--r--   0 ba        (1000) ba        (1000)        7 2023-04-22 16:31:45.000000 newick-tree-builder-0.4.8/newick_tree_builder.egg-info/top_level.txt
+-rw-r--r--   0 ba        (1000) ba        (1000)     1060 2023-04-22 16:31:35.000000 newick-tree-builder-0.4.8/pyproject.toml
+-rw-r--r--   0 ba        (1000) ba        (1000)       38 2023-04-22 16:31:45.364426 newick-tree-builder-0.4.8/setup.cfg
```

### Comparing `newick-tree-builder-0.4.7/PKG-INFO` & `newick-tree-builder-0.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newick-tree-builder
-Version: 0.4.7
+Version: 0.4.8
 Summary: Small lib to generate newick trees. Comes with NHX and rudimentary hybridization capabilities.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 Project-URL: Homepage, https://github.com/NiRit100/newick-tree-builder
 Keywords: biology,newick,newick-format,new hampshire,tree,graph-theory,x-nh
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `newick-tree-builder-0.4.7/newick/backend/nhx_util.py` & `newick-tree-builder-0.4.8/newick/backend/nhx_util.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.7/newick/backend/node.py` & `newick-tree-builder-0.4.8/newick/backend/node.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.7/newick/backend/path.py` & `newick-tree-builder-0.4.8/newick/backend/path.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.7/newick/backend/test/test_nhx_util.py` & `newick-tree-builder-0.4.8/newick/backend/test/test_nhx_util.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.7/newick/backend/test/test_node.py` & `newick-tree-builder-0.4.8/newick/backend/test/test_node.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.7/newick/backend/test/test_path.py` & `newick-tree-builder-0.4.8/newick/backend/test/test_path.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.7/newick/backend/test/test_tree.py` & `newick-tree-builder-0.4.8/newick/backend/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.7/newick/backend/tree.py` & `newick-tree-builder-0.4.8/newick/backend/tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,18 +75,17 @@
                 """
                 raise ValueError(root_node, msg)
         #TODO: validate other args
         
         # write class fields 
         self._root = root_node
         self._default_dist = default_dist
-        self._dist_adjust_strat = dist_adjust_strategy if dist_adjust_strategy \
-                                  else self._DIST_ADJUST_STRAT_AVERAGE_fn
         self._hybrids = dict()
         self._hybrid_ignore_set = set()
+        self.set_dist_adjust_strat(dist_adjust_strategy)
 
     
     def node_dist_or_def(self, 
                          dist:float):
         if dist == float("-inf"):
             return self._default_dist
         else:
@@ -249,14 +248,26 @@
                 cpath = cpath[1:]
                 cparent = achild
             ret |= cret
             is_first_path = False
         return ret
     
     
+    def set_dist_adjust_strat(self, dist_adjust_strat:Callable[[Node,float],float]):
+        """Sets the distance adjustment function of this tree. 
+
+        Args:
+            dist_adjust_strat (Callable[[Node,float],float])
+        """
+        if dist_adjust_strat:
+            self._dist_adjust_strat = dist_adjust_strat
+        else:
+            pass  # maybe throw error?
+    
+    
     def to_string(self,
                   with_labels:bool=True,
                   with_distances:bool=True,
                   with_additional_info_nhx:bool=False,
                   append_newline:bool=False,
                   outputlabel_mapper:Mapping[Node,str]=None) -> str:
         """
```

### Comparing `newick-tree-builder-0.4.7/newick/frontend/test/test_very_basic.py` & `newick-tree-builder-0.4.8/newick/frontend/test/test_very_basic.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.7/newick/frontend/very_basic.py` & `newick-tree-builder-0.4.8/newick/frontend/very_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
                      root_label:str=None, 
                      line_delim:str=";", 
                      waypoint_sep:str=",",
                      label_dist_sep:str=":", 
                      trim_sym:str='\r\n ',
                      blacklist:list[str]=["n.a.", "O", "Unclassified"],
                      blacklist_token_strat:BlacklistTokenStrat=BlacklistTokenStrat.DROP_AFTER_FIRST,
-                     default_dist:float=2.0,
+                     default_dist:float=1.0,
                      dist_adjust_strategy:Callable[[Node,float],float]=None) -> Tree:
     index = 0
     lines = text.split(line_delim)
     outtree = Tree(RootNode(root_label), 
-                   default_dist=default_dist,
-                   dist_adjust_strategy=dist_adjust_strategy)
+                   default_dist=default_dist)
+    outtree.set_dist_adjust_strat(dist_adjust_strategy)
     for line in lines:
         line = clean_token(line, trim_sym)
         if line != "":
             waypoints = line.split(waypoint_sep)
             outpath = Path(root_label=root_label)
             for waypoint in waypoints:
                 flag_drop_after_token = False
```

### Comparing `newick-tree-builder-0.4.7/newick_tree_builder.egg-info/PKG-INFO` & `newick-tree-builder-0.4.8/newick_tree_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newick-tree-builder
-Version: 0.4.7
+Version: 0.4.8
 Summary: Small lib to generate newick trees. Comes with NHX and rudimentary hybridization capabilities.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 Project-URL: Homepage, https://github.com/NiRit100/newick-tree-builder
 Keywords: biology,newick,newick-format,new hampshire,tree,graph-theory,x-nh
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `newick-tree-builder-0.4.7/newick_tree_builder.egg-info/SOURCES.txt` & `newick-tree-builder-0.4.8/newick_tree_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.7/pyproject.toml` & `newick-tree-builder-0.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "newick-tree-builder"
-version = "0.4.7"
+version = "0.4.8"
 description = "Small lib to generate newick trees. Comes with NHX and rudimentary hybridization capabilities."
 authors = [{ name = "Nico Rittinghaus", email = "nico@ritti.ng" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

