# Comparing `tmp/iode-0.0.1.tar.gz` & `tmp/iode-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iode-0.0.1.tar", last modified: Sun Aug 15 19:20:02 2021, max compression
+gzip compressed data, was "iode-0.0.2.tar", last modified: Wed Aug 18 16:43:11 2021, max compression
```

## Comparing `iode-0.0.1.tar` & `iode-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 egotrip    (501) staff       (20)        0 2021-08-15 19:20:02.091128 iode-0.0.1/
--rw-r--r--   0 egotrip    (501) staff       (20)     1060 2021-08-15 18:17:59.000000 iode-0.0.1/LICENSE
--rw-r--r--   0 egotrip    (501) staff       (20)     1368 2021-08-15 19:20:02.090942 iode-0.0.1/PKG-INFO
--rw-r--r--   0 egotrip    (501) staff       (20)      639 2021-08-15 19:09:40.000000 iode-0.0.1/README.md
-drwxr-xr-x   0 egotrip    (501) staff       (20)        0 2021-08-15 19:20:02.089615 iode-0.0.1/iode/
--rw-r--r--   0 egotrip    (501) staff       (20)       19 2021-08-15 18:17:59.000000 iode-0.0.1/iode/__init__.py
--rw-r--r--   0 egotrip    (501) staff       (20)     5383 2021-08-15 18:58:12.000000 iode-0.0.1/iode/iode.py
-drwxr-xr-x   0 egotrip    (501) staff       (20)        0 2021-08-15 19:20:02.090740 iode-0.0.1/iode.egg-info/
--rw-r--r--   0 egotrip    (501) staff       (20)     1368 2021-08-15 19:20:02.000000 iode-0.0.1/iode.egg-info/PKG-INFO
--rw-r--r--   0 egotrip    (501) staff       (20)      241 2021-08-15 19:20:02.000000 iode-0.0.1/iode.egg-info/SOURCES.txt
--rw-r--r--   0 egotrip    (501) staff       (20)        1 2021-08-15 19:20:02.000000 iode-0.0.1/iode.egg-info/dependency_links.txt
--rw-r--r--   0 egotrip    (501) staff       (20)       41 2021-08-15 19:20:02.000000 iode-0.0.1/iode.egg-info/entry_points.txt
--rw-r--r--   0 egotrip    (501) staff       (20)        1 2021-08-15 18:18:17.000000 iode-0.0.1/iode.egg-info/not-zip-safe
--rw-r--r--   0 egotrip    (501) staff       (20)        5 2021-08-15 19:20:02.000000 iode-0.0.1/iode.egg-info/top_level.txt
--rw-r--r--   0 egotrip    (501) staff       (20)       90 2021-08-15 18:17:59.000000 iode-0.0.1/pyproject.toml
--rw-r--r--   0 egotrip    (501) staff       (20)       38 2021-08-15 19:20:02.091176 iode-0.0.1/setup.cfg
--rw-r--r--   0 egotrip    (501) staff       (20)     1319 2021-08-15 19:19:22.000000 iode-0.0.1/setup.py
+drwxr-xr-x   0 egotrip    (501) staff       (20)        0 2021-08-18 16:43:11.404718 iode-0.0.2/
+-rw-r--r--   0 egotrip    (501) staff       (20)     1060 2021-08-15 18:17:59.000000 iode-0.0.2/LICENSE
+-rw-r--r--   0 egotrip    (501) staff       (20)     1727 2021-08-18 16:43:11.404525 iode-0.0.2/PKG-INFO
+-rw-r--r--   0 egotrip    (501) staff       (20)      998 2021-08-18 16:34:19.000000 iode-0.0.2/README.md
+drwxr-xr-x   0 egotrip    (501) staff       (20)        0 2021-08-18 16:43:11.402678 iode-0.0.2/iode/
+-rw-r--r--   0 egotrip    (501) staff       (20)       19 2021-08-15 18:17:59.000000 iode-0.0.2/iode/__init__.py
+-rw-r--r--   0 egotrip    (501) staff       (20)     5373 2021-08-18 16:34:50.000000 iode-0.0.2/iode/iode.py
+drwxr-xr-x   0 egotrip    (501) staff       (20)        0 2021-08-18 16:43:11.404287 iode-0.0.2/iode.egg-info/
+-rw-r--r--   0 egotrip    (501) staff       (20)     1727 2021-08-18 16:43:11.000000 iode-0.0.2/iode.egg-info/PKG-INFO
+-rw-r--r--   0 egotrip    (501) staff       (20)      241 2021-08-18 16:43:11.000000 iode-0.0.2/iode.egg-info/SOURCES.txt
+-rw-r--r--   0 egotrip    (501) staff       (20)        1 2021-08-18 16:43:11.000000 iode-0.0.2/iode.egg-info/dependency_links.txt
+-rw-r--r--   0 egotrip    (501) staff       (20)       41 2021-08-18 16:43:11.000000 iode-0.0.2/iode.egg-info/entry_points.txt
+-rw-r--r--   0 egotrip    (501) staff       (20)        1 2021-08-18 16:43:11.000000 iode-0.0.2/iode.egg-info/not-zip-safe
+-rw-r--r--   0 egotrip    (501) staff       (20)        5 2021-08-18 16:43:11.000000 iode-0.0.2/iode.egg-info/top_level.txt
+-rw-r--r--   0 egotrip    (501) staff       (20)       90 2021-08-15 18:17:59.000000 iode-0.0.2/pyproject.toml
+-rw-r--r--   0 egotrip    (501) staff       (20)       38 2021-08-18 16:43:11.404769 iode-0.0.2/setup.cfg
+-rw-r--r--   0 egotrip    (501) staff       (20)     1319 2021-08-18 16:40:17.000000 iode-0.0.2/setup.py
```

### Comparing `iode-0.0.1/LICENSE` & `iode-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iode-0.0.1/PKG-INFO` & `iode-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iode
-Version: 0.0.1
+Version: 0.0.2
 Summary: Isolate your vscode environment and keep it simple!
 Home-page: https://github.com/jugangdae/iode
 Author: Gangdae Ju
 Author-email: jugangdae@gamil.com
 License: MIT
 Keywords: iode,manage,isolated,vscode,envoronment,simple
 Platform: UNKNOWN
@@ -15,64 +15,81 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# IODE
+# iode
+![](./resources/screenshot.png)
+
+![](./resources/iode1.png)
 
 iode is a command-line tool for simple maintenance and management of isolated vscode environments written in Python.
 
-## download
 
+## Installation
+Install from pypi
 ```
-git clone https://github.com/jugangdae/iode
-cd iode
+pip install iode --user
 ```
-
-## install
-
+Install from soruce
 ```
+git clone https://github.com/jugangdae/iode
+cd iode
 pyhton -m build
 pip install iode-0.0.1-py3-none-any.whl
 ```
 
-## config
-
-create `~/.iode/config`
-```
-$ vi ~/.iode.conf
+## Configuration
+Using the default setting, does not require a config file
 ```
-```
-[default]
 iode_run = code
-iode_dir = /Users/username/.iode
+iode_dir = ~/.iode
 ```
-create `iode_dir`
+If you want to change the settings, create `~/.iode.config`
 ```
-$ mkdir ~/.iode
+[default]
+iode_run = [code or code-insiders]
+iode_dir = [absolute path]
 ```
 
 ## usage
 
-add new iode env
+Add new iode env
 ```
 $ iode add [iode_env]
 ```
-
-delete iode env
+```
+$ iode a [iode_env]
+```
+Delete iode env
 ```
 $ iode del [iode_env]
 ```
-
-show iode env list
+```
+$ iode d [iode_env]
+```
+Show iode env list
 ```
 $ iode list
 ```
-
-run iode
+```
+$ iode l
+```
+Run iode
 ```
 $ iode run [iode_env] [path]
 ```
+```
+$ iode r [iode_env] [path]
+```
+
+Show help
+```
+iode -h
+```
+```
+iode [command] -h
+```
```

### Comparing `iode-0.0.1/iode/iode.py` & `iode-0.0.2/iode/iode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import shutil
 import argparse
 import configparser
 
-version = '0.0.1'
-# default path
+version = '0.0.2'
 
 iode = {}
 
 def listIode(args):
     global iode
     if args.iode_dir:
         if not os.path.exists(args.iode_dir):
@@ -136,39 +135,39 @@
     else:
         return -1
 
 def main():
     global iode
 
     iode['run'] = 'code'
-    iode['dir'] = os.path.join(os.path.expanduser('~'), 'iode')
+    iode['dir'] = os.path.join(os.path.expanduser('~'), '.iode')
     iode['conf'] = os.path.join(os.path.expanduser('~'), '.iode.conf')
 
     parseConfig(iode)
 
     parser = argparse.ArgumentParser()
     parser.add_argument('-v', '--version', action='version', version=f'{version}')
     subparsers = parser.add_subparsers()
 
     cmd_add = subparsers.add_parser('add', aliases=['a'], help='Add environment.')
-    cmd_add.add_argument('--iode-dir', '-d', help='set iode directory')
+    cmd_add.add_argument( '-d', '--iode-dir', help='set iode directory')
     cmd_add.add_argument('env')
     cmd_add.set_defaults(func=addIode)
 
     cmd_del = subparsers.add_parser('del', aliases=['d'], help='Delete environment.')
-    cmd_del.add_argument('--iode-dir', '-d', help='set specified root dir')
+    cmd_del.add_argument( '-d', '--iode-dir', help='set specified root dir')
     cmd_del.add_argument('env')
     cmd_del.set_defaults(func=delIode)
 
     cmd_list = subparsers.add_parser('list', aliases=['l'], help='Show environment list.')
-    cmd_list.add_argument('--iode-dir', '-d', help='set specified root dir')
+    cmd_list.add_argument( '-d', '--iode-dir', help='set specified root dir')
     cmd_list.set_defaults(func=listIode)
 
     cmd_run = subparsers.add_parser('run', aliases=['r'], help='run vscode with iode.')
-    cmd_run.add_argument('--iode-dir', '-d', help='set specified root dir')
+    cmd_run.add_argument( '-d', '--iode-dir', help='set specified root dir')
     cmd_run.add_argument('env')
     cmd_run.add_argument('path')
     cmd_run.set_defaults(func=runIode)
     
     args = parser.parse_args()
     try:
         args.func(args)
```

### Comparing `iode-0.0.1/iode.egg-info/PKG-INFO` & `iode-0.0.2/iode.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iode
-Version: 0.0.1
+Version: 0.0.2
 Summary: Isolate your vscode environment and keep it simple!
 Home-page: https://github.com/jugangdae/iode
 Author: Gangdae Ju
 Author-email: jugangdae@gamil.com
 License: MIT
 Keywords: iode,manage,isolated,vscode,envoronment,simple
 Platform: UNKNOWN
@@ -15,64 +15,81 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# IODE
+# iode
+![](./resources/screenshot.png)
+
+![](./resources/iode1.png)
 
 iode is a command-line tool for simple maintenance and management of isolated vscode environments written in Python.
 
-## download
 
+## Installation
+Install from pypi
 ```
-git clone https://github.com/jugangdae/iode
-cd iode
+pip install iode --user
 ```
-
-## install
-
+Install from soruce
 ```
+git clone https://github.com/jugangdae/iode
+cd iode
 pyhton -m build
 pip install iode-0.0.1-py3-none-any.whl
 ```
 
-## config
-
-create `~/.iode/config`
-```
-$ vi ~/.iode.conf
+## Configuration
+Using the default setting, does not require a config file
 ```
-```
-[default]
 iode_run = code
-iode_dir = /Users/username/.iode
+iode_dir = ~/.iode
 ```
-create `iode_dir`
+If you want to change the settings, create `~/.iode.config`
 ```
-$ mkdir ~/.iode
+[default]
+iode_run = [code or code-insiders]
+iode_dir = [absolute path]
 ```
 
 ## usage
 
-add new iode env
+Add new iode env
 ```
 $ iode add [iode_env]
 ```
-
-delete iode env
+```
+$ iode a [iode_env]
+```
+Delete iode env
 ```
 $ iode del [iode_env]
 ```
-
-show iode env list
+```
+$ iode d [iode_env]
+```
+Show iode env list
 ```
 $ iode list
 ```
-
-run iode
+```
+$ iode l
+```
+Run iode
 ```
 $ iode run [iode_env] [path]
 ```
+```
+$ iode r [iode_env] [path]
+```
+
+Show help
+```
+iode -h
+```
+```
+iode [command] -h
+```
```

### Comparing `iode-0.0.1/setup.py` & `iode-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name                = 'iode',
-    version             = '0.0.1',
+    version             = '0.0.2',
     description         = 'Isolate your vscode environment and keep it simple!',
     long_description    = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     author              = 'Gangdae Ju',
     author_email        = 'jugangdae@gamil.com',
     license             = 'MIT',
     url                 = 'https://github.com/jugangdae/iode',
```

