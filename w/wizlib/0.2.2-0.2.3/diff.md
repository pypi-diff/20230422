# Comparing `tmp/wizlib-0.2.2.tar.gz` & `tmp/wizlib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-0.2.2.tar", last modified: Sat Apr  8 20:46:25 2023, max compression
+gzip compressed data, was "wizlib-0.2.3.tar", last modified: Sat Apr 22 17:27:30 2023, max compression
```

## Comparing `wizlib-0.2.2.tar` & `wizlib-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-08 20:46:25.179970 wizlib-0.2.2/
--rw-r--r--   0 francispotter   (501) staff       (20)     1771 2023-04-08 20:46:25.179190 wizlib-0.2.2/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)     1506 2023-04-06 16:26:14.000000 wizlib-0.2.2/README.md
--rw-r--r--   0 francispotter   (501) staff       (20)      540 2023-04-08 05:14:05.000000 wizlib-0.2.2/pyproject.toml
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-08 20:46:25.180263 wizlib-0.2.2/setup.cfg
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-08 20:46:06.000000 wizlib-0.2.2/version
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-08 20:46:25.173927 wizlib-0.2.2/wizlib/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-06 04:54:28.000000 wizlib-0.2.2/wizlib/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1750 2023-04-08 20:06:29.000000 wizlib-0.2.2/wizlib/rlinput.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-08 20:46:25.178398 wizlib-0.2.2/wizlib.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)     1771 2023-04-08 20:46:25.000000 wizlib-0.2.2/wizlib.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)      218 2023-04-08 20:46:25.000000 wizlib-0.2.2/wizlib.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-08 20:46:25.000000 wizlib-0.2.2/wizlib.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       89 2023-04-08 20:46:25.000000 wizlib-0.2.2/wizlib.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        7 2023-04-08 20:46:25.000000 wizlib-0.2.2/wizlib.egg-info/top_level.txt
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 17:27:30.594458 wizlib-0.2.3/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1771 2023-04-22 17:27:30.594100 wizlib-0.2.3/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)     1506 2023-04-06 16:26:14.000000 wizlib-0.2.3/README.md
+-rw-r--r--   0 francispotter   (501) staff       (20)      540 2023-04-08 05:14:05.000000 wizlib-0.2.3/pyproject.toml
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-22 17:27:30.594538 wizlib-0.2.3/setup.cfg
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-22 17:27:16.000000 wizlib-0.2.3/version
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 17:27:30.590810 wizlib-0.2.3/wizlib/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-06 04:54:28.000000 wizlib-0.2.3/wizlib/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1626 2023-04-22 17:25:11.000000 wizlib-0.2.3/wizlib/rlinput.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 17:27:30.593749 wizlib-0.2.3/wizlib.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1771 2023-04-22 17:27:30.000000 wizlib-0.2.3/wizlib.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)      218 2023-04-22 17:27:30.000000 wizlib-0.2.3/wizlib.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-22 17:27:30.000000 wizlib-0.2.3/wizlib.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       89 2023-04-22 17:27:30.000000 wizlib-0.2.3/wizlib.egg-info/requires.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        7 2023-04-22 17:27:30.000000 wizlib-0.2.3/wizlib.egg-info/top_level.txt
```

### Comparing `wizlib-0.2.2/PKG-INFO` & `wizlib-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.2.2
+Version: 0.2.3
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

### Comparing `wizlib-0.2.2/README.md` & `wizlib-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `wizlib-0.2.2/pyproject.toml` & `wizlib-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wizlib-0.2.2/wizlib/rlinput.py` & `wizlib-0.2.3/wizlib/rlinput.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,28 +4,26 @@
     import readline
 import sys
 
 
 # Use tab for completion
 readline.parse_and_bind('tab: complete')
 
+# Only a space separates words
+readline.set_completer_delims(' ')
+
 
 # Readline defaults to complete with local filenames. Definitely not what we
 # want.
 
 def null_complete(text, start):
     return None
 readline.set_completer(null_complete)
 
 
-# I'd like to bind a special key (like ctrl-del) to kill-whole-line, but I can't
-# get it to work on my Mac in iTerm. So we're going to use ctrl-A for that.
-# readline.parse_and_bind('"\C-a": kill-whole-line')
-
-
 def rlinput(prompt:str="", default:str="", options:list=None):
     """
     Get input with preset default and/or tab completion of options
 
     Parameters:
 
     prompt:str - string to output before requesting input, same as in the
@@ -57,9 +55,12 @@
     finally:
         readline.set_startup_hook()
         readline.set_completer(null_complete)
     return value.strip()
 
 def tryit():
     """Quick and dirty tester function"""
-    return rlinput(prompt='>', default='delete me', \
-            options=['start','stop'])
+    return rlinput(prompt='>', \
+            options=['a-b','a-c','b-a'])
+
+if __name__ == '__main__':
+    tryit()
```

### Comparing `wizlib-0.2.2/wizlib.egg-info/PKG-INFO` & `wizlib-0.2.3/wizlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.2.2
+Version: 0.2.3
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

