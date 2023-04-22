# Comparing `tmp/pCrunch-0.1.1.tar.gz` & `tmp/pCrunch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pCrunch-0.1.1.tar", last modified: Thu Aug 20 21:08:17 2020, max compression
+gzip compressed data, was "pCrunch-1.0.1.tar", last modified: Sat Apr 22 19:20:11 2023, max compression
```

## Comparing `pCrunch-0.1.1.tar` & `pCrunch-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,35 @@
-drwxr-xr-x   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)        0 2020-08-20 21:08:17.000000 pCrunch-0.1.1/
--rw-r--r--   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)     3468 2020-08-20 21:08:17.000000 pCrunch-0.1.1/PKG-INFO
-drwxr-xr-x   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)        0 2020-08-20 21:08:17.000000 pCrunch-0.1.1/pCrunch/
--rw-r--r--   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)    32313 2020-08-20 20:59:45.000000 pCrunch-0.1.1/pCrunch/Analysis.py
--rw-r--r--   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)     7645 2020-04-27 19:48:49.000000 pCrunch-0.1.1/pCrunch/CaseGen_Control.py
--rw-r--r--   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)    17072 2020-07-14 22:38:56.000000 pCrunch-0.1.1/pCrunch/Processing.py
--rw-r--r--   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)        0 2020-03-25 20:36:32.000000 pCrunch-0.1.1/pCrunch/__init__.py
--rw-r--r--   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)     2905 2020-05-12 18:51:13.000000 pCrunch-0.1.1/pCrunch/pdTools.py
-drwxr-xr-x   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)        0 2020-08-20 21:08:17.000000 pCrunch-0.1.1/pCrunch.egg-info/
--rw-r--r--   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)     3468 2020-08-20 21:08:17.000000 pCrunch-0.1.1/pCrunch.egg-info/PKG-INFO
--rw-r--r--   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)      270 2020-08-20 21:08:17.000000 pCrunch-0.1.1/pCrunch.egg-info/SOURCES.txt
--rw-r--r--   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)        1 2020-08-20 21:08:17.000000 pCrunch-0.1.1/pCrunch.egg-info/dependency_links.txt
--rw-r--r--   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)      132 2020-08-20 21:08:17.000000 pCrunch-0.1.1/pCrunch.egg-info/requires.txt
--rw-r--r--   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)        8 2020-08-20 21:08:17.000000 pCrunch-0.1.1/pCrunch.egg-info/top_level.txt
--rw-r--r--   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)       38 2020-08-20 21:08:17.000000 pCrunch-0.1.1/setup.cfg
--rw-r--r--   0 nabbas   (1976835063) NREL_NT\Domain Users (18434217)     4657 2020-08-20 21:07:42.000000 pCrunch-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:20:11.746086 pCrunch-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-04-22 19:20:01.000000 pCrunch-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-22 19:20:01.000000 pCrunch-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-22 19:20:11.746086 pCrunch-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-22 19:20:01.000000 pCrunch-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:20:11.734086 pCrunch-1.0.1/pCrunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-22 19:20:01.000000 pCrunch-1.0.1/pCrunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-22 19:20:01.000000 pCrunch-1.0.1/pCrunch/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:20:11.734086 pCrunch-1.0.1/pCrunch/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-22 19:20:01.000000 pCrunch-1.0.1/pCrunch/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13131 2023-04-22 19:20:01.000000 pCrunch-1.0.1/pCrunch/io/openfast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-04-22 19:20:01.000000 pCrunch-1.0.1/pCrunch/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:20:11.734086 pCrunch-1.0.1/pCrunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-22 19:20:11.000000 pCrunch-1.0.1/pCrunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-22 19:20:11.000000 pCrunch-1.0.1/pCrunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:20:11.000000 pCrunch-1.0.1/pCrunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-22 19:20:11.000000 pCrunch-1.0.1/pCrunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 19:20:11.000000 pCrunch-1.0.1/pCrunch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    32775 2023-04-22 19:20:01.000000 pCrunch-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 19:20:11.746086 pCrunch-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-22 19:20:01.000000 pCrunch-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:20:11.734086 pCrunch-1.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:20:11.734086 pCrunch-1.0.1/tests/io/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:20:11.746086 pCrunch-1.0.1/tests/io/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   186142 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/AOC_WSt.out
+-rw-r--r--   0 runner    (1001) docker     (123)   130830 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/AOC_WSt.outb
+-rw-r--r--   0 runner    (1001) docker     (123)  1477853 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/DLC2.3_1.out
+-rw-r--r--   0 runner    (1001) docker     (123)  1758122 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/DLC2.3_2.out
+-rw-r--r--   0 runner    (1001) docker     (123)  1758122 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/DLC2.3_3.out
+-rw-r--r--   0 runner    (1001) docker     (123)  1347618 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/Test1.outb
+-rw-r--r--   0 runner    (1001) docker     (123)  1347618 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/Test2.outb
+-rw-r--r--   0 runner    (1001) docker     (123)  1347618 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/Test3.outb
+-rw-r--r--   0 runner    (1001) docker     (123)  1204577 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/step_0.outb
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/test_direct_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/test_parsers.py
```

