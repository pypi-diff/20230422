# Comparing `tmp/pywhiten-1.0.3.tar.gz` & `tmp/pywhiten-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywhiten-1.0.3.tar", last modified: Wed Apr  5 20:37:08 2023, max compression
+gzip compressed data, was "pywhiten-1.1.0.tar", last modified: Fri Apr 21 23:14:02 2023, max compression
```

## Comparing `pywhiten-1.0.3.tar` & `pywhiten-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,43 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-05 20:37:08.449471 pywhiten-1.0.3/
--rw-r--r--   0 erik      (1000) erik      (1000)     1068 2023-02-06 23:54:19.000000 pywhiten-1.0.3/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)    12810 2023-04-05 20:37:08.449471 pywhiten-1.0.3/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)    12080 2023-03-28 22:07:49.000000 pywhiten-1.0.3/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)      803 2023-04-05 20:06:32.000000 pywhiten-1.0.3/pyproject.toml
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-05 20:37:08.449471 pywhiten-1.0.3/pywhiten/
--rw-r--r--   0 erik      (1000) erik      (1000)    11813 2023-04-05 20:07:44.000000 pywhiten-1.0.3/pywhiten/PyWhitener.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2180 2023-04-05 20:37:04.000000 pywhiten-1.0.3/pywhiten/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-05 20:37:08.449471 pywhiten-1.0.3/pywhiten.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)    12810 2023-04-05 20:37:08.000000 pywhiten-1.0.3/pywhiten.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      434 2023-04-05 20:37:08.000000 pywhiten-1.0.3/pywhiten.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-04-05 20:37:08.000000 pywhiten-1.0.3/pywhiten.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-03-20 22:16:20.000000 pywhiten-1.0.3/pywhiten.egg-info/not-zip-safe
--rw-r--r--   0 erik      (1000) erik      (1000)       43 2023-04-05 20:37:08.000000 pywhiten-1.0.3/pywhiten.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        9 2023-04-05 20:37:08.000000 pywhiten-1.0.3/pywhiten.egg-info/top_level.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       38 2023-04-05 20:37:08.449471 pywhiten-1.0.3/setup.cfg
--rw-r--r--   0 erik      (1000) erik      (1000)      682 2023-04-05 20:06:32.000000 pywhiten-1.0.3/setup.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-05 20:37:08.449471 pywhiten-1.0.3/tests/
--rw-r--r--   0 erik      (1000) erik      (1000)      988 2023-03-09 22:18:34.000000 pywhiten-1.0.3/tests/test_Frequency.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2200 2023-04-05 20:33:04.000000 pywhiten-1.0.3/tests/test_FrequencyContainer.py
--rw-r--r--   0 erik      (1000) erik      (1000)      236 2023-02-14 19:35:23.000000 pywhiten-1.0.3/tests/test_Lightcurve.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1828 2023-03-13 19:17:09.000000 pywhiten-1.0.3/tests/test_Optimizer.py
--rw-r--r--   0 erik      (1000) erik      (1000)      444 2023-03-01 22:51:53.000000 pywhiten-1.0.3/tests/test_OutputManager.py
--rw-r--r--   0 erik      (1000) erik      (1000)      152 2023-03-15 21:29:02.000000 pywhiten-1.0.3/tests/test_copyconfig.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.592459 pywhiten-1.1.0/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1068 2023-02-06 23:54:19.000000 pywhiten-1.1.0/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)    13435 2023-04-21 23:14:02.592459 pywhiten-1.1.0/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)    12705 2023-04-21 23:00:01.000000 pywhiten-1.1.0/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)      803 2023-04-21 22:49:21.000000 pywhiten-1.1.0/pyproject.toml
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.589126 pywhiten-1.1.0/pywhiten/
+-rw-r--r--   0 erik      (1000) erik      (1000)    11869 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/PyWhitener.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1579 2023-04-21 22:44:08.000000 pywhiten-1.1.0/pywhiten/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.589126 pywhiten-1.1.0/pywhiten/cfg/
+-rw-r--r--   0 erik      (1000) erik      (1000)       83 2023-04-21 22:45:16.000000 pywhiten-1.1.0/pywhiten/cfg/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      617 2023-04-21 22:45:49.000000 pywhiten-1.1.0/pywhiten/cfg/cfgutils.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     6437 2023-03-20 18:59:49.000000 pywhiten-1.1.0/pywhiten/cfg/default.toml
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.592459 pywhiten-1.1.0/pywhiten/data/
+-rw-r--r--   0 erik      (1000) erik      (1000)     3792 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/data/Frequency.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4510 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/data/FrequencyContainer.py
+-rw-r--r--   0 erik      (1000) erik      (1000)       58 2023-02-14 19:27:58.000000 pywhiten-1.1.0/pywhiten/data/InvalidConstructorArgumentsError.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2983 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/data/Lightcurve.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    17451 2023-04-21 22:43:40.000000 pywhiten-1.1.0/pywhiten/data/Periodogram.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1402 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/data/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.592459 pywhiten-1.1.0/pywhiten/optimization/
+-rw-r--r--   0 erik      (1000) erik      (1000)     9084 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/optimization/Optimizer.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      781 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/optimization/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1942 2023-03-09 22:20:31.000000 pywhiten-1.1.0/pywhiten/optimization/models.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.592459 pywhiten-1.1.0/pywhiten/pwio/
+-rw-r--r--   0 erik      (1000) erik      (1000)    14076 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/pwio/OutputManager.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      596 2023-04-21 22:38:42.000000 pywhiten-1.1.0/pywhiten/pwio/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1334 2023-03-09 20:17:13.000000 pywhiten-1.1.0/pywhiten/pwio/utilities.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.589126 pywhiten-1.1.0/pywhiten.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)    13435 2023-04-21 23:14:02.000000 pywhiten-1.1.0/pywhiten.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      891 2023-04-21 23:14:02.000000 pywhiten-1.1.0/pywhiten.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-04-21 23:14:02.000000 pywhiten-1.1.0/pywhiten.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-04-21 22:59:24.000000 pywhiten-1.1.0/pywhiten.egg-info/not-zip-safe
+-rw-r--r--   0 erik      (1000) erik      (1000)       43 2023-04-21 23:14:02.000000 pywhiten-1.1.0/pywhiten.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        9 2023-04-21 23:14:02.000000 pywhiten-1.1.0/pywhiten.egg-info/top_level.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       38 2023-04-21 23:14:02.592459 pywhiten-1.1.0/setup.cfg
+-rw-r--r--   0 erik      (1000) erik      (1000)      709 2023-04-21 23:13:52.000000 pywhiten-1.1.0/setup.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-21 23:14:02.592459 pywhiten-1.1.0/tests/
+-rw-r--r--   0 erik      (1000) erik      (1000)      988 2023-04-21 22:38:42.000000 pywhiten-1.1.0/tests/test_Frequency.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2200 2023-04-21 22:38:42.000000 pywhiten-1.1.0/tests/test_FrequencyContainer.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      236 2023-04-21 22:38:42.000000 pywhiten-1.1.0/tests/test_Lightcurve.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1828 2023-04-21 22:38:42.000000 pywhiten-1.1.0/tests/test_Optimizer.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      444 2023-04-21 22:38:42.000000 pywhiten-1.1.0/tests/test_OutputManager.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      156 2023-04-21 22:48:00.000000 pywhiten-1.1.0/tests/test_copyconfig.py
```

### Comparing `pywhiten-1.0.3/LICENSE` & `pywhiten-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywhiten-1.0.3/PKG-INFO` & `pywhiten-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywhiten
-Version: 1.0.3
+Version: 1.1.0
 Summary: A python package for conducting Lomb-Scargle based prewhitening of stellar time series. 
 Home-page: https://www.github.com/erikstacey/pywhiten
 Author: Erik William Stacey
 Author-email: Erik Stacey <erik@erikstacey.com>
 License: MIT
 Project-URL: Homepage, https://github.com/erikstacey/pywhiten
 Project-URL: Bug Tracker, https://github.com/erikstacey/pywhiten/issues
@@ -14,15 +14,19 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![##PyWhiten](docs/img/pywhitenlogo3.png)
 
-A python package for conducting Lomb-Scargle-based pre-whitening of time series data.
+A flexible python package for conducting Lomb-Scargle-based pre-whitening of time series data. It is distinguished from other, similar tools by a focus on automated pipeline-style analysis and a high degree of flexibility through its extensive [configuration](https://pywhiten.readthedocs.io/en/latest/configuration/) system.
+
+Written by [Erik Stacey](https://www.erikstacey.com/)
+
+Updated 19 April 2023.
 
 # Installation
 
 pywhiten is available through pip:  
 ```
 pip install pywhiten
 ```
@@ -31,15 +35,15 @@
 git clone https://github.com/erikstacey/pywhiten.git ./pywhiten
 cd pywhiten
 pip install .
 ```
 
 
 # Documentation
-The general documentation is available [here](https://pywhiten.readthedocs.io/en/latest/), and a getting started guide is available [here](https://pywhiten.readthedocs.io/en/latest/getting-started) or in the next section. Please note this documentation is currently under construction!
+The general documentation is available [here](https://pywhiten.readthedocs.io/en/latest/), and a getting started guide is available [here](https://pywhiten.readthedocs.io/en/latest/getting-started) or in the next section.
 # Getting Started
 Pywhiten was designed to be easy to get up and running quickly out of the box, so let us walk through a tutorial example.
 ## Setting up a tutorial directory
 First, lets create a tutorial directory somewhere:
 ```
 mkdir pywhiten_tutorial
 cd pywhiten_tutorial
@@ -202,9 +206,15 @@
 2) Allowing the frequencies to vary in the multi-frequency fit can cause the optimization to fail. Pywhiten implements two safeguards against this, which are generally effective at preventing anomalous results or runtime failures:
    1) New frequencies are not selected within 1.5/T of existing frequencies, where T is the total time baseline of the dataset. This is the (empirical) minimum separation between two frequencies necessary to make reliable independent measurements of each of them.
    2) As the multi-frequency fit is intended as a refinement step, where parameters shouldn't change significantly, frequencies and amplitudes are bounded by default to a small region around their initial values.
 
 
 
 
+## Change Log:
 
+* 1.1.0 (April 21, 2023)
+   * Fixed major bug with installion scripts while using pip where submodules would not be properly installed.
+   * Moved the default configuration loading and access to new module ```cfg```. Default configuration can now be accessed through ```pywhiten.cfg.default_cfg```.
+* 1.0.3 (April 5, 2023)
+   * First non-internal release
```

### Comparing `pywhiten-1.0.3/README.md` & `pywhiten-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 ![##PyWhiten](docs/img/pywhitenlogo3.png)
 
-A python package for conducting Lomb-Scargle-based pre-whitening of time series data.
+A flexible python package for conducting Lomb-Scargle-based pre-whitening of time series data. It is distinguished from other, similar tools by a focus on automated pipeline-style analysis and a high degree of flexibility through its extensive [configuration](https://pywhiten.readthedocs.io/en/latest/configuration/) system.
+
+Written by [Erik Stacey](https://www.erikstacey.com/)
+
+Updated 19 April 2023.
 
 # Installation
 
 pywhiten is available through pip:  
 ```
 pip install pywhiten
 ```
@@ -13,15 +17,15 @@
 git clone https://github.com/erikstacey/pywhiten.git ./pywhiten
 cd pywhiten
 pip install .
 ```
 
 
 # Documentation
-The general documentation is available [here](https://pywhiten.readthedocs.io/en/latest/), and a getting started guide is available [here](https://pywhiten.readthedocs.io/en/latest/getting-started) or in the next section. Please note this documentation is currently under construction!
+The general documentation is available [here](https://pywhiten.readthedocs.io/en/latest/), and a getting started guide is available [here](https://pywhiten.readthedocs.io/en/latest/getting-started) or in the next section.
 # Getting Started
 Pywhiten was designed to be easy to get up and running quickly out of the box, so let us walk through a tutorial example.
 ## Setting up a tutorial directory
 First, lets create a tutorial directory somewhere:
 ```
 mkdir pywhiten_tutorial
 cd pywhiten_tutorial
@@ -184,9 +188,15 @@
 2) Allowing the frequencies to vary in the multi-frequency fit can cause the optimization to fail. Pywhiten implements two safeguards against this, which are generally effective at preventing anomalous results or runtime failures:
    1) New frequencies are not selected within 1.5/T of existing frequencies, where T is the total time baseline of the dataset. This is the (empirical) minimum separation between two frequencies necessary to make reliable independent measurements of each of them.
    2) As the multi-frequency fit is intended as a refinement step, where parameters shouldn't change significantly, frequencies and amplitudes are bounded by default to a small region around their initial values.
 
 
 
 
+## Change Log:
 
+* 1.1.0 (April 21, 2023)
+   * Fixed major bug with installion scripts while using pip where submodules would not be properly installed.
+   * Moved the default configuration loading and access to new module ```cfg```. Default configuration can now be accessed through ```pywhiten.cfg.default_cfg```.
+* 1.0.3 (April 5, 2023)
+   * First non-internal release
```

### Comparing `pywhiten-1.0.3/pyproject.toml` & `pywhiten-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pywhiten"
-version = "1.0.3"
+version = "1.1.0"
 authors = [
   { name="Erik Stacey", email="erik@erikstacey.com" },
 ]
 description = "A python package for conducting Lomb-Scargle based prewhitening of stellar time series. "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pywhiten-1.0.3/pywhiten/PyWhitener.py` & `pywhiten-1.1.0/pywhiten/PyWhitener.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,17 @@
             self.cfg = merge_dict(self.cfg, cfg)
             self.cfg["title"] += " - Merged with runtime-specified arguments"
         # handle special logic cases
         pass
         # config setup done
         # now set up initial light curve, frequency container, output mgr
         if self.cfg["input"]["subtract_mean"]:
-            self.lcs = [Lightcurve(time, data-np.mean(data), err)]
+            self.lcs = [Lightcurve(time, data-np.mean(data), err, cfg=self.cfg)]
         else:
-            self.lcs = [Lightcurve(time, data, err)]
+            self.lcs = [Lightcurve(time, data, err, cfg=self.cfg)]
         self.freqs = FrequencyContainer()
         self.output_manager = OutputManager(cfg=self.cfg)
         self.optimizer = Optimizer(cfg = self.cfg)
 
         # we're now ready to do some frequency analysis
 
     def id_peak(self, method, min_prov_sig = 0, idx=-1):
@@ -155,18 +155,18 @@
         if self.cfg["output"]["print_runtime_messages"]:
             print(f"[pywhiten] Completed optimization of current complete variability model:")
             for f_to_print in self.freqs.get_flist():
                 f_to_print.prettyprint()
 
         # Final Stage, make a new light curve and append it to the lightcurves list
         if self.cfg["autopw"]["new_lc_generation_method"] == "mf":
-            self.lcs.append(Lightcurve(self.lcs[0].time, self.lcs[0].data - mf_mod, err = self.lcs[0].err))
+            self.lcs.append(Lightcurve(self.lcs[0].time, self.lcs[0].data - mf_mod, err = self.lcs[0].err, cfg=self.cfg))
             return 0
         elif self.cfg["autopw"]["new_lc_generation_method"] == "sf":
-            self.lcs.append(Lightcurve(self.lcs[-1].time, self.lcs[-1].data - sf_model, err=self.lcs[0].err))
+            self.lcs.append(Lightcurve(self.lcs[-1].time, self.lcs[-1].data - sf_model, err=self.lcs[0].err, cfg=self.cfg))
             return 0
         return 2
 
     def auto(self):
         for i in range(self.cfg["autopw"]["cutoff_iteration"]):
             success_flag = -1
             if i < self.cfg["autopw"]["peak_selection_highest_override"]:
```

### Comparing `pywhiten-1.0.3/pywhiten/__init__.py` & `pywhiten-1.1.0/pywhiten/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,37 +17,21 @@
     data: Contains data structures that are useful for pre-whitening
     optimization: Contains all mathematical optimization functionality for the package
     pwio: Contains input/output functionality
 Variables:
     default_cfg (dict): A dictionary storing the default configuration
     pkg_path (string): A string storing the local path to the package
 """
-import tomli
-import os
-
-pkg_path = os.path.dirname(os.path.abspath(__file__))
-default_cfg_path = os.path.join(pkg_path, 'cfg', 'default.toml')
-
-with open(default_cfg_path, "rb") as f:
-    default_cfg = tomli.load(f)
-
-from pywhiten.PyWhitener import PyWhitener
+import pywhiten.cfg
 import pywhiten.data
 import pywhiten.pwio
 import pywhiten.optimization
+from pywhiten.PyWhitener import PyWhitener
+
+
+
+
 
-def make_config_file(path="./default.toml"):
-    import shutil
-    """
-    Copies the default config file to somewhere (typically) outside the package files, so it can be edited by the user.
-    Args:
-        path (str): Path to copy the default configuration to
-
-    Returns:
-
-    """
-    shutil.copyfile(default_cfg_path, path)
-    print(f"[pywhiten] Made a copy of default configuration file at {path}!")
```

### Comparing `pywhiten-1.0.3/pywhiten.egg-info/PKG-INFO` & `pywhiten-1.1.0/pywhiten.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywhiten
-Version: 1.0.3
+Version: 1.1.0
 Summary: A python package for conducting Lomb-Scargle based prewhitening of stellar time series. 
 Home-page: https://www.github.com/erikstacey/pywhiten
 Author: Erik William Stacey
 Author-email: Erik Stacey <erik@erikstacey.com>
 License: MIT
 Project-URL: Homepage, https://github.com/erikstacey/pywhiten
 Project-URL: Bug Tracker, https://github.com/erikstacey/pywhiten/issues
@@ -14,15 +14,19 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![##PyWhiten](docs/img/pywhitenlogo3.png)
 
-A python package for conducting Lomb-Scargle-based pre-whitening of time series data.
+A flexible python package for conducting Lomb-Scargle-based pre-whitening of time series data. It is distinguished from other, similar tools by a focus on automated pipeline-style analysis and a high degree of flexibility through its extensive [configuration](https://pywhiten.readthedocs.io/en/latest/configuration/) system.
+
+Written by [Erik Stacey](https://www.erikstacey.com/)
+
+Updated 19 April 2023.
 
 # Installation
 
 pywhiten is available through pip:  
 ```
 pip install pywhiten
 ```
@@ -31,15 +35,15 @@
 git clone https://github.com/erikstacey/pywhiten.git ./pywhiten
 cd pywhiten
 pip install .
 ```
 
 
 # Documentation
-The general documentation is available [here](https://pywhiten.readthedocs.io/en/latest/), and a getting started guide is available [here](https://pywhiten.readthedocs.io/en/latest/getting-started) or in the next section. Please note this documentation is currently under construction!
+The general documentation is available [here](https://pywhiten.readthedocs.io/en/latest/), and a getting started guide is available [here](https://pywhiten.readthedocs.io/en/latest/getting-started) or in the next section.
 # Getting Started
 Pywhiten was designed to be easy to get up and running quickly out of the box, so let us walk through a tutorial example.
 ## Setting up a tutorial directory
 First, lets create a tutorial directory somewhere:
 ```
 mkdir pywhiten_tutorial
 cd pywhiten_tutorial
@@ -202,9 +206,15 @@
 2) Allowing the frequencies to vary in the multi-frequency fit can cause the optimization to fail. Pywhiten implements two safeguards against this, which are generally effective at preventing anomalous results or runtime failures:
    1) New frequencies are not selected within 1.5/T of existing frequencies, where T is the total time baseline of the dataset. This is the (empirical) minimum separation between two frequencies necessary to make reliable independent measurements of each of them.
    2) As the multi-frequency fit is intended as a refinement step, where parameters shouldn't change significantly, frequencies and amplitudes are bounded by default to a small region around their initial values.
 
 
 
 
+## Change Log:
 
+* 1.1.0 (April 21, 2023)
+   * Fixed major bug with installion scripts while using pip where submodules would not be properly installed.
+   * Moved the default configuration loading and access to new module ```cfg```. Default configuration can now be accessed through ```pywhiten.cfg.default_cfg```.
+* 1.0.3 (April 5, 2023)
+   * First non-internal release
```

### Comparing `pywhiten-1.0.3/tests/test_Frequency.py` & `pywhiten-1.1.0/tests/test_Frequency.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.0.3/tests/test_FrequencyContainer.py` & `pywhiten-1.1.0/tests/test_FrequencyContainer.py`

 * *Files identical despite different names*

### Comparing `pywhiten-1.0.3/tests/test_Optimizer.py` & `pywhiten-1.1.0/tests/test_Optimizer.py`

 * *Files identical despite different names*

