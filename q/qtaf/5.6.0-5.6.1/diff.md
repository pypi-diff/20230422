# Comparing `tmp/qtaf-5.6.0.tar.gz` & `tmp/qtaf-5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtaf-5.6.0.tar", last modified: Thu Apr 20 01:20:36 2023, max compression
+gzip compressed data, was "qtaf-5.6.1.tar", last modified: Sat Apr 22 12:16:41 2023, max compression
```

## Comparing `qtaf-5.6.0.tar` & `qtaf-5.6.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:20:36.331433 qtaf-5.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-20 01:20:26.000000 qtaf-5.6.0/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 01:20:26.000000 qtaf-5.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-20 01:20:36.331433 qtaf-5.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-20 01:20:26.000000 qtaf-5.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-20 01:20:26.000000 qtaf-5.6.0/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:20:36.323433 qtaf-5.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 01:20:26.000000 qtaf-5.6.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-20 01:20:26.000000 qtaf-5.6.0/qta-manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:20:36.323433 qtaf-5.6.0/qta_statics/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-20 01:20:26.000000 qtaf-5.6.0/qta_statics/TestReport.xsl
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-20 01:20:26.000000 qtaf-5.6.0/qta_statics/TestResult.xsl
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 01:20:26.000000 qtaf-5.6.0/qta_statics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1968182 2023-04-20 01:20:26.000000 qtaf-5.6.0/qta_statics/qta-report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:20:36.327433 qtaf-5.6.0/qtaf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-20 01:20:36.000000 qtaf-5.6.0/qtaf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-20 01:20:36.000000 qtaf-5.6.0/qtaf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 01:20:36.000000 qtaf-5.6.0/qtaf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 01:20:36.000000 qtaf-5.6.0/qtaf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 01:20:36.000000 qtaf-5.6.0/qtaf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 01:20:36.000000 qtaf-5.6.0/qtaf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-20 01:20:26.000000 qtaf-5.6.0/qtaf_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 01:20:26.000000 qtaf-5.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 01:20:36.331433 qtaf-5.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-20 01:20:26.000000 qtaf-5.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:20:36.327433 qtaf-5.6.0/testbase/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27250 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/datadrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/exlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    33826 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    35361 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    24595 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45863 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)    29712 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/testresult.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/testsuite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26680 2023-04-20 01:20:26.000000 qtaf-5.6.0/testbase/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 01:20:36.000000 qtaf-5.6.0/testbase/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 01:20:36.331433 qtaf-5.6.0/tuia/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/_tif.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/accessible.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/filedialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/gfcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/qpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/qpathparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/remoteprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/uiacontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/webcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/wincontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-20 01:20:26.000000 qtaf-5.6.0/tuia/wintypes.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 01:20:35.000000 qtaf-5.6.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:16:41.808263 qtaf-5.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-22 12:16:25.000000 qtaf-5.6.1/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-22 12:16:25.000000 qtaf-5.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-22 12:16:41.808263 qtaf-5.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-22 12:16:25.000000 qtaf-5.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-22 12:16:25.000000 qtaf-5.6.1/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:16:41.800263 qtaf-5.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-22 12:16:25.000000 qtaf-5.6.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-22 12:16:25.000000 qtaf-5.6.1/qta-manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:16:41.800263 qtaf-5.6.1/qta_statics/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-22 12:16:25.000000 qtaf-5.6.1/qta_statics/TestReport.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-22 12:16:25.000000 qtaf-5.6.1/qta_statics/TestResult.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:16:25.000000 qtaf-5.6.1/qta_statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1968182 2023-04-22 12:16:25.000000 qtaf-5.6.1/qta_statics/qta-report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:16:41.804263 qtaf-5.6.1/qtaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-22 12:16:41.000000 qtaf-5.6.1/qtaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-22 12:16:41.000000 qtaf-5.6.1/qtaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 12:16:41.000000 qtaf-5.6.1/qtaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-22 12:16:41.000000 qtaf-5.6.1/qtaf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 12:16:41.000000 qtaf-5.6.1/qtaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-22 12:16:41.000000 qtaf-5.6.1/qtaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-22 12:16:25.000000 qtaf-5.6.1/qtaf_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-22 12:16:25.000000 qtaf-5.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 12:16:41.808263 qtaf-5.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-22 12:16:25.000000 qtaf-5.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:16:41.808263 qtaf-5.6.1/testbase/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27250 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/datadrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/exlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33826 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35361 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24595 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45863 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29712 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/testresult.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/testsuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26680 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 12:16:41.000000 qtaf-5.6.1/testbase/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:16:41.808263 qtaf-5.6.1/tuia/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/_tif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/accessible.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/filedialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/gfcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/qpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/qpathparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/remoteprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/uiacontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/webcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/wincontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/wintypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-22 12:16:39.000000 qtaf-5.6.1/version.txt
```

### Comparing `qtaf-5.6.0/LICENSE.TXT` & `qtaf-5.6.1/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/PKG-INFO` & `qtaf-5.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtaf
-Version: 5.6.0
+Version: 5.6.1
 Summary: Basic test automation framework for QTA
 Home-page: https://github.com/Tencent/QTAF
 Author: Tencent
 License: Copyright(c)2010-2018 Tencent All Rights Reserved. 
 Project-URL: TestBase Documentation, https://qta-testbase.readthedocs.io/zh/latest/
 Project-URL: TUIA Documentation, https://qta-tuia.readthedocs.io/zh/latest/
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `qtaf-5.6.0/README.md` & `qtaf-5.6.1/README.md`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/__main__.py` & `qtaf-5.6.1/__main__.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/qta-manage.py` & `qtaf-5.6.1/qta-manage.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/qta_statics/TestReport.xsl` & `qtaf-5.6.1/qta_statics/TestReport.xsl`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/qta_statics/TestResult.xsl` & `qtaf-5.6.1/qta_statics/TestResult.xsl`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/qta_statics/qta-report.html` & `qtaf-5.6.1/qta_statics/qta-report.html`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/qtaf.egg-info/PKG-INFO` & `qtaf-5.6.1/qtaf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtaf
-Version: 5.6.0
+Version: 5.6.1
 Summary: Basic test automation framework for QTA
 Home-page: https://github.com/Tencent/QTAF
 Author: Tencent
 License: Copyright(c)2010-2018 Tencent All Rights Reserved. 
 Project-URL: TestBase Documentation, https://qta-testbase.readthedocs.io/zh/latest/
 Project-URL: TUIA Documentation, https://qta-tuia.readthedocs.io/zh/latest/
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `qtaf-5.6.0/qtaf.egg-info/SOURCES.txt` & `qtaf-5.6.1/qtaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/qtaf_settings.py` & `qtaf-5.6.1/qtaf_settings.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/setup.py` & `qtaf-5.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/__init__.py` & `qtaf-5.6.1/testbase/__init__.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/assertion.py` & `qtaf-5.6.1/testbase/assertion.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/conf.py` & `qtaf-5.6.1/testbase/conf.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/context.py` & `qtaf-5.6.1/testbase/context.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/datadrive.py` & `qtaf-5.6.1/testbase/datadrive.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/dist.py` & `qtaf-5.6.1/testbase/dist.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/exlib.py` & `qtaf-5.6.1/testbase/exlib.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/loader.py` & `qtaf-5.6.1/testbase/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,17 +296,23 @@
         """
         if exclude_data_key is None:
             exclude_data_key = []
         exclude_data_key = [smart_text(i) for i in exclude_data_key]
 
         tests = []
         if datadrive.is_datadrive(cls) or settings.DATA_DRIVE:
-            tests = datadrive.load_datadrive_tests(cls, data_key, attrs)
-            if len(tests) == 0:
-                tests = [cls(attrs=attrs)]
+            try:
+                tests = datadrive.load_datadrive_tests(cls, data_key, attrs)
+            except ValueError:
+                self._module_errs[
+                    "%s.%s/%s" % (cls.__module__, cls.__name__, data_key)
+                ] = traceback.format_exc()
+            else:
+                if len(tests) == 0:
+                    tests = [cls(attrs=attrs)]
         else:
             tests = [cls(attrs=attrs)]
 
         if self._filter:
             final_tests = []
             for it in tests:
                 filter_reason = self._filter(it)
```

### Comparing `qtaf-5.6.0/testbase/logger.py` & `qtaf-5.6.1/testbase/logger.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/management.py` & `qtaf-5.6.1/testbase/management.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/plan.py` & `qtaf-5.6.1/testbase/plan.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/project.py` & `qtaf-5.6.1/testbase/project.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/report.py` & `qtaf-5.6.1/testbase/report.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/resource.py` & `qtaf-5.6.1/testbase/resource.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/retry.py` & `qtaf-5.6.1/testbase/retry.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/runner.py` & `qtaf-5.6.1/testbase/runner.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/serialization.py` & `qtaf-5.6.1/testbase/serialization.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/test.py` & `qtaf-5.6.1/testbase/test.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/testcase.py` & `qtaf-5.6.1/testbase/testcase.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/testresult.py` & `qtaf-5.6.1/testbase/testresult.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/testsuite.py` & `qtaf-5.6.1/testbase/testsuite.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/types.py` & `qtaf-5.6.1/testbase/types.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/testbase/util.py` & `qtaf-5.6.1/testbase/util.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/__init__.py` & `qtaf-5.6.1/tuia/__init__.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/_tif.py` & `qtaf-5.6.1/tuia/_tif.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/accessible.py` & `qtaf-5.6.1/tuia/accessible.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/app.py` & `qtaf-5.6.1/tuia/app.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/control.py` & `qtaf-5.6.1/tuia/control.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/env.py` & `qtaf-5.6.1/tuia/env.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/exceptions.py` & `qtaf-5.6.1/tuia/exceptions.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/filedialog.py` & `qtaf-5.6.1/tuia/filedialog.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/gfcontrols.py` & `qtaf-5.6.1/tuia/gfcontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/keyboard.py` & `qtaf-5.6.1/tuia/keyboard.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/mouse.py` & `qtaf-5.6.1/tuia/mouse.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/qpath.py` & `qtaf-5.6.1/tuia/qpath.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/qpathparser.py` & `qtaf-5.6.1/tuia/qpathparser.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/remoteprocessing.py` & `qtaf-5.6.1/tuia/remoteprocessing.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/testcase.py` & `qtaf-5.6.1/tuia/testcase.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/uiacontrols.py` & `qtaf-5.6.1/tuia/uiacontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/util.py` & `qtaf-5.6.1/tuia/util.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/webcontrols.py` & `qtaf-5.6.1/tuia/webcontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/wincontrols.py` & `qtaf-5.6.1/tuia/wincontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.0/tuia/wintypes.py` & `qtaf-5.6.1/tuia/wintypes.py`

 * *Files identical despite different names*

