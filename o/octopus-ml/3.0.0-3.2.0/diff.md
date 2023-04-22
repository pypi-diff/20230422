# Comparing `tmp/octopus-ml-3.0.0.tar.gz` & `tmp/octopus-ml-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octopus-ml-3.0.0.tar", last modified: Sat Oct 15 08:45:08 2022, max compression
+gzip compressed data, was "octopus-ml-3.2.0.tar", last modified: Sat Apr 22 16:34:29 2023, max compression
```

## Comparing `octopus-ml-3.0.0.tar` & `octopus-ml-3.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-10-15 08:45:08.706000 octopus-ml-3.0.0/
--rw-rw-rw-   0        0        0     1073 2022-04-23 10:20:13.000000 octopus-ml-3.0.0/LICENSE
--rw-rw-rw-   0        0        0     3252 2022-10-15 08:45:08.701000 octopus-ml-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2703 2022-04-23 10:20:13.000000 octopus-ml-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2022-10-15 08:45:08.658000 octopus-ml-3.0.0/octopus_ml/
--rw-rw-rw-   0        0        0      932 2022-04-23 10:20:14.000000 octopus-ml-3.0.0/octopus_ml/__init__.py
--rw-rw-rw-   0        0        0     1126 2022-04-23 10:20:14.000000 octopus-ml-3.0.0/octopus_ml/misc.py
--rw-rw-rw-   0        0        0     9156 2022-04-23 10:20:14.000000 octopus-ml-3.0.0/octopus_ml/octopus_data.py
--rw-rw-rw-   0        0        0    20348 2022-06-04 17:01:20.000000 octopus-ml-3.0.0/octopus_ml/octopus_ml.py
-drwxrwxrwx   0        0        0        0 2022-10-15 08:45:08.696000 octopus-ml-3.0.0/octopus_ml.egg-info/
--rw-rw-rw-   0        0        0     3252 2022-10-15 08:45:08.000000 octopus-ml-3.0.0/octopus_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2022-10-15 08:45:08.000000 octopus-ml-3.0.0/octopus_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-15 08:45:08.000000 octopus-ml-3.0.0/octopus_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2022-10-15 08:45:08.000000 octopus-ml-3.0.0/octopus_ml.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-10-15 08:45:08.000000 octopus-ml-3.0.0/octopus_ml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-15 08:45:08.705000 octopus-ml-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      768 2022-06-04 16:58:32.000000 octopus-ml-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:34:29.664000 octopus-ml-3.2.0/
+-rw-rw-rw-   0        0        0     1073 2022-04-23 10:20:13.000000 octopus-ml-3.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3575 2023-04-22 16:34:29.658000 octopus-ml-3.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3068 2023-01-02 10:55:12.000000 octopus-ml-3.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 16:34:29.613000 octopus-ml-3.2.0/octopus_ml/
+-rw-rw-rw-   0        0        0      932 2022-04-23 10:20:14.000000 octopus-ml-3.2.0/octopus_ml/__init__.py
+-rw-rw-rw-   0        0        0     1126 2022-04-23 10:20:14.000000 octopus-ml-3.2.0/octopus_ml/misc.py
+-rw-rw-rw-   0        0        0     9156 2022-04-23 10:20:14.000000 octopus-ml-3.2.0/octopus_ml/octopus_data.py
+-rw-rw-rw-   0        0        0    20138 2023-04-22 15:49:20.000000 octopus-ml-3.2.0/octopus_ml/octopus_ml.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:34:29.652000 octopus-ml-3.2.0/octopus_ml.egg-info/
+-rw-rw-rw-   0        0        0     3575 2023-04-22 16:34:29.000000 octopus-ml-3.2.0/octopus_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-04-22 16:34:29.000000 octopus-ml-3.2.0/octopus_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 16:34:29.000000 octopus-ml-3.2.0/octopus_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-22 16:34:29.000000 octopus-ml-3.2.0/octopus_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-22 16:34:29.000000 octopus-ml-3.2.0/octopus_ml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 16:34:29.662000 octopus-ml-3.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      768 2023-04-22 16:34:08.000000 octopus-ml-3.2.0/setup.py
```

### Comparing `octopus-ml-3.0.0/LICENSE` & `octopus-ml-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `octopus-ml-3.0.0/PKG-INFO` & `octopus-ml-3.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octopus-ml
-Version: 3.0.0
+Version: 3.2.0
 Summary: A collection of handy ML and data validation tools
 Home-page: https://github.com/gershonc/octopus-ml
 Author: Gershon Celniker
 Author-email: gershonc@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -23,15 +23,15 @@
 [![Downloads](https://pepy.tech/badge/octopus-ml)](https://pepy.tech/project/octopus-ml)
 [![Colab Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1T1T15AZe0w7Zcld_09jxg-Yhq2pBefVZ?usp=sharing)
 
 
 <!-- 
 [![Code Coverage](https://codecov.io/gh/pandas-profiling/octopus-ml/branch/master/graph/badge.svg?token=gMptB4YUnF)](https://codecov.io/gh/octopus/octopus)
 -->
-Set of handy ML and data tools - from data exploration, visualization, pre-processing, hyper parameter tuning, modeling and all the way to final ML model evaluation 
+Set of handy ML and data tools - starting from data exploration, visualization, pre-processing, hyper parameter tuning, modeling and all the way to final ML model evaluation 
 <br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/octopus_know_your_data.png" width="540" height="460" /></center>
 
 Check out the octopus-ml demo notebook on Colab <a href="https://colab.research.google.com/drive/1T1T15AZe0w7Zcld_09jxg-Yhq2pBefVZ?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="google colab logo"></a>
  
 ## Installation
 The module can be easily installed with pip:
 
@@ -48,10 +48,16 @@
 
 ```python
 from octopus_ml import plot_imp, adjusted_classes, cv, cv_plot, roc_curve_plot, ...
 
 ```
 <br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_cv.png" width="820"/></center>
 <br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_prediction_distribution.png" width="720" /></center>
+
+## Selected visualizations:
+<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/target_distribution_plot.png" width="520"/></center>
+<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/histogram_on_target.png" width="520"/></center>
+
+
 <br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_roc.png" width="520"/></center>
 <br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_confusion_matrix.png" width="580" /></center>
 <br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_feature_imp.png" width="820"/></center>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: octopus-ml Version: 3.0.0 Summary: A collection of
+Metadata-Version: 2.1 Name: octopus-ml Version: 3.2.0 Summary: A collection of
 handy ML and data validation tools Home-page: https://github.com/gershonc/
 octopus-ml Author: Gershon Celniker Author-email: gershonc@gmail.com License:
 MIT Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 4 - Beta Description-Content-Type: text/
 markdown License-File: LICENSE # Octopus-ML [![PyPI Latest Release](https://
 img.shields.io/pypi/v/octopus-ml.svg)](https://pypi.org/project/octopus-ml/) [!
@@ -12,30 +12,36 @@
 octopus-ml/) [![Code style: black](https://img.shields.io/badge/code%20style-
 black-000000.svg)](https://github.com/python/black) [![Binder](https://
 mybinder.org/badge.svg)](https://hub.gke2.mybinder.org/user/gershonc-octopus-
 ml-k5of97xu/tree) [![Downloads](https://pepy.tech/badge/octopus-ml)](https://
 pepy.tech/project/octopus-ml) [![Colab Demo](https://colab.research.google.com/
 assets/colab-badge.svg)](https://colab.research.google.com/drive/
 1T1T15AZe0w7Zcld_09jxg-Yhq2pBefVZ?usp=sharing)  Set of handy ML and data tools
-- from data exploration, visualization, pre-processing, hyper parameter tuning,
-modeling and all the way to final ML model evaluation
+- starting from data exploration, visualization, pre-processing, hyper
+parameter tuning, modeling and all the way to final ML model evaluation
       [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
                           octopus_know_your_data.png]
 Check out the octopus-ml demo notebook on Colab [google_colab_logo] ##
 Installation The module can be easily installed with pip: ```conslole > pip
 install octopus-ml ``` This module depends on `Scikit-learn`, `NumPy`,
 `Pandas`, `TQDM`, `lightGBM` as defualt classifier. Optionally you can get also
 some nice visualisations if you have `Seaborn` installed. ## Usage The module
 contains ML and Data related methods: ```python from octopus_ml import
 plot_imp, adjusted_classes, cv, cv_plot, roc_curve_plot, ... ```
       [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
                                 oc_plot_cv.png]
 
       [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
                      oc_plot_prediction_distribution.png]
+## Selected visualizations:
+      [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
+                         target_distribution_plot.png]
+
+      [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
+                           histogram_on_target.png]
 
       [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
                                oc_plot_roc.png]
 
       [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
                          oc_plot_confusion_matrix.png]
```

### Comparing `octopus-ml-3.0.0/README.md` & `octopus-ml-3.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,48 @@
-# Octopus-ML
- 
-[![PyPI Latest Release](https://img.shields.io/pypi/v/octopus-ml.svg)](https://pypi.org/project/octopus-ml/)
-[![License](https://img.shields.io/pypi/l/octopus-ml.svg)](https://github.com/gershonc//octopus-ml/blob/master/LICENSE)
-[![Python Version](https://img.shields.io/pypi/pyversions/pandas-profiling)](https://pypi.org/project/octopus-ml/)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
-[![Binder](https://mybinder.org/badge.svg)](https://hub.gke2.mybinder.org/user/gershonc-octopus-ml-k5of97xu/tree)
-[![Downloads](https://pepy.tech/badge/octopus-ml)](https://pepy.tech/project/octopus-ml)
-[![Colab Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1T1T15AZe0w7Zcld_09jxg-Yhq2pBefVZ?usp=sharing)
-
-
-<!-- 
-[![Code Coverage](https://codecov.io/gh/pandas-profiling/octopus-ml/branch/master/graph/badge.svg?token=gMptB4YUnF)](https://codecov.io/gh/octopus/octopus)
--->
-Set of handy ML and data tools - from data exploration, visualization, pre-processing, hyper parameter tuning, modeling and all the way to final ML model evaluation 
-<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/octopus_know_your_data.png" width="540" height="460" /></center>
-
-Check out the octopus-ml demo notebook on Colab <a href="https://colab.research.google.com/drive/1T1T15AZe0w7Zcld_09jxg-Yhq2pBefVZ?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="google colab logo"></a>
- 
-## Installation
-The module can be easily installed with pip:
-
-```conslole
-> pip install octopus-ml
-```
-
-This module depends on `Scikit-learn`, `NumPy`, `Pandas`, `TQDM`, `lightGBM` as defualt classifier. Optionally you can get also some nice visualisations if you have `Seaborn` installed.
-
-
-
-## Usage
-The module contains ML and Data related methods:
-
-```python
-from octopus_ml import plot_imp, adjusted_classes, cv, cv_plot, roc_curve_plot, ...
-
-```
-<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_cv.png" width="820"/></center>
-<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_prediction_distribution.png" width="720" /></center>
-<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_roc.png" width="520"/></center>
-<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_confusion_matrix.png" width="580" /></center>
-<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_feature_imp.png" width="820"/></center>
+# Octopus-ML
+ 
+[![PyPI Latest Release](https://img.shields.io/pypi/v/octopus-ml.svg)](https://pypi.org/project/octopus-ml/)
+[![License](https://img.shields.io/pypi/l/octopus-ml.svg)](https://github.com/gershonc//octopus-ml/blob/master/LICENSE)
+[![Python Version](https://img.shields.io/pypi/pyversions/pandas-profiling)](https://pypi.org/project/octopus-ml/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+[![Binder](https://mybinder.org/badge.svg)](https://hub.gke2.mybinder.org/user/gershonc-octopus-ml-k5of97xu/tree)
+[![Downloads](https://pepy.tech/badge/octopus-ml)](https://pepy.tech/project/octopus-ml)
+[![Colab Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1T1T15AZe0w7Zcld_09jxg-Yhq2pBefVZ?usp=sharing)
+
+
+<!-- 
+[![Code Coverage](https://codecov.io/gh/pandas-profiling/octopus-ml/branch/master/graph/badge.svg?token=gMptB4YUnF)](https://codecov.io/gh/octopus/octopus)
+-->
+Set of handy ML and data tools - starting from data exploration, visualization, pre-processing, hyper parameter tuning, modeling and all the way to final ML model evaluation 
+<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/octopus_know_your_data.png" width="540" height="460" /></center>
+
+Check out the octopus-ml demo notebook on Colab <a href="https://colab.research.google.com/drive/1T1T15AZe0w7Zcld_09jxg-Yhq2pBefVZ?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="google colab logo"></a>
+ 
+## Installation
+The module can be easily installed with pip:
+
+```conslole
+> pip install octopus-ml
+```
+
+This module depends on `Scikit-learn`, `NumPy`, `Pandas`, `TQDM`, `lightGBM` as defualt classifier. Optionally you can get also some nice visualisations if you have `Seaborn` installed.
+
+
+
+## Usage
+The module contains ML and Data related methods:
+
+```python
+from octopus_ml import plot_imp, adjusted_classes, cv, cv_plot, roc_curve_plot, ...
+
+```
+<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_cv.png" width="820"/></center>
+<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_prediction_distribution.png" width="720" /></center>
+
+## Selected visualizations:
+<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/target_distribution_plot.png" width="520"/></center>
+<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/histogram_on_target.png" width="520"/></center>
+
+
+<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_roc.png" width="520"/></center>
+<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_confusion_matrix.png" width="580" /></center>
+<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_feature_imp.png" width="820"/></center>
```

#### html2text {}

```diff
@@ -5,31 +5,37 @@
 pandas-profiling)](https://pypi.org/project/octopus-ml/) [![Code style: black]
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
 github.com/python/black) [![Binder](https://mybinder.org/badge.svg)](https://
 hub.gke2.mybinder.org/user/gershonc-octopus-ml-k5of97xu/tree) [![Downloads]
 (https://pepy.tech/badge/octopus-ml)](https://pepy.tech/project/octopus-ml) [!
 [Colab Demo](https://colab.research.google.com/assets/colab-badge.svg)](https:/
 /colab.research.google.com/drive/1T1T15AZe0w7Zcld_09jxg-Yhq2pBefVZ?usp=sharing)
-Set of handy ML and data tools - from data exploration, visualization, pre-
-processing, hyper parameter tuning, modeling and all the way to final ML model
-evaluation
+Set of handy ML and data tools - starting from data exploration, visualization,
+pre-processing, hyper parameter tuning, modeling and all the way to final ML
+model evaluation
       [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
                           octopus_know_your_data.png]
 Check out the octopus-ml demo notebook on Colab [google_colab_logo] ##
 Installation The module can be easily installed with pip: ```conslole > pip
 install octopus-ml ``` This module depends on `Scikit-learn`, `NumPy`,
 `Pandas`, `TQDM`, `lightGBM` as defualt classifier. Optionally you can get also
 some nice visualisations if you have `Seaborn` installed. ## Usage The module
 contains ML and Data related methods: ```python from octopus_ml import
 plot_imp, adjusted_classes, cv, cv_plot, roc_curve_plot, ... ```
       [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
                                 oc_plot_cv.png]
 
       [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
                      oc_plot_prediction_distribution.png]
+## Selected visualizations:
+      [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
+                         target_distribution_plot.png]
+
+      [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
+                           histogram_on_target.png]
 
       [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
                                oc_plot_roc.png]
 
       [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
                          oc_plot_confusion_matrix.png]
```

### Comparing `octopus-ml-3.0.0/octopus_ml/__init__.py` & `octopus-ml-3.2.0/octopus_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `octopus-ml-3.0.0/octopus_ml/misc.py` & `octopus-ml-3.2.0/octopus_ml/misc.py`

 * *Files identical despite different names*

### Comparing `octopus-ml-3.0.0/octopus_ml/octopus_data.py` & `octopus-ml-3.2.0/octopus_ml/octopus_data.py`

 * *Files identical despite different names*

### Comparing `octopus-ml-3.0.0/octopus_ml/octopus_ml.py` & `octopus-ml-3.2.0/octopus_ml/octopus_ml.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,21 +43,17 @@
 
 # ML visualizations
 
 def plot_imp(
     clf, X, title, model="lgbm", num=30, importaince_type="gain", save_path=None
 ):
     # Feature importance plot supporting LGBM, RN and Catboost, return the list of features importance sorted by their contribution
-    #sns.set_style("whitegrid")
-    gcbest = ["#3498db", "#2ecc71"]
-    sns.set_context("paper", font_scale=1)
-    sns.set_palette(gcbest)
-
- 
-
+    sns.set_style("whitegrid")
+    
+    
     if model == "catboost":
         feature_imp = pd.DataFrame(
             {"Value": clf.get_feature_importance(), "Feature": X.columns}
         )
     elif model == "lgbm":
         feature_imp = pd.DataFrame(
             {
@@ -151,60 +147,60 @@
     plt.rcParams["figure.figsize"] = (10, size)
     imp_coef.plot(kind="barh", color="#3498db")
     plt.title("Features correlations to target")
 
     if save_path:
         plt.savefig(save_path)
 
-
 def label_dist(df, label, y=None):
     # Target distribution analysis
+    
+    set_matplotlib_formats('svg')
     gcbest = ["#3498db", "#2ecc71"]
-    sns.set_context("paper", font_scale=1)
     sns.set_palette(gcbest)
 
     fig, ax = plt.subplots(1, 2)
-    plt.figure(figsize=(2, 3))
-    #sns.set_style("whitegrid")
-    set_matplotlib_formats('svg')
-    #plt.style.use("seaborn-notebook")
-    #sns.set_context("paper", font_scale=1.3)
+    plt.figure(figsize=(2, 2.8))
+    #set_matplotlib_formats('svg')
     sns.set_context(font_scale=1)
     
     if y is not None:
-        splot = sns.countplot("label", data=y.to_frame("label").reset_index(), ax=ax[0])
+        splot = sns.countplot(x=label, data=y.to_frame("label").reset_index(), ax=ax[0])
 
         for p in splot.patches:
             splot.annotate(
                 format(p.get_height(), ".0f"),
                 (p.get_x() + p.get_width() / 2.0, p.get_height()),
                 ha="center",
                 va="center",
                 xytext=(0, 10),
                 textcoords="offset points",
             )
         y.value_counts().plot.pie(explode=[0, 0.2], autopct="%1.2f%%", ax=ax[1])
     else:
-        splot = sns.countplot(label, data=df, ax=ax[0])
+        splot = sns.countplot(x=label, data=df, ax=ax[0])
+
         for p in splot.patches:
             splot.annotate(
                 format(p.get_height(), ".0f"),
                 (p.get_x() + p.get_width() / 2.0, p.get_height()),
                 ha="center",
                 va="center",
                 xytext=(0, 10),
                 textcoords="offset points",
             )
 
         df[label].value_counts().plot.pie(explode=[0, 0.2], autopct="%1.2f%%", ax=ax[1])
     fig.show()
 
 
+
 def roc_curve_plot(y_test, predictions, save_path=None):
     # Roc curve visualization, binary classification including AUC calculation
+
     set_matplotlib_formats('svg')
     gcbest = ["#3498db", "#2ecc71"]
     sns.set_palette(gcbest)
     sns.set_context("paper", font_scale=1)
 
     #plt.style.use('classic')
     sns.set_style("whitegrid")
@@ -357,15 +353,15 @@
         alpha=0.5,
         label="negative",
         weights=weights_false,
     )
     ax.hist(
         y_pred_true,
         bins=bins,
-        color="g",
+        color="#2ecc71",
         alpha=0.5,
         label="positive",
         weights=weights_true,
     )
     ax.set_title(title, fontsize=title_fontsize)
     # _set_lim(max_y, ax.set_ylim)
     ax.set_ylim(0, max_y)
```

### Comparing `octopus-ml-3.0.0/octopus_ml.egg-info/PKG-INFO` & `octopus-ml-3.2.0/octopus_ml.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octopus-ml
-Version: 3.0.0
+Version: 3.2.0
 Summary: A collection of handy ML and data validation tools
 Home-page: https://github.com/gershonc/octopus-ml
 Author: Gershon Celniker
 Author-email: gershonc@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -23,15 +23,15 @@
 [![Downloads](https://pepy.tech/badge/octopus-ml)](https://pepy.tech/project/octopus-ml)
 [![Colab Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1T1T15AZe0w7Zcld_09jxg-Yhq2pBefVZ?usp=sharing)
 
 
 <!-- 
 [![Code Coverage](https://codecov.io/gh/pandas-profiling/octopus-ml/branch/master/graph/badge.svg?token=gMptB4YUnF)](https://codecov.io/gh/octopus/octopus)
 -->
-Set of handy ML and data tools - from data exploration, visualization, pre-processing, hyper parameter tuning, modeling and all the way to final ML model evaluation 
+Set of handy ML and data tools - starting from data exploration, visualization, pre-processing, hyper parameter tuning, modeling and all the way to final ML model evaluation 
 <br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/octopus_know_your_data.png" width="540" height="460" /></center>
 
 Check out the octopus-ml demo notebook on Colab <a href="https://colab.research.google.com/drive/1T1T15AZe0w7Zcld_09jxg-Yhq2pBefVZ?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="google colab logo"></a>
  
 ## Installation
 The module can be easily installed with pip:
 
@@ -48,10 +48,16 @@
 
 ```python
 from octopus_ml import plot_imp, adjusted_classes, cv, cv_plot, roc_curve_plot, ...
 
 ```
 <br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_cv.png" width="820"/></center>
 <br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_prediction_distribution.png" width="720" /></center>
+
+## Selected visualizations:
+<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/target_distribution_plot.png" width="520"/></center>
+<br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/histogram_on_target.png" width="520"/></center>
+
+
 <br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_roc.png" width="520"/></center>
 <br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_confusion_matrix.png" width="580" /></center>
 <br><center><img src="https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/oc_plot_feature_imp.png" width="820"/></center>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: octopus-ml Version: 3.0.0 Summary: A collection of
+Metadata-Version: 2.1 Name: octopus-ml Version: 3.2.0 Summary: A collection of
 handy ML and data validation tools Home-page: https://github.com/gershonc/
 octopus-ml Author: Gershon Celniker Author-email: gershonc@gmail.com License:
 MIT Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 4 - Beta Description-Content-Type: text/
 markdown License-File: LICENSE # Octopus-ML [![PyPI Latest Release](https://
 img.shields.io/pypi/v/octopus-ml.svg)](https://pypi.org/project/octopus-ml/) [!
@@ -12,30 +12,36 @@
 octopus-ml/) [![Code style: black](https://img.shields.io/badge/code%20style-
 black-000000.svg)](https://github.com/python/black) [![Binder](https://
 mybinder.org/badge.svg)](https://hub.gke2.mybinder.org/user/gershonc-octopus-
 ml-k5of97xu/tree) [![Downloads](https://pepy.tech/badge/octopus-ml)](https://
 pepy.tech/project/octopus-ml) [![Colab Demo](https://colab.research.google.com/
 assets/colab-badge.svg)](https://colab.research.google.com/drive/
 1T1T15AZe0w7Zcld_09jxg-Yhq2pBefVZ?usp=sharing)  Set of handy ML and data tools
-- from data exploration, visualization, pre-processing, hyper parameter tuning,
-modeling and all the way to final ML model evaluation
+- starting from data exploration, visualization, pre-processing, hyper
+parameter tuning, modeling and all the way to final ML model evaluation
       [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
                           octopus_know_your_data.png]
 Check out the octopus-ml demo notebook on Colab [google_colab_logo] ##
 Installation The module can be easily installed with pip: ```conslole > pip
 install octopus-ml ``` This module depends on `Scikit-learn`, `NumPy`,
 `Pandas`, `TQDM`, `lightGBM` as defualt classifier. Optionally you can get also
 some nice visualisations if you have `Seaborn` installed. ## Usage The module
 contains ML and Data related methods: ```python from octopus_ml import
 plot_imp, adjusted_classes, cv, cv_plot, roc_curve_plot, ... ```
       [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
                                 oc_plot_cv.png]
 
       [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
                      oc_plot_prediction_distribution.png]
+## Selected visualizations:
+      [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
+                         target_distribution_plot.png]
+
+      [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
+                           histogram_on_target.png]
 
       [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
                                oc_plot_roc.png]
 
       [https://raw.githubusercontent.com/gershonc/octopus-ml/main/images/
                          oc_plot_confusion_matrix.png]
```

### Comparing `octopus-ml-3.0.0/setup.py` & `octopus-ml-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="octopus-ml",
-    version="3.0.0",
+    version="3.2.0",
     description="A collection of handy ML and data validation tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["octopus_ml"],
     author="Gershon Celniker",
     author_email="gershonc@gmail.com",
     url="https://github.com/gershonc/octopus-ml",
```

