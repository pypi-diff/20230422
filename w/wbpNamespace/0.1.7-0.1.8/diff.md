# Comparing `tmp/wbpNamespace-0.1.7.tar.gz` & `tmp/wbpNamespace-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpNamespace-0.1.7.tar", last modified: Fri Mar 31 15:53:49 2023, max compression
+gzip compressed data, was "wbpNamespace-0.1.8.tar", last modified: Sat Apr 22 15:36:46 2023, max compression
```

## Comparing `wbpNamespace-0.1.7.tar` & `wbpNamespace-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:53:49.713340 wbpNamespace-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-03-31 15:53:47.000000 wbpNamespace-0.1.7/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:53:49.708340 wbpNamespace-0.1.7/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:53:49.711340 wbpNamespace-0.1.7/Lib/wbpNamespace/
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-03-31 15:53:47.000000 wbpNamespace-0.1.7/Lib/wbpNamespace/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2024 2023-03-31 15:53:47.000000 wbpNamespace-0.1.7/Lib/wbpNamespace/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-03-31 15:53:47.000000 wbpNamespace-0.1.7/Lib/wbpNamespace/control.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 15:53:49.713340 wbpNamespace-0.1.7/Lib/wbpNamespace.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1623 2023-03-31 15:53:49.000000 wbpNamespace-0.1.7/Lib/wbpNamespace.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      362 2023-03-31 15:53:49.000000 wbpNamespace-0.1.7/Lib/wbpNamespace.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 15:53:49.000000 wbpNamespace-0.1.7/Lib/wbpNamespace.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-03-31 15:53:49.000000 wbpNamespace-0.1.7/Lib/wbpNamespace.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-03-31 15:53:49.000000 wbpNamespace-0.1.7/Lib/wbpNamespace.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-31 15:53:49.000000 wbpNamespace-0.1.7/Lib/wbpNamespace.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1623 2023-03-31 15:53:49.713340 wbpNamespace-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-03-31 15:53:47.000000 wbpNamespace-0.1.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1969 2023-03-31 15:53:49.714341 wbpNamespace-0.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-03-31 15:53:47.000000 wbpNamespace-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:36:46.354631 wbpNamespace-0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-04-22 15:36:44.000000 wbpNamespace-0.1.8/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:36:46.350964 wbpNamespace-0.1.8/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:36:46.352798 wbpNamespace-0.1.8/Lib/wbpNamespace/
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-22 15:36:44.000000 wbpNamespace-0.1.8/Lib/wbpNamespace/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2057 2023-04-22 15:36:44.000000 wbpNamespace-0.1.8/Lib/wbpNamespace/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2023-04-22 15:36:44.000000 wbpNamespace-0.1.8/Lib/wbpNamespace/control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:36:46.354631 wbpNamespace-0.1.8/Lib/wbpNamespace.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-04-22 15:36:46.000000 wbpNamespace-0.1.8/Lib/wbpNamespace.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      362 2023-04-22 15:36:46.000000 wbpNamespace-0.1.8/Lib/wbpNamespace.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 15:36:46.000000 wbpNamespace-0.1.8/Lib/wbpNamespace.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-22 15:36:46.000000 wbpNamespace-0.1.8/Lib/wbpNamespace.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-22 15:36:46.000000 wbpNamespace-0.1.8/Lib/wbpNamespace.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-22 15:36:46.000000 wbpNamespace-0.1.8/Lib/wbpNamespace.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-04-22 15:36:46.354631 wbpNamespace-0.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-04-22 15:36:44.000000 wbpNamespace-0.1.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1975 2023-04-22 15:36:46.355548 wbpNamespace-0.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-22 15:36:44.000000 wbpNamespace-0.1.8/setup.py
```

### Comparing `wbpNamespace-0.1.7/LICENSE` & `wbpNamespace-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpNamespace-0.1.7/Lib/wbpNamespace.egg-info/PKG-INFO` & `wbpNamespace-0.1.8/Lib/wbpNamespace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpNamespace
-Version: 0.1.7
+Version: 0.1.8
 Summary: Namespace panel for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpnamespace
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpnamespace
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpnamespace/
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpnamespace/-/issues
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.8
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpNamespace
 
 Namespace plugin for Workbench applications
```

### Comparing `wbpNamespace-0.1.7/PKG-INFO` & `wbpNamespace-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpNamespace
-Version: 0.1.7
+Version: 0.1.8
 Summary: Namespace panel for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpnamespace
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpnamespace
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpnamespace/
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpnamespace/-/issues
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.8
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpNamespace
 
 Namespace plugin for Workbench applications
```

### Comparing `wbpNamespace-0.1.7/setup.cfg` & `wbpNamespace-0.1.8/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.7
+current_version = 0.1.8
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -47,17 +47,17 @@
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development :: User Interfaces
 
 [options]
 package_dir = 
 	=Lib
 packages = find:
-python_requires = >=3.8
+python_requires = >=3.8,<3.11
 install_requires = 
-	wbBase>=0.1.49
+	wbBase>=0.1.54
 
 [options.packages.find]
 where = Lib
 
 [options.entry_points]
 wbbase.plugin = namespace = wbpNamespace
```

