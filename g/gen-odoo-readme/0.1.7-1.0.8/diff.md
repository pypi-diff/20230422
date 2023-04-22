# Comparing `tmp/gen-odoo-readme-0.1.7.tar.gz` & `tmp/gen-odoo-readme-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen-odoo-readme-0.1.7.tar", last modified: Sat Apr 22 15:57:33 2023, max compression
+gzip compressed data, was "gen-odoo-readme-1.0.8.tar", last modified: Sat Apr 22 17:29:49 2023, max compression
```

## Comparing `gen-odoo-readme-0.1.7.tar` & `gen-odoo-readme-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:57:33.882892 gen-odoo-readme-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-22 15:57:22.000000 gen-odoo-readme-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-22 15:57:33.882892 gen-odoo-readme-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-22 15:57:22.000000 gen-odoo-readme-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:57:33.882892 gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-22 15:57:33.000000 gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-22 15:57:33.000000 gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 15:57:33.000000 gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-22 15:57:33.000000 gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 15:57:33.000000 gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 15:57:33.000000 gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-22 15:57:33.882892 gen-odoo-readme-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-22 15:57:22.000000 gen-odoo-readme-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:57:33.882892 gen-odoo-readme-0.1.7/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 15:57:22.000000 gen-odoo-readme-0.1.7/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-22 15:57:22.000000 gen-odoo-readme-0.1.7/tools/gen_addon_readme.template
--rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-04-22 15:57:22.000000 gen-odoo-readme-0.1.7/tools/gen_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-22 15:57:22.000000 gen-odoo-readme-0.1.7/tools/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:29:49.815744 gen-odoo-readme-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-22 17:29:36.000000 gen-odoo-readme-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-22 17:29:49.815744 gen-odoo-readme-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-22 17:29:36.000000 gen-odoo-readme-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:29:49.815744 gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-22 17:29:49.000000 gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-22 17:29:49.000000 gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:29:49.000000 gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-22 17:29:49.000000 gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 17:29:49.000000 gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 17:29:49.000000 gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-22 17:29:49.815744 gen-odoo-readme-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-22 17:29:36.000000 gen-odoo-readme-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:29:49.815744 gen-odoo-readme-1.0.8/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 17:29:36.000000 gen-odoo-readme-1.0.8/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-22 17:29:36.000000 gen-odoo-readme-1.0.8/tools/gen_addon_readme.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-04-22 17:29:36.000000 gen-odoo-readme-1.0.8/tools/gen_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-22 17:29:36.000000 gen-odoo-readme-1.0.8/tools/manifest.py
```

### Comparing `gen-odoo-readme-0.1.7/LICENSE` & `gen-odoo-readme-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.7/PKG-INFO` & `gen-odoo-readme-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-odoo-readme
-Version: 0.1.7
+Version: 1.0.8
 Summary: Tool to create README.rst files for Odoo
 Home-page: https://github.com/jobiols/gen-readme
 Author: Jorge E. Obiols
 Author-email: jorge.obiols@gmail.com
 Keywords: odoo documentation readme rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gen-odoo-readme-0.1.7/README.md` & `gen-odoo-readme-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.7/gen_odoo_readme.egg-info/PKG-INFO` & `gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-odoo-readme
-Version: 0.1.7
+Version: 1.0.8
 Summary: Tool to create README.rst files for Odoo
 Home-page: https://github.com/jobiols/gen-readme
 Author: Jorge E. Obiols
 Author-email: jorge.obiols@gmail.com
 Keywords: odoo documentation readme rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gen-odoo-readme-0.1.7/setup.py` & `gen-odoo-readme-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.7/tools/gen_addon_readme.template` & `gen-odoo-readme-1.0.8/tools/gen_addon_readme.template`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.7/tools/gen_readme.py` & `gen-odoo-readme-1.0.8/tools/gen_readme.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,24 +242,29 @@
     "--branch",
     required=True,
     help="Odoo series. eg 11.0.",
 )
 @click.option(
     "--addons-dir",
     type=click.Path(dir_okay=True, file_okay=False, exists=True),
-    required=True,
+    required=False,
     help="Directory containing several addons, the README will be "
     "generated for all installable addons found there.",
 )
 @click.option(
     "--gen-html/--no-gen-html",
     default=True,
     help="Generate index html file.",
 )
 def gen_readme(org_name, repo_name, branch, addons_dir, gen_html):
+    """main function"""
+
+    print("Gen Readme ------------------")
+    print(os.path.abspath(__file__))
+
     addons = list()
     if addons_dir:
         addons.extend(find_addons(addons_dir))
     readme_filenames = []
     for addon_name, addon_dir, manifest in addons:
         if not os.path.exists(
             os.path.join(addon_dir, FRAGMENTS_DIR, "DESCRIPTION.rst")
```

### Comparing `gen-odoo-readme-0.1.7/tools/manifest.py` & `gen-odoo-readme-1.0.8/tools/manifest.py`

 * *Files identical despite different names*

