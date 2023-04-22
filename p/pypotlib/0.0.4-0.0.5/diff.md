# Comparing `tmp/pypotlib-0.0.4.tar.gz` & `tmp/pypotlib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypotlib-0.0.4.tar", last modified: Sat Apr 22 03:31:36 2023, max compression
+gzip compressed data, was "pypotlib-0.0.5.tar", last modified: Sat Apr 22 21:21:51 2023, max compression
```

## Comparing `pypotlib-0.0.4.tar` & `pypotlib-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,24 @@
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 pypotlib-0.0.4/.clang-format
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 pypotlib-0.0.4/.github/workflows/build_test.yml
--rw-r--r--   0        0        0     2463 1970-01-01 00:00:00.000000 pypotlib-0.0.4/.github/workflows/build_wheels.yml
--rw-r--r--   0        0        0     5219 1970-01-01 00:00:00.000000 pypotlib-0.0.4/.gitignore
--rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 pypotlib-0.0.4/LICENSE
--rw-r--r--   0        0        0       76 1970-01-01 00:00:00.000000 pypotlib-0.0.4/README.md
--rw-r--r--   0        0        0      223 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/CuH2/py_cuh2pot.cc
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/CuH2/py_cuh2pot.hpp
--rw-r--r--   0        0        0      211 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/LennardJones/py_ljpot.cc
--rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/LennardJones/py_ljpot.hpp
--rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/py_potential.cc
--rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/py_potential.hpp
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/py_pottypes.cc
--rw-r--r--   0        0        0      155 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/py_wrapper.cc
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/py_wrapper.hpp
--rw-r--r--   0        0        0      326 1970-01-01 00:00:00.000000 pypotlib-0.0.4/environment.yml
--rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 pypotlib-0.0.4/meson.build
--rw-r--r--   0        0        0     1061 1970-01-01 00:00:00.000000 pypotlib-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      112 1970-01-01 00:00:00.000000 pypotlib-0.0.4/subprojects/potlib.wrap
--rw-r--r--   0        0        0      301 1970-01-01 00:00:00.000000 pypotlib-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 pypotlib-0.0.5/.clang-format
+-rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 pypotlib-0.0.5/.github/workflows/build_test.yml
+-rw-r--r--   0        0        0     2486 1970-01-01 00:00:00.000000 pypotlib-0.0.5/.github/workflows/build_wheels.yml
+-rw-r--r--   0        0        0     5219 1970-01-01 00:00:00.000000 pypotlib-0.0.5/.gitignore
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 pypotlib-0.0.5/CODEOWNERS
+-rw-r--r--   0        0        0     5488 1970-01-01 00:00:00.000000 pypotlib-0.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 pypotlib-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 pypotlib-0.0.5/README.md
+-rw-r--r--   0        0        0      326 1970-01-01 00:00:00.000000 pypotlib-0.0.5/environment.yml
+-rw-r--r--   0        0        0     1785 1970-01-01 00:00:00.000000 pypotlib-0.0.5/meson.build
+-rw-r--r--   0        0        0      223 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/CuH2/py_cuh2pot.cc
+-rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/CuH2/py_cuh2pot.hpp
+-rw-r--r--   0        0        0      211 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/LennardJones/py_ljpot.cc
+-rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/LennardJones/py_ljpot.hpp
+-rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/py_potential.cc
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/py_potential.hpp
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/py_pottypes.cc
+-rw-r--r--   0        0        0      151 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/py_wrapper.cc
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyb11_srcs/py_wrapper.hpp
+-rw-r--r--   0        0        0       26 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pypotlib/__init__.py
+-rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pypotlib/ase_adapters.py
+-rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 pypotlib-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      112 1970-01-01 00:00:00.000000 pypotlib-0.0.5/subprojects/potlib.wrap
+-rw-r--r--   0        0        0     2903 1970-01-01 00:00:00.000000 pypotlib-0.0.5/PKG-INFO
```

### Comparing `pypotlib-0.0.4/.clang-format` & `pypotlib-0.0.5/.clang-format`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.4/.github/workflows/build_wheels.yml` & `pypotlib-0.0.5/.github/workflows/build_wheels.yml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
       fail-fast: false
       matrix:
         # From NumPy
         # Github Actions doesn't support pairing matrix values together, let's improvise
         # https://github.com/github/feedback/discussions/7835#discussioncomment-1769026
         buildplat:
           - [ubuntu-20.04, manylinux_x86_64]
-          - [ubuntu-20.04, musllinux_x86_64]
+          - [ubuntu-20.04, musllinux_x86_64] # No OpenBlas, no test
           - [macos-12, macosx_x86_64]
           # - [windows-2019, win_amd64]
         python: ["cp310", "cp311"]
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `pypotlib-0.0.4/.gitignore` & `pypotlib-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.4/LICENSE` & `pypotlib-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.4/bindings/CuH2/py_cuh2pot.hpp` & `pypotlib-0.0.5/pyb11_srcs/CuH2/py_cuh2pot.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.4/bindings/LennardJones/py_ljpot.hpp` & `pypotlib-0.0.5/pyb11_srcs/LennardJones/py_ljpot.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.4/bindings/py_potential.hpp` & `pypotlib-0.0.5/pyb11_srcs/py_potential.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.4/bindings/py_wrapper.hpp` & `pypotlib-0.0.5/pyb11_srcs/py_wrapper.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.4/meson.build` & `pypotlib-0.0.5/meson.build`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project('pypotlib', 'cpp',
-       version: '0.0.4',
+       version: '0.0.5',
   default_options : ['warning_level=2', 'cpp_std=c++17'])
 # IMPORTANT!! warning_level=3 passes -fimplicit-none
 # Many of the older Fortran codes need implicit typing
 
 host_system = host_machine.system()
 
 # Add C++ compiler options
@@ -34,21 +34,39 @@
 pyb11f_deps = [ python_dep ]
 
 
 _deps += [dependency('python3'),
           dependency('pybind11'),
           declare_dependency(link_args: '-lstdc++') ]
 
+# cpot, for the bindings to potlib
 py.extension_module(
-  'pypotlib',
+  'cpot',
   sources : [
-    'bindings/py_wrapper.cc',
-    'bindings/py_pottypes.cc',
-    'bindings/py_potential.cc',
-    'bindings/LennardJones/py_ljpot.cc',
-    'bindings/CuH2/py_cuh2pot.cc',
+    'pyb11_srcs/py_wrapper.cc',
+    'pyb11_srcs/py_pottypes.cc',
+    'pyb11_srcs/py_potential.cc',
+    'pyb11_srcs/LennardJones/py_ljpot.cc',
+    'pyb11_srcs/CuH2/py_cuh2pot.cc',
   ],
   dependencies: _deps,
   link_with: _linkto,
   cpp_args : _args,
-  install: true
+  install: true,
+  subdir: 'pypotlib/'
+)
+
+# pypotlib, main package
+py.install_sources([
+    'pypotlib/__init__.py',
+  ],
+  pure: false, # install next to compiled extension
+  subdir: 'pypotlib'
+)
+
+# Adapters
+py.install_sources([
+    'pypotlib/ase_adapters.py',
+  ],
+  pure: false,
+  subdir: 'pypotlib'
 )
```

### Comparing `pypotlib-0.0.4/pyproject.toml` & `pypotlib-0.0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tool.pdm]
 
 [project]
 name = "pypotlib"
-version = "0.0.4"
+version = "0.0.5"
 description = "Python bindings and ASE adapters for potlib"
 authors = [
     {name = "Rohit Goswami", email = "rog32@hi.is"},
 ]
-dependencies = []
+# These are only if ase integration is requested, consider a group
+dependencies = [
+    "numpy>=1.24.2",
+    "ase>=3.22.1",
+]
 requires-python = ">=3.10"
 readme = "README.md"
 license = {text = "MIT"}
 
 [build-system]
 requires = ["wheel", "setuptools", "pybind11", "meson-python"]
 build-backend = "mesonpy"
@@ -24,14 +28,13 @@
     pip install meson cmake &&
     meson wrap install pybind11
 """
 test-command = "echo 'installed'"
 # XXX: This shouldn't be empty, --lib-sdir .
 # Normally is auditwheel repair -w {dest_dir} {wheel}
 repair-wheel-command = ""
+# Openblas for musllinux is painful, so don't install / test
+test-skip = "*-musllinux*"
 
 [tool.cibuildwheel.macos]
 environment = { RUNNER_OS="macOS" }
 before-all = "brew install gfortran && brew unlink gfortran && brew link gfortran"
-# [[tool.cibuildwheel.overrides]]
-# select = "*-musllinux*"
-# before-all = "apk add mylib" # hasn't got new enough Eigen versions, uses Apline 3.12
```

