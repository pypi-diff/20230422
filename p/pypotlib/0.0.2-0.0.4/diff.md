# Comparing `tmp/pypotlib-0.0.2.tar.gz` & `tmp/pypotlib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypotlib-0.0.2.tar", last modified: Fri Apr 21 21:11:34 2023, max compression
+gzip compressed data, was "pypotlib-0.0.4.tar", last modified: Sat Apr 22 03:31:36 2023, max compression
```

## Comparing `pypotlib-0.0.2.tar` & `pypotlib-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 pypotlib-0.0.2/.clang-format
--rw-r--r--   0        0        0     5188 1970-01-01 00:00:00.000000 pypotlib-0.0.2/.gitignore
--rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 pypotlib-0.0.2/LICENSE
--rw-r--r--   0        0        0       76 1970-01-01 00:00:00.000000 pypotlib-0.0.2/README.md
--rw-r--r--   0        0        0      223 1970-01-01 00:00:00.000000 pypotlib-0.0.2/bindings/CuH2/py_cuh2pot.cc
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 pypotlib-0.0.2/bindings/CuH2/py_cuh2pot.hpp
--rw-r--r--   0        0        0      211 1970-01-01 00:00:00.000000 pypotlib-0.0.2/bindings/LennardJones/py_ljpot.cc
--rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 pypotlib-0.0.2/bindings/LennardJones/py_ljpot.hpp
--rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 pypotlib-0.0.2/bindings/py_potential.cc
--rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 pypotlib-0.0.2/bindings/py_potential.hpp
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 pypotlib-0.0.2/bindings/py_pottypes.cc
--rw-r--r--   0        0        0      155 1970-01-01 00:00:00.000000 pypotlib-0.0.2/bindings/py_wrapper.cc
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pypotlib-0.0.2/bindings/py_wrapper.hpp
--rw-r--r--   0        0        0     1603 1970-01-01 00:00:00.000000 pypotlib-0.0.2/meson.build
--rw-r--r--   0        0        0      406 1970-01-01 00:00:00.000000 pypotlib-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      112 1970-01-01 00:00:00.000000 pypotlib-0.0.2/subprojects/potlib.wrap
--rw-r--r--   0        0        0      333 1970-01-01 00:00:00.000000 pypotlib-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 pypotlib-0.0.4/.clang-format
+-rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 pypotlib-0.0.4/.github/workflows/build_test.yml
+-rw-r--r--   0        0        0     2463 1970-01-01 00:00:00.000000 pypotlib-0.0.4/.github/workflows/build_wheels.yml
+-rw-r--r--   0        0        0     5219 1970-01-01 00:00:00.000000 pypotlib-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 pypotlib-0.0.4/LICENSE
+-rw-r--r--   0        0        0       76 1970-01-01 00:00:00.000000 pypotlib-0.0.4/README.md
+-rw-r--r--   0        0        0      223 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/CuH2/py_cuh2pot.cc
+-rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/CuH2/py_cuh2pot.hpp
+-rw-r--r--   0        0        0      211 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/LennardJones/py_ljpot.cc
+-rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/LennardJones/py_ljpot.hpp
+-rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/py_potential.cc
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/py_potential.hpp
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/py_pottypes.cc
+-rw-r--r--   0        0        0      155 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/py_wrapper.cc
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pypotlib-0.0.4/bindings/py_wrapper.hpp
+-rw-r--r--   0        0        0      326 1970-01-01 00:00:00.000000 pypotlib-0.0.4/environment.yml
+-rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 pypotlib-0.0.4/meson.build
+-rw-r--r--   0        0        0     1061 1970-01-01 00:00:00.000000 pypotlib-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      112 1970-01-01 00:00:00.000000 pypotlib-0.0.4/subprojects/potlib.wrap
+-rw-r--r--   0        0        0      301 1970-01-01 00:00:00.000000 pypotlib-0.0.4/PKG-INFO
```

### Comparing `pypotlib-0.0.2/.clang-format` & `pypotlib-0.0.4/.clang-format`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.2/.gitignore` & `pypotlib-0.0.4/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Added
-subprojects/potlib/
+subprojects/*
+!subprojects/potlib.wrap
 compile_commands.json
 pdm.lock
+wheelhouse/
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `pypotlib-0.0.2/LICENSE` & `pypotlib-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.2/bindings/CuH2/py_cuh2pot.hpp` & `pypotlib-0.0.4/bindings/CuH2/py_cuh2pot.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.2/bindings/LennardJones/py_ljpot.hpp` & `pypotlib-0.0.4/bindings/LennardJones/py_ljpot.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.2/bindings/py_potential.hpp` & `pypotlib-0.0.4/bindings/py_potential.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.2/bindings/py_wrapper.hpp` & `pypotlib-0.0.4/bindings/py_wrapper.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.2/meson.build` & `pypotlib-0.0.4/meson.build`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 project('pypotlib', 'cpp',
-       version: '0.0.1',
+       version: '0.0.4',
   default_options : ['warning_level=2', 'cpp_std=c++17'])
 # IMPORTANT!! warning_level=3 passes -fimplicit-none
 # Many of the older Fortran codes need implicit typing
 
 host_system = host_machine.system()
 
 # Add C++ compiler options
 cpp_args = ['-Wall', '-Wextra', '-Wpedantic']
 _args = [cpp_args] # Extra arguments
 _deps = [] # Dependencies
 _linkto = [] # All the sub-libraries (potentials)
 
-# Add conditionals
-if host_system == 'darwin'
-  _args += ['-DOSX=TRUE']
-  add_global_arguments(['-faligned-allocation'], language: 'cpp')
-endif
-
 # Languages
 add_languages('c', required: true)
 add_languages('fortran', required: true)
 cc = meson.get_compiler('c')
 cppc = meson.get_compiler('cpp')
 
 # ---------------------- Library Dependencies
```

