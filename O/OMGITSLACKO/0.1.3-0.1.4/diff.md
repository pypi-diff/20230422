# Comparing `tmp/OMGITSLACKO-0.1.3.tar.gz` & `tmp/OMGITSLACKO-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OMGITSLACKO-0.1.3.tar", last modified: Fri Apr 21 21:59:49 2023, max compression
+gzip compressed data, was "OMGITSLACKO-0.1.4.tar", last modified: Sat Apr 22 10:55:36 2023, max compression
```

## Comparing `OMGITSLACKO-0.1.3.tar` & `OMGITSLACKO-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 21:59:49.499080 OMGITSLACKO-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-04-21 21:59:49.490056 OMGITSLACKO-0.1.3/OMGITSLACKO/
--rw-rw-rw-   0        0        0       89 2023-04-21 15:20:32.000000 OMGITSLACKO-0.1.3/OMGITSLACKO/__init__.py
--rw-rw-rw-   0        0        0    11502 2023-04-21 21:58:32.000000 OMGITSLACKO-0.1.3/OMGITSLACKO/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-21 21:59:49.497075 OMGITSLACKO-0.1.3/OMGITSLACKO.egg-info/
--rw-rw-rw-   0        0        0      235 2023-04-21 21:59:49.000000 OMGITSLACKO-0.1.3/OMGITSLACKO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-04-21 21:59:49.000000 OMGITSLACKO-0.1.3/OMGITSLACKO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 21:59:49.000000 OMGITSLACKO-0.1.3/OMGITSLACKO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 11:06:38.000000 OMGITSLACKO-0.1.3/OMGITSLACKO.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-04-21 21:59:49.000000 OMGITSLACKO-0.1.3/OMGITSLACKO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 21:59:49.000000 OMGITSLACKO-0.1.3/OMGITSLACKO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      235 2023-04-21 21:59:49.498603 OMGITSLACKO-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-04-21 12:10:35.000000 OMGITSLACKO-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-21 21:59:49.499080 OMGITSLACKO-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      399 2023-04-21 21:59:20.000000 OMGITSLACKO-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 10:55:36.982061 OMGITSLACKO-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-04-22 10:55:36.974040 OMGITSLACKO-0.1.4/OMGITSLACKO/
+-rw-rw-rw-   0        0        0      195 2023-04-22 10:43:33.000000 OMGITSLACKO-0.1.4/OMGITSLACKO/__init__.py
+-rw-rw-rw-   0        0        0    11508 2023-04-21 22:28:48.000000 OMGITSLACKO-0.1.4/OMGITSLACKO/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-22 10:55:36.980056 OMGITSLACKO-0.1.4/OMGITSLACKO.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-04-22 10:55:36.000000 OMGITSLACKO-0.1.4/OMGITSLACKO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-22 10:55:36.000000 OMGITSLACKO-0.1.4/OMGITSLACKO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 10:55:36.000000 OMGITSLACKO-0.1.4/OMGITSLACKO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 11:06:38.000000 OMGITSLACKO-0.1.4/OMGITSLACKO.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-04-22 10:55:36.000000 OMGITSLACKO-0.1.4/OMGITSLACKO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-22 10:55:36.000000 OMGITSLACKO-0.1.4/OMGITSLACKO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-04-22 10:55:36.981129 OMGITSLACKO-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-04-21 12:10:35.000000 OMGITSLACKO-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-22 10:55:36.982061 OMGITSLACKO-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      399 2023-04-22 10:55:04.000000 OMGITSLACKO-0.1.4/setup.py
```

### Comparing `OMGITSLACKO-0.1.3/OMGITSLACKO/functions.py` & `OMGITSLACKO-0.1.4/OMGITSLACKO/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,18 +172,17 @@
     best_r2 = metrics.r2_score(df_y_test, y_pred_best)
     print("Metrics of the best model:")
     print("Mean Squared Error:", best_mse)
     print("Root Mean Squared Error:", best_rmse)
     print("R-squared:", best_r2)
 
 
-from sklearn.cluster import estimate_bandwidth
-import itertools
-
 def find_best_clustering_algorithm(data, scaling=True, n_clusters=None, visualize=True, test_feature_combinations=False):
+    from sklearn.cluster import estimate_bandwidth
+    import itertools
     if scaling:
         scaler = StandardScaler()
         data = scaler.fit_transform(data)
     
     if test_feature_combinations:
         print("\nTesting different feature combinations:")
         for num_features in range(1, data.shape[1] + 1):
```

