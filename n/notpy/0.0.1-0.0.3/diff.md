# Comparing `tmp/notpy-0.0.1.tar.gz` & `tmp/notpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notpy-0.0.1.tar", max compression
+gzip compressed data, was "notpy-0.0.3.tar", max compression
```

## Comparing `notpy-0.0.1.tar` & `notpy-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-04-21 23:25:40.662307 notpy-0.0.1/LICENSE
--rw-r--r--   0        0        0     2960 2023-04-21 23:25:40.662307 notpy-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-21 23:25:40.662307 notpy-0.0.1/notpy/__init__.py
--rw-r--r--   0        0        0     7995 2023-04-21 23:25:40.662307 notpy-0.0.1/notpy/modules/commandline.py
--rw-r--r--   0        0        0     3743 2023-04-21 23:25:40.662307 notpy-0.0.1/notpy/modules/configure.py
--rw-r--r--   0        0        0     1453 2023-04-21 23:25:40.662307 notpy-0.0.1/notpy/modules/edit_md.py
--rw-r--r--   0        0        0     6353 2023-04-21 23:25:40.662307 notpy-0.0.1/notpy/modules/notebook.py
--rw-r--r--   0        0        0      169 2023-04-21 23:25:40.662307 notpy-0.0.1/notpy/modules/read_md.py
--rw-r--r--   0        0        0      135 2023-04-21 23:25:40.662307 notpy-0.0.1/notpy/modules/render_md.py
--rw-r--r--   0        0        0     1264 2023-04-21 23:25:40.662307 notpy-0.0.1/notpy/modules/show_md.py
--rw-r--r--   0        0        0     1158 2023-04-21 23:25:40.662307 notpy-0.0.1/notpy/modules/style.css
--rw-r--r--   0        0        0     1715 2023-04-21 23:25:40.662307 notpy-0.0.1/notpy/notpy.py
--rw-r--r--   0        0        0      883 2023-04-21 23:25:40.662307 notpy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 notpy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-22 11:38:55.676868 notpy-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2960 2023-04-22 11:38:55.676868 notpy-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/__init__.py
+-rw-r--r--   0        0        0     7995 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/commandline.py
+-rw-r--r--   0        0        0     3803 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/configure.py
+-rw-r--r--   0        0        0     1453 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/edit_md.py
+-rw-r--r--   0        0        0     6353 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/notebook.py
+-rw-r--r--   0        0        0      169 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/read_md.py
+-rw-r--r--   0        0        0      135 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/render_md.py
+-rw-r--r--   0        0        0     1264 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/show_md.py
+-rw-r--r--   0        0        0     1158 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/modules/style.css
+-rw-r--r--   0        0        0     1715 2023-04-22 11:38:55.676868 notpy-0.0.3/notpy/notpy.py
+-rw-r--r--   0        0        0      883 2023-04-22 11:38:55.676868 notpy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 notpy-0.0.3/PKG-INFO
```

### Comparing `notpy-0.0.1/LICENSE` & `notpy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `notpy-0.0.1/README.md` & `notpy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `notpy-0.0.1/notpy/modules/commandline.py` & `notpy-0.0.3/notpy/modules/commandline.py`

 * *Files identical despite different names*

### Comparing `notpy-0.0.1/notpy/modules/configure.py` & `notpy-0.0.3/notpy/modules/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                     return "done"
         case "n" | "no":
             return "done"
         case _:
             print ("Not a valid value")
 
     config["setup"] = True
-    shutil.copyfile("./modules/style.css", str(Path.home()) + "/.config/notpy/style.css")
+    shutil.copyfile(str(Path.home()) + "/.local/lib/python3.10/site-packages/notpy/modules/style.css", str(Path.home()) + "/.config/notpy/style.css")
     setConfigFile(config_file, config)
     print("Setup finished")
 
 def editConfig():
     print("Configuration File located in $HOME/.config/notpy")
     home = str(Path.home())
     path = home + "/.config/notpy"
```

### Comparing `notpy-0.0.1/notpy/modules/edit_md.py` & `notpy-0.0.3/notpy/modules/edit_md.py`

 * *Files identical despite different names*

### Comparing `notpy-0.0.1/notpy/modules/notebook.py` & `notpy-0.0.3/notpy/modules/notebook.py`

 * *Files identical despite different names*

### Comparing `notpy-0.0.1/notpy/modules/show_md.py` & `notpy-0.0.3/notpy/modules/show_md.py`

 * *Files identical despite different names*

### Comparing `notpy-0.0.1/notpy/modules/style.css` & `notpy-0.0.3/notpy/modules/style.css`

 * *Files identical despite different names*

### Comparing `notpy-0.0.1/notpy/notpy.py` & `notpy-0.0.3/notpy/notpy.py`

 * *Files identical despite different names*

### Comparing `notpy-0.0.1/pyproject.toml` & `notpy-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notpy"
-version = "0.0.1"
+version = "0.0.3"
 description = "Create/Delete files and edit them as markdown files in neovim"
 authors = ["jontok <jonas@tokmaji.de>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     {include = "notpy"},
 ]
```

### Comparing `notpy-0.0.1/PKG-INFO` & `notpy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notpy
-Version: 0.0.1
+Version: 0.0.3
 Summary: Create/Delete files and edit them as markdown files in neovim
 Home-page: https://github.com/jontok/Notpy
 License: GPL-3.0-only
 Keywords: notes,markdown,python,nvim,neovim
 Author: jontok
 Author-email: jonas@tokmaji.de
 Requires-Python: >=3.10,<4.0
```

