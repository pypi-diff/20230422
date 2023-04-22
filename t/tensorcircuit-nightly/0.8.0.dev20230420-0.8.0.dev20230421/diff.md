# Comparing `tmp/tensorcircuit-nightly-0.8.0.dev20230420.tar.gz` & `tmp/tensorcircuit-nightly-0.8.0.dev20230421.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.8.0.dev20230420.tar", last modified: Thu Apr 20 12:39:42 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.8.0.dev20230421.tar", last modified: Fri Apr 21 12:38:52 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.8.0.dev20230420.tar` & `tensorcircuit-nightly-0.8.0.dev20230421.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:42.491498 tensorcircuit-nightly-0.8.0.dev20230420/
--rw-r--r--   0 runner    (1001) docker     (122)    23108 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-20 12:39:42.491498 tensorcircuit-nightly-0.8.0.dev20230420/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:42.479498 tensorcircuit-nightly-0.8.0.dev20230420/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:42.483498 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27374 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-20 12:39:42.491498 tensorcircuit-nightly-0.8.0.dev20230420/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-04-20 12:39:37.000000 tensorcircuit-nightly-0.8.0.dev20230420/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:42.483498 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-04-20 12:39:37.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:42.483498 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:42.487498 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    56998 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14944 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24632 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    30672 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36236 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:42.487498 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:42.487498 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    28754 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29161 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:42.487498 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     9942 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     5046 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     9975 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34398 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11878 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:42.487498 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31378 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:42.487498 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27351 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     6603 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:42.487498 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-20 12:39:42.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3438 2023-04-20 12:39:42.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 12:39:42.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-20 12:39:42.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-20 12:39:42.000000 tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:42.491498 tensorcircuit-nightly-0.8.0.dev20230420/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33200 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    45826 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13296 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-04-20 12:17:03.000000 tensorcircuit-nightly-0.8.0.dev20230420/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:38:52.215334 tensorcircuit-nightly-0.8.0.dev20230421/
+-rw-r--r--   0 runner    (1001) docker     (122)    23305 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-21 12:38:52.215334 tensorcircuit-nightly-0.8.0.dev20230421/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:38:52.203333 tensorcircuit-nightly-0.8.0.dev20230421/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:38:52.207333 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27374 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-21 12:38:52.215334 tensorcircuit-nightly-0.8.0.dev20230421/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-04-21 12:38:47.000000 tensorcircuit-nightly-0.8.0.dev20230421/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:38:52.211334 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-04-21 12:38:46.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:38:52.211334 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:38:52.211334 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56998 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24632 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30672 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:38:52.211334 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:38:52.211334 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28754 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:38:52.211334 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5030 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9959 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34350 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:38:52.211334 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/results/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:38:52.215334 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:38:52.215334 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-21 12:38:52.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3438 2023-04-21 12:38:52.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 12:38:52.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-21 12:38:52.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-21 12:38:52.000000 tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:38:52.215334 tensorcircuit-nightly-0.8.0.dev20230421/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33200 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46467 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-04-21 12:16:42.000000 tensorcircuit-nightly-0.8.0.dev20230421/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/CHANGELOG.md` & `tensorcircuit-nightly-0.8.0.dev20230421/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,30 @@
 
 ## Unreleased
 
 ### Added
 
 - Add `tc.about()` to print related software versions and configs
 
-- Torch support is updraded to 2.0, and now support native vmap and native functional grad, and thus `vvag`. Still jit support is conflict with these functional transformations and be turned off by default
+- Torch support is upgraded to 2.0, and now support native vmap and native functional grad, and thus `vvag`. Still jit support is conflict with these functional transformations and be turned off by default
 
 - Add `torch_interfaces_kws` that support static keyword arguments when wrapping with the interface
 
+- Add `gpu_memory_share` function and enable it by default
+
 ### Fixed
 
 - Add tests and fixed some missing methods for cupy backend, cupy backend is now ready to use (though still not guaranteed)
 
+- Fix adjoint gate numpy conversion for fixed gate case
+
+### Changed
+
+- Upgraded black and mypy==1.2.0 (breaking change for developers)
+
 ## 0.8.0
 
 ### Added
 
 - Add `initial_mapping` circuit method to return a new circuit with given `logical_physical_mapping`
 
 - Add `get_positional_logical_mapping` circuit method to return the mapping when only part of the qubits are measured
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/HISTORY.md` & `tensorcircuit-nightly-0.8.0.dev20230421/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/LICENSE` & `tensorcircuit-nightly-0.8.0.dev20230421/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/PKG-INFO` & `tensorcircuit-nightly-0.8.0.dev20230421/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.8.0.dev20230420
+Version: 0.8.0.dev20230421
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/README.md` & `tensorcircuit-nightly-0.8.0.dev20230421/README.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/README_cn.md` & `tensorcircuit-nightly-0.8.0.dev20230421/README_cn.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/docs/source/advance.rst` & `tensorcircuit-nightly-0.8.0.dev20230421/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/docs/source/cnconf.py` & `tensorcircuit-nightly-0.8.0.dev20230421/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/docs/source/conf.py` & `tensorcircuit-nightly-0.8.0.dev20230421/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/docs/source/contribution.rst` & `tensorcircuit-nightly-0.8.0.dev20230421/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/docs/source/faq.rst` & `tensorcircuit-nightly-0.8.0.dev20230421/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/docs/source/generate_rst.py` & `tensorcircuit-nightly-0.8.0.dev20230421/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/docs/source/index.rst` & `tensorcircuit-nightly-0.8.0.dev20230421/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/docs/source/infras.rst` & `tensorcircuit-nightly-0.8.0.dev20230421/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/docs/source/modules.rst` & `tensorcircuit-nightly-0.8.0.dev20230421/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/docs/source/modules.rst.backup` & `tensorcircuit-nightly-0.8.0.dev20230421/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.8.0.dev20230421/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.8.0.dev20230421/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.8.0.dev20230421/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.8.0.dev20230421/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.8.0.dev20230421/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/setup.py` & `tensorcircuit-nightly-0.8.0.dev20230421/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-__version__ = "0.8.0.dev20230420"
+__version__ = "0.8.0.dev20230421"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
+from .utils import gpu_memory_share
+
+gpu_memory_share()
+
 from .about import about
 from .cons import (
     backend,
     set_backend,
     set_dtype,
     set_contractor,
     get_backend,
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/about.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/cupy_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
     def left_shift(self, x: Tensor, y: Tensor) -> Tensor:
         return cp.left_shift(x, y)
 
     def solve(self, A: Tensor, b: Tensor, assume_a: str = "gen") -> Tensor:  # type: ignore
         raise NotImplementedError
 
     def searchsorted(self, a: Tensor, v: Tensor, side: str = "left") -> Tensor:
-        return cp.searchsorted(a, v, side=side)  # type: ignore
+        return cp.searchsorted(a, v, side=side)
 
     def set_random_state(
         self, seed: Optional[int] = None, get_only: bool = False
     ) -> Any:
         g = cp.random.default_rng(seed)  # None auto supported
         if get_only is False:
             self.g = g
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/jax_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 def jaxqr_bwd(res: Sequence[Array], tangents: Sequence[Array]) -> Tuple[Array]:
     a, q, r = res
     dq, dr = tangents
     dq = dq.conj()
     dr = dr.conj()
 
     def _TriangularSolve(x: Array, r: Array) -> Array:
-        return jax.scipy.linalg.solve_triangular(  # type: ignore
+        return jax.scipy.linalg.solve_triangular(
             r, x.T.conj(), lower=False, trans=0
         ).T.conj()
 
     def _QrGradSquareAndDeepMatrices(q: Array, r: Array, dq: Array, dr: Array) -> Array:
         # Modification begins
         rdiag = jnp.diag(r)
         rdiag = (jnp.abs(rdiag) < qr_epsilon) * qr_epsilon + (
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -770,15 +770,15 @@
         if with_prob:
             return sample, p
         else:
             return sample, -1.0
 
     # TODO(@refraction-ray): more _before function like state_before? and better API?
 
-    def expectation(  # type: ignore
+    def expectation(
         self,
         *ops: Tuple[tn.Node, List[int]],
         reuse: bool = True,
         enable_lightcone: bool = False,
         noise_conf: Optional[Any] = None,
         nmc: int = 1000,
         status: Optional[Tensor] = None,
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cloud/apis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cloud/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/compiler/composed_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/gates.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import warnings
 
 import numpy as np
 import tensornetwork as tn
 from scipy.stats import unitary_group
 
 from .cons import backend, dtypestr, npdtype
-from .backends import get_backend
 from .utils import arg_alias
 
 thismodule = sys.modules[__name__]
 
 Tensor = Any
 Array = Any
 Operator = Any  # QuOperator
@@ -253,30 +252,26 @@
         if not n:
             n = "unknowngate"
         self.m = m
         self.n = n
         self.ctrl = ctrl
 
     def __call__(self, *args: Any, **kws: Any) -> Gate:
-        # m = array_to_tensor(self.m)
+        m1 = array_to_tensor(self.m)
         # m = backend.cast(m, dtypestr)
-        m = self.m.astype(npdtype)
-        return Gate(deepcopy(m), name=self.n)
+        m1 = backend.cast(m1, dtypestr)
+        return Gate(m1, name=self.n)
 
     def adjoint(self) -> "GateF":
         m = self.__call__()
-        npb = get_backend("numpy")
-        shape0 = npb.shape_tuple(m.tensor)
-        m0 = npb.reshapem(m.tensor)
-        ma = npb.adjoint(m0)
-        if np.allclose(m0, ma, atol=1e-5):
-            name = self.n
-        else:
-            name = self.n + "d"
-        ma = npb.reshape(ma, shape0)
+        shape0 = backend.shape_tuple(m.tensor)
+        m0 = backend.reshapem(m.tensor)
+        ma = backend.adjoint(m0)
+        name = self.n + "d"
+        ma = backend.reshape(ma, shape0)
         return GateF(ma, name, self.ctrl)
 
     # TODO(@refraction-ray): adjoint gate convention finally determined
     def ided(self, before: bool = True) -> "GateF":
         def f(*args: Any, **kws: Any) -> Any:
             m = self.__call__(*args, **kws)
             u = m.tensor
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/interfaces/tensortrans.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,18 +46,20 @@
         return t
     if t is None:
         return
     return which_backend(t).numpy(t)
 
 
 def tensor_to_backend_jittable(t: Tensor) -> Tensor:
-    if which_backend(t, return_backend=False) == backend.name:
-        return t
     if isinstance(t, int) or isinstance(t, float):
         return t
+    if isinstance(t, QuOperator):
+        return t
+    if which_backend(t, return_backend=False) == backend.name:
+        return t
     return backend.convert_to_tensor(which_backend(t).numpy(t))
 
 
 def numpy_to_tensor(t: Array, backend: Any) -> Tensor:
     if isinstance(t, int) or isinstance(t, float):
         return t
     return backend.convert_to_tensor(t)
@@ -272,22 +274,33 @@
                 else:
                     is_krauslist = False
 
                 if gate_to_tensor:
                     arg = backend.tree_map(
                         partial(gate_to_matrix, is_reshapem=gate_as_matrix), arg
                     )
-                if qop_to_matrix:
+                if qop_as_matrix:
                     arg = backend.tree_map(
                         partial(qop_to_matrix, is_reshapem=qop_as_matrix), arg
                     )
                 arg = backend.tree_map(tensor_to_backend_jittable, arg)
+
                 # arg = backend.tree_map(backend.convert_to_tensor, arg)
+                def _cast(a: Tensor, dtype: str) -> Tensor:
+                    if isinstance(a, QuOperator):
+                        return a
+                    return backend.cast(a, dtype)
+
+                def _reshapem(a: Tensor) -> Tensor:
+                    if isinstance(a, QuOperator):
+                        return a
+                    return backend.reshapem(a)
+
                 if cast_dtype:
-                    arg = backend.tree_map(partial(backend.cast, dtype=dtypestr), arg)
+                    arg = backend.tree_map(partial(_cast, dtype=dtypestr), arg)
                 if tensor_as_matrix:
                     arg = backend.tree_map(backend.reshapem, arg)
 
                 if is_krauslist is True:
                     arg = KrausList(arg, name, is_unitary)
             nargs.append(arg)
         return f(*nargs, **kws)
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/interfaces/torch.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/interfaces/torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             )
             r = backend.tree_map(lambda s: s.to(device=ctx.device), r)
             if not is_sequence(r):
                 return (r,)
             return r
 
     # currently, memory transparent dlpack in these ML framework has broken support on complex dtypes
-    return Fun.apply  # type: ignore
+    return Fun.apply
 
 
 pytorch_interface = torch_interface
 
 
 def torch_interface_kws(
     f: Callable[..., Any], jit: bool = True, enable_dlpack: bool = False
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/keras.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     #     base_config = super().get_config()
     #     return dict(list(base_config.items()) + list(config.items()))
 
 
 KerasLayer = QuantumLayer
 
 
-class HardwareLayer(QuantumLayer):  # type: ignore
+class HardwareLayer(QuantumLayer):
     @tf.autograph.experimental.do_not_convert  # type: ignore
     def call(
         self,
         inputs: tf.Tensor,
         training: Optional[bool] = None,
         mask: Optional[tf.Tensor] = None,
         **kwargs: Any
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/mpscircuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,16 +518,16 @@
         # TODO(@SUSYUSTC): jax autograd is wrong on this function
         """
         Apply a n-qubit gate by transforming the gate to MPO
         """
         ordered = np.all(np.diff(index) > 0)
         if not ordered:
             order = np.argsort(index)
-            order2 = order + len(index)  # type: ignore
-            order_all = order.tolist() + order2.tolist()  # type: ignore
+            order2 = order + len(index)
+            order_all = order.tolist() + order2.tolist()
             newgate = backend.transpose(gate.tensor, order_all)
             index = np.sort(index).tolist()
             self.apply_nqubit_gate(newgate, *index, split=split)
             return
         if split is None:
             split = self.split
         MPO, index_left = self.gate_to_MPO(gate, *index)
@@ -810,15 +810,15 @@
             nqubits,
             tensors=tensors,
             center_position=center_position,
             split=self.split.copy(),
         )
         return mps
 
-    def expectation(  # type: ignore
+    def expectation(
         self,
         *ops: Tuple[Gate, List[int]],
         reuse: bool = True,
         other: Optional["MPSCircuit"] = None,
         conj: bool = True,
         normalize: bool = False,
         split: Optional[Dict[str, Any]] = None,
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/noisemodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         noise_conf = NoiseConf()
 
     readout_error = noise_conf.readout_error
 
     if noise_conf.has_quantum:
         # density matrix
         if isinstance(c, DMCircuit):
-            cnoise = circuit_with_noise(c, noise_conf)  #  type: ignore
+            cnoise = circuit_with_noise(c, noise_conf)
             return cnoise.sample_expectation_ps(
                 x=x, y=y, z=z, shots=shots, status=status, readout_error=readout_error
             )
 
         # monte carlo
         else:
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/results/readout_mitigation.py`

 * *Files 1% similar despite different names*

```diff
@@ -545,15 +545,15 @@
                 )
             )
 
         if not given_list:
             r = quasi_out[0]
             r = sort_count(r)
             r = {k: v * shots for k, v in r.items()}
-            return sort_count(r)  # type: ignore
+            return sort_count(r)
             # return quasi_out[0]  # type: ignore
         mitcounts = QuasiCollection(quasi_out)
         return sort_count(mitcounts.nearest_probability_distribution())  # type: ignore
 
     def _apply_correction(  # type: ignore
         self,
         counts,
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/translation.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,15 +437,15 @@
     :rtype: Any
     """
     if circuit_constructor is not None:
         Circ = circuit_constructor
     elif is_dm:
         Circ = DMCircuit2
     else:
-        Circ = Circuit  # type: ignore
+        Circ = Circuit
     if circuit_params is None:
         circuit_params = {}
     if "nqubits" not in circuit_params:
         circuit_params["nqubits"] = n
     if (
         len(qcdata) > 0
         and qcdata[0][0].name == "initialize"
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 """
 Helper functions
 """
 
 from typing import Any, Callable, Union, Sequence, Tuple, Dict
 from functools import wraps
+import os
 import platform
 import re
 import time
 
 
+def gpu_memory_share(flag: bool = True) -> None:
+    # TODO(@refraction-ray): the default torch behavior should be True
+    # preallocate behavior for torch to be investigated
+    if flag is True:
+        os.environ["TF_FORCE_GPU_ALLOW_GROWTH"] = "true"
+        os.environ["XLA_PYTHON_CLIENT_PREALLOCATE"] = "false"
+    else:
+        os.environ["TF_FORCE_GPU_ALLOW_GROWTH"] = "false"
+        os.environ["XLA_PYTHON_CLIENT_PREALLOCATE"] = "true"
+
+
 def return_partial(
     f: Callable[..., Any], return_argnums: Union[int, Sequence[int]] = 0
 ) -> Callable[..., Any]:
     r"""
     Return a callable function for output ith parts of the original output along the first axis.
     Original output supports List and Tensor.
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.8.0.dev20230420
+Version: 0.8.0.dev20230421
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.8.0.dev20230421/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/conftest.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_backends.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_calibrating.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_channels.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_circuit.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1511,7 +1511,28 @@
     assert c.get_positional_logical_mapping() == {0: 0, 1: 1, 2: 2}
     c = tc.Circuit(3)
     c.cx(0, 1)
     c.h(1)
     c.measure_instruction(2)
     c.measure_instruction(0)
     assert c.get_positional_logical_mapping() == {0: 2, 1: 0}
+
+
+@pytest.mark.parametrize("backend", [lf("tfb"), lf("jaxb")])
+def test_inverse_jit(backend):
+    K = tc.backend
+
+    def simple_ansatz(param):
+        c = tc.Circuit(3)
+        for i in range(3):
+            c.cx(i, (i + 1) % 3)
+            c.rzz(i, (i + 1) % 3, theta=param[i])
+        c1 = c.inverse()
+        c2 = tc.Circuit(3)
+        c2.x(1)
+        c1.append(c2)
+        return tc.backend.real(c1.expectation_ps(z=[1]))
+
+    v_ansatz = K.jit(K.vvag(simple_ansatz))
+    vs, gs = v_ansatz(K.ones([2, 3], dtype="float32"))
+    assert K.shape_tuple(gs) == (2, 3)
+    np.testing.assert_allclose(K.numpy(vs), -1.0 * K.ones([2]), atol=1e-5)
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_compiler.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_ensemble.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_gates.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_interfaces.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,10 +421,9 @@
         [tc.Gate(np.ones([2, 2])), tc.Gate(np.ones([2, 2, 2, 2]))],
         tc.QuOperator.from_tensor(np.ones([2, 2, 2, 2, 2, 2])),
         np.ones([2, 2, 2, 2]),
     )
 
     assert tc.interfaces.which_backend(a[0], return_backend=False) == tc.backend.name
     assert tc.backend.shape_tuple(a[1]) == (2, 2, 2, 2)
-    assert tc.interfaces.which_backend(b, return_backend=False) == tc.backend.name
-    assert tc.backend.shape_tuple(b) == (2, 2, 2, 2, 2, 2)
+    assert tc.backend.shape_tuple(b.eval()) == (2, 2, 2, 2, 2, 2)
     assert tc.backend.shape_tuple(c) == (2, 2, 2, 2)
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_keras.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_miscs.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_miscs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_qaoa.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_quantum.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_results.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_simplify.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_templates.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_torchnn.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230420/tests/test_van.py` & `tensorcircuit-nightly-0.8.0.dev20230421/tests/test_van.py`

 * *Files identical despite different names*

