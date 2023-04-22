# Comparing `tmp/esprepomanager-1.2.0.tar.gz` & `tmp/esprepomanager-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esprepomanager-1.2.0.tar", last modified: Sat Apr 22 11:18:49 2023, max compression
+gzip compressed data, was "esprepomanager-1.2.1.tar", last modified: Sat Apr 22 11:32:11 2023, max compression
```

## Comparing `esprepomanager-1.2.0.tar` & `esprepomanager-1.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 11:18:49.993553 esprepomanager-1.2.0/
--rw-r--r--   0 tobias    (1012) familie    (155)    35149 2023-04-11 14:23:15.000000 esprepomanager-1.2.0/LICENSE
--rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 11:18:49.993553 esprepomanager-1.2.0/PKG-INFO
--rw-r--r--   0 tobias    (1012) familie    (155)      127 2023-04-14 20:13:12.000000 esprepomanager-1.2.0/README.md
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 11:18:49.945668 esprepomanager-1.2.0/esprepomanager/
--rw-rw-r--   0 tobias    (1012) familie    (155)    13625 2023-04-20 15:25:44.000000 esprepomanager-1.2.0/esprepomanager/__init__.py
--rw-r--r--   0 tobias    (1012) familie    (155)      146 2023-04-11 14:32:23.000000 esprepomanager-1.2.0/esprepomanager/__main__.py
--rw-rw-r--   0 tobias    (1012) familie    (155)    10879 2023-04-22 11:18:34.000000 esprepomanager-1.2.0/esprepomanager/config.py
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 11:18:49.977591 esprepomanager-1.2.0/esprepomanager/gitlab/
--rw-rw-r--   0 tobias    (1012) familie    (155)     6495 2023-04-22 10:13:08.000000 esprepomanager-1.2.0/esprepomanager/gitlab/__init__.py
--rw-r--r--   0 tobias    (1012) familie    (155)     1915 2023-04-14 16:46:47.000000 esprepomanager-1.2.0/esprepomanager/gitlab/group.py
--rw-r--r--   0 tobias    (1012) familie    (155)     7260 2023-04-20 15:25:33.000000 esprepomanager-1.2.0/esprepomanager/gitlab/project.py
--rw-r--r--   0 tobias    (1012) familie    (155)      439 2023-04-13 01:24:15.000000 esprepomanager-1.2.0/esprepomanager/gitlab/user.py
--rw-r--r--   0 tobias    (1012) familie    (155)     1850 2023-04-13 22:10:58.000000 esprepomanager-1.2.0/esprepomanager/person.py
--rw-r--r--   0 tobias    (1012) familie    (155)      678 2023-04-12 20:47:34.000000 esprepomanager-1.2.0/esprepomanager/repo.py
--rw-rw-r--   0 tobias    (1012) familie    (155)     1828 2023-04-22 11:18:34.000000 esprepomanager-1.2.0/esprepomanager/team.py
--rw-rw-r--   0 tobias    (1012) familie    (155)     3928 2023-04-22 11:18:34.000000 esprepomanager-1.2.0/esprepomanager/utils.py
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 11:18:49.945668 esprepomanager-1.2.0/esprepomanager.egg-info/
--rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 11:18:49.000000 esprepomanager-1.2.0/esprepomanager.egg-info/PKG-INFO
--rw-rw-r--   0 tobias    (1012) familie    (155)      558 2023-04-22 11:18:49.000000 esprepomanager-1.2.0/esprepomanager.egg-info/SOURCES.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)        1 2023-04-22 11:18:49.000000 esprepomanager-1.2.0/esprepomanager.egg-info/dependency_links.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       55 2023-04-22 11:18:49.000000 esprepomanager-1.2.0/esprepomanager.egg-info/entry_points.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       14 2023-04-22 11:18:49.000000 esprepomanager-1.2.0/esprepomanager.egg-info/requires.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       15 2023-04-22 11:18:49.000000 esprepomanager-1.2.0/esprepomanager.egg-info/top_level.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       38 2023-04-22 11:18:49.993553 esprepomanager-1.2.0/setup.cfg
--rw-rw-r--   0 tobias    (1012) familie    (155)      768 2023-04-22 11:18:34.000000 esprepomanager-1.2.0/setup.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 11:32:11.978237 esprepomanager-1.2.1/
+-rw-r--r--   0 tobias    (1012) familie    (155)    35149 2023-04-11 14:23:15.000000 esprepomanager-1.2.1/LICENSE
+-rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 11:32:11.974245 esprepomanager-1.2.1/PKG-INFO
+-rw-r--r--   0 tobias    (1012) familie    (155)      127 2023-04-14 20:13:12.000000 esprepomanager-1.2.1/README.md
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 11:32:11.786652 esprepomanager-1.2.1/esprepomanager/
+-rw-rw-r--   0 tobias    (1012) familie    (155)    13694 2023-04-22 11:31:57.000000 esprepomanager-1.2.1/esprepomanager/__init__.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      146 2023-04-11 14:32:23.000000 esprepomanager-1.2.1/esprepomanager/__main__.py
+-rw-rw-r--   0 tobias    (1012) familie    (155)    10879 2023-04-22 11:18:34.000000 esprepomanager-1.2.1/esprepomanager/config.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 11:32:11.954289 esprepomanager-1.2.1/esprepomanager/gitlab/
+-rw-rw-r--   0 tobias    (1012) familie    (155)     6495 2023-04-22 10:13:08.000000 esprepomanager-1.2.1/esprepomanager/gitlab/__init__.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1915 2023-04-14 16:46:47.000000 esprepomanager-1.2.1/esprepomanager/gitlab/group.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     7260 2023-04-20 15:25:33.000000 esprepomanager-1.2.1/esprepomanager/gitlab/project.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      439 2023-04-13 01:24:15.000000 esprepomanager-1.2.1/esprepomanager/gitlab/user.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1850 2023-04-13 22:10:58.000000 esprepomanager-1.2.1/esprepomanager/person.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      678 2023-04-12 20:47:34.000000 esprepomanager-1.2.1/esprepomanager/repo.py
+-rw-rw-r--   0 tobias    (1012) familie    (155)     1828 2023-04-22 11:18:34.000000 esprepomanager-1.2.1/esprepomanager/team.py
+-rw-rw-r--   0 tobias    (1012) familie    (155)     3928 2023-04-22 11:18:34.000000 esprepomanager-1.2.1/esprepomanager/utils.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 11:32:11.786652 esprepomanager-1.2.1/esprepomanager.egg-info/
+-rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 11:32:11.000000 esprepomanager-1.2.1/esprepomanager.egg-info/PKG-INFO
+-rw-rw-r--   0 tobias    (1012) familie    (155)      558 2023-04-22 11:32:11.000000 esprepomanager-1.2.1/esprepomanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)        1 2023-04-22 11:32:11.000000 esprepomanager-1.2.1/esprepomanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       55 2023-04-22 11:32:11.000000 esprepomanager-1.2.1/esprepomanager.egg-info/entry_points.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       14 2023-04-22 11:32:11.000000 esprepomanager-1.2.1/esprepomanager.egg-info/requires.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       15 2023-04-22 11:32:11.000000 esprepomanager-1.2.1/esprepomanager.egg-info/top_level.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       38 2023-04-22 11:32:11.978237 esprepomanager-1.2.1/setup.cfg
+-rw-rw-r--   0 tobias    (1012) familie    (155)      768 2023-04-22 11:31:57.000000 esprepomanager-1.2.1/setup.py
```

### Comparing `esprepomanager-1.2.0/LICENSE` & `esprepomanager-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.0/PKG-INFO` & `esprepomanager-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esprepomanager
-Version: 1.2.0
+Version: 1.2.1
 Summary: manager for git repos
 Home-page: https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager
 Author: Teichi
 Author-email: tobias@teichmann.top
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `esprepomanager-1.2.0/esprepomanager/__init__.py` & `esprepomanager-1.2.1/esprepomanager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,17 @@
         config.branch = args.configbranch
     if args.dryrun:
         config.dryrun = args.dryrun
     config.ensure_fullconfig(args.fullconfig)
     config.ensure_database(args.database)
     config.fullconfig.get_group_info(config)  # type: ignore
 
+    if args.import_ or args.createrepos:
+        args.update = True
+
     for ass in config.fullconfig.assignments.values():  # type: ignore
         log.log(25, f"Getting upstream repository for assignment {ass.name}")
         ass.get_upstream_repo(config)
 
     return config
```

### Comparing `esprepomanager-1.2.0/esprepomanager/config.py` & `esprepomanager-1.2.1/esprepomanager/config.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.0/esprepomanager/gitlab/__init__.py` & `esprepomanager-1.2.1/esprepomanager/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.0/esprepomanager/gitlab/group.py` & `esprepomanager-1.2.1/esprepomanager/gitlab/group.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.0/esprepomanager/gitlab/project.py` & `esprepomanager-1.2.1/esprepomanager/gitlab/project.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.0/esprepomanager/person.py` & `esprepomanager-1.2.1/esprepomanager/person.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.0/esprepomanager/repo.py` & `esprepomanager-1.2.1/esprepomanager/repo.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.0/esprepomanager/team.py` & `esprepomanager-1.2.1/esprepomanager/team.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.0/esprepomanager/utils.py` & `esprepomanager-1.2.1/esprepomanager/utils.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.0/esprepomanager.egg-info/PKG-INFO` & `esprepomanager-1.2.1/esprepomanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esprepomanager
-Version: 1.2.0
+Version: 1.2.1
 Summary: manager for git repos
 Home-page: https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager
 Author: Teichi
 Author-email: tobias@teichmann.top
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `esprepomanager-1.2.0/esprepomanager.egg-info/SOURCES.txt` & `esprepomanager-1.2.1/esprepomanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.0/setup.py` & `esprepomanager-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="esprepomanager",
-    version="1.2.0",
+    version="1.2.1",
     author="Teichi",
     author_email="tobias@teichmann.top",
     description="manager for git repos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager",
     packages=setuptools.find_packages(),
```

