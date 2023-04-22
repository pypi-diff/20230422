# Comparing `tmp/gokyuzu-1.0.0.tar.gz` & `tmp/gokyuzu-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gokyuzu-1.0.0.tar", last modified: Sat Apr 22 18:27:08 2023, max compression
+gzip compressed data, was "gokyuzu-1.0.1.tar", last modified: Sat Apr 22 19:49:05 2023, max compression
```

## Comparing `gokyuzu-1.0.0.tar` & `gokyuzu-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 18:27:08.493571 gokyuzu-1.0.0/
--rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-1.0.0/LICENSE
--rw-r--r--   0 kilic      (501) staff       (20)     2537 2023-04-22 18:27:08.493447 gokyuzu-1.0.0/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)     1761 2023-04-22 18:24:18.000000 gokyuzu-1.0.0/README.md
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 18:27:08.491991 gokyuzu-1.0.0/gokyuzu/
--rw-r--r--   0 kilic      (501) staff       (20)     2274 2023-04-22 18:24:48.000000 gokyuzu-1.0.0/gokyuzu/BlueskyEndpoints.py
--rw-r--r--   0 kilic      (501) staff       (20)      178 2023-04-22 16:36:29.000000 gokyuzu-1.0.0/gokyuzu/BlueskyHelper.py
--rw-r--r--   0 kilic      (501) staff       (20)     2560 2023-04-22 17:00:10.000000 gokyuzu-1.0.0/gokyuzu/BlueskySession.py
--rw-r--r--   0 kilic      (501) staff       (20)     6990 2023-04-22 18:26:24.000000 gokyuzu-1.0.0/gokyuzu/__init__.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 18:27:08.492703 gokyuzu-1.0.0/gokyuzu.egg-info/
--rw-r--r--   0 kilic      (501) staff       (20)     2537 2023-04-22 18:27:08.000000 gokyuzu-1.0.0/gokyuzu.egg-info/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      331 2023-04-22 18:27:08.000000 gokyuzu-1.0.0/gokyuzu.egg-info/SOURCES.txt
--rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-22 18:27:08.000000 gokyuzu-1.0.0/gokyuzu.egg-info/dependency_links.txt
--rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-22 18:27:08.000000 gokyuzu-1.0.0/gokyuzu.egg-info/requires.txt
--rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-22 18:27:08.000000 gokyuzu-1.0.0/gokyuzu.egg-info/top_level.txt
--rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-22 18:25:59.000000 gokyuzu-1.0.0/pyproject.toml
--rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-22 18:27:08.493608 gokyuzu-1.0.0/setup.cfg
--rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-22 18:25:52.000000 gokyuzu-1.0.0/setup.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 18:27:08.492911 gokyuzu-1.0.0/tests/
--rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-1.0.0/tests/__init__.py
--rw-r--r--   0 kilic      (501) staff       (20)     4207 2023-04-22 18:05:49.000000 gokyuzu-1.0.0/tests/test_main.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 19:49:05.681692 gokyuzu-1.0.1/
+-rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-1.0.1/LICENSE
+-rw-r--r--   0 kilic      (501) staff       (20)     2537 2023-04-22 19:49:05.681589 gokyuzu-1.0.1/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)     1761 2023-04-22 18:24:18.000000 gokyuzu-1.0.1/README.md
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 19:49:05.680322 gokyuzu-1.0.1/gokyuzu/
+-rw-r--r--   0 kilic      (501) staff       (20)     6402 2023-04-22 19:28:38.000000 gokyuzu-1.0.1/gokyuzu/BlueskyEndpoints.py
+-rw-r--r--   0 kilic      (501) staff       (20)      178 2023-04-22 16:36:29.000000 gokyuzu-1.0.1/gokyuzu/BlueskyHelper.py
+-rw-r--r--   0 kilic      (501) staff       (20)     3075 2023-04-22 19:21:58.000000 gokyuzu-1.0.1/gokyuzu/BlueskySession.py
+-rw-r--r--   0 kilic      (501) staff       (20)     8830 2023-04-22 19:48:01.000000 gokyuzu-1.0.1/gokyuzu/__init__.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 19:49:05.681067 gokyuzu-1.0.1/gokyuzu.egg-info/
+-rw-r--r--   0 kilic      (501) staff       (20)     2537 2023-04-22 19:49:05.000000 gokyuzu-1.0.1/gokyuzu.egg-info/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)      331 2023-04-22 19:49:05.000000 gokyuzu-1.0.1/gokyuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-22 19:49:05.000000 gokyuzu-1.0.1/gokyuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-22 19:49:05.000000 gokyuzu-1.0.1/gokyuzu.egg-info/requires.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-22 19:49:05.000000 gokyuzu-1.0.1/gokyuzu.egg-info/top_level.txt
+-rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-22 19:48:23.000000 gokyuzu-1.0.1/pyproject.toml
+-rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-22 19:49:05.681727 gokyuzu-1.0.1/setup.cfg
+-rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-22 19:48:19.000000 gokyuzu-1.0.1/setup.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 19:49:05.681289 gokyuzu-1.0.1/tests/
+-rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-1.0.1/tests/__init__.py
+-rw-r--r--   0 kilic      (501) staff       (20)     4706 2023-04-22 19:03:38.000000 gokyuzu-1.0.1/tests/test_main.py
```

### Comparing `gokyuzu-1.0.0/PKG-INFO` & `gokyuzu-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 1.0.0
+Version: 1.0.1
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gokyuzu-1.0.0/README.md` & `gokyuzu-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gokyuzu-1.0.0/gokyuzu/BlueskySession.py` & `gokyuzu-1.0.1/gokyuzu/BlueskySession.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,11 +60,23 @@
         return response
         
     def post(self, url, data=None, json=None, **kwargs):
         headers = { 'Authorization': f'Bearer {self.getAccessToken()}'}
         response = requests.post(url, headers=headers, data=data, json=json, **kwargs)
         return response
     
+    def post(self, url, headers=None, data=None, json=None, **kwargs):
+        if headers is None:
+            headers = {}
+        headers['Authorization'] = f'Bearer {self.getAccessToken()}'
+        response = requests.post(url, headers=headers, data=data, json=json, **kwargs)
+        return response
+    
     def postJson(self, url, json, **kwargs):
         headers = { 'Authorization': f'Bearer {self.getAccessToken()}', 'Content-Type': 'application/json' }
         response = requests.post(url, headers=headers, json=json, **kwargs)
         return response
+    
+    def options(self, url, **kwargs):
+        headers = {'Authorization': f'Bearer {self.getAccessToken()}'}
+        response = requests.options(url, headers=headers, **kwargs)
+        return response
```

### Comparing `gokyuzu-1.0.0/gokyuzu/__init__.py` & `gokyuzu-1.0.1/gokyuzu/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,14 +32,19 @@
         return response
     
     def getAccountInviteCodes(self, limit=10):
         request_url = self.ENDPOINTS.getAccountInviteCodes() + "?limit={}".format(limit)
         response = self.SESSION.get(request_url)
         return response
 
+    def describeServer(self):
+        request_url = self.ENDPOINTS.describeServer()
+        response = self.SESSION.get(request_url)
+        return response
+
     # app.bsky.actor
     def getProfile(self, user_did):
         request_url = self.ENDPOINTS.getProfile() + "?actor={}".format(user_did)
         response = self.SESSION.get(request_url)
         return response
     
     def getProfiles(self, user_dids):
@@ -72,14 +77,24 @@
         return response
     
     def getPostThread(self, post_id, limit=10, cursor=""):
         request_url = self.ENDPOINTS.getPostThread() + "?uri={}&limit={}&cursor={}".format(post_id, limit, cursor)
         response = self.SESSION.get(request_url)
         return response
 
+    def getLikes(self, post_id, limit=10, cursor=""):
+        request_url = self.ENDPOINTS.getLikes() + "?uri={}&limit={}&cursor={}".format(post_id, limit, cursor)
+        response = self.SESSION.get(request_url)
+        return response
+
+    def getRepostedBy(self, post_id, limit=10, cursor=""):
+        request_url = self.ENDPOINTS.getRepostedBy() + "?uri={}&limit={}&cursor={}".format(post_id, limit, cursor)
+        response = self.SESSION.get(request_url)
+        return response
+
     # app.bsky.graph
     def getFollowers(self, handle=None, user_did=None, limit=10, cursor=""):
         if handle:
             actor = handle
         elif user_did:
             actor = user_did
         else:
@@ -183,7 +198,37 @@
     def updateHandle(self, handle):
         request_data = {
             "handle": handle
         }
 
         response = self.SESSION.postJson(self.ENDPOINTS.updateHandle(), json=request_data)
         return response
+
+    def health(self):
+        request_url = self.ENDPOINTS.health()
+        response = self.SESSION.get(request_url)
+        return response
+
+    def uploadImage(self, image_path, content_type="image/jpeg"):
+        request_url = self.ENDPOINTS.uploadBlob()
+        headers = {"Content-Type": content_type}
+        with open(image_path, 'rb') as f:
+            data = f.read()
+            response = self.SESSION.post(request_url, data=data, headers=headers)
+        return response
+
+    def searchTypeAhead(self, query="", limit=10):
+        typeahead_url = "https://bsky.social/xrpc/app.bsky.actor.searchActorsTypeahead"
+        request_url = "{}?term={}&limit={}".format(typeahead_url, query, limit)
+        response = self.SESSION.get(request_url)
+        return response
+
+    def search(self, query_type="posts", query=""):
+        request_url = "https://search.bsky.social/search/{}?q={}".format(query_type, query)
+        response = self.SESSION.get(request_url)
+        return response
+
+    def search_profiles(self, query):
+        return self.search(query_type="profiles", query=query)
+    
+    def search_posts(self, query):
+        return self.search(query_type="posts", query=query)
```

### Comparing `gokyuzu-1.0.0/gokyuzu.egg-info/PKG-INFO` & `gokyuzu-1.0.1/gokyuzu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 1.0.0
+Version: 1.0.1
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gokyuzu-1.0.0/setup.py` & `gokyuzu-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gokyuzu',
-    version='1.0.0',
+    version='1.0.1',
     description='bsky.social client library',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Muhammed Kılıç',
     author_email='muhammeddkilicc@gmail.com',
     url='https://github.com/kiliczsh/gokyuzu',
     packages=find_packages(),
```

### Comparing `gokyuzu-1.0.0/tests/test_main.py` & `gokyuzu-1.0.1/tests/test_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 import os
 from gokyuzu import *
 
 BSKY_SOCIAL_HANDLE = str(os.environ.get('BSKY_SOCIAL_HANDLE'))
 BSKY_SOCIAL_PASSWORD = str(os.environ.get('BSKY_SOCIAL_PASSWORD'))
 
 class TestBluesky(unittest.TestCase):
+    def test_health(self):
+        bsky = Bluesky(BSKY_SOCIAL_HANDLE, BSKY_SOCIAL_PASSWORD)
+        bsky.health()
+
     def test_env(self):
         self.assertNotEqual(BSKY_SOCIAL_HANDLE, '')
         self.assertNotEqual(BSKY_SOCIAL_PASSWORD, '')
 
     def test_login(self):
         bsky = Bluesky(BSKY_SOCIAL_HANDLE, BSKY_SOCIAL_PASSWORD)
         self.assertIsNotNone(bsky.SESSION)
@@ -87,7 +91,15 @@
 
     def test_getTimeline(self):
         bsky = Bluesky(BSKY_SOCIAL_HANDLE, BSKY_SOCIAL_PASSWORD)
         timeline = bsky.getTimeline()
         self.assertIsNotNone(timeline)
         feed = timeline.json().get('feed')
         self.assertEqual(len(feed), 10)
+
+    def test_options(self):
+        bsky = Bluesky(BSKY_SOCIAL_HANDLE, BSKY_SOCIAL_PASSWORD)
+        all_endpoints = bsky.ENDPOINTS.getAllEndpoints()
+        for endpoint in all_endpoints:
+            response = bsky.SESSION.options(endpoint)
+            print("{}: {}".format(endpoint, response.status_code))
+            # print(response.headers.get("Access-Control-Allow-Methods"))
```

