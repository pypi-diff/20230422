# Comparing `tmp/fabrictestbed-extensions-1.4.2rc6.tar.gz` & `tmp/fabrictestbed-extensions-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-extensions-1.4.2rc6.tar", last modified: Thu Apr 20 18:03:41 2023, max compression
+gzip compressed data, was "fabrictestbed-extensions-1.4.3.tar", last modified: Sat Apr 22 14:14:37 2023, max compression
```

## Comparing `fabrictestbed-extensions-1.4.2rc6.tar` & `fabrictestbed-extensions-1.4.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1025 2023-02-13 18:31:49.552350 fabrictestbed-extensions-1.4.2rc6/.github/workflows/build.yml
--rw-r--r--   0        0        0     1618 2023-04-06 16:18:57.453917 fabrictestbed-extensions-1.4.2rc6/.github/workflows/checks.yml
--rw-r--r--   0        0        0     2402 2023-04-06 16:18:57.454239 fabrictestbed-extensions-1.4.2rc6/.github/workflows/test.yml
--rw-r--r--   0        0        0     1799 2022-08-18 16:55:06.303125 fabrictestbed-extensions-1.4.2rc6/.gitignore
--rw-r--r--   0        0        0      666 2023-02-13 18:31:49.552528 fabrictestbed-extensions-1.4.2rc6/.readthedocs.yaml
--rw-r--r--   0        0        0     2395 2023-04-20 18:01:14.627945 fabrictestbed-extensions-1.4.2rc6/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2022-08-18 16:55:06.303384 fabrictestbed-extensions-1.4.2rc6/LICENSE
--rw-r--r--   0        0        0     4054 2023-04-06 16:18:57.455050 fabrictestbed-extensions-1.4.2rc6/README.md
--rw-r--r--   0        0        0      638 2022-08-18 16:55:06.303668 fabrictestbed-extensions-1.4.2rc6/docs/Makefile
--rw-r--r--   0        0        0      799 2022-08-18 16:55:06.303743 fabrictestbed-extensions-1.4.2rc6/docs/make.bat
--rw-r--r--   0        0        0     1996 2023-02-13 18:31:49.552781 fabrictestbed-extensions-1.4.2rc6/docs/source/conf.py
--rw-r--r--   0        0        0     8869 2022-10-28 15:15:07.136211 fabrictestbed-extensions-1.4.2rc6/docs/source/fablib.rst
--rw-r--r--   0        0        0     4470 2023-04-06 16:18:57.455278 fabrictestbed-extensions-1.4.2rc6/docs/source/index.rst
--rw-r--r--   0        0        0      151 2023-04-20 18:01:14.628067 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/__init__.py
--rw-r--r--   0        0        0        2 2023-02-13 18:31:49.553082 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/editors/__init__.py
--rw-r--r--   0        0        0    18044 2023-02-13 18:31:49.553270 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/editors/abc_topology_editor.py
--rw-r--r--   0        0        0     6277 2023-02-13 18:31:49.553528 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
--rw-r--r--   0        0        0    68479 2023-02-13 18:31:49.553650 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/editors/geo_topology_editor.py
--rw-r--r--   0        0        0        1 2022-08-18 16:55:06.304986 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/__init__.py
--rw-r--r--   0        0        0     4793 2023-02-13 18:31:49.553839 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/abc_fablib.py
--rw-r--r--   0        0        0    21062 2023-04-20 18:01:14.628314 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/component.py
--rw-r--r--   0        0        0    76799 2023-04-20 18:01:14.628593 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/fablib.py
--rw-r--r--   0        0        0     5807 2023-02-13 18:31:49.554628 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/facility_port.py
--rw-r--r--   0        0        0    25825 2023-04-20 18:01:14.628746 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/interface.py
--rw-r--r--   0        0        0    39140 2023-04-20 18:01:14.628864 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/network_service.py
--rw-r--r--   0        0        0    95917 2023-04-20 18:01:14.629267 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/node.py
--rw-r--r--   0        0        0    34672 2023-04-20 18:01:14.629639 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/resources.py
--rw-r--r--   0        0        0    81904 2023-04-20 18:01:14.629937 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/slice.py
--rw-r--r--   0        0        0        2 2023-02-13 18:31:49.555813 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/images/__init__.py
--rw-r--r--   0        0        0   199914 2022-08-18 16:55:06.307676 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/images/fabric_logo.png
--rw-r--r--   0        0        0     1316 2022-08-18 16:55:06.307757 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/images/server.png
--rw-r--r--   0        0        0    62250 2022-08-18 16:55:06.307862 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/images/slice_rack.png
--rw-r--r--   0        0        0        2 2023-02-13 18:31:49.555903 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/__init__.py
--rw-r--r--   0        0        0    14765 2023-02-13 18:31:49.556039 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/abc_test.py
--rw-r--r--   0        0        0    34231 2023-02-13 18:31:49.556263 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/component_tests.py
--rw-r--r--   0        0        0       85 2023-02-13 18:31:49.556325 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/dummy-token.json
--rw-r--r--   0        0        0    13366 2023-02-13 18:31:49.556445 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
--rw-r--r--   0        0        0    10227 2023-02-13 18:31:49.556551 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/hello_fabric.py
--rw-r--r--   0        0        0    20659 2023-02-13 18:31:49.556711 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/link_benchmark.py
--rw-r--r--   0        0        0    20919 2023-02-13 18:31:49.556814 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/local_network_benchmark.py
--rw-r--r--   0        0        0    44883 2023-02-13 18:31:49.557045 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/network_benchmark_tests.py
--rw-r--r--   0        0        0    10052 2023-02-13 18:31:49.557127 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/nvme_benchmark.py
--rw-r--r--   0        0        0     5095 2023-04-06 16:18:57.459146 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/test_basic.py
--rw-r--r--   0        0        0        2 2023-02-13 18:31:49.557261 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/utils/__init__.py
--rw-r--r--   0        0        0     3082 2023-02-13 18:31:49.557349 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/utils/abc_utils.py
--rw-r--r--   0        0        0     3304 2023-02-13 18:31:49.557428 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/utils/node.py
--rw-r--r--   0        0        0     8436 2023-02-13 18:31:49.557517 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/utils/slice.py
--rw-r--r--   0        0        0     1318 2023-04-20 18:01:14.630443 fabrictestbed-extensions-1.4.2rc6/pyproject.toml
--rwxr-xr-x   0        0        0      122 2022-08-18 16:55:06.309489 fabrictestbed-extensions-1.4.2rc6/sphinx.sh
--rw-r--r--   0        0        0     5267 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.4.2rc6/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-02-13 18:31:49.552350 fabrictestbed-extensions-1.4.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1618 2023-04-06 16:18:57.453917 fabrictestbed-extensions-1.4.3/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     2402 2023-04-06 16:18:57.454239 fabrictestbed-extensions-1.4.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1799 2022-08-18 16:55:06.303125 fabrictestbed-extensions-1.4.3/.gitignore
+-rw-r--r--   0        0        0      666 2023-02-13 18:31:49.552528 fabrictestbed-extensions-1.4.3/.readthedocs.yaml
+-rw-r--r--   0        0        0     2670 2023-04-22 14:13:43.304083 fabrictestbed-extensions-1.4.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2022-08-18 16:55:06.303384 fabrictestbed-extensions-1.4.3/LICENSE
+-rw-r--r--   0        0        0     4054 2023-04-21 21:53:04.312013 fabrictestbed-extensions-1.4.3/README.md
+-rw-r--r--   0        0        0      638 2022-08-18 16:55:06.303668 fabrictestbed-extensions-1.4.3/docs/Makefile
+-rw-r--r--   0        0        0      799 2022-08-18 16:55:06.303743 fabrictestbed-extensions-1.4.3/docs/make.bat
+-rw-r--r--   0        0        0     1996 2023-02-13 18:31:49.552781 fabrictestbed-extensions-1.4.3/docs/source/conf.py
+-rw-r--r--   0        0        0     8869 2022-10-28 15:15:07.136211 fabrictestbed-extensions-1.4.3/docs/source/fablib.rst
+-rw-r--r--   0        0        0     4470 2023-04-06 16:18:57.455278 fabrictestbed-extensions-1.4.3/docs/source/index.rst
+-rw-r--r--   0        0        0      147 2023-04-22 14:13:43.304224 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/__init__.py
+-rw-r--r--   0        0        0        2 2023-02-13 18:31:49.553082 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/editors/__init__.py
+-rw-r--r--   0        0        0    18044 2023-02-13 18:31:49.553270 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/editors/abc_topology_editor.py
+-rw-r--r--   0        0        0     6277 2023-02-13 18:31:49.553528 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
+-rw-r--r--   0        0        0    68479 2023-02-13 18:31:49.553650 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/editors/geo_topology_editor.py
+-rw-r--r--   0        0        0        1 2022-08-18 16:55:06.304986 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/__init__.py
+-rw-r--r--   0        0        0     4793 2023-02-13 18:31:49.553839 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/abc_fablib.py
+-rw-r--r--   0        0        0    21062 2023-04-20 18:01:14.628314 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/component.py
+-rw-r--r--   0        0        0    76799 2023-04-20 18:01:14.628593 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/fablib.py
+-rw-r--r--   0        0        0     5807 2023-02-13 18:31:49.554628 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/facility_port.py
+-rw-r--r--   0        0        0    25967 2023-04-22 14:13:43.304449 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/interface.py
+-rw-r--r--   0        0        0    39140 2023-04-20 18:01:14.628864 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/network_service.py
+-rw-r--r--   0        0        0    95919 2023-04-22 14:13:43.304819 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/node.py
+-rw-r--r--   0        0        0    34672 2023-04-20 18:01:14.629639 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/resources.py
+-rw-r--r--   0        0        0    81904 2023-04-20 18:01:14.629937 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/slice.py
+-rw-r--r--   0        0        0        2 2023-02-13 18:31:49.555813 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/images/__init__.py
+-rw-r--r--   0        0        0   199914 2022-08-18 16:55:06.307676 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/images/fabric_logo.png
+-rw-r--r--   0        0        0     1316 2022-08-18 16:55:06.307757 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/images/server.png
+-rw-r--r--   0        0        0    62250 2022-08-18 16:55:06.307862 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/images/slice_rack.png
+-rw-r--r--   0        0        0        2 2023-02-13 18:31:49.555903 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/__init__.py
+-rw-r--r--   0        0        0    14765 2023-02-13 18:31:49.556039 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/abc_test.py
+-rw-r--r--   0        0        0    34231 2023-02-13 18:31:49.556263 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/component_tests.py
+-rw-r--r--   0        0        0       85 2023-02-13 18:31:49.556325 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/dummy-token.json
+-rw-r--r--   0        0        0    13366 2023-02-13 18:31:49.556445 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
+-rw-r--r--   0        0        0    10227 2023-02-13 18:31:49.556551 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/hello_fabric.py
+-rw-r--r--   0        0        0    20659 2023-02-13 18:31:49.556711 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/link_benchmark.py
+-rw-r--r--   0        0        0    20919 2023-02-13 18:31:49.556814 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/local_network_benchmark.py
+-rw-r--r--   0        0        0    44883 2023-02-13 18:31:49.557045 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/network_benchmark_tests.py
+-rw-r--r--   0        0        0    10052 2023-02-13 18:31:49.557127 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/nvme_benchmark.py
+-rw-r--r--   0        0        0     5095 2023-04-06 16:18:57.459146 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/test_basic.py
+-rw-r--r--   0        0        0        2 2023-02-13 18:31:49.557261 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/utils/__init__.py
+-rw-r--r--   0        0        0     3082 2023-02-13 18:31:49.557349 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/utils/abc_utils.py
+-rw-r--r--   0        0        0     3304 2023-02-13 18:31:49.557428 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/utils/node.py
+-rw-r--r--   0        0        0     8436 2023-02-13 18:31:49.557517 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/utils/slice.py
+-rw-r--r--   0        0        0     1326 2023-04-21 16:27:35.017398 fabrictestbed-extensions-1.4.3/pyproject.toml
+-rwxr-xr-x   0        0        0      122 2022-08-18 16:55:06.309489 fabrictestbed-extensions-1.4.3/sphinx.sh
+-rw-r--r--   0        0        0     5272 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.4.3/PKG-INFO
```

### Comparing `fabrictestbed-extensions-1.4.2rc6/.github/workflows/build.yml` & `fabrictestbed-extensions-1.4.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/.github/workflows/checks.yml` & `fabrictestbed-extensions-1.4.3/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/.github/workflows/test.yml` & `fabrictestbed-extensions-1.4.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/.gitignore` & `fabrictestbed-extensions-1.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/.readthedocs.yaml` & `fabrictestbed-extensions-1.4.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/CHANGELOG.md` & `fabrictestbed-extensions-1.4.3/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,22 @@
 
 This is the changelog file for FABRIC testbed extensions.  All notable
 changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [Unreleased]
+
+## [1.4.3] - 2023-04-22
+
+### Fixed
+
+- The interface.get_ip_addr() fuction now returns address strings for devs that were manually configured. 
+
+## [1.4.2] - 2023-04-21
 
 ### Added
 
 - Support new GPU models has been added (PR
   [#122](https://github.com/fabric-testbed/fabrictestbed-extensions/pull/122)).
 - Support for maintenance mode (PR
   [#137](https://github.com/fabric-testbed/fabrictestbed-extensions/pull/137/),
@@ -23,14 +30,16 @@
   uploaded post-boot, and commands can be submitted to be run
   post-boot.
 - A way to define layer-2 networks.
 - A way to query link and facility port information
 - Added function to make IP address of node publicly routable with external networking. `make_ip_publicly_routable`
 - Streamlined polling after a submit to reduce load on the control framework
 - Added easy, one-line "add_fabnet" functionality simple L3 networks
+- ipython 8.12.0 is added as a direct dependency; this is a short-term
+  workaround until FABRIC's JupyterHub is updated.
 
 ### Changed
 
 - Fablib now uses pyproject.toml for specifying packaging metadata
   instead of setup.py and friends (issue
   [#74](https://github.com/fabric-testbed/fabrictestbed-extensions/issues/74)).
 - Make configure_nvme() more generic (PR
```

### Comparing `fabrictestbed-extensions-1.4.2rc6/LICENSE` & `fabrictestbed-extensions-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/README.md` & `fabrictestbed-extensions-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/docs/Makefile` & `fabrictestbed-extensions-1.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/docs/make.bat` & `fabrictestbed-extensions-1.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/docs/source/conf.py` & `fabrictestbed-extensions-1.4.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/docs/source/fablib.rst` & `fabrictestbed-extensions-1.4.3/docs/source/fablib.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/docs/source/index.rst` & `fabrictestbed-extensions-1.4.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/editors/abc_topology_editor.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/editors/abc_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/editors/cytoscape_topology_editor.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/editors/cytoscape_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/editors/geo_topology_editor.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/editors/geo_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/abc_fablib.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/abc_fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/component.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/component.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/fablib.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/facility_port.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/facility_port.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/interface.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -684,15 +684,15 @@
             logging.error(
                 f"Failed to get ip addr show info for interface {self.get_name()}"
             )
 
         return stdout
 
     # fablib.Interface.get_ip_addr()
-    def get_ip_addr(self, dev=None):
+    def get_ip_addr_ssh(self, dev=None):
         """
         Gets the ip addr info for this interface.
 
         :return ip addr info
         :rtype: str
         """
         try:
@@ -704,15 +704,16 @@
             # print(f"dev: {dev}")
 
             if dev == None:
                 return addrs
 
             for addr in addrs:
                 if addr["ifname"] == dev:
-                    return ipaddress.ip_address(addr["addr_info"][0]["local"])
+                    # Hack to make it backward compatible. Should return an object
+                    return str(ipaddress.ip_address(addr["addr_info"][0]["local"]))
 
             return None
         except Exception as e:
             print(f"Exception: {e}")
 
     # fablib.Interface.get_ip_addr()
     def get_ips(self, family=None):
@@ -795,15 +796,16 @@
         if "addr" in fablib_data:
             try:
                 addr = ipaddress.ip_address(fablib_data["addr"])
             except:
                 addr = fablib_data["addr"]
             return addr
         else:
-            return None
+            # get_ip_addr_ssh()
+            return self.get_ip_addr_ssh()
 
     def set_mode(self, mode: str = "config"):
         fablib_data = self.get_fablib_data()
         fablib_data["mode"] = mode
         self.set_fablib_data(fablib_data)
 
         return self
```

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/network_service.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/network_service.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/node.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -2658,15 +2658,15 @@
 
     def set_run_update_commands(self, run_update_commands: bool = True):
         fablib_data = self.get_fablib_data()
         fablib_data["run_update_commands"] = str(run_update_commands)
         self.set_fablib_data(fablib_data)
 
     def config(self, log_dir="."):
-        self.execute(f"sudo hostnamectl set-hostname {self.get_name()}", quiet=True)
+        self.execute(f"sudo hostnamectl set-hostname '{self.get_name()}'", quiet=True)
 
         for iface in self.get_interfaces():
             iface.config()
         self.config_routes()
 
         if not self.is_instantiated():
             self.set_instantiated(True)
```

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/resources.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/resources.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/slice.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/images/fabric_logo.png` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/images/fabric_logo.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/images/server.png` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/images/server.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/images/slice_rack.png` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/images/slice_rack.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/abc_test.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/abc_test.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/component_tests.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/component_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/hello_fabric.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/hello_fabric.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/link_benchmark.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/link_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/local_network_benchmark.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/local_network_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/network_benchmark_tests.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/network_benchmark_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/nvme_benchmark.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/nvme_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/test_basic.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/utils/abc_utils.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/utils/abc_utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/utils/node.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/utils/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/utils/slice.py` & `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/utils/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc6/pyproject.toml` & `fabrictestbed-extensions-1.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "ipycytoscape",
     "tabulate",
     "fabrictestbed==1.4.4",
     "paramiko",
     "jinja2>=3.0.0",
     "pandas",
     "numpy",
-    "ipython"
+    "ipython==8.12.0"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `fabrictestbed-extensions-1.4.2rc6/PKG-INFO` & `fabrictestbed-extensions-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-extensions
-Version: 1.4.2rc6
+Version: 1.4.3
 Summary: FABRIC Python Client Library and CLI Extensions
 Author-email: Paul Ruth <pruth@renci.org>, Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: ipycytoscape
 Requires-Dist: tabulate
 Requires-Dist: fabrictestbed==1.4.4
 Requires-Dist: paramiko
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: pandas
 Requires-Dist: numpy
-Requires-Dist: ipython
+Requires-Dist: ipython==8.12.0
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: furo ; extra == "doc"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: coverage[toml] ; extra == "test"
 Project-URL: ChangeLog, https://github.com/fabric-testbed/fabrictestbed-extensions/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://fabric-fablib.readthedocs.io/
 Project-URL: Homepage, https://fabric-testbed.net/
```

