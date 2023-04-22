# Comparing `tmp/celldancer-1.1.4.tar.gz` & `tmp/celldancer-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shengyuli/Library/CloudStorage/OneDrive-HoustonMethodist/work/Velocity/bin/cellDancer_matainance/cellDancer/dist/.tmp-vj", last modified: Wed Mar 22 00:03:38 2023, max compression
+gzip compressed data, was "/Users/shengyuli/Library/CloudStorage/OneDrive-HoustonMethodist/work/Velocity/bin/cellDancer_matainance/cellDancer/dist/.tmp-b6", last modified: Sat Apr 22 01:05:14 2023, max compression
```

## Comparing `celldancer-1.1.4.tar` & `celldancer-1.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-03-22 00:03:38.000000 celldancer-1.1.4/
--rw-r--r--   0 shengyuli   (503) staff       (20)     1516 2022-07-13 20:26:33.000000 celldancer-1.1.4/LICENSE
--rw-r--r--   0 shengyuli   (503) staff       (20)       58 2023-03-21 23:39:19.000000 celldancer-1.1.4/MANIFEST.in
--rw-r--r--   0 shengyuli   (503) staff       (20)     2373 2023-03-22 00:03:38.000000 celldancer-1.1.4/PKG-INFO
--rw-r--r--   0 shengyuli   (503) staff       (20)     1892 2023-03-21 23:57:24.000000 celldancer-1.1.4/readme.rst
--rw-r--r--   0 shengyuli   (503) staff       (20)     1803 2023-03-21 23:57:23.000000 celldancer-1.1.4/readme_pypi.rst
--rw-r--r--   0 shengyuli   (503) staff       (20)       38 2023-03-22 00:03:38.000000 celldancer-1.1.4/setup.cfg
--rw-r--r--   0 shengyuli   (503) staff       (20)     1827 2023-03-22 00:03:14.000000 celldancer-1.1.4/setup.py
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-03-22 00:03:38.000000 celldancer-1.1.4/src/
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-03-22 00:03:38.000000 celldancer-1.1.4/src/celldancer/
--rw-r--r--   0 shengyuli   (503) staff       (20)      613 2022-10-19 16:09:21.000000 celldancer-1.1.4/src/celldancer/__init__.py
--rw-r--r--   0 shengyuli   (503) staff       (20)       34 2022-07-12 10:42:41.000000 celldancer-1.1.4/src/celldancer/cdplt.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)     8814 2022-10-20 02:03:09.000000 celldancer-1.1.4/src/celldancer/compute_cell_velocity.py
--rw-r--r--   0 shengyuli   (503) staff       (20)    18218 2022-06-15 16:37:01.000000 celldancer-1.1.4/src/celldancer/diffusion.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)     2615 2022-10-19 23:46:04.000000 celldancer-1.1.4/src/celldancer/embedding_kinetic_para.py
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-03-22 00:03:38.000000 celldancer-1.1.4/src/celldancer/model/
--rwxr-xr-x   0 shengyuli   (503) staff       (20)    45399 2022-04-23 13:34:06.000000 celldancer-1.1.4/src/celldancer/model/branch.pt
--rw-r--r--   0 shengyuli   (503) staff       (20)    45399 2022-04-23 13:34:06.000000 celldancer-1.1.4/src/celldancer/model/circle.pt
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-03-22 00:03:38.000000 celldancer-1.1.4/src/celldancer/plotting/
--rw-r--r--   0 shengyuli   (503) staff       (20)      332 2022-07-12 10:41:52.000000 celldancer-1.1.4/src/celldancer/plotting/__init__.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)    15361 2022-10-20 02:33:52.000000 celldancer-1.1.4/src/celldancer/plotting/cell.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)     1597 2022-10-17 16:52:17.000000 celldancer-1.1.4/src/celldancer/plotting/colormap.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)     5653 2022-10-19 23:46:49.000000 celldancer-1.1.4/src/celldancer/plotting/gene.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)     9814 2022-10-20 02:22:31.000000 celldancer-1.1.4/src/celldancer/plotting/graph.py
--rw-r--r--   0 shengyuli   (503) staff       (20)    52642 2022-10-21 01:43:06.000000 celldancer-1.1.4/src/celldancer/pseudo_time.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)    11402 2022-05-28 03:30:31.000000 celldancer-1.1.4/src/celldancer/sampling.py
--rw-r--r--   0 shengyuli   (503) staff       (20)    22705 2022-10-20 02:20:20.000000 celldancer-1.1.4/src/celldancer/simulation.py
--rwxr-xr-x   0 shengyuli   (503) staff       (20)    28554 2022-10-20 11:20:01.000000 celldancer-1.1.4/src/celldancer/utilities.py
--rw-r--r--   0 shengyuli   (503) staff       (20)    37244 2022-10-19 23:44:22.000000 celldancer-1.1.4/src/celldancer/velocity_estimation.py
-drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-03-22 00:03:38.000000 celldancer-1.1.4/src/celldancer.egg-info/
--rw-r--r--   0 shengyuli   (503) staff       (20)     2373 2023-03-22 00:03:38.000000 celldancer-1.1.4/src/celldancer.egg-info/PKG-INFO
--rw-r--r--   0 shengyuli   (503) staff       (20)      787 2023-03-22 00:03:38.000000 celldancer-1.1.4/src/celldancer.egg-info/SOURCES.txt
--rw-r--r--   0 shengyuli   (503) staff       (20)        1 2023-03-22 00:03:38.000000 celldancer-1.1.4/src/celldancer.egg-info/dependency_links.txt
--rw-r--r--   0 shengyuli   (503) staff       (20)      331 2023-03-22 00:03:38.000000 celldancer-1.1.4/src/celldancer.egg-info/requires.txt
--rw-r--r--   0 shengyuli   (503) staff       (20)       11 2023-03-22 00:03:38.000000 celldancer-1.1.4/src/celldancer.egg-info/top_level.txt
+drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:05:14.000000 celldancer-1.1.5/
+-rw-r--r--   0 shengyuli   (503) staff       (20)     1516 2022-07-13 20:26:33.000000 celldancer-1.1.5/LICENSE
+-rw-r--r--   0 shengyuli   (503) staff       (20)       58 2023-03-21 23:39:19.000000 celldancer-1.1.5/MANIFEST.in
+-rw-r--r--   0 shengyuli   (503) staff       (20)     2648 2023-04-22 01:05:14.000000 celldancer-1.1.5/PKG-INFO
+-rw-r--r--   0 shengyuli   (503) staff       (20)     2438 2023-04-18 18:28:03.000000 celldancer-1.1.5/readme.rst
+-rw-r--r--   0 shengyuli   (503) staff       (20)     2078 2023-03-31 21:27:04.000000 celldancer-1.1.5/readme_pypi.rst
+-rw-r--r--   0 shengyuli   (503) staff       (20)       38 2023-04-22 01:05:14.000000 celldancer-1.1.5/setup.cfg
+-rw-r--r--   0 shengyuli   (503) staff       (20)     1827 2023-04-22 01:02:23.000000 celldancer-1.1.5/setup.py
+drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:05:14.000000 celldancer-1.1.5/src/
+drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:05:14.000000 celldancer-1.1.5/src/celldancer/
+-rw-r--r--   0 shengyuli   (503) staff       (20)      613 2022-10-19 16:09:21.000000 celldancer-1.1.5/src/celldancer/__init__.py
+-rw-r--r--   0 shengyuli   (503) staff       (20)       34 2022-07-12 10:42:41.000000 celldancer-1.1.5/src/celldancer/cdplt.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)     8814 2022-10-20 02:03:09.000000 celldancer-1.1.5/src/celldancer/compute_cell_velocity.py
+-rw-r--r--   0 shengyuli   (503) staff       (20)    18218 2022-06-15 16:37:01.000000 celldancer-1.1.5/src/celldancer/diffusion.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)     2615 2022-10-19 23:46:04.000000 celldancer-1.1.5/src/celldancer/embedding_kinetic_para.py
+drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:05:14.000000 celldancer-1.1.5/src/celldancer/model/
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)    45399 2022-04-23 13:34:06.000000 celldancer-1.1.5/src/celldancer/model/branch.pt
+-rw-r--r--   0 shengyuli   (503) staff       (20)    45399 2022-04-23 13:34:06.000000 celldancer-1.1.5/src/celldancer/model/circle.pt
+drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:05:14.000000 celldancer-1.1.5/src/celldancer/plotting/
+-rw-r--r--   0 shengyuli   (503) staff       (20)      332 2022-07-12 10:41:52.000000 celldancer-1.1.5/src/celldancer/plotting/__init__.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)    15361 2022-10-20 02:33:52.000000 celldancer-1.1.5/src/celldancer/plotting/cell.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)     1597 2022-10-17 16:52:17.000000 celldancer-1.1.5/src/celldancer/plotting/colormap.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)     5653 2022-10-19 23:46:49.000000 celldancer-1.1.5/src/celldancer/plotting/gene.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)     9814 2022-10-20 02:22:31.000000 celldancer-1.1.5/src/celldancer/plotting/graph.py
+-rw-r--r--   0 shengyuli   (503) staff       (20)    52642 2022-10-21 01:43:06.000000 celldancer-1.1.5/src/celldancer/pseudo_time.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)    11402 2022-05-28 03:30:31.000000 celldancer-1.1.5/src/celldancer/sampling.py
+-rw-r--r--   0 shengyuli   (503) staff       (20)    22705 2022-10-20 02:20:20.000000 celldancer-1.1.5/src/celldancer/simulation.py
+-rwxr-xr-x   0 shengyuli   (503) staff       (20)    28494 2023-04-18 19:05:53.000000 celldancer-1.1.5/src/celldancer/utilities.py
+-rw-r--r--   0 shengyuli   (503) staff       (20)    38369 2023-04-22 00:56:45.000000 celldancer-1.1.5/src/celldancer/velocity_estimation.py
+drwxr-xr-x   0 shengyuli   (503) staff       (20)        0 2023-04-22 01:05:14.000000 celldancer-1.1.5/src/celldancer.egg-info/
+-rw-r--r--   0 shengyuli   (503) staff       (20)     2648 2023-04-22 01:05:14.000000 celldancer-1.1.5/src/celldancer.egg-info/PKG-INFO
+-rw-r--r--   0 shengyuli   (503) staff       (20)      787 2023-04-22 01:05:14.000000 celldancer-1.1.5/src/celldancer.egg-info/SOURCES.txt
+-rw-r--r--   0 shengyuli   (503) staff       (20)        1 2023-04-22 01:05:14.000000 celldancer-1.1.5/src/celldancer.egg-info/dependency_links.txt
+-rw-r--r--   0 shengyuli   (503) staff       (20)      331 2023-04-22 01:05:14.000000 celldancer-1.1.5/src/celldancer.egg-info/requires.txt
+-rw-r--r--   0 shengyuli   (503) staff       (20)       11 2023-04-22 01:05:14.000000 celldancer-1.1.5/src/celldancer.egg-info/top_level.txt
```

### Comparing `celldancer-1.1.4/LICENSE` & `celldancer-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.4/PKG-INFO` & `celldancer-1.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celldancer
-Version: 1.1.4
+Version: 1.1.5
 Summary: Study RNA velocity through neural network.
 Author: Wang Lab
 Author-email: gwang2@houstonmethodist.org
 Project-URL: cellDancer, https://github.com/GuangyuWangLab2021/cellDancer
 Project-URL: Documentation, https://guangyuwanglab2021.github.io/cellDancer_website/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -40,10 +40,13 @@
 Installation
 ========================================================
 cellDancer requires Python version >= 3.7.6 to run.
 
 To run cellDancer locally, create an `conda <https://docs.conda.io/en/latest>`_ or `Anaconda <https://www.anaconda.com/>`_ environment as ``conda create -n cellDancer python==3.7.6``, and activate the new environment with ``conda activate cellDancer``. cellDancer could be installed with ``pip install celldancer``.
 
 To install cellDancer from source code, run:
-``pip install 'your_path/Source Code/cellDancer'``
+``pip install 'your_path/Source Code/cellDancer'``.
 
-The dependencies could also be installed by ``pip install -r requirements.txt``.
+For M1 Mac users if you encountered a problem while installing bezier. Please refer to the following link:
+https://bezier.readthedocs.io/en/2021.2.12/#installing
+
+If any other dependency could not be installed with ``pip install celldancer``, try ``pip install --no-deps celldancer``. Then install the dependencies by ``pip install -r requirements.txt``.
```

### Comparing `celldancer-1.1.4/readme.rst` & `celldancer-1.1.5/readme_pypi.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 cellDancer - Estimating Cell-dependent RNA Velocity
 ===========================================================================================
 
 **cellDancer** is a modularized, parallelized, and scalable tool based on a deep learning framework for the RNA velocity analysis of scRNA-seq. Our website of tutorials is available at `cellDancer Website <https://guangyuwanglab2021.github.io/cellDancer_website/>`_.
 
 
-.. image:: _static/training_progress.png
-  :width: 100%
-  :alt: cell_type_u_s_sample_df
-
 cellDancer's key applications
 ========================================================
 * Estimate cell-specific RNA velocity for each gene.
 * Derive cell fates in embedding space.
 * Estimate pseudotime for each cell in embedding space.
 
 What's new
@@ -29,10 +25,13 @@
 Installation
 ========================================================
 cellDancer requires Python version >= 3.7.6 to run.
 
 To run cellDancer locally, create an `conda <https://docs.conda.io/en/latest>`_ or `Anaconda <https://www.anaconda.com/>`_ environment as ``conda create -n cellDancer python==3.7.6``, and activate the new environment with ``conda activate cellDancer``. cellDancer could be installed with ``pip install celldancer``.
 
 To install cellDancer from source code, run:
-``pip install 'your_path/Source Code/cellDancer'``
+``pip install 'your_path/Source Code/cellDancer'``.
+
+For M1 Mac users if you encountered a problem while installing bezier. Please refer to the following link:
+https://bezier.readthedocs.io/en/2021.2.12/#installing
 
-The dependencies could also be installed by ``pip install -r requirements.txt``.
+If any other dependency could not be installed with ``pip install celldancer``, try ``pip install --no-deps celldancer``. Then install the dependencies by ``pip install -r requirements.txt``.
```

### Comparing `celldancer-1.1.4/readme_pypi.rst` & `celldancer-1.1.5/readme.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 cellDancer - Estimating Cell-dependent RNA Velocity
 ===========================================================================================
 
 **cellDancer** is a modularized, parallelized, and scalable tool based on a deep learning framework for the RNA velocity analysis of scRNA-seq. Our website of tutorials is available at `cellDancer Website <https://guangyuwanglab2021.github.io/cellDancer_website/>`_.
 
 
+.. image:: _static/training_progress.png
+  :width: 100%
+  :alt: cell_type_u_s_sample_df
+
+Cite
+
+Shengyu Li#, Pengzhi Zhang#, Weiqing Chen, Lingqun Ye, Kristopher W. Brannan, Nhat-Tu Le, Jun-ichi Abe, John P. Cooke, Guangyu Wang. A relay velocity model infers cell-dependent RNA velocity. Nature Biotechnology (2023) https://doi.org/10.1038/s41587-023-01728-5
+
 cellDancer's key applications
 ========================================================
 * Estimate cell-specific RNA velocity for each gene.
 * Derive cell fates in embedding space.
 * Estimate pseudotime for each cell in embedding space.
 
 What's new
@@ -25,10 +33,14 @@
 Installation
 ========================================================
 cellDancer requires Python version >= 3.7.6 to run.
 
 To run cellDancer locally, create an `conda <https://docs.conda.io/en/latest>`_ or `Anaconda <https://www.anaconda.com/>`_ environment as ``conda create -n cellDancer python==3.7.6``, and activate the new environment with ``conda activate cellDancer``. cellDancer could be installed with ``pip install celldancer``.
 
 To install cellDancer from source code, run:
-``pip install 'your_path/Source Code/cellDancer'``
+``pip install 'your_path/Source Code/cellDancer'``.
+
+For M1 Mac users if you encountered a problem while installing bezier. Please refer to the following link:
+https://bezier.readthedocs.io/en/2021.2.12/#installing
+
+If any other dependency could not be installed with ``pip install celldancer``, try ``pip install --no-deps celldancer``. Then install the dependencies by ``pip install -r requirements.txt``.
 
-The dependencies could also be installed by ``pip install -r requirements.txt``.
```

### Comparing `celldancer-1.1.4/setup.py` & `celldancer-1.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 }
 
 with open("readme_pypi.rst", "rt", encoding="utf8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="celldancer",
-    version="1.1.4",
+    version="1.1.5",
     author="Wang Lab",
     author_email="gwang2@houstonmethodist.org",
     description="Study RNA velocity through neural network.",
     long_description=long_description,
     long_description_content_type="text/x-rst; charset=UTF-8",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `celldancer-1.1.4/src/celldancer/__init__.py` & `celldancer-1.1.5/src/celldancer/__init__.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.4/src/celldancer/compute_cell_velocity.py` & `celldancer-1.1.5/src/celldancer/compute_cell_velocity.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.4/src/celldancer/diffusion.py` & `celldancer-1.1.5/src/celldancer/diffusion.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.4/src/celldancer/embedding_kinetic_para.py` & `celldancer-1.1.5/src/celldancer/embedding_kinetic_para.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.4/src/celldancer/model/branch.pt` & `celldancer-1.1.5/src/celldancer/model/branch.pt`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.4/src/celldancer/model/circle.pt` & `celldancer-1.1.5/src/celldancer/model/circle.pt`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.4/src/celldancer/plotting/cell.py` & `celldancer-1.1.5/src/celldancer/plotting/cell.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.4/src/celldancer/plotting/colormap.py` & `celldancer-1.1.5/src/celldancer/plotting/colormap.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.4/src/celldancer/plotting/gene.py` & `celldancer-1.1.5/src/celldancer/plotting/gene.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.4/src/celldancer/plotting/graph.py` & `celldancer-1.1.5/src/celldancer/plotting/graph.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.4/src/celldancer/pseudo_time.py` & `celldancer-1.1.5/src/celldancer/pseudo_time.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.4/src/celldancer/sampling.py` & `celldancer-1.1.5/src/celldancer/sampling.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.4/src/celldancer/simulation.py` & `celldancer-1.1.5/src/celldancer/simulation.py`

 * *Files identical despite different names*

### Comparing `celldancer-1.1.4/src/celldancer/utilities.py` & `celldancer-1.1.5/src/celldancer/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,32 +186,31 @@
     gene_list: `list` (default: None)
         Specific gene(s) to be transfered.
     Returns
     -------
     raw_data: `pandas.DataFrame` 
         pandas DataFrame with columns gene_name, unsplice, splice, cellID, clusters, embedding1, embedding2.
     """
-
+    from tqdm import tqdm
     def adata_to_raw_one_gene(data, us_para, gene):
         '''
         convert adata to raw data format (one gene)
         data: an anndata
         us_para: the varable name of u0, s0, and gene name
         us_para = ['Mu', 'Ms']
         '''
         data2 = data[:, data.var.index.isin([gene])].copy()
         u0 = data2.layers[us_para[0]][:,0].copy().astype(np.float32)
         s0 = data2.layers[us_para[1]][:,0].copy().astype(np.float32)
         raw_data = pd.DataFrame({'gene_name':gene, 'unsplice':u0, 'splice':s0})
         return(raw_data)
 
     if gene_list is None: gene_list=adata.var.index
-
-    for i,gene in enumerate(gene_list):
-        print("processing:"+str(i+1)+"/"+str(len(gene_list)))
+    
+    for i,gene in enumerate(tqdm(gene_list)):
         data_onegene = adata_to_raw_one_gene(adata, us_para=us_para, gene=gene)
         if i==0:
             data_onegene.to_csv(save_path,header=True,index=False)
         else:
             data_onegene.to_csv(save_path,mode='a',header=False,index=False)
     
     # cell info
@@ -441,14 +440,16 @@
     save_path:
     gene_list (optional):
     return: panda dataframe with gene_list,u0,s0,cellID
     
     run: test=adata_to_raw(adata,'/Users/shengyuli/Library/CloudStorage/OneDrive-HoustonMethodist/work/Velocity/bin/cellDancer-development_20220128/src/output/test.csv',gene_list=genelist_all)
     ref: mel - loom_to_celldancer_raw.py
     '''
+    from tqdm import tqdm
+
     def adata_to_raw_one_gene(data, para, gene):
         '''
         convert adata to raw data format (one gene)
         data: an anndata
         para: the varable name of u0, s0, and gene name
         para = ['Mu', 'Ms']
         '''
@@ -457,16 +458,15 @@
         s0 = data2.layers[para[1]][:,0].copy().astype(np.float32)
         raw_data = pd.DataFrame({'gene_name':gene, 'u0':u0, 's0':s0})
         raw_data['cellID']=adata.obs.index
         return(raw_data)
 
     if gene_list is None: gene_list=adata.var.index
 
-    for i,gene in enumerate(gene_list):
-        print("processing:"+str(i)+"/"+str(len(adata.var_names)))
+    for i,gene in enumerate(tqdm(gene_list)):
         data_onegene = adata_to_raw_one_gene(adata, para=['Mu', 'Ms'], gene=gene)
         if i==0:
             data_onegene.to_csv(save_path,header=True,index=False)
         else:
             data_onegene.to_csv(save_path,mode='a',header=False,index=False)
     raw_data=pd.read_csv(save_path)
```

### Comparing `celldancer-1.1.4/src/celldancer/velocity_estimation.py` & `celldancer-1.1.5/src/celldancer/velocity_estimation.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,22 @@
 from pytorch_lightning.callbacks.early_stopping import EarlyStopping
 from pytorch_lightning.callbacks import ModelCheckpoint
 from sklearn.neighbors import NearestNeighbors
 from joblib import Parallel, delayed
 from tqdm import tqdm
 import pkg_resources
 import warnings
+
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 warnings.simplefilter("ignore", UserWarning)
 import logging
+handle='cellDancer'
+logger_cd=logging.getLogger(handle)
+logging.getLogger(handle).setLevel(logging.INFO)
+
 logging.getLogger("pytorch_lightning").setLevel(logging.WARNING)
 from .sampling import *
 
 class DNN_layer(nn.Module):
 
     """Define network structure.
     """
@@ -536,106 +541,114 @@
                   patience=None,
                   learning_rate=None,
                   dt=None,
                   loss_func=None,
                   n_neighbors=None,
                   ini_model=None,
                   model_save_path=None):
-
-    seed = 0
-    torch.manual_seed(seed)
-    random.seed(seed)
-    np.random.seed(seed)
-
-    # iniate network (DNN_layer) and loss function (DynamicModule)
-    backbone = DNN_module(DNN_layer(100, 100), n_neighbors=n_neighbors)
-    model = ltModule(backbone=backbone, dt=dt, learning_rate=learning_rate, loss_func=loss_func)
-
-    selected_data = datamodule.subset(data_indices)
-
-    unsplice, splice, this_gene_name, unsplicemax, splicemax, embedding1, embedding2=selected_data.fit_dataset.__getitem__(0)
-
-    data_df=pd.DataFrame({'unsplice':unsplice,'splice':splice,'embedding1':embedding1,'embedding2':embedding2})
-    data_df['gene_name']=this_gene_name
+    
     try:
+        seed = 0
+        torch.manual_seed(seed)
+        random.seed(seed)
+        np.random.seed(seed)
+
+        # iniate network (DNN_layer) and loss function (DynamicModule)
+        backbone = DNN_module(DNN_layer(100, 100), n_neighbors=n_neighbors)
+        model = ltModule(backbone=backbone, dt=dt, learning_rate=learning_rate, loss_func=loss_func)
+
+        selected_data = datamodule.subset(data_indices)
+
+        unsplice, splice, this_gene_name, unsplicemax, splicemax, embedding1, embedding2=selected_data.fit_dataset.__getitem__(0)
+
+        data_df=pd.DataFrame({'unsplice':unsplice,'splice':splice,'embedding1':embedding1,'embedding2':embedding2})
+        data_df['gene_name']=this_gene_name
+        try:
+
+            # Note
+            # here n_neighbors in the downsampling_embedding function is for selecting initial model.
+            # which is different from the n_neighbors in _train_tread for velocity calculation.
+            _, sampling_ixs_select_model, _ = downsampling_embedding(data_df, # for select model
+                                para='neighbors',
+                                step=(20,20),
+                                n_neighbors=30,
+                                target_amount=None,
+                                projection_neighbor_choice='embedding')
+        except:
+            sampling_ixs_select_model=list(data_df.index)
+            
+        gene_downsampling=downsampling(data_df=data_df, gene_list=[this_gene_name], downsampling_ixs=sampling_ixs_select_model)
+        if ini_model=='circle':
+            model_path=model_path=pkg_resources.resource_stream(__name__,os.path.join('model', 'circle.pt')).name
+        if ini_model=='branch':
+            model_path=model_path=pkg_resources.resource_stream(__name__,os.path.join('model', 'branch.pt')).name
+        else:
+            model_path=select_initial_net(this_gene_name, gene_downsampling, data_df)
+        model.load(model_path)
 
-        # Note
-        # here n_neighbors in the downsampling_embedding function is for selecting initial model.
-        # which is different from the n_neighbors in _train_tread for velocity calculation.
-        _, sampling_ixs_select_model, _ = downsampling_embedding(data_df, # for select model
-                            para='neighbors',
-                            step=(20,20),
-                            n_neighbors=30,
-                            target_amount=None,
-                            projection_neighbor_choice='embedding')
-    except:
-        sampling_ixs_select_model=list(data_df.index)
-        
-    gene_downsampling=downsampling(data_df=data_df, gene_list=[this_gene_name], downsampling_ixs=sampling_ixs_select_model)
-    if ini_model=='circle':
-        model_path=model_path=pkg_resources.resource_stream(__name__,os.path.join('model', 'circle.pt')).name
-    if ini_model=='branch':
-        model_path=model_path=pkg_resources.resource_stream(__name__,os.path.join('model', 'branch.pt')).name
-    else:
-        model_path=select_initial_net(this_gene_name, gene_downsampling, data_df)
-    model.load(model_path)
-
-    early_stop_callback = EarlyStopping(monitor="loss", min_delta=0.0, patience=patience,mode='min')
-
-    if check_val_every_n_epoch is None:
-        # not use early stop
-        trainer = pl.Trainer(
-            max_epochs=max_epoches, 
-            progress_bar_refresh_rate=0, 
-            reload_dataloaders_every_n_epochs=1, 
-            logger = False,
-            enable_checkpointing = False,
-            enable_model_summary=False,
-            )
-    else:
-        # use early stop
-        trainer = pl.Trainer(
-            max_epochs=max_epoches, 
-            progress_bar_refresh_rate=0, 
-            reload_dataloaders_every_n_epochs=1, 
-            logger = False,
-            enable_checkpointing = False,
-            check_val_every_n_epoch = check_val_every_n_epoch,
-            enable_model_summary=False,
-            callbacks=[early_stop_callback]
-            )
+        early_stop_callback = EarlyStopping(monitor="loss", min_delta=0.0, patience=patience,mode='min')
 
-    if max_epoches > 0:
-        trainer.fit(model, selected_data)   # train network
+        if check_val_every_n_epoch is None:
+            # not use early stop
+            trainer = pl.Trainer(
+                max_epochs=max_epoches, 
+                progress_bar_refresh_rate=0, 
+                reload_dataloaders_every_n_epochs=1, 
+                logger = False,
+                enable_checkpointing = False,
+                enable_model_summary=False,
+                )
+        else:
+            # use early stop
+            trainer = pl.Trainer(
+                max_epochs=max_epoches, 
+                progress_bar_refresh_rate=0, 
+                reload_dataloaders_every_n_epochs=1, 
+                logger = False,
+                enable_checkpointing = False,
+                check_val_every_n_epoch = check_val_every_n_epoch,
+                enable_model_summary=False,
+                callbacks=[early_stop_callback]
+                )
+
+        if max_epoches > 0:
+            trainer.fit(model, selected_data)   # train network
+
+        trainer.test(model, selected_data,verbose=False)    # predict
+        
+        if(model_save_path != None):
+            model.save(model_save_path)
+
+        loss_df = model.validation_loss_df
+        cellDancer_df = model.test_cellDancer_df
+
+        if norm_u_s:
+            cellDancer_df.unsplice=cellDancer_df.unsplice*unsplicemax
+            cellDancer_df.splice=cellDancer_df.splice*splicemax
+            cellDancer_df.unsplice_predict=cellDancer_df.unsplice_predict*unsplicemax
+            cellDancer_df.splice_predict=cellDancer_df.splice_predict*splicemax
+            cellDancer_df.beta=cellDancer_df.beta*unsplicemax
+            cellDancer_df.gamma=cellDancer_df.gamma*splicemax
+
+        if(model_save_path != None):
+            model.save(model_save_path)
+        
+        header_loss_df=['gene_name','epoch','loss']
+        header_cellDancer_df=['cellIndex','gene_name','unsplice','splice','unsplice_predict','splice_predict','alpha','beta','gamma','loss']
+        
+        loss_df.to_csv(os.path.join(save_path,'TEMP', ('loss'+'_'+this_gene_name+'.csv')),header=header_loss_df,index=False)
+        cellDancer_df.to_csv(os.path.join(save_path,'TEMP', ('cellDancer_estimation_'+this_gene_name+'.csv')),header=header_cellDancer_df,index=False)
+        
+        return None
 
-    trainer.test(model, selected_data,verbose=False)    # predict
-    
-    if(model_save_path != None):
-        model.save(model_save_path)
+    except:
+        return this_gene_name
 
-    loss_df = model.validation_loss_df
-    cellDancer_df = model.test_cellDancer_df
 
-    if norm_u_s:
-        cellDancer_df.unsplice=cellDancer_df.unsplice*unsplicemax
-        cellDancer_df.splice=cellDancer_df.splice*splicemax
-        cellDancer_df.unsplice_predict=cellDancer_df.unsplice_predict*unsplicemax
-        cellDancer_df.splice_predict=cellDancer_df.splice_predict*splicemax
-        cellDancer_df.beta=cellDancer_df.beta*unsplicemax
-        cellDancer_df.gamma=cellDancer_df.gamma*splicemax
 
-    if(model_save_path != None):
-        model.save(model_save_path)
-    
-    header_loss_df=['gene_name','epoch','loss']
-    header_cellDancer_df=['cellIndex','gene_name','unsplice','splice','unsplice_predict','splice_predict','alpha','beta','gamma','loss']
-    
-    loss_df.to_csv(os.path.join(save_path,'TEMP', ('loss'+'_'+this_gene_name+'.csv')),header=header_loss_df,index=False)
-    cellDancer_df.to_csv(os.path.join(save_path,'TEMP', ('cellDancer_estimation_'+this_gene_name+'.csv')),header=header_cellDancer_df,index=False)
-    return None
 
 
 def build_datamodule(cell_type_u_s,
                    speed_up,
                    norm_u_s,
                    permutation_ratio, 
                    norm_cell_distribution=False, 
@@ -819,14 +832,21 @@
             loss_func=loss_func,
             learning_rate=learning_rate,
             patience=patience,
             save_path=save_path,
             norm_u_s=norm_u_s)
             for data_index in range(0,len(gene_list_batch)))
 
+    # show unpredicted gene list
+    gene_name_lst=[x for x in result if x is not None]
+    if len(gene_name_lst)!=0:
+        not_pred_info='Not predicted gene list:'+str(gene_name_lst)+'. Try visualizing the unspliced and spliced columns of the gene(s) to check the quality.'
+        logger_cd.info(not_pred_info)
+
+    # summarize
     cellDancer_df = os.path.join(save_path,'TEMP', "cellDancer_estimation*.csv")
     cellDancer_df_files = glob.glob(cellDancer_df)
     loss_df = os.path.join(save_path, 'TEMP',"loss*.csv")
     loss_df_files = glob.glob(loss_df)
 
     def combine_csv(save_path,files):
         with open(save_path,"wb") as fout:
@@ -836,31 +856,36 @@
             # the rest:    
             for filepath in files[1:]:
                 with open(filepath, "rb") as f:
                     next(f)
                     fout.write(f.read())
         return(pd.read_csv(save_path))
 
-    cellDancer_df=combine_csv(os.path.join(save_path,"cellDancer_estimation.csv"),cellDancer_df_files)
-    loss_df=combine_csv(os.path.join(save_path,"cellDancer_estimation.csv"),loss_df_files)
+    if len(cellDancer_df_files)==0:
+        # if no gene predicted
+        logger_cd.info('None of the genes were predicted. Try visualizing the unspliced and spliced columns of the gene(s) to check the quality.')
+        return None, None
+    else:
+        cellDancer_df=combine_csv(os.path.join(save_path,"cellDancer_estimation.csv"),cellDancer_df_files)
+        loss_df=combine_csv(os.path.join(save_path,"cellDancer_estimation.csv"),loss_df_files)
 
-    shutil.rmtree(os.path.join(save_path,'TEMP'))
+        shutil.rmtree(os.path.join(save_path,'TEMP'))
 
-    cellDancer_df.sort_values(by = ['gene_name', 'cellIndex'], ascending = [True, True])
-    onegene=cell_type_u_s[cell_type_u_s.gene_name==cell_type_u_s.gene_name[0]]
-    embedding_info=onegene[['cellID','clusters','embedding1','embedding2']]
-    gene_amt=len(cellDancer_df.gene_name.drop_duplicates())
-    embedding_col=pd.concat([embedding_info]*gene_amt)
-    embedding_col.index=cellDancer_df.index
-    cellDancer_df=pd.concat([cellDancer_df,embedding_col],axis=1)
-    cellDancer_df.to_csv(os.path.join(save_path, ('cellDancer_estimation.csv')),index=False)
+        cellDancer_df.sort_values(by = ['gene_name', 'cellIndex'], ascending = [True, True])
+        onegene=cell_type_u_s[cell_type_u_s.gene_name==cell_type_u_s.gene_name[0]]
+        embedding_info=onegene[['cellID','clusters','embedding1','embedding2']]
+        gene_amt=len(cellDancer_df.gene_name.drop_duplicates())
+        embedding_col=pd.concat([embedding_info]*gene_amt)
+        embedding_col.index=cellDancer_df.index
+        cellDancer_df=pd.concat([cellDancer_df,embedding_col],axis=1)
+        cellDancer_df.to_csv(os.path.join(save_path, ('cellDancer_estimation.csv')),index=False)
 
-    loss_df.to_csv(os.path.join(save_path, ('loss.csv')),index=False)
+        loss_df.to_csv(os.path.join(save_path, ('loss.csv')),index=False)
 
-    return loss_df, cellDancer_df
+        return loss_df, cellDancer_df
 
     
 def select_initial_net(gene, gene_downsampling, data_df):
     '''
     check if right top conner has cells
     circle.pt is the model for single kinetic
     branch.pt is multiple kinetic
```

### Comparing `celldancer-1.1.4/src/celldancer.egg-info/PKG-INFO` & `celldancer-1.1.5/src/celldancer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celldancer
-Version: 1.1.4
+Version: 1.1.5
 Summary: Study RNA velocity through neural network.
 Author: Wang Lab
 Author-email: gwang2@houstonmethodist.org
 Project-URL: cellDancer, https://github.com/GuangyuWangLab2021/cellDancer
 Project-URL: Documentation, https://guangyuwanglab2021.github.io/cellDancer_website/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -40,10 +40,13 @@
 Installation
 ========================================================
 cellDancer requires Python version >= 3.7.6 to run.
 
 To run cellDancer locally, create an `conda <https://docs.conda.io/en/latest>`_ or `Anaconda <https://www.anaconda.com/>`_ environment as ``conda create -n cellDancer python==3.7.6``, and activate the new environment with ``conda activate cellDancer``. cellDancer could be installed with ``pip install celldancer``.
 
 To install cellDancer from source code, run:
-``pip install 'your_path/Source Code/cellDancer'``
+``pip install 'your_path/Source Code/cellDancer'``.
 
-The dependencies could also be installed by ``pip install -r requirements.txt``.
+For M1 Mac users if you encountered a problem while installing bezier. Please refer to the following link:
+https://bezier.readthedocs.io/en/2021.2.12/#installing
+
+If any other dependency could not be installed with ``pip install celldancer``, try ``pip install --no-deps celldancer``. Then install the dependencies by ``pip install -r requirements.txt``.
```

### Comparing `celldancer-1.1.4/src/celldancer.egg-info/SOURCES.txt` & `celldancer-1.1.5/src/celldancer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

