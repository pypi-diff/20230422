# Comparing `tmp/maddaq-0.7.3.tar.gz` & `tmp/maddaq-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maddaq-0.7.3.tar", last modified: Fri Apr 14 16:23:32 2023, max compression
+gzip compressed data, was "maddaq-0.7.4.tar", last modified: Sat Apr 22 09:47:25 2023, max compression
```

## Comparing `maddaq-0.7.3.tar` & `maddaq-0.7.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-14 16:23:32.489770 maddaq-0.7.3/
--rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-14 16:23:32.489497 maddaq-0.7.3/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)     4553 2023-04-13 15:28:31.000000 maddaq-0.7.3/README.md
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-14 16:23:32.483177 maddaq-0.7.3/maddaq/
--rw-r--r--   0 lacasta    (503) staff       (20)      998 2019-09-19 07:26:57.000000 maddaq-0.7.3/maddaq/GTimer.py
--rw-r--r--   0 lacasta    (503) staff       (20)     7547 2022-10-13 08:37:37.000000 maddaq-0.7.3/maddaq/MadDAQData.py
--rw-r--r--   0 lacasta    (503) staff       (20)    14238 2023-04-14 16:21:00.000000 maddaq-0.7.3/maddaq/MadDAQModule.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2336 2022-01-12 19:26:43.000000 maddaq-0.7.3/maddaq/Progress.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4037 2022-10-01 17:07:05.000000 maddaq-0.7.3/maddaq/ScanManager.py
--rw-r--r--   0 lacasta    (503) staff       (20)      485 2023-04-14 16:15:11.000000 maddaq-0.7.3/maddaq/__init__.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-14 16:23:32.488980 maddaq-0.7.3/maddaq/cmmds/
--rw-r--r--   0 lacasta    (503) staff       (20)        0 2023-04-13 16:51:33.000000 maddaq-0.7.3/maddaq/cmmds/__init__.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     5865 2023-04-13 19:53:59.000000 maddaq-0.7.3/maddaq/cmmds/analyze_data.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)      586 2023-04-13 16:17:24.000000 maddaq-0.7.3/maddaq/cmmds/file_info.py
--rw-r--r--   0 lacasta    (503) staff       (20)     8197 2022-10-01 17:15:09.000000 maddaq-0.7.3/maddaq/cmmds/fit_utils.py
--rw-r--r--   0 lacasta    (503) staff       (20)     5783 2023-04-13 16:47:46.000000 maddaq-0.7.3/maddaq/cmmds/getSpectrum.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     1887 2023-04-13 16:16:23.000000 maddaq-0.7.3/maddaq/cmmds/read_data.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     6111 2023-04-13 16:13:35.000000 maddaq-0.7.3/maddaq/cmmds/show_data.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-14 16:23:32.485847 maddaq-0.7.3/maddaq.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-14 16:23:32.000000 maddaq-0.7.3/maddaq.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      513 2023-04-14 16:23:32.000000 maddaq-0.7.3/maddaq.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-04-14 16:23:32.000000 maddaq-0.7.3/maddaq.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      144 2023-04-14 16:23:32.000000 maddaq-0.7.3/maddaq.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       71 2023-04-14 16:23:32.000000 maddaq-0.7.3/maddaq.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        7 2023-04-14 16:23:32.000000 maddaq-0.7.3/maddaq.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      810 2023-04-14 16:15:11.000000 maddaq-0.7.3/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-04-14 16:23:32.489847 maddaq-0.7.3/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-22 09:47:25.716365 maddaq-0.7.4/
+-rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-22 09:47:25.716060 maddaq-0.7.4/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)     4553 2023-04-13 15:28:31.000000 maddaq-0.7.4/README.md
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-22 09:47:25.709880 maddaq-0.7.4/maddaq/
+-rw-r--r--   0 lacasta    (503) staff       (20)      998 2019-09-19 07:26:57.000000 maddaq-0.7.4/maddaq/GTimer.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     7547 2022-10-13 08:37:37.000000 maddaq-0.7.4/maddaq/MadDAQData.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    14238 2023-04-14 16:21:00.000000 maddaq-0.7.4/maddaq/MadDAQModule.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2336 2022-01-12 19:26:43.000000 maddaq-0.7.4/maddaq/Progress.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4037 2022-10-01 17:07:05.000000 maddaq-0.7.4/maddaq/ScanManager.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      485 2023-04-22 09:45:49.000000 maddaq-0.7.4/maddaq/__init__.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-22 09:47:25.715549 maddaq-0.7.4/maddaq/cmmds/
+-rw-r--r--   0 lacasta    (503) staff       (20)        0 2023-04-13 16:51:33.000000 maddaq-0.7.4/maddaq/cmmds/__init__.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     5865 2023-04-13 19:53:59.000000 maddaq-0.7.4/maddaq/cmmds/analyze_data.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)      586 2023-04-13 16:17:24.000000 maddaq-0.7.4/maddaq/cmmds/file_info.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     8197 2022-10-01 17:15:09.000000 maddaq-0.7.4/maddaq/cmmds/fit_utils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     5783 2023-04-22 09:37:21.000000 maddaq-0.7.4/maddaq/cmmds/getSpectrum.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     1887 2023-04-13 16:16:23.000000 maddaq-0.7.4/maddaq/cmmds/read_data.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     6111 2023-04-13 16:13:35.000000 maddaq-0.7.4/maddaq/cmmds/show_data.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-22 09:47:25.712659 maddaq-0.7.4/maddaq.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-22 09:47:25.000000 maddaq-0.7.4/maddaq.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      513 2023-04-22 09:47:25.000000 maddaq-0.7.4/maddaq.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-04-22 09:47:25.000000 maddaq-0.7.4/maddaq.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      144 2023-04-22 09:47:25.000000 maddaq-0.7.4/maddaq.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       71 2023-04-22 09:47:25.000000 maddaq-0.7.4/maddaq.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        7 2023-04-22 09:47:25.000000 maddaq-0.7.4/maddaq.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      810 2023-04-22 09:45:49.000000 maddaq-0.7.4/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-04-22 09:47:25.716508 maddaq-0.7.4/setup.cfg
```

### Comparing `maddaq-0.7.3/PKG-INFO` & `maddaq-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maddaq
-Version: 0.7.3
+Version: 0.7.4
 Summary: A collection of python scripts to access maddaq data.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `maddaq-0.7.3/README.md` & `maddaq-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.3/maddaq/GTimer.py` & `maddaq-0.7.4/maddaq/GTimer.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.3/maddaq/MadDAQData.py` & `maddaq-0.7.4/maddaq/MadDAQData.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.3/maddaq/MadDAQModule.py` & `maddaq-0.7.4/maddaq/MadDAQModule.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.3/maddaq/Progress.py` & `maddaq-0.7.4/maddaq/Progress.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.3/maddaq/ScanManager.py` & `maddaq-0.7.4/maddaq/ScanManager.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.3/maddaq/cmmds/analyze_data.py` & `maddaq-0.7.4/maddaq/cmmds/analyze_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.3/maddaq/cmmds/file_info.py` & `maddaq-0.7.4/maddaq/cmmds/file_info.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.3/maddaq/cmmds/fit_utils.py` & `maddaq-0.7.4/maddaq/cmmds/fit_utils.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.3/maddaq/cmmds/getSpectrum.py` & `maddaq-0.7.4/maddaq/cmmds/getSpectrum.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
     parser.add_argument("--start-time", dest="start_time", default=None, type=float,
                         help="Event time to start")
     parser.add_argument("--start-evt", dest="start_evt", default=None,
                         action=CommaSeparatedListAction,
                         help="Event number to start showing")
     parser.add_argument("--scan-point", dest="scan_point", type=int, default=None,
                         help="Scan point number to visit")
-    parser.add_argument("--nbin", default=-1, help="Number of bins in histogram.")
+    parser.add_argument("--nbin", default=50, help="Number of bins in histogram.")
     parser.add_argument("--logY", default=False, action="store_true", help="Log axis")
     parser.add_argument("--thrs", default=0.0, type=float, help="Min E to show in histogram")
     parser.add_argument("--two_peaks", default=False, action="store_true", help="Min E to show in histogram")
     parser.add_argument("--no-fit", dest="fit", default=True, action="store_false")
     parser.add_argument("--mid", dest="mid", default=-1,
                         type=int, help="The module ID")
```

### Comparing `maddaq-0.7.3/maddaq/cmmds/read_data.py` & `maddaq-0.7.4/maddaq/cmmds/read_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.3/maddaq/cmmds/show_data.py` & `maddaq-0.7.4/maddaq/cmmds/show_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.3/maddaq.egg-info/PKG-INFO` & `maddaq-0.7.4/maddaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maddaq
-Version: 0.7.3
+Version: 0.7.4
 Summary: A collection of python scripts to access maddaq data.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `maddaq-0.7.3/maddaq.egg-info/SOURCES.txt` & `maddaq-0.7.4/maddaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.3/pyproject.toml` & `maddaq-0.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maddaq"
-version = "0.7.3"
+version = "0.7.4"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@alibavasystems.com" },
 ]
 description = "A collection of python scripts to access maddaq data."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

