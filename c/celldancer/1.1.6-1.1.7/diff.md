# Comparing `tmp/celldancer-1.1.6.tar.gz` & `tmp/celldancer-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shengyuli/Library/CloudStorage/OneDrive-HoustonMethodist/work/Velocity/bin/cellDancer_matainance/cellDancer/dist/.tmp-xr", last modified: Sat Apr 22 01:47:32 2023, max compression
+gzip compressed data, was "/Users/shengyuli/Library/CloudStorage/OneDrive-HoustonMethodist/work/Velocity/bin/cellDancer_matainance/cellDancer/dist/.tmp-5p", last modified: Sat Apr 22 02:40:11 2023, max compression
```

## Comparing `celldancer-1.1.6.tar` & `celldancer-1.1.7.tar`

### file list

```diff
@@ -1,54 +1,35 @@
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:47:32.000000 celldancer-1.1.6/
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:47:32.000000 celldancer-1.1.6/.github/
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:47:32.000000 celldancer-1.1.6/.github/scripts/
--rw-r--r--   0 shengyuli   (503) staff       (20)     1328 2023-03-21 21:48:08.000000 celldancer-1.1.6/.github/scripts/release.py
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:47:32.000000 celldancer-1.1.6/.github/workflows/
--rw-r--r--   0 shengyuli   (503) staff       (20)      442 2023-03-21 21:48:08.000000 celldancer-1.1.6/.github/workflows/publish.yml
--rw-r--r--   0 shengyuli   (503) staff       (20)      319 2023-03-21 21:48:08.000000 celldancer-1.1.6/.github/workflows/release.yml
--rw-r--r--   0 shengyuli   (503) staff       (20)      410 2023-03-21 17:04:55.000000 celldancer-1.1.6/.gitignore
--rw-r--r--   0 shengyuli   (503) staff       (20)     1516 2022-07-13 20:26:33.000000 celldancer-1.1.6/LICENSE
--rw-r--r--   0 shengyuli   (503) staff       (20)       58 2023-03-21 23:39:19.000000 celldancer-1.1.6/MANIFEST.in
--rw-r--r--   0 shengyuli   (503) staff       (20)     2338 2023-04-22 01:47:32.000000 celldancer-1.1.6/PKG-INFO
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:47:32.000000 celldancer-1.1.6/_static/
--rw-r--r--   0 shengyuli   (503) staff       (20)   353246 2022-06-27 23:16:31.000000 celldancer-1.1.6/_static/training_progress.png
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:47:32.000000 celldancer-1.1.6/notebooks/
--rw-r--r--   0 shengyuli   (503) staff       (20)  2807993 2023-03-31 21:21:11.000000 celldancer-1.1.6/notebooks/case_study_gastrulation.ipynb
--rw-r--r--   0 shengyuli   (503) staff       (20)  1486711 2022-10-20 23:05:09.000000 celldancer-1.1.6/notebooks/case_study_hgforebrian.ipynb
--rw-r--r--   0 shengyuli   (503) staff       (20)  3343600 2023-03-31 21:20:48.000000 celldancer-1.1.6/notebooks/case_study_neuro.ipynb
--rw-r--r--   0 shengyuli   (503) staff       (20)   291080 2022-10-20 11:58:08.000000 celldancer-1.1.6/notebooks/case_study_pancreas.ipynb
--rw-r--r--   0 shengyuli   (503) staff       (20)  3794391 2022-10-20 12:05:15.000000 celldancer-1.1.6/notebooks/case_study_pancreas_dynamo.ipynb
--rw-r--r--   0 shengyuli   (503) staff       (20)  1342211 2022-10-20 20:12:10.000000 celldancer-1.1.6/notebooks/case_study_rpe1.ipynb
--rw-r--r--   0 shengyuli   (503) staff       (20)     2128 2023-04-22 01:45:31.000000 celldancer-1.1.6/readme.rst
--rw-r--r--   0 shengyuli   (503) staff       (20)     1768 2023-04-22 01:45:54.000000 celldancer-1.1.6/readme_pypi.rst
--rwx------   0 shengyuli   (503) staff       (20)      323 2023-04-22 01:46:53.000000 celldancer-1.1.6/requirements.txt
--rw-r--r--   0 shengyuli   (503) staff       (20)       38 2023-04-22 01:47:32.000000 celldancer-1.1.6/setup.cfg
--rw-r--r--   0 shengyuli   (503) staff       (20)     1820 2023-04-22 01:46:42.000000 celldancer-1.1.6/setup.py
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:47:32.000000 celldancer-1.1.6/src/
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:47:32.000000 celldancer-1.1.6/src/celldancer/
--rw-r--r--   0 shengyuli   (503) staff       (20)        0 2022-05-25 16:54:11.000000 celldancer-1.1.6/src/celldancer/.Rapp.history
--rw-r--r--   0 shengyuli   (503) staff       (20)      613 2022-10-19 16:09:21.000000 celldancer-1.1.6/src/celldancer/__init__.py
--rw-r--r--   0 shengyuli   (503) staff       (20)       34 2022-07-12 10:42:41.000000 celldancer-1.1.6/src/celldancer/cdplt.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)     8814 2022-10-20 02:03:09.000000 celldancer-1.1.6/src/celldancer/compute_cell_velocity.py
--rw-r--r--   0 shengyuli   (503) staff       (20)    18218 2022-06-15 16:37:01.000000 celldancer-1.1.6/src/celldancer/diffusion.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)     2615 2022-10-19 23:46:04.000000 celldancer-1.1.6/src/celldancer/embedding_kinetic_para.py
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:47:32.000000 celldancer-1.1.6/src/celldancer/model/
--rwxr-xr-x   0 shengyuli   (503) staff       (20)    45399 2022-04-23 13:34:06.000000 celldancer-1.1.6/src/celldancer/model/branch.pt
--rw-r--r--   0 shengyuli   (503) staff       (20)    45399 2022-04-23 13:34:06.000000 celldancer-1.1.6/src/celldancer/model/circle.pt
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:47:32.000000 celldancer-1.1.6/src/celldancer/plotting/
--rw-r--r--   0 shengyuli   (503) staff       (20)        0 2022-04-29 17:40:09.000000 celldancer-1.1.6/src/celldancer/plotting/.Rapp.history
--rw-r--r--   0 shengyuli   (503) staff       (20)      332 2022-07-12 10:41:52.000000 celldancer-1.1.6/src/celldancer/plotting/__init__.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)    15361 2022-10-20 02:33:52.000000 celldancer-1.1.6/src/celldancer/plotting/cell.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)     1597 2022-10-17 16:52:17.000000 celldancer-1.1.6/src/celldancer/plotting/colormap.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)     5653 2022-10-19 23:46:49.000000 celldancer-1.1.6/src/celldancer/plotting/gene.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)     9814 2022-10-20 02:22:31.000000 celldancer-1.1.6/src/celldancer/plotting/graph.py
--rw-r--r--   0 shengyuli   (503) staff       (20)    52642 2022-10-21 01:43:06.000000 celldancer-1.1.6/src/celldancer/pseudo_time.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)    11402 2022-05-28 03:30:31.000000 celldancer-1.1.6/src/celldancer/sampling.py
--rw-r--r--   0 shengyuli   (503) staff       (20)    22705 2022-10-20 02:20:20.000000 celldancer-1.1.6/src/celldancer/simulation.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)    28494 2023-04-18 19:05:53.000000 celldancer-1.1.6/src/celldancer/utilities.py
--rw-r--r--   0 shengyuli   (503) staff       (20)    38369 2023-04-22 01:28:18.000000 celldancer-1.1.6/src/celldancer/velocity_estimation.py
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:47:32.000000 celldancer-1.1.6/src/celldancer.egg-info/
--rw-r--r--   0 shengyuli   (503) staff       (20)     2338 2023-04-22 01:47:32.000000 celldancer-1.1.6/src/celldancer.egg-info/PKG-INFO
--rw-r--r--   0 shengyuli   (503) staff       (20)     1222 2023-04-22 01:47:32.000000 celldancer-1.1.6/src/celldancer.egg-info/SOURCES.txt
--rw-r--r--   0 shengyuli   (503) staff       (20)        1 2023-04-22 01:47:32.000000 celldancer-1.1.6/src/celldancer.egg-info/dependency_links.txt
--rw-r--r--   0 shengyuli   (503) staff       (20)      324 2023-04-22 01:47:32.000000 celldancer-1.1.6/src/celldancer.egg-info/requires.txt
--rw-r--r--   0 shengyuli   (503) staff       (20)       11 2023-04-22 01:47:32.000000 celldancer-1.1.6/src/celldancer.egg-info/top_level.txt
+drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 02:40:11.000000 celldancer-1.1.7/
+-rw-r--r--   0 shengyuli   (503) staff       (20)     1516 2022-07-13 20:26:33.000000 celldancer-1.1.7/LICENSE
+-rw-r--r--   0 shengyuli   (503) staff       (20)       58 2023-03-21 23:39:19.000000 celldancer-1.1.7/MANIFEST.in
+-rw-r--r--   0 shengyuli   (503) staff       (20)     2352 2023-04-22 02:40:11.000000 celldancer-1.1.7/PKG-INFO
+-rw-r--r--   0 shengyuli   (503) staff       (20)     2142 2023-04-22 02:33:20.000000 celldancer-1.1.7/readme.rst
+-rw-r--r--   0 shengyuli   (503) staff       (20)     1782 2023-04-22 02:33:11.000000 celldancer-1.1.7/readme_pypi.rst
+-rw-r--r--   0 shengyuli   (503) staff       (20)       38 2023-04-22 02:40:11.000000 celldancer-1.1.7/setup.cfg
+-rw-r--r--   0 shengyuli   (503) staff       (20)     1820 2023-04-22 02:34:08.000000 celldancer-1.1.7/setup.py
+drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 02:40:11.000000 celldancer-1.1.7/src/
+drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 02:40:11.000000 celldancer-1.1.7/src/celldancer/
+-rw-r--r--   0 shengyuli   (503) staff       (20)      613 2022-10-19 16:09:21.000000 celldancer-1.1.7/src/celldancer/__init__.py
+-rw-r--r--   0 shengyuli   (503) staff       (20)       34 2022-07-12 10:42:41.000000 celldancer-1.1.7/src/celldancer/cdplt.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)     8814 2022-10-20 02:03:09.000000 celldancer-1.1.7/src/celldancer/compute_cell_velocity.py
+-rw-r--r--   0 shengyuli   (503) staff       (20)    18218 2022-06-15 16:37:01.000000 celldancer-1.1.7/src/celldancer/diffusion.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)     2615 2022-10-19 23:46:04.000000 celldancer-1.1.7/src/celldancer/embedding_kinetic_para.py
+drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 02:40:11.000000 celldancer-1.1.7/src/celldancer/model/
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)    45399 2022-04-23 13:34:06.000000 celldancer-1.1.7/src/celldancer/model/branch.pt
+-rw-r--r--   0 shengyuli   (503) staff       (20)    45399 2022-04-23 13:34:06.000000 celldancer-1.1.7/src/celldancer/model/circle.pt
+drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 02:40:11.000000 celldancer-1.1.7/src/celldancer/plotting/
+-rw-r--r--   0 shengyuli   (503) staff       (20)      332 2022-07-12 10:41:52.000000 celldancer-1.1.7/src/celldancer/plotting/__init__.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)    15361 2022-10-20 02:33:52.000000 celldancer-1.1.7/src/celldancer/plotting/cell.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)     1597 2022-10-17 16:52:17.000000 celldancer-1.1.7/src/celldancer/plotting/colormap.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)     5653 2022-10-19 23:46:49.000000 celldancer-1.1.7/src/celldancer/plotting/gene.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)     9814 2022-10-20 02:22:31.000000 celldancer-1.1.7/src/celldancer/plotting/graph.py
+-rw-r--r--   0 shengyuli   (503) staff       (20)    52642 2022-10-21 01:43:06.000000 celldancer-1.1.7/src/celldancer/pseudo_time.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)    11402 2022-05-28 03:30:31.000000 celldancer-1.1.7/src/celldancer/sampling.py
+-rw-r--r--   0 shengyuli   (503) staff       (20)    22705 2022-10-20 02:20:20.000000 celldancer-1.1.7/src/celldancer/simulation.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)    28494 2023-04-18 19:05:53.000000 celldancer-1.1.7/src/celldancer/utilities.py
+-rw-r--r--   0 shengyuli   (503) staff       (20)    38493 2023-04-22 02:34:25.000000 celldancer-1.1.7/src/celldancer/velocity_estimation.py
+drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 02:40:11.000000 celldancer-1.1.7/src/celldancer.egg-info/
+-rw-r--r--   0 shengyuli   (503) staff       (20)     2352 2023-04-22 02:40:10.000000 celldancer-1.1.7/src/celldancer.egg-info/PKG-INFO
+-rw-r--r--   0 shengyuli   (503) staff       (20)      787 2023-04-22 02:40:10.000000 celldancer-1.1.7/src/celldancer.egg-info/SOURCES.txt
+-rw-r--r--   0 shengyuli   (503) staff       (20)        1 2023-04-22 02:40:10.000000 celldancer-1.1.7/src/celldancer.egg-info/dependency_links.txt
+-rw-r--r--   0 shengyuli   (503) staff       (20)      324 2023-04-22 02:40:10.000000 celldancer-1.1.7/src/celldancer.egg-info/requires.txt
+-rw-r--r--   0 shengyuli   (503) staff       (20)       11 2023-04-22 02:40:10.000000 celldancer-1.1.7/src/celldancer.egg-info/top_level.txt
```

### Comparing `celldancer-1.1.6/LICENSE` & `celldancer-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.6/PKG-INFO` & `celldancer-1.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celldancer
-Version: 1.1.6
+Version: 1.1.7
 Summary: Study RNA velocity through neural network.
 Author: Wang Lab
 Author-email: gwang2@houstonmethodist.org
 Project-URL: cellDancer, https://github.com/GuangyuWangLab2021/cellDancer
 Project-URL: Documentation, https://guangyuwanglab2021.github.io/cellDancer_website/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,18 +23,18 @@
 ========================================================
 * Estimate cell-specific RNA velocity for each gene.
 * Derive cell fates in embedding space.
 * Estimate pseudotime for each cell in embedding space.
 
 What's new
 ========================================================
-cellDancer is updated to v1.1.6
+cellDancer is updated to v1.1.7
 
 * Added progress bar for adata_to_df_with_embed() and adata_to_raw().
-* Added try except to catch genes with low quality.
+* Added try except to catch genes with low quality in velocity().
 
 Installation
 ========================================================
 cellDancer requires Python version >= 3.7.6 to run.
 
 To run cellDancer locally, create an `conda <https://docs.conda.io/en/latest>`_ or `Anaconda <https://www.anaconda.com/>`_ environment as ``conda create -n cellDancer python==3.7.6``, and activate the new environment with ``conda activate cellDancer``. cellDancer could be installed with ``pip install celldancer``.
```

### Comparing `celldancer-1.1.6/readme.rst` & `celldancer-1.1.7/readme.rst`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 ========================================================
 * Estimate cell-specific RNA velocity for each gene.
 * Derive cell fates in embedding space.
 * Estimate pseudotime for each cell in embedding space.
 
 What's new
 ========================================================
-cellDancer is updated to v1.1.6
+cellDancer is updated to v1.1.7
 
 * Added progress bar for adata_to_df_with_embed() and adata_to_raw().
-* Added try except to catch genes with low quality.
+* Added try except to catch genes with low quality in velocity().
 
 Installation
 ========================================================
 cellDancer requires Python version >= 3.7.6 to run.
 
 To run cellDancer locally, create an `conda <https://docs.conda.io/en/latest>`_ or `Anaconda <https://www.anaconda.com/>`_ environment as ``conda create -n cellDancer python==3.7.6``, and activate the new environment with ``conda activate cellDancer``. cellDancer could be installed with ``pip install celldancer``.
```

### Comparing `celldancer-1.1.6/readme_pypi.rst` & `celldancer-1.1.7/readme_pypi.rst`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 ========================================================
 * Estimate cell-specific RNA velocity for each gene.
 * Derive cell fates in embedding space.
 * Estimate pseudotime for each cell in embedding space.
 
 What's new
 ========================================================
-cellDancer is updated to v1.1.6
+cellDancer is updated to v1.1.7
 
 * Added progress bar for adata_to_df_with_embed() and adata_to_raw().
-* Added try except to catch genes with low quality.
+* Added try except to catch genes with low quality in velocity().
 
 Installation
 ========================================================
 cellDancer requires Python version >= 3.7.6 to run.
 
 To run cellDancer locally, create an `conda <https://docs.conda.io/en/latest>`_ or `Anaconda <https://www.anaconda.com/>`_ environment as ``conda create -n cellDancer python==3.7.6``, and activate the new environment with ``conda activate cellDancer``. cellDancer could be installed with ``pip install celldancer``.
```

### Comparing `celldancer-1.1.6/setup.py` & `celldancer-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 }
 
 with open("readme_pypi.rst", "rt", encoding="utf8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="celldancer",
-    version="1.1.6",
+    version="1.1.7",
     author="Wang Lab",
     author_email="gwang2@houstonmethodist.org",
     description="Study RNA velocity through neural network.",
     long_description=long_description,
     long_description_content_type="text/x-rst; charset=UTF-8",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `celldancer-1.1.6/src/celldancer/__init__.py` & `celldancer-1.1.7/src/celldancer/__init__.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.6/src/celldancer/compute_cell_velocity.py` & `celldancer-1.1.7/src/celldancer/compute_cell_velocity.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.6/src/celldancer/diffusion.py` & `celldancer-1.1.7/src/celldancer/diffusion.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.6/src/celldancer/embedding_kinetic_para.py` & `celldancer-1.1.7/src/celldancer/embedding_kinetic_para.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.6/src/celldancer/model/branch.pt` & `celldancer-1.1.7/src/celldancer/model/branch.pt`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.6/src/celldancer/model/circle.pt` & `celldancer-1.1.7/src/celldancer/model/circle.pt`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.6/src/celldancer/plotting/cell.py` & `celldancer-1.1.7/src/celldancer/plotting/cell.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.6/src/celldancer/plotting/colormap.py` & `celldancer-1.1.7/src/celldancer/plotting/colormap.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.6/src/celldancer/plotting/gene.py` & `celldancer-1.1.7/src/celldancer/plotting/gene.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.6/src/celldancer/plotting/graph.py` & `celldancer-1.1.7/src/celldancer/plotting/graph.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.6/src/celldancer/pseudo_time.py` & `celldancer-1.1.7/src/celldancer/pseudo_time.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.6/src/celldancer/sampling.py` & `celldancer-1.1.7/src/celldancer/sampling.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.6/src/celldancer/simulation.py` & `celldancer-1.1.7/src/celldancer/simulation.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.6/src/celldancer/utilities.py` & `celldancer-1.1.7/src/celldancer/utilities.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.6/src/celldancer/velocity_estimation.py` & `celldancer-1.1.7/src/celldancer/velocity_estimation.py`

 * *Files 1% similar despite different names*

```diff
@@ -813,14 +813,15 @@
         if id_ranges==1:
             print(data_len,' gene was arranged to ',len(id_ranges),' portion.')
         else:
             print(data_len,' genes were arranged to ',len(id_ranges),' portion.')
     else: 
         print(data_len,' genes were arranged to ',len(id_ranges),' portions.')
     
+    unpredicted_gene_lst=list()
     for id_range in tqdm(id_ranges,desc="Velocity Estimation", total=len(id_ranges),position=1,leave=False, bar_format='{l_bar}{bar:10}{r_bar}{bar:-10b}'):
         gene_list_batch=gene_list[id_range[0]:id_range[1]]
         datamodule=build_datamodule(cell_type_u_s,speed_up,norm_u_s,permutation_ratio,norm_cell_distribution,gene_list=gene_list_batch)
 
         result = Parallel(n_jobs=n_jobs, backend="loky")(
             delayed(_train_thread)(
             datamodule = datamodule,
@@ -832,18 +833,20 @@
             loss_func=loss_func,
             learning_rate=learning_rate,
             patience=patience,
             save_path=save_path,
             norm_u_s=norm_u_s)
             for data_index in range(0,len(gene_list_batch)))
 
-    # show unpredicted gene list
-    gene_name_lst=[x for x in result if x is not None]
-    if len(gene_name_lst)!=0:
-        not_pred_err='Not predicted gene list:'+str(gene_name_lst)+'. Try visualizing the unspliced and spliced columns of the gene(s) to check the quality.'
+        # unpredicted gene list
+        gene_name_lst=[x for x in result if x is not None]
+        for i in gene_name_lst:
+            unpredicted_gene_lst.append(i)
+    if len(unpredicted_gene_lst)!=0:
+        not_pred_err='Not predicted gene list:'+str(unpredicted_gene_lst)+'. Try visualizing the unspliced and spliced columns of the gene(s) to check the quality.'
         logger_cd.error(not_pred_err)
 
     # summarize
     cellDancer_df = os.path.join(save_path,'TEMP', "cellDancer_estimation*.csv")
     cellDancer_df_files = glob.glob(cellDancer_df)
     loss_df = os.path.join(save_path, 'TEMP',"loss*.csv")
     loss_df_files = glob.glob(loss_df)
```

### Comparing `celldancer-1.1.6/src/celldancer.egg-info/PKG-INFO` & `celldancer-1.1.7/src/celldancer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celldancer
-Version: 1.1.6
+Version: 1.1.7
 Summary: Study RNA velocity through neural network.
 Author: Wang Lab
 Author-email: gwang2@houstonmethodist.org
 Project-URL: cellDancer, https://github.com/GuangyuWangLab2021/cellDancer
 Project-URL: Documentation, https://guangyuwanglab2021.github.io/cellDancer_website/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,18 +23,18 @@
 ========================================================
 * Estimate cell-specific RNA velocity for each gene.
 * Derive cell fates in embedding space.
 * Estimate pseudotime for each cell in embedding space.
 
 What's new
 ========================================================
-cellDancer is updated to v1.1.6
+cellDancer is updated to v1.1.7
 
 * Added progress bar for adata_to_df_with_embed() and adata_to_raw().
-* Added try except to catch genes with low quality.
+* Added try except to catch genes with low quality in velocity().
 
 Installation
 ========================================================
 cellDancer requires Python version >= 3.7.6 to run.
 
 To run cellDancer locally, create an `conda <https://docs.conda.io/en/latest>`_ or `Anaconda <https://www.anaconda.com/>`_ environment as ``conda create -n cellDancer python==3.7.6``, and activate the new environment with ``conda activate cellDancer``. cellDancer could be installed with ``pip install celldancer``.
```

