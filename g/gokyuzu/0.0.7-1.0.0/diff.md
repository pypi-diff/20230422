# Comparing `tmp/gokyuzu-0.0.7.tar.gz` & `tmp/gokyuzu-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gokyuzu-0.0.7.tar", last modified: Sat Apr 22 17:21:23 2023, max compression
+gzip compressed data, was "gokyuzu-1.0.0.tar", last modified: Sat Apr 22 18:27:08 2023, max compression
```

## Comparing `gokyuzu-0.0.7.tar` & `gokyuzu-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:21:23.642806 gokyuzu-0.0.7/
--rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-0.0.7/LICENSE
--rw-r--r--   0 kilic      (501) staff       (20)     1953 2023-04-22 17:21:23.642701 gokyuzu-0.0.7/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)     1177 2023-04-22 17:08:59.000000 gokyuzu-0.0.7/README.md
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:21:23.641324 gokyuzu-0.0.7/gokyuzu/
--rw-r--r--   0 kilic      (501) staff       (20)     1384 2023-04-22 17:14:56.000000 gokyuzu-0.0.7/gokyuzu/BlueskyEndpoints.py
--rw-r--r--   0 kilic      (501) staff       (20)      178 2023-04-22 16:36:29.000000 gokyuzu-0.0.7/gokyuzu/BlueskyHelper.py
--rw-r--r--   0 kilic      (501) staff       (20)     2560 2023-04-22 17:00:10.000000 gokyuzu-0.0.7/gokyuzu/BlueskySession.py
--rw-r--r--   0 kilic      (501) staff       (20)     3644 2023-04-22 17:20:32.000000 gokyuzu-0.0.7/gokyuzu/__init__.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:21:23.642195 gokyuzu-0.0.7/gokyuzu.egg-info/
--rw-r--r--   0 kilic      (501) staff       (20)     1953 2023-04-22 17:21:23.000000 gokyuzu-0.0.7/gokyuzu.egg-info/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      331 2023-04-22 17:21:23.000000 gokyuzu-0.0.7/gokyuzu.egg-info/SOURCES.txt
--rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-22 17:21:23.000000 gokyuzu-0.0.7/gokyuzu.egg-info/dependency_links.txt
--rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-22 17:21:23.000000 gokyuzu-0.0.7/gokyuzu.egg-info/requires.txt
--rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-22 17:21:23.000000 gokyuzu-0.0.7/gokyuzu.egg-info/top_level.txt
--rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-22 17:21:05.000000 gokyuzu-0.0.7/pyproject.toml
--rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-22 17:21:23.642839 gokyuzu-0.0.7/setup.cfg
--rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-22 17:21:02.000000 gokyuzu-0.0.7/setup.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:21:23.642419 gokyuzu-0.0.7/tests/
--rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-0.0.7/tests/__init__.py
--rw-r--r--   0 kilic      (501) staff       (20)     4207 2023-04-22 17:20:05.000000 gokyuzu-0.0.7/tests/test_main.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 18:27:08.493571 gokyuzu-1.0.0/
+-rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-1.0.0/LICENSE
+-rw-r--r--   0 kilic      (501) staff       (20)     2537 2023-04-22 18:27:08.493447 gokyuzu-1.0.0/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)     1761 2023-04-22 18:24:18.000000 gokyuzu-1.0.0/README.md
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 18:27:08.491991 gokyuzu-1.0.0/gokyuzu/
+-rw-r--r--   0 kilic      (501) staff       (20)     2274 2023-04-22 18:24:48.000000 gokyuzu-1.0.0/gokyuzu/BlueskyEndpoints.py
+-rw-r--r--   0 kilic      (501) staff       (20)      178 2023-04-22 16:36:29.000000 gokyuzu-1.0.0/gokyuzu/BlueskyHelper.py
+-rw-r--r--   0 kilic      (501) staff       (20)     2560 2023-04-22 17:00:10.000000 gokyuzu-1.0.0/gokyuzu/BlueskySession.py
+-rw-r--r--   0 kilic      (501) staff       (20)     6990 2023-04-22 18:26:24.000000 gokyuzu-1.0.0/gokyuzu/__init__.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 18:27:08.492703 gokyuzu-1.0.0/gokyuzu.egg-info/
+-rw-r--r--   0 kilic      (501) staff       (20)     2537 2023-04-22 18:27:08.000000 gokyuzu-1.0.0/gokyuzu.egg-info/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)      331 2023-04-22 18:27:08.000000 gokyuzu-1.0.0/gokyuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-22 18:27:08.000000 gokyuzu-1.0.0/gokyuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-22 18:27:08.000000 gokyuzu-1.0.0/gokyuzu.egg-info/requires.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-22 18:27:08.000000 gokyuzu-1.0.0/gokyuzu.egg-info/top_level.txt
+-rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-22 18:25:59.000000 gokyuzu-1.0.0/pyproject.toml
+-rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-22 18:27:08.493608 gokyuzu-1.0.0/setup.cfg
+-rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-22 18:25:52.000000 gokyuzu-1.0.0/setup.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 18:27:08.492911 gokyuzu-1.0.0/tests/
+-rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-1.0.0/tests/__init__.py
+-rw-r--r--   0 kilic      (501) staff       (20)     4207 2023-04-22 18:05:49.000000 gokyuzu-1.0.0/tests/test_main.py
```

### Comparing `gokyuzu-0.0.7/PKG-INFO` & `gokyuzu-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 0.0.7
+Version: 1.0.0
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -38,22 +38,33 @@
 print(response.json())
 ```
 
 ### Documentation
 
 List of Implemented API Calls:
 
-- `resolveHandle(username)`
-- `getProfile(user_did)`
-- `follow(handle=None, user_did=None)`
-- `getAccountInviteCodes(limit=10)`
-- `getFollowers(handle=None, user_did=None, limit=10, cursor="")`
-- `getFollows(handle=None, user_did=None, limit=10, cursor="")`
-- `listNotifications(limit=10, cursor="")`
-- `updateSeen(limit=10, cursor="")`
+- `createAccount(self, email, handle, password, inviteCode)`
+- `getSession(self)`
+- `getAccountInviteCodes(self, limit=10)`
+- `getProfile(self, user_did)`
+- `getProfiles(self, user_dids)`
+- `getPopular(self, limit=10, cursor="")`
+- `getTimeline(self, limit=10, cursor="", algorithm="reverse-chronological")`
+- `getAuthorFeed(self, handle=None, user_did=None, limit=10, cursor="")`
+- `getPostThread(self, post_id, limit=10, cursor="")`
+- `getFollowers(self, handle=None, user_did=None, limit=10, cursor="")`
+- `getFollows(self, handle=None, user_did=None, limit=10, cursor="")`
+- `listNotifications(self, limit=10, cursor="")`
+- `updateSeen(self, limit=10, cursor="")`
+- `createRecord(self, repo, record, collection)`
+- `deleteRecord(self, repo, record, collection)`
+- `follow(self, handle=None, user_did=None)`
+- `unfollow(self, handle=None, user_did=None)`
+- `resolveHandle(self, handle)`
+- `updateHandle(self, handle)`
 
 
 ### Development
 
 ```bash
 python -m venv venv
 source venv/bin/activate
```

### Comparing `gokyuzu-0.0.7/gokyuzu/BlueskyEndpoints.py` & `gokyuzu-1.0.0/gokyuzu/BlueskyEndpoints.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,39 +3,70 @@
         self.BSKY_SERVER = BSKY_SERVER
         if not self.BSKY_SERVER:
             self.BSKY_SERVER = "https://bsky.social"
 
     def get_url(self, path):
         return self.BSKY_SERVER + path
     
+    # com.atproto.server
+    def createAccount(self):
+        return self.get_url("/xrpc/com.atproto.server.createAccount")
+
     def createSession(self):
         return self.get_url("/xrpc/com.atproto.server.createSession")
     
-    def resolveHandle(self):
-        return self.get_url("/xrpc/com.atproto.identity.resolveHandle")
+    def getSession(self):
+        return self.get_url("/xrpc/com.atproto.server.getSession")
+    
+    def getAccountInviteCodes(self):
+        return self.get_url("/xrpc/com.atproto.server.getAccountInviteCodes")
     
+    # app.bsky.actor
     def getProfile(self):
         return self.get_url("/xrpc/app.bsky.actor.getProfile")
     
-    def createRecord(self):
-        return self.get_url("/xrpc/com.atproto.repo.createRecord")
+    def getProfiles(self):
+        return self.get_url("/xrpc/app.bsky.actor.getProfiles")
     
-    def deleteRecord(self):
-        return self.get_url("/xrpc/com.atproto.repo.deleteRecord")
+    # app.bsky.unspecced
+    def getPopular(self):
+        return self.get_url("/xrpc/app.bsky.unspecced.getPopular")
     
-    def getAccountInviteCodes(self):
-        return self.get_url("/xrpc/com.atproto.server.getAccountInviteCodes")
+    # app.bsky.feed
+    def getTimeline(self):
+        return self.get_url("/xrpc/app.bsky.feed.getTimeline")
+    
+    def getAuthorFeed(self):
+        return self.get_url("/xrpc/app.bsky.feed.getAuthorFeed")
     
+    def getPostThread(self):
+        return self.get_url("/xrpc/app.bsky.feed.getPostThread")
+    
+    # app.bsky.graph    
     def getFollowers(self):
         return self.get_url("/xrpc/app.bsky.graph.getFollowers")
     
     def getFollows(self):
         return self.get_url("/xrpc/app.bsky.graph.getFollows")
     
+    # app.bsky.notification
     def listNotifications(self):
         return self.get_url("/xrpc/app.bsky.notification.listNotifications")
     
     def updateSeen(self):
         return self.get_url("/xrpc/app.bsky.notification.updateSeen")
     
-    def getTimeline(self):
-        return self.get_url("/xrpc/app.bsky.feed.getTimeline")
+    # com.atproto.repo
+    def createRecord(self):
+        return self.get_url("/xrpc/com.atproto.repo.createRecord")
+    
+    def deleteRecord(self):
+        return self.get_url("/xrpc/com.atproto.repo.deleteRecord")
+    
+    # com.atproto.identity
+    def resolveHandle(self):
+        return self.get_url("/xrpc/com.atproto.identity.resolveHandle")
+    
+    def updateHandle(self):
+        return self.get_url("/xrpc/com.atproto.identity.updateHandle")
+
+
```

### Comparing `gokyuzu-0.0.7/gokyuzu/BlueskySession.py` & `gokyuzu-1.0.0/gokyuzu/BlueskySession.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-0.0.7/gokyuzu.egg-info/PKG-INFO` & `gokyuzu-1.0.0/gokyuzu.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 0.0.7
+Version: 1.0.0
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -38,22 +38,33 @@
 print(response.json())
 ```
 
 ### Documentation
 
 List of Implemented API Calls:
 
-- `resolveHandle(username)`
-- `getProfile(user_did)`
-- `follow(handle=None, user_did=None)`
-- `getAccountInviteCodes(limit=10)`
-- `getFollowers(handle=None, user_did=None, limit=10, cursor="")`
-- `getFollows(handle=None, user_did=None, limit=10, cursor="")`
-- `listNotifications(limit=10, cursor="")`
-- `updateSeen(limit=10, cursor="")`
+- `createAccount(self, email, handle, password, inviteCode)`
+- `getSession(self)`
+- `getAccountInviteCodes(self, limit=10)`
+- `getProfile(self, user_did)`
+- `getProfiles(self, user_dids)`
+- `getPopular(self, limit=10, cursor="")`
+- `getTimeline(self, limit=10, cursor="", algorithm="reverse-chronological")`
+- `getAuthorFeed(self, handle=None, user_did=None, limit=10, cursor="")`
+- `getPostThread(self, post_id, limit=10, cursor="")`
+- `getFollowers(self, handle=None, user_did=None, limit=10, cursor="")`
+- `getFollows(self, handle=None, user_did=None, limit=10, cursor="")`
+- `listNotifications(self, limit=10, cursor="")`
+- `updateSeen(self, limit=10, cursor="")`
+- `createRecord(self, repo, record, collection)`
+- `deleteRecord(self, repo, record, collection)`
+- `follow(self, handle=None, user_did=None)`
+- `unfollow(self, handle=None, user_did=None)`
+- `resolveHandle(self, handle)`
+- `updateHandle(self, handle)`
 
 
 ### Development
 
 ```bash
 python -m venv venv
 source venv/bin/activate
```

### Comparing `gokyuzu-0.0.7/setup.py` & `gokyuzu-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gokyuzu',
-    version='0.0.7',
+    version='1.0.0',
     description='bsky.social client library',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Muhammed Kılıç',
     author_email='muhammeddkilicc@gmail.com',
     url='https://github.com/kiliczsh/gokyuzu',
     packages=find_packages(),
```

### Comparing `gokyuzu-0.0.7/tests/test_main.py` & `gokyuzu-1.0.0/tests/test_main.py`

 * *Files identical despite different names*

