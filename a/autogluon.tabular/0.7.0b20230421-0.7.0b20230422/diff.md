# Comparing `tmp/autogluon.tabular-0.7.0b20230421.tar.gz` & `tmp/autogluon.tabular-0.7.0b20230422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.tabular-0.7.0b20230421.tar", last modified: Fri Apr 21 09:04:06 2023, max compression
+gzip compressed data, was "autogluon.tabular-0.7.0b20230422.tar", last modified: Sat Apr 22 09:04:12 2023, max compression
```

## Comparing `autogluon.tabular-0.7.0b20230421.tar` & `autogluon.tabular-0.7.0b20230422.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.668425 autogluon.tabular-0.7.0b20230421/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.672425 autogluon.tabular-0.7.0b20230421/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.672425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.672425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/configs/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/configs/feature_generator_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/configs/hyperparameter_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.672425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47558 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/learner/abstract_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/learner/default_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.672425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.672425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/_utils/rapids_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.672425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/automm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/automm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/automm/automm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/automm/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.672425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15527 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/catboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/catboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.672425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.672425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/fastai_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.672425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/imports_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/quantile_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25059 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.672425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fasttext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fasttext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fasttext/fasttext_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.672425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fasttext/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.676425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/image_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/image_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/image_prediction/image_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.676425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/imodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/imodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/imodels/imodels_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.676425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/knn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/knn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/knn/_knn_loo_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/knn/knn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/knn/knn_rapids_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/knn/knn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.676425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lgb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lgb/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.676425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lgb/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lgb/lgb_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lgb/lgb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.676425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.676425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lr/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lr/lr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lr/lr_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.676425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/rf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/rf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.676425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/rf/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/rf/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/rf/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/rf/compilers/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/rf/rf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36321 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/rf/rf_quantile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/rf/rf_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.676425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.676425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/pretexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.676425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.676425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/mxnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/mxnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/mxnet/embednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/mxnet/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    37284 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_mxnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30442 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/text_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/text_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/vowpalwabbit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/vowpalwabbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xgboost/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xgboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xgboost/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xgboost/xgboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xt/xt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   249695 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/predictor/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/trainer/model_presets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/trainer/model_presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19038 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/trainer/model_presets/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/trainer/model_presets/presets_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/trainer/model_presets/presets_distill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.680425 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-04-21 09:03:38.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/tuning/feature_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-21 09:04:06.000000 autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:04:06.672425 autogluon.tabular-0.7.0b20230421/src/autogluon.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-21 09:04:06.000000 autogluon.tabular-0.7.0b20230421/src/autogluon.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-21 09:04:06.000000 autogluon.tabular-0.7.0b20230421/src/autogluon.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:04:06.000000 autogluon.tabular-0.7.0b20230421/src/autogluon.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 09:04:06.000000 autogluon.tabular-0.7.0b20230421/src/autogluon.tabular.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-21 09:04:06.000000 autogluon.tabular-0.7.0b20230421/src/autogluon.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 09:04:06.000000 autogluon.tabular-0.7.0b20230421/src/autogluon.tabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:04:06.000000 autogluon.tabular-0.7.0b20230421/src/autogluon.tabular.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.262043 autogluon.tabular-0.7.0b20230422/
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-22 09:04:12.262043 autogluon.tabular-0.7.0b20230422/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 09:04:12.262043 autogluon.tabular-0.7.0b20230422/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.234043 autogluon.tabular-0.7.0b20230422/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.238043 autogluon.tabular-0.7.0b20230422/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.238043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.238043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/configs/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/configs/feature_generator_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/configs/hyperparameter_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.242043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47558 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/learner/abstract_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/learner/default_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.242043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.242043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/_utils/rapids_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.242043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/automm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/automm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/automm/automm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/automm/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.242043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/catboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/catboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.242043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.242043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/fastai_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.242043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/imports_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/quantile_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25059 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.246043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fasttext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fasttext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fasttext/fasttext_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.246043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fasttext/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.246043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/image_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/image_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/image_prediction/image_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.246043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/imodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/imodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/imodels/imodels_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.246043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/knn/_knn_loo_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/knn/knn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/knn/knn_rapids_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/knn/knn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.246043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lgb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lgb/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.246043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lgb/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lgb/lgb_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lgb/lgb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.250043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.250043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lr/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lr/lr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lr/lr_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.250043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/rf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.250043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/rf/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/rf/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/rf/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/rf/compilers/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/rf/rf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36321 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/rf/rf_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/rf/rf_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.250043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.254043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/pretexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.254043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.254043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.254043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.254043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/mxnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/mxnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/mxnet/embednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/mxnet/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37284 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_mxnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.254043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30442 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.254043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.258043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/text_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/text_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.258043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/vowpalwabbit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/vowpalwabbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.258043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xgboost/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.258043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xgboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xgboost/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xgboost/xgboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.258043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xt/xt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.258043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   249695 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/predictor/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.258043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.258043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/trainer/model_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/trainer/model_presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19045 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/trainer/model_presets/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/trainer/model_presets/presets_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/trainer/model_presets/presets_distill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.262043 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-04-22 09:03:34.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/tuning/feature_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-22 09:04:12.000000 autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:04:12.238043 autogluon.tabular-0.7.0b20230422/src/autogluon.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-22 09:04:12.000000 autogluon.tabular-0.7.0b20230422/src/autogluon.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-22 09:04:12.000000 autogluon.tabular-0.7.0b20230422/src/autogluon.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:04:12.000000 autogluon.tabular-0.7.0b20230422/src/autogluon.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-22 09:04:12.000000 autogluon.tabular-0.7.0b20230422/src/autogluon.tabular.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-22 09:04:12.000000 autogluon.tabular-0.7.0b20230422/src/autogluon.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-22 09:04:12.000000 autogluon.tabular-0.7.0b20230422/src/autogluon.tabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:04:12.000000 autogluon.tabular-0.7.0b20230422/src/autogluon.tabular.egg-info/zip-safe
```

### Comparing `autogluon.tabular-0.7.0b20230421/PKG-INFO` & `autogluon.tabular-0.7.0b20230422/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.7.0b20230421
+Version: 0.7.0b20230422
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-0.7.0b20230421/setup.py` & `autogluon.tabular-0.7.0b20230422/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ]
 
 extras_require = {
     'lightgbm': [
         'lightgbm>=3.3,<3.4',
     ],
     'catboost': [
-        'catboost>=1.0,<1.2',
+        'catboost>=1.1,<1.2',
     ],
     # FIXME: Debug why xgboost 1.6 has 4x+ slower inference on multiclass datasets compared to 1.4
     #  It is possibly only present on MacOS, haven't tested linux.
     # XGBoost made API breaking changes in 1.6 with custom metric and callback support, so we don't support older versions.
     'xgboost': [
         'xgboost>=1.6,<1.8',
     ],
```

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/configs/config_helper.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/configs/config_helper.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/configs/feature_generator_presets.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/configs/feature_generator_presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/configs/hyperparameter_configs.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/configs/hyperparameter_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/configs/presets_configs.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/learner/abstract_learner.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/learner/default_learner.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/learner/default_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/__init__.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/_utils/rapids_utils.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/_utils/rapids_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/_utils/torch_utils.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/automm/automm_model.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/automm/automm_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/automm/ft_transformer.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/automm/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/callbacks.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/callbacks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 
 import logging
 import time
 
 from autogluon.common.utils.resource_utils import ResourceManager
 
+from .catboost_utils import CATBOOST_QUANTILE_PREFIX
+
+
 logger = logging.getLogger(__name__)
 
 
 class MemoryCheckCallback:
     """
     Callback to ensure memory usage is safe, otherwise early stops the model to avoid OOM errors.
 
@@ -132,18 +135,25 @@
         else:
             is_max_optimal = eval_metric.is_max_optimal()
             # FIXME: Unsure if this works for custom metrics!
             eval_metric_name = eval_metric.__class__.__name__
 
         self.eval_metric_name = eval_metric_name
         self.is_max_optimal = is_max_optimal
+        self.is_quantile = self.eval_metric_name.startswith(CATBOOST_QUANTILE_PREFIX)
 
     def after_iteration(self, info):
         is_best_iter = False
-        cur_score = info.metrics[self.compare_key][self.eval_metric_name][-1]
+        if self.is_quantile:
+            # FIXME: CatBoost adds extra ',' in the metric name if quantile levels are not balanced
+            # e.g., 'MultiQuantile:alpha=0.1,0.25,0.5,0.95' becomes 'MultiQuantile:alpha=0.1,,0.25,0.5,0.95'
+            eval_metric_name = [k for k in info.metrics[self.compare_key] if k.startswith(CATBOOST_QUANTILE_PREFIX)][0]
+        else:
+            eval_metric_name = self.eval_metric_name
+        cur_score = info.metrics[self.compare_key][eval_metric_name][-1]
         if not self.is_max_optimal:
             cur_score *= -1
         if self.best_score is None:
             self.best_score = cur_score
         elif cur_score > self.best_score:
             is_best_iter = True
             self.best_score = cur_score
```

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/catboost_model.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/catboost_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import time
 import numpy as np
 
 from autogluon.common.features.types import R_BOOL, R_INT, R_FLOAT, R_CATEGORY
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
 from autogluon.common.utils.resource_utils import ResourceManager
-from autogluon.core.constants import PROBLEM_TYPES_CLASSIFICATION, MULTICLASS, SOFTCLASS
+from autogluon.core.constants import PROBLEM_TYPES_CLASSIFICATION, MULTICLASS, QUANTILE, SOFTCLASS
 from autogluon.core.models import AbstractModel
 from autogluon.core.models._utils import get_early_stopping_rounds
 from autogluon.core.utils.exceptions import TimeLimitExceeded
 from autogluon.common.utils.try_import import try_import_catboost
 
 from .callbacks import EarlyStoppingCallback, MemoryCheckCallback, TimeCheckCallback
 from .catboost_utils import get_catboost_metric_from_ag_metric
@@ -35,15 +35,16 @@
         default_params = get_param_baseline(problem_type=self.problem_type)
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
         self._set_default_param_value('random_seed', 0)  # Remove randomness for reproducibility
         # Set 'allow_writing_files' to True in order to keep log files created by catboost during training (these will be saved in the directory where AutoGluon stores this model)
         self._set_default_param_value('allow_writing_files', False)  # Disables creation of catboost logging files during training by default
         if self.problem_type != SOFTCLASS:  # TODO: remove this after catboost 0.24
-            self._set_default_param_value('eval_metric', get_catboost_metric_from_ag_metric(self.stopping_metric, self.problem_type))
+            default_eval_metric = get_catboost_metric_from_ag_metric(self.stopping_metric, self.problem_type, self.quantile_levels)
+            self._set_default_param_value('eval_metric', default_eval_metric)
 
     def _get_default_searchspace(self):
         return get_default_searchspace(self.problem_type, num_classes=self.num_classes)
 
     def _preprocess_nonadaptive(self, X, **kwargs):
         X = super()._preprocess_nonadaptive(X, **kwargs)
         if self._category_features is None:
@@ -84,14 +85,17 @@
         params = self._get_model_params()
         params['thread_count'] = num_cpus
         if self.problem_type == SOFTCLASS:
             # FIXME: This is extremely slow due to unoptimized metric / objective sent to CatBoost
             from .catboost_softclass_utils import SoftclassCustomMetric, SoftclassObjective
             params['loss_function'] = SoftclassObjective.SoftLogLossObjective()
             params['eval_metric'] = SoftclassCustomMetric.SoftLogLossMetric()
+        elif self.problem_type == QUANTILE:
+            # FIXME: Unless specified, CatBoost defaults to loss_function='MultiQuantile' and raises an exception
+            params['loss_function'] = params['eval_metric']
 
         model_type = CatBoostClassifier if self.problem_type in PROBLEM_TYPES_CLASSIFICATION else CatBoostRegressor
         num_rows_train = len(X)
         num_cols_train = len(X.columns)
         num_classes = self.num_classes if self.num_classes else 1  # self.num_classes could be None after initialization if it's a regression problem
 
         X = self.preprocess(X)
@@ -189,15 +193,14 @@
                     model_type=model_type,
                 )
             if early_stopping_rounds is not None:
                 if isinstance(early_stopping_rounds, int):
                     extra_fit_kwargs['early_stopping_rounds'] = early_stopping_rounds
                 elif isinstance(early_stopping_rounds, tuple):
                     extra_fit_kwargs['early_stopping_rounds'] = 50
-
         self.model = model_type(**params)
 
         # TODO: Custom metrics don't seem to work anymore
         # TODO: Custom metrics not supported in GPU mode
         # TODO: Callbacks not supported in GPU mode
         fit_final_kwargs = dict(
             eval_set=eval_set,
```

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/catboost_utils.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/catboost_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
 
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, SOFTCLASS
+from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION, SOFTCLASS
 
 logger = logging.getLogger(__name__)
 
 
+CATBOOST_QUANTILE_PREFIX = 'MultiQuantile:'
+
+
 # TODO: Add weight support?
 # TODO: Can these be optimized? What computational cost do they have compared to the default catboost versions?
 class CustomMetric:
     def __init__(self, metric, is_higher_better, needs_pred_proba):
         self.metric = metric
         self.is_higher_better = is_higher_better
         self.needs_pred_proba = needs_pred_proba
@@ -20,15 +23,15 @@
     def is_max_optimal(self):
         return self.is_higher_better
 
     def evaluate(self, approxes, target, weight):
         raise NotImplementedError
 
 
-def get_catboost_metric_from_ag_metric(metric, problem_type):
+def get_catboost_metric_from_ag_metric(metric, problem_type, quantile_levels=None):
     if problem_type == SOFTCLASS:
         from .catboost_softclass_utils import SoftclassCustomMetric
         if metric.name != 'soft_log_loss':
             logger.warning("Setting metric=soft_log_loss, the only metric supported for softclass problem_type")
         return SoftclassCustomMetric(metric=None, is_higher_better=True, needs_pred_proba=True)
     elif problem_type == BINARY:
         metric_map = dict(
@@ -61,11 +64,18 @@
             mean_squared_error='RMSE',
             root_mean_squared_error='RMSE',
             mean_absolute_error='MAE',
             median_absolute_error='MedianAbsoluteError',
             r2='R2',
         )
         metric_class = metric_map.get(metric.name, 'RMSE')
+    elif problem_type == QUANTILE:
+        if quantile_levels is None:
+            raise AssertionError(f'quantile_levels must be provided for problem_type = {problem_type}')
+        if not all(0 < q < 1 for q in quantile_levels):
+            raise AssertionError(f'quantile_levels must fulfill 0 < q < 1, provided quantile_levels: {quantile_levels}')
+        quantile_string = ','.join(str(q) for q in quantile_levels)
+        metric_class = f'{CATBOOST_QUANTILE_PREFIX}alpha={quantile_string}'
     else:
         raise AssertionError(f'CatBoost does not support {problem_type} problem type.')
 
     return metric_class
```

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/callbacks.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/fastai_helpers.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/fastai_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/quantile_helpers.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/quantile_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fasttext/fasttext_model.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fasttext/fasttext_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/image_prediction/image_predictor.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/image_prediction/image_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/imodels/imodels_models.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/imodels/imodels_models.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/knn/_knn_loo_variants.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/knn/_knn_loo_variants.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/knn/knn_model.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/knn/knn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/knn/knn_rapids_model.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/knn/knn_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/knn/knn_utils.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/knn/knn_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lgb/callbacks.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lgb/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lgb/lgb_model.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lgb/lgb_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lgb/lgb_utils.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lgb/lgb_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lr/hyperparameters/parameters.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lr/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lr/lr_model.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lr/lr_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/lr/lr_rapids_model.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/lr/lr_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/rf/compilers/native.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/rf/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/rf/compilers/onnx.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/rf/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/rf/rf_model.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/rf/rf_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/rf/rf_quantile.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/rf/rf_quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/rf/rf_rapids_model.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/rf/rf_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/modified_transformer.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/modified_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/pretexts.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/pretexts.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/tab_model_base.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/tab_model_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/tab_transformer.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tab_transformer/utils.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tab_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/compilers/native.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/mxnet/embednet.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/mxnet/embednet.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/mxnet/lr_scheduler.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/mxnet/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_dataset.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_mxnet.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_mxnet.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xgboost/callbacks.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xgboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xgboost/xgboost_model.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xgboost/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xgboost/xgboost_utils.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xgboost/xgboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/models/xt/xt_model.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/models/xt/xt_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/predictor/predictor.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/trainer/auto_trainer.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/trainer/model_presets/presets.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/trainer/model_presets/presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     CAT=60,
     custom=0,
 )
 
 DEFAULT_CUSTOM_MODEL_PRIORITY = 0
 
 # FIXME: v0.7 : Remove this, it is a hack. Model classes should define what problem types they support instead of using this
-DEFAULT_QUANTILE_MODEL = ['DUMMY', 'RF', 'XT', 'FASTAI', 'NN_TORCH', 'ENS_WEIGHTED']  # TODO: OTHERS will be added
+DEFAULT_QUANTILE_MODEL = ['DUMMY', 'RF', 'XT', 'FASTAI', 'NN_TORCH', 'ENS_WEIGHTED', 'CAT']  # TODO: OTHERS will be added
 
 MODEL_TYPES = dict(
     RF=RFModel,
     XT=XTModel,
     KNN=KNNModel,
     GBM=LGBModel,
     CAT=CatBoostModel,
```

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/trainer/model_presets/presets_custom.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/trainer/model_presets/presets_custom.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/trainer/model_presets/presets_distill.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/trainer/model_presets/presets_distill.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon/tabular/tuning/feature_pruner.py` & `autogluon.tabular-0.7.0b20230422/src/autogluon/tabular/tuning/feature_pruner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon.tabular.egg-info/PKG-INFO` & `autogluon.tabular-0.7.0b20230422/src/autogluon.tabular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.7.0b20230421
+Version: 0.7.0b20230422
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-0.7.0b20230421/src/autogluon.tabular.egg-info/SOURCES.txt` & `autogluon.tabular-0.7.0b20230422/src/autogluon.tabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

