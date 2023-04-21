# Comparing `tmp/twitter-api-client-0.7.1.tar.gz` & `tmp/twitter-api-client-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.7.1.tar", last modified: Fri Apr 21 23:29:24 2023, max compression
+gzip compressed data, was "twitter-api-client-0.7.2.tar", last modified: Fri Apr 21 23:31:46 2023, max compression
```

## Comparing `twitter-api-client-0.7.1.tar` & `twitter-api-client-0.7.2.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 23:29:24.377502 twitter-api-client-0.7.1/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.7.1/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     6933 2023-04-21 23:29:24.377502 twitter-api-client-0.7.1/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-21 23:29:24.377502 twitter-api-client-0.7.1/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     8239 2023-04-21 23:29:20.000000 twitter-api-client-0.7.1/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 23:29:24.377502 twitter-api-client-0.7.1/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.1/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-21 23:27:09.000000 twitter-api-client-0.7.1/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-21 23:24:45.000000 twitter-api-client-0.7.1/twitter/account2.py
--rw-r--r--   0 x         (1000) x         (1000)    27260 2023-04-19 22:52:46.000000 twitter-api-client-0.7.1/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-21 22:39:59.000000 twitter-api-client-0.7.1/twitter/login.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 23:29:24.377502 twitter-api-client-0.7.1/twitter/noauth/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.1/twitter/noauth/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     2567 2023-04-19 22:52:46.000000 twitter-api-client-0.7.1/twitter/noauth/operation.py
--rw-r--r--   0 x         (1000) x         (1000)     7398 2023-04-21 23:29:07.000000 twitter-api-client-0.7.1/twitter/noauth/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     2852 2023-04-17 21:53:35.000000 twitter-api-client-0.7.1/twitter/noauth/util.py
--rw-r--r--   0 x         (1000) x         (1000)    10604 2023-04-21 23:27:09.000000 twitter-api-client-0.7.1/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)    10604 2023-04-21 23:12:32.000000 twitter-api-client-0.7.1/twitter/scraper2.py
--rw-r--r--   0 x         (1000) x         (1000)     4469 2023-04-21 23:25:19.000000 twitter-api-client-0.7.1/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     3270 2023-04-21 04:27:51.000000 twitter-api-client-0.7.1/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 23:29:24.377502 twitter-api-client-0.7.1/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     6933 2023-04-21 23:29:24.000000 twitter-api-client-0.7.1/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      499 2023-04-21 23:29:24.000000 twitter-api-client-0.7.1/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-21 23:29:24.000000 twitter-api-client-0.7.1/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       79 2023-04-21 23:29:24.000000 twitter-api-client-0.7.1/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-21 23:29:24.000000 twitter-api-client-0.7.1/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 23:31:46.213567 twitter-api-client-0.7.2/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.7.2/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     6933 2023-04-21 23:31:46.213567 twitter-api-client-0.7.2/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-21 23:31:46.213567 twitter-api-client-0.7.2/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     8239 2023-04-21 23:31:42.000000 twitter-api-client-0.7.2/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 23:31:46.213567 twitter-api-client-0.7.2/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.2/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-21 23:27:09.000000 twitter-api-client-0.7.2/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    27260 2023-04-19 22:52:46.000000 twitter-api-client-0.7.2/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-21 22:39:59.000000 twitter-api-client-0.7.2/twitter/login.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 23:31:46.213567 twitter-api-client-0.7.2/twitter/noauth/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.2/twitter/noauth/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     2567 2023-04-19 22:52:46.000000 twitter-api-client-0.7.2/twitter/noauth/operation.py
+-rw-r--r--   0 x         (1000) x         (1000)     7398 2023-04-21 23:29:07.000000 twitter-api-client-0.7.2/twitter/noauth/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     2852 2023-04-17 21:53:35.000000 twitter-api-client-0.7.2/twitter/noauth/util.py
+-rw-r--r--   0 x         (1000) x         (1000)    10604 2023-04-21 23:27:09.000000 twitter-api-client-0.7.2/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     4469 2023-04-21 23:25:19.000000 twitter-api-client-0.7.2/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-21 23:31:42.000000 twitter-api-client-0.7.2/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 23:31:46.213567 twitter-api-client-0.7.2/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     6933 2023-04-21 23:31:46.000000 twitter-api-client-0.7.2/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      459 2023-04-21 23:31:46.000000 twitter-api-client-0.7.2/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-21 23:31:46.000000 twitter-api-client-0.7.2/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       79 2023-04-21 23:31:46.000000 twitter-api-client-0.7.2/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-21 23:31:46.000000 twitter-api-client-0.7.2/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.7.1/LICENSE` & `twitter-api-client-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.1/PKG-INFO` & `twitter-api-client-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.1
+Version: 0.7.2
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.7.1/setup.py` & `twitter-api-client-0.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.7.1",
+    version="0.7.2",
     python_requires=">=3.11.0",
     description="Twitter API",
     long_description=dedent('''
     Complete implementation of the undocumented Twitter API
     
     Includes tools to **scrape**, **automate**, and **search** twitter
```

### Comparing `twitter-api-client-0.7.1/twitter/account.py` & `twitter-api-client-0.7.2/twitter/account.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.1/twitter/constants.py` & `twitter-api-client-0.7.2/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.1/twitter/login.py` & `twitter-api-client-0.7.2/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.1/twitter/noauth/operation.py` & `twitter-api-client-0.7.2/twitter/noauth/operation.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.1/twitter/noauth/scraper.py` & `twitter-api-client-0.7.2/twitter/noauth/scraper.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.1/twitter/noauth/util.py` & `twitter-api-client-0.7.2/twitter/noauth/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.1/twitter/scraper.py` & `twitter-api-client-0.7.2/twitter/scraper.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.1/twitter/search.py` & `twitter-api-client-0.7.2/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.1/twitter/util.py` & `twitter-api-client-0.7.2/twitter/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     Get the headers required for authenticated requests
     """
     headers = kwargs | {
         'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
         'cookie': '; '.join(f'{k}={v}' for k, v in session.cookies.items()),
         'referer': 'https://twitter.com/',
         'user-agent': 'Mozilla/5.0 (Linux; Android 11; Nokia G20) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.88 Mobile Safari/537.36',
-        'x-csrf-token': session.cookies.get('ct0'),
-        'x-guest-token': session.cookies.get('guest_token'),
+        'x-csrf-token': session.cookies.get('ct0', ''),
+        'x-guest-token': session.cookies.get('guest_token', ''),
         'x-twitter-auth-type': 'OAuth2Session' if session.cookies.get('auth_token') else '',
         'x-twitter-active-user': 'yes',
         'x-twitter-client-language': 'en',
     }
     return dict(sorted({k.lower(): v for k, v in headers.items()}.items()))
 
 
@@ -90,8 +90,7 @@
 
         if isinstance(obj, dict) and obj:
             for k in obj:
                 L.extend(helper(obj[k], key, []))
         return L
 
     return helper(obj, key, [])
-
```

### Comparing `twitter-api-client-0.7.1/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.7.2/twitter_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.1
+Version: 0.7.2
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
```

