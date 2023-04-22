# Comparing `tmp/spotRiver-0.0.91.tar.gz` & `tmp/spotRiver-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotRiver-0.0.91.tar", last modified: Wed Apr 19 20:56:29 2023, max compression
+gzip compressed data, was "spotRiver-0.0.92.tar", last modified: Sat Apr 22 19:32:22 2023, max compression
```

## Comparing `spotRiver-0.0.91.tar` & `spotRiver-0.0.92.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.738029 spotRiver-0.0.91/
--rw-r--r--   0 bartz      (501) staff       (20)     1520 2023-01-29 11:49:35.000000 spotRiver-0.0.91/LICENSE
--rw-r--r--   0 bartz      (501) staff       (20)      164 2023-03-22 20:43:16.000000 spotRiver-0.0.91/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     3383 2023-04-19 20:56:29.737903 spotRiver-0.0.91/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     2912 2023-01-29 16:41:52.000000 spotRiver-0.0.91/README.md
--rw-r--r--   0 bartz      (501) staff       (20)     1046 2023-04-19 18:27:37.000000 spotRiver-0.0.91/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2023-04-19 20:56:29.738063 spotRiver-0.0.91/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.729949 spotRiver-0.0.91/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.730449 spotRiver-0.0.91/src/spotRiver/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.734688 spotRiver-0.0.91/src/spotRiver/data/
--rw-r--r--   0 bartz      (501) staff       (20)      413 2023-01-29 11:52:00.000000 spotRiver-0.0.91/src/spotRiver/data/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)     2182 2023-01-17 12:39:58.000000 spotRiver-0.0.91/src/spotRiver/data/airline-passengers.csv
--rw-r--r--   0 bartz      (501) staff       (20)     1023 2023-03-27 20:31:30.000000 spotRiver-0.0.91/src/spotRiver/data/airline_passengers.py
--rw-r--r--   0 bartz      (501) staff       (20)    13646 2023-03-22 20:37:51.000000 spotRiver-0.0.91/src/spotRiver/data/base.py
--rw-r--r--   0 bartz      (501) staff       (20)     1113 2023-03-13 20:26:53.000000 spotRiver-0.0.91/src/spotRiver/data/bike_sharing.py
--rw-r--r--   0 bartz      (501) staff       (20)     1870 2023-03-07 16:50:39.000000 spotRiver-0.0.91/src/spotRiver/data/generic.py
--rw-r--r--   0 bartz      (501) staff       (20)     7751 2023-03-07 16:50:39.000000 spotRiver-0.0.91/src/spotRiver/data/opm.py
--rw-r--r--   0 bartz      (501) staff       (20)    17554 2023-04-08 14:44:16.000000 spotRiver-0.0.91/src/spotRiver/data/river_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      329 2023-03-31 21:04:02.000000 spotRiver-0.0.91/src/spotRiver/data/river_hyper_dict.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.735282 spotRiver-0.0.91/src/spotRiver/data/synth/
--rw-r--r--   0 bartz      (501) staff       (20)      328 2023-01-18 17:25:51.000000 spotRiver-0.0.91/src/spotRiver/data/synth/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)     2442 2023-02-20 15:46:37.000000 spotRiver-0.0.91/src/spotRiver/data/synth/sea.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.735467 spotRiver-0.0.91/src/spotRiver/drift/
--rw-r--r--   0 bartz      (501) staff       (20)      767 2023-02-20 15:46:37.000000 spotRiver-0.0.91/src/spotRiver/drift/drift_generator.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.736260 spotRiver-0.0.91/src/spotRiver/evaluation/
--rw-r--r--   0 bartz      (501) staff       (20)    29393 2023-04-06 12:46:27.000000 spotRiver-0.0.91/src/spotRiver/evaluation/eval_bml.py
--rw-r--r--   0 bartz      (501) staff       (20)     3958 2023-02-26 22:39:12.000000 spotRiver-0.0.91/src/spotRiver/evaluation/eval_nowcast.py
--rw-r--r--   0 bartz      (501) staff       (20)     6752 2023-04-06 12:44:54.000000 spotRiver-0.0.91/src/spotRiver/evaluation/eval_oml.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.736521 spotRiver-0.0.91/src/spotRiver/fun/
--rw-r--r--   0 bartz      (501) staff       (20)    30535 2023-04-19 18:43:21.000000 spotRiver-0.0.91/src/spotRiver/fun/hyperriver.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.736843 spotRiver-0.0.91/src/spotRiver/plot/
--rw-r--r--   0 bartz      (501) staff       (20)     1340 2023-03-11 14:52:45.000000 spotRiver-0.0.91/src/spotRiver/plot/stats.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.737051 spotRiver-0.0.91/src/spotRiver/preprocess/
--rw-r--r--   0 bartz      (501) staff       (20)     2488 2023-03-07 16:50:39.000000 spotRiver-0.0.91/src/spotRiver/preprocess/impute.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.737442 spotRiver-0.0.91/src/spotRiver/utils/
--rw-r--r--   0 bartz      (501) staff       (20)     2033 2023-04-04 17:58:20.000000 spotRiver-0.0.91/src/spotRiver/utils/data_conversion.py
--rw-r--r--   0 bartz      (501) staff       (20)     5549 2023-04-13 20:07:21.000000 spotRiver-0.0.91/src/spotRiver/utils/features.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.731794 spotRiver-0.0.91/src/spotRiver.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     3383 2023-04-19 20:56:29.000000 spotRiver-0.0.91/src/spotRiver.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)      951 2023-04-19 20:56:29.000000 spotRiver-0.0.91/src/spotRiver.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2023-04-19 20:56:29.000000 spotRiver-0.0.91/src/spotRiver.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)       20 2023-04-19 20:56:29.000000 spotRiver-0.0.91/src/spotRiver.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)       10 2023-04-19 20:56:29.000000 spotRiver-0.0.91/src/spotRiver.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.737715 spotRiver-0.0.91/test/
--rw-r--r--   0 bartz      (501) staff       (20)      510 2023-02-25 09:55:05.000000 spotRiver-0.0.91/test/test_features.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-22 19:32:22.141418 spotRiver-0.0.92/
+-rw-r--r--   0 bartz      (501) staff       (20)     1520 2023-01-29 11:49:35.000000 spotRiver-0.0.92/LICENSE
+-rw-r--r--   0 bartz      (501) staff       (20)      164 2023-03-22 20:43:16.000000 spotRiver-0.0.92/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     3383 2023-04-22 19:32:22.141281 spotRiver-0.0.92/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     2912 2023-01-29 16:41:52.000000 spotRiver-0.0.92/README.md
+-rw-r--r--   0 bartz      (501) staff       (20)     1046 2023-04-22 19:09:18.000000 spotRiver-0.0.92/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2023-04-22 19:32:22.141458 spotRiver-0.0.92/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-22 19:32:22.135161 spotRiver-0.0.92/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-22 19:32:22.135665 spotRiver-0.0.92/src/spotRiver/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-22 19:32:22.139114 spotRiver-0.0.92/src/spotRiver/data/
+-rw-r--r--   0 bartz      (501) staff       (20)      413 2023-01-29 11:52:00.000000 spotRiver-0.0.92/src/spotRiver/data/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2182 2023-01-17 12:39:58.000000 spotRiver-0.0.92/src/spotRiver/data/airline-passengers.csv
+-rw-r--r--   0 bartz      (501) staff       (20)     1023 2023-03-27 20:31:30.000000 spotRiver-0.0.92/src/spotRiver/data/airline_passengers.py
+-rw-r--r--   0 bartz      (501) staff       (20)    13646 2023-03-22 20:37:51.000000 spotRiver-0.0.92/src/spotRiver/data/base.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1113 2023-03-13 20:26:53.000000 spotRiver-0.0.92/src/spotRiver/data/bike_sharing.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1870 2023-03-07 16:50:39.000000 spotRiver-0.0.92/src/spotRiver/data/generic.py
+-rw-r--r--   0 bartz      (501) staff       (20)     7751 2023-03-07 16:50:39.000000 spotRiver-0.0.92/src/spotRiver/data/opm.py
+-rw-r--r--   0 bartz      (501) staff       (20)    17554 2023-04-08 14:44:16.000000 spotRiver-0.0.92/src/spotRiver/data/river_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      329 2023-03-31 21:04:02.000000 spotRiver-0.0.92/src/spotRiver/data/river_hyper_dict.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-22 19:32:22.139360 spotRiver-0.0.92/src/spotRiver/data/synth/
+-rw-r--r--   0 bartz      (501) staff       (20)      328 2023-01-18 17:25:51.000000 spotRiver-0.0.92/src/spotRiver/data/synth/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2442 2023-02-20 15:46:37.000000 spotRiver-0.0.92/src/spotRiver/data/synth/sea.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-22 19:32:22.139647 spotRiver-0.0.92/src/spotRiver/drift/
+-rw-r--r--   0 bartz      (501) staff       (20)      767 2023-02-20 15:46:37.000000 spotRiver-0.0.92/src/spotRiver/drift/drift_generator.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-22 19:32:22.140119 spotRiver-0.0.92/src/spotRiver/evaluation/
+-rw-r--r--   0 bartz      (501) staff       (20)    29393 2023-04-06 12:46:27.000000 spotRiver-0.0.92/src/spotRiver/evaluation/eval_bml.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3958 2023-02-26 22:39:12.000000 spotRiver-0.0.92/src/spotRiver/evaluation/eval_nowcast.py
+-rw-r--r--   0 bartz      (501) staff       (20)     6752 2023-04-06 12:44:54.000000 spotRiver-0.0.92/src/spotRiver/evaluation/eval_oml.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-22 19:32:22.140252 spotRiver-0.0.92/src/spotRiver/fun/
+-rw-r--r--   0 bartz      (501) staff       (20)    32460 2023-04-22 19:31:59.000000 spotRiver-0.0.92/src/spotRiver/fun/hyperriver.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-22 19:32:22.140415 spotRiver-0.0.92/src/spotRiver/plot/
+-rw-r--r--   0 bartz      (501) staff       (20)     1340 2023-03-11 14:52:45.000000 spotRiver-0.0.92/src/spotRiver/plot/stats.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-22 19:32:22.140556 spotRiver-0.0.92/src/spotRiver/preprocess/
+-rw-r--r--   0 bartz      (501) staff       (20)     2488 2023-03-07 16:50:39.000000 spotRiver-0.0.92/src/spotRiver/preprocess/impute.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-22 19:32:22.140829 spotRiver-0.0.92/src/spotRiver/utils/
+-rw-r--r--   0 bartz      (501) staff       (20)     2033 2023-04-04 17:58:20.000000 spotRiver-0.0.92/src/spotRiver/utils/data_conversion.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5549 2023-04-13 20:07:21.000000 spotRiver-0.0.92/src/spotRiver/utils/features.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-22 19:32:22.136952 spotRiver-0.0.92/src/spotRiver.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     3383 2023-04-22 19:32:22.000000 spotRiver-0.0.92/src/spotRiver.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)      951 2023-04-22 19:32:22.000000 spotRiver-0.0.92/src/spotRiver.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2023-04-22 19:32:22.000000 spotRiver-0.0.92/src/spotRiver.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       20 2023-04-22 19:32:22.000000 spotRiver-0.0.92/src/spotRiver.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       10 2023-04-22 19:32:22.000000 spotRiver-0.0.92/src/spotRiver.egg-info/top_level.txt
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-22 19:32:22.140957 spotRiver-0.0.92/test/
+-rw-r--r--   0 bartz      (501) staff       (20)      510 2023-02-25 09:55:05.000000 spotRiver-0.0.92/test/test_features.py
```

### Comparing `spotRiver-0.0.91/LICENSE` & `spotRiver-0.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/PKG-INFO` & `spotRiver-0.0.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotRiver
-Version: 0.0.91
+Version: 0.0.92
 Summary: spotRiver - Sequential Parameter Optimization Interface to River
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 Project-URL: Homepage, https://www.spotseven.de
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `spotRiver-0.0.91/README.md` & `spotRiver-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/pyproject.toml` & `spotRiver-0.0.92/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
             "numpy",
             "scikit-learn",
             "matplotlib"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotRiver"
-version = "0.0.91"
+version = "0.0.92"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
 description = "spotRiver - Sequential Parameter Optimization Interface to River"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `spotRiver-0.0.91/src/spotRiver/data/airline-passengers.csv` & `spotRiver-0.0.92/src/spotRiver/data/airline-passengers.csv`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver/data/airline_passengers.py` & `spotRiver-0.0.92/src/spotRiver/data/airline_passengers.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver/data/base.py` & `spotRiver-0.0.92/src/spotRiver/data/base.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver/data/bike_sharing.py` & `spotRiver-0.0.92/src/spotRiver/data/bike_sharing.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver/data/generic.py` & `spotRiver-0.0.92/src/spotRiver/data/generic.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver/data/opm.py` & `spotRiver-0.0.92/src/spotRiver/data/opm.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver/data/river_hyper_dict.json` & `spotRiver-0.0.92/src/spotRiver/data/river_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver/data/synth/sea.py` & `spotRiver-0.0.92/src/spotRiver/data/synth/sea.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver/drift/drift_generator.py` & `spotRiver-0.0.92/src/spotRiver/drift/drift_generator.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver/evaluation/eval_bml.py` & `spotRiver-0.0.92/src/spotRiver/evaluation/eval_bml.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver/evaluation/eval_nowcast.py` & `spotRiver-0.0.92/src/spotRiver/evaluation/eval_nowcast.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver/evaluation/eval_oml.py` & `spotRiver-0.0.92/src/spotRiver/evaluation/eval_oml.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver/fun/hyperriver.py` & `spotRiver-0.0.92/src/spotRiver/fun/hyperriver.py`

 * *Files 6% similar despite different names*

```diff
@@ -647,28 +647,70 @@
                 oml_grace_period=fun_control["oml_grace_period"],
                 metric=fun_control["metric_sklearn"],
             )
         except Exception as err:
             print(f"Error in fun_oml_horizon(). Call to eval_oml_horizon failed. {err=}, {type(err)=}")
         return df_eval, df_preds
 
-    def fun_oml_horizon(self, X, fun_control=None, return_model=False, return_df=False):
+    def get_river_df_eval_preds(self, model):
+        try:
+            df_eval, df_preds = self.evaluate_model(model, self.fun_control)
+        except Exception as err:
+            print(f"Error in get_river_df_eval_preds(). Call to evaluate_model failed. {err=}, {type(err)=}")
+            print("Setting df_eval and df.preds to np.nan")
+            df_eval = np.nan
+            df_preds = np.nan
+        return df_eval, df_preds
+
+    def fun_oml_horizon_old(self, X, fun_control=None):
         z_res = np.array([], dtype=float)
         self.fun_control.update(fun_control)
         self.check_weights()
         self.check_X_shape(X)
         var_dict = assign_values(X, self.fun_control["var_name"])
         for config in get_one_config_from_var_dict(var_dict, self.fun_control):
-            model = compose.Pipeline(self.fun_control["prep_model"], self.fun_control["core_model"](**config))
-            if return_model:
-                return model
-            df_eval, df_preds = self.evaluate_model(model, self.fun_control)
-            if return_df:
-                return df_eval, df_preds
+            if self.fun_control["prep_model"] is not None:
+                model = compose.Pipeline(self.fun_control["prep_model"], self.fun_control["core_model"](**config))
+            else:
+                model = self.fun_control["core_model"](**config)
+            try:
+                df_eval, _ = self.evaluate_model(model, self.fun_control)
+            except Exception as err:
+                df_eval = np.nan
+                print(f"Error in fun(). Call to evaluate failed. {err=}, {type(err)=}")
+                print("Setting df_eval to np.nan.")
             try:
                 y = self.compute_y(df_eval)
             except Exception as err:
                 y = np.nan
-                print(f"Error in fun(). Call to evaluate failed. {err=}, {type(err)=}")
-                print(f"Setting y to {y:.2f}.")
+                print(f"Error in fun(). Call to compute_y failed. {err=}, {type(err)=}")
+                print("Setting y to np.nan.")
             z_res = np.append(z_res, y / self.fun_control["n_samples"])
         return z_res
+
+    def fun_oml_horizon(self, X, fun_control=None):
+        """
+        This function calculates the horizon for a given set of data X and control parameters.
+
+        :param X: numpy array of data
+        :param fun_control: dictionary of control parameters
+        :return: numpy array of horizon values
+        """
+        self.fun_control.update(fun_control)
+        self.check_weights()
+        self.check_X_shape(X)
+        var_dict = assign_values(X, self.fun_control["var_name"])
+        z_res = []
+        for config in get_one_config_from_var_dict(var_dict, self.fun_control):
+            if self.fun_control["prep_model"] is not None:
+                model = compose.Pipeline(self.fun_control["prep_model"], self.fun_control["core_model"](**config))
+            else:
+                model = self.fun_control["core_model"](**config)
+            try:
+                df_eval, _ = self.evaluate_model(model, self.fun_control)
+                y = self.compute_y(df_eval)
+            except Exception as err:
+                y = np.nan
+                print(f"Error in fun(). Call to evaluate or compute_y failed. {err=}, {type(err)=}")
+                print("Setting y to np.nan.")
+            z_res.append(y / self.fun_control["n_samples"])
+        return np.array(z_res)
```

### Comparing `spotRiver-0.0.91/src/spotRiver/plot/stats.py` & `spotRiver-0.0.92/src/spotRiver/plot/stats.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver/preprocess/impute.py` & `spotRiver-0.0.92/src/spotRiver/preprocess/impute.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver/utils/data_conversion.py` & `spotRiver-0.0.92/src/spotRiver/utils/data_conversion.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver/utils/features.py` & `spotRiver-0.0.92/src/spotRiver/utils/features.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.91/src/spotRiver.egg-info/PKG-INFO` & `spotRiver-0.0.92/src/spotRiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotRiver
-Version: 0.0.91
+Version: 0.0.92
 Summary: spotRiver - Sequential Parameter Optimization Interface to River
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 Project-URL: Homepage, https://www.spotseven.de
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `spotRiver-0.0.91/src/spotRiver.egg-info/SOURCES.txt` & `spotRiver-0.0.92/src/spotRiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

