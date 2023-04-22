# Comparing `tmp/types-setuptools-67.6.0.8.tar.gz` & `tmp/types-setuptools-67.7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-setuptools-67.6.0.8.tar", last modified: Mon Apr 17 21:12:59 2023, max compression
+gzip compressed data, was "types-setuptools-67.7.0.0.tar", last modified: Sat Apr 22 18:17:48 2023, max compression
```

## Comparing `types-setuptools-67.6.0.8.tar` & `types-setuptools-67.7.0.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:12:59.953957 types-setuptools-67.6.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-04-17 21:12:57.000000 types-setuptools-67.6.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 21:12:57.000000 types-setuptools-67.6.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-17 21:12:59.953957 types-setuptools-67.6.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:12:59.941957 types-setuptools-67.6.0.8/pkg_resources-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 21:12:57.000000 types-setuptools-67.6.0.8/pkg_resources-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/pkg_resources-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 21:12:59.953957 types-setuptools-67.6.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-17 21:12:57.000000 types-setuptools-67.6.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:12:59.945957 types-setuptools-67.6.0.8/setuptools-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 21:12:57.000000 types-setuptools-67.6.0.8/setuptools-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_deprecation_warning.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:12:59.945957 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/cmd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:12:59.949957 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/_distutils/filelist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/build_meta.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:12:59.953957 types-setuptools-67.6.0.8/setuptools-stubs/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/alias.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/develop.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/dist_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/easy_install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/install_egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/rotate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/saveopts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/setopt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/test.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/command/upload_docs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/depends.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/extension.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:12:59.953957 types-setuptools-67.6.0.8/setuptools-stubs/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/extern/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/glob.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/installer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/launch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/monkey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/msvc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/namespaces.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/package_index.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/sandbox.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/unicode_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 21:12:36.000000 types-setuptools-67.6.0.8/setuptools-stubs/windows_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:12:59.953957 types-setuptools-67.6.0.8/types_setuptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-17 21:12:59.000000 types-setuptools-67.6.0.8/types_setuptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-17 21:12:59.000000 types-setuptools-67.6.0.8/types_setuptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 21:12:59.000000 types-setuptools-67.6.0.8/types_setuptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 21:12:59.000000 types-setuptools-67.6.0.8/types_setuptools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:17:48.945968 types-setuptools-67.7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-04-22 18:17:47.000000 types-setuptools-67.7.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-22 18:17:47.000000 types-setuptools-67.7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-22 18:17:48.945968 types-setuptools-67.7.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:17:48.937968 types-setuptools-67.7.0.0/pkg_resources-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-22 18:17:47.000000 types-setuptools-67.7.0.0/pkg_resources-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/pkg_resources-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 18:17:48.945968 types-setuptools-67.7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-22 18:17:47.000000 types-setuptools-67.7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:17:48.941968 types-setuptools-67.7.0.0/setuptools-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-22 18:17:47.000000 types-setuptools-67.7.0.0/setuptools-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:17:48.941968 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/cmd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:17:48.941968 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/_distutils/filelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/build_meta.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:17:48.945968 types-setuptools-67.7.0.0/setuptools-stubs/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/alias.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/develop.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/dist_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/easy_install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/install_egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/rotate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/saveopts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/setopt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/command/upload_docs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/depends.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/extension.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:17:48.945968 types-setuptools-67.7.0.0/setuptools-stubs/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/extern/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/glob.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/installer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/launch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/monkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/msvc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/namespaces.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/package_index.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/sandbox.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/unicode_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/warnings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-22 18:17:34.000000 types-setuptools-67.7.0.0/setuptools-stubs/windows_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:17:48.945968 types-setuptools-67.7.0.0/types_setuptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-22 18:17:48.000000 types-setuptools-67.7.0.0/types_setuptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-22 18:17:48.000000 types-setuptools-67.7.0.0/types_setuptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 18:17:48.000000 types-setuptools-67.7.0.0/types_setuptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-22 18:17:48.000000 types-setuptools-67.7.0.0/types_setuptools.egg-info/top_level.txt
```

### Comparing `types-setuptools-67.6.0.8/CHANGELOG.md` & `types-setuptools-67.7.0.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## 67.7.0.0 (2023-04-22)
+
+setuptools: bump to 67.7 (#10069)
+
+Fixes #10067
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 67.6.0.8 (2023-04-17)
 
 Add missing exception classes in `setuptools.errors` (#10057)
 
 Co-authored-by: AlexWaygood <alex.waygood@gmail.com>
 
 ## 67.6.0.7 (2023-04-04)
```

### Comparing `types-setuptools-67.6.0.8/PKG-INFO` & `types-setuptools-67.7.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 67.6.0.8
+Version: 67.7.0.0
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0b17fafbe3a3a75ae11431ebdee72af5bf751a9c`.
+This package was generated from typeshed commit `cc35f4be3b5c44361290bb88a8e31c58fde5a0e4`.
```

### Comparing `types-setuptools-67.6.0.8/pkg_resources-stubs/__init__.pyi` & `types-setuptools-67.7.0.0/pkg_resources-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setup.py` & `types-setuptools-67.7.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0b17fafbe3a3a75ae11431ebdee72af5bf751a9c`.
+This package was generated from typeshed commit `cc35f4be3b5c44361290bb88a8e31c58fde5a0e4`.
 '''.lstrip()
 
 setup(name=name,
-      version="67.6.0.8",
+      version="67.7.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['setuptools-stubs', 'pkg_resources-stubs'],
-      package_data={'setuptools-stubs': ['__init__.pyi', '_deprecation_warning.pyi', '_distutils/cmd.pyi', '_distutils/command/build_clib.pyi', '_distutils/command/build_ext.pyi', '_distutils/command/build_py.pyi', '_distutils/command/install.pyi', '_distutils/command/install_lib.pyi', '_distutils/command/install_scripts.pyi', '_distutils/command/register.pyi', '_distutils/command/sdist.pyi', '_distutils/command/upload.pyi', '_distutils/config.pyi', '_distutils/dist.pyi', '_distutils/errors.pyi', '_distutils/extension.pyi', '_distutils/filelist.pyi', 'archive_util.pyi', 'build_meta.pyi', 'command/__init__.pyi', 'command/alias.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/develop.pyi', 'command/dist_info.pyi', 'command/easy_install.pyi', 'command/egg_info.pyi', 'command/install.pyi', 'command/install_egg_info.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/rotate.pyi', 'command/saveopts.pyi', 'command/sdist.pyi', 'command/setopt.pyi', 'command/test.pyi', 'command/upload.pyi', 'command/upload_docs.pyi', 'config.pyi', 'dep_util.pyi', 'depends.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'extern/__init__.pyi', 'glob.pyi', 'installer.pyi', 'launch.pyi', 'monkey.pyi', 'msvc.pyi', 'namespaces.pyi', 'package_index.pyi', 'sandbox.pyi', 'unicode_utils.pyi', 'version.pyi', 'wheel.pyi', 'windows_support.pyi', 'METADATA.toml'], 'pkg_resources-stubs': ['__init__.pyi', 'METADATA.toml']},
+      package_data={'setuptools-stubs': ['__init__.pyi', '_distutils/cmd.pyi', '_distutils/command/build_clib.pyi', '_distutils/command/build_ext.pyi', '_distutils/command/build_py.pyi', '_distutils/command/install.pyi', '_distutils/command/install_lib.pyi', '_distutils/command/install_scripts.pyi', '_distutils/command/register.pyi', '_distutils/command/sdist.pyi', '_distutils/command/upload.pyi', '_distutils/config.pyi', '_distutils/dist.pyi', '_distutils/errors.pyi', '_distutils/extension.pyi', '_distutils/filelist.pyi', 'archive_util.pyi', 'build_meta.pyi', 'command/__init__.pyi', 'command/alias.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/develop.pyi', 'command/dist_info.pyi', 'command/easy_install.pyi', 'command/egg_info.pyi', 'command/install.pyi', 'command/install_egg_info.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/rotate.pyi', 'command/saveopts.pyi', 'command/sdist.pyi', 'command/setopt.pyi', 'command/test.pyi', 'command/upload.pyi', 'command/upload_docs.pyi', 'config.pyi', 'dep_util.pyi', 'depends.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'extern/__init__.pyi', 'glob.pyi', 'installer.pyi', 'launch.pyi', 'monkey.pyi', 'msvc.pyi', 'namespaces.pyi', 'package_index.pyi', 'sandbox.pyi', 'unicode_utils.pyi', 'version.pyi', 'warnings.pyi', 'wheel.pyi', 'windows_support.pyi', 'METADATA.toml'], 'pkg_resources-stubs': ['__init__.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/__init__.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import abstractmethod
 from collections.abc import Iterable, Mapping, Sequence
 from typing import Any
 
-from setuptools._deprecation_warning import SetuptoolsDeprecationWarning as SetuptoolsDeprecationWarning
 from setuptools.depends import Require as Require
 from setuptools.dist import Distribution as Distribution
 from setuptools.extension import Extension as Extension
+from setuptools.warnings import SetuptoolsDeprecationWarning as SetuptoolsDeprecationWarning
 
 from ._distutils.cmd import Command as _Command
 
 __version__: str
 
 class PackageFinder:
     @classmethod
```

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/_distutils/cmd.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/_distutils/cmd.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/build_clib.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/build_clib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/build_ext.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/build_py.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/install.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/install_lib.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/install_lib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/register.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/register.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/_distutils/command/sdist.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/_distutils/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/_distutils/dist.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/_distutils/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/_distutils/errors.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/_distutils/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/_distutils/extension.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/_distutils/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/_distutils/filelist.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/_distutils/filelist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/archive_util.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/archive_util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/build_meta.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/build_meta.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/command/build_ext.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/command/build_py.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/command/develop.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/command/develop.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/command/easy_install.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/command/easy_install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/command/egg_info.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/command/egg_info.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/command/sdist.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/command/setopt.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/command/setopt.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/command/test.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/command/test.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/command/upload_docs.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/command/upload_docs.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/depends.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/depends.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/dist.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/errors.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/extension.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/extern/__init__.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/extern/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/msvc.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/msvc.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/package_index.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/package_index.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/setuptools-stubs/sandbox.pyi` & `types-setuptools-67.7.0.0/setuptools-stubs/sandbox.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.6.0.8/types_setuptools.egg-info/PKG-INFO` & `types-setuptools-67.7.0.0/types_setuptools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 67.6.0.8
+Version: 67.7.0.0
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0b17fafbe3a3a75ae11431ebdee72af5bf751a9c`.
+This package was generated from typeshed commit `cc35f4be3b5c44361290bb88a8e31c58fde5a0e4`.
```

### Comparing `types-setuptools-67.6.0.8/types_setuptools.egg-info/SOURCES.txt` & `types-setuptools-67.7.0.0/types_setuptools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 CHANGELOG.md
 MANIFEST.in
 setup.py
 pkg_resources-stubs/METADATA.toml
 pkg_resources-stubs/__init__.pyi
 setuptools-stubs/METADATA.toml
 setuptools-stubs/__init__.pyi
-setuptools-stubs/_deprecation_warning.pyi
 setuptools-stubs/archive_util.pyi
 setuptools-stubs/build_meta.pyi
 setuptools-stubs/config.pyi
 setuptools-stubs/dep_util.pyi
 setuptools-stubs/depends.pyi
 setuptools-stubs/dist.pyi
 setuptools-stubs/errors.pyi
@@ -20,14 +19,15 @@
 setuptools-stubs/monkey.pyi
 setuptools-stubs/msvc.pyi
 setuptools-stubs/namespaces.pyi
 setuptools-stubs/package_index.pyi
 setuptools-stubs/sandbox.pyi
 setuptools-stubs/unicode_utils.pyi
 setuptools-stubs/version.pyi
+setuptools-stubs/warnings.pyi
 setuptools-stubs/wheel.pyi
 setuptools-stubs/windows_support.pyi
 setuptools-stubs/_distutils/cmd.pyi
 setuptools-stubs/_distutils/config.pyi
 setuptools-stubs/_distutils/dist.pyi
 setuptools-stubs/_distutils/errors.pyi
 setuptools-stubs/_distutils/extension.pyi
```

