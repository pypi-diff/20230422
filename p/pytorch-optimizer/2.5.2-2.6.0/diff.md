# Comparing `tmp/pytorch_optimizer-2.5.2.tar.gz` & `tmp/pytorch_optimizer-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_optimizer-2.5.2.tar", max compression
+gzip compressed data, was "pytorch_optimizer-2.6.0.tar", max compression
```

## Comparing `pytorch_optimizer-2.5.2.tar` & `pytorch_optimizer-2.6.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0    11357 2023-04-11 13:47:49.754721 pytorch_optimizer-2.5.2/LICENSE
--rw-r--r--   0        0        0    27626 2023-04-11 13:47:49.754721 pytorch_optimizer-2.5.2/README.rst
--rw-r--r--   0        0        0     3655 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pyproject.toml
--rw-r--r--   0        0        0     6018 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/base/__init__.py
--rw-r--r--   0        0        0     1561 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/base/exception.py
--rw-r--r--   0        0        0     4183 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/base/optimizer.py
--rw-r--r--   0        0        0     2761 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/base/scheduler.py
--rw-r--r--   0        0        0      491 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/base/types.py
--rw-r--r--   0        0        0        0 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/experimental/__init__.py
--rw-r--r--   0        0        0     1595 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py
--rw-r--r--   0        0        0      131 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/__init__.py
--rw-r--r--   0        0        0      971 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/chebyshev.py
--rw-r--r--   0        0        0     4034 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/cosine_anealing.py
--rw-r--r--   0        0        0     1255 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/linear_warmup.py
--rw-r--r--   0        0        0     1400 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/proportion.py
--rw-r--r--   0        0        0        0 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/__init__.py
--rw-r--r--   0        0        0     7108 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adabelief.py
--rw-r--r--   0        0        0     5460 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adabound.py
--rw-r--r--   0        0        0     7217 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adafactor.py
--rw-r--r--   0        0        0     5941 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adai.py
--rw-r--r--   0        0        0     5223 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adamp.py
--rw-r--r--   0        0        0     5004 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adams.py
--rw-r--r--   0        0        0     5828 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adan.py
--rw-r--r--   0        0        0     5053 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adapnm.py
--rw-r--r--   0        0        0      781 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/agc.py
--rw-r--r--   0        0        0     3862 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/alig.py
--rw-r--r--   0        0        0     5428 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/apollo.py
--rw-r--r--   0        0        0    18352 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/dadapt.py
--rw-r--r--   0        0        0     4165 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/diffgrad.py
--rw-r--r--   0        0        0     5540 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/diffrgrad.py
--rw-r--r--   0        0        0    10702 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/fp16.py
--rw-r--r--   0        0        0      474 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/gc.py
--rw-r--r--   0        0        0     7601 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/gsam.py
--rw-r--r--   0        0        0     5563 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lamb.py
--rw-r--r--   0        0        0     3954 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lars.py
--rw-r--r--   0        0        0     2920 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lion.py
--rw-r--r--   0        0        0     4178 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lookahead.py
--rw-r--r--   0        0        0     6550 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/madgrad.py
--rw-r--r--   0        0        0     3639 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/nero.py
--rw-r--r--   0        0        0     4149 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/novograd.py
--rw-r--r--   0        0        0     4314 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/pcgrad.py
--rw-r--r--   0        0        0     3702 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/pnm.py
--rw-r--r--   0        0        0     5242 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/radam.py
--rw-r--r--   0        0        0     6827 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/ralamb.py
--rw-r--r--   0        0        0     6224 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/ranger.py
--rw-r--r--   0        0        0    12516 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/ranger21.py
--rw-r--r--   0        0        0     4718 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/sam.py
--rw-r--r--   0        0        0     3907 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/sgdp.py
--rw-r--r--   0        0        0    15763 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/shampoo.py
--rw-r--r--   0        0        0    19688 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/shampoo_utils.py
--rw-r--r--   0        0        0     7895 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/utils.py
--rw-r--r--   0        0        0    29741 1970-01-01 00:00:00.000000 pytorch_optimizer-2.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-22 07:56:58.743183 pytorch_optimizer-2.6.0/LICENSE
+-rw-r--r--   0        0        0    28771 2023-04-22 07:56:58.743183 pytorch_optimizer-2.6.0/README.rst
+-rw-r--r--   0        0        0     3649 2023-04-22 07:56:58.747183 pytorch_optimizer-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6062 2023-04-22 07:56:58.747183 pytorch_optimizer-2.6.0/pytorch_optimizer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/base/__init__.py
+-rw-r--r--   0        0        0     1583 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/base/exception.py
+-rw-r--r--   0        0        0     4183 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/base/optimizer.py
+-rw-r--r--   0        0        0     2761 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/base/scheduler.py
+-rw-r--r--   0        0        0      491 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/base/types.py
+-rw-r--r--   0        0        0        0 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/experimental/__init__.py
+-rw-r--r--   0        0        0     1595 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py
+-rw-r--r--   0        0        0      131 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0      971 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/chebyshev.py
+-rw-r--r--   0        0        0     4034 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py
+-rw-r--r--   0        0        0     1255 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/linear_warmup.py
+-rw-r--r--   0        0        0     1400 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/proportion.py
+-rw-r--r--   0        0        0        0 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/__init__.py
+-rw-r--r--   0        0        0     7108 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adabelief.py
+-rw-r--r--   0        0        0     5460 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adabound.py
+-rw-r--r--   0        0        0     7217 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adafactor.py
+-rw-r--r--   0        0        0     5941 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adai.py
+-rw-r--r--   0        0        0     5223 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adamp.py
+-rw-r--r--   0        0        0     5004 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adams.py
+-rw-r--r--   0        0        0     5828 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adan.py
+-rw-r--r--   0        0        0     5053 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adapnm.py
+-rw-r--r--   0        0        0      781 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/agc.py
+-rw-r--r--   0        0        0     3857 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/alig.py
+-rw-r--r--   0        0        0     5428 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/apollo.py
+-rw-r--r--   0        0        0    18352 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/dadapt.py
+-rw-r--r--   0        0        0     4165 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/diffgrad.py
+-rw-r--r--   0        0        0     5540 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/diffrgrad.py
+-rw-r--r--   0        0        0    10702 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/fp16.py
+-rw-r--r--   0        0        0      474 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/gc.py
+-rw-r--r--   0        0        0     7601 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/gsam.py
+-rw-r--r--   0        0        0     5563 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lamb.py
+-rw-r--r--   0        0        0     3954 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lars.py
+-rw-r--r--   0        0        0     2920 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lion.py
+-rw-r--r--   0        0        0     4178 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lookahead.py
+-rw-r--r--   0        0        0     6550 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/madgrad.py
+-rw-r--r--   0        0        0     3639 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/nero.py
+-rw-r--r--   0        0        0     4149 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/novograd.py
+-rw-r--r--   0        0        0     4314 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/pcgrad.py
+-rw-r--r--   0        0        0     3702 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/pnm.py
+-rw-r--r--   0        0        0     5242 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/radam.py
+-rw-r--r--   0        0        0     6827 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/ralamb.py
+-rw-r--r--   0        0        0     6224 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/ranger.py
+-rw-r--r--   0        0        0    12516 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/ranger21.py
+-rw-r--r--   0        0        0     4718 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/sam.py
+-rw-r--r--   0        0        0     3907 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/sgdp.py
+-rw-r--r--   0        0        0    15773 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/shampoo.py
+-rw-r--r--   0        0        0    20180 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/shampoo_utils.py
+-rw-r--r--   0        0        0     5552 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/sm3.py
+-rw-r--r--   0        0        0     7895 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/utils.py
+-rw-r--r--   0        0        0    30887 1970-01-01 00:00:00.000000 pytorch_optimizer-2.6.0/PKG-INFO
```

### Comparing `pytorch_optimizer-2.5.2/LICENSE` & `pytorch_optimizer-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/README.rst` & `pytorch_optimizer-2.6.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 =================
 pytorch-optimizer
 =================
 
 +--------------+------------------------------------------+
 | Build        | |workflow| |Documentation Status|        |
 +--------------+------------------------------------------+
-| Quality      | |codecov| |black|                        |
+| Quality      | |codecov| |black| |ruff|                 |
 +--------------+------------------------------------------+
 | Package      | |PyPI version| |PyPI pyversions|         |
 +--------------+------------------------------------------+
 | Status       | |PyPi download| |PyPi month download|    |
 +--------------+------------------------------------------+
+| License      | |apache|                                 |
++--------------+------------------------------------------+
 
 | **pytorch-optimizer** is bunch of optimizer collections in PyTorch. Also, including useful optimization ideas.
 | Most of the implementations are based on the original paper, but I added some tweaks.
 | Highly inspired by `pytorch-optimizer <https://github.com/jettify/pytorch-optimizer>`__.
 
-Documentation
--------------
-
-https://pytorch-optimizers.readthedocs.io/en/latest/
+Getting Started
+---------------
 
-Usage
------
+For more, see the `documentation <https://pytorch-optimizers.readthedocs.io/en/latest/>`__.
 
-Install
-~~~~~~~
+Installation
+~~~~~~~~~~~~
 
 ::
 
     $ pip3 install -U pytorch-optimizer
 
 If there's a version issue when installing the package, try with `--no-deps` option.
 
@@ -70,15 +69,15 @@
 ::
 
     from pytorch_optimizer import create_optimizer
 
     optimizer = create_optimizer(
         model,
         'adamp',
-        lr=1e-2,
+        lr=1e-3,
         weight_decay=1e-3,
         use_gc=True,
         use_lookahead=True,
     )
 
 Supported Optimizers
 --------------------
@@ -135,14 +134,16 @@
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | NovoGrad     | *Stochastic Gradient Methods with Layer-wise Adaptive Moments for Training of Deep Networks*    | `github <https://github.com/lonePatient/NovoGrad-pytorch>`__                      | `https://arxiv.org/abs/1905.11286 <https://arxiv.org/abs/1905.11286>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | Lion         | *Symbolic Discovery of Optimization Algorithms*                                                 | `github <https://github.com/google/automl/tree/master/lion>`__                    | `https://arxiv.org/abs/2302.06675 <https://arxiv.org/abs/2302.06675>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | Ali-G        | *Adaptive Learning Rates for Interpolation with Gradients*                                      | `github <https://github.com/oval-group/ali-g>`__                                  | `https://arxiv.org/abs/1906.05661 <https://arxiv.org/abs/1906.05661>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| SM3          | *Memory-Efficient Adaptive Optimization*                                                        | `github <https://github.com/google-research/google-research/tree/master/sm3>`__   | `https://arxiv.org/abs/1901.11150 <https://arxiv.org/abs/1901.11150>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 
 Useful Resources
 ----------------
 
 Several optimization ideas to regularize & stabilize the training. Most
 of the ideas are applied in ``Ranger21`` optimizer.
 
@@ -340,14 +341,16 @@
 
 `NovoGrad <https://ui.adsabs.harvard.edu/abs/2019arXiv190511286G/exportcitation>`__
 
 `Lion <https://github.com/google/automl/tree/master/lion#citation>`__
 
 `Ali-G <https://github.com/oval-group/ali-g#adaptive-learning-rates-for-interpolation-with-gradients>`__
 
+`SM3 <https://ui.adsabs.harvard.edu/abs/2019arXiv190111150A/exportcitation>`__
+
 Citation
 --------
 
 Please cite original authors of optimization algorithms. If you use this software, please cite it as below.
 Or you can get from "cite this repository" button.
 
 ::
@@ -373,9 +376,13 @@
 .. |PyPi download| image:: https://pepy.tech/badge/pytorch-optimizer
    :target: https://pepy.tech/project/pytorch-optimizer
 .. |PyPi month download| image:: https://pepy.tech/badge/pytorch-optimizer/month
    :target: https://pepy.tech/project/pytorch-optimizer
 .. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/pytorch-optimizer.svg
    :target: https://pypi.python.org/pypi/pytorch-optimizer/
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. |ruff| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+   :target: https://github.com/charliermarsh/ruff
 .. |codecov| image:: https://codecov.io/gh/kozistr/pytorch_optimizer/branch/main/graph/badge.svg?token=L4K00EA0VD
    :target: https://codecov.io/gh/kozistr/pytorch_optimizer
+.. |apache| image:: https://img.shields.io/badge/License-Apache_2.0-blue.svg
+   :target: https://opensource.org/licenses/Apache-2.0
```

### Comparing `pytorch_optimizer-2.5.2/pyproject.toml` & `pytorch_optimizer-2.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytorch_optimizer"
-version = "2.5.2"
+version = "2.6.0"
 description = "optimizer & lr scheduler implementations in PyTorch with clean-code, strict types. Also, including useful optimization ideas."
 license = "Apache-2.0"
 authors = ["kozistr <kozistr@gmail.com>"]
 maintainers = ["kozistr <kozistr@gmail.com>"]
 readme = "README.rst"
 homepage = "https://github.com/kozistr/pytorch_optimizer"
 repository = "https://github.com/kozistr/pytorch_optimizer"
@@ -34,26 +34,26 @@
 [tool.poetry.dependencies]
 python = "^3.7.2"
 numpy = [
     { version = "=1.21.1", python = ">=3.7,<3.8" },
     { version = "*", python = ">=3.8" },
 ]
 torch = [
-    { version = ">=1.10,>=2.0", python = ">=3.8", source = "torch" },
+    { version = ">=1.10", python = ">=3.8", source = "torch" },
     { version = "^1.10", python = ">=3.7,<3.8", source = "torch" },
 ]
 
 [tool.poetry.dev-dependencies]
 isort = [
     { version = "==5.11.5", python = ">=3.7,<3.8"},
     { version = "^5.12.0", python = ">=3.8"}
 ]
 black = "^23.3.0"
-ruff = "^0.0.260"
-pytest = "^7.2.2"
+ruff = "^0.0.262"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 
 [[tool.poetry.source]]
 name = "torch"
 url = "https://download.pytorch.org/whl/cpu"
 secondary = true
```

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/__init__.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,18 +57,18 @@
     PreConditioner,
     PreConditionerType,
     RMSPropGraft,
     SGDGraft,
     SQRTNGraft,
     compute_power_schur_newton,
     compute_power_svd,
-    matrix_power,
     merge_small_dims,
-    power_iter,
+    power_iteration,
 )
+from pytorch_optimizer.optimizer.sm3 import SM3
 from pytorch_optimizer.optimizer.utils import (
     clip_grad_norm,
     disable_running_stats,
     enable_running_stats,
     get_optimizer_parameters,
     normalize_gradient,
     unit_norm,
@@ -100,14 +100,15 @@
     DAdaptSGD,
     AdamS,
     AdaFactor,
     Apollo,
     NovoGrad,
     Lion,
     AliG,
+    SM3,
 ]
 OPTIMIZERS: Dict[str, OPTIMIZER] = {str(optimizer.__name__).lower(): optimizer for optimizer in OPTIMIZER_LIST}
 
 LR_SCHEDULER_LIST: List[SCHEDULER] = [
     CosineAnnealingWarmupRestarts,
     ConstantLR,
     CosineAnnealingLR,
```

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/base/exception.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/base/exception.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         self.message: str = '[-] parameter size is 0'
         super().__init__(self.message)
 
 
 class NoClosureError(Exception):
     """Raised when there's no closure function."""
 
-    def __init__(self, optimizer_name: str):
-        self.message: str = f'[-] {optimizer_name} requires closure.'
+    def __init__(self, optimizer_name: str, note: str = ''):
+        self.message: str = f'[-] {optimizer_name} requires closure.{note}'
         super().__init__(self.message)
 
 
 class NegativeLRError(Exception):
     """Raised when learning rate is negative."""
 
     def __init__(self, lr: float, lr_type: str = ''):
```

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/base/optimizer.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/base/optimizer.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/base/scheduler.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/base/scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/chebyshev.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/chebyshev.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/cosine_anealing.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/linear_warmup.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/linear_warmup.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/proportion.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/proportion.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adabelief.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adabelief.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adabound.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adabound.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adafactor.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adafactor.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adai.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adai.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adamp.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adamp.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adams.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adams.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adan.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adan.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adapnm.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adapnm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/agc.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/agc.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/alig.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/alig.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Callable, Optional
 
 import torch
 from torch.optim.optimizer import Optimizer
 
-from pytorch_optimizer.base.exception import NoSparseGradientError
+from pytorch_optimizer.base.exception import NoClosureError, NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
 class AliG(Optimizer, BaseOptimizer):
     r"""Adaptive Learning Rates for Interpolation with Gradients.
 
@@ -68,15 +68,15 @@
                     global_grad_norm += p.grad.norm().pow(2).item()
 
         return loss / (global_grad_norm + self.eps)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         if closure is None:
-            raise ValueError('[-] AliG optimizer needs closure. (eg. `optimizer.step(lambda: float(loss))`).')
+            raise NoClosureError('AliG', '(e.g. `optimizer.step(lambda: float(loss))`).')
 
         loss = closure()
 
         un_clipped_step_size: float = self.compute_step_size(loss)
 
         for group in self.param_groups:
             step_size = group['step_size'] = (
```

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/apollo.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/apollo.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/dadapt.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/dadapt.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/diffgrad.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/diffgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/diffrgrad.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/diffrgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/fp16.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/fp16.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/gsam.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/gsam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lamb.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lamb.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lars.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lion.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lion.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lookahead.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lookahead.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/madgrad.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/madgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/nero.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/nero.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/novograd.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/novograd.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/pcgrad.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/pcgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/pnm.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/pnm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/radam.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/radam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/ralamb.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/ralamb.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/ranger.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/ranger.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/ranger21.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/ranger21.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/sam.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/sam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/sgdp.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/sgdp.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/shampoo.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/shampoo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 import torch
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 from pytorch_optimizer.optimizer.shampoo_utils import (
-    AdaGradGraft,
-    Graft,
     LayerWiseGrafting,
     PreConditioner,
     PreConditionerType,
-    RMSPropGraft,
-    SGDGraft,
-    SQRTNGraft,
+    build_graft,
     compute_power_svd,
 )
 
 
 class Shampoo(Optimizer, BaseOptimizer):
     r"""Preconditioned Stochastic Tensor Optimization.
 
@@ -130,14 +126,26 @@
 
         return loss
 
 
 class ScalableShampoo(Optimizer, BaseOptimizer):
     r"""Scalable Preconditioned Stochastic Tensor Optimization.
 
+        This version of Scalable Shampoo Optimizer aims for a single GPU environment, not for a distributed environment
+        or XLA devices. So, the original intention is to compute pre-conditioners asynchronously on the distributed
+        CPUs, but this implementation calculates them which takes 99% of the optimization time on a GPU synchronously.
+
+        Still, it is much faster than the previous Shampoo Optimizer because using coupled Newton iteration when
+        computing G^{-1/p} matrices while the previous one uses SVD which is really slow.
+
+        Also, this implementation offers
+            1. lots of plug-ins (e.g. gradient grafting, type of pre-conditioning, etc)
+            2. not-yet implemented features in the official Pytorch code.
+            3. readable, organized, clean code.
+
         Reference : https://github.com/google-research/google-research/blob/master/scalable_shampoo/pytorch/shampoo.py.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. beta1, beta2.
     :param moving_average_for_momentum: bool. perform moving_average for momentum (beta1).
     :param weight_decay: float. weight decay (L2 penalty).
@@ -151,14 +159,15 @@
         compute on the GPU (not CPU) and the precision is fp32 (not fp64).
         Also, followed by the paper, `preconditioning_compute_steps` does not have a significant effect on the
         performance. So, If you have a problem with the speed, try to set this step bigger (e.g. 1000).
     :param statistics_compute_steps: int. How often to compute statistics. usually set to 1 (or 10).
     :param block_size: int. Block size for large layers (if > 0).
         Block size = 1 ==> Adagrad (Don't do this, extremely inefficient!)
         Block size should be as large as feasible under memory/time constraints.
+    :param skip_preconditioning_rank_lt: int. Skips preconditioning for parameters with rank less than this value.
     :param no_preconditioning_for_layers_with_dim_gt: int. avoid preconditioning large layers to reduce overall memory.
     :param shape_interpretation: bool. Automatic shape interpretation (for eg: [4, 3, 1024, 512] would
         result in 12 x [1024, 512] L and R statistics. Disabled by default which results in Shampoo constructing
         statistics [4, 4], [3, 3], [1024, 1024], [512, 512].
     :param graft_type: int. type of grafting (SGD or AdaGrad or RMSProp or SQRT_N or None).
     :param pre_conditioner_type: int. type of pre-conditioner.
     :param nesterov: bool. Nesterov momentum.
@@ -176,18 +185,19 @@
         lr: float = 1e-3,
         betas: BETAS = (0.9, 0.999),
         moving_average_for_momentum: bool = False,
         weight_decay: float = 0.0,
         decoupled_weight_decay: bool = False,
         decoupled_learning_rate: bool = True,
         inverse_exponent_override: int = 0,
-        start_preconditioning_step: int = 5,
-        preconditioning_compute_steps: int = 1,
+        start_preconditioning_step: int = 25,
+        preconditioning_compute_steps: int = 1000,
         statistics_compute_steps: int = 1,
         block_size: int = 256,
+        skip_preconditioning_rank_lt: int = 1,
         no_preconditioning_for_layers_with_dim_gt: int = 8192,
         shape_interpretation: bool = True,
         graft_type: int = LayerWiseGrafting.SGD,
         pre_conditioner_type: int = PreConditionerType.ALL,
         nesterov: bool = True,
         diagonal_eps: float = 1e-10,
         matrix_eps: float = 1e-6,
@@ -200,30 +210,27 @@
         self.decoupled_weight_decay = decoupled_weight_decay
         self.decoupled_learning_rate = decoupled_learning_rate
         self.inverse_exponent_override = inverse_exponent_override
         self.start_preconditioning_step = start_preconditioning_step
         self.preconditioning_compute_steps = preconditioning_compute_steps
         self.statistics_compute_steps = statistics_compute_steps
         self.block_size = block_size
+        self.skip_preconditioning_rank_lt = skip_preconditioning_rank_lt
         self.no_preconditioning_for_layers_with_dim_gt = no_preconditioning_for_layers_with_dim_gt
         self.shape_interpretation = shape_interpretation
         self.graft_type = graft_type
         self.pre_conditioner_type = pre_conditioner_type
         self.nesterov = nesterov
         self.diagonal_eps = diagonal_eps
         self.matrix_eps = matrix_eps
         self.use_svd = use_svd
 
         self.validate_parameters()
 
-        defaults: DEFAULTS = {
-            'lr': lr,
-            'betas': betas,
-            'weight_decay': weight_decay,
-        }
+        defaults: DEFAULTS = {'lr': lr, 'betas': betas, 'weight_decay': weight_decay}
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
         self.validate_update_frequency(self.start_preconditioning_step)
@@ -234,130 +241,114 @@
 
     def __str__(self) -> str:
         return 'ScalableShampoo'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['step'] = 0
                 state['momentum'] = torch.zeros_like(p)
                 state['pre_conditioner'] = PreConditioner(
                     p,
                     group['betas'][1],  # beta2
                     self.inverse_exponent_override,
                     self.block_size,
+                    self.skip_preconditioning_rank_lt,
                     self.no_preconditioning_for_layers_with_dim_gt,
                     self.shape_interpretation,
-                    self.matrix_eps,
                     self.pre_conditioner_type,
+                    self.matrix_eps,
                     self.use_svd,
                 )
-                if self.graft_type == LayerWiseGrafting.ADAGRAD:
-                    state['graft'] = AdaGradGraft(p, self.diagonal_eps)
-                elif self.graft_type == LayerWiseGrafting.RMSPROP:
-                    state['graft'] = RMSPropGraft(p, self.diagonal_eps)
-                elif self.graft_type == LayerWiseGrafting.SGD:
-                    state['graft'] = SGDGraft(p)
-                elif self.graft_type == LayerWiseGrafting.SQRTN:
-                    state['graft'] = SQRTNGraft(p)
-                else:
-                    state['graft'] = Graft(p)
+                state['graft'] = build_graft(p, self.graft_type, self.diagonal_eps)
 
     def is_precondition_step(self, step: int) -> bool:
         return step >= self.start_preconditioning_step
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
+            if 'step' in group:
+                group['step'] += 1
+            else:
+                group['step'] = 1
+
+            is_precondition_step: bool = self.is_precondition_step(group['step'])
+            pre_conditioner_multiplier: float = group['lr'] if not self.decoupled_learning_rate else 1.0
+
             beta1, beta2 = group['betas']
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
                 if len(state) == 0:
-                    state['step'] = 0
                     state['momentum'] = torch.zeros_like(p)
                     state['pre_conditioner'] = PreConditioner(
                         p,
                         beta2,
                         self.inverse_exponent_override,
                         self.block_size,
+                        self.skip_preconditioning_rank_lt,
                         self.no_preconditioning_for_layers_with_dim_gt,
                         self.shape_interpretation,
-                        self.matrix_eps,
                         self.pre_conditioner_type,
+                        self.matrix_eps,
                         self.use_svd,
                     )
-                    if self.graft_type == LayerWiseGrafting.ADAGRAD:
-                        state['graft'] = AdaGradGraft(p, self.diagonal_eps)
-                    elif self.graft_type == LayerWiseGrafting.RMSPROP:
-                        state['graft'] = RMSPropGraft(p, self.diagonal_eps)
-                    elif self.graft_type == LayerWiseGrafting.SGD:
-                        state['graft'] = SGDGraft(p)
-                    elif self.graft_type == LayerWiseGrafting.SQRTN:
-                        state['graft'] = SQRTNGraft(p)
-                    else:
-                        state['graft'] = Graft(p)
+                    state['graft'] = build_graft(p, self.graft_type, self.diagonal_eps)
 
-                state['step'] += 1
                 pre_conditioner, graft = state['pre_conditioner'], state['graft']
 
-                is_precondition_step: bool = self.is_precondition_step(state['step'])
-
                 graft.add_statistics(grad, beta2)
-                if state['step'] % self.statistics_compute_steps == 0:
+                if group['step'] % self.statistics_compute_steps == 0:
                     pre_conditioner.add_statistics(grad)
-                if state['step'] % self.preconditioning_compute_steps == 0:
+                if group['step'] % self.preconditioning_compute_steps == 0:
                     pre_conditioner.compute_pre_conditioners()
 
-                pre_conditioner_multiplier: float = group['lr'] if not self.decoupled_learning_rate else 1.0
                 graft_grad: torch.Tensor = graft.precondition_gradient(grad * pre_conditioner_multiplier)
-                shampoo_grad: torch.Tensor = grad
-                if is_precondition_step:
-                    shampoo_grad = pre_conditioner.preconditioned_grad(grad)
+                shampoo_grad: torch.Tensor = (
+                    pre_conditioner.preconditioned_grad(grad) if is_precondition_step else grad
+                )
 
                 if self.graft_type != LayerWiseGrafting.NONE:
-                    graft_norm = torch.norm(graft_grad)
-                    shampoo_norm = torch.norm(shampoo_grad)
+                    graft_norm = torch.linalg.norm(graft_grad)
+                    shampoo_norm = torch.linalg.norm(shampoo_grad)
 
                     shampoo_grad.mul_(graft_norm / (shampoo_norm + 1e-16))
 
                 if group['weight_decay'] > 0.0:
                     if not self.decoupled_weight_decay:
-                        shampoo_grad.add_(p, alpha=group['weight_decay'])
                         graft_grad.add_(p, alpha=group['weight_decay'])
+                        shampoo_grad.add_(p, alpha=group['weight_decay'])
                     else:
-                        shampoo_grad.mul_(1.0 - group['lr'] * group['weight_decay'])
                         graft_grad.mul_(1.0 - group['lr'] * group['weight_decay'])
+                        shampoo_grad.mul_(1.0 - group['lr'] * group['weight_decay'])
 
                 state['momentum'].mul_(beta1).add_(shampoo_grad)
                 graft_momentum = graft.update_momentum(grad, beta1)
 
-                if is_precondition_step:
-                    momentum_update = state['momentum']
-                    wd_update = shampoo_grad
-                else:
-                    momentum_update = graft_momentum
-                    wd_update = graft_grad
+                momentum_update = state['momentum'] if is_precondition_step else graft_momentum
 
                 if self.nesterov:
                     w: float = (1.0 - beta1) if self.moving_average_for_momentum else 1.0
+
+                    wd_update = shampoo_grad if is_precondition_step else graft_grad
                     wd_update.mul_(w)
 
                     momentum_update.mul_(beta1).add_(wd_update)
 
                 p.add_(momentum_update, alpha=-group['lr'])
 
         return loss
```

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/shampoo_utils.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/shampoo_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import itertools
 from enum import IntEnum
-from typing import List, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 
 
 class LayerWiseGrafting(IntEnum):
     r"""Layer-wise grafting.
@@ -59,15 +59,15 @@
     r"""Graft using SQRTN."""
 
     def __init__(self, var: torch.Tensor):
         super().__init__(var)
 
     def precondition_gradient(self, grad: torch.Tensor) -> torch.Tensor:
         r"""Get preconditioned gradient."""
-        return torch.ones_like(grad) * torch.sign(grad)
+        return grad.sign_()
 
 
 class AdaGradGraft(SGDGraft):
     r"""Graft using Adagrad. Essentially an implementation of Adagrad with momentum.
 
     :param var: torch.Tensor. variable.
     :param diagonal_eps: float. diagonal epsilon.
@@ -111,46 +111,53 @@
 class BlockPartitioner:
     r"""Partition a tensor into smaller tensors for preconditioning.
 
         For example, if a variable has shape (4096, 512), we might split the 4096 into 4 blocks,
         so we effectively have 4 variables of size (1024, 512) each.
 
     :param var: torch.Tensor. tensor variable.
+    :param rank: int. rank.
     :param block_size: int. block size.
     :param pre_conditioner_type: int type of pre-conditioner.
     """
 
-    def __init__(self, var: torch.Tensor, block_size: int, pre_conditioner_type: int):
+    def __init__(self, var: torch.Tensor, rank: int, block_size: int, pre_conditioner_type: int):
         self.shape: List[int] = var.shape
 
         self.splits: List[Tuple[int, np.ndarray]] = []
         self.split_sizes: List[Tuple[int, np.ndarray]] = []
 
         split_sizes: List[np.ndarray] = []
 
         # We split var into smaller blocks. Here we store the metadata to make that split.
         for i, d in enumerate(self.shape):
-            if 0 < block_size < d:
-                # d - 1, otherwise split appends a 0-size array.
-                num_split: int = (d - 1) // block_size
-                indices = (np.arange(num_split, dtype=np.int32) + 1) * block_size
-                sizes = np.ones(num_split + 1, dtype=np.int32) * block_size
-                sizes[-1] = d - indices[-1]
-                self.splits.append((i, indices))
-                self.split_sizes.append((i, sizes))
-                split_sizes.append(sizes)
-            else:
+            if block_size <= 0 or block_size >= d:
                 split_sizes.append(np.array([d], dtype=np.int32))
+                continue
+
+            # d - 1, otherwise split appends a 0-size array.
+            num_split: int = (d - 1) // block_size
+            indices = (np.arange(num_split, dtype=np.int32) + 1) * block_size
+
+            sizes = np.ones(num_split + 1, dtype=np.int32) * block_size
+            sizes[-1] = d - indices[-1]
+
+            self.splits.append((i, indices))
+            self.split_sizes.append((i, sizes))
+            split_sizes.append(sizes)
 
         self.num_splits: int = len(split_sizes)
         self.pre_conditioner_shapes: List[List[int]] = []
         for t in itertools.product(*split_sizes):
-            if not (pre_conditioner_type == PreConditionerType.ALL or self.num_splits <= 1):
-                t = t[:-1]  # noqa: PLW2901
-            self.pre_conditioner_shapes.extend([[d, d] for d in t])
+            t_shape: List[Optional[List[int]]] = [[d, d] for d in t]
+            if pre_conditioner_type == PreConditionerType.INPUT:
+                t_shape = t_shape[:-1] + [None]
+            if pre_conditioner_type == PreConditionerType.OUTPUT:
+                t_shape = [None] * (rank - 1) + t_shape[-1:]
+            self.pre_conditioner_shapes.extend(t_shape)
 
     def shapes_for_pre_conditioners(self) -> List[List[int]]:
         r"""Get shapes of pre-conditioner."""
         return self.pre_conditioner_shapes
 
     def partition(self, x: torch.Tensor) -> List[torch.Tensor]:
         r"""Partition tensor into blocks."""
@@ -180,90 +187,107 @@
         return partitions[0]
 
 
 class PreConditionerType(IntEnum):
     r"""Type of PreConditioner.
 
     In default (ALL), computes pre-conditioner for each dim.
-    INPUT is one-sided Shampoo, in this case only on input dim.
+    INPUT/OUTPUT is one-sided Shampoo, in this case only on input/output dim.
     Assumes last dim is always the output dim and everything else input dim.
     """
 
     ALL = 0
     INPUT = 1
+    OUTPUT = 2
 
 
 class PreConditioner:
     r"""Compute statistics/shape from gradients for preconditioning.
 
     :param var: torch.Tensor. variable.
     :param beta2: float. beta2.
     :param inverse_exponent_override: int.
     :param block_size: int.
+    :param skip_preconditioning_rank_lt: int.
     :param no_preconditioning_for_layers_with_dim_gt: int.
     :param shape_interpretation: bool.
-    :param matrix_eps: float.
     :param pre_conditioner_type: int. type of pre-conditioner.
+    :param matrix_eps: float.
     :param use_svd: bool. use SVD instead of Schur-Newton method to calculate M^{-1/p}.
     """
 
     def __init__(
         self,
         var: torch.Tensor,
         beta2: float,
         inverse_exponent_override: int,
         block_size: int,
+        skip_preconditioning_rank_lt: int,
         no_preconditioning_for_layers_with_dim_gt: int,
         shape_interpretation: bool,
+        pre_conditioner_type: int,
         matrix_eps: float = 1e-6,
-        pre_conditioner_type: int = PreConditionerType.ALL,
         use_svd: bool = False,
     ):
         self.beta2 = beta2
         self.inverse_exponent_override = inverse_exponent_override
+        self.skip_preconditioning_rank_lt = skip_preconditioning_rank_lt
         self.no_preconditioning_for_layers_with_dim_gt = no_preconditioning_for_layers_with_dim_gt
-        self.matrix_eps = matrix_eps
         self.pre_conditioner_type = pre_conditioner_type
+        self.matrix_eps = matrix_eps
         self.use_svd = use_svd
 
         self.w2: float = 1.0 if self.beta2 == 1.0 else (1.0 - self.beta2)
 
         self.original_shape: List[int] = var.shape
-        self.transformed_shape: List[int] = var.shape
-        if shape_interpretation:
-            self.transformed_shape = merge_small_dims(self.original_shape, block_size)
-
-        self.should_precondition_dims: List[bool] = (
-            [True] * len(self.transformed_shape)
-            if self.pre_conditioner_type == PreConditionerType.ALL or len(self.transformed_shape) <= 1
-            else [True] * (len(self.transformed_shape) - 1) + [False]
+        self.transformed_shape: List[int] = (
+            merge_small_dims(self.original_shape, block_size) if shape_interpretation else var.shape
         )
+
+        self.should_precondition_dims: List[bool] = self.get_should_precondition_dims()
         self.rank: int = sum(self.should_precondition_dims)
         self.exponent_for_pre_conditioner: int = (
             self.inverse_exponent_override if self.inverse_exponent_override > 0 else 2 * self.rank
         )
 
         self.statistics: Union[List[torch.Tensor], torch.Tensor] = []
         self.pre_conditioners: Union[List[torch.Tensor], torch.Tensor] = []
+
         self.is_same_shapes: bool = False
         if len(self.transformed_shape) > 1 and not self.skip_precondition(var):
-            reshaped_var = torch.reshape(var, self.transformed_shape)
-            self.partitioner = BlockPartitioner(reshaped_var, block_size, self.pre_conditioner_type)
+            self.partitioner = BlockPartitioner(
+                var=torch.reshape(var, self.transformed_shape),
+                rank=self.rank,
+                block_size=block_size,
+                pre_conditioner_type=self.pre_conditioner_type,
+            )
 
-            shapes = self.partitioner.shapes_for_pre_conditioners()
-            self.statistics = [self.matrix_eps * torch.eye(s[0], device=var.device) for s in shapes]
-            self.pre_conditioners = [torch.eye(s[0], device=var.device) for s in shapes]
-            self.is_same_shapes = len(np.unique(shapes)) == 1
+            shapes: List[Optional[List[int]]] = self.partitioner.shapes_for_pre_conditioners()
+            self.statistics = [self.matrix_eps * torch.eye(shape[0], device=var.device) for shape in shapes if shape]
+            self.pre_conditioners = [torch.eye(shape[0], device=var.device) for shape in shapes if shape]
+            self.is_same_shapes = None not in shapes and len(np.unique(shapes)) == 1
 
         if self.is_same_shapes:
-            self.statistics = torch.stack(self.statistics)
-            self.pre_conditioners = torch.stack(self.pre_conditioners)
+            self.statistics = torch.stack(self.statistics, dim=0)
+            self.pre_conditioners = torch.stack(self.pre_conditioners, dim=0)
+
+    def get_should_precondition_dims(self) -> List[bool]:
+        r"""Get pre-condition dimensions by the type of conditioner."""
+        if self.pre_conditioner_type == PreConditionerType.ALL or len(self.transformed_shape) <= 1:
+            return [True] * len(self.transformed_shape)
+        if self.pre_conditioner_type == PreConditionerType.INPUT:
+            return [True] * (len(self.transformed_shape) - 1) + [False]
+        if self.pre_conditioner_type == PreConditionerType.OUTPUT:
+            return [False] * (len(self.transformed_shape) - 1) + [True]
+        raise ValueError
 
     def skip_precondition(self, x: torch.Tensor) -> bool:
-        return (len(x.shape) < 1) or any(s > self.no_preconditioning_for_layers_with_dim_gt for s in x.shape)
+        return (len(x.shape) < self.skip_preconditioning_rank_lt) or any(
+            dim > self.no_preconditioning_for_layers_with_dim_gt for dim in x.shape
+        )
 
     def add_statistics(self, grad: torch.Tensor):
         r"""Compute statistics from gradients and add to the correct state entries.
 
         :param grad: torch.Tensor. gradient to compute statistics from.
         """
         if len(self.statistics) == 0:
@@ -289,20 +313,20 @@
         """
         if self.use_svd and self.is_same_shapes:
             self.pre_conditioners = compute_power_svd(
                 matrix=self.statistics, power=-1.0 / self.exponent_for_pre_conditioner
             )
             return
 
-        for i in range(len(self.statistics)):
+        for i, statistic in enumerate(self.statistics):
             self.pre_conditioners[i] = (
-                compute_power_svd(matrix=self.statistics[i], power=-1.0 / self.exponent_for_pre_conditioner)
+                compute_power_svd(matrix=statistic, power=-1.0 / self.exponent_for_pre_conditioner)
                 if self.use_svd
                 else compute_power_schur_newton(
-                    mat_g=self.statistics[i], p=self.exponent_for_pre_conditioner, ridge_epsilon=self.matrix_eps
+                    mat_g=statistic, p=self.exponent_for_pre_conditioner, ridge_epsilon=self.matrix_eps
                 )
             )
 
     @staticmethod
     def precondition_block(
         partitioned_grad: torch.Tensor,
         should_preconditioned_dims: List[bool],
@@ -311,19 +335,24 @@
         r"""Perform a preconditioning operation on a single gradient block.
 
         Loop invariant: the dimension to be preconditioned is first
         We keep all axes in the same cyclic order they were originally.
         """
         rank: int = len(partitioned_grad.shape)
         roll: Tuple[int, ...] = (*tuple(range(1, rank)), 0)
-        for j, should_precondition in enumerate(should_preconditioned_dims):
-            if not should_precondition:
-                partitioned_grad = torch.permute(partitioned_grad, roll).contiguous()
+
+        i: int = 0
+        for should_precondition_dim in should_preconditioned_dims:
+            if not should_precondition_dim:
+                partitioned_grad = torch.permute(partitioned_grad, roll)
                 continue
-            partitioned_grad = torch.tensordot(partitioned_grad, pre_conditioners_for_grad[j], dims=[[0], [0]])
+
+            partitioned_grad = torch.tensordot(partitioned_grad, pre_conditioners_for_grad[i], dims=[[0], [0]])
+            i += 1
+
         return partitioned_grad
 
     def preconditioned_grad(self, grad: torch.Tensor) -> torch.Tensor:
         r"""Precondition the gradient.
 
         :param grad: torch.Tensor. a gradient tensor to precondition.
         """
@@ -343,78 +372,61 @@
         ]
 
         merged_grad = self.partitioner.merge_partitions(pre_cond_partitioned_grads)
 
         return torch.reshape(merged_grad, self.original_shape)
 
 
+def build_graft(p: torch.Tensor, graft_type: int, diagonal_eps: float = 1e-10):
+    r"""Build Graft by given graft_type."""
+    if graft_type == LayerWiseGrafting.ADAGRAD:
+        return AdaGradGraft(p, diagonal_eps)
+    if graft_type == LayerWiseGrafting.RMSPROP:
+        return RMSPropGraft(p, diagonal_eps)
+    if graft_type == LayerWiseGrafting.SGD:
+        return SGDGraft(p)
+    if graft_type == LayerWiseGrafting.SQRTN:
+        return SQRTNGraft(p)
+    return Graft(p)
+
+
 @torch.no_grad()
-def power_iter(mat_g: torch.Tensor, error_tolerance: float = 1e-6, num_iters: int = 100) -> torch.Tensor:
-    r"""Power iteration.
+def power_iteration(mat_g: torch.Tensor, error_tolerance: float = 1e-6, num_iters: int = 50) -> torch.Tensor:
+    r"""Compute the maximum eigenvalue of matrix, for scaling.
 
-        Compute the maximum eigenvalue of mat, for scaling. v is a random (uniform) vector with values in (-1, 1).
+        Usually, power_iteration method is faster than torch.einval in case of the symmetric PSD matrix.
 
     :param mat_g: torch.Tensor. the symmetric PSD matrix.
     :param error_tolerance: float. Iterative exit condition.
     :param num_iters: int. Number of iterations.
     """
-    v = 2.0 * torch.rand(list(mat_g.shape)[0], dtype=mat_g.dtype, device=mat_g.device) - 1
+    v = torch.randn(mat_g.shape[0], dtype=mat_g.dtype, device=mat_g.device)
+
+    singular_val = 1e-16
+
+    for _ in range(num_iters):
+        v.div_(torch.linalg.norm(v))
 
-    error: Union[torch.Tensor, float] = 1.0
-    iters: int = 0
-    singular_val: Union[torch.Tensor, float] = 0.0
-    while error > error_tolerance and iters < num_iters:
-        v.div_(v.norm())
         mat_v = torch.mv(mat_g, v)
         s_v = torch.dot(v, mat_v)
 
-        error = torch.abs(s_v - singular_val)
+        if torch.abs_(s_v - singular_val) <= error_tolerance:
+            break
 
         v = mat_v
         singular_val = s_v
-        iters += 1
 
     return singular_val
 
 
 @torch.no_grad()
-def matrix_power(mat_m: torch.Tensor, p: int) -> torch.Tensor:
-    r"""Compute mat_m^{p}.
-
-        Unroll the loop due to the performance.
-
-    :param mat_m: torch.Tensor. a square matrix.
-    :param p: int. a positive integer. usually p = (1, 2, 4, 8).
-    """
-    exponent: int = int(np.log2(p))
-
-    if exponent == 0:
-        return mat_m
-
-    mat_p2 = torch.matmul(mat_m, mat_m).float()
-    if exponent == 1:
-        return mat_p2
-
-    mat_p4 = torch.matmul(mat_p2, mat_p2).float()
-    if exponent == 2:
-        return mat_p4
-
-    mat_p8 = torch.matmul(mat_p4, mat_p4).float()
-    if exponent == 3:
-        return mat_p8
-
-    # most of the cases, never reached here.
-    return torch.matmul(mat_p8, mat_p8).float()
-
-
-@torch.no_grad()
 def compute_power_schur_newton(
     mat_g: torch.Tensor,
     p: int,
-    iter_count: int = 100,
+    max_iters: int = 100,
     error_tolerance: float = 1e-6,
     ridge_epsilon: float = 1e-6,
     max_error_ratio: float = 1.2,
 ) -> torch.Tensor:
     r"""Compute G^{-1/p} using a coupled Newton iteration.
 
         See for example equation 3.2 on page 9 of:
@@ -429,54 +441,55 @@
 
         z = (1 + p) / tf.trace(mat_g)
         If we want the method to always converge, use z = 1 / norm(mat_g) or z = 1 / tf.trace(mat_g),
         but these can result in many extra iterations.
 
     :param mat_g: torch.Tensor. A square positive semi-definite matrix.
     :param p: int. a positive integer.
-    :param iter_count: int. Stop iterating after this many rounds.
+    :param max_iters: int. Stop iterating after this many rounds.
     :param error_tolerance: float. Threshold for stopping iteration.
     :param ridge_epsilon: float. We add this times I to G, to make is positive definite.
         For scaling, we multiply it by the largest eigenvalue of G.
     :param max_error_ratio: float. Sometimes error increases after an iteration before decreasing and converging.
         1.2 factor is used to bound the maximal allowed increase.
     """
-    shape: List[int] = list(mat_g.shape)
+    shape: List[int] = mat_g.shape
     if len(shape) == 1:
         return torch.pow(mat_g + ridge_epsilon, -1.0 / p)
 
-    identity = torch.eye(shape[0], device=mat_g.device, dtype=torch.float32)
+    identity = torch.eye(shape[0], device=mat_g.device, dtype=mat_g.dtype)
     if shape[0] == 1:
         return identity
 
-    max_ev = power_iter(mat_g).clamp_(min=1e-16)
-    ridge_epsilon *= max_ev
-    mat_g += ridge_epsilon * identity
+    mat_g.add_(ridge_epsilon * power_iteration(mat_g) * identity)
 
-    z = (1 + p) / (2 * torch.norm(mat_g))
+    z = (1 + p) / (2 * torch.linalg.norm(mat_g))
 
     mat_root = identity * torch.pow(z, 1.0 / p)
     mat_m = mat_g * z
 
     alpha: float = -1.0 / p
     alpha_identity = (1.0 - alpha) * identity
+
     error = torch.max(torch.abs(mat_m - identity))
-    count: int = 0
-    while error > error_tolerance and count < iter_count:
+
+    new_mat_root = torch.empty_like(mat_root)
+
+    for _ in range(max_iters):
         mat_m_i = alpha_identity + alpha * mat_m
-        new_mat_root = torch.matmul(mat_root, mat_m_i).float()
-        mat_m = torch.matmul(matrix_power(mat_m_i, p), mat_m).float()
+
+        torch.matmul(mat_root, mat_m_i, out=new_mat_root)
+        torch.matmul(torch.linalg.matrix_power(mat_m_i, p), mat_m, out=mat_m)
 
         new_error = torch.max(torch.abs(mat_m - identity))
-        if new_error > error * max_error_ratio:
+        if new_error <= error_tolerance or new_error > error * max_error_ratio:
             break
 
         mat_root = new_mat_root
         error = new_error
-        count += 1
 
     return mat_root
 
 
 @torch.no_grad()
 def compute_power_svd(matrix: torch.Tensor, power: float) -> torch.Tensor:
     r"""Compute G^{-1/p} using a SVD.
@@ -495,28 +508,22 @@
 def merge_small_dims(shape_to_merge: List[int], max_dim: int) -> List[int]:
     r"""Merge small dimensions.
 
         If there are some small dimensions, we collapse them
             e.g. [1, 2, 512, 1, 2048, 1, 3, 4] --> [1024, 2048, 12] if max_dim = 1024
             [1, 2, 768, 1, 2048] --> [2, 768, 2048].
 
-    :param shape_to_merge: List. Shape to merge small dimensions.
+    :param shape_to_merge: List[int]. Shape to merge small dimensions.
     :param max_dim: int. Maximal dimension of output shape used in merging.
     """
-    if shape_to_merge and np.all(np.array(shape_to_merge) == 1):
-        return [1]
-
-    resulting_shape: List[int] = []
+    merged_shape: List[int] = []
 
     product: int = 1
-    for d in shape_to_merge:
-        if product * d <= max_dim:
-            product *= d
-        else:
-            if product > 1:
-                resulting_shape.append(product)
-            product = d
+    for dim in shape_to_merge:
+        product *= dim
+        if product > max_dim:
+            merged_shape.append(product // dim)
+            product = dim
 
-    if product > 1:
-        resulting_shape.append(product)
+    merged_shape.append(product)
 
-    return resulting_shape
+    return merged_shape if len(merged_shape) > 1 else [1]
```

### Comparing `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/utils.py` & `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.2/PKG-INFO` & `pytorch_optimizer-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-optimizer
-Version: 2.5.2
+Version: 2.6.0
 Summary: optimizer & lr scheduler implementations in PyTorch with clean-code, strict types. Also, including useful optimization ideas.
 Home-page: https://github.com/kozistr/pytorch_optimizer
 License: Apache-2.0
 Keywords: pytorch,deep-learning,optimizer,lr scheduler
 Author: kozistr
 Author-email: kozistr@gmail.com
 Maintainer: kozistr
@@ -31,48 +31,47 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: numpy (==1.21.1) ; python_version >= "3.7" and python_version < "3.8"
 Requires-Dist: numpy ; python_version >= "3.8"
+Requires-Dist: torch (>=1.10) ; python_version >= "3.8"
 Requires-Dist: torch (>=1.10,<2.0) ; python_version >= "3.7" and python_version < "3.8"
-Requires-Dist: torch (>=2.0) ; python_version >= "3.8"
 Project-URL: Documentation, https://pytorch-optimizers.readthedocs.io/en/latest
 Project-URL: Repository, https://github.com/kozistr/pytorch_optimizer
 Description-Content-Type: text/x-rst
 
 =================
 pytorch-optimizer
 =================
 
 +--------------+------------------------------------------+
 | Build        | |workflow| |Documentation Status|        |
 +--------------+------------------------------------------+
-| Quality      | |codecov| |black|                        |
+| Quality      | |codecov| |black| |ruff|                 |
 +--------------+------------------------------------------+
 | Package      | |PyPI version| |PyPI pyversions|         |
 +--------------+------------------------------------------+
 | Status       | |PyPi download| |PyPi month download|    |
 +--------------+------------------------------------------+
+| License      | |apache|                                 |
++--------------+------------------------------------------+
 
 | **pytorch-optimizer** is bunch of optimizer collections in PyTorch. Also, including useful optimization ideas.
 | Most of the implementations are based on the original paper, but I added some tweaks.
 | Highly inspired by `pytorch-optimizer <https://github.com/jettify/pytorch-optimizer>`__.
 
-Documentation
--------------
-
-https://pytorch-optimizers.readthedocs.io/en/latest/
+Getting Started
+---------------
 
-Usage
------
+For more, see the `documentation <https://pytorch-optimizers.readthedocs.io/en/latest/>`__.
 
-Install
-~~~~~~~
+Installation
+~~~~~~~~~~~~
 
 ::
 
     $ pip3 install -U pytorch-optimizer
 
 If there's a version issue when installing the package, try with `--no-deps` option.
 
@@ -113,15 +112,15 @@
 ::
 
     from pytorch_optimizer import create_optimizer
 
     optimizer = create_optimizer(
         model,
         'adamp',
-        lr=1e-2,
+        lr=1e-3,
         weight_decay=1e-3,
         use_gc=True,
         use_lookahead=True,
     )
 
 Supported Optimizers
 --------------------
@@ -178,14 +177,16 @@
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | NovoGrad     | *Stochastic Gradient Methods with Layer-wise Adaptive Moments for Training of Deep Networks*    | `github <https://github.com/lonePatient/NovoGrad-pytorch>`__                      | `https://arxiv.org/abs/1905.11286 <https://arxiv.org/abs/1905.11286>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | Lion         | *Symbolic Discovery of Optimization Algorithms*                                                 | `github <https://github.com/google/automl/tree/master/lion>`__                    | `https://arxiv.org/abs/2302.06675 <https://arxiv.org/abs/2302.06675>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | Ali-G        | *Adaptive Learning Rates for Interpolation with Gradients*                                      | `github <https://github.com/oval-group/ali-g>`__                                  | `https://arxiv.org/abs/1906.05661 <https://arxiv.org/abs/1906.05661>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| SM3          | *Memory-Efficient Adaptive Optimization*                                                        | `github <https://github.com/google-research/google-research/tree/master/sm3>`__   | `https://arxiv.org/abs/1901.11150 <https://arxiv.org/abs/1901.11150>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 
 Useful Resources
 ----------------
 
 Several optimization ideas to regularize & stabilize the training. Most
 of the ideas are applied in ``Ranger21`` optimizer.
 
@@ -383,14 +384,16 @@
 
 `NovoGrad <https://ui.adsabs.harvard.edu/abs/2019arXiv190511286G/exportcitation>`__
 
 `Lion <https://github.com/google/automl/tree/master/lion#citation>`__
 
 `Ali-G <https://github.com/oval-group/ali-g#adaptive-learning-rates-for-interpolation-with-gradients>`__
 
+`SM3 <https://ui.adsabs.harvard.edu/abs/2019arXiv190111150A/exportcitation>`__
+
 Citation
 --------
 
 Please cite original authors of optimization algorithms. If you use this software, please cite it as below.
 Or you can get from "cite this repository" button.
 
 ::
@@ -416,10 +419,14 @@
 .. |PyPi download| image:: https://pepy.tech/badge/pytorch-optimizer
    :target: https://pepy.tech/project/pytorch-optimizer
 .. |PyPi month download| image:: https://pepy.tech/badge/pytorch-optimizer/month
    :target: https://pepy.tech/project/pytorch-optimizer
 .. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/pytorch-optimizer.svg
    :target: https://pypi.python.org/pypi/pytorch-optimizer/
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. |ruff| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+   :target: https://github.com/charliermarsh/ruff
 .. |codecov| image:: https://codecov.io/gh/kozistr/pytorch_optimizer/branch/main/graph/badge.svg?token=L4K00EA0VD
    :target: https://codecov.io/gh/kozistr/pytorch_optimizer
+.. |apache| image:: https://img.shields.io/badge/License-Apache_2.0-blue.svg
+   :target: https://opensource.org/licenses/Apache-2.0
```

