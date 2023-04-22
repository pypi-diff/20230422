# Comparing `tmp/gokyuzu-0.0.3.tar.gz` & `tmp/gokyuzu-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gokyuzu-0.0.3.tar", last modified: Sat Apr 22 15:15:43 2023, max compression
+gzip compressed data, was "gokyuzu-0.0.4.tar", last modified: Sat Apr 22 15:56:12 2023, max compression
```

## Comparing `gokyuzu-0.0.3.tar` & `gokyuzu-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:15:43.692941 gokyuzu-0.0.3/
--rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 12:13:25.000000 gokyuzu-0.0.3/LICENSE
--rw-r--r--   0 kilic      (501) staff       (20)     1563 2023-04-22 15:15:43.692814 gokyuzu-0.0.3/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      787 2023-04-22 15:03:09.000000 gokyuzu-0.0.3/README.md
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:15:43.691710 gokyuzu-0.0.3/gokyuzu/
--rw-r--r--   0 kilic      (501) staff       (20)      761 2023-04-22 14:14:34.000000 gokyuzu-0.0.3/gokyuzu/BlueskyEndpoints.py
--rw-r--r--   0 kilic      (501) staff       (20)      161 2023-04-22 14:12:10.000000 gokyuzu-0.0.3/gokyuzu/BlueskyHelper.py
--rw-r--r--   0 kilic      (501) staff       (20)     2300 2023-04-22 14:17:06.000000 gokyuzu-0.0.3/gokyuzu/BlueskySession.py
--rw-r--r--   0 kilic      (501) staff       (20)     1723 2023-04-22 14:20:55.000000 gokyuzu-0.0.3/gokyuzu/__init__.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:15:43.692331 gokyuzu-0.0.3/gokyuzu.egg-info/
--rw-r--r--   0 kilic      (501) staff       (20)     1563 2023-04-22 15:15:43.000000 gokyuzu-0.0.3/gokyuzu.egg-info/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      331 2023-04-22 15:15:43.000000 gokyuzu-0.0.3/gokyuzu.egg-info/SOURCES.txt
--rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-22 15:15:43.000000 gokyuzu-0.0.3/gokyuzu.egg-info/dependency_links.txt
--rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-22 15:15:43.000000 gokyuzu-0.0.3/gokyuzu.egg-info/requires.txt
--rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-22 15:15:43.000000 gokyuzu-0.0.3/gokyuzu.egg-info/top_level.txt
--rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-22 15:13:44.000000 gokyuzu-0.0.3/pyproject.toml
--rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-22 15:15:43.692973 gokyuzu-0.0.3/setup.cfg
--rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-22 15:13:37.000000 gokyuzu-0.0.3/setup.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:15:43.692535 gokyuzu-0.0.3/tests/
--rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 11:38:56.000000 gokyuzu-0.0.3/tests/__init__.py
--rw-r--r--   0 kilic      (501) staff       (20)     1067 2023-04-22 14:33:58.000000 gokyuzu-0.0.3/tests/test_main.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:56:12.346914 gokyuzu-0.0.4/
+-rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-0.0.4/LICENSE
+-rw-r--r--   0 kilic      (501) staff       (20)     1563 2023-04-22 15:56:12.346789 gokyuzu-0.0.4/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)      787 2023-04-22 15:30:32.000000 gokyuzu-0.0.4/README.md
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:56:12.345371 gokyuzu-0.0.4/gokyuzu/
+-rw-r--r--   0 kilic      (501) staff       (20)      881 2023-04-22 15:47:35.000000 gokyuzu-0.0.4/gokyuzu/BlueskyEndpoints.py
+-rw-r--r--   0 kilic      (501) staff       (20)      161 2023-04-22 15:30:32.000000 gokyuzu-0.0.4/gokyuzu/BlueskyHelper.py
+-rw-r--r--   0 kilic      (501) staff       (20)     2300 2023-04-22 15:30:32.000000 gokyuzu-0.0.4/gokyuzu/BlueskySession.py
+-rw-r--r--   0 kilic      (501) staff       (20)     1932 2023-04-22 15:51:32.000000 gokyuzu-0.0.4/gokyuzu/__init__.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:56:12.346302 gokyuzu-0.0.4/gokyuzu.egg-info/
+-rw-r--r--   0 kilic      (501) staff       (20)     1563 2023-04-22 15:56:12.000000 gokyuzu-0.0.4/gokyuzu.egg-info/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)      331 2023-04-22 15:56:12.000000 gokyuzu-0.0.4/gokyuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-22 15:56:12.000000 gokyuzu-0.0.4/gokyuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-22 15:56:12.000000 gokyuzu-0.0.4/gokyuzu.egg-info/requires.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-22 15:56:12.000000 gokyuzu-0.0.4/gokyuzu.egg-info/top_level.txt
+-rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-22 15:55:36.000000 gokyuzu-0.0.4/pyproject.toml
+-rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-22 15:56:12.346958 gokyuzu-0.0.4/setup.cfg
+-rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-22 15:55:45.000000 gokyuzu-0.0.4/setup.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:56:12.346511 gokyuzu-0.0.4/tests/
+-rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-0.0.4/tests/__init__.py
+-rw-r--r--   0 kilic      (501) staff       (20)     1693 2023-04-22 15:54:26.000000 gokyuzu-0.0.4/tests/test_main.py
```

### Comparing `gokyuzu-0.0.3/PKG-INFO` & `gokyuzu-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 0.0.3
+Version: 0.0.4
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gokyuzu-0.0.3/README.md` & `gokyuzu-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gokyuzu-0.0.3/gokyuzu/BlueskyEndpoints.py` & `gokyuzu-0.0.4/gokyuzu/BlueskyEndpoints.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,7 +17,10 @@
         return self.get_url("/xrpc/app.bsky.actor.getProfile")
     
     def createRecord(self):
         return self.get_url("/xrpc/com.atproto.repo.createRecord")
     
     def deleteRecord(self):
         return self.get_url("/xrpc/com.atproto.repo.deleteRecord")
+    
+    def getAccountInviteCodes(self):
+        return self.get_url("/xrpc/com.atproto.server.getAccountInviteCodes")
```

### Comparing `gokyuzu-0.0.3/gokyuzu/BlueskySession.py` & `gokyuzu-0.0.4/gokyuzu/BlueskySession.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-0.0.3/gokyuzu/__init__.py` & `gokyuzu-0.0.4/gokyuzu/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,7 +37,12 @@
                 "$type": "app.bsky.graph.follow"
             },
             "collection": "app.bsky.graph.follow"
         }
 
         response = self.SESSION.post(self.ENDPOINTS.createRecord(), json=follow_request_data)
         return response
+
+    def getAccountInviteCodes(self, limit=10):
+        request_url = self.ENDPOINTS.getAccountInviteCodes() + "?limit={}".format(limit)
+        response = self.SESSION.get(request_url)
+        return response
```

### Comparing `gokyuzu-0.0.3/gokyuzu.egg-info/PKG-INFO` & `gokyuzu-0.0.4/gokyuzu.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 0.0.3
+Version: 0.0.4
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gokyuzu-0.0.3/setup.py` & `gokyuzu-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gokyuzu',
-    version='0.0.3',
+    version='0.0.4',
     description='bsky.social client library',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Muhammed Kılıç',
     author_email='muhammeddkilicc@gmail.com',
     url='https://github.com/kiliczsh/gokyuzu',
     packages=find_packages(),
```

### Comparing `gokyuzu-0.0.3/tests/test_main.py` & `gokyuzu-0.0.4/tests/test_main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import unittest
+import os
 from gokyuzu import *
 
-BSKY_SOCIAL_HANDLE = "handle.bsky.social"
-BSKY_SOCIAL_PASSWORD = ""
+BSKY_SOCIAL_HANDLE = str(os.environ.get('BSKY_SOCIAL_HANDLE'))
+BSKY_SOCIAL_PASSWORD = str(os.environ.get('BSKY_SOCIAL_PASSWORD'))
+
+class TestBluesky(unittest.TestCase):
+    def test_env(self):
+        self.assertNotEqual(BSKY_SOCIAL_HANDLE, '')
+        self.assertNotEqual(BSKY_SOCIAL_PASSWORD, '')
 
-class TestBlueskyLogin(unittest.TestCase):
     def test_login(self):
         bsky = Bluesky(BSKY_SOCIAL_HANDLE, BSKY_SOCIAL_PASSWORD)
         self.assertIsNotNone(bsky.SESSION)
         self.assertIsNotNone(bsky.SESSION.DID)
         self.assertIsNotNone(bsky.SESSION.ACCESS_TOKEN)
         self.assertNotEqual(bsky.SESSION.ACCESS_TOKEN, '') 
         self.assertIsNotNone(bsky.SESSION.REFRESH_TOKEN)
@@ -22,8 +27,16 @@
     def test_getProfile(self):
         bsky = Bluesky(BSKY_SOCIAL_HANDLE, BSKY_SOCIAL_PASSWORD)
         self.assertIsNotNone(bsky.SESSION)
         self.assertIsNotNone(bsky.SESSION.DID)
 
         profile = bsky.getProfile(bsky.SESSION.DID)
         self.assertIsNotNone(profile)
-        self.assertNotEqual(profile.json().get('did'), '')
+        self.assertNotEqual(profile.json().get('did'), '')
+
+    def test_invitationCodes(self):
+        bsky = Bluesky(BSKY_SOCIAL_HANDLE, BSKY_SOCIAL_PASSWORD)
+        invitationCodes = bsky.getAccountInviteCodes()
+        self.assertIsNotNone(invitationCodes)
+        self.assertNotEqual(invitationCodes.json().get('codes'), '')
+        self.assertNotEqual(invitationCodes.json().get('codes'), None)
+        print(f"Invitation codes count: {len(invitationCodes.json().get('codes'))}")
```

