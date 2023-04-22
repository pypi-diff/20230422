# Comparing `tmp/affine_transform-0.2.8.tar.gz` & `tmp/affine_transform-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/affine_transform-0.2.8.tar", last modified: Fri Feb 14 21:06:54 2020, max compression
+gzip compressed data, was "affine_transform-0.2.9.tar", last modified: Sat Apr 22 11:29:19 2023, max compression
```

## Comparing `affine_transform-0.2.8.tar` & `affine_transform-0.2.9.tar`

### file list

```diff
@@ -1,471 +1,487 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)      232 2020-02-14 21:05:58.000000 affine_transform-0.2.8/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      422 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/how_to_use.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     6862 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/conf.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/docs/cpp_docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      107 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/cpp_docs/transform_loop.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/cpp_docs/transform.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       75 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/cpp_docs/extract.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      357 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/cpp_docs/python_bindings.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      115 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/cpp_docs/constant_boundary.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/cpp_docs/linear_interpolation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/cpp_docs/apply_interpolation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1287 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/cpp_docs/interpolation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      107 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/cpp_docs/cubic_interpolation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      196 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/cpp_docs/data_struct.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      652 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/cpp_docs/affine_transform.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/module_doc.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/docs/cpp/
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/cpp/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)   112013 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/cpp/Doxyfile
--rw-rw-r--   0 travis    (2000) travis    (2000)      477 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      759 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/cpp_doc.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      752 2020-02-14 21:05:58.000000 affine_transform-0.2.8/docs/make.bat
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/include/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/include/affine_transform/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18132 2020-02-14 21:05:58.000000 affine_transform-0.2.8/include/affine_transform/interpolation.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6268 2020-02-14 21:05:58.000000 affine_transform-0.2.8/include/affine_transform/affine_transform.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4363 2020-02-14 21:06:54.000000 affine_transform-0.2.8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/src/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5312 2020-02-14 21:05:58.000000 affine_transform-0.2.8/src/main.cpp
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/affine_transform.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4363 2020-02-14 21:06:54.000000 affine_transform-0.2.8/affine_transform.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-14 21:06:54.000000 affine_transform-0.2.8/affine_transform.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2020-02-14 21:06:54.000000 affine_transform-0.2.8/affine_transform.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-14 21:06:12.000000 affine_transform-0.2.8/affine_transform.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)    18404 2020-02-14 21:06:54.000000 affine_transform-0.2.8/affine_transform.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2020-02-14 21:06:54.000000 affine_transform-0.2.8/affine_transform.egg-info/requires.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1389 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/KLUSupport
--rw-rw-r--   0 travis    (2000) travis    (2000)     1751 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/PaStiXSupport
--rw-rw-r--   0 travis    (2000) travis    (2000)     1235 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/SparseCholesky
--rw-rw-r--   0 travis    (2000) travis    (2000)     1948 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/Geometry
--rw-rw-r--   0 travis    (2000) travis    (2000)     1116 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/PardisoSupport
--rw-rw-r--   0 travis    (2000) travis    (2000)     1900 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/CholmodSupport
--rw-rw-r--   0 travis    (2000) travis    (2000)      991 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/MetisSupport
--rw-rw-r--   0 travis    (2000) travis    (2000)      122 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/Dense
--rw-rw-r--   0 travis    (2000) travis    (2000)      945 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/QtAlignedMalloc
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/KLUSupport/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11534 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/KLUSupport/KLUSupport.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/PaStiXSupport/
--rw-rw-r--   0 travis    (2000) travis    (2000)    22249 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCholesky/
--rw-rw-r--   0 travis    (2000) travis    (2000)    24177 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5816 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11962 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Hyperplane.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7773 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Translation.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/arch/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5823 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/arch/Geometry_SSE.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8423 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/AngleAxis.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6191 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Umeyama.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3639 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/EulerAngles.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    61854 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Transform.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8063 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/RotationBase.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    32995 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Quaternion.h
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6717 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Scaling.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9817 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/ParametrizedLine.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8955 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/OrthoMethods.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6877 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Rotation2D.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14840 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/AlignedBox.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    20539 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Homogeneous.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/PardisoSupport/
--rw-rw-r--   0 travis    (2000) travis    (2000)    20091 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/StlSupport/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2809 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/StlSupport/details.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5338 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/StlSupport/StdVector.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4155 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/StlSupport/StdList.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5125 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/StlSupport/StdDeque.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/CholmodSupport/
--rw-rw-r--   0 travis    (2000) travis    (2000)    25441 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/MetisSupport/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4588 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/MetisSupport/MetisSupport.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9028 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7602 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2889 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6584 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3681 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5723 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4181 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10034 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    27954 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10217 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6712 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8485 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4303 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLUImpl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4545 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4974 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_Structs.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/
--rw-rw-r--   0 travis    (2000) travis    (2000)    19027 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    59005 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/BlockMethods.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2937 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6915 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/ReshapedMethods.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13132 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6089 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4828 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6375 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    12283 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/IndexedViewMethods.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6850 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14962 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13349 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8875 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6755 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7349 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    15048 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4158 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SuperLUSupport/
--rw-rw-r--   0 travis    (2000) travis    (2000)    34346 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/misc/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2913 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/misc/Image.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1748 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/misc/RealSvd2x2.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    30560 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/misc/blas.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7834 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/misc/lapack.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2742 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/misc/Kernel.h
--rwxrwxr-x   0 travis    (2000) travis    (2000)  1058369 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/misc/lapacke.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      474 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/misc/lapacke_mangling.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Cholesky/
--rw-rw-r--   0 travis    (2000) travis    (2000)    24837 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Cholesky/LDLT.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    18683 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Cholesky/LLT.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3974 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SPQRSupport/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11826 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Jacobi/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16373 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Jacobi/Jacobi.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/UmfPackSupport/
--rw-rw-r--   0 travis    (2000) travis    (2000)    24456 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/LU/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3439 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/LU/Determinant.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/LU/arch/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13662 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/LU/arch/Inverse_SSE.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    21856 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/LU/PartialPivLU.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3555 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    15102 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/LU/InverseImpl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    32313 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/LU/FullPivLU.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15492 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseRef.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6437 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseTriangularView.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3175 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseTranspose.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4711 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    25715 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5808 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9657 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/TriangularSolver.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    57169 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseMatrix.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14832 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseVector.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6827 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseUtil.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    25426 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6485 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseColEtree.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13606 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7050 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseProduct.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8110 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseView.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13178 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    11368 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseAssign.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1107 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseFuzzy.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13256 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3080 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseDot.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2191 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    23759 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseBlock.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7329 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparsePermutation.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8743 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/CompressedStorage.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1699 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseRedux.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8704 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10537 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/AmbiVector.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    17451 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4424 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseSolverBase.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    12589 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseMap.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/QR/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4662 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2993 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    26768 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/QR/FullPivHouseholderQR.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    25498 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/QR/ColPivHouseholderQR.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14641 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/QR/HouseholderQR.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    23029 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Householder/
--rw-rw-r--   0 travis    (2000) travis    (2000)    23569 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Householder/HouseholderSequence.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5365 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Householder/Householder.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4784 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Householder/BlockHouseholder.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17000 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Reshaped.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    51671 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/MathFunctions.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5759 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Fuzzy.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    19214 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/ArithmeticSequence.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    28139 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/GenericPacketMath.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14670 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/DiagonalMatrix.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    38039 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/TriangularMatrix.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9197 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/PartialReduxEvaluator.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3488 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/VectorBlock.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9304 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Visitor.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    18400 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Block.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3519 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Inverse.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    23793 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/MatrixBase.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/GPU/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2695 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5838 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    16855 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    26865 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/GPU/Half.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    52270 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/GPU/PacketMathHalf.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/ZVector/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8025 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxrwxr-x   0 travis    (2000) travis    (2000)    40672 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    20514 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/ZVector/Complex.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5206 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1453 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    36713 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    19172 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX/Complex.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AltiVec/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2170 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rwxrwxr-x   0 travis    (2000) travis    (2000)    42819 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    17442 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/MSA/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16159 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    37020 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    20970 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/MSA/Complex.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/CUDA/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4244 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/CUDA/Complex.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SYCL/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11407 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2626 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    23172 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    21856 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6779 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/Default/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1746 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/Default/Settings.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    19102 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/NEON/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1145 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1338 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    31150 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    19035 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/NEON/Complex.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SSE/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5738 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2010 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
--rwxrwxr-x   0 travis    (2000) travis    (2000)    42840 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    20480 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SSE/Complex.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX512/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15855 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    54439 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    19583 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX512/Complex.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/HIP/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/HIP/hcc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      691 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7333 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Product.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7227 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Map.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14385 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Transpositions.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4218 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/ReturnByValue.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3877 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CwiseUnaryOp.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14553 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/StlIterators.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6990 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/ConditionEstimator.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6797 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Solve.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    16713 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Array.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9705 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Diagonal.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1697 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    11651 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Dot.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    11146 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/GlobalFunctions.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2458 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/NestByValue.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    21847 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/GeneralProduct.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8256 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CwiseTernaryOp.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6170 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/SolverBase.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    29874 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/DenseBase.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5209 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    20883 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14722 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6368 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6123 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/SelfadjointProduct.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    19887 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5017 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    21724 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10571 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9958 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6513 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5882 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/TriangularSolverVector.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5560 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/Parallelizer.h
--rw-rw-r--   0 travis    (2000) travis    (2000)   112678 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14051 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4104 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6906 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    11198 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13743 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    15244 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    20511 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rwxrwxr-x   0 travis    (2000) travis    (2000)    12488 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Assign_MKL.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14873 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/SelfAdjointView.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8901 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/StableNorm.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      988 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/DiagonalProduct.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/NonMPL2.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10643 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/StaticAssert.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14528 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/ForwardDeclarations.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6525 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/IndexedViewHelper.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    11987 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/SymbolicIndex.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    35678 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/XprHelper.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    16738 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/ConfigureVectorization.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    44804 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/Macros.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    45640 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/Memory.h
--rwxrwxr-x   0 travis    (2000) travis    (2000)    24335 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/Meta.h
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4514 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1432 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/ReshapedHelper.h
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4268 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/MKL_support.h
--rwxrwxr-x   0 travis    (2000) travis    (2000)    15726 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/BlasUtil.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    21806 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/Constants.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10895 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/IntegralConstant.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    21700 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/PermutationMatrix.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2765 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Swap.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7942 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CwiseBinaryOp.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/functors/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8020 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/functors/NullaryFunctors.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      607 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/functors/TernaryFunctors.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    34616 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/functors/UnaryFunctors.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    18317 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/functors/BinaryFunctors.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4400 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/functors/StlFunctors.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6686 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    33010 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CwiseNullaryOp.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13060 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Ref.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6397 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Random.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4745 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CoreIterators.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5261 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CwiseUnaryView.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4301 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/BooleanRedux.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5725 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CommaInitializer.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3865 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Stride.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    63323 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CoreEvaluators.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6020 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Select.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    33275 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/VectorwiseOp.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    40319 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/AssignEvaluator.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6775 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/ArrayWrapper.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7434 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/IO.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10337 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/NumTraits.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8321 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/IndexedView.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    24287 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Matrix.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    24220 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/DenseCoeffsBase.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2738 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Assign.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3620 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/NoAlias.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10991 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/MapBase.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    22395 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/DenseStorage.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5631 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Replicate.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    18669 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Redux.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4769 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/ForceAlignedAccess.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3106 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/MathFunctionsImpl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    53259 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/ProductEvaluators.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    48524 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/PlainObjectBase.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5751 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/EigenBase.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13910 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/BandMatrix.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7457 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Reverse.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9154 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/SolveTriangular.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    15268 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Transpose.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8159 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Core/ArrayBase.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/
--rw-rw-r--   0 travis    (2000) travis    (2000)    21078 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/RealSchur.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    33949 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4104 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    23640 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/RealQZ.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9716 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    12559 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3650 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    22538 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5575 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    17176 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    22970 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/EigenSolver.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14339 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    17274 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4178 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SVD/
--rw-rw-r--   0 travis    (2000) travis    (2000)    32993 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SVD/JacobiSVD.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14266 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SVD/SVDBase.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5099 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    15957 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SVD/UpperBidiagonalization.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    53680 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SVD/BDCSVD.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseQR/
--rw-rw-r--   0 travis    (2000) travis    (2000)    29167 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/SparseQR/SparseQR.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/OrderingMethods/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5204 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/OrderingMethods/Ordering.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    62265 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    16105 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/src/OrderingMethods/Amd.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1814 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/SparseLU
--rw-rw-r--   0 travis    (2000) travis    (2000)     2083 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/IterativeLinearSolvers
--rw-rw-r--   0 travis    (2000) travis    (2000)     2243 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/SuperLUSupport
--rw-rw-r--   0 travis    (2000) travis    (2000)      888 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/Sparse
--rw-rw-r--   0 travis    (2000) travis    (2000)      694 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/CMakeLists.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      797 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/StdDeque
--rw-rw-r--   0 travis    (2000) travis    (2000)     1206 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/Cholesky
--rw-rw-r--   0 travis    (2000) travis    (2000)       35 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/Eigen
--rw-rw-r--   0 travis    (2000) travis    (2000)     1162 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/SPQRSupport
--rw-rw-r--   0 travis    (2000) travis    (2000)      939 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/Jacobi
--rw-rw-r--   0 travis    (2000) travis    (2000)     1382 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/UmfPackSupport
--rw-rw-r--   0 travis    (2000) travis    (2000)     1433 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/LU
--rw-rw-r--   0 travis    (2000) travis    (2000)     2240 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/SparseCore
--rw-rw-r--   0 travis    (2000) travis    (2000)     1317 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/QR
--rw-rw-r--   0 travis    (2000) travis    (2000)      874 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/Householder
--rw-rw-r--   0 travis    (2000) travis    (2000)    11621 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/Core
--rw-rw-r--   0 travis    (2000) travis    (2000)      726 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/StdList
--rw-rw-r--   0 travis    (2000) travis    (2000)     1822 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/Eigenvalues
--rw-rw-r--   0 travis    (2000) travis    (2000)     1629 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/SVD
--rw-rw-r--   0 travis    (2000) travis    (2000)      803 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/StdVector
--rw-rw-r--   0 travis    (2000) travis    (2000)     1195 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/SparseQR
--rw-rw-r--   0 travis    (2000) travis    (2000)     2451 2020-02-14 21:06:06.000000 affine_transform-0.2.8/extern/eigen/Eigen/OrderingMethods
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/pybind11/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/pybind11/include/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5655 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6657 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/chrono.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/detail/
--rw-rw-r--   0 travis    (2000) travis    (2000)    37068 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1450 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/detail/typeid.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3566 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    24772 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    16322 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14022 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    66163 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/numpy.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    96604 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8749 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    89522 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/common.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    29043 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4326 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2001 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/complex.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    22528 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/stl_bind.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7731 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2031 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/options.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3599 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3865 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    19063 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14029 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    57794 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/include/pybind11/pytypes.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6507 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/CMakeLists.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/pybind11/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/tools/FindCatch.cmake
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2528 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/tools/check-style.sh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/extern/pybind11/tools/clang/
--rw-rw-r--   0 travis    (2000) travis    (2000)   115943 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/tools/clang/cindex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      172 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/tools/clang/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/tools/clang/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)     1077 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/tools/clang/enumerations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2749 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/tools/clang/LICENSE.TXT
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/tools/clang/.git
--rw-rw-r--   0 travis    (2000) travis    (2000)      565 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/tools/clang/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4153 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/tools/pybind11Config.cmake.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     9582 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/tools/pybind11Tools.cmake
--rw-rw-r--   0 travis    (2000) travis    (2000)     2995 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/tools/FindEigen3.cmake
--rw-rw-r--   0 travis    (2000) travis    (2000)     8336 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/tools/FindPythonLibsNew.cmake
--rwxrwxr-x   0 travis    (2000) travis    (2000)    12534 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/tools/mkdoc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1098 2020-02-14 21:06:07.000000 affine_transform-0.2.8/extern/pybind11/tools/libsize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      656 2020-02-14 21:05:58.000000 affine_transform-0.2.8/CMakeLists.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       94 2020-02-14 21:06:54.000000 affine_transform-0.2.8/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 21:06:54.000000 affine_transform-0.2.8/affine_transform/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6235 2020-02-14 21:05:58.000000 affine_transform-0.2.8/affine_transform/affine_transform.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2020-02-14 21:06:54.000000 affine_transform-0.2.8/affine_transform/version.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2020-02-14 21:05:58.000000 affine_transform-0.2.8/affine_transform/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2020-02-14 21:05:58.000000 affine_transform-0.2.8/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     3308 2020-02-14 21:05:58.000000 affine_transform-0.2.8/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4336 2020-02-14 21:05:58.000000 affine_transform-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.789102 affine_transform-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-22 11:28:58.000000 affine_transform-0.2.9/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-22 11:28:58.000000 affine_transform-0.2.9/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.713103 affine_transform-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.733103 affine_transform-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-22 11:28:58.000000 affine_transform-0.2.9/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-22 11:28:58.000000 affine_transform-0.2.9/.github/workflows/deploy_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-22 11:28:58.000000 affine_transform-0.2.9/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-22 11:28:58.000000 affine_transform-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-22 11:28:58.000000 affine_transform-0.2.9/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-22 11:28:58.000000 affine_transform-0.2.9/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-22 11:28:58.000000 affine_transform-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-22 11:28:58.000000 affine_transform-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-22 11:29:19.789102 affine_transform-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-22 11:28:58.000000 affine_transform-0.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.733103 affine_transform-0.2.9/affine_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-22 11:28:58.000000 affine_transform-0.2.9/affine_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-04-22 11:28:58.000000 affine_transform-0.2.9/affine_transform/affine_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-22 11:29:19.000000 affine_transform-0.2.9/affine_transform/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.733103 affine_transform-0.2.9/affine_transform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-22 11:29:19.000000 affine_transform-0.2.9/affine_transform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18664 2023-04-22 11:29:19.000000 affine_transform-0.2.9/affine_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 11:29:19.000000 affine_transform-0.2.9/affine_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 11:29:19.000000 affine_transform-0.2.9/affine_transform.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-22 11:29:19.000000 affine_transform-0.2.9/affine_transform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-22 11:29:19.000000 affine_transform-0.2.9/affine_transform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 11:28:58.000000 affine_transform-0.2.9/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.733103 affine_transform-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.733103 affine_transform-0.2.9/docs/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/cpp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)   112013 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/cpp/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/cpp_doc.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.737103 affine_transform-0.2.9/docs/cpp_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/cpp_docs/affine_transform.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/cpp_docs/apply_interpolation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/cpp_docs/constant_boundary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/cpp_docs/cubic_interpolation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/cpp_docs/data_struct.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/cpp_docs/extract.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/cpp_docs/interpolation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/cpp_docs/linear_interpolation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/cpp_docs/python_bindings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/cpp_docs/transform.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/cpp_docs/transform_loop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/how_to_use.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/module_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-22 11:28:58.000000 affine_transform-0.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.737103 affine_transform-0.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-22 11:28:58.000000 affine_transform-0.2.9/examples/rotation_and_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.729102 affine_transform-0.2.9/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.717103 affine_transform-0.2.9/extern/eigen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.741103 affine_transform-0.2.9/extern/eigen/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/Cholesky
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/CholmodSupport
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/Core
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/Dense
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/Eigen
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/Eigenvalues
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/Geometry
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/Householder
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/Jacobi
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/KLUSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/LU
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/MetisSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/OrderingMethods
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/PaStiXSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/PardisoSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/QR
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/QtAlignedMalloc
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/SPQRSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/SVD
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/Sparse
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/SparseCholesky
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/SparseCore
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/SparseLU
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/SparseQR
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/StdDeque
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/StdList
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/StdVector
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/SuperLUSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/UmfPackSupport
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.729102 affine_transform-0.2.9/extern/eigen/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.741103 affine_transform-0.2.9/extern/eigen/Eigen/src/Cholesky/
+-rw-r--r--   0 runner    (1001) docker     (123)    24837 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18683 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.741103 affine_transform-0.2.9/extern/eigen/Eigen/src/CholmodSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    25441 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.749102 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)    19214 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16713 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40319 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/AssignEvaluator.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12488 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18400 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    63323 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33010 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29874 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24220 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22395 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21847 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28139 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51671 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24287 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23793 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21700 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48524 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner    (1001) docker     (123)    53259 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14873 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38039 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33275 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9304 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.721103 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.749102 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36713 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.757102 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (123)    19583 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15855 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    54439 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.757102 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42819 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.757102 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/CUDA/Complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.757102 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19102 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/Default/Settings.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.757102 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 runner    (1001) docker     (123)    26865 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/GPU/Half.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16855 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52270 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/GPU/PacketMathHalf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.721103 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/HIP/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.757102 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.757102 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 runner    (1001) docker     (123)    20970 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16159 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.757102 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (123)    19035 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31150 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.757102 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42840 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.757102 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23172 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21856 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.757102 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner    (1001) docker     (123)    20514 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40672 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.761103 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/functors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18317 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34616 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.761103 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/
+-rw-r--r--   0 runner    (1001) docker     (123)   112678 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19887 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21724 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20883 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.765102 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15726 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16738 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21806 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4514 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/IntegralConstant.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4268 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44804 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45640 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/Memory.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24335 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35678 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.765102 affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14339 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33949 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22538 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.769102 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32995 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/RotationBase.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6717 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 runner    (1001) docker     (123)    61854 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.769102 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/arch/Geometry_SSE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.769102 affine_transform-0.2.9/extern/eigen/Eigen/src/Householder/
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23569 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.769102 affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14962 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.769102 affine_transform-0.2.9/extern/eigen/Eigen/src/Jacobi/
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.769102 affine_transform-0.2.9/extern/eigen/Eigen/src/KLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/KLUSupport/KLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.769102 affine_transform-0.2.9/extern/eigen/Eigen/src/LU/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32313 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21856 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.769102 affine_transform-0.2.9/extern/eigen/Eigen/src/LU/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/LU/arch/Inverse_SSE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.769102 affine_transform-0.2.9/extern/eigen/Eigen/src/MetisSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.769102 affine_transform-0.2.9/extern/eigen/Eigen/src/OrderingMethods/
+-rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    62265 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.769102 affine_transform-0.2.9/extern/eigen/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    22249 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.773102 affine_transform-0.2.9/extern/eigen/Eigen/src/PardisoSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    20091 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.773102 affine_transform-0.2.9/extern/eigen/Eigen/src/QR/
+-rw-r--r--   0 runner    (1001) docker     (123)    25498 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23029 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26768 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.773102 affine_transform-0.2.9/extern/eigen/Eigen/src/SPQRSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.773102 affine_transform-0.2.9/extern/eigen/Eigen/src/SVD/
+-rw-r--r--   0 runner    (1001) docker     (123)    53680 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32993 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.773102 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCholesky/
+-rw-r--r--   0 runner    (1001) docker     (123)    24177 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.777102 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/
+-rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23759 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25426 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13256 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57169 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17451 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.777102 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/
+-rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.777102 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseQR/
+-rw-r--r--   0 runner    (1001) docker     (123)    29167 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.777102 affine_transform-0.2.9/extern/eigen/Eigen/src/StlSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.777102 affine_transform-0.2.9/extern/eigen/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    34346 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.781102 affine_transform-0.2.9/extern/eigen/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    24456 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.781102 affine_transform-0.2.9/extern/eigen/Eigen/src/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/misc/Image.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30560 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/misc/blas.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/misc/lapack.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1058369 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.781102 affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19027 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    59005 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-04-22 11:29:06.000000 affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/ReshapedMethods.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.781102 affine_transform-0.2.9/extern/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.729102 affine_transform-0.2.9/extern/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.785102 affine_transform-0.2.9/extern/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    89522 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.785102 affine_transform-0.2.9/extern/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    24772 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37068 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29043 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    66163 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)    96604 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57794 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/pytypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22528 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.785102 affine_transform-0.2.9/extern/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2528 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/tools/check-style.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.785102 affine_transform-0.2.9/extern/pybind11/tools/clang/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/tools/clang/.git
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/tools/clang/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/tools/clang/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/tools/clang/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/tools/clang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115943 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/tools/clang/cindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/tools/clang/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12534 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/tools/mkdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-04-22 11:29:07.000000 affine_transform-0.2.9/extern/pybind11/tools/pybind11Tools.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.729102 affine_transform-0.2.9/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.789102 affine_transform-0.2.9/include/affine_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-04-22 11:28:58.000000 affine_transform-0.2.9/include/affine_transform/affine_transform.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18132 2023-04-22 11:28:58.000000 affine_transform-0.2.9/include/affine_transform/interpolation.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-22 11:28:58.000000 affine_transform-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-22 11:28:58.000000 affine_transform-0.2.9/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-22 11:29:19.789102 affine_transform-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-22 11:28:58.000000 affine_transform-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.789102 affine_transform-0.2.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-22 11:28:58.000000 affine_transform-0.2.9/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:29:19.789102 affine_transform-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-04-22 11:28:58.000000 affine_transform-0.2.9/tests/test_affine_transform.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `affine_transform-0.2.8/docs/conf.py` & `affine_transform-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/docs/cpp_docs/interpolation.rst` & `affine_transform-0.2.9/docs/cpp_docs/interpolation.rst`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/docs/cpp_docs/affine_transform.rst` & `affine_transform-0.2.9/docs/cpp_docs/affine_transform.rst`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/docs/cpp/Doxyfile` & `affine_transform-0.2.9/docs/cpp/Doxyfile`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/docs/cpp_doc.rst` & `affine_transform-0.2.9/docs/cpp_doc.rst`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/docs/make.bat` & `affine_transform-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/include/affine_transform/interpolation.hpp` & `affine_transform-0.2.9/include/affine_transform/interpolation.hpp`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/include/affine_transform/affine_transform.hpp` & `affine_transform-0.2.9/include/affine_transform/affine_transform.hpp`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/PKG-INFO` & `affine_transform-0.2.9/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,69 @@
-Metadata-Version: 1.2
-Name: affine_transform
-Version: 0.2.8
-Summary: Easy to use multi-core affine transformations
-Home-page: https://github.com/NOhs/affine_transform_nd
-Author: NOhs, TobelRunner
-License: MIT
-Description: Affine Transformation: C++17, OpenMP, Python
-        ============================================
-        
-        |travis| |appveyor| |codecov| |rtd| |pypi| |python_vers| |GCC| |license| |codacy| |black| |requirements|
-        
-        
-        .. |travis| image:: https://travis-ci.org/NOhs/affine_transform_nd.svg?branch=master
-            :target: https://travis-ci.org/NOhs/affine_transform_nd
-            :alt: Travis Status
-        .. |appveyor| image:: https://ci.appveyor.com/api/projects/status/bh3gsedf83576wus/branch/master?svg=true
-            :target: https://ci.appveyor.com/project/NOhs/affine-transform-nd/branch/master
-            :alt: AppVeyor Status
-        .. |codecov| image:: https://codecov.io/gh/NOhs/affine_transform_nd/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/NOhs/affine_transform_nd
-            :alt: Codecov Status
-        .. |rtd| image:: https://readthedocs.org/projects/affine-transform-nd/badge/?version=latest
-            :target: https://affine-transform-nd.readthedocs.io/en/latest/?badge=latest
-            :alt: ReadTheDocs Status
-        .. |pypi| image:: https://img.shields.io/pypi/v/affine_transform.svg?color=dark%20green
-            :target: https://pypi.org/project/affine_transform
-            :alt: PyPI
-        .. |python_vers| image:: https://img.shields.io/pypi/pyversions/affine_transform   
-            :alt: PyPI - Python Version
-        .. |GCC| image:: https://img.shields.io/badge/GCC-6%20%7C%207%20%7C%208%20%7C%209-blue
-            :alt: Compiler Version
-        .. |license| image:: https://img.shields.io/github/license/NOhs/affine_transform_nd.svg?color=blue
-            :target: https://opensource.org/licenses/MIT
-            :alt: license
-        .. |codacy| image:: https://api.codacy.com/project/badge/Grade/e39c4c5b913d4237b77fa07f679ab521
-            :target: https://www.codacy.com/app/NOhs/affine_transform_nd?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=NOhs/affine_transform_nd&amp;utm_campaign=Badge_Grade
-            :alt: code quality
-        .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :target: https://github.com/ambv/black
-            :alt: code style
-        .. |requirements| image:: https://requires.io/github/NOhs/affine_transform_nd/requirements.svg?branch=master
-             :target: https://requires.io/github/NOhs/affine_transform_nd/requirements/?branch=master
-             :alt: Requirements Status
-        
-        
-        This project explores how C++17 and OpenMP can be combined to write a
-        surprisingly compact implementation of n-dimensional parallel affine
-        transformations which are linked into Python via the ``affine_transform``
-        module.
-        
-        While this project is still under development, the following features
-        are supported:
-        
-        - Linear and cubic (without prefiltering) interpolation
-        - Constant boundaries
-        - Compiling code for arbitrarily dimensional data
-        - Parallelism via OpenMP
-        - Arbitrary shaped output arrays, allowing e.g. to only extract a transformed slice
-        
-        Short example usage
-        -------------------
-        
-        .. code-block:: python
-        
-            import numpy as np
-        
-            from affine_transform import transform
-            from mgen import rotation_from_angle
-        
-            import matplotlib.pyplot as plt
-        
-        
-            # Create a simple white square in an image
-            original = np.zeros((601, 401))
-            original[100:300, 100:300] = 1
-        
-            # Rotate by 22.5° (around the centre of the square (200,200))
-            # and shift +200 in x and +100 in y
-            transformed = transform(
-                original, rotation_from_angle(np.pi / 8), np.array([200, 100]), origin=(200, 200)
-            )
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: C++
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Affine Transformation: C++17, OpenMP, Python
+============================================
+
+|test| |appveyor| |codecov| |rtd| |pypi| |python_vers| |GCC| |license| |codacy| |black|
+
+
+.. |test| image:: https://github.com/NOhs/mgen/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/NOhs/mgen/actions/workflows/test.yml
+    :alt: Test Status
+.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/bh3gsedf83576wus/branch/master?svg=true
+    :target: https://ci.appveyor.com/project/NOhs/affine-transform-nd/branch/master
+    :alt: AppVeyor Status
+.. |codecov| image:: https://codecov.io/gh/NOhs/affine_transform_nd/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/NOhs/affine_transform_nd
+    :alt: Codecov Status
+.. |rtd| image:: https://readthedocs.org/projects/affine-transform-nd/badge/?version=latest
+    :target: https://affine-transform-nd.readthedocs.io/en/latest/?badge=latest
+    :alt: ReadTheDocs Status
+.. |pypi| image:: https://img.shields.io/pypi/v/affine_transform.svg?color=dark%20green
+    :target: https://pypi.org/project/affine_transform
+    :alt: PyPI
+.. |python_vers| image:: https://img.shields.io/pypi/pyversions/affine_transform
+    :alt: PyPI - Python Version
+.. |GCC| image:: https://img.shields.io/badge/GCC-9%20|%2010%20|%2011%20|%2012-blue
+    :alt: Compiler Version
+.. |license| image:: https://img.shields.io/github/license/NOhs/affine_transform_nd.svg?color=blue
+    :target: https://opensource.org/licenses/MIT
+    :alt: license
+.. |codacy| image:: https://api.codacy.com/project/badge/Grade/e39c4c5b913d4237b77fa07f679ab521
+    :target: https://www.codacy.com/app/NOhs/affine_transform_nd?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=NOhs/affine_transform_nd&amp;utm_campaign=Badge_Grade
+    :alt: code quality
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/ambv/black
+    :alt: code style
+
+This project explores how C++17 and OpenMP can be combined to write a
+surprisingly compact implementation of n-dimensional parallel affine
+transformations which are linked into Python via the ``affine_transform``
+module.
+
+While this project is still under development, the following features
+are supported:
+
+- Linear and cubic (without prefiltering) interpolation
+- Constant boundaries
+- Compiling code for arbitrarily dimensional data
+- Parallelism via OpenMP
+- Arbitrary shaped output arrays, allowing e.g. to only extract a transformed slice
+
+Short example usage
+-------------------
+
+.. code-block:: python
+
+    import numpy as np
+
+    from affine_transform import transform
+    from mgen import rotation_from_angle
+
+
+    # Create a simple white square in an image
+    original = np.zeros((601, 401))
+    original[100:300, 100:300] = 1
+
+    # Rotate by 22.5° (around the centre of the square (200,200))
+    # and shift +200 in x and +100 in y
+    transformed = transform(
+        original, rotation_from_angle(np.pi / 8), np.array([200, 100]), origin=(200, 200)
+    )
```

### Comparing `affine_transform-0.2.8/src/main.cpp` & `affine_transform-0.2.9/src/main.cpp`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/affine_transform.egg-info/PKG-INFO` & `affine_transform-0.2.9/affine_transform.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,89 +1,84 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: affine-transform
-Version: 0.2.8
+Version: 0.2.9
 Summary: Easy to use multi-core affine transformations
 Home-page: https://github.com/NOhs/affine_transform_nd
 Author: NOhs, TobelRunner
 License: MIT
-Description: Affine Transformation: C++17, OpenMP, Python
-        ============================================
-        
-        |travis| |appveyor| |codecov| |rtd| |pypi| |python_vers| |GCC| |license| |codacy| |black| |requirements|
-        
-        
-        .. |travis| image:: https://travis-ci.org/NOhs/affine_transform_nd.svg?branch=master
-            :target: https://travis-ci.org/NOhs/affine_transform_nd
-            :alt: Travis Status
-        .. |appveyor| image:: https://ci.appveyor.com/api/projects/status/bh3gsedf83576wus/branch/master?svg=true
-            :target: https://ci.appveyor.com/project/NOhs/affine-transform-nd/branch/master
-            :alt: AppVeyor Status
-        .. |codecov| image:: https://codecov.io/gh/NOhs/affine_transform_nd/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/NOhs/affine_transform_nd
-            :alt: Codecov Status
-        .. |rtd| image:: https://readthedocs.org/projects/affine-transform-nd/badge/?version=latest
-            :target: https://affine-transform-nd.readthedocs.io/en/latest/?badge=latest
-            :alt: ReadTheDocs Status
-        .. |pypi| image:: https://img.shields.io/pypi/v/affine_transform.svg?color=dark%20green
-            :target: https://pypi.org/project/affine_transform
-            :alt: PyPI
-        .. |python_vers| image:: https://img.shields.io/pypi/pyversions/affine_transform   
-            :alt: PyPI - Python Version
-        .. |GCC| image:: https://img.shields.io/badge/GCC-6%20%7C%207%20%7C%208%20%7C%209-blue
-            :alt: Compiler Version
-        .. |license| image:: https://img.shields.io/github/license/NOhs/affine_transform_nd.svg?color=blue
-            :target: https://opensource.org/licenses/MIT
-            :alt: license
-        .. |codacy| image:: https://api.codacy.com/project/badge/Grade/e39c4c5b913d4237b77fa07f679ab521
-            :target: https://www.codacy.com/app/NOhs/affine_transform_nd?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=NOhs/affine_transform_nd&amp;utm_campaign=Badge_Grade
-            :alt: code quality
-        .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :target: https://github.com/ambv/black
-            :alt: code style
-        .. |requirements| image:: https://requires.io/github/NOhs/affine_transform_nd/requirements.svg?branch=master
-             :target: https://requires.io/github/NOhs/affine_transform_nd/requirements/?branch=master
-             :alt: Requirements Status
-        
-        
-        This project explores how C++17 and OpenMP can be combined to write a
-        surprisingly compact implementation of n-dimensional parallel affine
-        transformations which are linked into Python via the ``affine_transform``
-        module.
-        
-        While this project is still under development, the following features
-        are supported:
-        
-        - Linear and cubic (without prefiltering) interpolation
-        - Constant boundaries
-        - Compiling code for arbitrarily dimensional data
-        - Parallelism via OpenMP
-        - Arbitrary shaped output arrays, allowing e.g. to only extract a transformed slice
-        
-        Short example usage
-        -------------------
-        
-        .. code-block:: python
-        
-            import numpy as np
-        
-            from affine_transform import transform
-            from mgen import rotation_from_angle
-        
-            import matplotlib.pyplot as plt
-        
-        
-            # Create a simple white square in an image
-            original = np.zeros((601, 401))
-            original[100:300, 100:300] = 1
-        
-            # Rotate by 22.5° (around the centre of the square (200,200))
-            # and shift +200 in x and +100 in y
-            transformed = transform(
-                original, rotation_from_angle(np.pi / 8), np.array([200, 100]), origin=(200, 200)
-            )
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.8
+License-File: LICENSE
+
+Affine Transformation: C++17, OpenMP, Python
+============================================
+
+|test| |appveyor| |codecov| |rtd| |pypi| |python_vers| |GCC| |license| |codacy| |black|
+
+
+.. |test| image:: https://github.com/NOhs/mgen/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/NOhs/mgen/actions/workflows/test.yml
+    :alt: Test Status
+.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/bh3gsedf83576wus/branch/master?svg=true
+    :target: https://ci.appveyor.com/project/NOhs/affine-transform-nd/branch/master
+    :alt: AppVeyor Status
+.. |codecov| image:: https://codecov.io/gh/NOhs/affine_transform_nd/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/NOhs/affine_transform_nd
+    :alt: Codecov Status
+.. |rtd| image:: https://readthedocs.org/projects/affine-transform-nd/badge/?version=latest
+    :target: https://affine-transform-nd.readthedocs.io/en/latest/?badge=latest
+    :alt: ReadTheDocs Status
+.. |pypi| image:: https://img.shields.io/pypi/v/affine_transform.svg?color=dark%20green
+    :target: https://pypi.org/project/affine_transform
+    :alt: PyPI
+.. |python_vers| image:: https://img.shields.io/pypi/pyversions/affine_transform
+    :alt: PyPI - Python Version
+.. |GCC| image:: https://img.shields.io/badge/GCC-9%20|%2010%20|%2011%20|%2012-blue
+    :alt: Compiler Version
+.. |license| image:: https://img.shields.io/github/license/NOhs/affine_transform_nd.svg?color=blue
+    :target: https://opensource.org/licenses/MIT
+    :alt: license
+.. |codacy| image:: https://api.codacy.com/project/badge/Grade/e39c4c5b913d4237b77fa07f679ab521
+    :target: https://www.codacy.com/app/NOhs/affine_transform_nd?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=NOhs/affine_transform_nd&amp;utm_campaign=Badge_Grade
+    :alt: code quality
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/ambv/black
+    :alt: code style
+
+This project explores how C++17 and OpenMP can be combined to write a
+surprisingly compact implementation of n-dimensional parallel affine
+transformations which are linked into Python via the ``affine_transform``
+module.
+
+While this project is still under development, the following features
+are supported:
+
+- Linear and cubic (without prefiltering) interpolation
+- Constant boundaries
+- Compiling code for arbitrarily dimensional data
+- Parallelism via OpenMP
+- Arbitrary shaped output arrays, allowing e.g. to only extract a transformed slice
+
+Short example usage
+-------------------
+
+.. code-block:: python
+
+    import numpy as np
+
+    from affine_transform import transform
+    from mgen import rotation_from_angle
+
+
+    # Create a simple white square in an image
+    original = np.zeros((601, 401))
+    original[100:300, 100:300] = 1
+
+    # Rotate by 22.5° (around the centre of the square (200,200))
+    # and shift +200 in x and +100 in y
+    transformed = transform(
+        original, rotation_from_angle(np.pi / 8), np.array([200, 100]), origin=(200, 200)
+    )
```

### Comparing `affine_transform-0.2.8/affine_transform.egg-info/SOURCES.txt` & `affine_transform-0.2.9/affine_transform.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,23 @@
+.appveyor.yml
+.clang-format
+.gitignore
+.gitmodules
 CMakeLists.txt
 LICENSE
 MANIFEST.in
 README.rst
+codecov.yml
+pyproject.toml
+readthedocs.yml
 setup.cfg
 setup.py
+.github/workflows/deploy.yml
+.github/workflows/deploy_test.yml
+.github/workflows/test-package.yml
 affine_transform/__init__.py
 affine_transform/affine_transform.py
 affine_transform/version.txt
 affine_transform.egg-info/PKG-INFO
 affine_transform.egg-info/SOURCES.txt
 affine_transform.egg-info/dependency_links.txt
 affine_transform.egg-info/not-zip-safe
@@ -29,14 +39,15 @@
 docs/cpp_docs/data_struct.rst
 docs/cpp_docs/extract.rst
 docs/cpp_docs/interpolation.rst
 docs/cpp_docs/linear_interpolation.rst
 docs/cpp_docs/python_bindings.rst
 docs/cpp_docs/transform.rst
 docs/cpp_docs/transform_loop.rst
+examples/rotation_and_translation.py
 extern/eigen/Eigen/CMakeLists.txt
 extern/eigen/Eigen/Cholesky
 extern/eigen/Eigen/CholmodSupport
 extern/eigen/Eigen/Core
 extern/eigen/Eigen/Dense
 extern/eigen/Eigen/Eigen
 extern/eigen/Eigen/Eigenvalues
@@ -399,8 +410,9 @@
 extern/pybind11/tools/clang/LICENSE.TXT
 extern/pybind11/tools/clang/README.md
 extern/pybind11/tools/clang/__init__.py
 extern/pybind11/tools/clang/cindex.py
 extern/pybind11/tools/clang/enumerations.py
 include/affine_transform/affine_transform.hpp
 include/affine_transform/interpolation.hpp
-src/main.cpp
+src/main.cpp
+tests/test_affine_transform.py
```

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/KLUSupport` & `affine_transform-0.2.9/extern/eigen/Eigen/KLUSupport`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/PaStiXSupport` & `affine_transform-0.2.9/extern/eigen/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/SparseCholesky` & `affine_transform-0.2.9/extern/eigen/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/Geometry` & `affine_transform-0.2.9/extern/eigen/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/PardisoSupport` & `affine_transform-0.2.9/extern/eigen/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/CholmodSupport` & `affine_transform-0.2.9/extern/eigen/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/MetisSupport` & `affine_transform-0.2.9/extern/eigen/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/QtAlignedMalloc` & `affine_transform-0.2.9/extern/eigen/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/KLUSupport/KLUSupport.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/KLUSupport/KLUSupport.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Hyperplane.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Translation.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/arch/Geometry_SSE.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/arch/Geometry_SSE.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/AngleAxis.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Umeyama.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/EulerAngles.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Transform.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/RotationBase.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Quaternion.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Scaling.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/ParametrizedLine.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/OrthoMethods.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Rotation2D.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/AlignedBox.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Geometry/Homogeneous.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/PardisoSupport/PardisoSupport.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/StlSupport/details.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/StlSupport/StdVector.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/StlSupport/StdList.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/StlSupport/StdDeque.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/CholmodSupport/CholmodSupport.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/MetisSupport/MetisSupport.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_Memory.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_Utils.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLUImpl.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseLU/SparseLU_Structs.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/BlockMethods.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/ReshapedMethods.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/plugins/IndexedViewMethods.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/misc/Image.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/misc/RealSvd2x2.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/misc/blas.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/misc/lapack.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/misc/Kernel.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/misc/lapacke.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Cholesky/LDLT.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Cholesky/LLT.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Jacobi/Jacobi.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/LU/Determinant.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/LU/arch/Inverse_SSE.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/LU/arch/Inverse_SSE.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/LU/PartialPivLU.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/LU/InverseImpl.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/LU/FullPivLU.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseRef.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseTriangularView.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseTranspose.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/TriangularSolver.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseMatrix.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseVector.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseUtil.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseColEtree.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseCompressedBase.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseProduct.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseView.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseAssign.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseFuzzy.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseDenseProduct.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseDot.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseBlock.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparsePermutation.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/CompressedStorage.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseRedux.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/AmbiVector.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseMatrixBase.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseSolverBase.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseCore/SparseMap.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/QR/FullPivHouseholderQR.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/QR/ColPivHouseholderQR.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/QR/HouseholderQR.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Householder/HouseholderSequence.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Householder/Householder.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Householder/BlockHouseholder.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Reshaped.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/MathFunctions.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Fuzzy.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/ArithmeticSequence.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/GenericPacketMath.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/DiagonalMatrix.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/TriangularMatrix.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/PartialReduxEvaluator.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/VectorBlock.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Visitor.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Block.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Inverse.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/MatrixBase.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/GPU/PacketMath.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/GPU/Half.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/GPU/Half.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/GPU/PacketMathHalf.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/GPU/PacketMathHalf.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/ZVector/Complex.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX/PacketMath.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX/Complex.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AltiVec/Complex.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/MSA/PacketMath.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/MSA/Complex.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/CUDA/Complex.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/Default/ConjHelper.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/Default/Settings.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/NEON/PacketMath.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/NEON/Complex.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SSE/PacketMath.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/SSE/Complex.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/AVX512/Complex.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Product.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Map.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Transpositions.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/ReturnByValue.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CwiseUnaryOp.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/StlIterators.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/ConditionEstimator.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Solve.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Array.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Diagonal.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Dot.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/GlobalFunctions.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/NestByValue.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/GeneralProduct.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CwiseTernaryOp.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/SolverBase.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/DenseBase.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/TriangularMatrixVector.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/SelfadjointProduct.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/GeneralMatrixVector.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/TriangularSolverVector.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/Parallelizer.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Assign_MKL.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/SelfAdjointView.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/StableNorm.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/DiagonalProduct.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/StaticAssert.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/ForwardDeclarations.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/IndexedViewHelper.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/SymbolicIndex.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/XprHelper.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/ConfigureVectorization.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/Macros.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/Memory.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/Meta.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/DisableStupidWarnings.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/ReshapedHelper.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/MKL_support.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/BlasUtil.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/Constants.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/util/IntegralConstant.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/PermutationMatrix.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Swap.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CwiseBinaryOp.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/functors/NullaryFunctors.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/functors/TernaryFunctors.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/functors/UnaryFunctors.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/functors/BinaryFunctors.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/functors/StlFunctors.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/functors/AssignmentFunctors.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CwiseNullaryOp.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Ref.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Random.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CoreIterators.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CwiseUnaryView.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/BooleanRedux.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CommaInitializer.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Stride.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/CoreEvaluators.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Select.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/VectorwiseOp.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/AssignEvaluator.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/ArrayWrapper.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/IO.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/NumTraits.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/IndexedView.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Matrix.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/DenseCoeffsBase.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Assign.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/NoAlias.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/MapBase.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/DenseStorage.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Replicate.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Redux.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/ForceAlignedAccess.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/MathFunctionsImpl.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/ProductEvaluators.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/PlainObjectBase.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/EigenBase.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/BandMatrix.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Reverse.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/SolveTriangular.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/Transpose.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Core/ArrayBase.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/RealSchur.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/RealQZ.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/EigenSolver.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/ComplexSchur.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SVD/JacobiSVD.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SVD/SVDBase.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SVD/UpperBidiagonalization.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SVD/BDCSVD.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/SparseQR/SparseQR.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/OrderingMethods/Ordering.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/src/OrderingMethods/Amd.h` & `affine_transform-0.2.9/extern/eigen/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/SparseLU` & `affine_transform-0.2.9/extern/eigen/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/IterativeLinearSolvers` & `affine_transform-0.2.9/extern/eigen/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/SuperLUSupport` & `affine_transform-0.2.9/extern/eigen/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/Sparse` & `affine_transform-0.2.9/extern/eigen/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/CMakeLists.txt` & `affine_transform-0.2.9/extern/eigen/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/StdDeque` & `affine_transform-0.2.9/extern/eigen/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/Cholesky` & `affine_transform-0.2.9/extern/eigen/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/SPQRSupport` & `affine_transform-0.2.9/extern/eigen/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/Jacobi` & `affine_transform-0.2.9/extern/eigen/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/UmfPackSupport` & `affine_transform-0.2.9/extern/eigen/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/LU` & `affine_transform-0.2.9/extern/eigen/Eigen/LU`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/SparseCore` & `affine_transform-0.2.9/extern/eigen/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/QR` & `affine_transform-0.2.9/extern/eigen/Eigen/QR`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/Householder` & `affine_transform-0.2.9/extern/eigen/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/Core` & `affine_transform-0.2.9/extern/eigen/Eigen/Core`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/StdList` & `affine_transform-0.2.9/extern/eigen/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/Eigenvalues` & `affine_transform-0.2.9/extern/eigen/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/SVD` & `affine_transform-0.2.9/extern/eigen/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/StdVector` & `affine_transform-0.2.9/extern/eigen/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/SparseQR` & `affine_transform-0.2.9/extern/eigen/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/eigen/Eigen/OrderingMethods` & `affine_transform-0.2.9/extern/eigen/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/iostream.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/chrono.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/detail/common.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/detail/typeid.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/detail/descr.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/detail/class.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/detail/init.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/detail/internals.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/numpy.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/pybind11.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/operators.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/cast.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/eigen.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/buffer_info.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/complex.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/stl_bind.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/embed.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/options.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/functional.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/eval.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/attr.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/stl.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/include/pybind11/pytypes.h` & `affine_transform-0.2.9/extern/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/CMakeLists.txt` & `affine_transform-0.2.9/extern/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/tools/FindCatch.cmake` & `affine_transform-0.2.9/extern/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/tools/check-style.sh` & `affine_transform-0.2.9/extern/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/tools/clang/cindex.py` & `affine_transform-0.2.9/extern/pybind11/tools/clang/cindex.py`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/tools/clang/enumerations.py` & `affine_transform-0.2.9/extern/pybind11/tools/clang/enumerations.py`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/tools/clang/LICENSE.TXT` & `affine_transform-0.2.9/extern/pybind11/tools/clang/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/tools/clang/__init__.py` & `affine_transform-0.2.9/extern/pybind11/tools/clang/__init__.py`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/tools/pybind11Config.cmake.in` & `affine_transform-0.2.9/extern/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/tools/pybind11Tools.cmake` & `affine_transform-0.2.9/extern/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/tools/FindEigen3.cmake` & `affine_transform-0.2.9/extern/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/tools/FindPythonLibsNew.cmake` & `affine_transform-0.2.9/extern/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/tools/mkdoc.py` & `affine_transform-0.2.9/extern/pybind11/tools/mkdoc.py`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/extern/pybind11/tools/libsize.py` & `affine_transform-0.2.9/extern/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/CMakeLists.txt` & `affine_transform-0.2.9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/affine_transform/affine_transform.py` & `affine_transform-0.2.9/affine_transform/affine_transform.py`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/LICENSE` & `affine_transform-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `affine_transform-0.2.8/setup.py` & `affine_transform-0.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,39 +72,35 @@
         )
 
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
-from subprocess import check_output, CalledProcessError
+from setuptools_scm import get_version
+from datetime import datetime
 
 try:
     # If in git repository, get git label
-    v = (
-        check_output(
-            ["git", "describe", "--always", "--dirty", "--tags"], cwd=this_directory
-        )
-        .decode("utf-8")
-        .strip()
-    )
-    if not "." in v:
-        v = "0.0.0"
+    v = get_version(root='.', relative_to=__file__)
+
+    if "+" in v:
+        v = v.split("+")[0] + datetime.today().strftime("%Y%m%d%H%M%S")
 
     with open(
         os.path.join(
             os.path.abspath(os.path.dirname(__file__)),
             "affine_transform",
             "version.txt",
         ),
         "w",
         encoding="utf-8",
     ) as f:
         f.write(v)
-except CalledProcessError:
+except LookupError:
     # Otherwise get version from version.txt (sdist for example)
     with open(
         os.path.join(
             os.path.abspath(os.path.dirname(__file__)),
             "affine_transform",
             "version.txt",
         ),
@@ -114,25 +110,26 @@
 
 setup(
     name="affine_transform",
     author="NOhs, TobelRunner",
     version=v,
     url="https://github.com/NOhs/affine_transform_nd",
     description="Easy to use multi-core affine transformations",
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     long_description=long_description,
     license="MIT",
     ext_modules=[CMakeExtension("affine_transform")],
     package_data={"affine_transform": ["version.txt"]},
     classifiers=[
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: C++",
         "License :: OSI Approved :: MIT License",
     ],
     packages=find_packages(),
     cmdclass=dict(build_ext=CMakeBuild),
     zip_safe=False,
-    install_requires=["numpy"],
-    setup_requires=["pytest-runner"],
+    install_requires=["numpy", "mgen", "setuptools_scm"],
+    setup_requires=["pytest-runner", "setuptools_scm"],
     tests_require=["numpy", "mgen", "pytest"],
 )
```

