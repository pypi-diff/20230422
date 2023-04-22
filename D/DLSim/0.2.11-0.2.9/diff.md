# Comparing `tmp/DLSim-0.2.11.tar.gz` & `tmp/DLSim-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLSim-0.2.11.tar", last modified: Sat Apr 22 00:12:48 2023, max compression
+gzip compressed data, was "DLSim-0.2.9.tar", last modified: Mon Apr 17 22:19:09 2023, max compression
```

## Comparing `DLSim-0.2.11.tar` & `DLSim-0.2.9.tar`

### file list

```diff
@@ -1,26 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 00:12:48.006641 DLSim-0.2.11/
-drwxrwxrwx   0        0        0        0 2023-04-22 00:12:47.852269 DLSim-0.2.11/DLSim/
-drwxrwxrwx   0        0        0        0 2023-04-22 00:12:47.869255 DLSim-0.2.11/DLSim/DLSim/
--rw-rw-rw-   0        0        0     7774 2023-04-21 23:58:18.000000 DLSim-0.2.11/DLSim/DLSim/DLSim.py
--rw-rw-rw-   0        0        0      424 2023-04-21 23:58:35.000000 DLSim-0.2.11/DLSim/DLSim/__init__.py
--rw-rw-rw-   0        0        0      325 2023-04-21 22:55:04.000000 DLSim-0.2.11/DLSim/DLSim/_init_api.py
--rw-rw-rw-   0        0        0     4354 2023-04-21 23:48:10.000000 DLSim-0.2.11/DLSim/DLSim/func_lib.py
-drwxrwxrwx   0        0        0        0 2023-04-22 00:12:48.002213 DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/
--rw-rw-rw-   0        0        0   181248 2023-01-13 07:12:46.000000 DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/DTALite.dll
--rw-rw-rw-   0        0        0   225704 2023-01-13 07:12:46.000000 DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/DTALite.so
--rw-rw-rw-   0        0        0   250141 2023-01-13 07:12:46.000000 DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/DTALite_arm.dylib
--rw-rw-rw-   0        0        0   269200 2023-01-13 07:12:46.000000 DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/DTALite_x86.dylib
--rw-rw-rw-   0        0        0      278 2023-04-17 17:37:11.000000 DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/__init__.py
--rw-rw-rw-   0        0        0    11776 2023-01-13 07:12:46.000000 DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/path_engine.dll
--rw-rw-rw-   0        0        0    12208 2023-01-13 07:12:46.000000 DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/path_engine.so
--rw-rw-rw-   0        0        0    33553 2023-01-13 07:12:46.000000 DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/path_engine_arm.dylib
--rw-rw-rw-   0        0        0    49560 2023-01-13 07:12:46.000000 DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/path_engine_x86.dylib
-drwxrwxrwx   0        0        0        0 2023-04-22 00:12:47.895257 DLSim-0.2.11/DLSim/DLSim.egg-info/
--rw-rw-rw-   0        0        0     3667 2023-04-22 00:12:47.000000 DLSim-0.2.11/DLSim/DLSim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2023-04-22 00:12:47.000000 DLSim-0.2.11/DLSim/DLSim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 00:12:47.000000 DLSim-0.2.11/DLSim/DLSim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-22 00:12:47.000000 DLSim-0.2.11/DLSim/DLSim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3667 2023-04-22 00:12:48.005208 DLSim-0.2.11/PKG-INFO
--rw-rw-rw-   0        0        0     3046 2023-04-22 00:10:16.000000 DLSim-0.2.11/README.md
--rw-rw-rw-   0        0        0       42 2023-04-22 00:12:48.006641 DLSim-0.2.11/setup.cfg
--rw-rw-rw-   0        0        0     1480 2023-04-22 00:07:09.000000 DLSim-0.2.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:19:09.099168 DLSim-0.2.9/
+drwxrwxrwx   0        0        0        0 2023-04-17 22:19:09.012169 DLSim-0.2.9/DLSim/
+drwxrwxrwx   0        0        0        0 2023-04-17 22:19:09.051160 DLSim-0.2.9/DLSim/DLSim/
+-rw-rw-rw-   0        0        0    37812 2023-04-16 23:20:13.000000 DLSim-0.2.9/DLSim/DLSim/DLSim.py
+-rw-rw-rw-   0        0        0      302 2023-04-16 23:29:57.000000 DLSim-0.2.9/DLSim/DLSim/__init__.py
+-rw-rw-rw-   0        0        0      367 2023-04-17 16:33:35.000000 DLSim-0.2.9/DLSim/DLSim/_init_api.py
+-rw-rw-rw-   0        0        0    33862 2023-04-15 17:38:56.000000 DLSim-0.2.9/DLSim/DLSim/agent.csv
+-rw-rw-rw-   0        0        0    11082 2023-04-15 17:38:56.000000 DLSim-0.2.9/DLSim/DLSim/input_agent.csv
+-rw-rw-rw-   0        0        0     2425 2023-04-15 17:38:56.000000 DLSim-0.2.9/DLSim/DLSim/link.csv
+-rw-rw-rw-   0        0        0     3917 2023-04-15 17:38:56.000000 DLSim-0.2.9/DLSim/DLSim/link_performance.csv
+-rw-rw-rw-   0        0        0        0 2023-04-16 21:20:07.000000 DLSim-0.2.9/DLSim/DLSim/log.txt
+-rw-rw-rw-   0        0        0      511 2023-04-15 17:38:56.000000 DLSim-0.2.9/DLSim/DLSim/node.csv
+-rw-rw-rw-   0        0        0     3577 2023-04-17 18:49:21.000000 DLSim-0.2.9/DLSim/DLSim/pydtalite.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:19:09.094164 DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/
+-rw-rw-rw-   0        0        0   181248 2023-01-13 07:12:46.000000 DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/DTALite.dll
+-rw-rw-rw-   0        0        0   225704 2023-01-13 07:12:46.000000 DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/DTALite.so
+-rw-rw-rw-   0        0        0   250141 2023-01-13 07:12:46.000000 DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/DTALite_arm.dylib
+-rw-rw-rw-   0        0        0   269200 2023-01-13 07:12:46.000000 DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/DTALite_x86.dylib
+-rw-rw-rw-   0        0        0      278 2023-04-17 17:37:11.000000 DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/__init__.py
+-rw-rw-rw-   0        0        0    11776 2023-01-13 07:12:46.000000 DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/path_engine.dll
+-rw-rw-rw-   0        0        0    12208 2023-01-13 07:12:46.000000 DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/path_engine.so
+-rw-rw-rw-   0        0        0    33553 2023-01-13 07:12:46.000000 DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/path_engine_arm.dylib
+-rw-rw-rw-   0        0        0    49560 2023-01-13 07:12:46.000000 DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/path_engine_x86.dylib
+-rw-rw-rw-   0        0        0       98 2023-04-15 17:38:56.000000 DLSim-0.2.9/DLSim/DLSim/solution.csv
+drwxrwxrwx   0        0        0        0 2023-04-17 22:19:09.066167 DLSim-0.2.9/DLSim/DLSim.egg-info/
+-rw-rw-rw-   0        0        0     4107 2023-04-17 22:19:08.000000 DLSim-0.2.9/DLSim/DLSim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      803 2023-04-17 22:19:09.000000 DLSim-0.2.9/DLSim/DLSim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 22:19:08.000000 DLSim-0.2.9/DLSim/DLSim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-17 22:19:08.000000 DLSim-0.2.9/DLSim/DLSim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4107 2023-04-17 22:19:09.097165 DLSim-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3487 2023-04-17 18:53:30.000000 DLSim-0.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 22:19:09.099168 DLSim-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1479 2023-04-17 22:18:14.000000 DLSim-0.2.9/setup.py
```

### Comparing `DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/DTALite.dll` & `DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/DTALite.dll`

 * *Files identical despite different names*

### Comparing `DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/DTALite.so` & `DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/DTALite.so`

 * *Files identical despite different names*

### Comparing `DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/DTALite_arm.dylib` & `DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/DTALite_arm.dylib`

 * *Files identical despite different names*

### Comparing `DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/DTALite_x86.dylib` & `DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/DTALite_x86.dylib`

 * *Files identical despite different names*

### Comparing `DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/path_engine.dll` & `DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/path_engine.dll`

 * *Files identical despite different names*

### Comparing `DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/path_engine.so` & `DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/path_engine.so`

 * *Files identical despite different names*

### Comparing `DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/path_engine_arm.dylib` & `DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/path_engine_arm.dylib`

 * *Files identical despite different names*

### Comparing `DLSim-0.2.11/DLSim/DLSim/pydtalite_bin/path_engine_x86.dylib` & `DLSim-0.2.9/DLSim/DLSim/pydtalite_bin/path_engine_x86.dylib`

 * *Files identical despite different names*

### Comparing `DLSim-0.2.11/DLSim/DLSim.egg-info/PKG-INFO` & `DLSim-0.2.9/DLSim/DLSim.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLSim
-Version: 0.2.11
+Version: 0.2.9
 Summary: DLSim is an open-source, cross-platform, lightweight, and fast Python traffic assignment tool adopted and modified from ASU TransAI Lab
 Home-page: https://github.com/asu-trans-ai-lab/DLSim
 Author: Dr.Xuesong (Simon) Zhou, Dr.Cafer Avci, Xiangyong Luo
 Author-email: xzhou74@asu.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -13,60 +13,66 @@
 
 "Dynamic Traffic Simulation Package with Multi-Resolution Modelling" (DLSim-MRM) is an open source, high-fidelity multi-resolution (i.e., macroscopic, mesoscopic, and microscopic simulation) traffic simulation package which users jointly apply varying temporal and spatial resolutions to solve a single question or set of questions that mirror the physical world with complex intersections. Users can perform traffic assignments and feed results from one model to another while maintaining consistency between the model assumptions. DLSim-MRM typically takes the following steps for simulation based on [General Modeling Network Specification (GMNS)](https://github.com/zephyr-data-specs/GMNS) format:
 
 1. Use demand forecasting models to determine overall trip patterns in a regional network, including trip generation, trip distribution, mode split, and initial O-D matrices.
 2. Use mesoscopic simulation-based dynamic traffic assignment (DTA) to realistically assign traffic to the network by accounting for strategic traveler behavior.
 3. Use microscopic analysis of traffic at the corridor level or subnetwork level.
 
+
 DLSim-MRM uses 3 open-source packages; [OSM2GMNS](https://github.com/asu-trans-ai-lab/OSM2GMNS), [Path4GMNS](https://github.com/asu-trans-ai-lab/Path4GMNS) and [Vol2Timing](https://github.com/asu-trans-ai-lab/Vol2Timing) with the additional developments along the multi-resolution modelling and dyanmic traffic simulation.
 
 -OSM2GMNS can help users easily convert networks from OpenStreetMap to .csv files with standard GMNS format for visualization, traffic simulation and planning purpose.
 
 -Path4GMNS is an open-source AMS library for efficiently macroscopic and mesoscopic traffic assignment based on General Modeling Network Specification (GMNS) format.
 
 -Vol2Timing is a python tool aims to offer a light-weight computational engine to generate optimize signal control timing data, and analyze the effectiveness of signal control strategies.
 
+
 ## Installation:
 
 DLSim has been published on [PyPI](https://pypi.org/project/dlsim/), and can be installed by using package manager [pip](https://pip.pypa.io/en/stable/) to install DLSim.
 
 ```
 pip install DLSim
 ```
 
 If you need a specific version of DLSim, say, 0.2.1,
 
 ```
-$ pip install dlsim==0.2.11
+$ pip install dlsim==0.2.5
 ```
 
 ## Usage
 
 Find the shortest path (based on distance) and output it in the format of a sequence of node/link IDs.
 
 ```
-from DLSim import DLSim
-
-# load the DLSim class
-DL = DLSim()
-
-# check the working directory
-DL.check_working_directory()
-
-# check all the required files exist
-DL.check_DLSim_input_files()
-
-# load and update settings
-DL.DLSim_settings
-
-# perform kernel network assignment simulation
-DL.perform_kernel_network_assignment_simulation()
-
+import DLSim as ds
+import time
 
+network = ds.Network()
 
+ds.g_ReadInputData(network.node_list,
+                   network.link_list,
+                   network.agent_list,
+                   network.internal_node_seq_no_dict,
+                   network.external_node_id_dict,
+                   network.agent_td_list_dict,
+                   network.zone_to_nodes_dict,network.node_seq_to_link_seq)
+network.allocate()
+
+ds.begin_time = time.time()
+
+ds.g_find_shortest_path_for_agent(network)
+ds.g_TrafficSimulation(network.node_list, network.link_list,
+                       network.agent_list, network.agent_td_list_dict)
+ds.end_time = time.time()
+ds.g_OutputFiles(network.link_list,
+                 network.agent_list,
+                 network.external_node_id_dict)
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please [open an issue](https://github.com/asu-trans-ai-lab/DLSim-MRM) first to discuss what you would like to change.
 
 ## License
```

### Comparing `DLSim-0.2.11/DLSim/DLSim.egg-info/SOURCES.txt` & `DLSim-0.2.9/DLSim/DLSim.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 README.md
 setup.py
 DLSim/DLSim/DLSim.py
 DLSim/DLSim/__init__.py
 DLSim/DLSim/_init_api.py
-DLSim/DLSim/func_lib.py
+DLSim/DLSim/agent.csv
+DLSim/DLSim/input_agent.csv
+DLSim/DLSim/link.csv
+DLSim/DLSim/link_performance.csv
+DLSim/DLSim/log.txt
+DLSim/DLSim/node.csv
+DLSim/DLSim/pydtalite.py
+DLSim/DLSim/solution.csv
 DLSim/DLSim.egg-info/PKG-INFO
 DLSim/DLSim.egg-info/SOURCES.txt
 DLSim/DLSim.egg-info/dependency_links.txt
 DLSim/DLSim.egg-info/top_level.txt
 DLSim/DLSim/pydtalite_bin/DTALite.dll
 DLSim/DLSim/pydtalite_bin/DTALite.so
 DLSim/DLSim/pydtalite_bin/DTALite_arm.dylib
```

### Comparing `DLSim-0.2.11/PKG-INFO` & `DLSim-0.2.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLSim
-Version: 0.2.11
+Version: 0.2.9
 Summary: DLSim is an open-source, cross-platform, lightweight, and fast Python traffic assignment tool adopted and modified from ASU TransAI Lab
 Home-page: https://github.com/asu-trans-ai-lab/DLSim
 Author: Dr.Xuesong (Simon) Zhou, Dr.Cafer Avci, Xiangyong Luo
 Author-email: xzhou74@asu.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -13,60 +13,66 @@
 
 "Dynamic Traffic Simulation Package with Multi-Resolution Modelling" (DLSim-MRM) is an open source, high-fidelity multi-resolution (i.e., macroscopic, mesoscopic, and microscopic simulation) traffic simulation package which users jointly apply varying temporal and spatial resolutions to solve a single question or set of questions that mirror the physical world with complex intersections. Users can perform traffic assignments and feed results from one model to another while maintaining consistency between the model assumptions. DLSim-MRM typically takes the following steps for simulation based on [General Modeling Network Specification (GMNS)](https://github.com/zephyr-data-specs/GMNS) format:
 
 1. Use demand forecasting models to determine overall trip patterns in a regional network, including trip generation, trip distribution, mode split, and initial O-D matrices.
 2. Use mesoscopic simulation-based dynamic traffic assignment (DTA) to realistically assign traffic to the network by accounting for strategic traveler behavior.
 3. Use microscopic analysis of traffic at the corridor level or subnetwork level.
 
+
 DLSim-MRM uses 3 open-source packages; [OSM2GMNS](https://github.com/asu-trans-ai-lab/OSM2GMNS), [Path4GMNS](https://github.com/asu-trans-ai-lab/Path4GMNS) and [Vol2Timing](https://github.com/asu-trans-ai-lab/Vol2Timing) with the additional developments along the multi-resolution modelling and dyanmic traffic simulation.
 
 -OSM2GMNS can help users easily convert networks from OpenStreetMap to .csv files with standard GMNS format for visualization, traffic simulation and planning purpose.
 
 -Path4GMNS is an open-source AMS library for efficiently macroscopic and mesoscopic traffic assignment based on General Modeling Network Specification (GMNS) format.
 
 -Vol2Timing is a python tool aims to offer a light-weight computational engine to generate optimize signal control timing data, and analyze the effectiveness of signal control strategies.
 
+
 ## Installation:
 
 DLSim has been published on [PyPI](https://pypi.org/project/dlsim/), and can be installed by using package manager [pip](https://pip.pypa.io/en/stable/) to install DLSim.
 
 ```
 pip install DLSim
 ```
 
 If you need a specific version of DLSim, say, 0.2.1,
 
 ```
-$ pip install dlsim==0.2.11
+$ pip install dlsim==0.2.5
 ```
 
 ## Usage
 
 Find the shortest path (based on distance) and output it in the format of a sequence of node/link IDs.
 
 ```
-from DLSim import DLSim
-
-# load the DLSim class
-DL = DLSim()
-
-# check the working directory
-DL.check_working_directory()
-
-# check all the required files exist
-DL.check_DLSim_input_files()
-
-# load and update settings
-DL.DLSim_settings
-
-# perform kernel network assignment simulation
-DL.perform_kernel_network_assignment_simulation()
-
+import DLSim as ds
+import time
 
+network = ds.Network()
 
+ds.g_ReadInputData(network.node_list,
+                   network.link_list,
+                   network.agent_list,
+                   network.internal_node_seq_no_dict,
+                   network.external_node_id_dict,
+                   network.agent_td_list_dict,
+                   network.zone_to_nodes_dict,network.node_seq_to_link_seq)
+network.allocate()
+
+ds.begin_time = time.time()
+
+ds.g_find_shortest_path_for_agent(network)
+ds.g_TrafficSimulation(network.node_list, network.link_list,
+                       network.agent_list, network.agent_td_list_dict)
+ds.end_time = time.time()
+ds.g_OutputFiles(network.link_list,
+                 network.agent_list,
+                 network.external_node_id_dict)
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please [open an issue](https://github.com/asu-trans-ai-lab/DLSim-MRM) first to discuss what you would like to change.
 
 ## License
```

### Comparing `DLSim-0.2.11/setup.py` & `DLSim-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open("requirements.txt", "r", encoding="utf-8") as f:
         modules_needed = [i.strip() for i in fh.readlines()]
 except Exception:
     modules_needed = []
 
 setuptools.setup(
     name="DLSim",
-    version="0.2.11",
+    version="0.2.9",
     author="Dr.Xuesong (Simon) Zhou, Dr.Cafer Avci, Xiangyong Luo",
     author_email="xzhou74@asu.edu",
     License="Apache Software License (http://www.apache.org/licenses/LICENSE-2.0)",
     description="DLSim is an open-source, cross-platform, lightweight, and fast Python traffic assignment tool adopted and modified from ASU TransAI Lab",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/asu-trans-ai-lab/DLSim",
```

