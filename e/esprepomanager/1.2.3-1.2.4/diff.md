# Comparing `tmp/esprepomanager-1.2.3.tar.gz` & `tmp/esprepomanager-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esprepomanager-1.2.3.tar", last modified: Sat Apr 22 12:06:00 2023, max compression
+gzip compressed data, was "esprepomanager-1.2.4.tar", last modified: Sat Apr 22 13:01:48 2023, max compression
```

## Comparing `esprepomanager-1.2.3.tar` & `esprepomanager-1.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 12:06:00.466123 esprepomanager-1.2.3/
--rw-r--r--   0 tobias    (1012) familie    (155)    35149 2023-04-11 14:23:15.000000 esprepomanager-1.2.3/LICENSE
--rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 12:06:00.466123 esprepomanager-1.2.3/PKG-INFO
--rw-r--r--   0 tobias    (1012) familie    (155)      127 2023-04-14 20:13:12.000000 esprepomanager-1.2.3/README.md
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 12:06:00.466123 esprepomanager-1.2.3/esprepomanager/
--rw-rw-r--   0 tobias    (1012) familie    (155)    13694 2023-04-22 11:31:57.000000 esprepomanager-1.2.3/esprepomanager/__init__.py
--rw-r--r--   0 tobias    (1012) familie    (155)      146 2023-04-11 14:32:23.000000 esprepomanager-1.2.3/esprepomanager/__main__.py
--rw-rw-r--   0 tobias    (1012) familie    (155)    10879 2023-04-22 11:18:34.000000 esprepomanager-1.2.3/esprepomanager/config.py
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 12:06:00.466123 esprepomanager-1.2.3/esprepomanager/gitlab/
--rw-rw-r--   0 tobias    (1012) familie    (155)     6495 2023-04-22 10:13:08.000000 esprepomanager-1.2.3/esprepomanager/gitlab/__init__.py
--rw-r--r--   0 tobias    (1012) familie    (155)     1915 2023-04-14 16:46:47.000000 esprepomanager-1.2.3/esprepomanager/gitlab/group.py
--rw-rw-r--   0 tobias    (1012) familie    (155)     7744 2023-04-22 12:05:52.000000 esprepomanager-1.2.3/esprepomanager/gitlab/project.py
--rw-r--r--   0 tobias    (1012) familie    (155)      439 2023-04-13 01:24:15.000000 esprepomanager-1.2.3/esprepomanager/gitlab/user.py
--rw-r--r--   0 tobias    (1012) familie    (155)     1850 2023-04-13 22:10:58.000000 esprepomanager-1.2.3/esprepomanager/person.py
--rw-r--r--   0 tobias    (1012) familie    (155)      678 2023-04-12 20:47:34.000000 esprepomanager-1.2.3/esprepomanager/repo.py
--rw-rw-r--   0 tobias    (1012) familie    (155)     1828 2023-04-22 11:18:34.000000 esprepomanager-1.2.3/esprepomanager/team.py
--rw-rw-r--   0 tobias    (1012) familie    (155)     3928 2023-04-22 11:18:34.000000 esprepomanager-1.2.3/esprepomanager/utils.py
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 12:06:00.466123 esprepomanager-1.2.3/esprepomanager.egg-info/
--rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 12:06:00.000000 esprepomanager-1.2.3/esprepomanager.egg-info/PKG-INFO
--rw-rw-r--   0 tobias    (1012) familie    (155)      558 2023-04-22 12:06:00.000000 esprepomanager-1.2.3/esprepomanager.egg-info/SOURCES.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)        1 2023-04-22 12:06:00.000000 esprepomanager-1.2.3/esprepomanager.egg-info/dependency_links.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       55 2023-04-22 12:06:00.000000 esprepomanager-1.2.3/esprepomanager.egg-info/entry_points.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       14 2023-04-22 12:06:00.000000 esprepomanager-1.2.3/esprepomanager.egg-info/requires.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       15 2023-04-22 12:06:00.000000 esprepomanager-1.2.3/esprepomanager.egg-info/top_level.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       38 2023-04-22 12:06:00.466123 esprepomanager-1.2.3/setup.cfg
--rw-rw-r--   0 tobias    (1012) familie    (155)      768 2023-04-22 12:05:52.000000 esprepomanager-1.2.3/setup.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 13:01:48.745155 esprepomanager-1.2.4/
+-rw-r--r--   0 tobias    (1012) familie    (155)    35149 2023-04-11 14:23:15.000000 esprepomanager-1.2.4/LICENSE
+-rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 13:01:48.745155 esprepomanager-1.2.4/PKG-INFO
+-rw-r--r--   0 tobias    (1012) familie    (155)      127 2023-04-14 20:13:12.000000 esprepomanager-1.2.4/README.md
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 13:01:48.745155 esprepomanager-1.2.4/esprepomanager/
+-rw-rw-r--   0 tobias    (1012) familie    (155)    13725 2023-04-22 13:01:44.000000 esprepomanager-1.2.4/esprepomanager/__init__.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      146 2023-04-11 14:32:23.000000 esprepomanager-1.2.4/esprepomanager/__main__.py
+-rw-rw-r--   0 tobias    (1012) familie    (155)    10879 2023-04-22 11:18:34.000000 esprepomanager-1.2.4/esprepomanager/config.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 13:01:48.745155 esprepomanager-1.2.4/esprepomanager/gitlab/
+-rw-rw-r--   0 tobias    (1012) familie    (155)     6642 2023-04-22 13:01:44.000000 esprepomanager-1.2.4/esprepomanager/gitlab/__init__.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1915 2023-04-14 16:46:47.000000 esprepomanager-1.2.4/esprepomanager/gitlab/group.py
+-rw-rw-r--   0 tobias    (1012) familie    (155)     7744 2023-04-22 12:05:52.000000 esprepomanager-1.2.4/esprepomanager/gitlab/project.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      439 2023-04-13 01:24:15.000000 esprepomanager-1.2.4/esprepomanager/gitlab/user.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1850 2023-04-13 22:10:58.000000 esprepomanager-1.2.4/esprepomanager/person.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      678 2023-04-12 20:47:34.000000 esprepomanager-1.2.4/esprepomanager/repo.py
+-rw-rw-r--   0 tobias    (1012) familie    (155)     1828 2023-04-22 11:18:34.000000 esprepomanager-1.2.4/esprepomanager/team.py
+-rw-rw-r--   0 tobias    (1012) familie    (155)     4102 2023-04-22 13:01:44.000000 esprepomanager-1.2.4/esprepomanager/utils.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 13:01:48.745155 esprepomanager-1.2.4/esprepomanager.egg-info/
+-rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 13:01:48.000000 esprepomanager-1.2.4/esprepomanager.egg-info/PKG-INFO
+-rw-rw-r--   0 tobias    (1012) familie    (155)      558 2023-04-22 13:01:48.000000 esprepomanager-1.2.4/esprepomanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)        1 2023-04-22 13:01:48.000000 esprepomanager-1.2.4/esprepomanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       55 2023-04-22 13:01:48.000000 esprepomanager-1.2.4/esprepomanager.egg-info/entry_points.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       14 2023-04-22 13:01:48.000000 esprepomanager-1.2.4/esprepomanager.egg-info/requires.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       15 2023-04-22 13:01:48.000000 esprepomanager-1.2.4/esprepomanager.egg-info/top_level.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       38 2023-04-22 13:01:48.745155 esprepomanager-1.2.4/setup.cfg
+-rw-rw-r--   0 tobias    (1012) familie    (155)      768 2023-04-22 13:01:44.000000 esprepomanager-1.2.4/setup.py
```

### Comparing `esprepomanager-1.2.3/LICENSE` & `esprepomanager-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.3/PKG-INFO` & `esprepomanager-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esprepomanager
-Version: 1.2.3
+Version: 1.2.4
 Summary: manager for git repos
 Home-page: https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager
 Author: Teichi
 Author-email: tobias@teichmann.top
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `esprepomanager-1.2.3/esprepomanager/__init__.py` & `esprepomanager-1.2.4/esprepomanager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
         t = ThreadPoolExecutor(config.git.max_threads)
         for team, val in t.map(_fork_wrapper,
                                (t for t in config.teams.values() if t.assignment == ass.name and t.persons)):
             if not val:
                 log.error(f"Failed to create repo for team {team.id}")
                 continue
-            if team.repository or isinstance(val, bool):
+            if (team.repository and team.repository.id != -1) or isinstance(val, bool):
                 continue
             web_url, pid = val
             server = web_url.split("//", 1)[1].split("/", 1)
             team.repository = Repository(server[0], server[1], pid)
 
 
 def download(args: argparse.Namespace, config: ConfigRepo) -> None:
```

### Comparing `esprepomanager-1.2.3/esprepomanager/config.py` & `esprepomanager-1.2.4/esprepomanager/config.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.3/esprepomanager/gitlab/__init__.py` & `esprepomanager-1.2.4/esprepomanager/gitlab/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,17 +92,15 @@
                 raise ex
             time.sleep(5)
             return self.send_request(method, url, data, params_, max_tries - 1)
 
     def send_requests(
         self, requests_: Iterable[Tuple[methods, str, Any, Optional[Dict[str, str]]]]
     ) -> Iterable[requests.Response]:
-        def _send_wrapper(
-            args: Tuple[methods, str, Any, Optional[Dict[str, str]]]
-        ) -> requests.Response:
+        def _send_wrapper(args: Tuple[methods, str, Any, Optional[Dict[str, str]]]) -> requests.Response:
             return self.send_request(*args)
 
         executor = ThreadPoolExecutor(max_workers=self.max_threads)
         return executor.map(_send_wrapper, requests_)
 
     def project_members(self, projects: List[int]) -> 'Dict[int, List[User]]':
         def _send_wrapper(project: int) -> 'Tuple[int, List[User]]':
@@ -114,15 +112,18 @@
         for i, users in enumerate(executor.map(_send_wrapper, projects)):
             print(f"Getting project members {(i+1):04d}/{len(projects):04d}", end="\r")
             ret[users[0]] = users[1]
         print()
         return ret
 
     def search(self, search: str, scope: Literal["projects", "users"]) -> 'List[Dict[str, str | int]]':
-        resp = self.send_request("GET", "search", params_={"scope": scope, "search": search})
+        if scope == "projects":
+            resp = self.send_request("GET", "projects", params_={"search": search, "order_by": "name", "sort": "asc"})
+        else:
+            resp = self.send_request("GET", "search", params_={"scope": scope, "search": search})
         return resp.json()
 
     def search_persons(self, users: 'List[Person]') -> None:
         def _send_wrapper(user: 'Person') -> 'Optional[Tuple[Person, List[Dict[str, str | int]]]]':
             resp = self.search(user.reverseName, "users")
             resp = [r for r in resp if user.checkGitLabName(str(r.get("name", "")))]
             if len(resp) > 1:
```

### Comparing `esprepomanager-1.2.3/esprepomanager/gitlab/group.py` & `esprepomanager-1.2.4/esprepomanager/gitlab/group.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.3/esprepomanager/gitlab/project.py` & `esprepomanager-1.2.4/esprepomanager/gitlab/project.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.3/esprepomanager/person.py` & `esprepomanager-1.2.4/esprepomanager/person.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.3/esprepomanager/repo.py` & `esprepomanager-1.2.4/esprepomanager/repo.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.3/esprepomanager/team.py` & `esprepomanager-1.2.4/esprepomanager/team.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.3/esprepomanager/utils.py` & `esprepomanager-1.2.4/esprepomanager/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,19 +58,22 @@
             save_get(lines, h_dic["GitlabUsername"], ""),
         )
         persons.append(person_)
         teams_ = Team.from_csv_line(h_dic, lines, assignments, person_)
         for team in teams_:
             if team.key is None:
                 continue
-            if team.key not in teams_:
+            if team.key not in teams:
                 teams[team.key] = team
             else:
+                repo = teams[team.key].repository
+                if (repo and repo.id == -1 and team.repository):
+                    repo.id = team.repository.id
                 teams[team.key].persons.append(person_)
-            person_.teams[team.assignment] = team
+            person_.teams[team.assignment] = teams[team.key]
 
     return (persons, teams)
 
 
 def dump_csv(config: 'ConfigRepo') -> str:
     assignments_names = []
     if config.fullconfig:
```

### Comparing `esprepomanager-1.2.3/esprepomanager.egg-info/PKG-INFO` & `esprepomanager-1.2.4/esprepomanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esprepomanager
-Version: 1.2.3
+Version: 1.2.4
 Summary: manager for git repos
 Home-page: https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager
 Author: Teichi
 Author-email: tobias@teichmann.top
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `esprepomanager-1.2.3/esprepomanager.egg-info/SOURCES.txt` & `esprepomanager-1.2.4/esprepomanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.3/setup.py` & `esprepomanager-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="esprepomanager",
-    version="1.2.3",
+    version="1.2.4",
     author="Teichi",
     author_email="tobias@teichmann.top",
     description="manager for git repos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager",
     packages=setuptools.find_packages(),
```

