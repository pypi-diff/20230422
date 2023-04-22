# Comparing `tmp/eds-utils-0.3.0.tar.gz` & `tmp/eds-utils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eds-utils-0.3.0.tar", last modified: Sun Apr 16 16:33:08 2023, max compression
+gzip compressed data, was "eds-utils-0.3.1.tar", last modified: Sat Apr 22 17:26:31 2023, max compression
```

## Comparing `eds-utils-0.3.0.tar` & `eds-utils-0.3.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.263846 eds-utils-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 16:32:56.000000 eds-utils-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-16 16:33:08.263846 eds-utils-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-16 16:32:56.000000 eds-utils-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.259847 eds-utils-0.3.0/eds_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.259847 eds-utils-0.3.0/eds_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12779 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/eds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.259847 eds-utils-0.3.0/eds_utils/core/file_io/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/file_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/file_io/read_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/file_io/write_canopennode.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/file_io/write_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/file_io/write_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/file_io/write_rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/core/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds2dcf.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds2md.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds2rst.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_autofix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.259847 eds-utils-0.3.0/eds_utils/eds_editor/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.259847 eds-utils-0.3.0/eds_utils/eds_editor/dialogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/dialogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/dialogs/add_object_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/dialogs/copy_object_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/dialogs/errors_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/dialogs/open_tmp_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/eds_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.263846 eds-utils-0.3.0/eds_utils/eds_editor/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12753 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/pages/_object_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/pages/device_commissioning_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/pages/general_info_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/pages/object_dictionary_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/pages/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/pages/pdo_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_editor/window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-16 16:32:56.000000 eds-utils-0.3.0/eds_utils/eds_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.259847 eds-utils-0.3.0/eds_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-16 16:33:08.000000 eds-utils-0.3.0/eds_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-16 16:33:08.000000 eds-utils-0.3.0/eds_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:33:08.000000 eds-utils-0.3.0/eds_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-16 16:33:08.000000 eds-utils-0.3.0/eds_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 16:33:08.000000 eds-utils-0.3.0/eds_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 16:33:08.000000 eds-utils-0.3.0/eds_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 16:32:56.000000 eds-utils-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-16 16:33:08.263846 eds-utils-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:33:08.263846 eds-utils-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:32:56.000000 eds-utils-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-16 16:32:56.000000 eds-utils-0.3.0/tests/test_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-16 16:32:56.000000 eds-utils-0.3.0/tests/test_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:31.278891 eds-utils-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-22 17:26:18.000000 eds-utils-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-22 17:26:31.278891 eds-utils-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-22 17:26:18.000000 eds-utils-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:31.274891 eds-utils-0.3.1/eds_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:31.274891 eds-utils-0.3.1/eds_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/core/eds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:31.274891 eds-utils-0.3.1/eds_utils/core/file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/core/file_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/core/file_io/read_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/core/file_io/write_canopennode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/core/file_io/write_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/core/file_io/write_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/core/file_io/write_rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/core/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds2dcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds2md.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds2rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_autofix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:31.274891 eds-utils-0.3.1/eds_utils/eds_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:31.274891 eds-utils-0.3.1/eds_utils/eds_editor/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/dialogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/dialogs/add_object_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/dialogs/copy_object_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/dialogs/errors_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/dialogs/open_tmp_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/eds_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:31.278891 eds-utils-0.3.1/eds_utils/eds_editor/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12753 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/pages/_object_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/pages/device_commissioning_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/pages/general_info_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/pages/object_dictionary_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/pages/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/pages/pdo_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_editor/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-22 17:26:18.000000 eds-utils-0.3.1/eds_utils/eds_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:31.274891 eds-utils-0.3.1/eds_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-22 17:26:31.000000 eds-utils-0.3.1/eds_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-22 17:26:31.000000 eds-utils-0.3.1/eds_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:26:31.000000 eds-utils-0.3.1/eds_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-22 17:26:31.000000 eds-utils-0.3.1/eds_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 17:26:31.000000 eds-utils-0.3.1/eds_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 17:26:31.000000 eds-utils-0.3.1/eds_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-22 17:26:18.000000 eds-utils-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-22 17:26:31.278891 eds-utils-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:31.278891 eds-utils-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 eds-utils-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-22 17:26:18.000000 eds-utils-0.3.1/tests/test_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-22 17:26:18.000000 eds-utils-0.3.1/tests/test_objects.py
```

### Comparing `eds-utils-0.3.0/LICENSE` & `eds-utils-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/PKG-INFO` & `eds-utils-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eds-utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: Utilities for editing CANopen EDS/DCF files
 Home-page: https://github.com/oresat/eds-utils
 Author: psas
 Author-email: oresat@pdx.edu
 Maintainer: psas
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `eds-utils-0.3.0/README.rst` & `eds-utils-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/__main__.py` & `eds-utils-0.3.1/eds_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/core/__init__.py` & `eds-utils-0.3.1/eds_utils/core/__init__.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/core/eds.py` & `eds-utils-0.3.1/eds_utils/core/eds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
 from dataclasses import dataclass, field
 from typing import Dict, List
+from copy import deepcopy
 
 from . import DataType
 from .objects import Variable, Record
 
 
 class EDSError(Exception):
     '''Error with EDS'''
@@ -297,15 +298,15 @@
 
         return count
 
     @property
     def indexes(self) -> List[int]:
         '''The list of indexes in the OD'''
 
-        return sorted(self._data.keys())
+        return list(self._data.keys())
 
     @property
     def mandatory_objects(self) -> List[int]:
         '''The list of mandatory objects indexes in the OD'''
 
         objects = []
 
@@ -371,16 +372,16 @@
 
         if not isinstance(self._data[index], Variable) and new_subindex is not None:
             raise EDSError('cannot move a non-Variable to a subindex')
 
         obj = self._data[index] if subindex is None else self._data[index][subindex]
 
         if new_subindex is None:
-            self._data[new_index] = obj
+            self._data[new_index] = deepcopy(obj)
         else:
-            self._data[new_index][new_subindex] = obj
+            self._data[new_index][new_subindex] = deepcopy(obj)
 
         if move:
             if subindex is None:
                 del self._data[index]
             else:
                 del self._data[index][subindex]
```

### Comparing `eds-utils-0.3.0/eds_utils/core/file_io/read_eds.py` & `eds-utils-0.3.1/eds_utils/core/file_io/read_eds.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/core/file_io/write_canopennode.py` & `eds-utils-0.3.1/eds_utils/core/file_io/write_canopennode.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/core/file_io/write_eds.py` & `eds-utils-0.3.1/eds_utils/core/file_io/write_eds.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/core/file_io/write_md.py` & `eds-utils-0.3.1/eds_utils/core/file_io/write_md.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/core/file_io/write_rst.py` & `eds-utils-0.3.1/eds_utils/core/file_io/write_rst.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/core/objects.py` & `eds-utils-0.3.1/eds_utils/core/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 '''All the object class for the object dictionary'''
 
 from dataclasses import dataclass
+from typing import List
 
 from . import DataType, AccessType, ObjectType
 
 
 @dataclass
 class Variable:
     '''Holds EDS variable data'''
@@ -105,18 +106,18 @@
 
         del self._data[subindex]
 
         # update record size subindex
         self._data[0].default_value = f'0x{len(self._data) - 1:02X}'
 
     @property
-    def subindexes(self) -> list:
+    def subindexes(self) -> List[int]:
         '''Get the list of subindexes'''
 
-        return self._data.keys()
+        return list(self._data.keys())
 
     @property
     def storage_location(self) -> str:
         '''The storage location of object'''
 
         return self._storage_location
```

### Comparing `eds-utils-0.3.0/eds_utils/eds2c.py` & `eds-utils-0.3.1/eds_utils/eds2c.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds2dcf.py` & `eds-utils-0.3.1/eds_utils/eds2dcf.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds2md.py` & `eds-utils-0.3.1/eds_utils/eds2md.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds2rst.py` & `eds-utils-0.3.1/eds_utils/eds2rst.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_autofix.py` & `eds-utils-0.3.1/eds_utils/eds_autofix.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_editor/app.py` & `eds-utils-0.3.1/eds_utils/eds_editor/app.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py` & `eds-utils-0.3.1/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_editor/dialogs/add_object_dialog.py` & `eds-utils-0.3.1/eds_utils/eds_editor/dialogs/add_object_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_editor/dialogs/copy_object_dialog.py` & `eds-utils-0.3.1/eds_utils/eds_editor/dialogs/copy_object_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_editor/dialogs/errors_dialog.py` & `eds-utils-0.3.1/eds_utils/eds_editor/dialogs/errors_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_editor/dialogs/open_tmp_dialog.py` & `eds-utils-0.3.1/eds_utils/eds_editor/dialogs/open_tmp_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_editor/eds_notebook.py` & `eds-utils-0.3.1/eds_utils/eds_editor/eds_notebook.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_editor/main.py` & `eds-utils-0.3.1/eds_utils/eds_editor/main.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_editor/pages/_object_grid.py` & `eds-utils-0.3.1/eds_utils/eds_editor/pages/_object_grid.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_editor/pages/device_commissioning_page.py` & `eds-utils-0.3.1/eds_utils/eds_editor/pages/device_commissioning_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_editor/pages/general_info_page.py` & `eds-utils-0.3.1/eds_utils/eds_editor/pages/general_info_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_editor/pages/object_dictionary_page.py` & `eds-utils-0.3.1/eds_utils/eds_editor/pages/object_dictionary_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_editor/pages/pdo_page.py` & `eds-utils-0.3.1/eds_utils/eds_editor/pages/pdo_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_editor/window.py` & `eds-utils-0.3.1/eds_utils/eds_editor/window.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils/eds_merge.py` & `eds-utils-0.3.1/eds_utils/eds_merge.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,22 +35,28 @@
     for index in eds1.indexes:
         if (args.rpdo and index >= eds1.RPDO_COMM_START and index <= eds1.RPDO_COMM_END) or \
                 (args.tpdo and index >= eds1.TPDO_COMM_START and index <= eds1.TPDO_COMM_END):
             continue
 
         index_obj = eds1[index]
 
-        if strategy == 'override' or index not in eds2.indexes:
+        if strategy == 'override' and index in eds2.indexes:
+            del eds2[index]
+        if index not in eds2.indexes:
             print(f'0x{index:04X}')
             eds2[index] = eds1[index]
+        if strategy == 'override':
+            continue  # no need to subindex after doing the full index
 
         if index_obj.object_type != ObjectType.VAR:
             for subindex in index_obj.subindexes:
-                if strategy == 'override' or subindex not in eds2[index].subindexes:
-                    print(f'0x{index:04X} sub 0x{index:02X}')
+                if subindex == 0:
+                    continue
+                if subindex not in eds2[index].subindexes:
+                    print(f'0x{index:04X} sub 0x{subindex:02X}')
                     eds2[index][subindex] = eds1[index][subindex]
 
     # when merging an EDS into a DCF, update the LastEDS field
     if args.filepath1.endswith('.eds') and args.filepath2.endswith('.dcf'):
         eds2.file_info.last_eds = eds1.file_info.file_name
 
     write_eds(eds2)
```

### Comparing `eds-utils-0.3.0/eds_utils/eds_validate.py` & `eds-utils-0.3.1/eds_utils/eds_validate.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/eds_utils.egg-info/PKG-INFO` & `eds-utils-0.3.1/eds_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eds-utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: Utilities for editing CANopen EDS/DCF files
 Home-page: https://github.com/oresat/eds-utils
 Author: psas
 Author-email: oresat@pdx.edu
 Maintainer: psas
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `eds-utils-0.3.0/eds_utils.egg-info/SOURCES.txt` & `eds-utils-0.3.1/eds_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/setup.cfg` & `eds-utils-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/tests/test_eds.py` & `eds-utils-0.3.1/tests/test_eds.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.3.0/tests/test_objects.py` & `eds-utils-0.3.1/tests/test_objects.py`

 * *Files identical despite different names*

