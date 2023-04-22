# Comparing `tmp/gedcomx-v1-1.0.8.tar.gz` & `tmp/gedcomx-v1-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gedcomx-v1-1.0.8.tar", last modified: Sat Apr  8 13:56:12 2023, max compression
+gzip compressed data, was "gedcomx-v1-1.0.9.tar", last modified: Sat Apr 22 14:50:30 2023, max compression
```

## Comparing `gedcomx-v1-1.0.8.tar` & `gedcomx-v1-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jean      (1001) famille    (501)        0 2023-04-08 13:56:12.096782 gedcomx-v1-1.0.8/
--rw-r--r--   0 jean      (1001) famille    (501)    35149 2022-11-27 20:59:23.000000 gedcomx-v1-1.0.8/LICENSE
--rw-r--r--   0 jean      (1001) famille    (501)     1833 2023-04-08 13:56:12.096782 gedcomx-v1-1.0.8/PKG-INFO
--rw-r--r--   0 jean      (1001) famille    (501)     1258 2022-11-28 11:40:31.000000 gedcomx-v1-1.0.8/README.md
-drwxr-xr-x   0 jean      (1001) famille    (501)        0 2023-04-08 13:56:12.092782 gedcomx-v1-1.0.8/gedcomx/
--rw-r--r--   0 jean      (1001) famille    (501)      144 2023-01-01 20:40:41.000000 gedcomx-v1-1.0.8/gedcomx/__init__.py
--rw-r--r--   0 jean      (1001) famille    (501)     1429 2022-11-27 21:00:02.000000 gedcomx-v1-1.0.8/gedcomx/_utila.py
--rw-r--r--   0 jean      (1001) famille    (501)     4475 2023-01-27 22:29:59.000000 gedcomx-v1-1.0.8/gedcomx/dateformal.py
--rw-r--r--   0 jean      (1001) famille    (501)    11619 2023-04-08 13:53:26.000000 gedcomx-v1-1.0.8/gedcomx/fs_session.py
--rw-r--r--   0 jean      (1001) famille    (501)    13936 2023-01-19 16:16:37.000000 gedcomx-v1-1.0.8/gedcomx/gedcomx.py
--rw-r--r--   0 jean      (1001) famille    (501)     5851 2023-01-21 16:39:19.000000 gedcomx-v1-1.0.8/gedcomx/json.py
--rw-r--r--   0 jean      (1001) famille    (501)    10275 2023-01-21 16:37:50.000000 gedcomx-v1-1.0.8/gedcomx/xml.py
-drwxr-xr-x   0 jean      (1001) famille    (501)        0 2023-04-08 13:56:12.096782 gedcomx-v1-1.0.8/gedcomx_v1.egg-info/
--rw-r--r--   0 jean      (1001) famille    (501)     1833 2023-04-08 13:56:12.000000 gedcomx-v1-1.0.8/gedcomx_v1.egg-info/PKG-INFO
--rw-r--r--   0 jean      (1001) famille    (501)      343 2023-04-08 13:56:12.000000 gedcomx-v1-1.0.8/gedcomx_v1.egg-info/SOURCES.txt
--rw-r--r--   0 jean      (1001) famille    (501)        1 2023-04-08 13:56:12.000000 gedcomx-v1-1.0.8/gedcomx_v1.egg-info/dependency_links.txt
--rw-r--r--   0 jean      (1001) famille    (501)        9 2023-04-08 13:56:12.000000 gedcomx-v1-1.0.8/gedcomx_v1.egg-info/requires.txt
--rw-r--r--   0 jean      (1001) famille    (501)        8 2023-04-08 13:56:12.000000 gedcomx-v1-1.0.8/gedcomx_v1.egg-info/top_level.txt
--rw-r--r--   0 jean      (1001) famille    (501)      104 2022-11-27 16:32:40.000000 gedcomx-v1-1.0.8/pyproject.toml
--rw-r--r--   0 jean      (1001) famille    (501)      838 2023-04-08 13:56:12.096782 gedcomx-v1-1.0.8/setup.cfg
+drwxr-xr-x   0 jean      (1001) famille    (501)        0 2023-04-22 14:50:30.873655 gedcomx-v1-1.0.9/
+-rw-r--r--   0 jean      (1001) famille    (501)    35149 2022-11-27 20:59:23.000000 gedcomx-v1-1.0.9/LICENSE
+-rw-r--r--   0 jean      (1001) famille    (501)     1833 2023-04-22 14:50:30.873655 gedcomx-v1-1.0.9/PKG-INFO
+-rw-r--r--   0 jean      (1001) famille    (501)     1258 2022-11-28 11:40:31.000000 gedcomx-v1-1.0.9/README.md
+drwxr-xr-x   0 jean      (1001) famille    (501)        0 2023-04-22 14:50:30.869655 gedcomx-v1-1.0.9/gedcomx/
+-rw-r--r--   0 jean      (1001) famille    (501)      144 2023-01-01 20:40:41.000000 gedcomx-v1-1.0.9/gedcomx/__init__.py
+-rw-r--r--   0 jean      (1001) famille    (501)     1429 2022-11-27 21:00:02.000000 gedcomx-v1-1.0.9/gedcomx/_utila.py
+-rw-r--r--   0 jean      (1001) famille    (501)     4475 2023-01-27 22:29:59.000000 gedcomx-v1-1.0.9/gedcomx/dateformal.py
+-rw-r--r--   0 jean      (1001) famille    (501)    11868 2023-04-22 12:49:48.000000 gedcomx-v1-1.0.9/gedcomx/fs_session.py
+-rw-r--r--   0 jean      (1001) famille    (501)    13936 2023-01-19 16:16:37.000000 gedcomx-v1-1.0.9/gedcomx/gedcomx.py
+-rw-r--r--   0 jean      (1001) famille    (501)     5851 2023-01-21 16:39:19.000000 gedcomx-v1-1.0.9/gedcomx/json.py
+-rw-r--r--   0 jean      (1001) famille    (501)    10275 2023-01-21 16:37:50.000000 gedcomx-v1-1.0.9/gedcomx/xml.py
+drwxr-xr-x   0 jean      (1001) famille    (501)        0 2023-04-22 14:50:30.873655 gedcomx-v1-1.0.9/gedcomx_v1.egg-info/
+-rw-r--r--   0 jean      (1001) famille    (501)     1833 2023-04-22 14:50:30.000000 gedcomx-v1-1.0.9/gedcomx_v1.egg-info/PKG-INFO
+-rw-r--r--   0 jean      (1001) famille    (501)      343 2023-04-22 14:50:30.000000 gedcomx-v1-1.0.9/gedcomx_v1.egg-info/SOURCES.txt
+-rw-r--r--   0 jean      (1001) famille    (501)        1 2023-04-22 14:50:30.000000 gedcomx-v1-1.0.9/gedcomx_v1.egg-info/dependency_links.txt
+-rw-r--r--   0 jean      (1001) famille    (501)        9 2023-04-22 14:50:30.000000 gedcomx-v1-1.0.9/gedcomx_v1.egg-info/requires.txt
+-rw-r--r--   0 jean      (1001) famille    (501)        8 2023-04-22 14:50:30.000000 gedcomx-v1-1.0.9/gedcomx_v1.egg-info/top_level.txt
+-rw-r--r--   0 jean      (1001) famille    (501)      104 2022-11-27 16:32:40.000000 gedcomx-v1-1.0.9/pyproject.toml
+-rw-r--r--   0 jean      (1001) famille    (501)      838 2023-04-22 14:50:30.873655 gedcomx-v1-1.0.9/setup.cfg
```

### Comparing `gedcomx-v1-1.0.8/LICENSE` & `gedcomx-v1-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gedcomx-v1-1.0.8/PKG-INFO` & `gedcomx-v1-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gedcomx-v1
-Version: 1.0.8
+Version: 1.0.9
 Summary: gedcomx-v1
 Home-page: https://github.com/jmichault/gedcomx
 Author: Jean Michault
 Author-email: author@example.com
 License: GNU General Public License v3.0
 Project-URL: Bug Tracker, https://github.com/jmichault/gedcomx/issues
 Keywords: genealogio,gedcomx
```

### Comparing `gedcomx-v1-1.0.8/README.md` & `gedcomx-v1-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gedcomx-v1-1.0.8/gedcomx/_utila.py` & `gedcomx-v1-1.0.9/gedcomx/_utila.py`

 * *Files identical despite different names*

### Comparing `gedcomx-v1-1.0.8/gedcomx/dateformal.py` & `gedcomx-v1-1.0.9/gedcomx/dateformal.py`

 * *Files identical despite different names*

### Comparing `gedcomx-v1-1.0.8/gedcomx/fs_session.py` & `gedcomx-v1-1.0.9/gedcomx/fs_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # global imports
 import sys
 import time
 
 import requests
 
+STATO_INIT = 0
+STATO_KONEKTITA = 1
+STATO_PASVORTA_ERARO = -1
+STATO_ERARO = -2
+
 
 class FsSession:
     """Create a FamilySearch session
     :param username and password: valid FamilySearch credentials
     :param verbose: True to active verbose mode
     :param logfile: a file object or similar
     :param timeout: time before retry a request
@@ -18,14 +23,15 @@
         self.password = password
         self.verbose = verbose
         self.logfile = logfile
         self.timeout = timeout
         self.fid = self.display_name = None
         self.counter = 0
         self.lingvo = lingvo
+        self.stato = STATO_INIT
         self.logged = self.login()
 
     def write_log(self, text):
         """write text in the log file"""
         log = "[%s]: %s\n" % (time.strftime("%Y-%m-%d %H:%M:%S"), text)
         if self.verbose:
             sys.stderr.write(log)
@@ -36,14 +42,15 @@
         """retrieve FamilySearch session ID
         (https://www.familysearch.org/developers/docs/guides/oauth2)
         """
         nbtry = 1
         while True:
             try:
                 if nbtry > 3 :
+                  self.stato = STATO_ERARO
                   return False
                 nbtry = nbtry + 1
                 url = "https://www.familysearch.org/auth/familysearch/login"
                 headers = {'User-Agent':'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/106.0.0.0 Safari/537.36'}
                 #headers ["Accept-Language"] = self.lingvo
                 self.write_log("Downloading : " + url)
                 r = requests.get(url, params={"ldsauth": False}, allow_redirects=False, headers=headers)
@@ -64,14 +71,15 @@
                         "password": self.password,
                     },
                     allow_redirects=False,headers=headers,
                 )
 
                 if "The username or password was incorrect" in r.text:
                     self.write_log("The username or password was incorrect")
+                    self.stato = STATO_PASVORTA_ERARO
                     return False
 
                 if "Invalid Oauth2 Request" in r.text:
                     self.write_log("Invalid Oauth2 Request")
                     time.sleep(self.timeout)
                     continue
 
@@ -97,14 +105,15 @@
                 continue
             except ValueError:
                 self.write_log("ValueError")
                 time.sleep(self.timeout)
                 continue
             self.write_log("FamilySearch session id: " + self.fssessionid)
             self.set_current()
+            self.stato = STATO_KONEKTITA
             return True
 
     def post_url(self, url, datumoj, headers=None):
         if headers is None:
             headers = {"Accept": "application/x-gedcomx-v1+json","Content-Type": "application/x-gedcomx-v1+json"}
         headers.update( {'User-Agent':'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/106.0.0.0 Safari/537.36'})
         while True:
```

### Comparing `gedcomx-v1-1.0.8/gedcomx/gedcomx.py` & `gedcomx-v1-1.0.9/gedcomx/gedcomx.py`

 * *Files identical despite different names*

### Comparing `gedcomx-v1-1.0.8/gedcomx/json.py` & `gedcomx-v1-1.0.9/gedcomx/json.py`

 * *Files identical despite different names*

### Comparing `gedcomx-v1-1.0.8/gedcomx/xml.py` & `gedcomx-v1-1.0.9/gedcomx/xml.py`

 * *Files identical despite different names*

### Comparing `gedcomx-v1-1.0.8/gedcomx_v1.egg-info/PKG-INFO` & `gedcomx-v1-1.0.9/gedcomx_v1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gedcomx-v1
-Version: 1.0.8
+Version: 1.0.9
 Summary: gedcomx-v1
 Home-page: https://github.com/jmichault/gedcomx
 Author: Jean Michault
 Author-email: author@example.com
 License: GNU General Public License v3.0
 Project-URL: Bug Tracker, https://github.com/jmichault/gedcomx/issues
 Keywords: genealogio,gedcomx
```

### Comparing `gedcomx-v1-1.0.8/setup.cfg` & `gedcomx-v1-1.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gedcomx-v1
-version = 1.0.8
+version = 1.0.9
 author = Jean Michault
 author_email = author@example.com
 description = gedcomx-v1
 url = https://github.com/jmichault/gedcomx
 keywords = genealogio, gedcomx
 project_urls = 
 	Bug Tracker = https://github.com/jmichault/gedcomx/issues
```

