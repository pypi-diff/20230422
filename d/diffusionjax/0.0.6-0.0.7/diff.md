# Comparing `tmp/diffusionjax-0.0.6.tar.gz` & `tmp/diffusionjax-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffusionjax-0.0.6.tar", last modified: Tue Mar 21 00:04:29 2023, max compression
+gzip compressed data, was "diffusionjax-0.0.7.tar", last modified: Sat Apr 22 09:36:12 2023, max compression
```

## Comparing `diffusionjax-0.0.6.tar` & `diffusionjax-0.0.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:04:29.427078 diffusionjax-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:04:29.423078 diffusionjax-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:04:29.423078 diffusionjax-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-03-21 00:04:29.427078 diffusionjax-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:04:29.427078 diffusionjax-0.0.6/diffusionjax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/diffusionjax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-21 00:04:29.000000 diffusionjax-0.0.6/diffusionjax/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/diffusionjax/inverse_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/diffusionjax/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/diffusionjax/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/diffusionjax/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/diffusionjax/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/diffusionjax/sde.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/diffusionjax/solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:04:29.427078 diffusionjax-0.0.6/diffusionjax/test/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/diffusionjax/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/diffusionjax/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/diffusionjax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:04:29.427078 diffusionjax-0.0.6/diffusionjax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-03-21 00:04:29.000000 diffusionjax-0.0.6/diffusionjax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-21 00:04:29.000000 diffusionjax-0.0.6/diffusionjax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 00:04:29.000000 diffusionjax-0.0.6/diffusionjax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-21 00:04:29.000000 diffusionjax-0.0.6/diffusionjax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-21 00:04:29.000000 diffusionjax-0.0.6/diffusionjax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:04:29.427078 diffusionjax-0.0.6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/examples/example1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/examples/example2.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    69970 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/readme_empirical_score.png
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/readme_heatmap_bounded_perturbation.png
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/readme_heatmap_empirical_score.png
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/readme_heatmap_inpainted.png
--rw-r--r--   0 runner    (1001) docker     (123)    28810 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/readme_heatmap_trained_score.png
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/readme_samples.png
--rw-r--r--   0 runner    (1001) docker     (123)    74170 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/readme_trained_score.png
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 00:04:29.427078 diffusionjax-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-21 00:04:10.000000 diffusionjax-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:12.868917 diffusionjax-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/diffusionjax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-22 09:36:12.000000 diffusionjax-0.0.7/diffusionjax/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/inverse_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/diffusionjax/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/diffusionjax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/diffusionjax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-04-22 09:36:12.000000 diffusionjax-0.0.7/diffusionjax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-22 09:36:12.000000 diffusionjax-0.0.7/diffusionjax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:36:12.000000 diffusionjax-0.0.7/diffusionjax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-22 09:36:12.000000 diffusionjax-0.0.7/diffusionjax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-22 09:36:12.000000 diffusionjax-0.0.7/diffusionjax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/examples/example1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/examples/example2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    52645 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/readme_empirical_score.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/readme_heatmap_bounded_perturbation.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/readme_heatmap_empirical_score.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/readme_heatmap_inpainted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28810 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/readme_heatmap_trained_score.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/readme_samples.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55853 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/readme_trained_score.png
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 09:36:12.872917 diffusionjax-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-22 09:35:57.000000 diffusionjax-0.0.7/setup.py
```

### Comparing `diffusionjax-0.0.6/.github/workflows/CI.yml` & `diffusionjax-0.0.7/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.6/.github/workflows/publish.yml` & `diffusionjax-0.0.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.6/.gitignore` & `diffusionjax-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.6/LICENSE.rst` & `diffusionjax-0.0.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.6/PKG-INFO` & `diffusionjax-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffusionjax
-Version: 0.0.6
+Version: 0.0.7
 Summary: diffusionjax is a simple and accessible diffusion models package in JAX
 Home-page: https://github.com/bb515/diffusionjax
 Author: Jakiw Pidstrigach and Benjamin Boys
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -27,15 +27,15 @@
     - [Introduction to diffusion models](#introduction-to-diffusion-models)
 - [Does haves](#does-haves)
 - [Doesn't haves](#doesn't-haves)
 - [References](#references)
 - [Acknowledgements](#acknowledgements)
 
 ## Installation
-The package requires Python 3.8+. `pip install diffusionjax` or for developers,
+The package requires Python 3.8+. First, it is recommended to [create a new python virtual environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). Then, `pip install diffusionjax` or for developers,
 - Clone the repository `git clone git@github.com:bb515/diffusionjax.git`
 - Install using pip `pip install -e .` from the root directory of the repository (see the `setup.py` for the requirements that this command installs).
 
 ## Examples
 
 ### Introduction to diffusion models
 - Run the example by typing `python examples/example.py` on the command line from the root directory of the repository.
@@ -46,16 +46,16 @@
 >>> num_samples = 8
 >>> samples = sample_circle(num_samples)
 >>> N = samples.shape[1]
 >>> plot_samples(samples=samples, index=(0, 1), fname="samples", lims=((-3, 3), (-3, 3)))
 ```
 ![Prediction](readme_samples.png)
 ```python
-# Get sde model
->>> sde = OU()
+>>> # Get variance preserving (VP) a.k.a. time-changed Ohrnstein Uhlenbeck (OU) sde model
+>>> sde = VP()
 >>>
 >>> def log_hat_pt(x, t):
 >>>     """
 >>>     Empirical distribution score.
 >>>
 >>>     Args:
 >>>     x: One location in $\mathbb{R}^2$
```

### Comparing `diffusionjax-0.0.6/README.md` & `diffusionjax-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     - [Introduction to diffusion models](#introduction-to-diffusion-models)
 - [Does haves](#does-haves)
 - [Doesn't haves](#doesn't-haves)
 - [References](#references)
 - [Acknowledgements](#acknowledgements)
 
 ## Installation
-The package requires Python 3.8+. `pip install diffusionjax` or for developers,
+The package requires Python 3.8+. First, it is recommended to [create a new python virtual environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). Then, `pip install diffusionjax` or for developers,
 - Clone the repository `git clone git@github.com:bb515/diffusionjax.git`
 - Install using pip `pip install -e .` from the root directory of the repository (see the `setup.py` for the requirements that this command installs).
 
 ## Examples
 
 ### Introduction to diffusion models
 - Run the example by typing `python examples/example.py` on the command line from the root directory of the repository.
@@ -36,16 +36,16 @@
 >>> num_samples = 8
 >>> samples = sample_circle(num_samples)
 >>> N = samples.shape[1]
 >>> plot_samples(samples=samples, index=(0, 1), fname="samples", lims=((-3, 3), (-3, 3)))
 ```
 ![Prediction](readme_samples.png)
 ```python
-# Get sde model
->>> sde = OU()
+>>> # Get variance preserving (VP) a.k.a. time-changed Ohrnstein Uhlenbeck (OU) sde model
+>>> sde = VP()
 >>>
 >>> def log_hat_pt(x, t):
 >>>     """
 >>>     Empirical distribution score.
 >>>
 >>>     Args:
 >>>     x: One location in $\mathbb{R}^2$
```

### Comparing `diffusionjax-0.0.6/diffusionjax/inverse_problems.py` & `diffusionjax-0.0.7/diffusionjax/inverse_problems.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,34 +27,14 @@
         z_data = data_mean + batch_mul(std, z)
         x = merge_data_with_mask(x, z_data, mask, coeff)
 
         rng, step_rng = random.split(rng)
         x, x_mean = solver.update(step_rng, x, vec_t)
         return x, x_mean
 
-    # def get_update():
-    #     sampler_update = solver.get_update()
-    #     sde = solver.sde
-
-    #     def update(rng, data, mask, x, vec_t, coeff):
-    #         x_space = x
-    #         data_mean, std = sde.marginal_prob(data, vec_t)
-    #         z = random.normal(rng, x.shape)
-    #         z_space = z
-    #         z_data = data_mean + batch_mul(std, z_space)
-    #         x_space = merge_data_with_mask(x_space, z_data, mask, coeff)
-    #         x = x_space
-
-    #         rng, step_rng = random.split(rng)
-    #         x, x_mean = sampler_update(step_rng, x, vec_t)
-    #         return x, x_mean
-
-    #     return update
-
-    # update = get_update()
     ts = solver.ts
 
     def projection_sampler(rng, data, mask, coeff):
         """Sampler for image inpainting.
 
         Args:
             rng: A JAX random state.
@@ -104,30 +84,14 @@
         masked_data_mean, std = solver.sde.marginal_prob(data, vec_t)
         rng, step_rng = random.split(rng)
         masked_data = masked_data_mean + batch_mul(random.normal(rng, x.shape), std)
         x = x * (1. - mask) + masked_data * mask
         x_mean = x * (1. - mask) + masked_data_mean * mask
         return x, x_mean
 
-    # def get_update():
-    #     sampler_update = solver.get_update()
-    #     sde = solver.sde
-
-    #     def update(rng, data, mask, x, vec_t):
-    #         x, x_mean = sampler_update(rng, x, vec_t)
-    #         masked_data_mean, std = sde.marginal_prob(data, vec_t)
-    #         rng, step_rng = random.split(rng)
-    #         masked_data = masked_data_mean + batch_mul(random.normal(rng, x.shape), std)
-    #         x = x * (1. - mask) + masked_data * mask
-    #         x_mean = x * (1. - mask) + masked_data_mean * mask
-    #         return x, x_mean
-
-    #     return update
-
-    # update = get_update()
     ts = solver.ts
 
     def inpainter(rng, data, mask):
         """Sampler for image inpainting.
 
         Args:
             rng: A JAX random state.
```

### Comparing `diffusionjax-0.0.6/diffusionjax/losses.py` & `diffusionjax-0.0.7/diffusionjax/losses.py`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.6/diffusionjax/models.py` & `diffusionjax-0.0.7/diffusionjax/models.py`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.6/diffusionjax/plot.py` & `diffusionjax-0.0.7/diffusionjax/plot.py`

 * *Files 20% similar despite different names*

```diff
@@ -71,39 +71,107 @@
     Writer = animation.writers['ffmpeg']
     writer = Writer(fps=fps, metadata=dict(artist='Me'), bitrate=bitrate)
     # Note that mp4 does not work on pdf
     ani.save('{}.mp4'.format(fname), writer=writer, dpi=dpi)
 
 
 def plot_score(score, t, area_min=-1, area_max=1, fname="plot_score"):
+    fig, ax = plt.subplots(1, 1)
     # this helper function is here so that we can jit it.
     # We can not jit the whole function since plt.quiver cannot
     # be jitted
     @partial(jit, static_argnums=[0,])
     def helper(score, t, area_min, area_max):
         x = jnp.linspace(area_min, area_max, 16)
         x, y = jnp.meshgrid(x, x)
         grid = jnp.stack([x.flatten(), y.flatten()], axis=1)
         t = jnp.ones((grid.shape[0],)) * t
         scores = score(grid, t)
         return grid, scores
     grid, scores = helper(score, t, area_min, area_max)
-    plt.quiver(grid[:, 0], grid[:, 1], scores[:, 0], scores[:, 1])
-    plt.savefig(fname)
+    ax.quiver(grid[:, 0], grid[:, 1], scores[:, 0], scores[:, 1])
+    ax.set_xlabel(r"$x_0$")
+    ax.set_ylabel(r"$x_1$")
+    plt.gca().set_aspect('equal', adjustable='box')
+    fig.savefig(fname)
     plt.close()
 
 
-def plot_score_ax(ax, score, t, area_min=-1, area_max=1, fname="plot_score"):
-    #this helper function is here so that we can jit it.
-    #We can not jit the whole function since plt.quiver cannot
-    #be jitted
+def plot_score_ax(ax, score, t, area_min=-1, area_max=1):
+    # This helper function is here so that we can jit it.
+    # We can not jit the whole function since plt.quiver cannot be jitted
     @partial(jit, static_argnums=[0,])
     def helper(score, t, area_min, area_max):
         x = jnp.linspace(area_min, area_max, 16)
         x, y = jnp.meshgrid(x, x)
         grid = jnp.stack([x.flatten(), y.flatten()], axis=1)
         t = jnp.ones((grid.shape[0],)) * t
         scores = score(grid, t)
         return grid, scores
     grid, scores = helper(score, t, area_min, area_max)
     ax.quiver(grid[:, 0], grid[:, 1], scores[:, 0], scores[:, 3])
+    ax.set_xlabel(r"$x_0$")
+    ax.set_ylabel(r"$x_1$")
 
+
+def plot_heatmap_ax(ax, samples, area_min=-3, area_max=3):
+    """Plots a heatmap of all samples in the area [area_min, area_max] x [area_min, area_max].
+    Args:
+        samples: locations of all particles in R^2, array (J, 2)
+        area_min: lowest x and y coordinate
+        area_max: highest x and y coordinate
+    """
+    def small_kernel(z, area_min, area_max):
+        a = jnp.linspace(area_min, area_max, 512)
+        x, y = jnp.meshgrid(a, a)
+        dist = (x - z[0])**2 + (y - z[1])**2
+        hm = jnp.exp(-350 * dist)
+        return hm
+
+    # We try to jit most of the code, but use the helper functions
+    # since we cannot jit all of it because of the plt functions
+    @jit
+    def produce_heatmap(samples, area_min, area_max):
+        return jnp.sum(vmap(small_kernel, in_axes=(0, None, None))(samples, area_min, area_max), axis=0)
+
+    hm = produce_heatmap(samples, area_min, area_max)
+    extent = [area_min, area_max, area_max, area_min]
+    ax.imshow(hm, cmap=cm, interpolation='nearest', extent=extent)
+    ax = plt.gca()
+    ax.invert_yaxis()
+    ax.set_xlabel(r"$x_0$")
+    ax.set_ylabel(r"$x_1$")
+
+
+def plot_temperature_schedule(sde, solver):
+    """Plots the temperature schedule of the SDE marginals.
+
+    Args:
+        sde: a valid SDE class.
+    """
+    m2 = sde.mean_coeff(solver.ts)
+    v = sde.variance(solver.ts)
+    plt.plot(solver.ts, m2, label="m2")
+    plt.plot(solver.ts, v, label="v")
+    plt.legend()
+    plt.savefig("plot_temperature_schedule.png")
+    plt.close()
+
+
+def plot_scatter(samples, fname="samples"):
+    fig, ax = plt.subplots(1, 1)
+    fig.patch.set_facecolor('white')
+    fig.patch.set_alpha(1.0)
+    ax.scatter(
+        samples[:, 0], samples[:, 1],
+        alpha=0.1, label=r"$x$")
+    ax.legend()
+    ax.set_xlabel(r"$x_{}$".format(0))
+    ax.set_ylabel(r"$x_{}$".format(1))
+    ax.set_xlim(-3, 3)
+    ax.set_ylim(-3, 3)
+    plt.gca().set_aspect('equal', adjustable='box')
+    plt.draw()
+    fig.savefig(
+        fname,
+        facecolor=fig.get_facecolor(), edgecolor='none')
+    plt.close()
```

### Comparing `diffusionjax-0.0.6/diffusionjax/samplers.py` & `diffusionjax-0.0.7/diffusionjax/samplers.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                         return (rng, x, x_mean), x_mean
                     else:
                         return (rng, x, x_mean), x
 
         rng, step_rng = random.split(rng)
         num_samples_shape = (num_samples,) + shape
         if x_0 is None:
-            x = random.normal(step_rng, num_samples_shape)
+            x = outer_solver.sde.prior(step_rng, num_samples_shape)
         else:
             assert(x_0.shape==num_samples_shape)
             x = x_0
         if not stack_samples:
             (_, x, x_mean), _ = scan(outer_step, (rng, x, x), outer_ts)
             if denoise:
                 return x_mean
@@ -163,16 +163,15 @@
                     return (rng, x, xd), ()
                 else:
                     return (rng, x, xd), x
 
         rng, step_rng = random.split(rng)
         num_samples_shape = (num_samples,) + shape
         if x_0 is None:
-            x = random.normal(step_rng, num_samples_shape)
-            xd = random.normal(step_rng, num_samples_shape)
+            x, xd = outer_solver.sde.prior(step_rng, num_samples_shape)
         else:
             assert(x_0.shape==num_samples_shape)
             assert(xd_0.shape==num_samples_shape)
             x = x_0
             xd = xd_0
         if not stack_samples:
             (_, x, xd, _), _ = scan(outer_step, (rng, x, xd, xd), outer_ts)
```

### Comparing `diffusionjax-0.0.6/diffusionjax/solvers.py` & `diffusionjax-0.0.7/diffusionjax/solvers.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 class Solver(abc.ABC):
     """Solver abstract class. Functions are designed for a mini-batch of inputs."""
 
     def __init__(self, num_steps=1000, dt=None):
         """Construct an SDE.
         Args:
             num_steps: number of discretization time steps.
+            dt: time step duration, float or `None`.
+                Optional, if provided then final time, t1 = dt * num_steps.
         """
         self.num_steps = num_steps
         if dt is None:
             self.dt = 1. / self.num_steps
             self.ts = jnp.linspace(0, 1, num_steps + 1)[:-1].reshape(-1, 1)
         else:
             self.dt = dt
@@ -38,17 +40,18 @@
         """
 
 
 class EulerMaruyama(Solver):
     """Euler Maruyama numerical solver of an SDE. Functions are designed for a mini-batch of inputs."""
 
     def __init__(self, sde, num_steps=1000):
-        """Constructs an Euler Maruyama sampler.
+        """Constructs an Euler-Maruyama Solver.
         Args:
             sde: A valid SDE class.
+            num_steps: number of discretization time steps.
         """
         super().__init__(num_steps)
         self.sde = sde
 
     def update(self, rng, x, t):
         """
         Args:
```

### Comparing `diffusionjax-0.0.6/diffusionjax/utils.py` & `diffusionjax-0.0.7/diffusionjax/utils.py`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.6/diffusionjax.egg-info/PKG-INFO` & `diffusionjax-0.0.7/diffusionjax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffusionjax
-Version: 0.0.6
+Version: 0.0.7
 Summary: diffusionjax is a simple and accessible diffusion models package in JAX
 Home-page: https://github.com/bb515/diffusionjax
 Author: Jakiw Pidstrigach and Benjamin Boys
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -27,15 +27,15 @@
     - [Introduction to diffusion models](#introduction-to-diffusion-models)
 - [Does haves](#does-haves)
 - [Doesn't haves](#doesn't-haves)
 - [References](#references)
 - [Acknowledgements](#acknowledgements)
 
 ## Installation
-The package requires Python 3.8+. `pip install diffusionjax` or for developers,
+The package requires Python 3.8+. First, it is recommended to [create a new python virtual environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). Then, `pip install diffusionjax` or for developers,
 - Clone the repository `git clone git@github.com:bb515/diffusionjax.git`
 - Install using pip `pip install -e .` from the root directory of the repository (see the `setup.py` for the requirements that this command installs).
 
 ## Examples
 
 ### Introduction to diffusion models
 - Run the example by typing `python examples/example.py` on the command line from the root directory of the repository.
@@ -46,16 +46,16 @@
 >>> num_samples = 8
 >>> samples = sample_circle(num_samples)
 >>> N = samples.shape[1]
 >>> plot_samples(samples=samples, index=(0, 1), fname="samples", lims=((-3, 3), (-3, 3)))
 ```
 ![Prediction](readme_samples.png)
 ```python
-# Get sde model
->>> sde = OU()
+>>> # Get variance preserving (VP) a.k.a. time-changed Ohrnstein Uhlenbeck (OU) sde model
+>>> sde = VP()
 >>>
 >>> def log_hat_pt(x, t):
 >>>     """
 >>>     Empirical distribution score.
 >>>
 >>>     Args:
 >>>     x: One location in $\mathbb{R}^2$
```

### Comparing `diffusionjax-0.0.6/diffusionjax.egg-info/SOURCES.txt` & `diffusionjax-0.0.7/diffusionjax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.6/examples/example.py` & `diffusionjax-0.0.7/examples/example.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 Based off the Jupyter notebook: https://jakiw.com/sgm_intro
 A tutorial on the theoretical and implementation aspects of score-based generative models, also called diffusion models.
 """
 from jax import jit, vmap, grad
 import jax.random as random
 import jax.numpy as jnp
 from jax.scipy.special import logsumexp
+from flax import serialization
 import matplotlib.pyplot as plt
 from diffusionjax.plot import (
-    plot_samples, plot_score, plot_score_ax, plot_heatmap, plot_animation)
+    plot_samples, plot_score, plot_score_ax, plot_heatmap, plot_heatmap_ax,
+    plot_animation)
 from diffusionjax.losses import get_loss
-from diffusionjax.solvers import EulerMaruyama
+from diffusionjax.solvers import EulerMaruyama, Annealed
 from diffusionjax.samplers import get_sampler
 from diffusionjax.inverse_problems import get_inpainter
 from diffusionjax.models import MLP
 from diffusionjax.utils import (
     get_score,
     update_step,
     optimizer,
     retrain_nn)
-from diffusionjax.sde import OU
+from diffusionjax.sde import VP, VE, UDLangevin
 
 
 def sample_circle(num_samples):
     """Samples from the unit circle, angles split.
 
     Args:
         num_samples: The number of samples.
@@ -44,16 +46,18 @@
     rng = random.PRNGKey(2023)
     rng, step_rng = random.split(rng, 2)
     num_samples = 8
     samples = sample_circle(num_samples)
     N = samples.shape[1]
     plot_samples(samples=samples, index=(0, 1), fname="samples", lims=((-3, 3), (-3, 3)))
 
-    # Get sde model
-    sde = OU(beta_min=0.01, beta_max=3.0)
+    # Get sde model, variance preserving (VP) a.k.a. time-changed Ohrnstein Uhlenbeck (OU)
+    sde = VP(beta_min=0.01, beta_max=3.0)
+    # Alternative sde model, variance exploding (VE) a.k.a. time-dependent diffusion process
+    # sde = VE(sigma_min=0.01, sigma_max=3.0)
 
     def log_hat_pt(x, t):
         """
         Empirical distribution score.
 
         Args:
             x: One location in $\mathbb{R}^2$
@@ -70,15 +74,15 @@
     # Get a jax grad function, which can be batched with vmap
     nabla_log_hat_pt = jit(vmap(grad(log_hat_pt), in_axes=(0, 0), out_axes=(0)))
 
     # Running the reverse SDE with the empirical drift
     plot_score(score=nabla_log_hat_pt, t=0.01, area_min=-3, area_max=3, fname="empirical score")
     reverse_sde = sde.reverse(nabla_log_hat_pt)
     solver = EulerMaruyama(reverse_sde)
-    sampler = get_sampler(solver)
+    sampler = get_sampler(solver, stack_samples=False)
     q_samples = sampler(rng, num_samples=5000, shape=(N,))
     plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap empirical score")
 
     # What happens when I perturb the score with a constant?
     perturbed_score = lambda x, t: nabla_log_hat_pt(x, t) + 1
     rng, step_rng = random.split(rng)
     reverse_sde = sde.reverse(perturbed_score)
@@ -91,53 +95,66 @@
     batch_size=16
     score_model = MLP()
     score_scaling = True
     # Initialize parameters
     params = score_model.init(step_rng, jnp.zeros((batch_size, N)), jnp.ones((batch_size,)))
     # Initialize optimizer
     opt_state = optimizer.init(params)
-    # Get loss function
-    solver = EulerMaruyama(sde)
-    loss = get_loss(
-        sde, solver, score_model, score_scaling=score_scaling, likelihood_weighting=False,
-        reduce_mean=True, pointwise_t=False)
-    # Train with score matching
-    score_model, params, opt_state, mean_losses = retrain_nn(
-        update_step=update_step,
-        num_epochs=num_epochs,
-        step_rng=step_rng,
-        samples=samples,
-        score_model=score_model,
-        params=params,
-        opt_state=opt_state,
-        loss=loss,
-        batch_size=batch_size)
+    if 0:  # Load pre-trained model parameters
+        f = open('/tmp/output0', 'rb')
+        output = f.read()
+        params = serialization.from_bytes(params, output)
+    else:
+        # Get loss function
+        solver = EulerMaruyama(sde)
+        loss = get_loss(
+            sde, solver, score_model, score_scaling=score_scaling, likelihood_weighting=False,
+            reduce_mean=True, pointwise_t=False)
+        # Train with score matching
+        score_model, params, opt_state, mean_losses = retrain_nn(
+            update_step=update_step,
+            num_epochs=num_epochs,
+            step_rng=step_rng,
+            samples=samples,
+            score_model=score_model,
+            params=params,
+            opt_state=opt_state,
+            loss=loss,
+            batch_size=batch_size)
+
+        # Save params
+        output = serialization.to_bytes(params)
+        f = open('/tmp/output0', 'wb')
+        f.write(output)
 
     # Get trained score
     trained_score = get_score(sde, score_model, params, score_scaling=score_scaling)
     plot_score(score=trained_score, t=0.01, area_min=-3, area_max=3, fname="trained score")
     reverse_sde = sde.reverse(trained_score)
     solver = EulerMaruyama(reverse_sde)
-    sampler = get_sampler(solver)
+    sampler = get_sampler(solver, stack_samples=False)
     q_samples = sampler(rng, num_samples=1000, shape=(N,))
     plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap trained score")
 
     # Condition on one of the coordinates
     data = jnp.array([-0.5, 0.0])
     mask = jnp.array([1, 0])
     data = jnp.tile(data, (64, 1))
     mask = jnp.tile(mask, (64, 1))
     inpainter = get_inpainter(solver, stack_samples=False)
     q_samples = inpainter(rng, data, mask)
     plot_heatmap(samples=q_samples[:, [0, 1]], area_min=-3, area_max=3, fname="heatmap inpainted")
 
     frames = 100
-    fig, ax = plt.subplots()
+    fig, ax = plt.subplots(1, 1)
+    plt.gca().set_aspect('equal', adjustable='box')
     def animate(i, ax):
         ax.clear()
         plot_score_ax(
-            ax, trained_score, t=1 - (i / frames), area_min=-3, area_max=3, fname="trained score")
+            ax, trained_score, t=1 - (i / frames), area_min=-1, area_max=1)
+
     # Plot animation of the trained score over time
     plot_animation(fig, ax, animate, frames, "trained_score")
+    plt.close()
 
 if __name__ == "__main__":
     main()
```

### Comparing `diffusionjax-0.0.6/examples/example1.py` & `diffusionjax-0.0.7/examples/example1.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from diffusionjax.samplers import get_sampler
 from diffusionjax.models import MLP
 from diffusionjax.utils import (
     get_score,
     update_step,
     optimizer,
     retrain_nn)
-from diffusionjax.sde import OU
+from diffusionjax.sde import VE
 from mlkernels import Matern52
 import numpy as np
 import lab as B
 from functools import partial
 
 
 x_max = 5.0
@@ -75,15 +75,15 @@
     samples, C = sample_image_rgb(rng, num_samples=num_samples, image_size=image_size, kernel=Matern52(), num_channels=num_channels)  # (num_samples, image_size, num_channels)
 
     # Reshape image data
     samples = samples.reshape(-1, image_size, num_channels)
     plot_samples_1D(samples[:64], image_size, "samples")
 
     # Get sde model
-    sde = OU(beta_min=0.1, beta_max=3.0)
+    sde = VE(sigma_min=0.01, sigma_max=3.0)
 
     def log_hat_pt_tmp(x, t):
         """
         Empirical distribution score.
 
         Args:
             x: One location in $\mathbb{R}^2$
@@ -175,15 +175,15 @@
     # Initialize parameters
     params = score_model.init(step_rng, jnp.zeros((batch_size, image_size, num_channels)), jnp.ones((batch_size,)))
 
     # Initialize optimizer
     opt_state = optimizer.init(params)
 
     if 0:  # Load pre-trained model parameters
-        f = open('/tmp/output', 'rb')
+        f = open('/tmp/output1', 'rb')
         output = f.read()
         params = serialization.from_bytes(params, output)
     else:
         solver = EulerMaruyama(sde)
         # Get loss function
         loss = get_loss(
             sde, solver, score_model, score_scaling=True, likelihood_weighting=False,
@@ -199,15 +199,15 @@
             params=params,
             opt_state=opt_state,
             loss=loss,
             batch_size=batch_size)
 
         # Save params
         output = serialization.to_bytes(params)
-        f = open('/tmp/output', 'wb')
+        f = open('/tmp/output1', 'wb')
         f.write(output)
 
     # Get trained score
     trained_score = get_score(sde, score_model, params, score_scaling=True)
     solver = EulerMaruyama(sde.reverse(trained_score))
     sampler = get_sampler(solver, denoise=True)
     rng, step_rng = random.split(rng, 2)
@@ -245,8 +245,7 @@
     projection_sampler = get_projection_sampler(solver, stack_samples=False)
     q_samples = projection_sampler(rng, data, mask, coeff=1e-2)
     plot_samples_1D(q_samples, image_size=image_size, fname="samples projected")
 
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `diffusionjax-0.0.6/examples/example2.py` & `diffusionjax-0.0.7/examples/example2.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 An example using 2 dimensional image data.
 """
 from jax import jit, vmap, grad
 import jax.random as random
 import jax.numpy as jnp
 from jax.scipy.special import logsumexp
+from flax import serialization
 import matplotlib.pyplot as plt
 from diffusionjax.plot import plot_samples, plot_heatmap
 from diffusionjax.losses import get_loss
 from diffusionjax.solvers import EulerMaruyama, Annealed
 from diffusionjax.samplers import get_sampler
 from diffusionjax.models import CNN
 from diffusionjax.utils import (
     get_score,
     update_step,
     optimizer,
     retrain_nn)
-from diffusionjax.sde import OU, UDLangevin
+from diffusionjax.sde import VP, UDLangevin
 from mlkernels import Matern52
 import numpy as np
 import lab as B
 
 
 x_max = 5.0
 epsilon = 1e-4
@@ -74,16 +75,16 @@
 
     samples, C = sample_image_rgb(rng, num_samples=num_samples, image_size=image_size, kernel=Matern52(), num_channels=num_channels)  # (num_samples, image_size**2, num_channels)
     plot_samples(samples[:64], image_size=image_size, num_channels=num_channels)
     # Reshape image data
     samples = samples.reshape(-1, image_size, image_size, num_channels)
     plot_samples_1D(samples[:64], image_size, "samples 1D")
 
-    # Get sde model
-    sde = OU(beta_min=0.1, beta_max=10.0)
+    # Get sde model, variance preserving (VP) a.k.a. time-changed Ohrnstein Uhlenbeck (OU)
+    sde = VP(beta_min=0.1, beta_max=10.0)
 
     def log_hat_pt(x, t):
         """
         Empirical distribution score.
 
         Args:
             x: One location in $\mathbb{R}^2$
@@ -137,30 +138,41 @@
     # Neural network training via score matching
     batch_size = 16
     score_model = CNN()
     # Initialize parameters
     params = score_model.init(step_rng, jnp.zeros((batch_size, image_size, image_size, num_channels)), jnp.ones((batch_size,)))
     # Initialize optimizer
     opt_state = optimizer.init(params)
-    # Get loss function
-    solver = EulerMaruyama(sde, num_steps=num_steps)
-    loss = get_loss(
-        sde, solver, score_model, score_scaling=True, likelihood_weighting=False,
-        reduce_mean=True, pointwise_t=False)
-    # Train with score matching
-    score_model, params, opt_state, mean_losses = retrain_nn(
-        update_step=update_step,
-        num_epochs=num_epochs,
-        step_rng=step_rng,
-        samples=samples,
-        score_model=score_model,
-        params=params,
-        opt_state=opt_state,
-        loss=loss,
-        batch_size=batch_size)
+    if 0:  # Load pre-trained model parameters
+        f = open('/tmp/output2', 'rb')
+        output = f.read()
+        params = serialization.from_bytes(params, output)
+    else:
+        # Get loss function
+        solver = EulerMaruyama(sde, num_steps=num_steps)
+        loss = get_loss(
+            sde, solver, score_model, score_scaling=True, likelihood_weighting=False,
+            reduce_mean=True, pointwise_t=False)
+        # Train with score matching
+        score_model, params, opt_state, mean_losses = retrain_nn(
+            update_step=update_step,
+            num_epochs=num_epochs,
+            step_rng=step_rng,
+            samples=samples,
+            score_model=score_model,
+            params=params,
+            opt_state=opt_state,
+            loss=loss,
+            batch_size=batch_size)
+
+        # Save params
+        output = serialization.to_bytes(params)
+        f = open('/tmp/output2', 'wb')
+        f.write(output)
+
     # Get trained score
     trained_score = get_score(sde, score_model, params, score_scaling=True)
 
     # Get the outer loop of a numerical solver, also known as "predictor"
     outer_solver = EulerMaruyama(sde.reverse(trained_score), num_steps=num_steps)
 
     # Get the inner loop of a numerical solver, also known as "corrector"
@@ -174,8 +186,7 @@
     plot_samples(q_samples, image_size=image_size, num_channels=num_channels, fname="samples trained score")
     plot_samples_1D(q_samples, image_size, fname="samples 1D trained score")
     plot_heatmap(samples=q_samples[:, [0, 1], 0, 0], area_min=-3, area_max=3, fname="heatmap trained score")
 
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `diffusionjax-0.0.6/readme_heatmap_bounded_perturbation.png` & `diffusionjax-0.0.7/readme_heatmap_bounded_perturbation.png`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.6/readme_heatmap_empirical_score.png` & `diffusionjax-0.0.7/readme_heatmap_empirical_score.png`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.6/readme_heatmap_inpainted.png` & `diffusionjax-0.0.7/readme_heatmap_inpainted.png`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.6/readme_heatmap_trained_score.png` & `diffusionjax-0.0.7/readme_heatmap_trained_score.png`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.6/readme_samples.png` & `diffusionjax-0.0.7/readme_samples.png`

 * *Files identical despite different names*

### Comparing `diffusionjax-0.0.6/setup.py` & `diffusionjax-0.0.7/setup.py`

 * *Files identical despite different names*

