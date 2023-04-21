# Comparing `tmp/pywhiten-1.1.0.tar.gz` & `tmp/pywhiten-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywhiten-1.1.0.tar", last modified: Fri Apr 21 23:14:02 2023, max compression
+gzip compressed data, was "pywhiten-1.1.1.tar", last modified: Fri Apr 21 23:32:47 2023, max compression
```

## Comparing `pywhiten-1.1.0.tar` & `pywhiten-1.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.592459 pywhiten-1.1.0/
--rw-r--r--   0 erik      (1000) erik      (1000)     1068 2023-02-06 23:54:19.000000 pywhiten-1.1.0/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)    13435 2023-04-21 23:14:02.592459 pywhiten-1.1.0/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)    12705 2023-04-21 23:00:01.000000 pywhiten-1.1.0/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)      803 2023-04-21 22:49:21.000000 pywhiten-1.1.0/pyproject.toml
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.589126 pywhiten-1.1.0/pywhiten/
--rw-r--r--   0 erik      (1000) erik      (1000)    11869 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/PyWhitener.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1579 2023-04-21 22:44:08.000000 pywhiten-1.1.0/pywhiten/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.589126 pywhiten-1.1.0/pywhiten/cfg/
--rw-r--r--   0 erik      (1000) erik      (1000)       83 2023-04-21 22:45:16.000000 pywhiten-1.1.0/pywhiten/cfg/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)      617 2023-04-21 22:45:49.000000 pywhiten-1.1.0/pywhiten/cfg/cfgutils.py
--rw-r--r--   0 erik      (1000) erik      (1000)     6437 2023-03-20 18:59:49.000000 pywhiten-1.1.0/pywhiten/cfg/default.toml
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.592459 pywhiten-1.1.0/pywhiten/data/
--rw-r--r--   0 erik      (1000) erik      (1000)     3792 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/data/Frequency.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4510 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/data/FrequencyContainer.py
--rw-r--r--   0 erik      (1000) erik      (1000)       58 2023-02-14 19:27:58.000000 pywhiten-1.1.0/pywhiten/data/InvalidConstructorArgumentsError.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2983 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/data/Lightcurve.py
--rw-r--r--   0 erik      (1000) erik      (1000)    17451 2023-04-21 22:43:40.000000 pywhiten-1.1.0/pywhiten/data/Periodogram.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1402 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/data/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.592459 pywhiten-1.1.0/pywhiten/optimization/
--rw-r--r--   0 erik      (1000) erik      (1000)     9084 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/optimization/Optimizer.py
--rw-r--r--   0 erik      (1000) erik      (1000)      781 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/optimization/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1942 2023-03-09 22:20:31.000000 pywhiten-1.1.0/pywhiten/optimization/models.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.592459 pywhiten-1.1.0/pywhiten/pwio/
--rw-r--r--   0 erik      (1000) erik      (1000)    14076 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/pwio/OutputManager.py
--rw-r--r--   0 erik      (1000) erik      (1000)      596 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/pwio/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1334 2023-03-09 20:17:13.000000 pywhiten-1.1.0/pywhiten/pwio/utilities.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.589126 pywhiten-1.1.0/pywhiten.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)    13435 2023-04-21 23:14:02.000000 pywhiten-1.1.0/pywhiten.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      891 2023-04-21 23:14:02.000000 pywhiten-1.1.0/pywhiten.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-04-21 23:14:02.000000 pywhiten-1.1.0/pywhiten.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-04-21 22:59:24.000000 pywhiten-1.1.0/pywhiten.egg-info/not-zip-safe
--rw-r--r--   0 erik      (1000) erik      (1000)       43 2023-04-21 23:14:02.000000 pywhiten-1.1.0/pywhiten.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        9 2023-04-21 23:14:02.000000 pywhiten-1.1.0/pywhiten.egg-info/top_level.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       38 2023-04-21 23:14:02.592459 pywhiten-1.1.0/setup.cfg
--rw-r--r--   0 erik      (1000) erik      (1000)      709 2023-04-21 23:13:52.000000 pywhiten-1.1.0/setup.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.592459 pywhiten-1.1.0/tests/
--rw-r--r--   0 erik      (1000) erik      (1000)      988 2023-04-21 22:38:42.000000 pywhiten-1.1.0/tests/test_Frequency.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2200 2023-04-21 22:38:42.000000 pywhiten-1.1.0/tests/test_FrequencyContainer.py
--rw-r--r--   0 erik      (1000) erik      (1000)      236 2023-04-21 22:38:42.000000 pywhiten-1.1.0/tests/test_Lightcurve.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1828 2023-04-21 22:38:42.000000 pywhiten-1.1.0/tests/test_Optimizer.py
--rw-r--r--   0 erik      (1000) erik      (1000)      444 2023-04-21 22:38:42.000000 pywhiten-1.1.0/tests/test_OutputManager.py
--rw-r--r--   0 erik      (1000) erik      (1000)      156 2023-04-21 22:48:00.000000 pywhiten-1.1.0/tests/test_copyconfig.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:32:47.792461 pywhiten-1.1.1/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1068 2023-02-06 23:54:19.000000 pywhiten-1.1.1/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)    13517 2023-04-21 23:32:47.792461 pywhiten-1.1.1/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)    12787 2023-04-21 23:29:22.000000 pywhiten-1.1.1/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)      803 2023-04-21 23:28:03.000000 pywhiten-1.1.1/pyproject.toml
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:32:47.789127 pywhiten-1.1.1/pywhiten/
+-rw-r--r--   0 erik      (1000) erik      (1000)    11869 2023-04-21 22:38:42.000000 pywhiten-1.1.1/pywhiten/PyWhitener.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1579 2023-04-21 22:44:08.000000 pywhiten-1.1.1/pywhiten/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:32:47.792461 pywhiten-1.1.1/pywhiten/cfg/
+-rw-r--r--   0 erik      (1000) erik      (1000)       83 2023-04-21 22:45:16.000000 pywhiten-1.1.1/pywhiten/cfg/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      617 2023-04-21 22:45:49.000000 pywhiten-1.1.1/pywhiten/cfg/cfgutils.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     6437 2023-03-20 18:59:49.000000 pywhiten-1.1.1/pywhiten/cfg/default.toml
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:32:47.792461 pywhiten-1.1.1/pywhiten/data/
+-rw-r--r--   0 erik      (1000) erik      (1000)     3794 2023-04-21 23:15:49.000000 pywhiten-1.1.1/pywhiten/data/Frequency.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4510 2023-04-21 22:38:42.000000 pywhiten-1.1.1/pywhiten/data/FrequencyContainer.py
+-rw-r--r--   0 erik      (1000) erik      (1000)       58 2023-02-14 19:27:58.000000 pywhiten-1.1.1/pywhiten/data/InvalidConstructorArgumentsError.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2983 2023-04-21 22:38:42.000000 pywhiten-1.1.1/pywhiten/data/Lightcurve.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    17451 2023-04-21 22:43:40.000000 pywhiten-1.1.1/pywhiten/data/Periodogram.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1402 2023-04-21 22:38:42.000000 pywhiten-1.1.1/pywhiten/data/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:32:47.792461 pywhiten-1.1.1/pywhiten/optimization/
+-rw-r--r--   0 erik      (1000) erik      (1000)     9084 2023-04-21 22:38:42.000000 pywhiten-1.1.1/pywhiten/optimization/Optimizer.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      781 2023-04-21 22:38:42.000000 pywhiten-1.1.1/pywhiten/optimization/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1942 2023-03-09 22:20:31.000000 pywhiten-1.1.1/pywhiten/optimization/models.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:32:47.792461 pywhiten-1.1.1/pywhiten/pwio/
+-rw-r--r--   0 erik      (1000) erik      (1000)    14076 2023-04-21 22:38:42.000000 pywhiten-1.1.1/pywhiten/pwio/OutputManager.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      596 2023-04-21 22:38:42.000000 pywhiten-1.1.1/pywhiten/pwio/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1334 2023-03-09 20:17:13.000000 pywhiten-1.1.1/pywhiten/pwio/utilities.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:32:47.792461 pywhiten-1.1.1/pywhiten.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)    13517 2023-04-21 23:32:47.000000 pywhiten-1.1.1/pywhiten.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      891 2023-04-21 23:32:47.000000 pywhiten-1.1.1/pywhiten.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-04-21 23:32:47.000000 pywhiten-1.1.1/pywhiten.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-04-21 23:32:47.000000 pywhiten-1.1.1/pywhiten.egg-info/not-zip-safe
+-rw-r--r--   0 erik      (1000) erik      (1000)       43 2023-04-21 23:32:47.000000 pywhiten-1.1.1/pywhiten.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        9 2023-04-21 23:32:47.000000 pywhiten-1.1.1/pywhiten.egg-info/top_level.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       38 2023-04-21 23:32:47.795794 pywhiten-1.1.1/setup.cfg
+-rw-r--r--   0 erik      (1000) erik      (1000)      709 2023-04-21 23:28:03.000000 pywhiten-1.1.1/setup.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:32:47.792461 pywhiten-1.1.1/tests/
+-rw-r--r--   0 erik      (1000) erik      (1000)      988 2023-04-21 22:38:42.000000 pywhiten-1.1.1/tests/test_Frequency.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2200 2023-04-21 22:38:42.000000 pywhiten-1.1.1/tests/test_FrequencyContainer.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      236 2023-04-21 22:38:42.000000 pywhiten-1.1.1/tests/test_Lightcurve.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1828 2023-04-21 22:38:42.000000 pywhiten-1.1.1/tests/test_Optimizer.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      444 2023-04-21 22:38:42.000000 pywhiten-1.1.1/tests/test_OutputManager.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      156 2023-04-21 22:48:00.000000 pywhiten-1.1.1/tests/test_copyconfig.py
```

### Comparing `pywhiten-1.1.0/LICENSE` & `pywhiten-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/PKG-INFO` & `pywhiten-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywhiten
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python package for conducting Lomb-Scargle based prewhitening of stellar time series. 
 Home-page: https://www.github.com/erikstacey/pywhiten
 Author: Erik William Stacey
 Author-email: Erik Stacey <erik@erikstacey.com>
 License: MIT
 Project-URL: Homepage, https://github.com/erikstacey/pywhiten
 Project-URL: Bug Tracker, https://github.com/erikstacey/pywhiten/issues
@@ -208,13 +208,17 @@
    2) As the multi-frequency fit is intended as a refinement step, where parameters shouldn't change significantly, frequencies and amplitudes are bounded by default to a small region around their initial values.
 
 
 
 
 ## Change Log:
 
+* 1.1.1 (April 21, 2023)
+   * Made t0 of Frequency object an optional parameter
+
 * 1.1.0 (April 21, 2023)
    * Fixed major bug with installion scripts while using pip where submodules would not be properly installed.
    * Moved the default configuration loading and access to new module ```cfg```. Default configuration can now be accessed through ```pywhiten.cfg.default_cfg```.
+
 * 1.0.3 (April 5, 2023)
    * First non-internal release
```

### Comparing `pywhiten-1.1.0/README.md` & `pywhiten-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -190,13 +190,17 @@
    2) As the multi-frequency fit is intended as a refinement step, where parameters shouldn't change significantly, frequencies and amplitudes are bounded by default to a small region around their initial values.
 
 
 
 
 ## Change Log:
 
+* 1.1.1 (April 21, 2023)
+   * Made t0 of Frequency object an optional parameter
+
 * 1.1.0 (April 21, 2023)
    * Fixed major bug with installion scripts while using pip where submodules would not be properly installed.
    * Moved the default configuration loading and access to new module ```cfg```. Default configuration can now be accessed through ```pywhiten.cfg.default_cfg```.
+
 * 1.0.3 (April 5, 2023)
    * First non-internal release
```

### Comparing `pywhiten-1.1.0/pyproject.toml` & `pywhiten-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pywhiten"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Erik Stacey", email="erik@erikstacey.com" },
 ]
 description = "A python package for conducting Lomb-Scargle based prewhitening of stellar time series. "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pywhiten-1.1.0/pywhiten/PyWhitener.py` & `pywhiten-1.1.1/pywhiten/PyWhitener.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/pywhiten/__init__.py` & `pywhiten-1.1.1/pywhiten/__init__.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/pywhiten/cfg/cfgutils.py` & `pywhiten-1.1.1/pywhiten/cfg/cfgutils.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/pywhiten/cfg/default.toml` & `pywhiten-1.1.1/pywhiten/cfg/default.toml`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/pywhiten/data/Frequency.py` & `pywhiten-1.1.1/pywhiten/data/Frequency.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     f0 : float
     a0 : float
     p0 : float
 
     n = None
     model_function = None
 
-    def __init__(self, f:float, a:float, p:float, t0:float, model_function=sin_model, n:Union[int, None]=None):
+    def __init__(self, f:float, a:float, p:float, t0:float=0, model_function=sin_model, n:Union[int, None]=None):
         """
 
         Args:
             f (float): initial frequency
             a (float): initial amplitude
             p (float): initial phase
             t0 (float): reference time for phase
```

### Comparing `pywhiten-1.1.0/pywhiten/data/FrequencyContainer.py` & `pywhiten-1.1.1/pywhiten/data/FrequencyContainer.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/pywhiten/data/Lightcurve.py` & `pywhiten-1.1.1/pywhiten/data/Lightcurve.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/pywhiten/data/Periodogram.py` & `pywhiten-1.1.1/pywhiten/data/Periodogram.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/pywhiten/data/__init__.py` & `pywhiten-1.1.1/pywhiten/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/pywhiten/optimization/Optimizer.py` & `pywhiten-1.1.1/pywhiten/optimization/Optimizer.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/pywhiten/optimization/__init__.py` & `pywhiten-1.1.1/pywhiten/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/pywhiten/optimization/models.py` & `pywhiten-1.1.1/pywhiten/optimization/models.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/pywhiten/pwio/OutputManager.py` & `pywhiten-1.1.1/pywhiten/pwio/OutputManager.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/pywhiten/pwio/__init__.py` & `pywhiten-1.1.1/pywhiten/pwio/__init__.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/pywhiten/pwio/utilities.py` & `pywhiten-1.1.1/pywhiten/pwio/utilities.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/pywhiten.egg-info/PKG-INFO` & `pywhiten-1.1.1/pywhiten.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywhiten
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python package for conducting Lomb-Scargle based prewhitening of stellar time series. 
 Home-page: https://www.github.com/erikstacey/pywhiten
 Author: Erik William Stacey
 Author-email: Erik Stacey <erik@erikstacey.com>
 License: MIT
 Project-URL: Homepage, https://github.com/erikstacey/pywhiten
 Project-URL: Bug Tracker, https://github.com/erikstacey/pywhiten/issues
@@ -208,13 +208,17 @@
    2) As the multi-frequency fit is intended as a refinement step, where parameters shouldn't change significantly, frequencies and amplitudes are bounded by default to a small region around their initial values.
 
 
 
 
 ## Change Log:
 
+* 1.1.1 (April 21, 2023)
+   * Made t0 of Frequency object an optional parameter
+
 * 1.1.0 (April 21, 2023)
    * Fixed major bug with installion scripts while using pip where submodules would not be properly installed.
    * Moved the default configuration loading and access to new module ```cfg```. Default configuration can now be accessed through ```pywhiten.cfg.default_cfg```.
+
 * 1.0.3 (April 5, 2023)
    * First non-internal release
```

### Comparing `pywhiten-1.1.0/pywhiten.egg-info/SOURCES.txt` & `pywhiten-1.1.1/pywhiten.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/setup.py` & `pywhiten-1.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name="pywhiten",
-      version="1.1.0",
+      version="1.1.1",
       description="A python package for conducting Lomb-Scargle-based prewhitening of stellar time series. ",
       url="https://www.github.com/erikstacey/pywhiten",
       author="Erik William Stacey",
       author_email = "erik@erikstacey.com",
       license="MIT",
       packages= find_packages(where='.'),
       install_requires=[
```

### Comparing `pywhiten-1.1.0/tests/test_Frequency.py` & `pywhiten-1.1.1/tests/test_Frequency.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/tests/test_FrequencyContainer.py` & `pywhiten-1.1.1/tests/test_FrequencyContainer.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.1.0/tests/test_Optimizer.py` & `pywhiten-1.1.1/tests/test_Optimizer.py`

 * *Files identical despite different names*

