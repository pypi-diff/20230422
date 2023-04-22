# Comparing `tmp/esprepomanager-1.2.2.tar.gz` & `tmp/esprepomanager-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esprepomanager-1.2.2.tar", last modified: Sat Apr 22 11:49:37 2023, max compression
+gzip compressed data, was "esprepomanager-1.2.3.tar", last modified: Sat Apr 22 12:06:00 2023, max compression
```

## Comparing `esprepomanager-1.2.2.tar` & `esprepomanager-1.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 11:49:37.675037 esprepomanager-1.2.2/
--rw-r--r--   0 tobias    (1012) familie    (155)    35149 2023-04-11 14:23:15.000000 esprepomanager-1.2.2/LICENSE
--rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 11:49:37.675037 esprepomanager-1.2.2/PKG-INFO
--rw-r--r--   0 tobias    (1012) familie    (155)      127 2023-04-14 20:13:12.000000 esprepomanager-1.2.2/README.md
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 11:49:37.675037 esprepomanager-1.2.2/esprepomanager/
--rw-rw-r--   0 tobias    (1012) familie    (155)    13694 2023-04-22 11:31:57.000000 esprepomanager-1.2.2/esprepomanager/__init__.py
--rw-r--r--   0 tobias    (1012) familie    (155)      146 2023-04-11 14:32:23.000000 esprepomanager-1.2.2/esprepomanager/__main__.py
--rw-rw-r--   0 tobias    (1012) familie    (155)    10879 2023-04-22 11:18:34.000000 esprepomanager-1.2.2/esprepomanager/config.py
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 11:49:37.675037 esprepomanager-1.2.2/esprepomanager/gitlab/
--rw-rw-r--   0 tobias    (1012) familie    (155)     6495 2023-04-22 10:13:08.000000 esprepomanager-1.2.2/esprepomanager/gitlab/__init__.py
--rw-r--r--   0 tobias    (1012) familie    (155)     1915 2023-04-14 16:46:47.000000 esprepomanager-1.2.2/esprepomanager/gitlab/group.py
--rw-rw-r--   0 tobias    (1012) familie    (155)     7605 2023-04-22 11:49:28.000000 esprepomanager-1.2.2/esprepomanager/gitlab/project.py
--rw-r--r--   0 tobias    (1012) familie    (155)      439 2023-04-13 01:24:15.000000 esprepomanager-1.2.2/esprepomanager/gitlab/user.py
--rw-r--r--   0 tobias    (1012) familie    (155)     1850 2023-04-13 22:10:58.000000 esprepomanager-1.2.2/esprepomanager/person.py
--rw-r--r--   0 tobias    (1012) familie    (155)      678 2023-04-12 20:47:34.000000 esprepomanager-1.2.2/esprepomanager/repo.py
--rw-rw-r--   0 tobias    (1012) familie    (155)     1828 2023-04-22 11:18:34.000000 esprepomanager-1.2.2/esprepomanager/team.py
--rw-rw-r--   0 tobias    (1012) familie    (155)     3928 2023-04-22 11:18:34.000000 esprepomanager-1.2.2/esprepomanager/utils.py
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 11:49:37.675037 esprepomanager-1.2.2/esprepomanager.egg-info/
--rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 11:49:37.000000 esprepomanager-1.2.2/esprepomanager.egg-info/PKG-INFO
--rw-rw-r--   0 tobias    (1012) familie    (155)      558 2023-04-22 11:49:37.000000 esprepomanager-1.2.2/esprepomanager.egg-info/SOURCES.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)        1 2023-04-22 11:49:37.000000 esprepomanager-1.2.2/esprepomanager.egg-info/dependency_links.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       55 2023-04-22 11:49:37.000000 esprepomanager-1.2.2/esprepomanager.egg-info/entry_points.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       14 2023-04-22 11:49:37.000000 esprepomanager-1.2.2/esprepomanager.egg-info/requires.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       15 2023-04-22 11:49:37.000000 esprepomanager-1.2.2/esprepomanager.egg-info/top_level.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       38 2023-04-22 11:49:37.675037 esprepomanager-1.2.2/setup.cfg
--rw-rw-r--   0 tobias    (1012) familie    (155)      768 2023-04-22 11:49:28.000000 esprepomanager-1.2.2/setup.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 12:06:00.466123 esprepomanager-1.2.3/
+-rw-r--r--   0 tobias    (1012) familie    (155)    35149 2023-04-11 14:23:15.000000 esprepomanager-1.2.3/LICENSE
+-rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 12:06:00.466123 esprepomanager-1.2.3/PKG-INFO
+-rw-r--r--   0 tobias    (1012) familie    (155)      127 2023-04-14 20:13:12.000000 esprepomanager-1.2.3/README.md
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 12:06:00.466123 esprepomanager-1.2.3/esprepomanager/
+-rw-rw-r--   0 tobias    (1012) familie    (155)    13694 2023-04-22 11:31:57.000000 esprepomanager-1.2.3/esprepomanager/__init__.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      146 2023-04-11 14:32:23.000000 esprepomanager-1.2.3/esprepomanager/__main__.py
+-rw-rw-r--   0 tobias    (1012) familie    (155)    10879 2023-04-22 11:18:34.000000 esprepomanager-1.2.3/esprepomanager/config.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 12:06:00.466123 esprepomanager-1.2.3/esprepomanager/gitlab/
+-rw-rw-r--   0 tobias    (1012) familie    (155)     6495 2023-04-22 10:13:08.000000 esprepomanager-1.2.3/esprepomanager/gitlab/__init__.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1915 2023-04-14 16:46:47.000000 esprepomanager-1.2.3/esprepomanager/gitlab/group.py
+-rw-rw-r--   0 tobias    (1012) familie    (155)     7744 2023-04-22 12:05:52.000000 esprepomanager-1.2.3/esprepomanager/gitlab/project.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      439 2023-04-13 01:24:15.000000 esprepomanager-1.2.3/esprepomanager/gitlab/user.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1850 2023-04-13 22:10:58.000000 esprepomanager-1.2.3/esprepomanager/person.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      678 2023-04-12 20:47:34.000000 esprepomanager-1.2.3/esprepomanager/repo.py
+-rw-rw-r--   0 tobias    (1012) familie    (155)     1828 2023-04-22 11:18:34.000000 esprepomanager-1.2.3/esprepomanager/team.py
+-rw-rw-r--   0 tobias    (1012) familie    (155)     3928 2023-04-22 11:18:34.000000 esprepomanager-1.2.3/esprepomanager/utils.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 12:06:00.466123 esprepomanager-1.2.3/esprepomanager.egg-info/
+-rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 12:06:00.000000 esprepomanager-1.2.3/esprepomanager.egg-info/PKG-INFO
+-rw-rw-r--   0 tobias    (1012) familie    (155)      558 2023-04-22 12:06:00.000000 esprepomanager-1.2.3/esprepomanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)        1 2023-04-22 12:06:00.000000 esprepomanager-1.2.3/esprepomanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       55 2023-04-22 12:06:00.000000 esprepomanager-1.2.3/esprepomanager.egg-info/entry_points.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       14 2023-04-22 12:06:00.000000 esprepomanager-1.2.3/esprepomanager.egg-info/requires.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       15 2023-04-22 12:06:00.000000 esprepomanager-1.2.3/esprepomanager.egg-info/top_level.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       38 2023-04-22 12:06:00.466123 esprepomanager-1.2.3/setup.cfg
+-rw-rw-r--   0 tobias    (1012) familie    (155)      768 2023-04-22 12:05:52.000000 esprepomanager-1.2.3/setup.py
```

### Comparing `esprepomanager-1.2.2/LICENSE` & `esprepomanager-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.2/PKG-INFO` & `esprepomanager-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esprepomanager
-Version: 1.2.2
+Version: 1.2.3
 Summary: manager for git repos
 Home-page: https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager
 Author: Teichi
 Author-email: tobias@teichmann.top
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `esprepomanager-1.2.2/esprepomanager/__init__.py` & `esprepomanager-1.2.3/esprepomanager/__init__.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.2/esprepomanager/config.py` & `esprepomanager-1.2.3/esprepomanager/config.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.2/esprepomanager/gitlab/__init__.py` & `esprepomanager-1.2.3/esprepomanager/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.2/esprepomanager/gitlab/group.py` & `esprepomanager-1.2.3/esprepomanager/gitlab/group.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.2/esprepomanager/gitlab/project.py` & `esprepomanager-1.2.3/esprepomanager/gitlab/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,19 +130,20 @@
                 "POST", "fork", params_={
                     "name": name, "path": name, "namespace_id": str(namespace_id), "visibility": visibility_
                 }
             )
             j_resp = resp.json()
             log.debug(j_resp)
             is_ok = resp.ok
-            if j_resp['message']['path'] == 'has already been taken':
+            if j_resp['message']['path'][0] == 'has already been taken':
                 rresp = self.gitlab.search(name, "projects")
                 for proj in rresp:
                     if proj["name"] == name:
                         j_resp["id"] = proj["id"]
+                        j_resp["web_url"] = proj["web_url"]
                         is_ok = True
                         break
             if is_ok:
                 pid = int(j_resp["id"])
                 web_url = j_resp["web_url"]
                 time.sleep(1)
                 if not tree or self.gitlab.project(pid).tree(recursive=True) == tree:
@@ -166,17 +167,18 @@
             return True
 
         for _ in range(max_tries):
             resp = self.send_request(
                 "POST", "members", params_={"user_id": ids, "access_level": str(access_level_)}
             )
 
-            if resp.ok:
+            j_resp = resp.json()
+            if resp.ok or j_resp['message'] == 'Member already exists':
                 return True
-            log.debug(resp.json())
+            log.debug(j_resp)
             time.sleep(1)
         return False
 
     def create(
         self, name: str, namespace_id: int, members: 'Optional[List[Person]]' = None,
         max_tries: int = 3
     ) -> 'Literal[False] | Tuple[str, int]':
```

### Comparing `esprepomanager-1.2.2/esprepomanager/person.py` & `esprepomanager-1.2.3/esprepomanager/person.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.2/esprepomanager/repo.py` & `esprepomanager-1.2.3/esprepomanager/repo.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.2/esprepomanager/team.py` & `esprepomanager-1.2.3/esprepomanager/team.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.2/esprepomanager/utils.py` & `esprepomanager-1.2.3/esprepomanager/utils.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.2/esprepomanager.egg-info/PKG-INFO` & `esprepomanager-1.2.3/esprepomanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esprepomanager
-Version: 1.2.2
+Version: 1.2.3
 Summary: manager for git repos
 Home-page: https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager
 Author: Teichi
 Author-email: tobias@teichmann.top
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `esprepomanager-1.2.2/esprepomanager.egg-info/SOURCES.txt` & `esprepomanager-1.2.3/esprepomanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.2/setup.py` & `esprepomanager-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="esprepomanager",
-    version="1.2.2",
+    version="1.2.3",
     author="Teichi",
     author_email="tobias@teichmann.top",
     description="manager for git repos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager",
     packages=setuptools.find_packages(),
```

