# Comparing `tmp/bdgd_tools-0.2.3.tar.gz` & `tmp/bdgd_tools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdgd_tools-0.2.3.tar", last modified: Wed Mar 22 14:16:09 2023, max compression
+gzip compressed data, was "bdgd_tools-1.0.2.tar", last modified: Sat Apr 22 13:51:42 2023, max compression
```

## Comparing `bdgd_tools-0.2.3.tar` & `bdgd_tools-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:16:09.393029 bdgd_tools-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-22 14:16:03.000000 bdgd_tools-0.2.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-03-22 14:16:03.000000 bdgd_tools-0.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-22 14:16:03.000000 bdgd_tools-0.2.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-22 14:16:03.000000 bdgd_tools-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-22 14:16:03.000000 bdgd_tools-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-03-22 14:16:09.393029 bdgd_tools-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-22 14:16:03.000000 bdgd_tools-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:16:09.393029 bdgd_tools-0.2.3/bdgd_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-22 14:16:03.000000 bdgd_tools-0.2.3/bdgd_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-22 14:16:03.000000 bdgd_tools-0.2.3/bdgd_tools/bdgd_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:16:09.393029 bdgd_tools-0.2.3/bdgd_tools/sample/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-22 14:16:03.000000 bdgd_tools-0.2.3/bdgd_tools/sample/Sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-22 14:16:03.000000 bdgd_tools-0.2.3/bdgd_tools/sample/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:16:09.393029 bdgd_tools-0.2.3/bdgd_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-03-22 14:16:09.000000 bdgd_tools-0.2.3/bdgd_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-22 14:16:09.000000 bdgd_tools-0.2.3/bdgd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 14:16:09.000000 bdgd_tools-0.2.3/bdgd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 14:16:09.000000 bdgd_tools-0.2.3/bdgd_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-22 14:16:09.000000 bdgd_tools-0.2.3/bdgd_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:16:09.393029 bdgd_tools-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-22 14:16:04.000000 bdgd_tools-0.2.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-22 14:16:04.000000 bdgd_tools-0.2.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-03-22 14:16:04.000000 bdgd_tools-0.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-22 14:16:04.000000 bdgd_tools-0.2.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-22 14:16:04.000000 bdgd_tools-0.2.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-22 14:16:04.000000 bdgd_tools-0.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-22 14:16:04.000000 bdgd_tools-0.2.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-22 14:16:04.000000 bdgd_tools-0.2.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-22 14:16:04.000000 bdgd_tools-0.2.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-22 14:16:04.000000 bdgd_tools-0.2.3/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-22 14:16:09.393029 bdgd_tools-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-22 14:16:07.000000 bdgd_tools-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:16:09.393029 bdgd_tools-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-22 14:16:04.000000 bdgd_tools-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-22 14:16:04.000000 bdgd_tools-0.2.3/tests/test_bdgd_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.535063 bdgd_tools-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-22 13:51:42.535063 bdgd_tools-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.531063 bdgd_tools-1.0.2/bdgd_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.531063 bdgd_tools-1.0.2/bdgd_tools/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/core/Core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/core/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.531063 bdgd_tools-1.0.2/bdgd_tools/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/gui/GUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.535063 bdgd_tools-1.0.2/bdgd_tools/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/BusCoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/Capacitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/Case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/Circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/Count_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/LineCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/Loadshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.535063 bdgd_tools-1.0.2/bdgd_tools/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/sample/Sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/sample/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.531063 bdgd_tools-1.0.2/bdgd_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-22 13:51:42.000000 bdgd_tools-1.0.2/bdgd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-22 13:51:42.000000 bdgd_tools-1.0.2/bdgd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 13:51:42.000000 bdgd_tools-1.0.2/bdgd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 13:51:42.000000 bdgd_tools-1.0.2/bdgd_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 13:51:42.000000 bdgd_tools-1.0.2/bdgd_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.535063 bdgd_tools-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-22 13:51:42.535063 bdgd_tools-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-22 13:51:41.000000 bdgd_tools-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.535063 bdgd_tools-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/tests/test_bdgd_tools.py
```

### Comparing `bdgd_tools-0.2.3/CONTRIBUTING.rst` & `bdgd_tools-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bdgd_tools-0.2.3/LICENSE` & `bdgd_tools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bdgd_tools-0.2.3/PKG-INFO` & `bdgd_tools-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdgd_tools
-Version: 0.2.3
+Version: 1.0.2
 Summary: Short description
 Home-page: https://github.com/eniocc/bdgd_tools
 Author: Ênio Rodrigues
 Author-email: eniocc@gmail.com
 License: MIT license
 Keywords: bdgd_tools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,62 +13,83 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-==========
 bdgd-tools
-==========
+=======================
+A set of tools to work with the BDGD (Base de Dados da Distribuidora) format, conversion to the DSS format (OpenDSS) and visualization.
 
 
 .. image:: https://img.shields.io/pypi/v/bdgd_tools.svg
         :target: https://pypi.python.org/pypi/bdgd_tools
 
+
 .. image:: https://img.shields.io/travis/eniocc/bdgd_tools.svg
         :target: https://travis-ci.com/eniocc/bdgd_tools
 
+
 .. image:: https://readthedocs.org/projects/bdgd-tools/badge/?version=latest
         :target: https://bdgd-tools.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
-
-.. image:: https://pyup.io/repos/github/eniocc/bdgd_tools/shield.svg
-     :target: https://pyup.io/repos/github/eniocc/bdgd_tools/
-     :alt: Updates
+..
+    .. image:: https://pyup.io/repos/github/eniocc/bdgd_tools/shield.svg
+         :target: https://pyup.io/repos/github/eniocc/bdgd_tools/
+         :alt: Updates
 
 
+.. |OK_ICON| image:: https://raw.githubusercontent.com/awesomedata/apd-core/master/deploy/ok-24.png
+.. |FIXME_ICON| image:: https://raw.githubusercontent.com/awesomedata/apd-core/master/deploy/fixme-24.png
 
-A set of tools to work with the BDGD format, conversion to the DSS format (OPENDSS) and visualization.
+..
+  _
 
 
 * Free software: MIT license
-* Documentation: https://bdgd-tools.readthedocs.io.
+* Documentation: https://bdgd-tools.readthedocs.io
+
+
+
+Installation
+=======================
+  pip install bdgd-tools
 
 
 Features
---------
+=======================
+Conversion of Electric Power Systems from BGDG format to DSS (Opendss), including.
+
+* |OK_ICON| Improved memory management by loading the layers of the disk
+* |OK_ICON| Circuit OpenDSS element creation
+* |OK_ICON|  LineCode OpenDSS element creation
+* |FIXME_ICON|  LoadShape OpenDSS element creation
+* |FIXME_ICON|  Line OpenDSS element creation
+* |FIXME_ICON|  Transformer OpenDSS element creation
+* |FIXME_ICON|  Reactor OpenDSS element creation
+* |FIXME_ICON|  RegControl OpenDSS element creation
+* |FIXME_ICON|  Load OpenDSS element creation
+
 
-* Conversion of Electric Power Systems from BGDG format to DSS (Opendss)
 
-Credits
--------
 
-This package was created by [Ênio Rodrigues](https://github.com/eniocc) and Rodolgo Londero
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+1.0.1(2023-04-22)
+------------------
+
+* Backend modifications to run properly auto publish and readthedocs.
+
 1.0.0(2023-03-22)
 ------------------
 
 * Tested and running on python 3.9
 * Clean architecture. Old models, classes and tests were removed
 * Major conversion using json file based was inserted
 * Now we can read different bdgd versions
```

### Comparing `bdgd_tools-0.2.3/bdgd_tools.egg-info/PKG-INFO` & `bdgd_tools-1.0.2/bdgd_tools.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdgd-tools
-Version: 0.2.3
+Version: 1.0.2
 Summary: Short description
 Home-page: https://github.com/eniocc/bdgd_tools
 Author: Ênio Rodrigues
 Author-email: eniocc@gmail.com
 License: MIT license
 Keywords: bdgd_tools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,62 +13,83 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-==========
 bdgd-tools
-==========
+=======================
+A set of tools to work with the BDGD (Base de Dados da Distribuidora) format, conversion to the DSS format (OpenDSS) and visualization.
 
 
 .. image:: https://img.shields.io/pypi/v/bdgd_tools.svg
         :target: https://pypi.python.org/pypi/bdgd_tools
 
+
 .. image:: https://img.shields.io/travis/eniocc/bdgd_tools.svg
         :target: https://travis-ci.com/eniocc/bdgd_tools
 
+
 .. image:: https://readthedocs.org/projects/bdgd-tools/badge/?version=latest
         :target: https://bdgd-tools.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
-
-.. image:: https://pyup.io/repos/github/eniocc/bdgd_tools/shield.svg
-     :target: https://pyup.io/repos/github/eniocc/bdgd_tools/
-     :alt: Updates
+..
+    .. image:: https://pyup.io/repos/github/eniocc/bdgd_tools/shield.svg
+         :target: https://pyup.io/repos/github/eniocc/bdgd_tools/
+         :alt: Updates
 
 
+.. |OK_ICON| image:: https://raw.githubusercontent.com/awesomedata/apd-core/master/deploy/ok-24.png
+.. |FIXME_ICON| image:: https://raw.githubusercontent.com/awesomedata/apd-core/master/deploy/fixme-24.png
 
-A set of tools to work with the BDGD format, conversion to the DSS format (OPENDSS) and visualization.
+..
+  _
 
 
 * Free software: MIT license
-* Documentation: https://bdgd-tools.readthedocs.io.
+* Documentation: https://bdgd-tools.readthedocs.io
+
+
+
+Installation
+=======================
+  pip install bdgd-tools
 
 
 Features
---------
+=======================
+Conversion of Electric Power Systems from BGDG format to DSS (Opendss), including.
+
+* |OK_ICON| Improved memory management by loading the layers of the disk
+* |OK_ICON| Circuit OpenDSS element creation
+* |OK_ICON|  LineCode OpenDSS element creation
+* |FIXME_ICON|  LoadShape OpenDSS element creation
+* |FIXME_ICON|  Line OpenDSS element creation
+* |FIXME_ICON|  Transformer OpenDSS element creation
+* |FIXME_ICON|  Reactor OpenDSS element creation
+* |FIXME_ICON|  RegControl OpenDSS element creation
+* |FIXME_ICON|  Load OpenDSS element creation
+
 
-* Conversion of Electric Power Systems from BGDG format to DSS (Opendss)
 
-Credits
--------
 
-This package was created by [Ênio Rodrigues](https://github.com/eniocc) and Rodolgo Londero
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+1.0.1(2023-04-22)
+------------------
+
+* Backend modifications to run properly auto publish and readthedocs.
+
 1.0.0(2023-03-22)
 ------------------
 
 * Tested and running on python 3.9
 * Clean architecture. Old models, classes and tests were removed
 * Major conversion using json file based was inserted
 * Now we can read different bdgd versions
```

### Comparing `bdgd_tools-0.2.3/docs/Makefile` & `bdgd_tools-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bdgd_tools-0.2.3/docs/conf.py` & `bdgd_tools-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bdgd_tools-0.2.3/docs/installation.rst` & `bdgd_tools-1.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `bdgd_tools-0.2.3/docs/make.bat` & `bdgd_tools-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bdgd_tools-0.2.3/setup.py` & `bdgd_tools-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,10 +33,10 @@
     include_package_data=True,
     keywords='bdgd_tools',
     name='bdgd_tools',
     packages=find_packages(include=['bdgd_tools', 'bdgd_tools.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/eniocc/bdgd_tools',
-    version='0.2.3',
+    version='1.0.2',
     zip_safe=False,
 )
```

