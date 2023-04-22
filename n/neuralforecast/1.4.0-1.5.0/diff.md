# Comparing `tmp/neuralforecast-1.4.0.tar.gz` & `tmp/neuralforecast-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralforecast-1.4.0.tar", last modified: Tue Feb 14 22:26:33 2023, max compression
+gzip compressed data, was "neuralforecast-1.5.0.tar", last modified: Sat Apr 22 19:28:50 2023, max compression
```

## Comparing `neuralforecast-1.4.0.tar` & `neuralforecast-1.5.0.tar`

### file list

```diff
@@ -1,46 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 22:26:33.237479 neuralforecast-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-02-14 22:26:33.237479 neuralforecast-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 22:26:33.233478 neuralforecast-1.4.0/neuralforecast/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68621 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)    17871 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 22:26:33.233478 neuralforecast-1.4.0/neuralforecast/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/common/_base_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)    23224 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/common/_base_recurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    24402 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/common/_base_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/common/_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/common/_scalers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22310 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 22:26:33.233478 neuralforecast-1.4.0/neuralforecast/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15633 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/losses/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    66878 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/losses/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 22:26:33.237479 neuralforecast-1.4.0/neuralforecast/models/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/models/dilated_rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/models/gru.py
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/models/lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/models/nbeats.py
--rw-r--r--   0 runner    (1001) docker     (123)    19213 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/models/nbeatsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/models/nhits.py
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/models/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/models/tcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    28040 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/models/tft.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/tsdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/neuralforecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 22:26:33.233478 neuralforecast-1.4.0/neuralforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-02-14 22:26:33.000000 neuralforecast-1.4.0/neuralforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-02-14 22:26:33.000000 neuralforecast-1.4.0/neuralforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 22:26:33.000000 neuralforecast-1.4.0/neuralforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-14 22:26:33.000000 neuralforecast-1.4.0/neuralforecast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 22:26:33.000000 neuralforecast-1.4.0/neuralforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-14 22:26:33.000000 neuralforecast-1.4.0/neuralforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-14 22:26:33.000000 neuralforecast-1.4.0/neuralforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 22:26:33.237479 neuralforecast-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-02-14 22:26:19.000000 neuralforecast-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:50.670371 neuralforecast-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-04-22 19:28:50.670371 neuralforecast-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:50.662371 neuralforecast-1.5.0/neuralforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111564 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28950 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:50.666370 neuralforecast-1.5.0/neuralforecast/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/common/_base_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24293 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/common/_base_multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25497 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/common/_base_recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26826 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/common/_base_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/common/_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14762 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/common/_scalers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28117 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:50.666370 neuralforecast-1.5.0/neuralforecast/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15633 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/losses/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70389 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/losses/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:50.670371 neuralforecast-1.5.0/neuralforecast/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25546 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/autoformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/dilated_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/gru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16078 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/informer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/nbeats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19321 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/nbeatsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/nhits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35403 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/patchtst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/stemgnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/tcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28684 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/tft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/models/vanillatransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/tsdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/neuralforecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:28:50.666370 neuralforecast-1.5.0/neuralforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-04-22 19:28:50.000000 neuralforecast-1.5.0/neuralforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-22 19:28:50.000000 neuralforecast-1.5.0/neuralforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:28:50.000000 neuralforecast-1.5.0/neuralforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-22 19:28:50.000000 neuralforecast-1.5.0/neuralforecast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:28:50.000000 neuralforecast-1.5.0/neuralforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-22 19:28:50.000000 neuralforecast-1.5.0/neuralforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-22 19:28:50.000000 neuralforecast-1.5.0/neuralforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 19:28:50.670371 neuralforecast-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-22 19:28:40.000000 neuralforecast-1.5.0/setup.py
```

### Comparing `neuralforecast-1.4.0/LICENSE` & `neuralforecast-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.4.0/PKG-INFO` & `neuralforecast-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: neuralforecast
-Version: 1.4.0
+Version: 1.5.0
 Summary: Time series forecasting suite using deep learning models
 Home-page: https://github.com/Nixtla/neuralforecast/
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series forecasting deep-learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# Nixtla &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/neuralforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting) &nbsp;[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlaworkspace/shared_invite/zt-135dssye9-fWTzMpv2WBthq8NK0Yvu6A)
+# Nixtla &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/neuralforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting) &nbsp;[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 
 <div align="center">
 <!--- <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast1/main/nbs/imgs_indx/logo_mid.png"> --->
 <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png">
 <h1 align="center">Neural 🧠 Forecast</h1>
 <h3 align="center">User friendly state-of-the-art neural forecasting models.</h3>
 
@@ -71,15 +70,15 @@
 git clone https://github.com/Nixtla/neuralforecast.git
 cd neuralforecast
 pip install -e .
 ```
 </details>
 
 ## 🏃🏻‍♀️🏃 Getting Started
-To get started follow this [guide](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/Getting_Started_with_NBEATS_and_NHITS.ipynb), where we explore `NBEATS`, extend it towards probabilistic predictions and exogenous variables.
+To get started follow this [guide](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/Getting_Started.ipynb), where we explore `NBEATS`, extend it towards probabilistic predictions and exogenous variables.
 
 Or follow this simple example where we train the `NBEATS` model and predict the classic Box-Jenkins air passengers dataset.
 ```python
 import numpy as np
 import pandas as pd
 from IPython.display import display, Markdown
 
@@ -89,21 +88,21 @@
 from neuralforecast.utils import AirPassengersDF
 
 # Split data and declare panel dataset
 Y_df = AirPassengersDF
 Y_train_df = Y_df[Y_df.ds<='1959-12-31'] # 132 train
 Y_test_df = Y_df[Y_df.ds>'1959-12-31'] # 12 test
 
-# Fit and predict with N-BEATS and N-HiTS models
+# Fit and predict with NBEATS and NHITS models
 horizon = len(Y_test_df)
 models = [NBEATS(input_size=2 * horizon, h=horizon, max_epochs=50),
           NHITS(input_size=2 * horizon, h=horizon, max_epochs=50)]
-nforecast = NeuralForecast(models=models, freq='M')
-nforecast.fit(df=Y_train_df)
-Y_hat_df = nforecast.predict().reset_index()
+nf = NeuralForecast(models=models, freq='M')
+nf.fit(df=Y_train_df)
+Y_hat_df = nf.predict().reset_index()
 
 # Plot predictions
 fig, ax = plt.subplots(1, 1, figsize = (20, 7))
 Y_hat_df = Y_test_df.merge(Y_hat_df, how='left', on=['unique_id', 'ds'])
 plot_df = pd.concat([Y_train_df, Y_hat_df]).set_index('ds')
 
 plot_df[['y', 'NBEATS', 'NHITS']].plot(ax=ax, linewidth=2)
@@ -113,50 +112,51 @@
 ax.set_xlabel('Timestamp [t]', fontsize=20)
 ax.legend(prop={'size': 15})
 ax.grid()
 ```
 <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/nbeats_example.png">
 
 ## 🎉 New!
-* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/Getting_Started_with_NBEATS_and_NHITS.ipynb) **Quick Start**: Minimal usage example of the NeuralForecast library on Box's AirPassengers Data.
+* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/Getting_Started.ipynb) **Quick Start**: Minimal usage example of the NeuralForecast library on Box's AirPassengers Data.
 * [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/UncertaintyIntervals.ipynb) **Multi Quantile NBEATS Example**: Produce accurate and efficient probabilistic forecasts in long-horizon settings. Outperforming AutoARIMA's accuracy in a fraction of the time.
-* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/LongHorizon_with_NHITS.ipynb) **Long Horizon N-HiTS Example**:  Load, train, and tune hyperparameters, to achieve Long-Horizon SoTA. Outperform Award Winning Transformers by 25% in 50x less time.
+* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/LongHorizon_with_NHITS.ipynb) **Long Horizon NHITS Example**:  Load, train, and tune hyperparameters, to achieve Long-Horizon SoTA. Outperform Award Winning Transformers by 25% in 50x less time.
+* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/HierarchicalNetworks.ipynb) **Hierarchical Forecasting HINT Example**:  Obtain accurate probabilistic coherent predictions for hierarchical datasets.
 
 ## 🔥  Highlights
 
 * Unified `StatsForecast` interface `NeuralForecast().fit(Y_df).predict(h=7)`.
 * Industry/Competition proven `ESRNN`, `NBEATS`, and `TFT` implementations.
 * Improve accuracy and speed over classic `ARIMA`/`ETS` in two lines of code. Check the experiments [here](xXmissingXx).
-* Predict Series with little to no history, using Transfer learning. Check the experiments [here](xXmissingXx).
+* Predict Series with little to no history, using Transfer learning. Check the experiments [here](https://github.com/Nixtla/transfer-learning-time-series).
 
 ## 🎊 Features 
 
 * **Exogenous Variables**: Static, lagged and future exogenous support.
 * **Forecast Interpretability**: Plot trend, seasonality and exogenous `NBEATS`, `NHITS`, `TFT`, `ESRNN` prediction components.
 * **Probabilistic Forecasting**: Simple model adapters for quantile losses and parametric distributions.
 * **Train and Evaluation Losses** Scale-dependent, percentage and scale independent errors, and parametric likelihoods.
 * **Automatic Model Selection** Parallelized automatic hyperparameter tuning, that efficiently searches best validation configuration.
 * **Simple Interface** Unified SKLearn Interface for `StatsForecast` and `MLForecast` compatibility.
-* **Model Collection**: Out of the box implementation of `MLP`, `LSTM`, `RNN`, `TCN`, `DilatedRNN`, `NBEATS`, `NHITS`, `ESRNN`, `AutoFormer`, `Informer`, `TFT`, `AutoFormer`, `Informer`, and vanilla `Transformer`. See the entire [collection here](https://nixtla.github.io/neuralforecast/models.html).
+* **Model Collection**: Out of the box implementation of `MLP`, `LSTM`, `RNN`, `TCN`, `DilatedRNN`, `NBEATS`, `NHITS`, `ESRNN`, `TFT`, `Informer`, `PatchTST` and `HINT`. See the entire [collection here](https://nixtla.github.io/neuralforecast/models.html).
 
 Missing something? Please open an issue or write us in [![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlaworkspace/shared_invite/zt-135dssye9-fWTzMpv2WBthq8NK0Yvu6A)
 
 ## 📖 Why? 
 
 There is a shared belief in Neural forecasting methods' capacity to improve our pipeline's accuracy and efficiency.
 
 Unfortunately, available implementations and published research are yet to realize neural networks' potential. They are hard to use and continuously fail to improve over statistical methods while being computationally prohibitive. For this reason, we created `NeuralForecast`, a library favoring proven accurate and efficient models focusing on their usability.
 
 ## 🔬 Accuracy & ⏲ Speed 
 
 ### Industry/Competition Proven Methods
-An extensive empirical evaluation is critical to generate confidence and promote the adoption and development of novel methods. For this reason, we replicate and verify the results of our implementation of the following industry/competition-proven methods: `ESRNN`, `NBEATS`, `NHITS`, and `TFT`. If you are interested in reproducing the results, check the experiments [here](xXmissingXx).
+An extensive empirical evaluation is critical to generate confidence and promote the adoption and development of novel methods. For this reason, we replicate and verify the results of our implementation of the following industry/competition-proven methods: `ESRNN`, `NBEATS`, `NHITS`, and `TFT`. If you are interested in reproducing the results, check the experiments [here](https://github.com/Nixtla/neuralforecast/blob/main/nbs/experiments/).
 
 ### Simple and Efficient Method's Comparison
-Like `core.StatsForecast`, the `core.NeuralForecast` wrapper class allows us to easily compare any model in the collection to select or ensemble the best performing methods. Aditionally it offers a high-end interface that operates with (potentially large) sets of time series data stored in pandas DataFrames. The `core.NeuralForecast` efficiently parallelizes computation across CPU or GPU resources. Check the experiments [here](xXmissingXx).
+Like `core.StatsForecast`, the `core.NeuralForecast` wrapper class allows us to easily compare any model in the collection to select or ensemble the best performing methods. Aditionally it offers a high-end interface that operates with (potentially large) sets of time series data stored in pandas DataFrames. The `core.NeuralForecast` efficiently parallelizes computation across GPU resources. Check the experiments [here](https://github.com/Nixtla/neuralforecast/blob/main/nbs/examples/Getting_Started_complete.ipynb).
 
 ## 📖 Documentation (WIP)
 The [documentation page](https://nixtla.github.io/neuralforecast/) contains the models' code documentation, methods, utils, and other tutorials. Docstrings accompany most code.
 
 ## 🔨 How to contribute
 If you wish to contribute to the project, please refer to our [contribution guidelines](https://github.com/Nixtla/neuralforecast/blob/main/CONTRIBUTING.md).
```

### Comparing `neuralforecast-1.4.0/README.md` & `neuralforecast-1.5.0/neuralforecast.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,29 @@
-# Nixtla &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/neuralforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting) &nbsp;[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlaworkspace/shared_invite/zt-135dssye9-fWTzMpv2WBthq8NK0Yvu6A)
+Metadata-Version: 2.1
+Name: neuralforecast
+Version: 1.5.0
+Summary: Time series forecasting suite using deep learning models
+Home-page: https://github.com/Nixtla/neuralforecast/
+Author: Nixtla
+Author-email: business@nixtla.io
+License: Apache Software License 2.0
+Keywords: time-series forecasting deep-learning
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# Nixtla &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/neuralforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting) &nbsp;[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 
 <div align="center">
 <!--- <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast1/main/nbs/imgs_indx/logo_mid.png"> --->
 <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png">
 <h1 align="center">Neural 🧠 Forecast</h1>
 <h3 align="center">User friendly state-of-the-art neural forecasting models.</h3>
 
@@ -49,15 +70,15 @@
 git clone https://github.com/Nixtla/neuralforecast.git
 cd neuralforecast
 pip install -e .
 ```
 </details>
 
 ## 🏃🏻‍♀️🏃 Getting Started
-To get started follow this [guide](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/Getting_Started_with_NBEATS_and_NHITS.ipynb), where we explore `NBEATS`, extend it towards probabilistic predictions and exogenous variables.
+To get started follow this [guide](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/Getting_Started.ipynb), where we explore `NBEATS`, extend it towards probabilistic predictions and exogenous variables.
 
 Or follow this simple example where we train the `NBEATS` model and predict the classic Box-Jenkins air passengers dataset.
 ```python
 import numpy as np
 import pandas as pd
 from IPython.display import display, Markdown
 
@@ -67,21 +88,21 @@
 from neuralforecast.utils import AirPassengersDF
 
 # Split data and declare panel dataset
 Y_df = AirPassengersDF
 Y_train_df = Y_df[Y_df.ds<='1959-12-31'] # 132 train
 Y_test_df = Y_df[Y_df.ds>'1959-12-31'] # 12 test
 
-# Fit and predict with N-BEATS and N-HiTS models
+# Fit and predict with NBEATS and NHITS models
 horizon = len(Y_test_df)
 models = [NBEATS(input_size=2 * horizon, h=horizon, max_epochs=50),
           NHITS(input_size=2 * horizon, h=horizon, max_epochs=50)]
-nforecast = NeuralForecast(models=models, freq='M')
-nforecast.fit(df=Y_train_df)
-Y_hat_df = nforecast.predict().reset_index()
+nf = NeuralForecast(models=models, freq='M')
+nf.fit(df=Y_train_df)
+Y_hat_df = nf.predict().reset_index()
 
 # Plot predictions
 fig, ax = plt.subplots(1, 1, figsize = (20, 7))
 Y_hat_df = Y_test_df.merge(Y_hat_df, how='left', on=['unique_id', 'ds'])
 plot_df = pd.concat([Y_train_df, Y_hat_df]).set_index('ds')
 
 plot_df[['y', 'NBEATS', 'NHITS']].plot(ax=ax, linewidth=2)
@@ -91,50 +112,51 @@
 ax.set_xlabel('Timestamp [t]', fontsize=20)
 ax.legend(prop={'size': 15})
 ax.grid()
 ```
 <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/nbeats_example.png">
 
 ## 🎉 New!
-* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/Getting_Started_with_NBEATS_and_NHITS.ipynb) **Quick Start**: Minimal usage example of the NeuralForecast library on Box's AirPassengers Data.
+* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/Getting_Started.ipynb) **Quick Start**: Minimal usage example of the NeuralForecast library on Box's AirPassengers Data.
 * [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/UncertaintyIntervals.ipynb) **Multi Quantile NBEATS Example**: Produce accurate and efficient probabilistic forecasts in long-horizon settings. Outperforming AutoARIMA's accuracy in a fraction of the time.
-* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/LongHorizon_with_NHITS.ipynb) **Long Horizon N-HiTS Example**:  Load, train, and tune hyperparameters, to achieve Long-Horizon SoTA. Outperform Award Winning Transformers by 25% in 50x less time.
+* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/LongHorizon_with_NHITS.ipynb) **Long Horizon NHITS Example**:  Load, train, and tune hyperparameters, to achieve Long-Horizon SoTA. Outperform Award Winning Transformers by 25% in 50x less time.
+* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/HierarchicalNetworks.ipynb) **Hierarchical Forecasting HINT Example**:  Obtain accurate probabilistic coherent predictions for hierarchical datasets.
 
 ## 🔥  Highlights
 
 * Unified `StatsForecast` interface `NeuralForecast().fit(Y_df).predict(h=7)`.
 * Industry/Competition proven `ESRNN`, `NBEATS`, and `TFT` implementations.
 * Improve accuracy and speed over classic `ARIMA`/`ETS` in two lines of code. Check the experiments [here](xXmissingXx).
-* Predict Series with little to no history, using Transfer learning. Check the experiments [here](xXmissingXx).
+* Predict Series with little to no history, using Transfer learning. Check the experiments [here](https://github.com/Nixtla/transfer-learning-time-series).
 
 ## 🎊 Features 
 
 * **Exogenous Variables**: Static, lagged and future exogenous support.
 * **Forecast Interpretability**: Plot trend, seasonality and exogenous `NBEATS`, `NHITS`, `TFT`, `ESRNN` prediction components.
 * **Probabilistic Forecasting**: Simple model adapters for quantile losses and parametric distributions.
 * **Train and Evaluation Losses** Scale-dependent, percentage and scale independent errors, and parametric likelihoods.
 * **Automatic Model Selection** Parallelized automatic hyperparameter tuning, that efficiently searches best validation configuration.
 * **Simple Interface** Unified SKLearn Interface for `StatsForecast` and `MLForecast` compatibility.
-* **Model Collection**: Out of the box implementation of `MLP`, `LSTM`, `RNN`, `TCN`, `DilatedRNN`, `NBEATS`, `NHITS`, `ESRNN`, `AutoFormer`, `Informer`, `TFT`, `AutoFormer`, `Informer`, and vanilla `Transformer`. See the entire [collection here](https://nixtla.github.io/neuralforecast/models.html).
+* **Model Collection**: Out of the box implementation of `MLP`, `LSTM`, `RNN`, `TCN`, `DilatedRNN`, `NBEATS`, `NHITS`, `ESRNN`, `TFT`, `Informer`, `PatchTST` and `HINT`. See the entire [collection here](https://nixtla.github.io/neuralforecast/models.html).
 
 Missing something? Please open an issue or write us in [![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlaworkspace/shared_invite/zt-135dssye9-fWTzMpv2WBthq8NK0Yvu6A)
 
 ## 📖 Why? 
 
 There is a shared belief in Neural forecasting methods' capacity to improve our pipeline's accuracy and efficiency.
 
 Unfortunately, available implementations and published research are yet to realize neural networks' potential. They are hard to use and continuously fail to improve over statistical methods while being computationally prohibitive. For this reason, we created `NeuralForecast`, a library favoring proven accurate and efficient models focusing on their usability.
 
 ## 🔬 Accuracy & ⏲ Speed 
 
 ### Industry/Competition Proven Methods
-An extensive empirical evaluation is critical to generate confidence and promote the adoption and development of novel methods. For this reason, we replicate and verify the results of our implementation of the following industry/competition-proven methods: `ESRNN`, `NBEATS`, `NHITS`, and `TFT`. If you are interested in reproducing the results, check the experiments [here](xXmissingXx).
+An extensive empirical evaluation is critical to generate confidence and promote the adoption and development of novel methods. For this reason, we replicate and verify the results of our implementation of the following industry/competition-proven methods: `ESRNN`, `NBEATS`, `NHITS`, and `TFT`. If you are interested in reproducing the results, check the experiments [here](https://github.com/Nixtla/neuralforecast/blob/main/nbs/experiments/).
 
 ### Simple and Efficient Method's Comparison
-Like `core.StatsForecast`, the `core.NeuralForecast` wrapper class allows us to easily compare any model in the collection to select or ensemble the best performing methods. Aditionally it offers a high-end interface that operates with (potentially large) sets of time series data stored in pandas DataFrames. The `core.NeuralForecast` efficiently parallelizes computation across CPU or GPU resources. Check the experiments [here](xXmissingXx).
+Like `core.StatsForecast`, the `core.NeuralForecast` wrapper class allows us to easily compare any model in the collection to select or ensemble the best performing methods. Aditionally it offers a high-end interface that operates with (potentially large) sets of time series data stored in pandas DataFrames. The `core.NeuralForecast` efficiently parallelizes computation across GPU resources. Check the experiments [here](https://github.com/Nixtla/neuralforecast/blob/main/nbs/examples/Getting_Started_complete.ipynb).
 
 ## 📖 Documentation (WIP)
 The [documentation page](https://nixtla.github.io/neuralforecast/) contains the models' code documentation, methods, utils, and other tutorials. Docstrings accompany most code.
 
 ## 🔨 How to contribute
 If you wish to contribute to the project, please refer to our [contribution guidelines](https://github.com/Nixtla/neuralforecast/blob/main/CONTRIBUTING.md).
```

### Comparing `neuralforecast-1.4.0/neuralforecast/_modidx.py` & `neuralforecast-1.5.0/neuralforecast/_modidx.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,72 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/neuralforecast/',
                 'doc_host': 'https://Nixtla.github.io',
                 'git_url': 'https://github.com/Nixtla/neuralforecast/',
                 'lib_path': 'neuralforecast'},
-  'syms': { 'neuralforecast.auto': { 'neuralforecast.auto.AutoDilatedRNN': ('models.html#autodilatedrnn', 'neuralforecast/auto.py'),
+  'syms': { 'neuralforecast.auto': { 'neuralforecast.auto.AutoAutoformer': ('models.html#autoautoformer', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoAutoformer.__init__': ( 'models.html#autoautoformer.__init__',
+                                                                                      'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoDilatedRNN': ('models.html#autodilatedrnn', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDilatedRNN.__init__': ( 'models.html#autodilatedrnn.__init__',
                                                                                       'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoGRU': ('models.html#autogru', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoGRU.__init__': ('models.html#autogru.__init__', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoInformer': ('models.html#autoinformer', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoInformer.__init__': ( 'models.html#autoinformer.__init__',
+                                                                                    'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoLSTM': ('models.html#autolstm', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoLSTM.__init__': ('models.html#autolstm.__init__', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoMLP': ('models.html#automlp', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoMLP.__init__': ('models.html#automlp.__init__', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoNBEATS': ('models.html#autonbeats', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoNBEATS.__init__': ( 'models.html#autonbeats.__init__',
                                                                                   'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoNBEATSx': ('models.html#autonbeatsx', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoNBEATSx.__init__': ( 'models.html#autonbeatsx.__init__',
                                                                                    'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoNHITS': ('models.html#autonhits', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoNHITS.__init__': ('models.html#autonhits.__init__', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoPatchTST': ('models.html#autopatchtst', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoPatchTST.__init__': ( 'models.html#autopatchtst.__init__',
+                                                                                    'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoRNN': ('models.html#autornn', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoRNN.__init__': ('models.html#autornn.__init__', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoStemGNN': ('models.html#autostemgnn', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoStemGNN.__init__': ( 'models.html#autostemgnn.__init__',
+                                                                                   'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoTCN': ('models.html#autotcn', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoTCN.__init__': ('models.html#autotcn.__init__', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoTFT': ('models.html#autotft', 'neuralforecast/auto.py'),
-                                     'neuralforecast.auto.AutoTFT.__init__': ('models.html#autotft.__init__', 'neuralforecast/auto.py')},
+                                     'neuralforecast.auto.AutoTFT.__init__': ('models.html#autotft.__init__', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoVanillaTransformer': ( 'models.html#autovanillatransformer',
+                                                                                     'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoVanillaTransformer.__init__': ( 'models.html#autovanillatransformer.__init__',
+                                                                                              'neuralforecast/auto.py')},
             'neuralforecast.core': { 'neuralforecast.core.NeuralForecast': ('core.html#neuralforecast', 'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast.__init__': ( 'core.html#neuralforecast.__init__',
                                                                                       'neuralforecast/core.py'),
-                                     'neuralforecast.core.NeuralForecast._make_future_df': ( 'core.html#neuralforecast._make_future_df',
-                                                                                             'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast._prepare_fit': ( 'core.html#neuralforecast._prepare_fit',
                                                                                           'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast.cross_validation': ( 'core.html#neuralforecast.cross_validation',
                                                                                               'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast.fit': ('core.html#neuralforecast.fit', 'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast.load': ('core.html#neuralforecast.load', 'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast.predict': ( 'core.html#neuralforecast.predict',
                                                                                      'neuralforecast/core.py'),
+                                     'neuralforecast.core.NeuralForecast.predict_insample': ( 'core.html#neuralforecast.predict_insample',
+                                                                                              'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast.predict_rolled': ( 'core.html#neuralforecast.predict_rolled',
                                                                                             'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast.save': ('core.html#neuralforecast.save', 'neuralforecast/core.py'),
-                                     'neuralforecast.core._cv_dates': ('core.html#_cv_dates', 'neuralforecast/core.py')},
+                                     'neuralforecast.core._cv_dates': ('core.html#_cv_dates', 'neuralforecast/core.py'),
+                                     'neuralforecast.core._future_dates': ('core.html#_future_dates', 'neuralforecast/core.py'),
+                                     'neuralforecast.core._insample_dates': ('core.html#_insample_dates', 'neuralforecast/core.py')},
             'neuralforecast.losses.numpy': { 'neuralforecast.losses.numpy._divide_no_nan': ( 'losses.numpy.html#_divide_no_nan',
                                                                                              'neuralforecast/losses/numpy.py'),
                                              'neuralforecast.losses.numpy._metric_protections': ( 'losses.numpy.html#_metric_protections',
                                                                                                   'neuralforecast/losses/numpy.py'),
                                              'neuralforecast.losses.numpy.mae': ('losses.numpy.html#mae', 'neuralforecast/losses/numpy.py'),
                                              'neuralforecast.losses.numpy.mape': ( 'losses.numpy.html#mape',
                                                                                    'neuralforecast/losses/numpy.py'),
@@ -225,14 +243,20 @@
                                                                                                         'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.poisson_domain_map': ( 'losses.pytorch.html#poisson_domain_map',
                                                                                                      'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.poisson_scale_decouple': ( 'losses.pytorch.html#poisson_scale_decouple',
                                                                                                          'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.quantiles_to_outputs': ( 'losses.pytorch.html#quantiles_to_outputs',
                                                                                                        'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.relMSE': ( 'losses.pytorch.html#relmse',
+                                                                                         'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.relMSE.__call__': ( 'losses.pytorch.html#relmse.__call__',
+                                                                                                  'neuralforecast/losses/pytorch.py'),
+                                               'neuralforecast.losses.pytorch.relMSE.__init__': ( 'losses.pytorch.html#relmse.__init__',
+                                                                                                  'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.sCRPS': ( 'losses.pytorch.html#scrps',
                                                                                         'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.sCRPS.__call__': ( 'losses.pytorch.html#scrps.__call__',
                                                                                                  'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.sCRPS.__init__': ( 'losses.pytorch.html#scrps.__init__',
                                                                                                  'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.student_domain_map': ( 'losses.pytorch.html#student_domain_map',
@@ -249,14 +273,80 @@
                                                                                                    'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.wMQLoss.__init__': ( 'losses.pytorch.html#wmqloss.__init__',
                                                                                                    'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.wMQLoss.domain_map': ( 'losses.pytorch.html#wmqloss.domain_map',
                                                                                                      'neuralforecast/losses/pytorch.py'),
                                                'neuralforecast.losses.pytorch.weighted_average': ( 'losses.pytorch.html#weighted_average',
                                                                                                    'neuralforecast/losses/pytorch.py')},
+            'neuralforecast.models.autoformer': { 'neuralforecast.models.autoformer.AutoCorrelation': ( 'models.autoformer.html#autocorrelation',
+                                                                                                        'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.AutoCorrelation.__init__': ( 'models.autoformer.html#autocorrelation.__init__',
+                                                                                                                 'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.AutoCorrelation.forward': ( 'models.autoformer.html#autocorrelation.forward',
+                                                                                                                'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.AutoCorrelation.time_delay_agg_full': ( 'models.autoformer.html#autocorrelation.time_delay_agg_full',
+                                                                                                                            'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.AutoCorrelation.time_delay_agg_inference': ( 'models.autoformer.html#autocorrelation.time_delay_agg_inference',
+                                                                                                                                 'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.AutoCorrelation.time_delay_agg_training': ( 'models.autoformer.html#autocorrelation.time_delay_agg_training',
+                                                                                                                                'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.AutoCorrelationLayer': ( 'models.autoformer.html#autocorrelationlayer',
+                                                                                                             'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.AutoCorrelationLayer.__init__': ( 'models.autoformer.html#autocorrelationlayer.__init__',
+                                                                                                                      'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.AutoCorrelationLayer.forward': ( 'models.autoformer.html#autocorrelationlayer.forward',
+                                                                                                                     'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.Autoformer': ( 'models.autoformer.html#autoformer',
+                                                                                                   'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.Autoformer.__init__': ( 'models.autoformer.html#autoformer.__init__',
+                                                                                                            'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.Autoformer.forward': ( 'models.autoformer.html#autoformer.forward',
+                                                                                                           'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.Decoder': ( 'models.autoformer.html#decoder',
+                                                                                                'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.Decoder.__init__': ( 'models.autoformer.html#decoder.__init__',
+                                                                                                         'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.Decoder.forward': ( 'models.autoformer.html#decoder.forward',
+                                                                                                        'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.DecoderLayer': ( 'models.autoformer.html#decoderlayer',
+                                                                                                     'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.DecoderLayer.__init__': ( 'models.autoformer.html#decoderlayer.__init__',
+                                                                                                              'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.DecoderLayer.forward': ( 'models.autoformer.html#decoderlayer.forward',
+                                                                                                             'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.Encoder': ( 'models.autoformer.html#encoder',
+                                                                                                'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.Encoder.__init__': ( 'models.autoformer.html#encoder.__init__',
+                                                                                                         'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.Encoder.forward': ( 'models.autoformer.html#encoder.forward',
+                                                                                                        'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.EncoderLayer': ( 'models.autoformer.html#encoderlayer',
+                                                                                                     'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.EncoderLayer.__init__': ( 'models.autoformer.html#encoderlayer.__init__',
+                                                                                                              'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.EncoderLayer.forward': ( 'models.autoformer.html#encoderlayer.forward',
+                                                                                                             'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.LayerNorm': ( 'models.autoformer.html#layernorm',
+                                                                                                  'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.LayerNorm.__init__': ( 'models.autoformer.html#layernorm.__init__',
+                                                                                                           'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.LayerNorm.forward': ( 'models.autoformer.html#layernorm.forward',
+                                                                                                          'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.MovingAvg': ( 'models.autoformer.html#movingavg',
+                                                                                                  'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.MovingAvg.__init__': ( 'models.autoformer.html#movingavg.__init__',
+                                                                                                           'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.MovingAvg.forward': ( 'models.autoformer.html#movingavg.forward',
+                                                                                                          'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.SeriesDecomp': ( 'models.autoformer.html#seriesdecomp',
+                                                                                                     'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.SeriesDecomp.__init__': ( 'models.autoformer.html#seriesdecomp.__init__',
+                                                                                                              'neuralforecast/models/autoformer.py'),
+                                                  'neuralforecast.models.autoformer.SeriesDecomp.forward': ( 'models.autoformer.html#seriesdecomp.forward',
+                                                                                                             'neuralforecast/models/autoformer.py')},
             'neuralforecast.models.dilated_rnn': { 'neuralforecast.models.dilated_rnn.AttentiveLSTMLayer': ( 'models.dilated_rnn.html#attentivelstmlayer',
                                                                                                              'neuralforecast/models/dilated_rnn.py'),
                                                    'neuralforecast.models.dilated_rnn.AttentiveLSTMLayer.__init__': ( 'models.dilated_rnn.html#attentivelstmlayer.__init__',
                                                                                                                       'neuralforecast/models/dilated_rnn.py'),
                                                    'neuralforecast.models.dilated_rnn.AttentiveLSTMLayer.forward': ( 'models.dilated_rnn.html#attentivelstmlayer.forward',
                                                                                                                      'neuralforecast/models/dilated_rnn.py'),
                                                    'neuralforecast.models.dilated_rnn.DRNN': ( 'models.dilated_rnn.html#drnn',
@@ -302,14 +392,63 @@
                                                    'neuralforecast.models.dilated_rnn.ResLSTMLayer.forward': ( 'models.dilated_rnn.html#reslstmlayer.forward',
                                                                                                                'neuralforecast/models/dilated_rnn.py')},
             'neuralforecast.models.gru': { 'neuralforecast.models.gru.GRU': ('models.gru.html#gru', 'neuralforecast/models/gru.py'),
                                            'neuralforecast.models.gru.GRU.__init__': ( 'models.gru.html#gru.__init__',
                                                                                        'neuralforecast/models/gru.py'),
                                            'neuralforecast.models.gru.GRU.forward': ( 'models.gru.html#gru.forward',
                                                                                       'neuralforecast/models/gru.py')},
+            'neuralforecast.models.hint': { 'neuralforecast.models.hint.HINT': ('models.hint.html#hint', 'neuralforecast/models/hint.py'),
+                                            'neuralforecast.models.hint.HINT.__init__': ( 'models.hint.html#hint.__init__',
+                                                                                          'neuralforecast/models/hint.py'),
+                                            'neuralforecast.models.hint.HINT.__repr__': ( 'models.hint.html#hint.__repr__',
+                                                                                          'neuralforecast/models/hint.py'),
+                                            'neuralforecast.models.hint.HINT.fit': ( 'models.hint.html#hint.fit',
+                                                                                     'neuralforecast/models/hint.py'),
+                                            'neuralforecast.models.hint.HINT.predict': ( 'models.hint.html#hint.predict',
+                                                                                         'neuralforecast/models/hint.py'),
+                                            'neuralforecast.models.hint.HINT.save': ( 'models.hint.html#hint.save',
+                                                                                      'neuralforecast/models/hint.py'),
+                                            'neuralforecast.models.hint.HINT.set_test_size': ( 'models.hint.html#hint.set_test_size',
+                                                                                               'neuralforecast/models/hint.py'),
+                                            'neuralforecast.models.hint.get_bottomup_P': ( 'models.hint.html#get_bottomup_p',
+                                                                                           'neuralforecast/models/hint.py'),
+                                            'neuralforecast.models.hint.get_mintrace_ols_P': ( 'models.hint.html#get_mintrace_ols_p',
+                                                                                               'neuralforecast/models/hint.py'),
+                                            'neuralforecast.models.hint.get_mintrace_wls_P': ( 'models.hint.html#get_mintrace_wls_p',
+                                                                                               'neuralforecast/models/hint.py')},
+            'neuralforecast.models.informer': { 'neuralforecast.models.informer.ConvLayer': ( 'models.informer.html#convlayer',
+                                                                                              'neuralforecast/models/informer.py'),
+                                                'neuralforecast.models.informer.ConvLayer.__init__': ( 'models.informer.html#convlayer.__init__',
+                                                                                                       'neuralforecast/models/informer.py'),
+                                                'neuralforecast.models.informer.ConvLayer.forward': ( 'models.informer.html#convlayer.forward',
+                                                                                                      'neuralforecast/models/informer.py'),
+                                                'neuralforecast.models.informer.Informer': ( 'models.informer.html#informer',
+                                                                                             'neuralforecast/models/informer.py'),
+                                                'neuralforecast.models.informer.Informer.__init__': ( 'models.informer.html#informer.__init__',
+                                                                                                      'neuralforecast/models/informer.py'),
+                                                'neuralforecast.models.informer.Informer.forward': ( 'models.informer.html#informer.forward',
+                                                                                                     'neuralforecast/models/informer.py'),
+                                                'neuralforecast.models.informer.ProbAttention': ( 'models.informer.html#probattention',
+                                                                                                  'neuralforecast/models/informer.py'),
+                                                'neuralforecast.models.informer.ProbAttention.__init__': ( 'models.informer.html#probattention.__init__',
+                                                                                                           'neuralforecast/models/informer.py'),
+                                                'neuralforecast.models.informer.ProbAttention._get_initial_context': ( 'models.informer.html#probattention._get_initial_context',
+                                                                                                                       'neuralforecast/models/informer.py'),
+                                                'neuralforecast.models.informer.ProbAttention._prob_QK': ( 'models.informer.html#probattention._prob_qk',
+                                                                                                           'neuralforecast/models/informer.py'),
+                                                'neuralforecast.models.informer.ProbAttention._update_context': ( 'models.informer.html#probattention._update_context',
+                                                                                                                  'neuralforecast/models/informer.py'),
+                                                'neuralforecast.models.informer.ProbAttention.forward': ( 'models.informer.html#probattention.forward',
+                                                                                                          'neuralforecast/models/informer.py'),
+                                                'neuralforecast.models.informer.ProbMask': ( 'models.informer.html#probmask',
+                                                                                             'neuralforecast/models/informer.py'),
+                                                'neuralforecast.models.informer.ProbMask.__init__': ( 'models.informer.html#probmask.__init__',
+                                                                                                      'neuralforecast/models/informer.py'),
+                                                'neuralforecast.models.informer.ProbMask.mask': ( 'models.informer.html#probmask.mask',
+                                                                                                  'neuralforecast/models/informer.py')},
             'neuralforecast.models.lstm': { 'neuralforecast.models.lstm.LSTM': ('models.lstm.html#lstm', 'neuralforecast/models/lstm.py'),
                                             'neuralforecast.models.lstm.LSTM.__init__': ( 'models.lstm.html#lstm.__init__',
                                                                                           'neuralforecast/models/lstm.py'),
                                             'neuralforecast.models.lstm.LSTM.forward': ( 'models.lstm.html#lstm.forward',
                                                                                          'neuralforecast/models/lstm.py')},
             'neuralforecast.models.mlp': { 'neuralforecast.models.mlp.MLP': ('models.mlp.html#mlp', 'neuralforecast/models/mlp.py'),
                                            'neuralforecast.models.mlp.MLP.__init__': ( 'models.mlp.html#mlp.__init__',
@@ -396,19 +535,129 @@
                                                                                                  'neuralforecast/models/nhits.py'),
                                              'neuralforecast.models.nhits._IdentityBasis': ( 'models.nhits.html#_identitybasis',
                                                                                              'neuralforecast/models/nhits.py'),
                                              'neuralforecast.models.nhits._IdentityBasis.__init__': ( 'models.nhits.html#_identitybasis.__init__',
                                                                                                       'neuralforecast/models/nhits.py'),
                                              'neuralforecast.models.nhits._IdentityBasis.forward': ( 'models.nhits.html#_identitybasis.forward',
                                                                                                      'neuralforecast/models/nhits.py')},
+            'neuralforecast.models.patchtst': { 'neuralforecast.models.patchtst.Coord1dPosEncoding': ( 'models.patchtst.html#coord1dposencoding',
+                                                                                                       'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.Coord2dPosEncoding': ( 'models.patchtst.html#coord2dposencoding',
+                                                                                                       'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.Flatten_Head': ( 'models.patchtst.html#flatten_head',
+                                                                                                 'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.Flatten_Head.__init__': ( 'models.patchtst.html#flatten_head.__init__',
+                                                                                                          'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.Flatten_Head.forward': ( 'models.patchtst.html#flatten_head.forward',
+                                                                                                         'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.PatchTST': ( 'models.patchtst.html#patchtst',
+                                                                                             'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.PatchTST.__init__': ( 'models.patchtst.html#patchtst.__init__',
+                                                                                                      'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.PatchTST.forward': ( 'models.patchtst.html#patchtst.forward',
+                                                                                                     'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.PatchTST_backbone': ( 'models.patchtst.html#patchtst_backbone',
+                                                                                                      'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.PatchTST_backbone.__init__': ( 'models.patchtst.html#patchtst_backbone.__init__',
+                                                                                                               'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.PatchTST_backbone.create_pretrain_head': ( 'models.patchtst.html#patchtst_backbone.create_pretrain_head',
+                                                                                                                           'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.PatchTST_backbone.forward': ( 'models.patchtst.html#patchtst_backbone.forward',
+                                                                                                              'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.PositionalEncoding': ( 'models.patchtst.html#positionalencoding',
+                                                                                                       'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.RevIN': ( 'models.patchtst.html#revin',
+                                                                                          'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.RevIN.__init__': ( 'models.patchtst.html#revin.__init__',
+                                                                                                   'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.RevIN._denormalize': ( 'models.patchtst.html#revin._denormalize',
+                                                                                                       'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.RevIN._get_statistics': ( 'models.patchtst.html#revin._get_statistics',
+                                                                                                          'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.RevIN._init_params': ( 'models.patchtst.html#revin._init_params',
+                                                                                                       'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.RevIN._normalize': ( 'models.patchtst.html#revin._normalize',
+                                                                                                     'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.RevIN.forward': ( 'models.patchtst.html#revin.forward',
+                                                                                                  'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.TSTEncoder': ( 'models.patchtst.html#tstencoder',
+                                                                                               'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.TSTEncoder.__init__': ( 'models.patchtst.html#tstencoder.__init__',
+                                                                                                        'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.TSTEncoder.forward': ( 'models.patchtst.html#tstencoder.forward',
+                                                                                                       'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.TSTEncoderLayer': ( 'models.patchtst.html#tstencoderlayer',
+                                                                                                    'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.TSTEncoderLayer.__init__': ( 'models.patchtst.html#tstencoderlayer.__init__',
+                                                                                                             'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.TSTEncoderLayer.forward': ( 'models.patchtst.html#tstencoderlayer.forward',
+                                                                                                            'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.TSTiEncoder': ( 'models.patchtst.html#tstiencoder',
+                                                                                                'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.TSTiEncoder.__init__': ( 'models.patchtst.html#tstiencoder.__init__',
+                                                                                                         'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.TSTiEncoder.forward': ( 'models.patchtst.html#tstiencoder.forward',
+                                                                                                        'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.Transpose': ( 'models.patchtst.html#transpose',
+                                                                                              'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.Transpose.__init__': ( 'models.patchtst.html#transpose.__init__',
+                                                                                                       'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.Transpose.forward': ( 'models.patchtst.html#transpose.forward',
+                                                                                                      'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst._MultiheadAttention': ( 'models.patchtst.html#_multiheadattention',
+                                                                                                        'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst._MultiheadAttention.__init__': ( 'models.patchtst.html#_multiheadattention.__init__',
+                                                                                                                 'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst._MultiheadAttention.forward': ( 'models.patchtst.html#_multiheadattention.forward',
+                                                                                                                'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst._ScaledDotProductAttention': ( 'models.patchtst.html#_scaleddotproductattention',
+                                                                                                               'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst._ScaledDotProductAttention.__init__': ( 'models.patchtst.html#_scaleddotproductattention.__init__',
+                                                                                                                        'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst._ScaledDotProductAttention.forward': ( 'models.patchtst.html#_scaleddotproductattention.forward',
+                                                                                                                       'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.get_activation_fn': ( 'models.patchtst.html#get_activation_fn',
+                                                                                                      'neuralforecast/models/patchtst.py'),
+                                                'neuralforecast.models.patchtst.positional_encoding': ( 'models.patchtst.html#positional_encoding',
+                                                                                                        'neuralforecast/models/patchtst.py')},
             'neuralforecast.models.rnn': { 'neuralforecast.models.rnn.RNN': ('models.rnn.html#rnn', 'neuralforecast/models/rnn.py'),
                                            'neuralforecast.models.rnn.RNN.__init__': ( 'models.rnn.html#rnn.__init__',
                                                                                        'neuralforecast/models/rnn.py'),
                                            'neuralforecast.models.rnn.RNN.forward': ( 'models.rnn.html#rnn.forward',
                                                                                       'neuralforecast/models/rnn.py')},
+            'neuralforecast.models.stemgnn': { 'neuralforecast.models.stemgnn.GLU': ( 'models.stemgnn.html#glu',
+                                                                                      'neuralforecast/models/stemgnn.py'),
+                                               'neuralforecast.models.stemgnn.GLU.__init__': ( 'models.stemgnn.html#glu.__init__',
+                                                                                               'neuralforecast/models/stemgnn.py'),
+                                               'neuralforecast.models.stemgnn.GLU.forward': ( 'models.stemgnn.html#glu.forward',
+                                                                                              'neuralforecast/models/stemgnn.py'),
+                                               'neuralforecast.models.stemgnn.StemGNN': ( 'models.stemgnn.html#stemgnn',
+                                                                                          'neuralforecast/models/stemgnn.py'),
+                                               'neuralforecast.models.stemgnn.StemGNN.__init__': ( 'models.stemgnn.html#stemgnn.__init__',
+                                                                                                   'neuralforecast/models/stemgnn.py'),
+                                               'neuralforecast.models.stemgnn.StemGNN.cheb_polynomial': ( 'models.stemgnn.html#stemgnn.cheb_polynomial',
+                                                                                                          'neuralforecast/models/stemgnn.py'),
+                                               'neuralforecast.models.stemgnn.StemGNN.forward': ( 'models.stemgnn.html#stemgnn.forward',
+                                                                                                  'neuralforecast/models/stemgnn.py'),
+                                               'neuralforecast.models.stemgnn.StemGNN.get_laplacian': ( 'models.stemgnn.html#stemgnn.get_laplacian',
+                                                                                                        'neuralforecast/models/stemgnn.py'),
+                                               'neuralforecast.models.stemgnn.StemGNN.graph_fft': ( 'models.stemgnn.html#stemgnn.graph_fft',
+                                                                                                    'neuralforecast/models/stemgnn.py'),
+                                               'neuralforecast.models.stemgnn.StemGNN.latent_correlation_layer': ( 'models.stemgnn.html#stemgnn.latent_correlation_layer',
+                                                                                                                   'neuralforecast/models/stemgnn.py'),
+                                               'neuralforecast.models.stemgnn.StemGNN.self_graph_attention': ( 'models.stemgnn.html#stemgnn.self_graph_attention',
+                                                                                                               'neuralforecast/models/stemgnn.py'),
+                                               'neuralforecast.models.stemgnn.StockBlockLayer': ( 'models.stemgnn.html#stockblocklayer',
+                                                                                                  'neuralforecast/models/stemgnn.py'),
+                                               'neuralforecast.models.stemgnn.StockBlockLayer.__init__': ( 'models.stemgnn.html#stockblocklayer.__init__',
+                                                                                                           'neuralforecast/models/stemgnn.py'),
+                                               'neuralforecast.models.stemgnn.StockBlockLayer.forward': ( 'models.stemgnn.html#stockblocklayer.forward',
+                                                                                                          'neuralforecast/models/stemgnn.py'),
+                                               'neuralforecast.models.stemgnn.StockBlockLayer.spe_seq_cell': ( 'models.stemgnn.html#stockblocklayer.spe_seq_cell',
+                                                                                                               'neuralforecast/models/stemgnn.py')},
             'neuralforecast.models.tcn': { 'neuralforecast.models.tcn.TCN': ('models.tcn.html#tcn', 'neuralforecast/models/tcn.py'),
                                            'neuralforecast.models.tcn.TCN.__init__': ( 'models.tcn.html#tcn.__init__',
                                                                                        'neuralforecast/models/tcn.py'),
                                            'neuralforecast.models.tcn.TCN.forward': ( 'models.tcn.html#tcn.forward',
                                                                                       'neuralforecast/models/tcn.py')},
             'neuralforecast.models.tft': { 'neuralforecast.models.tft.GLU': ('models.tft.html#glu', 'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.GLU.__init__': ( 'models.tft.html#glu.__init__',
@@ -443,16 +692,14 @@
                                                                                        'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.TFT.forward': ( 'models.tft.html#tft.forward',
                                                                                       'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.TFT.predict_step': ( 'models.tft.html#tft.predict_step',
                                                                                            'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.TFT.training_step': ( 'models.tft.html#tft.training_step',
                                                                                             'neuralforecast/models/tft.py'),
-                                           'neuralforecast.models.tft.TFT.validation_epoch_end': ( 'models.tft.html#tft.validation_epoch_end',
-                                                                                                   'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.TFT.validation_step': ( 'models.tft.html#tft.validation_step',
                                                                                               'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.TFTEmbedding': ( 'models.tft.html#tftembedding',
                                                                                        'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.TFTEmbedding.__init__': ( 'models.tft.html#tftembedding.__init__',
                                                                                                 'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.TFTEmbedding._apply_embedding': ( 'models.tft.html#tftembedding._apply_embedding',
@@ -473,14 +720,32 @@
                                                                                                         'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.VariableSelectionNetwork': ( 'models.tft.html#variableselectionnetwork',
                                                                                                    'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.VariableSelectionNetwork.__init__': ( 'models.tft.html#variableselectionnetwork.__init__',
                                                                                                             'neuralforecast/models/tft.py'),
                                            'neuralforecast.models.tft.VariableSelectionNetwork.forward': ( 'models.tft.html#variableselectionnetwork.forward',
                                                                                                            'neuralforecast/models/tft.py')},
+            'neuralforecast.models.vanillatransformer': { 'neuralforecast.models.vanillatransformer.FullAttention': ( 'models.vanillatransformer.html#fullattention',
+                                                                                                                      'neuralforecast/models/vanillatransformer.py'),
+                                                          'neuralforecast.models.vanillatransformer.FullAttention.__init__': ( 'models.vanillatransformer.html#fullattention.__init__',
+                                                                                                                               'neuralforecast/models/vanillatransformer.py'),
+                                                          'neuralforecast.models.vanillatransformer.FullAttention.forward': ( 'models.vanillatransformer.html#fullattention.forward',
+                                                                                                                              'neuralforecast/models/vanillatransformer.py'),
+                                                          'neuralforecast.models.vanillatransformer.TriangularCausalMask': ( 'models.vanillatransformer.html#triangularcausalmask',
+                                                                                                                             'neuralforecast/models/vanillatransformer.py'),
+                                                          'neuralforecast.models.vanillatransformer.TriangularCausalMask.__init__': ( 'models.vanillatransformer.html#triangularcausalmask.__init__',
+                                                                                                                                      'neuralforecast/models/vanillatransformer.py'),
+                                                          'neuralforecast.models.vanillatransformer.TriangularCausalMask.mask': ( 'models.vanillatransformer.html#triangularcausalmask.mask',
+                                                                                                                                  'neuralforecast/models/vanillatransformer.py'),
+                                                          'neuralforecast.models.vanillatransformer.VanillaTransformer': ( 'models.vanillatransformer.html#vanillatransformer',
+                                                                                                                           'neuralforecast/models/vanillatransformer.py'),
+                                                          'neuralforecast.models.vanillatransformer.VanillaTransformer.__init__': ( 'models.vanillatransformer.html#vanillatransformer.__init__',
+                                                                                                                                    'neuralforecast/models/vanillatransformer.py'),
+                                                          'neuralforecast.models.vanillatransformer.VanillaTransformer.forward': ( 'models.vanillatransformer.html#vanillatransformer.forward',
+                                                                                                                                   'neuralforecast/models/vanillatransformer.py')},
             'neuralforecast.tsdataset': { 'neuralforecast.tsdataset.TimeSeriesDataModule': ( 'tsdataset.html#timeseriesdatamodule',
                                                                                              'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesDataModule.__init__': ( 'tsdataset.html#timeseriesdatamodule.__init__',
                                                                                                       'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesDataModule.predict_dataloader': ( 'tsdataset.html#timeseriesdatamodule.predict_dataloader',
                                                                                                                 'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesDataModule.train_dataloader': ( 'tsdataset.html#timeseriesdatamodule.train_dataloader',
@@ -497,16 +762,53 @@
                                                                                                    'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesDataset.__len__': ( 'tsdataset.html#timeseriesdataset.__len__',
                                                                                                   'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesDataset.__repr__': ( 'tsdataset.html#timeseriesdataset.__repr__',
                                                                                                    'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesDataset.from_df': ( 'tsdataset.html#timeseriesdataset.from_df',
                                                                                                   'neuralforecast/tsdataset.py'),
+                                          'neuralforecast.tsdataset.TimeSeriesDataset.trim_dataset': ( 'tsdataset.html#timeseriesdataset.trim_dataset',
+                                                                                                       'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesDataset.update_dataset': ( 'tsdataset.html#timeseriesdataset.update_dataset',
                                                                                                          'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesLoader': ( 'tsdataset.html#timeseriesloader',
                                                                                          'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesLoader.__init__': ( 'tsdataset.html#timeseriesloader.__init__',
                                                                                                   'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesLoader._collate_fn': ( 'tsdataset.html#timeseriesloader._collate_fn',
                                                                                                      'neuralforecast/tsdataset.py')},
-            'neuralforecast.utils': {'neuralforecast.utils.generate_series': ('utils.html#generate_series', 'neuralforecast/utils.py')}}}
+            'neuralforecast.utils': { 'neuralforecast.utils.DayOfMonth': ('utils.html#dayofmonth', 'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.DayOfMonth.__call__': ( 'utils.html#dayofmonth.__call__',
+                                                                                    'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.DayOfWeek': ('utils.html#dayofweek', 'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.DayOfWeek.__call__': ( 'utils.html#dayofweek.__call__',
+                                                                                   'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.DayOfYear': ('utils.html#dayofyear', 'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.DayOfYear.__call__': ( 'utils.html#dayofyear.__call__',
+                                                                                   'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.HourOfDay': ('utils.html#hourofday', 'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.HourOfDay.__call__': ( 'utils.html#hourofday.__call__',
+                                                                                   'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.MinuteOfHour': ('utils.html#minuteofhour', 'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.MinuteOfHour.__call__': ( 'utils.html#minuteofhour.__call__',
+                                                                                      'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.MonthOfYear': ('utils.html#monthofyear', 'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.MonthOfYear.__call__': ( 'utils.html#monthofyear.__call__',
+                                                                                     'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.SecondOfMinute': ('utils.html#secondofminute', 'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.SecondOfMinute.__call__': ( 'utils.html#secondofminute.__call__',
+                                                                                        'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.TimeFeature': ('utils.html#timefeature', 'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.TimeFeature.__call__': ( 'utils.html#timefeature.__call__',
+                                                                                     'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.TimeFeature.__init__': ( 'utils.html#timefeature.__init__',
+                                                                                     'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.TimeFeature.__repr__': ( 'utils.html#timefeature.__repr__',
+                                                                                     'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.WeekOfYear': ('utils.html#weekofyear', 'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.WeekOfYear.__call__': ( 'utils.html#weekofyear.__call__',
+                                                                                    'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.augment_calendar_df': ( 'utils.html#augment_calendar_df',
+                                                                                    'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.generate_series': ('utils.html#generate_series', 'neuralforecast/utils.py'),
+                                      'neuralforecast.utils.time_features_from_frequency_str': ( 'utils.html#time_features_from_frequency_str',
+                                                                                                 'neuralforecast/utils.py')}}}
```

### Comparing `neuralforecast-1.4.0/neuralforecast/auto.py` & `neuralforecast-1.5.0/neuralforecast/auto.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/models.ipynb.
 
 # %% auto 0
 __all__ = ['AutoRNN', 'AutoLSTM', 'AutoGRU', 'AutoTCN', 'AutoDilatedRNN', 'AutoMLP', 'AutoNBEATS', 'AutoNBEATSx', 'AutoNHITS',
-           'AutoTFT']
+           'AutoTFT', 'AutoVanillaTransformer', 'AutoInformer', 'AutoAutoformer', 'AutoPatchTST', 'AutoStemGNN']
 
 # %% ../nbs/models.ipynb 2
 from os import cpu_count
 import torch
 
 from ray import tune
 from ray.tune.search.basic_variant import BasicVariantGenerator
@@ -21,22 +21,28 @@
 
 from .models.mlp import MLP
 from .models.nbeats import NBEATS
 from .models.nbeatsx import NBEATSx
 from .models.nhits import NHITS
 
 from .models.tft import TFT
+from .models.vanillatransformer import VanillaTransformer
+from .models.informer import Informer
+from .models.autoformer import Autoformer
+from .models.patchtst import PatchTST
+
+from .models.stemgnn import StemGNN
 
 from .losses.pytorch import MAE
 
 # %% ../nbs/models.ipynb 8
 class AutoRNN(BaseAuto):
-
     default_config = {
         "input_size_multiplier": [-1, 4, 16, 64],
+        "inference_input_size_multiplier": [-1],
         "h": None,
         "encoder_hidden_size": tune.choice([50, 100, 200, 300]),
         "encoder_n_layers": tune.randint(1, 4),
         "context_size": tune.choice([5, 10, 50]),
         "decoder_hidden_size": tune.choice([64, 128, 256, 512]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "max_steps": tune.choice([500, 1000]),
@@ -65,14 +71,17 @@
         """
         # Define search space, input/output sizes
         if config is None:
             config = self.default_config.copy()
             config["input_size"] = tune.choice(
                 [h * x for x in self.default_config["input_size_multiplier"]]
             )
+            config["inference_input_size"] = tune.choice(
+                [h * x for x in self.default_config["inference_input_size_multiplier"]]
+            )
             del config["input_size_multiplier"]
 
         super(AutoRNN, self).__init__(
             cls_model=RNN,
             h=h,
             loss=loss,
             valid_loss=valid_loss,
@@ -83,17 +92,17 @@
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
         )
 
 # %% ../nbs/models.ipynb 13
 class AutoLSTM(BaseAuto):
-
     default_config = {
         "input_size_multiplier": [-1, 4, 16, 64],
+        "inference_input_size_multiplier": [-1],
         "h": None,
         "encoder_hidden_size": tune.choice([50, 100, 200, 300]),
         "encoder_n_layers": tune.randint(1, 4),
         "context_size": tune.choice([5, 10, 50]),
         "decoder_hidden_size": tune.choice([64, 128, 256, 512]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "max_steps": tune.choice([500, 1000]),
@@ -111,21 +120,23 @@
         search_alg=BasicVariantGenerator(random_state=1),
         num_samples=10,
         refit_with_val=False,
         cpus=cpu_count(),
         gpus=torch.cuda.device_count(),
         verbose=False,
     ):
-
         # Define search space, input/output sizes
         if config is None:
             config = self.default_config.copy()
             config["input_size"] = tune.choice(
                 [h * x for x in self.default_config["input_size_multiplier"]]
             )
+            config["inference_input_size"] = tune.choice(
+                [h * x for x in self.default_config["inference_input_size_multiplier"]]
+            )
             del config["input_size_multiplier"]
 
         super(AutoLSTM, self).__init__(
             cls_model=LSTM,
             h=h,
             loss=loss,
             valid_loss=valid_loss,
@@ -136,17 +147,17 @@
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
         )
 
 # %% ../nbs/models.ipynb 17
 class AutoGRU(BaseAuto):
-
     default_config = {
         "input_size_multiplier": [-1, 4, 16, 64],
+        "inference_input_size_multiplier": [-1],
         "h": None,
         "encoder_hidden_size": tune.choice([50, 100, 200, 300]),
         "encoder_n_layers": tune.randint(1, 4),
         "context_size": tune.choice([5, 10, 50]),
         "decoder_hidden_size": tune.choice([64, 128, 256, 512]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "max_steps": tune.choice([500, 1000]),
@@ -163,43 +174,47 @@
         config=None,
         search_alg=BasicVariantGenerator(random_state=1),
         num_samples=10,
         refit_with_val=False,
         cpus=cpu_count(),
         gpus=torch.cuda.device_count(),
         verbose=False,
+        alias=None,
     ):
-
         # Define search space, input/output sizes
         if config is None:
             config = self.default_config.copy()
             config["input_size"] = tune.choice(
                 [h * x for x in self.default_config["input_size_multiplier"]]
             )
+            config["inference_input_size"] = tune.choice(
+                [h * x for x in self.default_config["inference_input_size_multiplier"]]
+            )
             del config["input_size_multiplier"]
 
         super(AutoGRU, self).__init__(
             cls_model=GRU,
             h=h,
             loss=loss,
             valid_loss=valid_loss,
             config=config,
             search_alg=search_alg,
             num_samples=num_samples,
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
+            alias=alias,
         )
 
 # %% ../nbs/models.ipynb 21
 class AutoTCN(BaseAuto):
-
     default_config = {
         "input_size_multiplier": [-1, 4, 16, 64],
+        "inference_input_size_multiplier": [-1],
         "h": None,
         "encoder_hidden_size": tune.choice([50, 100, 200, 300]),
         "context_size": tune.choice([5, 10, 50]),
         "decoder_hidden_size": tune.choice([64, 128]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "max_steps": tune.choice([500, 1000]),
         "batch_size": tune.choice([16, 32]),
@@ -215,43 +230,47 @@
         config=None,
         search_alg=BasicVariantGenerator(random_state=1),
         num_samples=10,
         refit_with_val=False,
         cpus=cpu_count(),
         gpus=torch.cuda.device_count(),
         verbose=False,
+        alias=None,
     ):
-
         # Define search space, input/output sizes
         if config is None:
             config = self.default_config.copy()
             config["input_size"] = tune.choice(
                 [h * x for x in self.default_config["input_size_multiplier"]]
             )
+            config["inference_input_size"] = tune.choice(
+                [h * x for x in self.default_config["inference_input_size_multiplier"]]
+            )
             del config["input_size_multiplier"]
 
         super(AutoTCN, self).__init__(
             cls_model=TCN,
             h=h,
             loss=loss,
             valid_loss=valid_loss,
             config=config,
             search_alg=search_alg,
             num_samples=num_samples,
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
+            alias=alias,
         )
 
 # %% ../nbs/models.ipynb 25
 class AutoDilatedRNN(BaseAuto):
-
     default_config = {
         "input_size_multiplier": [-1, 4, 16, 64],
+        "inference_input_size_multiplier": [-1],
         "h": None,
         "cell_type": tune.choice(["LSTM", "GRU"]),
         "encoder_hidden_size": tune.choice([50, 100, 200, 300]),
         "dilations": tune.choice([[[1, 2], [4, 8]], [[1, 2, 4, 8]]]),
         "context_size": tune.choice([5, 10, 50]),
         "decoder_hidden_size": tune.choice([64, 128, 256, 512]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
@@ -269,41 +288,44 @@
         config=None,
         search_alg=BasicVariantGenerator(random_state=1),
         num_samples=10,
         refit_with_val=False,
         cpus=cpu_count(),
         gpus=torch.cuda.device_count(),
         verbose=False,
+        alias=None,
     ):
-
         # Define search space, input/output sizes
         if config is None:
             config = self.default_config.copy()
             config["input_size"] = tune.choice(
                 [h * x for x in self.default_config["input_size_multiplier"]]
             )
+            config["inference_input_size"] = tune.choice(
+                [h * x for x in self.default_config["inference_input_size_multiplier"]]
+            )
             del config["input_size_multiplier"]
 
         super(AutoDilatedRNN, self).__init__(
             cls_model=DilatedRNN,
             h=h,
             loss=loss,
             valid_loss=valid_loss,
             config=config,
             search_alg=search_alg,
             num_samples=num_samples,
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
+            alias=alias,
         )
 
 # %% ../nbs/models.ipynb 30
 class AutoMLP(BaseAuto):
-
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([256, 512, 1024]),
         "num_layers": tune.randint(2, 6),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "scaler_type": tune.choice([None, "robust", "standard"]),
@@ -322,16 +344,16 @@
         config=None,
         search_alg=BasicVariantGenerator(random_state=1),
         num_samples=10,
         refit_with_val=False,
         cpus=cpu_count(),
         gpus=torch.cuda.device_count(),
         verbose=False,
+        alias=None,
     ):
-
         # Define search space, input/output sizes
         if config is None:
             config = self.default_config.copy()
             config["input_size"] = tune.choice(
                 [h * x for x in self.default_config["input_size_multiplier"]]
             )
 
@@ -348,19 +370,19 @@
             config=config,
             search_alg=search_alg,
             num_samples=num_samples,
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
+            alias=alias,
         )
 
 # %% ../nbs/models.ipynb 34
 class AutoNBEATS(BaseAuto):
-
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "scaler_type": tune.choice([None, "robust", "standard"]),
         "max_steps": tune.choice([500, 1000]),
         "batch_size": tune.choice([32, 64, 128, 256]),
@@ -377,16 +399,16 @@
         config=None,
         search_alg=BasicVariantGenerator(random_state=1),
         num_samples=10,
         refit_with_val=False,
         cpus=cpu_count(),
         gpus=torch.cuda.device_count(),
         verbose=False,
+        alias=None,
     ):
-
         # Define search space, input/output sizes
         if config is None:
             config = self.default_config.copy()
             config["input_size"] = tune.choice(
                 [h * x for x in self.default_config["input_size_multiplier"]]
             )
 
@@ -403,19 +425,19 @@
             config=config,
             search_alg=search_alg,
             num_samples=num_samples,
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
+            alias=alias,
         )
 
 # %% ../nbs/models.ipynb 38
 class AutoNBEATSx(BaseAuto):
-
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "scaler_type": tune.choice([None, "robust", "standard"]),
         "max_steps": tune.choice([500, 1000]),
         "batch_size": tune.choice([32, 64, 128, 256]),
@@ -432,16 +454,16 @@
         config=None,
         search_alg=BasicVariantGenerator(random_state=1),
         num_samples=10,
         refit_with_val=False,
         cpus=cpu_count(),
         gpus=torch.cuda.device_count(),
         verbose=False,
+        alias=None,
     ):
-
         # Define search space, input/output sizes
         if config is None:
             config = self.default_config.copy()
             config["input_size"] = tune.choice(
                 [h * x for x in self.default_config["input_size_multiplier"]]
             )
 
@@ -458,19 +480,19 @@
             config=config,
             search_alg=search_alg,
             num_samples=num_samples,
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
+            alias=alias,
         )
 
 # %% ../nbs/models.ipynb 42
 class AutoNHITS(BaseAuto):
-
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "n_pool_kernel_size": tune.choice(
             [3 * [1], 3 * [2], 3 * [4], [8, 4, 1], [16, 8, 1]]
         ),
         "n_freq_downsample": tune.choice(
@@ -500,16 +522,16 @@
         config=None,
         search_alg=BasicVariantGenerator(random_state=1),
         num_samples=10,
         refit_with_val=False,
         cpus=cpu_count(),
         gpus=torch.cuda.device_count(),
         verbose=False,
+        alias=None,
     ):
-
         # Define search space, input/output sizes
         if config is None:
             config = self.default_config.copy()
             config["input_size"] = tune.choice(
                 [h * x for x in self.default_config["input_size_multiplier"]]
             )
 
@@ -526,19 +548,19 @@
             config=config,
             search_alg=search_alg,
             num_samples=num_samples,
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
+            alias=alias,
         )
 
 # %% ../nbs/models.ipynb 47
 class AutoTFT(BaseAuto):
-
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "scaler_type": tune.choice([None, "robust", "standard"]),
@@ -557,16 +579,16 @@
         config=None,
         search_alg=BasicVariantGenerator(random_state=1),
         num_samples=10,
         refit_with_val=False,
         cpus=cpu_count(),
         gpus=torch.cuda.device_count(),
         verbose=False,
+        alias=None,
     ):
-
         # Define search space, input/output sizes
         if config is None:
             config = self.default_config.copy()
             config["input_size"] = tune.choice(
                 [h * x for x in self.default_config["input_size_multiplier"]]
             )
 
@@ -583,8 +605,300 @@
             config=config,
             search_alg=search_alg,
             num_samples=num_samples,
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
+            alias=alias,
+        )
+
+# %% ../nbs/models.ipynb 51
+class AutoVanillaTransformer(BaseAuto):
+    default_config = {
+        "input_size_multiplier": [1, 2, 3, 4, 5],
+        "h": None,
+        "hidden_size": tune.choice([64, 128, 256]),
+        "n_head": tune.choice([4, 8]),
+        "learning_rate": tune.loguniform(1e-4, 1e-1),
+        "scaler_type": tune.choice([None, "robust", "standard"]),
+        "max_steps": tune.choice([500, 1000, 2000]),
+        "batch_size": tune.choice([32, 64, 128, 256]),
+        "windows_batch_size": tune.choice([128, 256, 512, 1024]),
+        "loss": None,
+        "random_seed": tune.randint(1, 20),
+    }
+
+    def __init__(
+        self,
+        h,
+        loss=MAE(),
+        valid_loss=None,
+        config=None,
+        search_alg=BasicVariantGenerator(random_state=1),
+        num_samples=10,
+        refit_with_val=False,
+        cpus=cpu_count(),
+        gpus=torch.cuda.device_count(),
+        verbose=False,
+        alias=None,
+    ):
+        # Define search space, input/output sizes
+        if config is None:
+            config = self.default_config.copy()
+            config["input_size"] = tune.choice(
+                [h * x for x in self.default_config["input_size_multiplier"]]
+            )
+
+            # Rolling windows with step_size=1 or step_size=h
+            # See `BaseWindows` and `BaseRNN`'s create_windows
+            config["step_size"] = tune.choice([1, h])
+            del config["input_size_multiplier"]
+
+        super(AutoVanillaTransformer, self).__init__(
+            cls_model=VanillaTransformer,
+            h=h,
+            loss=loss,
+            valid_loss=valid_loss,
+            config=config,
+            search_alg=search_alg,
+            num_samples=num_samples,
+            refit_with_val=refit_with_val,
+            cpus=cpus,
+            gpus=gpus,
+            verbose=verbose,
+            alias=alias,
+        )
+
+# %% ../nbs/models.ipynb 55
+class AutoInformer(BaseAuto):
+    default_config = {
+        "input_size_multiplier": [1, 2, 3, 4, 5],
+        "h": None,
+        "hidden_size": tune.choice([64, 128, 256]),
+        "n_head": tune.choice([4, 8]),
+        "learning_rate": tune.loguniform(1e-4, 1e-1),
+        "scaler_type": tune.choice([None, "robust", "standard"]),
+        "max_steps": tune.choice([500, 1000, 2000]),
+        "batch_size": tune.choice([32, 64, 128, 256]),
+        "windows_batch_size": tune.choice([128, 256, 512, 1024]),
+        "loss": None,
+        "random_seed": tune.randint(1, 20),
+    }
+
+    def __init__(
+        self,
+        h,
+        loss=MAE(),
+        valid_loss=None,
+        config=None,
+        search_alg=BasicVariantGenerator(random_state=1),
+        num_samples=10,
+        refit_with_val=False,
+        cpus=cpu_count(),
+        gpus=torch.cuda.device_count(),
+        verbose=False,
+        alias=None,
+    ):
+        # Define search space, input/output sizes
+        if config is None:
+            config = self.default_config.copy()
+            config["input_size"] = tune.choice(
+                [h * x for x in self.default_config["input_size_multiplier"]]
+            )
+
+            # Rolling windows with step_size=1 or step_size=h
+            # See `BaseWindows` and `BaseRNN`'s create_windows
+            config["step_size"] = tune.choice([1, h])
+            del config["input_size_multiplier"]
+
+        super(AutoInformer, self).__init__(
+            cls_model=Informer,
+            h=h,
+            loss=loss,
+            valid_loss=valid_loss,
+            config=config,
+            search_alg=search_alg,
+            num_samples=num_samples,
+            refit_with_val=refit_with_val,
+            cpus=cpus,
+            gpus=gpus,
+            verbose=verbose,
+            alias=alias,
+        )
+
+# %% ../nbs/models.ipynb 59
+class AutoAutoformer(BaseAuto):
+    default_config = {
+        "input_size_multiplier": [1, 2, 3, 4, 5],
+        "h": None,
+        "hidden_size": tune.choice([64, 128, 256]),
+        "n_head": tune.choice([4, 8]),
+        "learning_rate": tune.loguniform(1e-4, 1e-1),
+        "scaler_type": tune.choice([None, "robust", "standard"]),
+        "max_steps": tune.choice([500, 1000, 2000]),
+        "batch_size": tune.choice([32, 64, 128, 256]),
+        "windows_batch_size": tune.choice([128, 256, 512, 1024]),
+        "loss": None,
+        "random_seed": tune.randint(1, 20),
+    }
+
+    def __init__(
+        self,
+        h,
+        loss=MAE(),
+        valid_loss=None,
+        config=None,
+        search_alg=BasicVariantGenerator(random_state=1),
+        num_samples=10,
+        refit_with_val=False,
+        cpus=cpu_count(),
+        gpus=torch.cuda.device_count(),
+        verbose=False,
+        alias=None,
+    ):
+        # Define search space, input/output sizes
+        if config is None:
+            config = self.default_config.copy()
+            config["input_size"] = tune.choice(
+                [h * x for x in self.default_config["input_size_multiplier"]]
+            )
+
+            # Rolling windows with step_size=1 or step_size=h
+            # See `BaseWindows` and `BaseRNN`'s create_windows
+            config["step_size"] = tune.choice([1, h])
+            del config["input_size_multiplier"]
+
+        super(AutoAutoformer, self).__init__(
+            cls_model=Autoformer,
+            h=h,
+            loss=loss,
+            valid_loss=valid_loss,
+            config=config,
+            search_alg=search_alg,
+            num_samples=num_samples,
+            refit_with_val=refit_with_val,
+            cpus=cpus,
+            gpus=gpus,
+            verbose=verbose,
+            alias=alias,
+        )
+
+# %% ../nbs/models.ipynb 63
+class AutoPatchTST(BaseAuto):
+    default_config = {
+        "input_size_multiplier": [1, 2, 3],
+        "h": None,
+        "hidden_size": tune.choice([16, 128, 256]),
+        "n_head": tune.choice([4, 16]),
+        "patch_len": tune.choice([16, 24]),
+        "learning_rate": tune.loguniform(1e-4, 1e-1),
+        "scaler_type": tune.choice([None, "robust", "standard"]),
+        "revin": tune.choice([False, True]),
+        "max_steps": tune.choice([500, 1000, 5000]),
+        "batch_size": tune.choice([32, 64, 128, 256]),
+        "windows_batch_size": tune.choice([128, 256, 512, 1024]),
+        "loss": None,
+        "random_seed": tune.randint(1, 20),
+    }
+
+    def __init__(
+        self,
+        h,
+        loss=MAE(),
+        valid_loss=None,
+        config=None,
+        search_alg=BasicVariantGenerator(random_state=1),
+        num_samples=10,
+        refit_with_val=False,
+        cpus=cpu_count(),
+        gpus=torch.cuda.device_count(),
+        verbose=False,
+        alias=None,
+    ):
+        # Define search space, input/output sizes
+        if config is None:
+            config = self.default_config.copy()
+            config["input_size"] = tune.choice(
+                [h * x for x in self.default_config["input_size_multiplier"]]
+            )
+
+            # Rolling windows with step_size=1 or step_size=h
+            # See `BaseWindows` and `BaseRNN`'s create_windows
+            config["step_size"] = tune.choice([1, h])
+            del config["input_size_multiplier"]
+
+        super(AutoPatchTST, self).__init__(
+            cls_model=PatchTST,
+            h=h,
+            loss=loss,
+            valid_loss=valid_loss,
+            config=config,
+            search_alg=search_alg,
+            num_samples=num_samples,
+            refit_with_val=refit_with_val,
+            cpus=cpus,
+            gpus=gpus,
+            verbose=verbose,
+            alias=alias,
+        )
+
+# %% ../nbs/models.ipynb 68
+class AutoStemGNN(BaseAuto):
+    default_config = {
+        "input_size_multiplier": [1, 2, 3, 4],
+        "h": None,
+        "n_series": None,
+        "n_stacks": tune.choice([2, 3]),
+        "multi_layer": tune.choice([3, 5, 7]),
+        "learning_rate": tune.loguniform(1e-4, 1e-1),
+        "scaler_type": tune.choice([None, "robust", "standard"]),
+        "max_steps": tune.choice([500, 1000, 2000]),
+        "batch_size": tune.choice([32, 64, 128, 256]),
+        "loss": None,
+        "random_seed": tune.randint(1, 20),
+    }
+
+    def __init__(
+        self,
+        h,
+        n_series,
+        loss=MAE(),
+        valid_loss=None,
+        config=None,
+        search_alg=BasicVariantGenerator(random_state=1),
+        num_samples=10,
+        refit_with_val=False,
+        cpus=cpu_count(),
+        gpus=torch.cuda.device_count(),
+        verbose=False,
+        alias=None,
+    ):
+        # Define search space, input/output sizes
+        if config is None:
+            config = self.default_config.copy()
+            config["input_size"] = tune.choice(
+                [h * x for x in self.default_config["input_size_multiplier"]]
+            )
+
+            # Rolling windows with step_size=1 or step_size=h
+            # See `BaseWindows` and `BaseRNN`'s create_windows
+            config["step_size"] = tune.choice([1, h])
+            del config["input_size_multiplier"]
+
+        # Always use n_series from parameters
+        config["n_series"] = n_series
+
+        super(AutoStemGNN, self).__init__(
+            cls_model=StemGNN,
+            h=h,
+            loss=loss,
+            valid_loss=valid_loss,
+            config=config,
+            search_alg=search_alg,
+            num_samples=num_samples,
+            refit_with_val=refit_with_val,
+            cpus=cpus,
+            gpus=gpus,
+            verbose=verbose,
+            alias=alias,
         )
```

### Comparing `neuralforecast-1.4.0/neuralforecast/common/_base_auto.py` & `neuralforecast-1.5.0/neuralforecast/common/_base_auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     `search_alg`: ray.tune.search variant, BasicVariantGenerator, HyperOptSearch, DragonflySearch, TuneBOHB for details
         see [tune.search](https://docs.ray.io/en/latest/tune/api_docs/suggestion.html#).<br>
     `num_samples`: int, number of hyperparameter optimization steps/samples.<br>
     `cpus`: int, number of cpus to use during optimization, default all available.<br>
     `gpus`: int, number of gpus to use during optimization, default all available.<br>
     `refit_wo_val`: bool, number of gpus to use during optimization, default all available.<br>
     `verbose`: bool, wether print partial outputs.<br>
+    `alias`: str, optional,  Custom name of the model.<br>
     """
 
     def __init__(
         self,
         cls_model,
         h,
         loss,
@@ -109,14 +110,15 @@
         config,
         search_alg=BasicVariantGenerator(random_state=1),
         num_samples=10,
         cpus=cpu_count(),
         gpus=torch.cuda.device_count(),
         refit_with_val=False,
         verbose=False,
+        alias=None,
     ):
         super(BaseAuto, self).__init__()
         self.save_hyperparameters()  # Allows instantiation from a checkpoint from class
 
         if config.get("h", None) is not None:
             raise Exception("Please use `h` init argument instead of `config['h']`.")
         if config.get("loss", None) is not None:
@@ -144,14 +146,21 @@
         self.search_alg = search_alg
         self.cpus = cpus
         self.gpus = gpus
         self.refit_with_val = refit_with_val
         self.verbose = verbose
         self.loss = self.config.get("loss", MAE())
         self.valid_loss = self.config.get("valid_loss", self.loss)
+        self.alias = alias
+
+        # Base Class attributes
+        self.SAMPLING_TYPE = cls_model.SAMPLING_TYPE
+
+    def __repr__(self):
+        return type(self).__name__ if self.alias is None else self.alias
 
     def fit(self, dataset, val_size=0, test_size=0):
         """BaseAuto.fit
 
         Perform the hyperparameter optimization as specified by the BaseAuto configuration
         dictionary `config`.
 
@@ -205,14 +214,17 @@
         `y_hat`: numpy predictions of the `NeuralForecast` model.<br>
         """
         return self.model.predict(dataset=dataset, step_size=step_size, **data_kwargs)
 
     def set_test_size(self, test_size):
         self.model.set_test_size(test_size)
 
+    def get_test_size(self):
+        return self.model.test_size
+
     def save(self, path):
         """BaseAuto.save
 
         Save the fitted model to disk.
 
         **Parameters:**<br>
         `path`: str, path to save the model.<br>
```

### Comparing `neuralforecast-1.4.0/neuralforecast/common/_base_recurrent.py` & `neuralforecast-1.5.0/neuralforecast/common/_base_recurrent.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,30 @@
 from pytorch_lightning.callbacks.early_stopping import EarlyStopping
 
 from ._scalers import TemporalNorm
 from ..tsdataset import TimeSeriesDataModule
 
 # %% ../../nbs/common.base_recurrent.ipynb 6
 class BaseRecurrent(pl.LightningModule):
+    """Base Recurrent
+
+    Base class for all recurrent-based models. The forecasts are produced sequentially between
+    windows.
+
+    This class implements the basic functionality for all windows-based models, including:
+    - PyTorch Lightning's methods training_step, validation_step, predict_step. <br>
+    - fit and predict methods used by NeuralForecast.core class. <br>
+    - sampling and wrangling methods to sequential windows. <br>
+    """
+
     def __init__(
         self,
         h,
         input_size,
+        inference_input_size,
         loss,
         valid_loss,
         learning_rate,
         max_steps,
         val_check_steps,
         batch_size,
         valid_batch_size,
@@ -35,40 +47,42 @@
         early_stop_patience_steps=-1,
         futr_exog_list=None,
         hist_exog_list=None,
         stat_exog_list=None,
         num_workers_loader=0,
         drop_last_loader=False,
         random_seed=1,
+        alias=None,
         **trainer_kwargs,
     ):
         super(BaseRecurrent, self).__init__()
 
         self.save_hyperparameters()  # Allows instantiation from a checkpoint from class
         self.random_seed = random_seed
         pl.seed_everything(self.random_seed, workers=True)
 
         # Padder to complete train windows,
         # example y=[1,2,3,4,5] h=3 -> last y_output = [5,0,0]
         self.h = h
         self.input_size = input_size
+        self.inference_input_size = inference_input_size
         self.padder = nn.ConstantPad1d(padding=(0, self.h), value=0)
 
         # Loss
         self.loss = loss
-        if valid_loss == None:
+        if valid_loss is None:
             self.valid_loss = loss
         else:
             self.valid_loss = valid_loss
         self.train_trajectories = []
         self.valid_trajectories = []
 
         # Valid batch_size
         self.batch_size = batch_size
-        if valid_batch_size == None:
+        if valid_batch_size is None:
             self.valid_batch_size = batch_size
         else:
             self.valid_batch_size = valid_batch_size
 
         # Optimization
         self.learning_rate = learning_rate
         self.max_steps = max_steps
@@ -126,14 +140,20 @@
             trainer_kwargs["enable_checkpointing"] = False
 
         self.trainer_kwargs = trainer_kwargs
 
         # DataModule arguments
         self.num_workers_loader = num_workers_loader
         self.drop_last_loader = drop_last_loader
+        # used by on_validation_epoch_end hook
+        self.validation_step_outputs = []
+        self.alias = alias
+
+    def __repr__(self):
+        return type(self).__name__ if self.alias is None else self.alias
 
     def on_fit_start(self):
         torch.manual_seed(self.random_seed)
         np.random.seed(self.random_seed)
         random.seed(self.random_seed)
 
     def configure_optimizers(self):
@@ -144,15 +164,14 @@
             ),
             "frequency": 1,
             "interval": "step",
         }
         return {"optimizer": optimizer, "lr_scheduler": scheduler}
 
     def _normalization(self, batch, val_size=0, test_size=0):
-
         temporal = batch["temporal"]  # B, C, T
         temporal_cols = batch["temporal_cols"].copy()
 
         # Separate data and mask
         temporal_data_cols = temporal_cols.drop("available_mask").tolist()
         temporal_data = temporal[:, temporal_cols.get_indexer(temporal_data_cols), :]
         temporal_mask = temporal[:, temporal_cols.get_loc("available_mask"), :].clone()
@@ -231,28 +250,40 @@
                 temporal = temporal[:, :, : -self.test_size]
             temporal = self.padder(temporal)
 
         if step == "predict":
             if (self.test_size == 0) and (len(self.futr_exog_list) == 0):
                 temporal = self.padder(temporal)
 
+            # Test size covers all data, pad left one timestep with zeros
+            if temporal.shape[-1] == self.test_size:
+                padder_left = nn.ConstantPad1d(padding=(1, 0), value=0)
+                temporal = padder_left(temporal)
+
         # Parse batch
         window_size = 1 + self.h  # 1 for current t and h for future
         windows = temporal.unfold(dimension=-1, size=window_size, step=1)
 
-        # Truncated backprogatation during training (shorten sequence where RNNs unroll)
+        # Truncated backprogatation/inference (shorten sequence where RNNs unroll)
         n_windows = windows.shape[2]
-        if (
-            (step == "train")
-            and (self.input_size > 0)
-            and (n_windows > self.input_size)
-        ):
-            max_sampleable_time = n_windows - self.input_size + 1
-            start = np.random.choice(max_sampleable_time)
-            windows = windows[:, :, start : (start + self.input_size), :]
+        input_size = -1
+        if (step == "train") and (self.input_size > 0):
+            input_size = self.input_size
+            if (input_size > 0) and (n_windows > input_size):
+                max_sampleable_time = n_windows - self.input_size + 1
+                start = np.random.choice(max_sampleable_time)
+                windows = windows[:, :, start : (start + input_size), :]
+
+        if (step == "val") and (self.inference_input_size > 0):
+            cutoff = self.inference_input_size + self.val_size
+            windows = windows[:, :, -cutoff:, :]
+
+        if (step == "predict") and (self.inference_input_size > 0):
+            cutoff = self.inference_input_size + self.test_size
+            windows = windows[:, :, -cutoff:, :]
 
         # [B, C, input_size, 1+H]
         windows_batch = dict(
             temporal=windows,
             temporal_cols=temporal_cols,
             static=batch.get("static", None),
             static_cols=batch.get("static_cols", None),
@@ -402,48 +433,56 @@
             outsample_y = outsample_y.reshape(B * T, H)
             outsample_mask = outsample_mask.reshape(B * T, H)
             y_loc = y_loc.repeat_interleave(repeats=T, dim=0).squeeze(-1)
             y_scale = y_scale.repeat_interleave(repeats=T, dim=0).squeeze(-1)
             distr_args = self.loss.scale_decouple(
                 output=output, loc=y_loc, scale=y_scale
             )
+            _, sample_mean, quants = self.loss.sample(distr_args=distr_args)
 
             if str(type(self.valid_loss)) in [
                 "<class 'neuralforecast.losses.pytorch.sCRPS'>",
                 "<class 'neuralforecast.losses.pytorch.MQLoss'>",
             ]:
-                _, y_hat = self.loss.sample(distr_args=distr_args, num_samples=500)
+                output = quants
+            elif str(type(self.valid_loss)) in [
+                "<class 'neuralforecast.losses.pytorch.relMSE'>"
+            ]:
+                output = torch.unsqueeze(sample_mean, dim=-1)  # [N,H,1] -> [N,H]
+
         else:
-            y_hat = output[:, -val_windows:-1, :]
+            output = output[:, -val_windows:-1, :]
 
         # Validation Loss evaluation
         if self.valid_loss.is_distribution_output:
             valid_loss = self.valid_loss(
                 y=outsample_y, distr_args=distr_args, mask=outsample_mask
             )
         else:
             valid_loss = self.valid_loss(
-                y=outsample_y, y_hat=y_hat, mask=outsample_mask
+                y=outsample_y, y_hat=output, mask=outsample_mask
             )
 
         self.log(
             "valid_loss",
             valid_loss,
             batch_size=self.batch_size,
             prog_bar=True,
             on_epoch=True,
         )
+        self.validation_step_outputs.append(valid_loss)
         return valid_loss
 
-    def validation_epoch_end(self, outputs):
+    def on_validation_epoch_end(self):
         if self.val_size == 0:
             return
-        avg_loss = torch.stack(outputs).mean()
+        avg_loss = torch.stack(self.validation_step_outputs).mean()
         self.log("ptl/val_loss", avg_loss, batch_size=self.batch_size)
         self.valid_trajectories.append((self.global_step, float(avg_loss)))
+        self.validation_step_outputs.clear()  # free memory (compute `avg_loss` per epoch)
 
     def predict_step(self, batch, batch_idx):
         # Create and normalize windows [Ws, L+H, C]
         batch = self._normalization(batch, val_size=0, test_size=self.test_size)
         windows = self._create_windows(batch, step="predict")
 
         # Parse windows
@@ -476,29 +515,29 @@
             H = output[0].size()[2]
             output = [arg.reshape(-1, *(arg.size()[2:])) for arg in output]
             y_loc = y_loc.repeat_interleave(repeats=T, dim=0).squeeze(-1)
             y_scale = y_scale.repeat_interleave(repeats=T, dim=0).squeeze(-1)
             distr_args = self.loss.scale_decouple(
                 output=output, loc=y_loc, scale=y_scale
             )
-            _, y_hat = self.loss.sample(distr_args=distr_args, num_samples=500)
+            _, sample_mean, quants = self.loss.sample(distr_args=distr_args)
+            y_hat = torch.concat((sample_mean, quants), axis=2)
             y_hat = y_hat.view(B, T, H, -1)
 
             if self.loss.return_params:
                 distr_args = torch.stack(distr_args, dim=-1)
                 distr_args = torch.reshape(distr_args, (B, T, H, -1))
                 y_hat = torch.concat((y_hat, distr_args), axis=3)
         else:
             y_hat, _, _ = self._inv_normalization(
                 y_hat=output, temporal_cols=batch["temporal_cols"]
             )
-
         return y_hat
 
-    def fit(self, dataset, val_size=0, test_size=0):
+    def fit(self, dataset, val_size=0, test_size=0, random_seed=None):
         """Fit.
 
         The `fit` method, optimizes the neural network's weights using the
         initialization parameters (`learning_rate`, `batch_size`, ...)
         and the `loss` function as defined during the initialization.
         Within `fit` we use a PyTorch Lightning `Trainer` that
         inherits the initialization's `self.trainer_kwargs`, to customize
@@ -511,14 +550,19 @@
         disk memory, to get them change `enable_checkpointing=True` in `__init__`.
 
         **Parameters:**<br>
         `dataset`: NeuralForecast's `TimeSeriesDataset`, see [documentation](https://nixtla.github.io/neuralforecast/tsdataset.html).<br>
         `val_size`: int, validation size for temporal cross-validation.<br>
         `test_size`: int, test size for temporal cross-validation.<br>
         """
+        # Restart random seed
+        if random_seed is None:
+            random_seed = self.random_seed
+        torch.manual_seed(random_seed)
+
         self.val_size = val_size
         self.test_size = test_size
         datamodule = TimeSeriesDataModule(
             dataset=dataset,
             batch_size=self.batch_size,
             valid_batch_size=self.valid_batch_size,
             num_workers=self.num_workers_loader,
@@ -543,24 +587,29 @@
 
         self.trainer_kwargs["val_check_interval"] = val_check_interval
         self.trainer_kwargs["check_val_every_n_epoch"] = check_val_every_n_epoch
 
         trainer = pl.Trainer(**self.trainer_kwargs)
         trainer.fit(self, datamodule=datamodule)
 
-    def predict(self, dataset, step_size=1, **data_module_kwargs):
+    def predict(self, dataset, step_size=1, random_seed=None, **data_module_kwargs):
         """Predict.
 
         Neural network prediction with PL's `Trainer` execution of `predict_step`.
 
         **Parameters:**<br>
         `dataset`: NeuralForecast's `TimeSeriesDataset`, see [documentation](https://nixtla.github.io/neuralforecast/tsdataset.html).<br>
         `step_size`: int=1, Step size between each window.<br>
         `**data_module_kwargs`: PL's TimeSeriesDataModule args, see [documentation](https://pytorch-lightning.readthedocs.io/en/1.6.1/extensions/datamodules.html#using-a-datamodule).
         """
+        # Restart random seed
+        if random_seed is None:
+            random_seed = self.random_seed
+        torch.manual_seed(random_seed)
+
         if step_size > 1:
             raise Exception("Recurrent models do not support step_size > 1")
 
         # fcsts (window, batch, h)
         # Protect when case of multiple gpu. PL does not support return preds with multiple gpu.
         pred_trainer_kwargs = self.trainer_kwargs.copy()
         if (pred_trainer_kwargs.get("accelerator", None) == "gpu") and (
@@ -589,14 +638,17 @@
             fcsts = torch.vstack([fcst[:, -1:, :] for fcst in fcsts]).numpy().flatten()
             fcsts = fcsts.reshape(-1, len(self.loss.output_names))
         return fcsts
 
     def set_test_size(self, test_size):
         self.test_size = test_size
 
+    def get_test_size(self):
+        return self.test_size
+
     def save(self, path):
         """BaseRecurrent.save
 
         Save the fitted model to disk.
 
         **Parameters:**<br>
         `path`: str, path to save the model.<br>
```

### Comparing `neuralforecast-1.4.0/neuralforecast/common/_base_windows.py` & `neuralforecast-1.5.0/neuralforecast/common/_base_windows.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,25 @@
 from pytorch_lightning.callbacks.early_stopping import EarlyStopping
 
 from ._scalers import TemporalNorm
 from ..tsdataset import TimeSeriesDataModule
 
 # %% ../../nbs/common.base_windows.ipynb 5
 class BaseWindows(pl.LightningModule):
+    """Base Windows
+
+    Base class for all windows-based models. The forecasts are produced separately
+    for each window, which are randomly sampled during training.
+
+    This class implements the basic functionality for all windows-based models, including:
+    - PyTorch Lightning's methods training_step, validation_step, predict_step.<br>
+    - fit and predict methods used by NeuralForecast.core class.<br>
+    - sampling and wrangling methods to generate windows.
+    """
+
     def __init__(
         self,
         h,
         input_size,
         loss,
         valid_loss,
         learning_rate,
@@ -37,14 +48,15 @@
         scaler_type="identity",
         futr_exog_list=None,
         hist_exog_list=None,
         stat_exog_list=None,
         num_workers_loader=0,
         drop_last_loader=False,
         random_seed=1,
+        alias=None,
         **trainer_kwargs,
     ):
         super(BaseWindows, self).__init__()
 
         self.save_hyperparameters()  # Allows instantiation from a checkpoint from class
         self.random_seed = random_seed
         pl.seed_everything(self.random_seed, workers=True)
@@ -53,24 +65,24 @@
         # example y=[1,2,3,4,5] h=3 -> last y_output = [5,0,0]
         self.h = h
         self.input_size = input_size
         self.padder = nn.ConstantPad1d(padding=(0, self.h), value=0)
 
         # Loss
         self.loss = loss
-        if valid_loss == None:
+        if valid_loss is None:
             self.valid_loss = loss
         else:
             self.valid_loss = valid_loss
         self.train_trajectories = []
         self.valid_trajectories = []
 
         # Valid batch_size
         self.batch_size = batch_size
-        if valid_batch_size == None:
+        if valid_batch_size is None:
             self.valid_batch_size = batch_size
         else:
             self.valid_batch_size = valid_batch_size
 
         # Optimization
         self.learning_rate = learning_rate
         self.max_steps = max_steps
@@ -136,14 +148,20 @@
             trainer_kwargs["enable_checkpointing"] = False
 
         self.trainer_kwargs = trainer_kwargs
 
         # DataModule arguments
         self.num_workers_loader = num_workers_loader
         self.drop_last_loader = drop_last_loader
+        # used by on_validation_epoch_end hook
+        self.validation_step_outputs = []
+        self.alias = alias
+
+    def __repr__(self):
+        return type(self).__name__ if self.alias is None else self.alias
 
     def on_fit_start(self):
         torch.manual_seed(self.random_seed)
         np.random.seed(self.random_seed)
         random.seed(self.random_seed)
 
     def configure_optimizers(self):
@@ -222,19 +240,26 @@
                 temporal_cols=temporal_cols,
                 static=static,
                 static_cols=static_cols,
             )
             return windows_batch
 
         elif step in ["predict", "val"]:
-
             if step == "predict":
+                initial_input = temporal.shape[-1] - self.test_size
+                if (
+                    initial_input <= self.input_size
+                ):  # There is not enough data to predict first timestamp
+                    padder_left = nn.ConstantPad1d(
+                        padding=(self.input_size - initial_input, 0), value=0
+                    )
+                    temporal = padder_left(temporal)
                 predict_step_size = self.predict_step_size
                 cutoff = -self.input_size - self.test_size
-                temporal = batch["temporal"][:, :, cutoff:]
+                temporal = temporal[:, :, cutoff:]
 
             elif step == "val":
                 predict_step_size = self.step_size
                 cutoff = -self.input_size - self.val_size - self.test_size
                 if self.test_size > 0:
                     temporal = batch["temporal"][:, :, cutoff : -self.test_size]
                 else:
@@ -363,14 +388,15 @@
             futr_exog,
             stat_exog,
         )
 
     def training_step(self, batch, batch_idx):
         # Create and normalize windows [Ws, L+H, C]
         windows = self._create_windows(batch, step="train")
+        original_outsample_y = torch.clone(windows["temporal"][:, -self.h :, 0])
         windows = self._normalization(windows=windows)
 
         # Parse windows
         (
             insample_y,
             insample_mask,
             outsample_y,
@@ -387,17 +413,18 @@
             hist_exog=hist_exog,  # [Ws, L]
             stat_exog=stat_exog,
         )  # [Ws, 1]
 
         # Model Predictions
         output = self(windows_batch)
         if self.loss.is_distribution_output:
-            outsample_y, y_loc, y_scale = self._inv_normalization(
+            _, y_loc, y_scale = self._inv_normalization(
                 y_hat=outsample_y, temporal_cols=batch["temporal_cols"]
             )
+            outsample_y = original_outsample_y
             distr_args = self.loss.scale_decouple(
                 output=output, loc=y_loc, scale=y_scale
             )
             loss = self.loss(y=outsample_y, distr_args=distr_args, mask=outsample_mask)
         else:
             loss = self.loss(y=outsample_y, y_hat=output, mask=outsample_mask)
 
@@ -407,14 +434,15 @@
 
     def validation_step(self, batch, batch_idx):
         if self.val_size == 0:
             return np.nan
 
         # Create and normalize windows [Ws, L+H, C]
         windows = self._create_windows(batch, step="val")
+        original_outsample_y = torch.clone(windows["temporal"][:, -self.h :, 0])
         windows = self._normalization(windows=windows)
 
         # Parse windows
         (
             insample_y,
             insample_mask,
             outsample_y,
@@ -431,46 +459,54 @@
             hist_exog=hist_exog,  # [Ws, L]
             stat_exog=stat_exog,
         )  # [Ws, 1]
 
         # Model Predictions
         output = self(windows_batch)
         if self.loss.is_distribution_output:
-            outsample_y, y_loc, y_scale = self._inv_normalization(
+            _, y_loc, y_scale = self._inv_normalization(
                 y_hat=outsample_y, temporal_cols=batch["temporal_cols"]
             )
+            outsample_y = original_outsample_y
             distr_args = self.loss.scale_decouple(
                 output=output, loc=y_loc, scale=y_scale
             )
+            _, sample_mean, quants = self.loss.sample(distr_args=distr_args)
 
             if str(type(self.valid_loss)) in [
                 "<class 'neuralforecast.losses.pytorch.sCRPS'>",
                 "<class 'neuralforecast.losses.pytorch.MQLoss'>",
             ]:
-                _, output = self.loss.sample(distr_args=distr_args, num_samples=500)
+                output = quants
+            elif str(type(self.valid_loss)) in [
+                "<class 'neuralforecast.losses.pytorch.relMSE'>"
+            ]:
+                output = torch.unsqueeze(sample_mean, dim=-1)  # [N,H,1] -> [N,H]
 
         # Validation Loss evaluation
         if self.valid_loss.is_distribution_output:
             valid_loss = self.valid_loss(
                 y=outsample_y, distr_args=distr_args, mask=outsample_mask
             )
         else:
             valid_loss = self.valid_loss(
                 y=outsample_y, y_hat=output, mask=outsample_mask
             )
 
         self.log("valid_loss", valid_loss, prog_bar=True, on_epoch=True)
+        self.validation_step_outputs.append(valid_loss)
         return valid_loss
 
-    def validation_epoch_end(self, outputs):
+    def on_validation_epoch_end(self):
         if self.val_size == 0:
             return
-        avg_loss = torch.stack(outputs).mean()
+        avg_loss = torch.stack(self.validation_step_outputs).mean()
         self.log("ptl/val_loss", avg_loss)
         self.valid_trajectories.append((self.global_step, float(avg_loss)))
+        self.validation_step_outputs.clear()  # free memory (compute `avg_loss` per epoch)
 
     def predict_step(self, batch, batch_idx):
         # Create and normalize windows [Ws, L+H, C]
         windows = self._create_windows(batch, step="predict")
         windows = self._normalization(windows=windows)
 
         # Parse windows
@@ -497,29 +533,30 @@
         if self.loss.is_distribution_output:
             _, y_loc, y_scale = self._inv_normalization(
                 y_hat=output[0], temporal_cols=batch["temporal_cols"]
             )
             distr_args = self.loss.scale_decouple(
                 output=output, loc=y_loc, scale=y_scale
             )
-            _, y_hat = self.loss.sample(distr_args=distr_args, num_samples=500)
+            _, sample_mean, quants = self.loss.sample(distr_args=distr_args)
+            y_hat = torch.concat((sample_mean, quants), axis=2)
 
             if self.loss.return_params:
                 distr_args = torch.stack(distr_args, dim=-1)
                 distr_args = torch.reshape(
                     distr_args, (len(windows["temporal"]), self.h, -1)
                 )
                 y_hat = torch.concat((y_hat, distr_args), axis=2)
         else:
             y_hat, _, _ = self._inv_normalization(
                 y_hat=output, temporal_cols=batch["temporal_cols"]
             )
         return y_hat
 
-    def fit(self, dataset, val_size=0, test_size=0):
+    def fit(self, dataset, val_size=0, test_size=0, random_seed=None):
         """Fit.
 
         The `fit` method, optimizes the neural network's weights using the
         initialization parameters (`learning_rate`, `windows_batch_size`, ...)
         and the `loss` function as defined during the initialization.
         Within `fit` we use a PyTorch Lightning `Trainer` that
         inherits the initialization's `self.trainer_kwargs`, to customize
@@ -532,14 +569,19 @@
         disk memory, to get them change `enable_checkpointing=True` in `__init__`.
 
         **Parameters:**<br>
         `dataset`: NeuralForecast's `TimeSeriesDataset`, see [documentation](https://nixtla.github.io/neuralforecast/tsdataset.html).<br>
         `val_size`: int, validation size for temporal cross-validation.<br>
         `test_size`: int, test size for temporal cross-validation.<br>
         """
+        # Restart random seed
+        if random_seed is None:
+            random_seed = self.random_seed
+        torch.manual_seed(random_seed)
+
         self.val_size = val_size
         self.test_size = test_size
         datamodule = TimeSeriesDataModule(
             dataset=dataset,
             batch_size=self.batch_size,
             valid_batch_size=self.valid_batch_size,
             num_workers=self.num_workers_loader,
@@ -564,25 +606,37 @@
 
         self.trainer_kwargs["val_check_interval"] = val_check_interval
         self.trainer_kwargs["check_val_every_n_epoch"] = check_val_every_n_epoch
 
         trainer = pl.Trainer(**self.trainer_kwargs)
         trainer.fit(self, datamodule=datamodule)
 
-    def predict(self, dataset, test_size=None, step_size=1, **data_module_kwargs):
+    def predict(
+        self,
+        dataset,
+        test_size=None,
+        step_size=1,
+        random_seed=None,
+        **data_module_kwargs,
+    ):
         """Predict.
 
         Neural network prediction with PL's `Trainer` execution of `predict_step`.
 
         **Parameters:**<br>
         `dataset`: NeuralForecast's `TimeSeriesDataset`, see [documentation](https://nixtla.github.io/neuralforecast/tsdataset.html).<br>
         `test_size`: int=None, test size for temporal cross-validation.<br>
         `step_size`: int=1, Step size between each window.<br>
         `**data_module_kwargs`: PL's TimeSeriesDataModule args, see [documentation](https://pytorch-lightning.readthedocs.io/en/1.6.1/extensions/datamodules.html#using-a-datamodule).
         """
+        # Restart random seed
+        if random_seed is None:
+            random_seed = self.random_seed
+        torch.manual_seed(random_seed)
+
         self.predict_step_size = step_size
         self.decompose_forecast = False
         datamodule = TimeSeriesDataModule(
             dataset=dataset,
             valid_batch_size=self.valid_batch_size,
             **data_module_kwargs,
         )
@@ -596,25 +650,30 @@
 
         trainer = pl.Trainer(**pred_trainer_kwargs)
         fcsts = trainer.predict(self, datamodule=datamodule)
         fcsts = torch.vstack(fcsts).numpy().flatten()
         fcsts = fcsts.reshape(-1, len(self.loss.output_names))
         return fcsts
 
-    def decompose(self, dataset, step_size=1, **data_module_kwargs):
+    def decompose(self, dataset, step_size=1, random_seed=None, **data_module_kwargs):
         """Decompose Predictions.
 
         Decompose the predictions through the network's layers.
         Available methods are `ESRNN`, `NHITS`, `NBEATS`, and `NBEATSx`.
 
         **Parameters:**<br>
         `dataset`: NeuralForecast's `TimeSeriesDataset`, see [documentation here](https://nixtla.github.io/neuralforecast/tsdataset.html).<br>
         `step_size`: int=1, step size between each window of temporal data.<br>
         `**data_module_kwargs`: PL's TimeSeriesDataModule args, see [documentation](https://pytorch-lightning.readthedocs.io/en/1.6.1/extensions/datamodules.html#using-a-datamodule).
         """
+        # Restart random seed
+        if random_seed is None:
+            random_seed = self.random_seed
+        torch.manual_seed(random_seed)
+
         self.predict_step_size = step_size
         self.decompose_forecast = True
         datamodule = TimeSeriesDataModule(
             dataset=dataset,
             valid_batch_size=self.valid_batch_size,
             **data_module_kwargs,
         )
@@ -625,14 +684,17 @@
 
     def forward(self, insample_y, insample_mask):
         raise NotImplementedError("forward")
 
     def set_test_size(self, test_size):
         self.test_size = test_size
 
+    def get_test_size(self):
+        return self.test_size
+
     def save(self, path):
         """BaseWindows.save
 
         Save the fitted model to disk.
 
         **Parameters:**<br>
         `path`: str, path to save the model.<br>
```

### Comparing `neuralforecast-1.4.0/neuralforecast/common/_scalers.py` & `neuralforecast-1.5.0/neuralforecast/common/_scalers.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,21 +275,26 @@
             dimension dim to avoid NaNs from zero division.<br>
     `eps` (float, optional): Small value to avoid division by zero. Defaults to 1e-6.<br>
     `dim` (int, optional): Dimension over to compute median and mad. Defaults to -1.<br>
 
     **Returns:**<br>
     `x`: original torch.Tensor `x`.
     """
-    x_shift = torch.zeros_like(x)[:, [0], :]
-    x_scale = torch.ones_like(x)[:, [0], :]
+    # Collapse dim dimension
+    shape = list(x.shape)
+    shape[dim] = 1
+
+    x_shift = torch.zeros(shape)
+    x_scale = torch.ones(shape)
+
     return x, x_shift, x_scale
 
 # %% ../../nbs/common.scalers.ipynb 27
 def inv_identity_scaler(z, x_shift, x_scale):
-    return z * x_scale + x_shift
+    return z
 
 # %% ../../nbs/common.scalers.ipynb 30
 class TemporalNorm(nn.Module):
     """Temporal Normalization
 
     Standardization of the features is a common requirement for many
     machine learning estimators, and it is commonly achieved by removing
```

### Comparing `neuralforecast-1.4.0/neuralforecast/core.py` & `neuralforecast-1.5.0/neuralforecast/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,19 @@
     TCN,
     DilatedRNN,
     MLP,
     NHITS,
     NBEATS,
     NBEATSx,
     TFT,
+    VanillaTransformer,
+    Informer,
+    Autoformer,
+    StemGNN,
+    PatchTST,
 )
 
 # %% ../nbs/core.ipynb 5
 def _cv_dates(last_dates, freq, h, test_size, step_size=1):
     # assuming step_size = 1
     if (test_size - h) % step_size:
         raise Exception("`test_size - h` should be module `step_size`")
@@ -63,37 +68,84 @@
                 _cv_dates(np.array([ld]), freq, h, test_size, step_size)
                 for ld in last_dates
             ]
         )
         dates = dates.reset_index(drop=True)
     return dates
 
-# %% ../nbs/core.ipynb 9
+# %% ../nbs/core.ipynb 6
+def _insample_dates(uids, last_dates, freq, h, len_series, step_size=1):
+    """
+    Generate insample dates for `predict_insample` function. Uses `_cv_dates`
+    method with separate sizes and last dates for each series.
+    """
+    if (len(np.unique(last_dates)) == 1) and (len(np.unique(len_series)) == 1):
+        # Dates can be generated simulatenously if ld and ls are the same for all series
+        dates = _cv_dates(last_dates, freq, h, len_series[0], step_size)
+        dates["unique_id"] = np.repeat(uids, len(dates) // len(uids))
+    else:
+        dates = []
+        for ui, ld, ls in zip(uids, last_dates, len_series):
+            # Dates have to be generated for each series separately, considering its own ld and ls
+            dates_series = _cv_dates(np.array([ld]), freq, h, ls, step_size)
+            dates_series["unique_id"] = ui
+            dates.append(dates_series)
+        dates = pd.concat(dates)
+    dates = dates.reset_index(drop=True)
+    dates = dates[["unique_id", "ds", "cutoff"]]
+    return dates
+
+# %% ../nbs/core.ipynb 7
+def _future_dates(dataset, uids, last_dates, freq, h):
+    """
+    Generate future dates for `predict` function.
+    """
+    if issubclass(last_dates.dtype.type, np.integer):
+        last_date_f = lambda x: np.arange(x + 1, x + 1 + h, dtype=last_dates.dtype)
+    else:
+        last_date_f = lambda x: pd.date_range(x + freq, periods=h, freq=freq)
+    if len(np.unique(last_dates)) == 1:
+        dates = np.tile(last_date_f(last_dates[0]), len(dataset))
+    else:
+        dates = np.hstack([last_date_f(last_date) for last_date in last_dates])
+    idx = pd.Index(np.repeat(uids, h), name="unique_id")
+    df = pd.DataFrame({"ds": dates}, index=idx)
+    return df
+
+# %% ../nbs/core.ipynb 11
 MODEL_FILENAME_DICT = {
     "gru": GRU,
     "lstm": LSTM,
     "rnn": RNN,
     "tcn": TCN,
     "dilatedrnn": DilatedRNN,
     "mlp": MLP,
     "nbeats": NBEATS,
     "nbeatsx": NBEATSx,
     "nhits": NHITS,
     "tft": TFT,
+    "stemgnn": StemGNN,
+    "informer": Informer,
     "autogru": GRU,
     "autolstm": LSTM,
     "autornn": RNN,
     "autotcn": TCN,
     "autodilatedrnn": DilatedRNN,
     "automlp": MLP,
     "autonbeats": NBEATS,
     "autonhits": NHITS,
+    "autotft": TFT,
+    "autovanillatransformer": VanillaTransformer,
+    "autoinformer": Informer,
+    "autoautoformer": Autoformer,
+    "autopatchtst": PatchTST,
+    "autostemgnn": StemGNN,
 }
 
-# %% ../nbs/core.ipynb 10
+# %% ../nbs/core.ipynb 12
 class NeuralForecast:
     def __init__(self, models: List[Any], freq: str):
         """
         The `core.StatsForecast` class allows you to efficiently fit multiple `NeuralForecast` models
         for large sets of time series. It operates with pandas DataFrame `df` that identifies series
         and datestamps with the `unique_id` and `ds` columns. The `y` column denotes the target
         time series variable.
@@ -121,18 +173,18 @@
         self.freq = pd.tseries.frequencies.to_offset(freq)
 
         # Flags and attributes
         self._fitted = False
 
     def _prepare_fit(self, df, static_df, sort_df):
         # TODO: uids, last_dates and ds should be properties of the dataset class. See github issue.
-        self.dataset, self.uids, self.last_dates, self.ds = TimeSeriesDataset.from_df(
+        dataset, uids, last_dates, ds = TimeSeriesDataset.from_df(
             df=df, static_df=static_df, sort_df=sort_df
         )
-        self.sort_df = sort_df
+        return dataset, uids, last_dates, ds
 
     def fit(
         self,
         df: Optional[pd.DataFrame] = None,
         static_df: Optional[pd.DataFrame] = None,
         val_size: Optional[int] = 0,
         sort_df: bool = True,
@@ -163,15 +215,18 @@
             Returns `NeuralForecast` class with fitted `models`.
         """
         if (df is None) and not (hasattr(self, "dataset")):
             raise Exception("You must pass a DataFrame or have one stored.")
 
         # Process and save new dataset (in self)
         if df is not None:
-            self._prepare_fit(df=df, static_df=static_df, sort_df=sort_df)
+            self.dataset, self.uids, self.last_dates, self.ds = self._prepare_fit(
+                df=df, static_df=static_df, sort_df=sort_df
+            )
+            self.sort_df = sort_df
         else:
             if verbose:
                 print("Using stored dataset.")
 
         if val_size is not None:
             if self.dataset.min_size < val_size:
                 warnings.warn(
@@ -181,31 +236,14 @@
         # train + validation
         for model in self.models:
             model.fit(self.dataset, val_size=val_size)
         # train with the full dataset
 
         self._fitted = True
 
-    def _make_future_df(self, h: int):
-        if issubclass(self.last_dates.dtype.type, np.integer):
-            last_date_f = lambda x: np.arange(
-                x + 1, x + 1 + h, dtype=self.last_dates.dtype
-            )
-        else:
-            last_date_f = lambda x: pd.date_range(
-                x + self.freq, periods=h, freq=self.freq
-            )
-        if len(np.unique(self.last_dates)) == 1:
-            dates = np.tile(last_date_f(self.last_dates[0]), len(self.dataset))
-        else:
-            dates = np.hstack([last_date_f(last_date) for last_date in self.last_dates])
-        idx = pd.Index(np.repeat(self.uids, h), name="unique_id")
-        df = pd.DataFrame({"ds": dates}, index=idx)
-        return df
-
     def predict(
         self,
         df: Optional[pd.DataFrame] = None,
         static_df: Optional[pd.DataFrame] = None,
         futr_df: Optional[pd.DataFrame] = None,
         sort_df: bool = True,
         verbose: bool = False,
@@ -236,52 +274,61 @@
         fcsts_df : pandas.DataFrame
             DataFrame with insample `models` columns for point predictions and probabilistic
             predictions for all fitted `models`.
         """
         if (df is None) and not (hasattr(self, "dataset")):
             raise Exception("You must pass a DataFrame or have one stored.")
 
-        # Process and save new dataset (in self)
+        # Process new dataset but does not store it.
         if df is not None:
-            self._prepare_fit(df=df, static_df=static_df, sort_df=sort_df)
+            dataset, uids, last_dates, _ = self._prepare_fit(
+                df=df, static_df=static_df, sort_df=sort_df
+            )
         else:
+            dataset = self.dataset
+            uids = self.uids
+            last_dates = self.last_dates
             if verbose:
                 print("Using stored dataset.")
 
         cols = []
         count_names = {"model": 0}
         for model in self.models:
-            model_name = type(model).__name__
+            model_name = repr(model)
             count_names[model_name] = count_names.get(model_name, -1) + 1
             if count_names[model_name] > 0:
                 model_name += str(count_names[model_name])
             cols += [model_name + n for n in model.loss.output_names]
 
         # Placeholder dataframe for predictions with unique_id and ds
-        fcsts_df = self._make_future_df(h=self.h)
+        fcsts_df = _future_dates(
+            dataset=dataset, uids=uids, last_dates=last_dates, freq=self.freq, h=self.h
+        )
 
         # Update and define new forecasting dataset
         if futr_df is not None:
             dataset = TimeSeriesDataset.update_dataset(
-                dataset=self.dataset, future_df=futr_df
+                dataset=dataset, future_df=futr_df
             )
         else:
             dataset = TimeSeriesDataset.update_dataset(
-                dataset=self.dataset, future_df=fcsts_df.reset_index()
+                dataset=dataset, future_df=fcsts_df.reset_index()
             )
 
         col_idx = 0
-        fcsts = np.full((self.h * len(self.uids), len(cols)), fill_value=np.nan)
+        fcsts = np.full((self.h * len(uids), len(cols)), fill_value=np.nan)
         for model in self.models:
+            old_test_size = model.get_test_size()
             model.set_test_size(self.h)  # To predict h steps ahead
             model_fcsts = model.predict(dataset=dataset, **data_kwargs)
             # Append predictions in memory placeholder
             output_length = len(model.loss.output_names)
             fcsts[:, col_idx : col_idx + output_length] = model_fcsts
             col_idx += output_length
+            model.set_test_size(old_test_size)  # Set back to original value
 
         # Declare predictions pd.DataFrame
         fcsts = pd.DataFrame.from_records(fcsts, columns=cols, index=fcsts_df.index)
         fcsts_df = pd.concat([fcsts_df, fcsts], axis=1)
 
         return fcsts_df
 
@@ -332,25 +379,28 @@
         fcsts_df : pandas.DataFrame
             DataFrame with insample `models` columns for point predictions and probabilistic
             predictions for all fitted `models`.
         """
         if (df is None) and not (hasattr(self, "dataset")):
             raise Exception("You must pass a DataFrame or have one stored.")
 
-        # Declare predictions pd.DataFrame
+        # Process and save new dataset (in self)
         if df is not None:
-            self._prepare_fit(df=df, static_df=static_df, sort_df=sort_df)
+            self.dataset, self.uids, self.last_dates, self.ds = self._prepare_fit(
+                df=df, static_df=static_df, sort_df=sort_df
+            )
+            self.sort_df = sort_df
         else:
             if verbose:
                 print("Using stored dataset.")
 
         cols = []
         count_names = {"model": 0}
         for model in self.models:
-            model_name = type(model).__name__
+            model_name = repr(model)
             count_names[model_name] = count_names.get(model_name, -1) + 1
             if count_names[model_name] > 0:
                 model_name += str(count_names[model_name])
             cols += [model_name + n for n in model.loss.output_names]
 
         h = self.models[0].h
         if test_size is None:
@@ -396,23 +446,118 @@
                 self.dataset, step_size=step_size, **data_kwargs
             )
 
             # Append predictions in memory placeholder
             output_length = len(model.loss.output_names)
             fcsts[:, col_idx : (col_idx + output_length)] = model_fcsts
             col_idx += output_length
+        if fit_models:
+            self._fitted = True
 
         # Add predictions to forecasts DataFrame
         fcsts = pd.DataFrame.from_records(fcsts, columns=cols, index=fcsts_df.index)
         fcsts_df = pd.concat([fcsts_df, fcsts], axis=1)
 
         # Add original input df's y to forecasts DataFrame
         fcsts_df = fcsts_df.merge(df, how="left", on=["unique_id", "ds"])
         return fcsts_df
 
+    def predict_insample(self, step_size: int = 1):
+        """Predict insample with core.NeuralForecast.
+
+        `core.NeuralForecast`'s `predict_insample` uses stored fitted `models`
+        to predict historic values of a time series from the stored dataframe.
+
+        Parameters
+        ----------
+        step_size : int (default=1)
+            Step size between each window.
+
+        Returns
+        -------
+        fcsts_df : pandas.DataFrame
+            DataFrame with insample predictions for all fitted `models`.
+        """
+        if not self._fitted:
+            raise Exception(
+                "The models must be fitted first with `fit` or `cross_validation`."
+            )
+
+        for model in self.models:
+            if model.SAMPLING_TYPE == "recurrent":
+                warnings.warn(
+                    f"Predict insample might not provide accurate predictions for \
+                       recurrent model {repr(model)} class yet due to scaling."
+                )
+                print(
+                    f"WARNING: Predict insample might not provide accurate predictions for \
+                      recurrent model {repr(model)} class yet due to scaling."
+                )
+
+        cols = []
+        count_names = {"model": 0}
+        for model in self.models:
+            model_name = repr(model)
+            count_names[model_name] = count_names.get(model_name, -1) + 1
+            if count_names[model_name] > 0:
+                model_name += str(count_names[model_name])
+            cols += [model_name + n for n in model.loss.output_names]
+
+        # Remove test set from dataset and last dates
+        test_size = self.models[0].get_test_size()
+        if test_size > 0:
+            trimmed_dataset = TimeSeriesDataset.trim_dataset(
+                dataset=self.dataset, right_trim=test_size, left_trim=0
+            )
+            last_dates_train = self.last_dates.shift(-test_size, freq=self.freq)
+        else:
+            trimmed_dataset = self.dataset
+            last_dates_train = self.last_dates
+
+        # Generate dates
+        len_series = np.diff(
+            trimmed_dataset.indptr
+        )  # Computes the length of each time series based on indptr
+        fcsts_df = _insample_dates(
+            uids=self.uids,
+            last_dates=last_dates_train,
+            freq=self.freq,
+            h=self.h,
+            len_series=len_series,
+            step_size=step_size,
+        )
+        fcsts_df = fcsts_df.set_index("unique_id")
+
+        col_idx = 0
+        fcsts = np.full((len(fcsts_df), len(cols)), np.nan, dtype=np.float32)
+
+        for model in self.models:
+            # Test size is the number of periods to forecast (full size of trimmed dataset)
+            model.set_test_size(test_size=trimmed_dataset.max_size)
+
+            # Predict
+            model_fcsts = model.predict(trimmed_dataset, step_size=step_size)
+            # Append predictions in memory placeholder
+            output_length = len(model.loss.output_names)
+            fcsts[:, col_idx : (col_idx + output_length)] = model_fcsts
+            col_idx += output_length
+            model.set_test_size(test_size=test_size)  # Set original test_size
+
+        # Add predictions to forecasts DataFrame
+        fcsts = pd.DataFrame.from_records(fcsts, columns=cols, index=fcsts_df.index)
+        fcsts_df = pd.concat([fcsts_df, fcsts], axis=1)
+
+        # Add original input df's y to forecasts DataFrame
+        Y_df = pd.DataFrame.from_records(
+            self.dataset.temporal[:, [0]].numpy(), columns=["y"], index=self.ds
+        )
+        Y_df = Y_df.reset_index(drop=False)
+        fcsts_df = fcsts_df.merge(Y_df, how="left", on=["unique_id", "ds"])
+        return fcsts_df
+
     def predict_rolled(
         self,
         df: Optional[pd.DataFrame] = None,
         static_df: Optional[pd.DataFrame] = None,
         n_windows: int = 1,
         step_size: int = 1,
         insample_size: Optional[int] = None,
@@ -446,14 +591,17 @@
 
         Returns
         -------
         fcsts_df : pandas.DataFrame
             DataFrame with insample `models` columns for point predictions and probabilistic
             predictions for all fitted `models`.
         """
+        print(
+            "WARNING: this method will be deprecated. Use `cross_validation` or `predict_insample` instead."
+        )
         fcsts_df = self.cross_validation(
             df=df,
             static_df=static_df,
             n_windows=n_windows,
             step_size=step_size,
             val_size=0,
             test_size=insample_size,
@@ -511,15 +659,15 @@
         # Save models
         count_names = {"model": 0}
         for i, model in enumerate(self.models):
             # Skip model if not in list
             if i not in model_index:
                 continue
 
-            model_name = type(model).__name__.lower().replace("_", "")
+            model_name = repr(model).lower().replace("_", "")
             count_names[model_name] = count_names.get(model_name, -1) + 1
             model.save(f"{path}/{model_name}_{count_names[model_name]}.ckpt")
 
         # Save dataset
         if (save_dataset) and (hasattr(self, "dataset")):
             with open(f"{path}/dataset.pkl", "wb") as f:
                 pickle.dump(self.dataset, f)
```

### Comparing `neuralforecast-1.4.0/neuralforecast/losses/numpy.py` & `neuralforecast-1.5.0/neuralforecast/losses/numpy.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.4.0/neuralforecast/losses/pytorch.py` & `neuralforecast-1.5.0/neuralforecast/losses/pytorch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/losses.pytorch.ipynb.
 
 # %% auto 0
-__all__ = ['MAE', 'MSE', 'RMSE', 'MAPE', 'SMAPE', 'MASE', 'QuantileLoss', 'Accuracy', 'MQLoss', 'wMQLoss', 'sCRPS',
+__all__ = ['MAE', 'MSE', 'RMSE', 'MAPE', 'SMAPE', 'MASE', 'QuantileLoss', 'Accuracy', 'MQLoss', 'wMQLoss', 'sCRPS', 'relMSE',
            'DistributionLoss', 'PMM', 'GMM', 'NBMM']
 
 # %% ../../nbs/losses.pytorch.ipynb 3
 from typing import Optional, Union, Tuple
 
 import math
 import numpy as np
 import torch
 
 import torch.nn.functional as F
 from torch.distributions import Distribution
 from torch.distributions import Bernoulli, Normal, StudentT, Poisson, NegativeBinomial
 
+from torch.distributions import constraints
+
 # %% ../../nbs/losses.pytorch.ipynb 5
 def _divide_no_nan(a: torch.Tensor, b: torch.Tensor) -> torch.Tensor:
     """
     Auxiliary funtion to handle divide by 0
     """
     div = a / b
     div[div != div] = 0.0
@@ -682,26 +684,77 @@
         y_hat: torch.Tensor,
         mask: Union[torch.Tensor, None] = None,
     ):
         """
         **Parameters:**<br>
         `y`: tensor, Actual values.<br>
         `y_hat`: tensor, Predicted values.<br>
-        `mask`: tensor, Specifies date stamps per serie to consider in loss.<br>
+        `mask`: tensor, Specifies date stamps per series to consider in loss.<br>
 
         **Returns:**<br>
         `scrps`: tensor (single value).
         """
         mql = self.mql(y=y, y_hat=y_hat, mask=mask)
-        norm = torch.sum(y)
+        norm = torch.sum(torch.abs(y))
         unmean = torch.sum(mask)
         scrps = 2 * mql * unmean / (norm + 1e-5)
         return scrps
 
-# %% ../../nbs/losses.pytorch.ipynb 63
+# %% ../../nbs/losses.pytorch.ipynb 62
+class relMSE(torch.nn.Module):
+    """Relative Mean Squared Error
+    Computes Relative Mean Squared Error (relMSE), as proposed by Hyndman & Koehler (2006)
+    as an alternative to percentage errors, to avoid measure unstability.
+    $$ \mathrm{relMSE}(\\mathbf{y}, \\mathbf{\hat{y}}, \\mathbf{\hat{y}}^{naive1}) =
+    \\frac{\mathrm{MSE}(\\mathbf{y}, \\mathbf{\hat{y}})}{\mathrm{MSE}(\\mathbf{y}, \\mathbf{\hat{y}}^{naive1})} $$
+    **Parameters:**<br>
+    `y_train`: numpy array, Training values.<br>
+    **References:**<br>
+    - [Hyndman, R. J and Koehler, A. B. (2006).
+       "Another look at measures of forecast accuracy",
+       International Journal of Forecasting, Volume 22, Issue 4.](https://www.sciencedirect.com/science/article/pii/S0169207006000239)<br>
+    - [Kin G. Olivares, O. Nganba Meetei, Ruijun Ma, Rohan Reddy, Mengfei Cao, Lee Dicker.
+       "Probabilistic Hierarchical Forecasting with Deep Poisson Mixtures.
+       Submitted to the International Journal Forecasting, Working paper available at arxiv.](https://arxiv.org/pdf/2110.13179.pdf)
+    """
+
+    def __init__(self, y_train):
+        super(relMSE, self).__init__()
+        self.y_train = y_train
+        self.mse = MSE()
+        self.is_distribution_output = False
+
+    def __call__(
+        self,
+        y: torch.Tensor,
+        y_hat: torch.Tensor,
+        mask: Union[torch.Tensor, None] = None,
+    ):
+        """
+        **Parameters:**<br>
+        `y`: tensor, Actual values.<br>
+        `y_hat`: tensor, Predicted values.<br>
+        `mask`: tensor, Specifies date stamps per series to consider in loss.<br>
+
+        **Returns:**<br>
+        `relmse`: tensor (single value).
+        """
+        if mask is None:
+            mask = torch.ones_like(y)
+        n_series, horizon = y.shape
+
+        last_col = self.y_train[:, -1].unsqueeze(1)
+        y_naive = last_col.repeat(1, horizon)
+
+        norm = self.mse(y=y, y_hat=y_naive)
+        loss = self.mse(y=y, y_hat=y_hat, mask=mask)
+        loss = loss / (norm + 1e-5)
+        return loss
+
+# %% ../../nbs/losses.pytorch.ipynb 66
 def weighted_average(
     x: torch.Tensor, weights: Optional[torch.Tensor] = None, dim=None
 ) -> torch.Tensor:
     """
     Computes the weighted average of a given tensor across a given dim, masking
     values associated with weight zero,
     meaning instead of `nan * 0 = nan` you will get `0 * 0 = 0`.
@@ -721,15 +774,15 @@
         )
         return (
             weighted_tensor.sum(dim=dim) if dim else weighted_tensor.sum()
         ) / sum_weights
     else:
         return x.mean(dim=dim)
 
-# %% ../../nbs/losses.pytorch.ipynb 64
+# %% ../../nbs/losses.pytorch.ipynb 67
 def bernoulli_domain_map(input: torch.Tensor):
     """Bernoulli Domain Map
     Maps input into distribution constraints, by construction input's
     last dimension is of matching `distr_args` length.
 
     **Parameters:**<br>
     `input`: tensor, of dimensions [B,T,H,theta] or [B,H,theta].<br>
@@ -807,18 +860,15 @@
 
     Stabilizes model's output optimization, by learning residual
     variance and residual location based on anchoring `loc`, `scale`.
     Also adds Normal domain protection to the distribution parameters.
     """
     mean, std = output
     std = F.softplus(std)
-    print("mean.shape", mean.shape)
     if (loc is not None) and (scale is not None):
-        print("scale.shape", scale.shape)
-        print("loc.shape", loc.shape)
         mean = (mean * scale) + loc
         std = (std + eps) * scale
     return (mean, std)
 
 
 def poisson_domain_map(input: torch.Tensor):
     """Poisson Domain Map
@@ -837,18 +887,19 @@
 def poisson_scale_decouple(output, loc=None, scale=None):
     """Poisson Scale Decouple
 
     Stabilizes model's output optimization, by learning residual
     variance and residual location based on anchoring `loc`, `scale`.
     Also adds Poisson domain protection to the distribution parameters.
     """
+    eps = 1e-10
     rate = output[0]
     if (loc is not None) and (scale is not None):
         rate = (rate * scale) + loc
-    rate = F.softplus(rate)  # .clone()
+    rate = F.softplus(rate) + eps
     return (rate,)
 
 
 def nbinomial_domain_map(input: torch.Tensor):
     """Negative Binomial Domain Map
     Maps input into distribution constraints, by construction input's
     last dimension is of matching `distr_args` length.
@@ -880,15 +931,15 @@
     # mu = total_count * (probs/(1-probs))
     # => probs = mu / (total_count + mu)
     # => probs = mu / [total_count * (1 + mu * (1/total_count))]
     total_count = 1.0 / alpha
     probs = (mu * alpha / (1.0 + mu * alpha)) + 1e-8
     return (total_count, probs)
 
-# %% ../../nbs/losses.pytorch.ipynb 65
+# %% ../../nbs/losses.pytorch.ipynb 68
 def est_lambda(mu, rho):
     return mu ** (2 - rho) / (2 - rho)
 
 
 def est_alpha(rho):
     return (2 - rho) / (rho - 1)
 
@@ -1001,15 +1052,15 @@
     Also adds Tweedie domain protection to the distribution parameters.
     """
     log_mu = output[0]
     if (loc is not None) and (scale is not None):
         log_mu += torch.log(loc)  # TODO : rho scaling
     return (log_mu,)
 
-# %% ../../nbs/losses.pytorch.ipynb 67
+# %% ../../nbs/losses.pytorch.ipynb 69
 class DistributionLoss(torch.nn.Module):
     """DistributionLoss
 
     This PyTorch module wraps the `torch.distribution` classes allowing it to
     interact with NeuralForecast models modularly. It shares the negative
     log-likelihood as the optimization objective and a sample method to
     generate empirically the quantiles defined by the `level` list.
@@ -1039,15 +1090,15 @@
     """
 
     def __init__(
         self,
         distribution,
         level=[80, 90],
         quantiles=None,
-        num_samples=500,
+        num_samples=1000,
         return_params=False,
         **distribution_kwargs,
     ):
         super(DistributionLoss, self).__init__()
 
         available_distributions = dict(
             Bernoulli=Bernoulli,
@@ -1104,14 +1155,17 @@
         self.num_samples = num_samples
 
         # If True, predict_step will return Distribution's parameters
         self.return_params = return_params
         if self.return_params:
             self.output_names = self.output_names + self.param_names
 
+        # Add first output entry for the sample_mean
+        self.output_names.insert(0, "")
+
         self.outputsize_multiplier = len(self.param_names)
         self.is_distribution_output = True
 
     def get_distribution(self, distr_args, **distribution_kwargs) -> Distribution:
         """
         Construct the associated Pytorch Distribution, given the collection of
         constructor arguments and, optionally, location and scale tensors.
@@ -1120,14 +1174,17 @@
         `distr_args`: Constructor arguments for the underlying Distribution type.<br>
 
         **Returns**<br>
         `Distribution`: AffineTransformed distribution.<br>
         """
         # TransformedDistribution(distr, [AffineTransform(loc=loc, scale=scale)])
         distr = self._base_distribution(*distr_args, **distribution_kwargs)
+
+        if self.distribution == "Poisson":
+            distr.support = constraints.nonnegative
         return distr
 
     def sample(self, distr_args: torch.Tensor, num_samples: Optional[int] = None):
         """
         Construct the empirical quantiles from the estimated Distribution,
         sampling from it `num_samples` independently.
 
@@ -1151,24 +1208,27 @@
 
         # Instantiate Scaled Decoupled Distribution
         distr = self.get_distribution(distr_args=distr_args, **self.distribution_kwargs)
         samples = distr.sample(sample_shape=(num_samples,))
         samples = samples.permute(1, 2, 0)  # [samples,B,H] -> [B,H,samples]
         samples = samples.to(distr_args[0].device)
         samples = samples.view(B * H, num_samples)
+        sample_mean = torch.mean(samples, dim=-1)
 
         # Compute quantiles
         quantiles_device = self.quantiles.to(distr_args[0].device)
         quants = torch.quantile(input=samples, q=quantiles_device, dim=1)
         quants = quants.permute((1, 0))  # [Q, B*H] -> [B*H, Q]
 
         # Final reshapes
         samples = samples.view(B, H, num_samples)
+        sample_mean = sample_mean.view(B, H, 1)
         quants = quants.view(B, H, Q)
-        return samples, quants
+
+        return samples, sample_mean, quants
 
     def __call__(
         self,
         y: torch.Tensor,
         distr_args: torch.Tensor,
         mask: Union[torch.Tensor, None] = None,
     ):
@@ -1195,15 +1255,15 @@
         """
         # Instantiate Scaled Decoupled Distribution
         distr = self.get_distribution(distr_args=distr_args, **self.distribution_kwargs)
         loss_values = -distr.log_prob(y)
         loss_weights = mask
         return weighted_average(loss_values, weights=loss_weights)
 
-# %% ../../nbs/losses.pytorch.ipynb 73
+# %% ../../nbs/losses.pytorch.ipynb 75
 class PMM(torch.nn.Module):
     """Poisson Mixture Mesh
 
     This Poisson Mixture statistical model assumes independence across groups of
     data $\mathcal{G}=\{[g_{i}]\}$, and estimates relationships within the group.
 
     $$ \mathrm{P}\\left(\mathbf{y}_{[b][t+1:t+H]}\\right) =
@@ -1211,48 +1271,57 @@
     \prod_{\\beta\in[g_{i}]}
     \\left(\sum_{k=1}^{K} w_k \prod_{(\\beta,\\tau) \in [g_i][t+1:t+H]} \mathrm{Poisson}(y_{\\beta,\\tau}, \hat{\\lambda}_{\\beta,\\tau,k}) \\right)$$
 
     **Parameters:**<br>
     `n_components`: int=10, the number of mixture components.<br>
     `level`: float list [0,100], confidence levels for prediction intervals.<br>
     `quantiles`: float list [0,1], alternative to level list, target quantiles.<br>
-    `return_params`: bool=False, wether or not return the Distribution parameters.<br><br>
+    `return_params`: bool=False, wether or not return the Distribution parameters.<br>
+    `batch_correlation`: bool=False, wether or not model batch correlations.<br>
+    `horizon_correlation`: bool=False, wether or not model horizon correlations.<br>
 
     **References:**<br>
     [Kin G. Olivares, O. Nganba Meetei, Ruijun Ma, Rohan Reddy, Mengfei Cao, Lee Dicker.
     Probabilistic Hierarchical Forecasting with Deep Poisson Mixtures. Submitted to the International
     Journal Forecasting, Working paper available at arxiv.](https://arxiv.org/pdf/2110.13179.pdf)
     """
 
     def __init__(
         self,
         n_components=10,
         level=[80, 90],
         quantiles=None,
-        num_samples=500,
+        num_samples=1000,
         return_params=False,
+        batch_correlation=False,
+        horizon_correlation=False,
     ):
         super(PMM, self).__init__()
         # Transform level to MQLoss parameters
         qs, self.output_names = level_to_outputs(level)
         qs = torch.Tensor(qs)
 
         # Transform quantiles to homogeneus output names
         if quantiles is not None:
             _, self.output_names = quantiles_to_outputs(quantiles)
             qs = torch.Tensor(quantiles)
         self.quantiles = torch.nn.Parameter(qs, requires_grad=False)
         self.num_samples = num_samples
+        self.batch_correlation = batch_correlation
+        self.horizon_correlation = horizon_correlation
 
         # If True, predict_step will return Distribution's parameters
         self.return_params = return_params
         if self.return_params:
             self.param_names = [f"-lambda-{i}" for i in range(1, n_components + 1)]
             self.output_names = self.output_names + self.param_names
 
+        # Add first output entry for the sample_mean
+        self.output_names.insert(0, "")
+
         self.outputsize_multiplier = n_components
         self.is_distribution_output = True
 
     def domain_map(self, output: torch.Tensor):
         return (output,)  # , weights
 
     def scale_decouple(
@@ -1322,25 +1391,27 @@
         sample_idxs = sample_idxs.flatten()
 
         sample_lambdas = lambdas[sample_idxs]
 
         # Sample y ~ Poisson(lambda) independently
         samples = torch.poisson(sample_lambdas).to(lambdas.device)
         samples = samples.view(B * H, num_samples)
+        sample_mean = torch.mean(samples, dim=-1)
 
         # Compute quantiles
         quantiles_device = self.quantiles.to(lambdas.device)
         quants = torch.quantile(input=samples, q=quantiles_device, dim=1)
         quants = quants.permute((1, 0))  # Q, B*H
 
         # Final reshapes
         samples = samples.view(B, H, num_samples)
+        sample_mean = sample_mean.view(B, H, 1)
         quants = quants.view(B, H, Q)
 
-        return samples, quants
+        return samples, sample_mean, quants
 
     def neglog_likelihood(
         self,
         y: torch.Tensor,
         distr_args: Tuple[torch.Tensor],
         mask: Union[torch.Tensor, None] = None,
     ):
@@ -1354,40 +1425,43 @@
         B, H, K = lambdas.size()
 
         weights = (1 / K) * torch.ones_like(lambdas).to(lambdas.device)
 
         y = y[:, :, None]
         mask = mask[:, :, None]
 
-        y = y * mask  # Protect target variable negative entries
+        y = y * mask  # Protect y negative entries
 
-        log = y.xlogy(lambdas + eps) - lambdas - (y + 1).lgamma()
+        # Single Poisson likelihood
+        log_pi = y.xlogy(lambdas + eps) - lambdas - (y + 1).lgamma()
 
-        # log  = torch.sum(log, dim=0, keepdim=True) # Joint within batch/group
-        # log  = torch.sum(log, dim=1, keepdim=True) # Joint within horizon
+        if self.batch_correlation:
+            log_pi = torch.sum(log_pi, dim=0, keepdim=True)
 
-        # Numerical stability mixture and loglik
-        log_max = torch.amax(log, dim=2, keepdim=True)  # [1,1,K] (collapsed joints)
-        lik = weights * torch.exp(log - log_max)  # Take max
-        loglik = torch.log(torch.sum(lik, dim=2, keepdim=True)) + log_max  # Return max
-        loglik = loglik * mask  # replace with mask
+        if self.horizon_correlation:
+            log_pi = torch.sum(log_pi, dim=1, keepdim=True)
 
-        loss = -torch.mean(loglik)
+        # Numerically Stable Mixture loglikelihood
+        loglik = torch.logsumexp((torch.log(weights) + log_pi), dim=2, keepdim=True)
+        loglik = loglik * mask
+
+        mean = torch.sum(weights * lambdas, axis=-1, keepdims=True)
+        reglrz = torch.mean(torch.square(y - mean) * mask)
+        loss = -torch.mean(loglik) + 0.001 * reglrz
         return loss
 
     def __call__(
         self,
         y: torch.Tensor,
         distr_args: Tuple[torch.Tensor],
         mask: Union[torch.Tensor, None] = None,
     ):
-
         return self.neglog_likelihood(y=y, distr_args=distr_args, mask=mask)
 
-# %% ../../nbs/losses.pytorch.ipynb 80
+# %% ../../nbs/losses.pytorch.ipynb 83
 class GMM(torch.nn.Module):
     """Gaussian Mixture Mesh
 
     This Gaussian Mixture statistical model assumes independence across groups of
     data $\mathcal{G}=\{[g_{i}]\}$, and estimates relationships within the group.
 
     $$ \mathrm{P}\\left(\mathbf{y}_{[b][t+1:t+H]}\\right) =
@@ -1396,50 +1470,59 @@
     \\left(\sum_{k=1}^{K} w_k \prod_{(\\beta,\\tau) \in [g_i][t+1:t+H]}
     \mathrm{Gaussian}(y_{\\beta,\\tau}, \hat{\mu}_{\\beta,\\tau,k}, \sigma_{\\beta,\\tau,k})\\right)$$
 
     **Parameters:**<br>
     `n_components`: int=10, the number of mixture components.<br>
     `level`: float list [0,100], confidence levels for prediction intervals.<br>
     `quantiles`: float list [0,1], alternative to level list, target quantiles.<br>
-    `return_params`: bool=False, wether or not return the Distribution parameters.<br><br>
+    `return_params`: bool=False, wether or not return the Distribution parameters.<br>
+    `batch_correlation`: bool=False, wether or not model batch correlations.<br>
+    `horizon_correlation`: bool=False, wether or not model horizon correlations.<br><br>
 
     **References:**<br>
     [Kin G. Olivares, O. Nganba Meetei, Ruijun Ma, Rohan Reddy, Mengfei Cao, Lee Dicker.
     Probabilistic Hierarchical Forecasting with Deep Poisson Mixtures. Submitted to the International
     Journal Forecasting, Working paper available at arxiv.](https://arxiv.org/pdf/2110.13179.pdf)
     """
 
     def __init__(
         self,
         n_components=1,
         level=[80, 90],
         quantiles=None,
-        num_samples=500,
+        num_samples=1000,
         return_params=False,
+        batch_correlation=False,
+        horizon_correlation=False,
     ):
         super(GMM, self).__init__()
         # Transform level to MQLoss parameters
         qs, self.output_names = level_to_outputs(level)
         qs = torch.Tensor(qs)
 
         # Transform quantiles to homogeneus output names
         if quantiles is not None:
             _, self.output_names = quantiles_to_outputs(quantiles)
             qs = torch.Tensor(quantiles)
         self.quantiles = torch.nn.Parameter(qs, requires_grad=False)
         self.num_samples = num_samples
+        self.batch_correlation = batch_correlation
+        self.horizon_correlation = horizon_correlation
 
         # If True, predict_step will return Distribution's parameters
         self.return_params = return_params
         if self.return_params:
             mu_names = [f"-mu-{i}" for i in range(1, n_components + 1)]
             std_names = [f"-std-{i}" for i in range(1, n_components + 1)]
             mu_std_names = [i for j in zip(mu_names, std_names) for i in j]
             self.output_names = self.output_names + mu_std_names
 
+        # Add first output entry for the sample_mean
+        self.output_names.insert(0, "")
+
         self.outputsize_multiplier = 2 * n_components
         self.is_distribution_output = True
 
     def domain_map(self, output: torch.Tensor):
         means, stds = torch.tensor_split(output, 2, dim=-1)
         return (means, stds)
 
@@ -1516,76 +1599,75 @@
 
         sample_means = means[sample_idxs]
         sample_stds = stds[sample_idxs]
 
         # Sample y ~ Normal(mu, std) independently
         samples = torch.normal(sample_means, sample_stds).to(means.device)
         samples = samples.view(B * H, num_samples)
+        sample_mean = torch.mean(samples, dim=-1)
 
         # Compute quantiles
         quantiles_device = self.quantiles.to(means.device)
         quants = torch.quantile(input=samples, q=quantiles_device, dim=1)
         quants = quants.permute((1, 0))  # Q, B*H
 
         # Final reshapes
         samples = samples.view(B, H, num_samples)
+        sample_mean = sample_mean.view(B, H, 1)
         quants = quants.view(B, H, Q)
 
-        return samples, quants
+        return samples, sample_mean, quants
 
     def neglog_likelihood(
         self,
         y: torch.Tensor,
         distr_args: Tuple[torch.Tensor, torch.Tensor],
         mask: Union[torch.Tensor, None] = None,
     ):
-
         if mask is None:
             mask = torch.ones_like(y)
 
         means, stds = distr_args
         B, H, K = means.size()
 
         weights = (1 / K) * torch.ones_like(means).to(means.device)
-        # eps  = 1e-10
 
         y = y[:, :, None]
         mask = mask[:, :, None]
 
         var = stds**2
         log_stds = torch.log(stds)
-        log = (
+        log_pi = (
             -((y - means) ** 2 / (2 * var))
             - log_stds
             - math.log(math.sqrt(2 * math.pi))
         )
 
-        # log  = torch.sum(log, dim=0, keepdim=True) # Joint within batch/group
-        # log  = torch.sum(log, dim=1, keepdim=True) # Joint within horizon
+        if self.batch_correlation:
+            log_pi = torch.sum(log_pi, dim=0, keepdim=True)
 
-        # Numerical stability mixture and loglik
-        log_max = torch.amax(log, dim=2, keepdim=True)  # [1,1,K] (collapsed joints)
-        lik = weights * torch.exp(log - log_max)  # Take max
-        loglik = torch.log(torch.sum(lik, dim=2, keepdim=True)) + log_max  # Return max
+        if self.horizon_correlation:
+            log_pi = torch.sum(log_pi, dim=1, keepdim=True)
 
-        loglik = loglik * mask  # replace with mask
+        # Numerically Stable Mixture loglikelihood
+        loglik = torch.logsumexp((torch.log(weights) + log_pi), dim=2, keepdim=True)
+        loglik = loglik * mask
 
         loss = -torch.mean(loglik)
         return loss
 
     def __call__(
         self,
         y: torch.Tensor,
         distr_args: Tuple[torch.Tensor, torch.Tensor],
         mask: Union[torch.Tensor, None] = None,
     ):
-
         return self.neglog_likelihood(y=y, distr_args=distr_args, mask=mask)
 
-# %% ../../nbs/losses.pytorch.ipynb 87
+# %% ../../nbs/losses.pytorch.ipynb 91
 class NBMM(torch.nn.Module):
     """Negative Binomial Mixture Mesh
 
     This N. Binomial Mixture statistical model assumes independence across groups of
     data $\mathcal{G}=\{[g_{i}]\}$, and estimates relationships within the group.
 
     $$ \mathrm{P}\\left(\mathbf{y}_{[b][t+1:t+H]}\\right) =
@@ -1607,15 +1689,15 @@
     """
 
     def __init__(
         self,
         n_components=1,
         level=[80, 90],
         quantiles=None,
-        num_samples=500,
+        num_samples=1000,
         return_params=False,
     ):
         super(NBMM, self).__init__()
         # Transform level to MQLoss parameters
         qs, self.output_names = level_to_outputs(level)
         qs = torch.Tensor(qs)
 
@@ -1632,14 +1714,17 @@
             total_count_names = [
                 f"-total_count-{i}" for i in range(1, n_components + 1)
             ]
             probs_names = [f"-probs-{i}" for i in range(1, n_components + 1)]
             param_names = [i for j in zip(total_count_names, probs_names) for i in j]
             self.output_names = self.output_names + param_names
 
+        # Add first output entry for the sample_mean
+        self.output_names.insert(0, "")
+
         self.outputsize_multiplier = 2 * n_components
         self.is_distribution_output = True
 
     def domain_map(self, output: torch.Tensor):
         mu, alpha = torch.tensor_split(output, 2, dim=-1)
         return (mu, alpha)
 
@@ -1724,33 +1809,34 @@
         sample_total_count = total_count[sample_idxs]
         sample_probs = probs[sample_idxs]
 
         # Sample y ~ NBinomial(total_count, probs) independently
         dist = NegativeBinomial(total_count=sample_total_count, probs=sample_probs)
         samples = dist.sample(sample_shape=(1,)).to(probs.device)[0]
         samples = samples.view(B * H, num_samples)
+        sample_mean = torch.mean(samples, dim=-1)
 
         # Compute quantiles
         quantiles_device = self.quantiles.to(probs.device)
         quants = torch.quantile(input=samples, q=quantiles_device, dim=1)
         quants = quants.permute((1, 0))  # Q, B*H
 
         # Final reshapes
         samples = samples.view(B, H, num_samples)
+        sample_mean = sample_mean.view(B, H, 1)
         quants = quants.view(B, H, Q)
 
-        return samples, quants
+        return samples, sample_mean, quants
 
     def neglog_likelihood(
         self,
         y: torch.Tensor,
         distr_args: Tuple[torch.Tensor, torch.Tensor],
         mask: Union[torch.Tensor, None] = None,
     ):
-
         if mask is None:
             mask = torch.ones_like(y)
 
         total_count, probs = distr_args
         B, H, K = total_count.size()
 
         weights = (1 / K) * torch.ones_like(probs).to(probs.device)
@@ -1784,9 +1870,8 @@
 
     def __call__(
         self,
         y: torch.Tensor,
         distr_args: Tuple[torch.Tensor, torch.Tensor],
         mask: Union[torch.Tensor, None] = None,
     ):
-
         return self.neglog_likelihood(y=y, distr_args=distr_args, mask=mask)
```

### Comparing `neuralforecast-1.4.0/neuralforecast/models/dilated_rnn.py` & `neuralforecast-1.5.0/neuralforecast/models/dilated_rnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,14 +287,15 @@
 # %% ../../nbs/models.dilated_rnn.ipynb 12
 class DilatedRNN(BaseRecurrent):
     """DilatedRNN
 
     **Parameters:**<br>
     `h`: int, forecast horizon.<br>
     `input_size`: int, maximum sequence length for truncated train backpropagation. Default -1 uses all history.<br>
+    `inference_input_size`: int, maximum sequence length for truncated inference. Default -1 uses all history.<br>
     `cell_type`: str, type of RNN cell to use. Options: 'GRU', 'RNN', 'LSTM', 'ResLSTM', 'AttentiveLSTM'.<br>
     `dilations`: int list, dilations betweem layers.<br>
     `encoder_hidden_size`: int=200, units for the RNN's hidden state size.<br>
     `context_size`: int=10, size of context vector for each timestamp on the forecasting window.<br>
     `decoder_hidden_size`: int=200, size of hidden layer for the MLP decoder.<br>
     `decoder_layers`: int=2, number of layers for the MLP decoder.<br>
     `futr_exog_list`: str list, future exogenous columns.<br>
@@ -310,21 +311,26 @@
     `batch_size`: int=32, number of different series in each batch.<br>
     `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
     `step_size`: int=1, step size between each window of temporal data.<br>
     `scaler_type`: str='robust', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int=1, random_seed for pytorch initializer and numpy generators.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
+    `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
     """
 
+    # Class attributes
+    SAMPLING_TYPE = "recurrent"
+
     def __init__(
         self,
         h: int,
         input_size: int = -1,
+        inference_input_size: int = -1,
         cell_type: str = "LSTM",
         dilations: List[List[int]] = [[1, 2], [4, 8]],
         encoder_hidden_size: int = 200,
         context_size: int = 10,
         decoder_hidden_size: int = 200,
         decoder_layers: int = 2,
         futr_exog_list=None,
@@ -345,14 +351,15 @@
         num_workers_loader: int = 0,
         drop_last_loader: bool = False,
         **trainer_kwargs
     ):
         super(DilatedRNN, self).__init__(
             h=h,
             input_size=input_size,
+            inference_input_size=inference_input_size,
             loss=loss,
             valid_loss=valid_loss,
             max_steps=max_steps,
             learning_rate=learning_rate,
             num_lr_decays=num_lr_decays,
             early_stop_patience_steps=early_stop_patience_steps,
             val_check_steps=val_check_steps,
@@ -418,15 +425,14 @@
             hidden_size=self.decoder_hidden_size,
             num_layers=self.decoder_layers,
             activation="ReLU",
             dropout=0.0,
         )
 
     def forward(self, windows_batch):
-
         # Parse windows_batch
         encoder_input = windows_batch["insample_y"]  # [B, seq_len, 1]
         futr_exog = windows_batch["futr_exog"]
         hist_exog = windows_batch["hist_exog"]
         stat_exog = windows_batch["stat_exog"]
 
         # Concatenate y, historic and static inputs
```

### Comparing `neuralforecast-1.4.0/neuralforecast/models/gru.py` & `neuralforecast-1.5.0/neuralforecast/models/gru.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     MLP decoder. The network has `tanh` or `relu` non-linearities, it is trained
     using ADAM stochastic gradient descent. The network accepts static, historic
     and future exogenous data, flattens the inputs.
 
         **Parameters:**<br>
     `h`: int, forecast horizon.<br>
     `input_size`: int, maximum sequence length for truncated train backpropagation. Default -1 uses all history.<br>
+    `inference_input_size`: int, maximum sequence length for truncated inference. Default -1 uses all history.<br>
     `encoder_n_layers`: int=2, number of layers for the GRU.<br>
     `encoder_hidden_size`: int=200, units for the GRU's hidden state size.<br>
     `encoder_activation`: str=`tanh`, type of GRU activation from `tanh` or `relu`.<br>
     `encoder_bias`: bool=True, whether or not to use biases b_ih, b_hh within GRU units.<br>
     `encoder_dropout`: float=0., dropout regularization applied to GRU outputs.<br>
     `context_size`: int=10, size of context vector for each timestamp on the forecasting window.<br>
     `decoder_hidden_size`: int=200, size of hidden layer for the MLP decoder.<br>
@@ -45,21 +46,26 @@
     `val_check_steps`: int=100, Number of training steps between every validation loss check.<br>
     `batch_size`: int=32, number of differentseries in each batch.<br>
     `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
     `scaler_type`: str='robust', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int=1, random_seed for pytorch initializer and numpy generators.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
+    `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
     """
 
+    # Class attributes
+    SAMPLING_TYPE = "recurrent"
+
     def __init__(
         self,
         h: int,
         input_size: int = -1,
+        inference_input_size: int = -1,
         encoder_n_layers: int = 2,
         encoder_hidden_size: int = 200,
         encoder_activation: str = "tanh",
         encoder_bias: bool = True,
         encoder_dropout: float = 0.0,
         context_size: int = 10,
         decoder_hidden_size: int = 200,
@@ -81,14 +87,15 @@
         num_workers_loader=0,
         drop_last_loader=False,
         **trainer_kwargs
     ):
         super(GRU, self).__init__(
             h=h,
             input_size=input_size,
+            inference_input_size=inference_input_size,
             loss=loss,
             valid_loss=valid_loss,
             max_steps=max_steps,
             learning_rate=learning_rate,
             num_lr_decays=num_lr_decays,
             early_stop_patience_steps=early_stop_patience_steps,
             val_check_steps=val_check_steps,
@@ -147,15 +154,14 @@
             hidden_size=self.decoder_hidden_size,
             num_layers=self.decoder_layers,
             activation="ReLU",
             dropout=0.0,
         )
 
     def forward(self, windows_batch):
-
         # Parse windows_batch
         encoder_input = windows_batch["insample_y"]  # [B, seq_len, 1]
         futr_exog = windows_batch["futr_exog"]
         hist_exog = windows_batch["hist_exog"]
         stat_exog = windows_batch["stat_exog"]
 
         # Concatenate y, historic and static inputs
```

### Comparing `neuralforecast-1.4.0/neuralforecast/models/lstm.py` & `neuralforecast-1.5.0/neuralforecast/models/lstm.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     The network has `tanh` or `relu` non-linearities, it is trained using
     ADAM stochastic gradient descent. The network accepts static, historic
     and future exogenous data.
 
     **Parameters:**<br>
     `h`: int, forecast horizon.<br>
     `input_size`: int, maximum sequence length for truncated train backpropagation. Default -1 uses all history.<br>
+    `inference_input_size`: int, maximum sequence length for truncated inference. Default -1 uses all history.<br>
     `encoder_n_layers`: int=2, number of layers for the LSTM.<br>
     `encoder_hidden_size`: int=200, units for the LSTM's hidden state size.<br>
     `encoder_activation`: str=`tanh`, type of LSTM activation from `tanh` or `relu`.<br>
     `encoder_bias`: bool=True, whether or not to use biases b_ih, b_hh within LSTM units.<br>
     `encoder_dropout`: float=0., dropout regularization applied to LSTM outputs.<br>
     `context_size`: int=10, size of context vector for each timestamp on the forecasting window.<br>
     `decoder_hidden_size`: int=200, size of hidden layer for the MLP decoder.<br>
@@ -45,21 +46,26 @@
     `val_check_steps`: int=100, Number of training steps between every validation loss check.<br>
     `batch_size`: int=32, number of differentseries in each batch.<br>
     `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
     `scaler_type`: str='robust', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int=1, random_seed for pytorch initializer and numpy generators.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
+    `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
     """
 
+    # Class attributes
+    SAMPLING_TYPE = "recurrent"
+
     def __init__(
         self,
         h: int,
         input_size: int = -1,
+        inference_input_size: int = -1,
         encoder_n_layers: int = 2,
         encoder_hidden_size: int = 200,
         encoder_bias: bool = True,
         encoder_dropout: float = 0.0,
         context_size: int = 10,
         decoder_hidden_size: int = 200,
         decoder_layers: int = 2,
@@ -80,14 +86,15 @@
         num_workers_loader=0,
         drop_last_loader=False,
         **trainer_kwargs
     ):
         super(LSTM, self).__init__(
             h=h,
             input_size=input_size,
+            inference_input_size=inference_input_size,
             loss=loss,
             valid_loss=valid_loss,
             max_steps=max_steps,
             learning_rate=learning_rate,
             num_lr_decays=num_lr_decays,
             early_stop_patience_steps=early_stop_patience_steps,
             val_check_steps=val_check_steps,
@@ -146,15 +153,14 @@
             hidden_size=self.decoder_hidden_size,
             num_layers=self.decoder_layers,
             activation="ReLU",
             dropout=0.0,
         )
 
     def forward(self, windows_batch):
-
         # Parse windows_batch
         encoder_input = windows_batch["insample_y"]  # [B, seq_len, 1]
         futr_exog = windows_batch["futr_exog"]
         hist_exog = windows_batch["hist_exog"]
         stat_exog = windows_batch["stat_exog"]
 
         # Concatenate y, historic and static inputs
```

### Comparing `neuralforecast-1.4.0/neuralforecast/models/mlp.py` & `neuralforecast-1.5.0/neuralforecast/models/mlp.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,17 +41,21 @@
     `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
     `windows_batch_size`: int=None, windows sampled from rolled data, if None uses all.<br>
     `step_size`: int=1, step size between each window of temporal data.<br>
     `scaler_type`: str='identity', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int=1, random_seed for pytorch initializer and numpy generators.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
+    `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
     """
 
+    # Class attributes
+    SAMPLING_TYPE = "windows"
+
     def __init__(
         self,
         h,
         input_size,
         futr_exog_list=None,
         hist_exog_list=None,
         stat_exog_list=None,
@@ -70,15 +74,14 @@
         step_size: int = 1,
         scaler_type: str = "identity",
         random_seed: int = 1,
         num_workers_loader: int = 0,
         drop_last_loader: bool = False,
         **trainer_kwargs
     ):
-
         # Inherit BaseWindows class
         super(MLP, self).__init__(
             h=h,
             input_size=input_size,
             futr_exog_list=futr_exog_list,
             hist_exog_list=hist_exog_list,
             stat_exog_list=stat_exog_list,
@@ -125,15 +128,14 @@
 
         # Adapter with Loss dependent dimensions
         self.out = nn.Linear(
             in_features=hidden_size, out_features=h * self.loss.outputsize_multiplier
         )
 
     def forward(self, windows_batch):
-
         # Parse windows_batch
         insample_y = windows_batch["insample_y"]
         futr_exog = windows_batch["futr_exog"]
         hist_exog = windows_batch["hist_exog"]
         stat_exog = windows_batch["stat_exog"]
 
         # Flatten MLP inputs [B, L+H, C] -> [B, (L+H)*C]
@@ -154,9 +156,11 @@
                 (insample_y, stat_exog.reshape(batch_size, -1)), dim=1
             )
 
         y_pred = insample_y.clone()
         for layer in self.mlp:
             y_pred = torch.relu(layer(y_pred))
         y_pred = self.out(y_pred)
+
+        y_pred = y_pred.reshape(batch_size, self.h, self.loss.outputsize_multiplier)
         y_pred = self.loss.domain_map(y_pred)
         return y_pred
```

### Comparing `neuralforecast-1.4.0/neuralforecast/models/nbeats.py` & `neuralforecast-1.5.0/neuralforecast/models/nbeats.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,21 +221,25 @@
     `windows_batch_size`: int=None, windows sampled from rolled data, default uses all.<br>
     `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
     `step_size`: int=1, step size between each window of temporal data.<br>
     `scaler_type`: str='identity', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int, random_seed for pytorch initializer and numpy generators.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
+    `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
 
     **References:**<br>
     -[Boris N. Oreshkin, Dmitri Carpov, Nicolas Chapados, Yoshua Bengio (2019).
     "N-BEATS: Neural basis expansion analysis for interpretable time series forecasting".](https://arxiv.org/abs/1905.10437)
     """
 
+    # Class attributes
+    SAMPLING_TYPE = "windows"
+
     def __init__(
         self,
         h,
         input_size,
         n_harmonics: int = 2,
         n_polynomials: int = 2,
         stack_types: list = ["identity", "trend", "seasonality"],
@@ -257,15 +261,14 @@
         step_size: int = 1,
         scaler_type: str = "identity",
         random_seed: int = 1,
         num_workers_loader: int = 0,
         drop_last_loader: bool = False,
         **trainer_kwargs,
     ):
-
         # Inherit BaseWindows class
         super(NBEATS, self).__init__(
             h=h,
             input_size=input_size,
             loss=loss,
             valid_loss=valid_loss,
             max_steps=max_steps,
@@ -308,19 +311,17 @@
         mlp_units,
         dropout_prob_theta,
         activation,
         shared_weights,
         n_polynomials,
         n_harmonics,
     ):
-
         block_list = []
         for i in range(len(stack_types)):
             for block_id in range(n_blocks[i]):
-
                 # Shared weights
                 if shared_weights and block_id > 0:
                     nbeats_block = block_list[-1]
                 else:
                     if stack_types[i] == "seasonality":
                         n_theta = (
                             2
@@ -366,15 +367,14 @@
 
                 # Select type of evaluation and apply it to all layers of block
                 block_list.append(nbeats_block)
 
         return block_list
 
     def forward(self, windows_batch):
-
         # Parse windows_batch
         insample_y = windows_batch["insample_y"]
         insample_mask = windows_batch["insample_mask"]
 
         # NBEATS' forward
         residuals = insample_y.flip(dims=(-1,))  # backcast init
         insample_mask = insample_mask.flip(dims=(-1,))
```

### Comparing `neuralforecast-1.4.0/neuralforecast/models/nbeatsx.py` & `neuralforecast-1.5.0/neuralforecast/models/nbeatsx.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,14 @@
     def forward(
         self,
         insample_y: torch.Tensor,
         futr_exog: torch.Tensor,
         hist_exog: torch.Tensor,
         stat_exog: torch.Tensor,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
-
         # Flatten MLP inputs [B, L+H, C] -> [B, (L+H)*C]
         # Contatenate [ Y_t, | X_{t-L},..., X_{t} | F_{t-L},..., F_{t+H} | S ]
         batch_size = len(insample_y)
         if self.hist_input_size > 0:
             insample_y = torch.cat(
                 (insample_y, hist_exog.reshape(batch_size, -1)), dim=1
             )
@@ -265,21 +264,25 @@
     `windows_batch_size`: int=None, windows sampled from rolled data, default uses all.<br>
     `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
     `step_size`: int=1, step size between each window of temporal data.<br>
     `scaler_type`: str='identity', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int, random seed initialization for replicability.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
+    `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
 
     **References:**<br>
     -[Kin G. Olivares, Cristian Challu, Grzegorz Marcjasz, Rafał Weron, Artur Dubrawski (2021).
     "Neural basis expansion analysis with exogenous variables: Forecasting electricity prices with NBEATSx".](https://arxiv.org/abs/2104.05522)
     """
 
+    # Class attributes
+    SAMPLING_TYPE = "windows"
+
     def __init__(
         self,
         h,
         input_size,
         futr_exog_list=None,
         hist_exog_list=None,
         stat_exog_list=None,
@@ -304,15 +307,14 @@
         step_size: int = 1,
         scaler_type: str = "identity",
         random_seed: int = 1,
         num_workers_loader: int = 0,
         drop_last_loader: bool = False,
         **trainer_kwargs,
     ):
-
         # Inherit BaseWindows class
         super(NBEATSx, self).__init__(
             h=h,
             input_size=input_size,
             futr_exog_list=futr_exog_list,
             hist_exog_list=hist_exog_list,
             stat_exog_list=stat_exog_list,
@@ -374,19 +376,17 @@
         shared_weights,
         n_polynomials,
         n_harmonics,
         futr_input_size,
         hist_input_size,
         stat_input_size,
     ):
-
         block_list = []
         for i in range(len(stack_types)):
             for block_id in range(n_blocks[i]):
-
                 # Shared weights
                 if shared_weights and block_id > 0:
                     nbeats_block = block_list[-1]
                 else:
                     if stack_types[i] == "seasonality":
                         n_theta = (
                             2
@@ -436,15 +436,14 @@
 
                 # Select type of evaluation and apply it to all layers of block
                 block_list.append(nbeats_block)
 
         return block_list
 
     def forward(self, windows_batch):
-
         # Parse windows_batch
         insample_y = windows_batch["insample_y"]
         insample_mask = windows_batch["insample_mask"]
         futr_exog = windows_batch["futr_exog"]
         hist_exog = windows_batch["hist_exog"]
         stat_exog = windows_batch["stat_exog"]
```

### Comparing `neuralforecast-1.4.0/neuralforecast/models/nhits.py` & `neuralforecast-1.5.0/neuralforecast/models/nhits.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         )
         self.forecast_size = forecast_size
         self.backcast_size = backcast_size
         self.interpolation_mode = interpolation_mode
         self.out_features = out_features
 
     def forward(self, theta: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
-
         backcast = theta[:, : self.backcast_size]
         knots = theta[:, self.backcast_size :]
 
         # Interpolation is performed on default dim=-1 := H
         knots = knots.reshape(len(knots), self.out_features, -1)
         if self.interpolation_mode in ["nearest", "linear"]:
             # knots = knots[:,None,:]
@@ -68,15 +67,15 @@
 ACTIVATIONS = ["ReLU", "Softplus", "Tanh", "SELU", "LeakyReLU", "PReLU", "Sigmoid"]
 
 POOLING = ["MaxPool1d", "AvgPool1d"]
 
 
 class NHITSBlock(nn.Module):
     """
-    N-HiTS block which takes a basis function as an argument.
+    NHITS block which takes a basis function as an argument.
     """
 
     def __init__(
         self,
         input_size: int,
         h: int,
         n_theta: int,
@@ -136,15 +135,14 @@
     def forward(
         self,
         insample_y: torch.Tensor,
         futr_exog: torch.Tensor,
         hist_exog: torch.Tensor,
         stat_exog: torch.Tensor,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
-
         # Pooling
         # Pool1d needs 3D input, (B,C,L), adding C dimension
         insample_y = insample_y.unsqueeze(1)
         insample_y = self.pooling_layer(insample_y)
         insample_y = insample_y.squeeze(1)
 
         # Flatten MLP inputs [B, L+H, C] -> [B, (L+H)*C]
@@ -209,22 +207,26 @@
     `windows_batch_size`: int=None, windows sampled from rolled data, default uses all.<br>
     `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
     `step_size`: int=1, step size between each window of temporal data.<br>
     `scaler_type`: str='identity', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int, random_seed for pytorch initializer and numpy generators.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
+    `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
 
     **References:**<br>
     -[Cristian Challu, Kin G. Olivares, Boris N. Oreshkin, Federico Garza,
-    Max Mergenthaler-Canseco, Artur Dubrawski (2022). "N-HiTS: Neural Hierarchical Interpolation for Time Series Forecasting".
+    Max Mergenthaler-Canseco, Artur Dubrawski (2022). "NHITS: Neural Hierarchical Interpolation for Time Series Forecasting".
     Accepted at the Thirty-Seventh AAAI Conference on Artificial Intelligence.](https://arxiv.org/abs/2201.12886)
     """
 
+    # Class attributes
+    SAMPLING_TYPE = "windows"
+
     def __init__(
         self,
         h,
         input_size,
         futr_exog_list=None,
         hist_exog_list=None,
         stat_exog_list=None,
@@ -250,15 +252,14 @@
         step_size: int = 1,
         scaler_type: str = "identity",
         random_seed: int = 1,
         num_workers_loader=0,
         drop_last_loader=False,
         **trainer_kwargs,
     ):
-
         # Inherit BaseWindows class
         super(NHITS, self).__init__(
             h=h,
             input_size=input_size,
             futr_exog_list=futr_exog_list,
             hist_exog_list=hist_exog_list,
             stat_exog_list=stat_exog_list,
@@ -316,19 +317,17 @@
         interpolation_mode,
         dropout_prob_theta,
         activation,
         futr_input_size,
         hist_input_size,
         stat_input_size,
     ):
-
         block_list = []
         for i in range(len(stack_types)):
             for block_id in range(n_blocks[i]):
-
                 assert (
                     stack_types[i] == "identity"
                 ), f"Block type {stack_types[i]} not found!"
 
                 n_theta = input_size + self.loss.outputsize_multiplier * max(
                     h // n_freq_downsample[i], 1
                 )
@@ -356,15 +355,14 @@
 
                 # Select type of evaluation and apply it to all layers of block
                 block_list.append(nbeats_block)
 
         return block_list
 
     def forward(self, windows_batch):
-
         # Parse windows_batch
         insample_y = windows_batch["insample_y"]
         insample_mask = windows_batch["insample_mask"]
         futr_exog = windows_batch["futr_exog"]
         hist_exog = windows_batch["hist_exog"]
         stat_exog = windows_batch["stat_exog"]
```

### Comparing `neuralforecast-1.4.0/neuralforecast/models/rnn.py` & `neuralforecast-1.5.0/neuralforecast/models/rnn.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     The network has `tanh` or `relu` non-linearities, it is trained using
     ADAM stochastic gradient descent. The network accepts static, historic
     and future exogenous data.
 
     **Parameters:**<br>
     `h`: int, forecast horizon.<br>
     `input_size`: int, maximum sequence length for truncated train backpropagation. Default -1 uses all history.<br>
+    `inference_input_size`: int, maximum sequence length for truncated inference. Default -1 uses all history.<br>
     `encoder_n_layers`: int=2, number of layers for the RNN.<br>
     `encoder_hidden_size`: int=200, units for the RNN's hidden state size.<br>
     `encoder_activation`: str=`tanh`, type of RNN activation from `tanh` or `relu`.<br>
     `encoder_bias`: bool=True, whether or not to use biases b_ih, b_hh within RNN units.<br>
     `encoder_dropout`: float=0., dropout regularization applied to RNN outputs.<br>
     `context_size`: int=10, size of context vector for each timestamp on the forecasting window.<br>
     `decoder_hidden_size`: int=200, size of hidden layer for the MLP decoder.<br>
@@ -45,21 +46,26 @@
     `val_check_steps`: int=100, Number of training steps between every validation loss check.<br>
     `batch_size`: int=32, number of differentseries in each batch.<br>
     `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
     `scaler_type`: str='robust', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int=1, random_seed for pytorch initializer and numpy generators.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
+    `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
     """
 
+    # Class attributes
+    SAMPLING_TYPE = "recurrent"
+
     def __init__(
         self,
         h: int,
         input_size: int = -1,
+        inference_input_size: int = -1,
         encoder_n_layers: int = 2,
         encoder_hidden_size: int = 200,
         encoder_activation: str = "tanh",
         encoder_bias: bool = True,
         encoder_dropout: float = 0.0,
         context_size: int = 10,
         decoder_hidden_size: int = 200,
@@ -81,14 +87,15 @@
         num_workers_loader=0,
         drop_last_loader=False,
         **trainer_kwargs
     ):
         super(RNN, self).__init__(
             h=h,
             input_size=input_size,
+            inference_input_size=inference_input_size,
             loss=loss,
             valid_loss=valid_loss,
             max_steps=max_steps,
             learning_rate=learning_rate,
             num_lr_decays=num_lr_decays,
             early_stop_patience_steps=early_stop_patience_steps,
             val_check_steps=val_check_steps,
@@ -149,15 +156,14 @@
             hidden_size=self.decoder_hidden_size,
             num_layers=self.decoder_layers,
             activation="ReLU",
             dropout=0.0,
         )
 
     def forward(self, windows_batch):
-
         # Parse windows_batch
         encoder_input = windows_batch["insample_y"]  # [B, seq_len, 1]
         futr_exog = windows_batch["futr_exog"]
         hist_exog = windows_batch["hist_exog"]
         stat_exog = windows_batch["stat_exog"]
 
         # Concatenate y, historic and static inputs
```

### Comparing `neuralforecast-1.4.0/neuralforecast/models/tcn.py` & `neuralforecast-1.5.0/neuralforecast/models/tcn.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     Temporal Convolution Network (TCN), with MLP decoder.
     The historical encoder uses dilated skip connections to obtain efficient long memory,
     while the rest of the architecture allows for future exogenous alignment.
 
     **Parameters:**<br>
     `h`: int, forecast horizon.<br>
     `input_size`: int, maximum sequence length for truncated train backpropagation. Default -1 uses all history.<br>
+    `inference_input_size`: int, maximum sequence length for truncated inference. Default -1 uses all history.<br>
     `kernel_size`: int, size of the convolving kernel.<br>
     `dilations`: int list, ontrols the temporal spacing between the kernel points; also known as the à trous algorithm.<br>
     `encoder_hidden_size`: int=200, units for the TCN's hidden state size.<br>
     `encoder_activation`: str=`tanh`, type of TCN activation from `tanh` or `relu`.<br>
     `context_size`: int=10, size of context vector for each timestamp on the forecasting window.<br>
     `decoder_hidden_size`: int=200, size of hidden layer for the MLP decoder.<br>
     `decoder_layers`: int=2, number of layers for the MLP decoder.<br>
@@ -41,21 +42,26 @@
     `num_lr_decays`: int=-1, Number of learning rate decays, evenly distributed across max_steps.<br>
     `early_stop_patience_steps`: int=-1, Number of validation iterations before early stopping.<br>
     `val_check_steps`: int=100, Number of training steps between every validation loss check.<br>    `batch_size`: int=32, number of differentseries in each batch.<br>
     `scaler_type`: str='robust', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int=1, random_seed for pytorch initializer and numpy generators.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
+    `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
     """
 
+    # Class attributes
+    SAMPLING_TYPE = "recurrent"
+
     def __init__(
         self,
         h: int,
         input_size: int = -1,
+        inference_input_size: int = -1,
         kernel_size: int = 2,
         dilations: List[int] = [1, 2, 4, 8, 16],
         encoder_hidden_size: int = 200,
         encoder_activation: str = "ReLU",
         context_size: int = 10,
         decoder_hidden_size: int = 200,
         decoder_layers: int = 2,
@@ -76,14 +82,15 @@
         num_workers_loader=0,
         drop_last_loader=False,
         **trainer_kwargs
     ):
         super(TCN, self).__init__(
             h=h,
             input_size=input_size,
+            inference_input_size=inference_input_size,
             loss=loss,
             valid_loss=valid_loss,
             max_steps=max_steps,
             learning_rate=learning_rate,
             num_lr_decays=num_lr_decays,
             early_stop_patience_steps=early_stop_patience_steps,
             val_check_steps=val_check_steps,
@@ -143,15 +150,14 @@
             hidden_size=self.decoder_hidden_size,
             num_layers=self.decoder_layers,
             activation="ReLU",
             dropout=0.0,
         )
 
     def forward(self, windows_batch):
-
         # Parse windows_batch
         encoder_input = windows_batch["insample_y"]  # [B, seq_len, 1]
         futr_exog = windows_batch["futr_exog"]
         hist_exog = windows_batch["hist_exog"]
         stat_exog = windows_batch["stat_exog"]
 
         # Concatenate y, historic and static inputs
```

### Comparing `neuralforecast-1.4.0/neuralforecast/models/tft.py` & `neuralforecast-1.5.0/neuralforecast/models/tft.py`

 * *Files 5% similar despite different names*

```diff
@@ -117,15 +117,14 @@
 
     def _apply_embedding(
         self,
         cont: Optional[Tensor],
         cont_emb: Tensor,
         cont_bias: Tensor,
     ):
-
         if cont is not None:
             # the line below is equivalent to following einsums
             # e_cont = torch.einsum('btf,fh->bthf', cont, cont_emb)
             # e_cont = torch.einsum('bf,fh->bhf', cont, cont_emb)
             e_cont = torch.mul(cont.unsqueeze(-1), cont_emb)
             e_cont = e_cont + cont_bias
             return e_cont
@@ -412,21 +411,25 @@
     `windows_batch_size`: int=None, windows sampled from rolled data, default uses all.<br>
     `valid_batch_size`: int=None, number of different series in each validation and test batch.<br>
     `step_size`: int=1, step size between each window of temporal data.<br>
     `scaler_type`: str='robust', type of scaler for temporal inputs normalization see [temporal scalers](https://nixtla.github.io/neuralforecast/common.scalers.html).<br>
     `random_seed`: int, random seed initialization for replicability.<br>
     `num_workers_loader`: int=os.cpu_count(), workers to be used by `TimeSeriesDataLoader`.<br>
     `drop_last_loader`: bool=False, if True `TimeSeriesDataLoader` drops last non-full batch.<br>
+    `alias`: str, optional,  Custom name of the model.<br>
     `**trainer_kwargs`: int,  keyword trainer arguments inherited from [PyTorch Lighning's trainer](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.trainer.trainer.Trainer.html?highlight=trainer).<br>
 
     **References:**<br>
     - [Bryan Lim, Sercan O. Arik, Nicolas Loeff, Tomas Pfister,
     "Temporal Fusion Transformers for interpretable multi-horizon time series forecasting"](https://www.sciencedirect.com/science/article/pii/S0169207021000637)
     """
 
+    # Class attributes
+    SAMPLING_TYPE = "windows"
+
     def __init__(
         self,
         h,
         input_size,
         tgt_size: int = 1,
         stat_exog_list=None,
         hist_exog_list=None,
@@ -448,15 +451,14 @@
         step_size: int = 1,
         scaler_type: str = "robust",
         num_workers_loader=0,
         drop_last_loader=False,
         random_seed: int = 1,
         **trainer_kwargs
     ):
-
         # Inherit BaseWindows class
         super(TFT, self).__init__(
             h=h,
             input_size=input_size,
             loss=loss,
             valid_loss=valid_loss,
             max_steps=max_steps,
@@ -518,15 +520,14 @@
 
         # Adapter with Loss dependent dimensions
         self.output_adapter = nn.Linear(
             in_features=hidden_size, out_features=self.loss.outputsize_multiplier
         )
 
     def forward(self, x):
-
         # Extract static and temporal features
         y_idx = x["temporal_cols"].get_loc("y")
         y_insample = x["temporal"][:, :, y_idx, None]
 
         # Historic variables
         if len(self.hist_exog_list) > 0:
             hist_exog = x["temporal"][
@@ -607,28 +608,30 @@
     def training_step(self, batch, batch_idx):
         # Deviates from orignal `BaseWindows.training_step` to
         # allow the model to receive future exogenous available
         # at the time of the prediction.
 
         # Create and normalize windows [Ws, L+H, C]
         windows = self._create_windows(batch, step="train")
+        original_outsample_y = torch.clone(windows["temporal"][:, -self.h :, 0])
         windows = self._normalization(windows=windows)
 
         # Parse outsample data
         y_idx = batch["temporal_cols"].get_loc("y")
         mask_idx = batch["temporal_cols"].get_loc("available_mask")
         outsample_y = windows["temporal"][:, -self.h :, y_idx]
         outsample_mask = windows["temporal"][:, -self.h :, mask_idx]
 
         # Model predictions
         output = self(x=windows)
         if self.loss.is_distribution_output:
-            outsample_y, y_loc, y_scale = self._inv_normalization(
+            _, y_loc, y_scale = self._inv_normalization(
                 y_hat=outsample_y, temporal_cols=batch["temporal_cols"]
             )
+            outsample_y = original_outsample_y
             distr_args = self.loss.scale_decouple(
                 output=output, loc=y_loc, scale=y_scale
             )
             loss = self.loss(y=outsample_y, distr_args=distr_args, mask=outsample_mask)
         else:
             loss = self.loss(y=outsample_y, y_hat=output, mask=outsample_mask)
 
@@ -642,53 +645,59 @@
         # at the time of the prediction.
 
         if self.val_size == 0:
             return np.nan
 
         # Create and normalize windows [Ws, L+H, C]
         windows = self._create_windows(batch, step="val")
+        original_outsample_y = torch.clone(windows["temporal"][:, -self.h :, 0])
         windows = self._normalization(windows=windows)
 
         # Parse outsample data
         y_idx = batch["temporal_cols"].get_loc("y")
         mask_idx = batch["temporal_cols"].get_loc("available_mask")
         outsample_y = windows["temporal"][:, -self.h :, y_idx]
         outsample_mask = windows["temporal"][:, -self.h :, mask_idx]
 
         # Model Predictions
         output = self(windows)
         if self.loss.is_distribution_output:
             outsample_y, y_loc, y_scale = self._inv_normalization(
                 y_hat=outsample_y, temporal_cols=batch["temporal_cols"]
             )
+            outsample_y = original_outsample_y
             distr_args = self.loss.scale_decouple(
                 output=output, loc=y_loc, scale=y_scale
             )
-            _, output = self.loss.sample(distr_args=distr_args, num_samples=500)
+            _, sample_mean, quants = self.loss.sample(distr_args=distr_args)
+
+            if str(type(self.valid_loss)) in [
+                "<class 'neuralforecast.losses.pytorch.sCRPS'>",
+                "<class 'neuralforecast.losses.pytorch.MQLoss'>",
+            ]:
+                output = quants
+            elif str(type(self.valid_loss)) in [
+                "<class 'neuralforecast.losses.pytorch.relMSE'>"
+            ]:
+                output = torch.unsqueeze(sample_mean, dim=-1)  # [N,H,1] -> [N,H]
 
         # Validation Loss evaluation
         if self.valid_loss.is_distribution_output:
             valid_loss = self.valid_loss(
                 y=outsample_y, distr_args=distr_args, mask=outsample_mask
             )
         else:
             valid_loss = self.valid_loss(
                 y=outsample_y, y_hat=output, mask=outsample_mask
             )
 
         self.log("valid_loss", valid_loss, prog_bar=True, on_epoch=True)
+        self.validation_step_outputs.append(valid_loss)
         return valid_loss
 
-    def validation_epoch_end(self, outputs):
-        if self.val_size == 0:
-            return
-        avg_loss = torch.stack(outputs).mean()
-        self.log("ptl/val_loss", avg_loss)
-        self.valid_trajectories.append((self.global_step, float(avg_loss)))
-
     def predict_step(self, batch, batch_idx):
         # Deviates from orignal `BaseWindows.training_step` to
         # allow the model to receive future exogenous available
         # at the time of the prediction.
 
         # Create and normalize windows [Ws, L+H, C]
         windows = self._create_windows(batch, step="predict")
@@ -699,15 +708,16 @@
         if self.loss.is_distribution_output:
             _, y_loc, y_scale = self._inv_normalization(
                 y_hat=output[0], temporal_cols=batch["temporal_cols"]
             )
             distr_args = self.loss.scale_decouple(
                 output=output, loc=y_loc, scale=y_scale
             )
-            _, y_hat = self.loss.sample(distr_args=distr_args, num_samples=500)
+            _, sample_mean, quants = self.loss.sample(distr_args=distr_args)
+            y_hat = torch.concat((sample_mean, quants), axis=2)
 
             if self.loss.return_params:
                 distr_args = torch.stack(distr_args, dim=-1)
                 distr_args = torch.reshape(
                     distr_args, (len(windows["temporal"]), self.h, -1)
                 )
                 y_hat = torch.concat((y_hat, distr_args), axis=2)
```

### Comparing `neuralforecast-1.4.0/neuralforecast/tsdataset.py` & `neuralforecast-1.5.0/neuralforecast/tsdataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -196,14 +196,63 @@
             static_cols=dataset.static_cols,
             sorted=dataset.sorted,
         )
 
         return updated_dataset
 
     @staticmethod
+    def trim_dataset(dataset, left_trim: int = 0, right_trim: int = 0):
+        """
+        Trim temporal information from a dataset.
+        Returns temporal indexes [t+left:t-right] for all series.
+        """
+        if dataset.min_size <= left_trim + right_trim:
+            raise Exception(
+                f"left_trim + right_trim ({left_trim} + {right_trim}) \
+                                must be lower than the shorter time series ({dataset.min_size})"
+            )
+
+        # Remove available mask from temporal_cols
+        temporal_cols = dataset.temporal_cols.copy()
+        temporal_cols = temporal_cols.delete(len(temporal_cols) - 1)
+
+        # Define and fill new temporal with trimmed information
+        len_temporal, col_temporal = dataset.temporal.shape
+        total_trim = (left_trim + right_trim) * dataset.n_groups
+        new_temporal = torch.zeros(size=(len_temporal - total_trim, col_temporal))
+        new_indptr = [0]
+
+        acum = 0
+        for i in range(dataset.n_groups):
+            series_length = dataset.indptr[i + 1] - dataset.indptr[i]
+            new_length = series_length - left_trim - right_trim
+            new_temporal[acum : (acum + new_length), :] = dataset.temporal[
+                dataset.indptr[i] + left_trim : dataset.indptr[i + 1] - right_trim, :
+            ]
+            acum += new_length
+            new_indptr.append(acum)
+
+        new_max_size = dataset.max_size - left_trim - right_trim
+        new_min_size = dataset.min_size - left_trim - right_trim
+
+        # Define new dataset
+        updated_dataset = TimeSeriesDataset(
+            temporal=new_temporal,
+            temporal_cols=temporal_cols,
+            indptr=np.array(new_indptr).astype(np.int32),
+            max_size=new_max_size,
+            min_size=new_min_size,
+            static=dataset.static,
+            static_cols=dataset.static_cols,
+            sorted=dataset.sorted,
+        )
+
+        return updated_dataset
+
+    @staticmethod
     def from_df(df, static_df=None, sort_df=False):
         # TODO: protect on equality of static_df + df indexes
         # Define indexes if not given
         if df.index.name != "unique_id":
             df = df.set_index("unique_id")
             if static_df is not None:
                 static_df = static_df.set_index("unique_id")
```

### Comparing `neuralforecast-1.4.0/neuralforecast.egg-info/PKG-INFO` & `neuralforecast-1.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,8 @@
-Metadata-Version: 2.1
-Name: neuralforecast
-Version: 1.4.0
-Summary: Time series forecasting suite using deep learning models
-Home-page: https://github.com/Nixtla/neuralforecast/
-Author: Nixtla
-Author-email: business@nixtla.io
-License: Apache Software License 2.0
-Keywords: time-series forecasting deep-learning
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# Nixtla &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/neuralforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting) &nbsp;[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlaworkspace/shared_invite/zt-135dssye9-fWTzMpv2WBthq8NK0Yvu6A)
+# Nixtla &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/neuralforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting) &nbsp;[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 
 <div align="center">
 <!--- <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast1/main/nbs/imgs_indx/logo_mid.png"> --->
 <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png">
 <h1 align="center">Neural 🧠 Forecast</h1>
 <h3 align="center">User friendly state-of-the-art neural forecasting models.</h3>
 
@@ -71,15 +49,15 @@
 git clone https://github.com/Nixtla/neuralforecast.git
 cd neuralforecast
 pip install -e .
 ```
 </details>
 
 ## 🏃🏻‍♀️🏃 Getting Started
-To get started follow this [guide](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/Getting_Started_with_NBEATS_and_NHITS.ipynb), where we explore `NBEATS`, extend it towards probabilistic predictions and exogenous variables.
+To get started follow this [guide](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/Getting_Started.ipynb), where we explore `NBEATS`, extend it towards probabilistic predictions and exogenous variables.
 
 Or follow this simple example where we train the `NBEATS` model and predict the classic Box-Jenkins air passengers dataset.
 ```python
 import numpy as np
 import pandas as pd
 from IPython.display import display, Markdown
 
@@ -89,21 +67,21 @@
 from neuralforecast.utils import AirPassengersDF
 
 # Split data and declare panel dataset
 Y_df = AirPassengersDF
 Y_train_df = Y_df[Y_df.ds<='1959-12-31'] # 132 train
 Y_test_df = Y_df[Y_df.ds>'1959-12-31'] # 12 test
 
-# Fit and predict with N-BEATS and N-HiTS models
+# Fit and predict with NBEATS and NHITS models
 horizon = len(Y_test_df)
 models = [NBEATS(input_size=2 * horizon, h=horizon, max_epochs=50),
           NHITS(input_size=2 * horizon, h=horizon, max_epochs=50)]
-nforecast = NeuralForecast(models=models, freq='M')
-nforecast.fit(df=Y_train_df)
-Y_hat_df = nforecast.predict().reset_index()
+nf = NeuralForecast(models=models, freq='M')
+nf.fit(df=Y_train_df)
+Y_hat_df = nf.predict().reset_index()
 
 # Plot predictions
 fig, ax = plt.subplots(1, 1, figsize = (20, 7))
 Y_hat_df = Y_test_df.merge(Y_hat_df, how='left', on=['unique_id', 'ds'])
 plot_df = pd.concat([Y_train_df, Y_hat_df]).set_index('ds')
 
 plot_df[['y', 'NBEATS', 'NHITS']].plot(ax=ax, linewidth=2)
@@ -113,50 +91,51 @@
 ax.set_xlabel('Timestamp [t]', fontsize=20)
 ax.legend(prop={'size': 15})
 ax.grid()
 ```
 <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/nbeats_example.png">
 
 ## 🎉 New!
-* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/Getting_Started_with_NBEATS_and_NHITS.ipynb) **Quick Start**: Minimal usage example of the NeuralForecast library on Box's AirPassengers Data.
+* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/Getting_Started.ipynb) **Quick Start**: Minimal usage example of the NeuralForecast library on Box's AirPassengers Data.
 * [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/UncertaintyIntervals.ipynb) **Multi Quantile NBEATS Example**: Produce accurate and efficient probabilistic forecasts in long-horizon settings. Outperforming AutoARIMA's accuracy in a fraction of the time.
-* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/LongHorizon_with_NHITS.ipynb) **Long Horizon N-HiTS Example**:  Load, train, and tune hyperparameters, to achieve Long-Horizon SoTA. Outperform Award Winning Transformers by 25% in 50x less time.
+* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/LongHorizon_with_NHITS.ipynb) **Long Horizon NHITS Example**:  Load, train, and tune hyperparameters, to achieve Long-Horizon SoTA. Outperform Award Winning Transformers by 25% in 50x less time.
+* [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nixtla/neuralforecast/blob/main/nbs/examples/HierarchicalNetworks.ipynb) **Hierarchical Forecasting HINT Example**:  Obtain accurate probabilistic coherent predictions for hierarchical datasets.
 
 ## 🔥  Highlights
 
 * Unified `StatsForecast` interface `NeuralForecast().fit(Y_df).predict(h=7)`.
 * Industry/Competition proven `ESRNN`, `NBEATS`, and `TFT` implementations.
 * Improve accuracy and speed over classic `ARIMA`/`ETS` in two lines of code. Check the experiments [here](xXmissingXx).
-* Predict Series with little to no history, using Transfer learning. Check the experiments [here](xXmissingXx).
+* Predict Series with little to no history, using Transfer learning. Check the experiments [here](https://github.com/Nixtla/transfer-learning-time-series).
 
 ## 🎊 Features 
 
 * **Exogenous Variables**: Static, lagged and future exogenous support.
 * **Forecast Interpretability**: Plot trend, seasonality and exogenous `NBEATS`, `NHITS`, `TFT`, `ESRNN` prediction components.
 * **Probabilistic Forecasting**: Simple model adapters for quantile losses and parametric distributions.
 * **Train and Evaluation Losses** Scale-dependent, percentage and scale independent errors, and parametric likelihoods.
 * **Automatic Model Selection** Parallelized automatic hyperparameter tuning, that efficiently searches best validation configuration.
 * **Simple Interface** Unified SKLearn Interface for `StatsForecast` and `MLForecast` compatibility.
-* **Model Collection**: Out of the box implementation of `MLP`, `LSTM`, `RNN`, `TCN`, `DilatedRNN`, `NBEATS`, `NHITS`, `ESRNN`, `AutoFormer`, `Informer`, `TFT`, `AutoFormer`, `Informer`, and vanilla `Transformer`. See the entire [collection here](https://nixtla.github.io/neuralforecast/models.html).
+* **Model Collection**: Out of the box implementation of `MLP`, `LSTM`, `RNN`, `TCN`, `DilatedRNN`, `NBEATS`, `NHITS`, `ESRNN`, `TFT`, `Informer`, `PatchTST` and `HINT`. See the entire [collection here](https://nixtla.github.io/neuralforecast/models.html).
 
 Missing something? Please open an issue or write us in [![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlaworkspace/shared_invite/zt-135dssye9-fWTzMpv2WBthq8NK0Yvu6A)
 
 ## 📖 Why? 
 
 There is a shared belief in Neural forecasting methods' capacity to improve our pipeline's accuracy and efficiency.
 
 Unfortunately, available implementations and published research are yet to realize neural networks' potential. They are hard to use and continuously fail to improve over statistical methods while being computationally prohibitive. For this reason, we created `NeuralForecast`, a library favoring proven accurate and efficient models focusing on their usability.
 
 ## 🔬 Accuracy & ⏲ Speed 
 
 ### Industry/Competition Proven Methods
-An extensive empirical evaluation is critical to generate confidence and promote the adoption and development of novel methods. For this reason, we replicate and verify the results of our implementation of the following industry/competition-proven methods: `ESRNN`, `NBEATS`, `NHITS`, and `TFT`. If you are interested in reproducing the results, check the experiments [here](xXmissingXx).
+An extensive empirical evaluation is critical to generate confidence and promote the adoption and development of novel methods. For this reason, we replicate and verify the results of our implementation of the following industry/competition-proven methods: `ESRNN`, `NBEATS`, `NHITS`, and `TFT`. If you are interested in reproducing the results, check the experiments [here](https://github.com/Nixtla/neuralforecast/blob/main/nbs/experiments/).
 
 ### Simple and Efficient Method's Comparison
-Like `core.StatsForecast`, the `core.NeuralForecast` wrapper class allows us to easily compare any model in the collection to select or ensemble the best performing methods. Aditionally it offers a high-end interface that operates with (potentially large) sets of time series data stored in pandas DataFrames. The `core.NeuralForecast` efficiently parallelizes computation across CPU or GPU resources. Check the experiments [here](xXmissingXx).
+Like `core.StatsForecast`, the `core.NeuralForecast` wrapper class allows us to easily compare any model in the collection to select or ensemble the best performing methods. Aditionally it offers a high-end interface that operates with (potentially large) sets of time series data stored in pandas DataFrames. The `core.NeuralForecast` efficiently parallelizes computation across GPU resources. Check the experiments [here](https://github.com/Nixtla/neuralforecast/blob/main/nbs/examples/Getting_Started_complete.ipynb).
 
 ## 📖 Documentation (WIP)
 The [documentation page](https://nixtla.github.io/neuralforecast/) contains the models' code documentation, methods, utils, and other tutorials. Docstrings accompany most code.
 
 ## 🔨 How to contribute
 If you wish to contribute to the project, please refer to our [contribution guidelines](https://github.com/Nixtla/neuralforecast/blob/main/CONTRIBUTING.md).
```

### Comparing `neuralforecast-1.4.0/neuralforecast.egg-info/SOURCES.txt` & `neuralforecast-1.5.0/neuralforecast.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,25 +14,32 @@
 neuralforecast.egg-info/dependency_links.txt
 neuralforecast.egg-info/entry_points.txt
 neuralforecast.egg-info/not-zip-safe
 neuralforecast.egg-info/requires.txt
 neuralforecast.egg-info/top_level.txt
 neuralforecast/common/__init__.py
 neuralforecast/common/_base_auto.py
+neuralforecast/common/_base_multivariate.py
 neuralforecast/common/_base_recurrent.py
 neuralforecast/common/_base_windows.py
 neuralforecast/common/_modules.py
 neuralforecast/common/_scalers.py
 neuralforecast/losses/__init__.py
 neuralforecast/losses/numpy.py
 neuralforecast/losses/pytorch.py
 neuralforecast/models/__init__.py
+neuralforecast/models/autoformer.py
 neuralforecast/models/dilated_rnn.py
 neuralforecast/models/gru.py
+neuralforecast/models/hint.py
+neuralforecast/models/informer.py
 neuralforecast/models/lstm.py
 neuralforecast/models/mlp.py
 neuralforecast/models/nbeats.py
 neuralforecast/models/nbeatsx.py
 neuralforecast/models/nhits.py
+neuralforecast/models/patchtst.py
 neuralforecast/models/rnn.py
+neuralforecast/models/stemgnn.py
 neuralforecast/models/tcn.py
-neuralforecast/models/tft.py
+neuralforecast/models/tft.py
+neuralforecast/models/vanillatransformer.py
```

### Comparing `neuralforecast-1.4.0/settings.ini` & `neuralforecast-1.5.0/settings.ini`

 * *Files 7% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 user = Nixtla
 description = Time series forecasting suite using deep learning models
 keywords = time-series forecasting deep-learning 
 author = Nixtla
 author_email = business@nixtla.io
 copyright = Nixtla Inc.
 branch = main
-version = 1.4.0
-min_python = 3.7
+version = 1.5.0
+min_python = 3.8
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 2
-requirements = numpy>=1.21.6 pandas>=1.3.5 torch>=1.12.1 pytorch-lightning==1.6.5 ray[tune]==2.0.1
-dev_requirements = nbdev black mypy flake8 matplotlib
+requirements = numpy>=1.21.6 pandas>=1.3.5 torch>=2.0.0 pytorch-lightning>=2.0.0 ray[tune]>=2.2.0
+dev_requirements = nbdev black mypy flake8 matplotlib hyperopt
 nbs_path = nbs
 doc_path = _docs
 recursive = True
 doc_host =  https://%(user)s.github.io
 doc_baseurl = /neuralforecast/
 git_url = https://github.com/%(user)s/neuralforecast/
 lib_path = %(lib_name)s
```

### Comparing `neuralforecast-1.4.0/setup.py` & `neuralforecast-1.5.0/setup.py`

 * *Files identical despite different names*

