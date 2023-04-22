# Comparing `tmp/filewiz-1.0.2.tar.gz` & `tmp/filewiz-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filewiz-1.0.2.tar", last modified: Mon Apr 10 05:24:53 2023, max compression
+gzip compressed data, was "filewiz-1.0.3.tar", last modified: Sat Apr 22 17:32:43 2023, max compression
```

## Comparing `filewiz-1.0.2.tar` & `filewiz-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 05:24:53.185915 filewiz-1.0.2/
--rw-r--r--   0 francispotter   (501) staff       (20)     1602 2023-04-10 05:24:53.185262 filewiz-1.0.2/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)     1347 2023-04-10 05:15:01.000000 filewiz-1.0.2/README.md
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 05:24:53.181953 filewiz-1.0.2/filewiz/
--rw-r--r--   0 francispotter   (501) staff       (20)     1499 2023-04-10 05:18:52.000000 filewiz-1.0.2/filewiz/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-04-10 05:20:07.000000 filewiz-1.0.2/filewiz/__main__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      103 2023-04-10 05:20:31.000000 filewiz-1.0.2/filewiz/handler.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1283 2023-04-05 00:32:38.000000 filewiz-1.0.2/filewiz/readline_util.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 05:24:53.184775 filewiz-1.0.2/filewiz.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)     1602 2023-04-10 05:24:53.000000 filewiz-1.0.2/filewiz.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)      304 2023-04-10 05:24:53.000000 filewiz-1.0.2/filewiz.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-10 05:24:53.000000 filewiz-1.0.2/filewiz.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       49 2023-04-10 05:24:53.000000 filewiz-1.0.2/filewiz.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       14 2023-04-10 05:24:53.000000 filewiz-1.0.2/filewiz.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        8 2023-04-10 05:24:53.000000 filewiz-1.0.2/filewiz.egg-info/top_level.txt
--rw-r--r--   0 francispotter   (501) staff       (20)      562 2023-04-10 05:14:21.000000 filewiz-1.0.2/pyproject.toml
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-10 05:24:53.186030 filewiz-1.0.2/setup.cfg
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-10 05:24:14.000000 filewiz-1.0.2/version
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 17:32:43.618800 filewiz-1.0.3/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1873 2023-04-22 17:32:43.618399 filewiz-1.0.3/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)     1618 2023-04-10 05:40:23.000000 filewiz-1.0.3/README.md
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 17:32:43.614318 filewiz-1.0.3/filewiz/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1504 2023-04-22 17:30:41.000000 filewiz-1.0.3/filewiz/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-04-10 05:20:07.000000 filewiz-1.0.3/filewiz/__main__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      309 2023-04-22 05:29:13.000000 filewiz-1.0.3/filewiz/handler.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1283 2023-04-05 00:32:38.000000 filewiz-1.0.3/filewiz/readline_util.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 17:32:43.617745 filewiz-1.0.3/filewiz.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1873 2023-04-22 17:32:43.000000 filewiz-1.0.3/filewiz.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)      304 2023-04-22 17:32:43.000000 filewiz-1.0.3/filewiz.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-22 17:32:43.000000 filewiz-1.0.3/filewiz.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       49 2023-04-22 17:32:43.000000 filewiz-1.0.3/filewiz.egg-info/entry_points.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       14 2023-04-22 17:32:43.000000 filewiz-1.0.3/filewiz.egg-info/requires.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        8 2023-04-22 17:32:43.000000 filewiz-1.0.3/filewiz.egg-info/top_level.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)      562 2023-04-22 17:30:53.000000 filewiz-1.0.3/pyproject.toml
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-22 17:32:43.618934 filewiz-1.0.3/setup.cfg
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-22 17:32:29.000000 filewiz-1.0.3/version
```

### Comparing `filewiz-1.0.2/PKG-INFO` & `filewiz-1.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1
-Name: filewiz
-Version: 1.0.2
-Summary: Quickly rename and move new files into structured folders
-Author-email: Francis Potter <filewiz@steampunkwizard.ca>
-License: MIT
-Requires-Python: >=3.6.5
-Description-Content-Type: text/markdown
-
 # FileWiz
 
 I keep files named and organized in a certain way in DropBox. This tool names new files correctly and puts them in the right directory.
 
+## Installation
+
+It's best to install using `pipx`. See [the pipx site](https://pypa.github.io/pipx/) if you need it. Then:
+
+```bash
+pipx install filewiz
+```
+
+## Usage
+
 The directory pattern for account documents is:
 
 ```
 ~/Dropbox/accounts/<year>/<account>/<date>-<part>.<extension>
 ```
 
 Where:
@@ -31,9 +32,13 @@
 filewiz ~/Desktop/123456789SomeFileIDownloaded.pdf
 ```
 
 FileWiz will ask a series of questions, then move the file.
 
 Note the `part` supports tab-completion, where it looks up all the files previously stored under that account, in any year. So it's easy to reproduce names of periodic files such as financial statements or invoices.
 
-Logo by [vectorsmarket15](https://www.flaticon.com/free-icon/folders_2821739?term=file&page=1&position=15&origin=search&related_id=2821739#:~:text=have%20to%20attribute-,vectorsmarket15,-Every%20time%20you)
+## Credits
+
+Copyright (C) 2023 by Francis Potter. Licensed under the MIT license.
+
+Logo shown on GitLab is by [vectorsmarket15](https://www.flaticon.com/free-icon/folders_2821739?term=file&page=1&position=15&origin=search&related_id=2821739#:~:text=have%20to%20attribute-,vectorsmarket15,-Every%20time%20you)
```

### Comparing `filewiz-1.0.2/README.md` & `filewiz-1.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,30 @@
+Metadata-Version: 2.1
+Name: filewiz
+Version: 1.0.3
+Summary: Quickly rename and move new files into structured folders
+Author-email: Francis Potter <filewiz@steampunkwizard.ca>
+License: MIT
+Requires-Python: >=3.6.5
+Description-Content-Type: text/markdown
+
 # FileWiz
 
 I keep files named and organized in a certain way in DropBox. This tool names new files correctly and puts them in the right directory.
 
+## Installation
+
+It's best to install using `pipx`. See [the pipx site](https://pypa.github.io/pipx/) if you need it. Then:
+
+```bash
+pipx install filewiz
+```
+
+## Usage
+
 The directory pattern for account documents is:
 
 ```
 ~/Dropbox/accounts/<year>/<account>/<date>-<part>.<extension>
 ```
 
 Where:
@@ -22,9 +41,13 @@
 filewiz ~/Desktop/123456789SomeFileIDownloaded.pdf
 ```
 
 FileWiz will ask a series of questions, then move the file.
 
 Note the `part` supports tab-completion, where it looks up all the files previously stored under that account, in any year. So it's easy to reproduce names of periodic files such as financial statements or invoices.
 
-Logo by [vectorsmarket15](https://www.flaticon.com/free-icon/folders_2821739?term=file&page=1&position=15&origin=search&related_id=2821739#:~:text=have%20to%20attribute-,vectorsmarket15,-Every%20time%20you)
+## Credits
+
+Copyright (C) 2023 by Francis Potter. Licensed under the MIT license.
+
+Logo shown on GitLab is by [vectorsmarket15](https://www.flaticon.com/free-icon/folders_2821739?term=file&page=1&position=15&origin=search&related_id=2821739#:~:text=have%20to%20attribute-,vectorsmarket15,-Every%20time%20you)
```

### Comparing `filewiz-1.0.2/filewiz/__init__.py` & `filewiz-1.0.3/filewiz/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from pathlib import Path
 import re
 import sys
 
 from wizlib.rlinput import rlinput
 
-root = Path("~/Dropbox/accounts/").expanduser()
-
 PATTERN = re.compile(r'\d{8}\-([a-zA-Z0-9-]+)\.(\w+)')
 
-def get_parts(root:str, sub:str):
+def get_parts(root:Path, sub:str):
     """Return a set of past filename parts"""
     parts = set()
     for year in root.iterdir():
         if year.name.isdigit():
             subdir = year / sub
             if subdir.is_dir():
                 for file in subdir.iterdir():
                     match = re.match(PATTERN, file.name)
                     if match:
                         parts.add(match.groups()[0])
     return parts
 
-def move_file(source):
+def move_file(source, root_dir:str):
     """Ask the user some questions then move the file"""
+    root = Path(root_dir).expanduser()
     sourcepath = Path(source).expanduser()
     assert sourcepath.is_file()
     extension = sourcepath.suffix
     print("Only handling accounts")
     date = input("Date: ")
     account = input("Account: ")
     parts = get_parts(root, account)
```

### Comparing `filewiz-1.0.2/filewiz/readline_util.py` & `filewiz-1.0.3/filewiz/readline_util.py`

 * *Files identical despite different names*

### Comparing `filewiz-1.0.2/filewiz.egg-info/PKG-INFO` & `filewiz-1.0.3/filewiz.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 Metadata-Version: 2.1
 Name: filewiz
-Version: 1.0.2
+Version: 1.0.3
 Summary: Quickly rename and move new files into structured folders
 Author-email: Francis Potter <filewiz@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 
 # FileWiz
 
 I keep files named and organized in a certain way in DropBox. This tool names new files correctly and puts them in the right directory.
 
+## Installation
+
+It's best to install using `pipx`. See [the pipx site](https://pypa.github.io/pipx/) if you need it. Then:
+
+```bash
+pipx install filewiz
+```
+
+## Usage
+
 The directory pattern for account documents is:
 
 ```
 ~/Dropbox/accounts/<year>/<account>/<date>-<part>.<extension>
 ```
 
 Where:
@@ -31,9 +41,13 @@
 filewiz ~/Desktop/123456789SomeFileIDownloaded.pdf
 ```
 
 FileWiz will ask a series of questions, then move the file.
 
 Note the `part` supports tab-completion, where it looks up all the files previously stored under that account, in any year. So it's easy to reproduce names of periodic files such as financial statements or invoices.
 
-Logo by [vectorsmarket15](https://www.flaticon.com/free-icon/folders_2821739?term=file&page=1&position=15&origin=search&related_id=2821739#:~:text=have%20to%20attribute-,vectorsmarket15,-Every%20time%20you)
+## Credits
+
+Copyright (C) 2023 by Francis Potter. Licensed under the MIT license.
+
+Logo shown on GitLab is by [vectorsmarket15](https://www.flaticon.com/free-icon/folders_2821739?term=file&page=1&position=15&origin=search&related_id=2821739#:~:text=have%20to%20attribute-,vectorsmarket15,-Every%20time%20you)
```

### Comparing `filewiz-1.0.2/pyproject.toml` & `filewiz-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     {name = "Francis Potter", email = "filewiz@steampunkwizard.ca"}
 ]
 description = "Quickly rename and move new files into structured folders"
 readme = "README.md"
 requires-python = ">=3.6.5"
 license = {text = "MIT"}
 dependencies = [
-    "wizlib >=0.2.2"
+    "wizlib >=0.2.3"
 ]
 dynamic = ["version"]
 
 [tool.setuptools.package-dir]
 filewiz = "filewiz"
 
 [project.scripts]
```

