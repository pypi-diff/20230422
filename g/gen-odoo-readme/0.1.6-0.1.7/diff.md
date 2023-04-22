# Comparing `tmp/gen-odoo-readme-0.1.6.tar.gz` & `tmp/gen-odoo-readme-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen-odoo-readme-0.1.6.tar", last modified: Sat Apr 15 18:01:29 2023, max compression
+gzip compressed data, was "gen-odoo-readme-0.1.7.tar", last modified: Sat Apr 22 15:57:33 2023, max compression
```

## Comparing `gen-odoo-readme-0.1.6.tar` & `gen-odoo-readme-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:01:29.181465 gen-odoo-readme-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-15 18:01:16.000000 gen-odoo-readme-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-15 18:01:29.181465 gen-odoo-readme-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-15 18:01:16.000000 gen-odoo-readme-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:01:29.181465 gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-15 18:01:29.000000 gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-15 18:01:29.000000 gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:01:29.000000 gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-15 18:01:29.000000 gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-15 18:01:29.000000 gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 18:01:29.000000 gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-15 18:01:29.181465 gen-odoo-readme-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-15 18:01:16.000000 gen-odoo-readme-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:01:29.181465 gen-odoo-readme-0.1.6/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-15 18:01:16.000000 gen-odoo-readme-0.1.6/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-15 18:01:16.000000 gen-odoo-readme-0.1.6/tools/gen_addon_readme.template
--rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-04-15 18:01:16.000000 gen-odoo-readme-0.1.6/tools/gen_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-15 18:01:16.000000 gen-odoo-readme-0.1.6/tools/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:57:33.882892 gen-odoo-readme-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-22 15:57:22.000000 gen-odoo-readme-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-22 15:57:33.882892 gen-odoo-readme-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-22 15:57:22.000000 gen-odoo-readme-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:57:33.882892 gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-22 15:57:33.000000 gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-22 15:57:33.000000 gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 15:57:33.000000 gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-22 15:57:33.000000 gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 15:57:33.000000 gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 15:57:33.000000 gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-22 15:57:33.882892 gen-odoo-readme-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-22 15:57:22.000000 gen-odoo-readme-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:57:33.882892 gen-odoo-readme-0.1.7/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 15:57:22.000000 gen-odoo-readme-0.1.7/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-22 15:57:22.000000 gen-odoo-readme-0.1.7/tools/gen_addon_readme.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-04-22 15:57:22.000000 gen-odoo-readme-0.1.7/tools/gen_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-22 15:57:22.000000 gen-odoo-readme-0.1.7/tools/manifest.py
```

### Comparing `gen-odoo-readme-0.1.6/LICENSE` & `gen-odoo-readme-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.6/PKG-INFO` & `gen-odoo-readme-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-odoo-readme
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tool to create README.rst files for Odoo
 Home-page: https://github.com/jobiols/gen-readme
 Author: Jorge E. Obiols
 Author-email: jorge.obiols@gmail.com
 Keywords: odoo documentation readme rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gen-odoo-readme-0.1.6/README.md` & `gen-odoo-readme-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.6/gen_odoo_readme.egg-info/PKG-INFO` & `gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-odoo-readme
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tool to create README.rst files for Odoo
 Home-page: https://github.com/jobiols/gen-readme
 Author: Jorge E. Obiols
 Author-email: jorge.obiols@gmail.com
 Keywords: odoo documentation readme rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gen-odoo-readme-0.1.6/setup.py` & `gen-odoo-readme-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.6/tools/gen_addon_readme.template` & `gen-odoo-readme-0.1.7/tools/gen_addon_readme.template`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.6/tools/gen_readme.py` & `gen-odoo-readme-0.1.7/tools/gen_readme.py`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.6/tools/manifest.py` & `gen-odoo-readme-0.1.7/tools/manifest.py`

 * *Files identical despite different names*

