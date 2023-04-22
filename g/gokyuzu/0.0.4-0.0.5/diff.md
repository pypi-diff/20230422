# Comparing `tmp/gokyuzu-0.0.4.tar.gz` & `tmp/gokyuzu-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gokyuzu-0.0.4.tar", last modified: Sat Apr 22 15:56:12 2023, max compression
+gzip compressed data, was "gokyuzu-0.0.5.tar", last modified: Sat Apr 22 17:00:57 2023, max compression
```

## Comparing `gokyuzu-0.0.4.tar` & `gokyuzu-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:56:12.346914 gokyuzu-0.0.4/
--rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-0.0.4/LICENSE
--rw-r--r--   0 kilic      (501) staff       (20)     1563 2023-04-22 15:56:12.346789 gokyuzu-0.0.4/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      787 2023-04-22 15:30:32.000000 gokyuzu-0.0.4/README.md
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:56:12.345371 gokyuzu-0.0.4/gokyuzu/
--rw-r--r--   0 kilic      (501) staff       (20)      881 2023-04-22 15:47:35.000000 gokyuzu-0.0.4/gokyuzu/BlueskyEndpoints.py
--rw-r--r--   0 kilic      (501) staff       (20)      161 2023-04-22 15:30:32.000000 gokyuzu-0.0.4/gokyuzu/BlueskyHelper.py
--rw-r--r--   0 kilic      (501) staff       (20)     2300 2023-04-22 15:30:32.000000 gokyuzu-0.0.4/gokyuzu/BlueskySession.py
--rw-r--r--   0 kilic      (501) staff       (20)     1932 2023-04-22 15:51:32.000000 gokyuzu-0.0.4/gokyuzu/__init__.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:56:12.346302 gokyuzu-0.0.4/gokyuzu.egg-info/
--rw-r--r--   0 kilic      (501) staff       (20)     1563 2023-04-22 15:56:12.000000 gokyuzu-0.0.4/gokyuzu.egg-info/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      331 2023-04-22 15:56:12.000000 gokyuzu-0.0.4/gokyuzu.egg-info/SOURCES.txt
--rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-22 15:56:12.000000 gokyuzu-0.0.4/gokyuzu.egg-info/dependency_links.txt
--rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-22 15:56:12.000000 gokyuzu-0.0.4/gokyuzu.egg-info/requires.txt
--rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-22 15:56:12.000000 gokyuzu-0.0.4/gokyuzu.egg-info/top_level.txt
--rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-22 15:55:36.000000 gokyuzu-0.0.4/pyproject.toml
--rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-22 15:56:12.346958 gokyuzu-0.0.4/setup.cfg
--rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-22 15:55:45.000000 gokyuzu-0.0.4/setup.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 15:56:12.346511 gokyuzu-0.0.4/tests/
--rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-0.0.4/tests/__init__.py
--rw-r--r--   0 kilic      (501) staff       (20)     1693 2023-04-22 15:54:26.000000 gokyuzu-0.0.4/tests/test_main.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:00:57.679827 gokyuzu-0.0.5/
+-rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-0.0.5/LICENSE
+-rw-r--r--   0 kilic      (501) staff       (20)     1563 2023-04-22 17:00:57.679715 gokyuzu-0.0.5/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)      787 2023-04-22 15:30:32.000000 gokyuzu-0.0.5/README.md
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:00:57.678492 gokyuzu-0.0.5/gokyuzu/
+-rw-r--r--   0 kilic      (501) staff       (20)     1289 2023-04-22 17:00:00.000000 gokyuzu-0.0.5/gokyuzu/BlueskyEndpoints.py
+-rw-r--r--   0 kilic      (501) staff       (20)      178 2023-04-22 16:36:29.000000 gokyuzu-0.0.5/gokyuzu/BlueskyHelper.py
+-rw-r--r--   0 kilic      (501) staff       (20)     2560 2023-04-22 17:00:10.000000 gokyuzu-0.0.5/gokyuzu/BlueskySession.py
+-rw-r--r--   0 kilic      (501) staff       (20)     3377 2023-04-22 17:00:04.000000 gokyuzu-0.0.5/gokyuzu/__init__.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:00:57.679178 gokyuzu-0.0.5/gokyuzu.egg-info/
+-rw-r--r--   0 kilic      (501) staff       (20)     1563 2023-04-22 17:00:57.000000 gokyuzu-0.0.5/gokyuzu.egg-info/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)      331 2023-04-22 17:00:57.000000 gokyuzu-0.0.5/gokyuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-22 17:00:57.000000 gokyuzu-0.0.5/gokyuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-22 17:00:57.000000 gokyuzu-0.0.5/gokyuzu.egg-info/requires.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-22 17:00:57.000000 gokyuzu-0.0.5/gokyuzu.egg-info/top_level.txt
+-rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-22 17:00:46.000000 gokyuzu-0.0.5/pyproject.toml
+-rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-22 17:00:57.679867 gokyuzu-0.0.5/setup.cfg
+-rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-22 17:00:43.000000 gokyuzu-0.0.5/setup.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 17:00:57.679424 gokyuzu-0.0.5/tests/
+-rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-0.0.5/tests/__init__.py
+-rw-r--r--   0 kilic      (501) staff       (20)     3947 2023-04-22 16:59:52.000000 gokyuzu-0.0.5/tests/test_main.py
```

### Comparing `gokyuzu-0.0.4/PKG-INFO` & `gokyuzu-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 0.0.4
+Version: 0.0.5
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gokyuzu-0.0.4/README.md` & `gokyuzu-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gokyuzu-0.0.4/gokyuzu/BlueskySession.py` & `gokyuzu-0.0.5/gokyuzu/BlueskySession.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,10 +56,15 @@
         
     def get(self, url, **kwargs):
         headers = {'Authorization': f'Bearer {self.getAccessToken()}'}
         response = requests.get(url, headers=headers, **kwargs)
         return response
         
     def post(self, url, data=None, json=None, **kwargs):
-        headers = {'Authorization': f'Bearer {self.getAccessToken()}'}
+        headers = { 'Authorization': f'Bearer {self.getAccessToken()}'}
         response = requests.post(url, headers=headers, data=data, json=json, **kwargs)
         return response
+    
+    def postJson(self, url, json, **kwargs):
+        headers = { 'Authorization': f'Bearer {self.getAccessToken()}', 'Content-Type': 'application/json' }
+        response = requests.post(url, headers=headers, json=json, **kwargs)
+        return response
```

### Comparing `gokyuzu-0.0.4/gokyuzu.egg-info/PKG-INFO` & `gokyuzu-0.0.5/gokyuzu.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 0.0.4
+Version: 0.0.5
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gokyuzu-0.0.4/setup.py` & `gokyuzu-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gokyuzu',
-    version='0.0.4',
+    version='0.0.5',
     description='bsky.social client library',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Muhammed Kılıç',
     author_email='muhammeddkilicc@gmail.com',
     url='https://github.com/kiliczsh/gokyuzu',
     packages=find_packages(),
```

