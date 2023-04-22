# Comparing `tmp/notpy-0.0.3.tar.gz` & `tmp/notpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notpy-0.0.3.tar", max compression
+gzip compressed data, was "notpy-0.0.4.tar", max compression
```

## Comparing `notpy-0.0.3.tar` & `notpy-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    35149 2023-04-22 11:38:55.676868 notpy-0.0.3/LICENSE
--rw-r--r--   0        0        0     2960 2023-04-22 11:38:55.676868 notpy-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/__init__.py
--rw-r--r--   0        0        0     7995 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/commandline.py
--rw-r--r--   0        0        0     3803 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/configure.py
--rw-r--r--   0        0        0     1453 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/edit_md.py
--rw-r--r--   0        0        0     6353 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/notebook.py
--rw-r--r--   0        0        0      169 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/read_md.py
--rw-r--r--   0        0        0      135 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/render_md.py
--rw-r--r--   0        0        0     1264 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/show_md.py
--rw-r--r--   0        0        0     1158 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/style.css
--rw-r--r--   0        0        0     1715 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/notpy.py
--rw-r--r--   0        0        0      883 2023-04-22 11:38:55.676868 notpy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 notpy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-22 12:16:21.772439 notpy-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2960 2023-04-22 12:16:21.772439 notpy-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 12:16:21.776439 notpy-0.0.4/notpy/__init__.py
+-rw-r--r--   0        0        0     2960 2023-04-22 12:16:21.776439 notpy-0.0.4/notpy/modules/README.md
+-rw-r--r--   0        0        0     7995 2023-04-22 12:16:21.776439 notpy-0.0.4/notpy/modules/commandline.py
+-rw-r--r--   0        0        0     3871 2023-04-22 12:16:21.776439 notpy-0.0.4/notpy/modules/configure.py
+-rw-r--r--   0        0        0     1453 2023-04-22 12:16:21.776439 notpy-0.0.4/notpy/modules/edit_md.py
+-rw-r--r--   0        0        0     6353 2023-04-22 12:16:21.776439 notpy-0.0.4/notpy/modules/notebook.py
+-rw-r--r--   0        0        0      169 2023-04-22 12:16:21.776439 notpy-0.0.4/notpy/modules/read_md.py
+-rw-r--r--   0        0        0      135 2023-04-22 12:16:21.776439 notpy-0.0.4/notpy/modules/render_md.py
+-rw-r--r--   0        0        0     1264 2023-04-22 12:16:21.776439 notpy-0.0.4/notpy/modules/show_md.py
+-rw-r--r--   0        0        0     1158 2023-04-22 12:16:21.776439 notpy-0.0.4/notpy/modules/style.css
+-rw-r--r--   0        0        0     1715 2023-04-22 12:16:21.776439 notpy-0.0.4/notpy/notpy.py
+-rw-r--r--   0        0        0      883 2023-04-22 12:16:21.776439 notpy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 notpy-0.0.4/PKG-INFO
```

### Comparing `notpy-0.0.3/LICENSE` & `notpy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `notpy-0.0.3/README.md` & `notpy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `notpy-0.0.3/notpy/modules/commandline.py` & `notpy-0.0.4/notpy/modules/commandline.py`

 * *Files identical despite different names*

### Comparing `notpy-0.0.3/notpy/modules/configure.py` & `notpy-0.0.4/notpy/modules/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 def setConfigFile(config_file, config):
     with open(config_file, "r+") as f:
         f.seek(0)
         json.dump(config, f)
         f.close()
 
 def getDefaultPage():
-    with open("./README.md", "r") as readme:
+    with open(str(Path.home()) + "/.local/lib/python3.10/site-packages/notpy/modules/README.md", "r") as readme:
         default_md = readme.read()
         return default_md
 
 def generatePageObject(config, notebook_id, pg_dir):
     page_obj = {
         "id": len(config["notebooks"][notebook_id]["pages"]),
         "name": pg_dir
```

### Comparing `notpy-0.0.3/notpy/modules/edit_md.py` & `notpy-0.0.4/notpy/modules/edit_md.py`

 * *Files identical despite different names*

### Comparing `notpy-0.0.3/notpy/modules/notebook.py` & `notpy-0.0.4/notpy/modules/notebook.py`

 * *Files identical despite different names*

### Comparing `notpy-0.0.3/notpy/modules/show_md.py` & `notpy-0.0.4/notpy/modules/show_md.py`

 * *Files identical despite different names*

### Comparing `notpy-0.0.3/notpy/modules/style.css` & `notpy-0.0.4/notpy/modules/style.css`

 * *Files identical despite different names*

### Comparing `notpy-0.0.3/notpy/notpy.py` & `notpy-0.0.4/notpy/notpy.py`

 * *Files identical despite different names*

### Comparing `notpy-0.0.3/pyproject.toml` & `notpy-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notpy"
-version = "0.0.3"
+version = "0.0.4"
 description = "Create/Delete files and edit them as markdown files in neovim"
 authors = ["jontok <jonas@tokmaji.de>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     {include = "notpy"},
 ]
```

### Comparing `notpy-0.0.3/PKG-INFO` & `notpy-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create/Delete files and edit them as markdown files in neovim
 Home-page: https://github.com/jontok/Notpy
 License: GPL-3.0-only
 Keywords: notes,markdown,python,nvim,neovim
 Author: jontok
 Author-email: jonas@tokmaji.de
 Requires-Python: >=3.10,<4.0
```

