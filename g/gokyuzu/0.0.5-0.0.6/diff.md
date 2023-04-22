# Comparing `tmp/gokyuzu-0.0.5.tar.gz` & `tmp/gokyuzu-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gokyuzu-0.0.5.tar", last modified: Sat Apr 22 17:00:57 2023, max compression
+gzip compressed data, was "gokyuzu-0.0.6.tar", last modified: Sat Apr 22 17:10:26 2023, max compression
```

## Comparing `gokyuzu-0.0.5.tar` & `gokyuzu-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:00:57.679827 gokyuzu-0.0.5/
--rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-0.0.5/LICENSE
--rw-r--r--   0 kilic      (501) staff       (20)     1563 2023-04-22 17:00:57.679715 gokyuzu-0.0.5/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      787 2023-04-22 15:30:32.000000 gokyuzu-0.0.5/README.md
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:00:57.678492 gokyuzu-0.0.5/gokyuzu/
--rw-r--r--   0 kilic      (501) staff       (20)     1289 2023-04-22 17:00:00.000000 gokyuzu-0.0.5/gokyuzu/BlueskyEndpoints.py
--rw-r--r--   0 kilic      (501) staff       (20)      178 2023-04-22 16:36:29.000000 gokyuzu-0.0.5/gokyuzu/BlueskyHelper.py
--rw-r--r--   0 kilic      (501) staff       (20)     2560 2023-04-22 17:00:10.000000 gokyuzu-0.0.5/gokyuzu/BlueskySession.py
--rw-r--r--   0 kilic      (501) staff       (20)     3377 2023-04-22 17:00:04.000000 gokyuzu-0.0.5/gokyuzu/__init__.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:00:57.679178 gokyuzu-0.0.5/gokyuzu.egg-info/
--rw-r--r--   0 kilic      (501) staff       (20)     1563 2023-04-22 17:00:57.000000 gokyuzu-0.0.5/gokyuzu.egg-info/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      331 2023-04-22 17:00:57.000000 gokyuzu-0.0.5/gokyuzu.egg-info/SOURCES.txt
--rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-22 17:00:57.000000 gokyuzu-0.0.5/gokyuzu.egg-info/dependency_links.txt
--rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-22 17:00:57.000000 gokyuzu-0.0.5/gokyuzu.egg-info/requires.txt
--rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-22 17:00:57.000000 gokyuzu-0.0.5/gokyuzu.egg-info/top_level.txt
--rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-22 17:00:46.000000 gokyuzu-0.0.5/pyproject.toml
--rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-22 17:00:57.679867 gokyuzu-0.0.5/setup.cfg
--rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-22 17:00:43.000000 gokyuzu-0.0.5/setup.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:00:57.679424 gokyuzu-0.0.5/tests/
--rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-0.0.5/tests/__init__.py
--rw-r--r--   0 kilic      (501) staff       (20)     3947 2023-04-22 16:59:52.000000 gokyuzu-0.0.5/tests/test_main.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:10:26.275395 gokyuzu-0.0.6/
+-rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-0.0.6/LICENSE
+-rw-r--r--   0 kilic      (501) staff       (20)     1953 2023-04-22 17:10:26.275274 gokyuzu-0.0.6/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)     1177 2023-04-22 17:08:59.000000 gokyuzu-0.0.6/README.md
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:10:26.274116 gokyuzu-0.0.6/gokyuzu/
+-rw-r--r--   0 kilic      (501) staff       (20)     1289 2023-04-22 17:00:00.000000 gokyuzu-0.0.6/gokyuzu/BlueskyEndpoints.py
+-rw-r--r--   0 kilic      (501) staff       (20)      178 2023-04-22 16:36:29.000000 gokyuzu-0.0.6/gokyuzu/BlueskyHelper.py
+-rw-r--r--   0 kilic      (501) staff       (20)     2560 2023-04-22 17:00:10.000000 gokyuzu-0.0.6/gokyuzu/BlueskySession.py
+-rw-r--r--   0 kilic      (501) staff       (20)     3362 2023-04-22 17:08:56.000000 gokyuzu-0.0.6/gokyuzu/__init__.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:10:26.274772 gokyuzu-0.0.6/gokyuzu.egg-info/
+-rw-r--r--   0 kilic      (501) staff       (20)     1953 2023-04-22 17:10:26.000000 gokyuzu-0.0.6/gokyuzu.egg-info/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)      331 2023-04-22 17:10:26.000000 gokyuzu-0.0.6/gokyuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-22 17:10:26.000000 gokyuzu-0.0.6/gokyuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-22 17:10:26.000000 gokyuzu-0.0.6/gokyuzu.egg-info/requires.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-22 17:10:26.000000 gokyuzu-0.0.6/gokyuzu.egg-info/top_level.txt
+-rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-22 17:09:57.000000 gokyuzu-0.0.6/pyproject.toml
+-rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-22 17:10:26.275436 gokyuzu-0.0.6/setup.cfg
+-rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-22 17:09:54.000000 gokyuzu-0.0.6/setup.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:10:26.274994 gokyuzu-0.0.6/tests/
+-rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-0.0.6/tests/__init__.py
+-rw-r--r--   0 kilic      (501) staff       (20)     3947 2023-04-22 16:59:52.000000 gokyuzu-0.0.6/tests/test_main.py
```

### Comparing `gokyuzu-0.0.5/gokyuzu/BlueskyEndpoints.py` & `gokyuzu-0.0.6/gokyuzu/BlueskyEndpoints.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-0.0.5/gokyuzu/BlueskySession.py` & `gokyuzu-0.0.6/gokyuzu/BlueskySession.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-0.0.5/gokyuzu/__init__.py` & `gokyuzu-0.0.6/gokyuzu/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,35 +10,35 @@
         self.BSKY_SERVER = "https://bsky.social"
         self.ENDPOINTS = BlueskyEndpoints(self.BSKY_SERVER)
         self.SESSION = BlueskySession(handle=handle, password=password)
 
     def __str__(self):
         return f"Bluesky(server={self.BSKY_SERVER}, handle={self.SESSION.getHandle()}, email={self.SESSION.getEmail()}, did={self.SESSION.getDID()}, accessToken={self.SESSION.getAccessToken()}, refreshToken={self.SESSION.getRefreshToken()})"
 
-    def resolveHandle(self, username):
-        request_url = self.ENDPOINTS.resolveHandle() + "?handle={}".format(username)
+    def resolveHandle(self, handle):
+        request_url = self.ENDPOINTS.resolveHandle() + "?handle={}".format(handle)
         response = self.SESSION.get(request_url)
         return response
     
-    def getProfile(self, did):
-        request_url = self.ENDPOINTS.getProfile() + "?actor={}".format(did)
+    def getProfile(self, user_did):
+        request_url = self.ENDPOINTS.getProfile() + "?actor={}".format(user_did)
         response = self.SESSION.get(request_url)
         return response
 
-    def follow(self, username=None, did_of_user=None):
-        if username:
-            did_of_user = self.resolveHandle(username).json().get("did")
+    def follow(self, handle=None, user_did=None):
+        if handle:
+            user_did = self.resolveHandle(handle).json().get("did")
 
-        if not did_of_user or did_of_user is None:
+        if not user_did or user_did is None:
             raise ValueError("Invalid username")
 
         follow_request_data = {
             "repo": self.DID,
             "record": {
-                "subject": did_of_user,
+                "subject": user_did,
                 "createdAt": BlueskyHelper.getTimestamp(),
                 "$type": "app.bsky.graph.follow"
             },
             "collection": "app.bsky.graph.follow"
         }
 
         response = self.SESSION.post(self.ENDPOINTS.createRecord(), json=follow_request_data)
```

### Comparing `gokyuzu-0.0.5/setup.py` & `gokyuzu-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gokyuzu',
-    version='0.0.5',
+    version='0.0.6',
     description='bsky.social client library',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Muhammed Kılıç',
     author_email='muhammeddkilicc@gmail.com',
     url='https://github.com/kiliczsh/gokyuzu',
     packages=find_packages(),
```

### Comparing `gokyuzu-0.0.5/tests/test_main.py` & `gokyuzu-0.0.6/tests/test_main.py`

 * *Files identical despite different names*

