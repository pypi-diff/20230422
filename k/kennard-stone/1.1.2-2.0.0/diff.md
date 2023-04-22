# Comparing `tmp/kennard_stone-1.1.2.tar.gz` & `tmp/kennard_stone-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kennard_stone-1.1.2.tar", last modified: Wed May 18 13:24:38 2022, max compression
+gzip compressed data, was "kennard_stone-2.0.0.tar", last modified: Sat Apr 22 05:18:59 2023, max compression
```

## Comparing `kennard_stone-1.1.2.tar` & `kennard_stone-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2022-05-18 13:24:38.253802 kennard_stone-1.1.2/
--rw-r--r--   0 yu9824     (501) staff       (20)     1063 2022-04-23 07:40:26.000000 kennard_stone-1.1.2/LICENSE
--rw-r--r--   0 yu9824     (501) staff       (20)       71 2022-04-23 07:40:26.000000 kennard_stone-1.1.2/MANIFEST.in
--rw-r--r--   0 yu9824     (501) staff       (20)     4585 2022-05-18 13:24:38.253664 kennard_stone-1.1.2/PKG-INFO
-drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2022-05-18 13:24:38.252764 kennard_stone-1.1.2/kennard_stone/
--rw-r--r--   0 yu9824     (501) staff       (20)      382 2022-05-18 13:22:02.000000 kennard_stone-1.1.2/kennard_stone/__init__.py
--rw-r--r--   0 yu9824     (501) staff       (20)      724 2022-04-23 10:33:40.000000 kennard_stone-1.1.2/kennard_stone/_test.py
--rw-r--r--   0 yu9824     (501) staff       (20)     8145 2021-08-11 09:41:55.000000 kennard_stone-1.1.2/kennard_stone/kennard_stone.py
-drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2022-05-18 13:24:38.253489 kennard_stone-1.1.2/kennard_stone.egg-info/
--rw-r--r--   0 yu9824     (501) staff       (20)     4585 2022-05-18 13:24:37.000000 kennard_stone-1.1.2/kennard_stone.egg-info/PKG-INFO
--rw-r--r--   0 yu9824     (501) staff       (20)      309 2022-05-18 13:24:38.000000 kennard_stone-1.1.2/kennard_stone.egg-info/SOURCES.txt
--rw-r--r--   0 yu9824     (501) staff       (20)        1 2022-05-18 13:24:38.000000 kennard_stone-1.1.2/kennard_stone.egg-info/dependency_links.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       26 2022-05-18 13:24:38.000000 kennard_stone-1.1.2/kennard_stone.egg-info/requires.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       14 2022-05-18 13:24:38.000000 kennard_stone-1.1.2/kennard_stone.egg-info/top_level.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       25 2022-04-23 07:40:26.000000 kennard_stone-1.1.2/requirements.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       38 2022-05-18 13:24:38.253851 kennard_stone-1.1.2/setup.cfg
--rw-r--r--   0 yu9824     (501) staff       (20)     6191 2022-05-18 13:22:02.000000 kennard_stone-1.1.2/setup.py
+drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-04-22 05:18:59.646309 kennard_stone-2.0.0/
+-rw-r--r--   0 yu9824     (501) staff       (20)     1063 2022-04-23 07:40:26.000000 kennard_stone-2.0.0/LICENSE
+-rw-r--r--   0 yu9824     (501) staff       (20)       71 2022-04-23 07:40:26.000000 kennard_stone-2.0.0/MANIFEST.in
+-rw-r--r--   0 yu9824     (501) staff       (20)     5461 2023-04-22 05:18:59.646162 kennard_stone-2.0.0/PKG-INFO
+drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-04-22 05:18:59.644975 kennard_stone-2.0.0/kennard_stone/
+-rw-r--r--   0 yu9824     (501) staff       (20)      360 2023-04-22 05:15:52.000000 kennard_stone-2.0.0/kennard_stone/__init__.py
+-rw-r--r--   0 yu9824     (501) staff       (20)     3160 2023-04-20 15:35:56.000000 kennard_stone-2.0.0/kennard_stone/_deprecated.py
+-rw-r--r--   0 yu9824     (501) staff       (20)     9586 2023-04-22 05:10:32.000000 kennard_stone-2.0.0/kennard_stone/kennard_stone.py
+drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-04-22 05:18:59.645939 kennard_stone-2.0.0/kennard_stone.egg-info/
+-rw-r--r--   0 yu9824     (501) staff       (20)     5461 2023-04-22 05:18:59.000000 kennard_stone-2.0.0/kennard_stone.egg-info/PKG-INFO
+-rw-r--r--   0 yu9824     (501) staff       (20)      315 2023-04-22 05:18:59.000000 kennard_stone-2.0.0/kennard_stone.egg-info/SOURCES.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)        1 2023-04-22 05:18:59.000000 kennard_stone-2.0.0/kennard_stone.egg-info/dependency_links.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       19 2023-04-22 05:18:59.000000 kennard_stone-2.0.0/kennard_stone.egg-info/requires.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       14 2023-04-22 05:18:59.000000 kennard_stone-2.0.0/kennard_stone.egg-info/top_level.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       19 2023-04-20 13:09:17.000000 kennard_stone-2.0.0/requirements.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       38 2023-04-22 05:18:59.646801 kennard_stone-2.0.0/setup.cfg
+-rw-r--r--   0 yu9824     (501) staff       (20)     2645 2023-04-22 04:08:08.000000 kennard_stone-2.0.0/setup.py
```

### Comparing `kennard_stone-1.1.2/LICENSE` & `kennard_stone-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kennard_stone-1.1.2/PKG-INFO` & `kennard_stone-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,119 +1,141 @@
 Metadata-Version: 2.1
 Name: kennard_stone
-Version: 1.1.2
+Version: 2.0.0
 Summary: A method for selecting samples by spreading the training data evenly.
 Home-page: https://github.com/yu9824/kennard_stone
 Author: yu9824
 Author-email: yu.9824.job@gmail.com
 Maintainer: yu9824
 Maintainer-email: yu.9824.job@gmail.com
 License: MIT
 Keywords: kennard_stone,scikit-learn,train_test_split,KFold
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Kennard Stone
 [![python_badge](https://img.shields.io/pypi/pyversions/kennard-stone)](https://pypi.org/project/kennard-stone/)
 [![license_badge](https://img.shields.io/pypi/l/kennard-stone)](https://pypi.org/project/kennard-stone/)
+[![PyPI version](https://badge.fury.io/py/kennard-stone.svg)](https://pypi.org/project/kennard-stone/)
 [![Downloads](https://pepy.tech/badge/kennard-stone)](https://pepy.tech/project/kennard-stone)
 
-[![Anaconda-Server Badge](https://anaconda.org/conda-forge/kennard-stone/badges/installer/conda.svg)](https://conda.anaconda.org/conda-forge)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/kennard-stone/badges/version.svg)](https://anaconda.org/conda-forge/kennard-stone)
+[![Anaconda-platform badge](https://anaconda.org/conda-forge/kennard-stone/badges/platforms.svg)](https://anaconda.org/conda-forge/kennard-stone)
+[![Anaconda-license badge](https://anaconda.org/conda-forge/kennard-stone/badges/license.svg)](https://anaconda.org/conda-forge/kennard-stone)
 
 ## What is this?
+
 This is an algorithm for evenly partitioning data in a `scikit-learn`-like interface. (See [References](#References) for details of the algorithm.)
 
 ![simulateion_gif](https://github.com/yu9824/kennard_stone/blob/main/example/simulate.gif?raw=true "Simulateion")
 
 ## How to install
 
 ### PyPI
 
 ```bash
 pip install kennard-stone
 ```
 
+The project site is [here](https://pypi.org/project/kennard-stone/).
+
 ### Anaconda
 
 ```bash
 conda install -c conda-forge kennard-stone
 ```
 
-You need `numpy`, `pandas` and `scikit-learn`.
+The project site is [here](https://anaconda.org/conda-forge/kennard-stone).
+
+You need `numpy` and `scikit-learn` to run.
 
 ## How to use
+
 You can use them like [scikit-learn](https://scikit-learn.org/stable/modules/classes.html#module-sklearn.model_selection).
 
 See [example](https://github.com/yu9824/kennard_stone/tree/main/example) for details.
 
 In the following, `X` denotes an arbitrary explanatory variable and `y` an arbitrary objective variable.
 And, `estimator` indicates an arbitrary prediction model that conforms to scikit-learn.
 
 ### train_test_split
+
 #### kennard_stone
+
 ```python
 from kennard_stone import train_test_split
 
-X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = 0.2)
+X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
 ```
 
 #### scikit-learn
+
 ```python
 from sklearn.model_selection import train_test_split
 
-X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = 0.2, random_state = 334)
+X_train, X_test, y_train, y_test = train_test_split(
+    X, y, test_size=0.2, random_state=334
+)
 ```
 
 ### KFold
+
 #### kennard_stone
+
 ```python
 from kennard_stone import KFold
 
-kf = KFold(n_splits = 5)
+# Always shuffled and uniquely determined for a data set.
+kf = KFold(n_splits=5)
 for i_train, i_test in kf.split(X, y):
     X_train = X[i_train]
     y_train = y[i_train]
     X_test = X[i_test]
     y_test = y[i_test]
 ```
 
 #### scikit-learn
+
 ```python
 from sklearn.model_selection import KFold
 
-kf = KFold(n_splits = 5, shuffle = True, random_state = 334)
+kf = KFold(n_splits=5, shuffle=True, random_state=334)
 for i_train, i_test in kf.split(X, y):
     X_train = X[i_train]
     y_train = y[i_train]
     X_test = X[i_test]
     y_test = y[i_test]
 ```
 
-### Others
+### Other usages
+
 If you ever specify `cv` in scikit-learn, you can assign `KFold` objects to it and apply it to various functions.
 
 An example is [`cross_validate`](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.cross_validate.html).
 
 #### kennard_stone
+
 ```python
 from kennard_stone import KFold
 from sklearn.model_selection import cross_validate
 
 kf = KFold(n_splits = 5)
 print(cross_validate(estimator, X, y, cv = kf))
 ```
 
 #### scikit-learn
+
 ```python
 from sklearn.model_selection import KFold
 from sklearn.model_selection import cross_validate
 
 kf = KFold(n_splits = 5, shuffle = True, random_state = 334)
 print(cross_validate(estimator, X, y, cv = kf))
 ```
@@ -121,26 +143,40 @@
 ```python
 from sklearn.model_selection import cross_validate
 
 print(cross_validate(estimator, X, y, cv = 5))
 ```
 
 
-## Points to note
+## Notes
+
 There is no notion of `random_state` or `shuffle` because the partitioning is determined uniquely for the dataset.
 If these arguments are included, they do not cause an error. They simply have no effect on the result. Please be careful.
 
-If you want to run the notebook in example directory, you will need to additionally download matplotlib, seaborn, tqdm, and jupyter other than the packages in requirements.txt.
+If you want to run the notebook in example directory, you will need to additionally download `pandas`, `matplotlib`, `seaborn`, `tqdm`, and `jupyter` other than the packages in requirements.txt.
 
 ## LICENSE
 
 MIT Licence
 
 Copyright (c) 2021 yu9824
 
 
 ## References
 ### Papers
+
 * R. W. Kennard & L. A. Stone (1969) Computer Aided Design of Experiments, Technometrics, 11:1, 137-148, DOI: [10.1080/00401706.1969.10490666](https://doi.org/10.1080/00401706.1969.10490666)
+
 ### Sites
-* [https://datachemeng.com/trainingtestdivision/](https://datachemeng.com/trainingtestdivision/)
+
+* [https://datachemeng.com/trainingtestdivision/](https://datachemeng.com/trainingtestdivision/) (Japanese site)
+
+
+## Histories
+
+### v2.0.0
+
+- Define Extended Kennard-Stone algorithm (multi-class) i.e. Improve KFold algorithm.
+- Delete `alternate` argument in `KFold`.
+- Delete requirements of `pandas`.
+
```

### Comparing `kennard_stone-1.1.2/kennard_stone.egg-info/PKG-INFO` & `kennard_stone-2.0.0/kennard_stone.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,119 +1,141 @@
 Metadata-Version: 2.1
 Name: kennard-stone
-Version: 1.1.2
+Version: 2.0.0
 Summary: A method for selecting samples by spreading the training data evenly.
 Home-page: https://github.com/yu9824/kennard_stone
 Author: yu9824
 Author-email: yu.9824.job@gmail.com
 Maintainer: yu9824
 Maintainer-email: yu.9824.job@gmail.com
 License: MIT
 Keywords: kennard_stone,scikit-learn,train_test_split,KFold
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Kennard Stone
 [![python_badge](https://img.shields.io/pypi/pyversions/kennard-stone)](https://pypi.org/project/kennard-stone/)
 [![license_badge](https://img.shields.io/pypi/l/kennard-stone)](https://pypi.org/project/kennard-stone/)
+[![PyPI version](https://badge.fury.io/py/kennard-stone.svg)](https://pypi.org/project/kennard-stone/)
 [![Downloads](https://pepy.tech/badge/kennard-stone)](https://pepy.tech/project/kennard-stone)
 
-[![Anaconda-Server Badge](https://anaconda.org/conda-forge/kennard-stone/badges/installer/conda.svg)](https://conda.anaconda.org/conda-forge)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/kennard-stone/badges/version.svg)](https://anaconda.org/conda-forge/kennard-stone)
+[![Anaconda-platform badge](https://anaconda.org/conda-forge/kennard-stone/badges/platforms.svg)](https://anaconda.org/conda-forge/kennard-stone)
+[![Anaconda-license badge](https://anaconda.org/conda-forge/kennard-stone/badges/license.svg)](https://anaconda.org/conda-forge/kennard-stone)
 
 ## What is this?
+
 This is an algorithm for evenly partitioning data in a `scikit-learn`-like interface. (See [References](#References) for details of the algorithm.)
 
 ![simulateion_gif](https://github.com/yu9824/kennard_stone/blob/main/example/simulate.gif?raw=true "Simulateion")
 
 ## How to install
 
 ### PyPI
 
 ```bash
 pip install kennard-stone
 ```
 
+The project site is [here](https://pypi.org/project/kennard-stone/).
+
 ### Anaconda
 
 ```bash
 conda install -c conda-forge kennard-stone
 ```
 
-You need `numpy`, `pandas` and `scikit-learn`.
+The project site is [here](https://anaconda.org/conda-forge/kennard-stone).
+
+You need `numpy` and `scikit-learn` to run.
 
 ## How to use
+
 You can use them like [scikit-learn](https://scikit-learn.org/stable/modules/classes.html#module-sklearn.model_selection).
 
 See [example](https://github.com/yu9824/kennard_stone/tree/main/example) for details.
 
 In the following, `X` denotes an arbitrary explanatory variable and `y` an arbitrary objective variable.
 And, `estimator` indicates an arbitrary prediction model that conforms to scikit-learn.
 
 ### train_test_split
+
 #### kennard_stone
+
 ```python
 from kennard_stone import train_test_split
 
-X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = 0.2)
+X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
 ```
 
 #### scikit-learn
+
 ```python
 from sklearn.model_selection import train_test_split
 
-X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = 0.2, random_state = 334)
+X_train, X_test, y_train, y_test = train_test_split(
+    X, y, test_size=0.2, random_state=334
+)
 ```
 
 ### KFold
+
 #### kennard_stone
+
 ```python
 from kennard_stone import KFold
 
-kf = KFold(n_splits = 5)
+# Always shuffled and uniquely determined for a data set.
+kf = KFold(n_splits=5)
 for i_train, i_test in kf.split(X, y):
     X_train = X[i_train]
     y_train = y[i_train]
     X_test = X[i_test]
     y_test = y[i_test]
 ```
 
 #### scikit-learn
+
 ```python
 from sklearn.model_selection import KFold
 
-kf = KFold(n_splits = 5, shuffle = True, random_state = 334)
+kf = KFold(n_splits=5, shuffle=True, random_state=334)
 for i_train, i_test in kf.split(X, y):
     X_train = X[i_train]
     y_train = y[i_train]
     X_test = X[i_test]
     y_test = y[i_test]
 ```
 
-### Others
+### Other usages
+
 If you ever specify `cv` in scikit-learn, you can assign `KFold` objects to it and apply it to various functions.
 
 An example is [`cross_validate`](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.cross_validate.html).
 
 #### kennard_stone
+
 ```python
 from kennard_stone import KFold
 from sklearn.model_selection import cross_validate
 
 kf = KFold(n_splits = 5)
 print(cross_validate(estimator, X, y, cv = kf))
 ```
 
 #### scikit-learn
+
 ```python
 from sklearn.model_selection import KFold
 from sklearn.model_selection import cross_validate
 
 kf = KFold(n_splits = 5, shuffle = True, random_state = 334)
 print(cross_validate(estimator, X, y, cv = kf))
 ```
@@ -121,26 +143,40 @@
 ```python
 from sklearn.model_selection import cross_validate
 
 print(cross_validate(estimator, X, y, cv = 5))
 ```
 
 
-## Points to note
+## Notes
+
 There is no notion of `random_state` or `shuffle` because the partitioning is determined uniquely for the dataset.
 If these arguments are included, they do not cause an error. They simply have no effect on the result. Please be careful.
 
-If you want to run the notebook in example directory, you will need to additionally download matplotlib, seaborn, tqdm, and jupyter other than the packages in requirements.txt.
+If you want to run the notebook in example directory, you will need to additionally download `pandas`, `matplotlib`, `seaborn`, `tqdm`, and `jupyter` other than the packages in requirements.txt.
 
 ## LICENSE
 
 MIT Licence
 
 Copyright (c) 2021 yu9824
 
 
 ## References
 ### Papers
+
 * R. W. Kennard & L. A. Stone (1969) Computer Aided Design of Experiments, Technometrics, 11:1, 137-148, DOI: [10.1080/00401706.1969.10490666](https://doi.org/10.1080/00401706.1969.10490666)
+
 ### Sites
-* [https://datachemeng.com/trainingtestdivision/](https://datachemeng.com/trainingtestdivision/)
+
+* [https://datachemeng.com/trainingtestdivision/](https://datachemeng.com/trainingtestdivision/) (Japanese site)
+
+
+## Histories
+
+### v2.0.0
+
+- Define Extended Kennard-Stone algorithm (multi-class) i.e. Improve KFold algorithm.
+- Delete `alternate` argument in `KFold`.
+- Delete requirements of `pandas`.
+
```

