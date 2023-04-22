# Comparing `tmp/esprepomanager-1.1.0.tar.gz` & `tmp/esprepomanager-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esprepomanager-1.1.0.tar", last modified: Thu Apr 20 15:27:27 2023, max compression
+gzip compressed data, was "esprepomanager-1.1.1.tar", last modified: Sat Apr 22 10:13:15 2023, max compression
```

## Comparing `esprepomanager-1.1.0.tar` & `esprepomanager-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-20 15:27:27.645192 esprepomanager-1.1.0/
--rw-r--r--   0 tobias    (1012) familie    (155)    35149 2023-04-11 14:23:15.000000 esprepomanager-1.1.0/LICENSE
--rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-20 15:27:27.641192 esprepomanager-1.1.0/PKG-INFO
--rw-r--r--   0 tobias    (1012) familie    (155)      127 2023-04-14 20:13:12.000000 esprepomanager-1.1.0/README.md
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-20 15:27:27.641192 esprepomanager-1.1.0/esprepomanager/
--rw-rw-r--   0 tobias    (1012) familie    (155)    13625 2023-04-20 15:25:44.000000 esprepomanager-1.1.0/esprepomanager/__init__.py
--rw-r--r--   0 tobias    (1012) familie    (155)      146 2023-04-11 14:32:23.000000 esprepomanager-1.1.0/esprepomanager/__main__.py
--rw-r--r--   0 tobias    (1012) familie    (155)    10644 2023-04-14 17:25:28.000000 esprepomanager-1.1.0/esprepomanager/config.py
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-20 15:27:27.641192 esprepomanager-1.1.0/esprepomanager/gitlab/
--rw-r--r--   0 tobias    (1012) familie    (155)     6496 2023-04-14 20:16:08.000000 esprepomanager-1.1.0/esprepomanager/gitlab/__init__.py
--rw-r--r--   0 tobias    (1012) familie    (155)     1915 2023-04-14 16:46:47.000000 esprepomanager-1.1.0/esprepomanager/gitlab/group.py
--rw-r--r--   0 tobias    (1012) familie    (155)     7260 2023-04-20 15:25:33.000000 esprepomanager-1.1.0/esprepomanager/gitlab/project.py
--rw-r--r--   0 tobias    (1012) familie    (155)      439 2023-04-13 01:24:15.000000 esprepomanager-1.1.0/esprepomanager/gitlab/user.py
--rw-r--r--   0 tobias    (1012) familie    (155)     1850 2023-04-13 22:10:58.000000 esprepomanager-1.1.0/esprepomanager/person.py
--rw-r--r--   0 tobias    (1012) familie    (155)      678 2023-04-12 20:47:34.000000 esprepomanager-1.1.0/esprepomanager/repo.py
--rw-r--r--   0 tobias    (1012) familie    (155)     1594 2023-04-14 15:42:33.000000 esprepomanager-1.1.0/esprepomanager/team.py
--rw-r--r--   0 tobias    (1012) familie    (155)     3887 2023-04-14 18:31:34.000000 esprepomanager-1.1.0/esprepomanager/utils.py
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-20 15:27:27.641192 esprepomanager-1.1.0/esprepomanager.egg-info/
--rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-20 15:27:27.000000 esprepomanager-1.1.0/esprepomanager.egg-info/PKG-INFO
--rw-rw-r--   0 tobias    (1012) familie    (155)      558 2023-04-20 15:27:27.000000 esprepomanager-1.1.0/esprepomanager.egg-info/SOURCES.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)        1 2023-04-20 15:27:27.000000 esprepomanager-1.1.0/esprepomanager.egg-info/dependency_links.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       55 2023-04-20 15:27:27.000000 esprepomanager-1.1.0/esprepomanager.egg-info/entry_points.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       14 2023-04-20 15:27:27.000000 esprepomanager-1.1.0/esprepomanager.egg-info/requires.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       15 2023-04-20 15:27:27.000000 esprepomanager-1.1.0/esprepomanager.egg-info/top_level.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       38 2023-04-20 15:27:27.645192 esprepomanager-1.1.0/setup.cfg
--rw-rw-r--   0 tobias    (1012) familie    (155)      768 2023-04-20 14:32:14.000000 esprepomanager-1.1.0/setup.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 10:13:15.207487 esprepomanager-1.1.1/
+-rw-r--r--   0 tobias    (1012) familie    (155)    35149 2023-04-11 14:23:15.000000 esprepomanager-1.1.1/LICENSE
+-rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 10:13:15.207487 esprepomanager-1.1.1/PKG-INFO
+-rw-r--r--   0 tobias    (1012) familie    (155)      127 2023-04-14 20:13:12.000000 esprepomanager-1.1.1/README.md
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 10:13:15.163487 esprepomanager-1.1.1/esprepomanager/
+-rw-rw-r--   0 tobias    (1012) familie    (155)    13625 2023-04-20 15:25:44.000000 esprepomanager-1.1.1/esprepomanager/__init__.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      146 2023-04-11 14:32:23.000000 esprepomanager-1.1.1/esprepomanager/__main__.py
+-rw-r--r--   0 tobias    (1012) familie    (155)    10644 2023-04-14 17:25:28.000000 esprepomanager-1.1.1/esprepomanager/config.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 10:13:15.187487 esprepomanager-1.1.1/esprepomanager/gitlab/
+-rw-rw-r--   0 tobias    (1012) familie    (155)     6495 2023-04-22 10:13:08.000000 esprepomanager-1.1.1/esprepomanager/gitlab/__init__.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1915 2023-04-14 16:46:47.000000 esprepomanager-1.1.1/esprepomanager/gitlab/group.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     7260 2023-04-20 15:25:33.000000 esprepomanager-1.1.1/esprepomanager/gitlab/project.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      439 2023-04-13 01:24:15.000000 esprepomanager-1.1.1/esprepomanager/gitlab/user.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1850 2023-04-13 22:10:58.000000 esprepomanager-1.1.1/esprepomanager/person.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      678 2023-04-12 20:47:34.000000 esprepomanager-1.1.1/esprepomanager/repo.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1594 2023-04-14 15:42:33.000000 esprepomanager-1.1.1/esprepomanager/team.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     3887 2023-04-14 18:31:34.000000 esprepomanager-1.1.1/esprepomanager/utils.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 10:13:15.175487 esprepomanager-1.1.1/esprepomanager.egg-info/
+-rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 10:13:15.000000 esprepomanager-1.1.1/esprepomanager.egg-info/PKG-INFO
+-rw-rw-r--   0 tobias    (1012) familie    (155)      558 2023-04-22 10:13:15.000000 esprepomanager-1.1.1/esprepomanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)        1 2023-04-22 10:13:15.000000 esprepomanager-1.1.1/esprepomanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       55 2023-04-22 10:13:15.000000 esprepomanager-1.1.1/esprepomanager.egg-info/entry_points.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       14 2023-04-22 10:13:15.000000 esprepomanager-1.1.1/esprepomanager.egg-info/requires.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       15 2023-04-22 10:13:15.000000 esprepomanager-1.1.1/esprepomanager.egg-info/top_level.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       38 2023-04-22 10:13:15.207487 esprepomanager-1.1.1/setup.cfg
+-rw-rw-r--   0 tobias    (1012) familie    (155)      768 2023-04-22 10:13:08.000000 esprepomanager-1.1.1/setup.py
```

### Comparing `esprepomanager-1.1.0/LICENSE` & `esprepomanager-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.1.0/PKG-INFO` & `esprepomanager-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esprepomanager
-Version: 1.1.0
+Version: 1.1.1
 Summary: manager for git repos
 Home-page: https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager
 Author: Teichi
 Author-email: tobias@teichmann.top
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `esprepomanager-1.1.0/esprepomanager/__init__.py` & `esprepomanager-1.1.1/esprepomanager/__init__.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.1.0/esprepomanager/config.py` & `esprepomanager-1.1.1/esprepomanager/config.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.1.0/esprepomanager/gitlab/__init__.py` & `esprepomanager-1.1.1/esprepomanager/gitlab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 ret = requests.get(
                     f"{self.base_url}/api/{self.api_version}/{url}",
                     params=params
                 )
             elif method == "PUT":
                 ret = requests.put(
                     f"{self.base_url}/api/{self.api_version}/{url}",
-                    json=data, params=params_
+                    json=data, params=params
                 )
             elif method == "POST":
                 ret = requests.post(
                     f"{self.base_url}/api/{self.api_version}/{url}",
                     json=data,
                     params=params
                 )
```

### Comparing `esprepomanager-1.1.0/esprepomanager/gitlab/group.py` & `esprepomanager-1.1.1/esprepomanager/gitlab/group.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.1.0/esprepomanager/gitlab/project.py` & `esprepomanager-1.1.1/esprepomanager/gitlab/project.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.1.0/esprepomanager/person.py` & `esprepomanager-1.1.1/esprepomanager/person.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.1.0/esprepomanager/repo.py` & `esprepomanager-1.1.1/esprepomanager/repo.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.1.0/esprepomanager/team.py` & `esprepomanager-1.1.1/esprepomanager/team.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.1.0/esprepomanager/utils.py` & `esprepomanager-1.1.1/esprepomanager/utils.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.1.0/esprepomanager.egg-info/PKG-INFO` & `esprepomanager-1.1.1/esprepomanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esprepomanager
-Version: 1.1.0
+Version: 1.1.1
 Summary: manager for git repos
 Home-page: https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager
 Author: Teichi
 Author-email: tobias@teichmann.top
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `esprepomanager-1.1.0/esprepomanager.egg-info/SOURCES.txt` & `esprepomanager-1.1.1/esprepomanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.1.0/setup.py` & `esprepomanager-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="esprepomanager",
-    version="1.1.0",
+    version="1.1.1",
     author="Teichi",
     author_email="tobias@teichmann.top",
     description="manager for git repos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager",
     packages=setuptools.find_packages(),
```

