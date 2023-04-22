# Comparing `tmp/Anilist-0.5.0.tar.gz` & `tmp/Anilist-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Anilist-0.5.0.tar", last modified: Fri Apr 21 07:32:04 2023, max compression
+gzip compressed data, was "Anilist-0.8.0.tar", last modified: Sat Apr 22 06:31:47 2023, max compression
```

## Comparing `Anilist-0.5.0.tar` & `Anilist-0.8.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.647638 Anilist-0.5.0/
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.575798 Anilist-0.5.0/Anilist/
--rw-rw-rw-   0        0        0      164 2023-04-21 07:31:24.000000 Anilist-0.5.0/Anilist/__init__.py
--rw-rw-rw-   0        0        0      702 2023-04-21 07:19:11.000000 Anilist-0.5.0/Anilist/anilist_types.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.599784 Anilist-0.5.0/Anilist/auth/
--rw-rw-rw-   0        0        0       22 2023-04-21 03:25:44.000000 Anilist-0.5.0/Anilist/auth/__init__.py
--rw-rw-rw-   0        0        0      719 2023-04-19 21:58:46.000000 Anilist-0.5.0/Anilist/auth/auth.py
--rw-rw-rw-   0        0        0     1007 2023-04-19 23:18:58.000000 Anilist-0.5.0/Anilist/auth/code.py
--rw-rw-rw-   0        0        0      503 2023-04-21 03:30:49.000000 Anilist-0.5.0/Anilist/auth/token.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.605785 Anilist-0.5.0/Anilist/client/
--rw-rw-rw-   0        0        0       98 2023-04-21 03:31:08.000000 Anilist-0.5.0/Anilist/client/__init__.py
--rw-rw-rw-   0        0        0     1870 2023-04-21 07:28:07.000000 Anilist-0.5.0/Anilist/client/client.py
--rw-rw-rw-   0        0        0      457 2023-04-21 07:26:48.000000 Anilist-0.5.0/Anilist/client/mutation.py
--rw-rw-rw-   0        0        0      690 2023-04-21 07:24:53.000000 Anilist-0.5.0/Anilist/client/query.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.610783 Anilist-0.5.0/Anilist/errors/
--rw-rw-rw-   0        0        0       55 2023-04-21 04:04:44.000000 Anilist-0.5.0/Anilist/errors/__init__.py
--rw-rw-rw-   0        0        0      998 2023-04-21 04:21:59.000000 Anilist-0.5.0/Anilist/errors/request.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.620776 Anilist-0.5.0/Anilist/mutation/
--rw-rw-rw-   0        0        0       41 2023-04-21 03:30:29.000000 Anilist-0.5.0/Anilist/mutation/__init__.py
--rw-rw-rw-   0        0        0     1302 2023-04-19 23:39:31.000000 Anilist-0.5.0/Anilist/mutation/media_list.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.625774 Anilist-0.5.0/Anilist/query/
--rw-rw-rw-   0        0        0       38 2023-04-21 03:30:22.000000 Anilist-0.5.0/Anilist/query/__init__.py
--rw-rw-rw-   0        0        0       70 2023-04-21 06:25:57.000000 Anilist-0.5.0/Anilist/query/media_entry.py
--rw-rw-rw-   0        0        0     1844 2023-04-21 07:23:57.000000 Anilist-0.5.0/Anilist/query/media_list.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.631987 Anilist-0.5.0/Anilist/scheme/
--rw-rw-rw-   0        0        0       65 2023-04-21 03:27:28.000000 Anilist-0.5.0/Anilist/scheme/__init__.py
--rw-rw-rw-   0        0        0      149 2023-04-21 03:27:33.000000 Anilist-0.5.0/Anilist/scheme/media_scheme.py
--rw-rw-rw-   0        0        0     1900 2023-04-21 07:10:08.000000 Anilist-0.5.0/Anilist/scheme/scheme.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.638643 Anilist-0.5.0/Anilist/utils/
--rw-rw-rw-   0        0        0       92 2023-04-21 03:29:38.000000 Anilist-0.5.0/Anilist/utils/__init__.py
--rw-rw-rw-   0        0        0      190 2023-04-21 03:11:45.000000 Anilist-0.5.0/Anilist/utils/consts.py
--rw-rw-rw-   0        0        0     1571 2023-04-20 22:06:18.000000 Anilist-0.5.0/Anilist/utils/logging.py
--rw-rw-rw-   0        0        0      584 2023-04-21 03:28:31.000000 Anilist-0.5.0/Anilist/utils/object.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.642640 Anilist-0.5.0/Anilist/vars/
--rw-rw-rw-   0        0        0       22 2023-04-21 06:57:34.000000 Anilist-0.5.0/Anilist/vars/__init__.py
--rw-rw-rw-   0        0        0      455 2023-04-21 07:19:48.000000 Anilist-0.5.0/Anilist/vars/vars.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.592789 Anilist-0.5.0/Anilist.egg-info/
--rw-rw-rw-   0        0        0      563 2023-04-21 07:32:04.000000 Anilist-0.5.0/Anilist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      836 2023-04-21 07:32:04.000000 Anilist-0.5.0/Anilist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 07:32:04.000000 Anilist-0.5.0/Anilist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 07:32:04.000000 Anilist-0.5.0/Anilist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2023-04-20 22:07:52.000000 Anilist-0.5.0/LICENSE
--rw-rw-rw-   0        0        0      563 2023-04-21 07:32:04.645639 Anilist-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-20 21:05:02.000000 Anilist-0.5.0/README.md
--rw-rw-rw-   0        0        0      601 2023-04-21 07:31:33.000000 Anilist-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 07:32:04.647638 Anilist-0.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.643640 Anilist-0.5.0/tests/
--rw-rw-rw-   0        0        0      383 2023-04-21 07:15:50.000000 Anilist-0.5.0/tests/test_base.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:31:47.468289 Anilist-0.8.0/
+drwxrwxrwx   0        0        0        0 2023-04-22 06:31:47.378344 Anilist-0.8.0/Anilist/
+-rw-rw-rw-   0        0        0      164 2023-04-21 07:31:24.000000 Anilist-0.8.0/Anilist/__init__.py
+-rw-rw-rw-   0        0        0     1072 2023-04-22 06:25:28.000000 Anilist-0.8.0/Anilist/anilist_types.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:31:47.406328 Anilist-0.8.0/Anilist/auth/
+-rw-rw-rw-   0        0        0       22 2023-04-21 03:25:44.000000 Anilist-0.8.0/Anilist/auth/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-04-19 21:58:46.000000 Anilist-0.8.0/Anilist/auth/auth.py
+-rw-rw-rw-   0        0        0     1007 2023-04-19 23:18:58.000000 Anilist-0.8.0/Anilist/auth/code.py
+-rw-rw-rw-   0        0        0      503 2023-04-21 03:30:49.000000 Anilist-0.8.0/Anilist/auth/token.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:31:47.415321 Anilist-0.8.0/Anilist/client/
+-rw-rw-rw-   0        0        0       98 2023-04-21 03:31:08.000000 Anilist-0.8.0/Anilist/client/__init__.py
+-rw-rw-rw-   0        0        0     2573 2023-04-22 06:07:42.000000 Anilist-0.8.0/Anilist/client/client.py
+-rw-rw-rw-   0        0        0      477 2023-04-21 20:55:21.000000 Anilist-0.8.0/Anilist/client/mutation.py
+-rw-rw-rw-   0        0        0      923 2023-04-22 03:59:01.000000 Anilist-0.8.0/Anilist/client/query.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:31:47.420318 Anilist-0.8.0/Anilist/errors/
+-rw-rw-rw-   0        0        0       55 2023-04-21 04:04:44.000000 Anilist-0.8.0/Anilist/errors/__init__.py
+-rw-rw-rw-   0        0        0      998 2023-04-21 04:21:59.000000 Anilist-0.8.0/Anilist/errors/request.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:31:47.427314 Anilist-0.8.0/Anilist/mutation/
+-rw-rw-rw-   0        0        0       41 2023-04-21 03:30:29.000000 Anilist-0.8.0/Anilist/mutation/__init__.py
+-rw-rw-rw-   0        0        0      962 2023-04-22 06:24:47.000000 Anilist-0.8.0/Anilist/mutation/media_list.py
+-rw-rw-rw-   0        0        0      393 2023-04-22 06:22:20.000000 Anilist-0.8.0/Anilist/mutation/mutable.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:31:47.436309 Anilist-0.8.0/Anilist/query/
+-rw-rw-rw-   0        0        0       80 2023-04-22 01:33:28.000000 Anilist-0.8.0/Anilist/query/__init__.py
+-rw-rw-rw-   0        0        0      574 2023-04-22 04:10:12.000000 Anilist-0.8.0/Anilist/query/media_entry.py
+-rw-rw-rw-   0        0        0      624 2023-04-22 04:10:00.000000 Anilist-0.8.0/Anilist/query/media_list.py
+-rw-rw-rw-   0        0        0     3252 2023-04-22 06:06:26.000000 Anilist-0.8.0/Anilist/query/query.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:31:47.443304 Anilist-0.8.0/Anilist/scheme/
+-rw-rw-rw-   0        0        0      112 2023-04-22 01:40:50.000000 Anilist-0.8.0/Anilist/scheme/__init__.py
+-rw-rw-rw-   0        0        0      662 2023-04-22 01:52:21.000000 Anilist-0.8.0/Anilist/scheme/media_scheme.py
+-rw-rw-rw-   0        0        0     2234 2023-04-21 20:53:49.000000 Anilist-0.8.0/Anilist/scheme/scheme.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:31:47.456296 Anilist-0.8.0/Anilist/utils/
+-rw-rw-rw-   0        0        0       92 2023-04-21 03:29:38.000000 Anilist-0.8.0/Anilist/utils/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-04-21 03:11:45.000000 Anilist-0.8.0/Anilist/utils/consts.py
+-rw-rw-rw-   0        0        0     1571 2023-04-20 22:06:18.000000 Anilist-0.8.0/Anilist/utils/logging.py
+-rw-rw-rw-   0        0        0      652 2023-04-21 20:02:38.000000 Anilist-0.8.0/Anilist/utils/object.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:31:47.462293 Anilist-0.8.0/Anilist/vars/
+-rw-rw-rw-   0        0        0       22 2023-04-21 06:57:34.000000 Anilist-0.8.0/Anilist/vars/__init__.py
+-rw-rw-rw-   0        0        0     1119 2023-04-22 06:23:55.000000 Anilist-0.8.0/Anilist/vars/vars.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:31:47.398333 Anilist-0.8.0/Anilist.egg-info/
+-rw-rw-rw-   0        0        0      563 2023-04-22 06:31:47.000000 Anilist-0.8.0/Anilist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      887 2023-04-22 06:31:47.000000 Anilist-0.8.0/Anilist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 06:31:47.000000 Anilist-0.8.0/Anilist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-22 06:31:47.000000 Anilist-0.8.0/Anilist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2023-04-20 22:07:52.000000 Anilist-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0      563 2023-04-22 06:31:47.467289 Anilist-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-20 21:05:02.000000 Anilist-0.8.0/README.md
+-rw-rw-rw-   0        0        0      601 2023-04-22 06:31:25.000000 Anilist-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-22 06:31:47.469288 Anilist-0.8.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-22 06:31:47.464293 Anilist-0.8.0/tests/
+-rw-rw-rw-   0        0        0     1333 2023-04-22 06:24:01.000000 Anilist-0.8.0/tests/test_base.py
```

### Comparing `Anilist-0.5.0/Anilist/anilist_types.py` & `Anilist-0.8.0/Anilist/anilist_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,46 @@
 class AnilistType:
     def __new__(cls, v):
         if cls == AnilistType:
             if type(v) is str: 
                 return AnilistString(None)
             if type(v) is int:
                 return AnilistInt(None)
-            if issubclass(v, AnilistType):
+            if type(v) is float:
+                return AnilistFloat(None)
+            if isinstance(v, AnilistType):
                 return v
         else:
             return super().__new__(cls)
 
     def __str__(self):
-        print(self.__class__)
         return self.__class__.ANILIST_TYPE_NAME
     
     def __repr__(self):
         return str(self)
+    
+    def get_inner(self):
+        return None
 
 class AnilistString(AnilistType):
     
     ANILIST_TYPE_NAME = "String"
 
 class AnilistInt(AnilistType):
 
     ANILIST_TYPE_NAME = "Int"
 
+class AnilistFloat(AnilistType):
+
+    ANILIST_TYPE_NAME = "Float"
+
+class AnilistMediaType(AnilistType):
+    
+    ANILIST_TYPE_NAME = "MediaType"
+
+    def __init__(self, s):
+        self._inner = s
+
+    def get_inner(self):
+        return self._inner
+    
+
```

### Comparing `Anilist-0.5.0/Anilist/auth/auth.py` & `Anilist-0.8.0/Anilist/auth/auth.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.5.0/Anilist/auth/code.py` & `Anilist-0.8.0/Anilist/auth/code.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.5.0/Anilist/client/client.py` & `Anilist-0.8.0/Anilist/client/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,73 @@
 import requests, logging
 from Anilist.scheme.scheme import Scheme
 
 from Anilist.utils import AnilistObject, AnilistLogger, consts
 from Anilist.errors import RequestError
+from Anilist.vars.vars import Vars
 class Client:
 
     URI = consts.API_URI
     DEFAULT_HEADERS = consts.DEFAULT_HEADERS
 
-    def __init__(self, auth, level):
+    def __init__(self, auth, level, max_pages=100):
         self._auth = auth
         self._headers = None
+        self._max = max_pages
         _ = AnilistLogger(level)
 
-    def _request(self, query, vars):
+    def _page_request(self, query, vars: Vars, k, f=lambda x: x):        
+        pg = vars._json["page"]
+
+        temp = []
+
+        while pg <= self._max:
+            resp = self._request(query, vars)
+            data = ([f(v) for v in resp.Page[k]])
+
+            temp.extend(data)
+
+            if data == []:
+                break
+
+            pg += 1
+            vars.update("page", pg)
+
+        return temp
+
+    def _request(self, query, vars: Vars):
 
         log = AnilistLogger()
         log.info(f"Sending request to URI {self.URI} with headers {self.headers}")
         log.debug(f"The query is {query}\n The variables are {vars}")
         
         req = requests.post(self.URI, json={
             "query": query,
-            "variables": vars,
+            "variables": vars._json,
         }, headers = self.headers)
 
         resp = req.json()
 
         log.info(f"Received response to request with status code {req.status_code}")
 
         if "errors" in resp and resp["errors"] != []:
             raise RequestError.from_json(resp["errors"][0])
         
         obj = AnilistObject(resp["data"])
         return obj
         
     def _create_query(self, vars, *schs, head_sch=None):
         schs = list(schs) if head_sch is None else [Scheme._combine(head_sch, sch) for sch in schs]
-
-        query = """
+        if vars._names == "":
+            return """
+            {} {{
+                {}
+            }}
+            """.format(self._query_type(), Scheme._construct(*schs))
+        return """
             {} ({}) {{
                 {}
             }}
         """.format(self._query_type(), vars._names, Scheme._construct(*schs))
 
         return query
```

### Comparing `Anilist-0.5.0/Anilist/client/query.py` & `Anilist-0.8.0/Anilist/client/query.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,31 @@
     
 from Anilist.client import Client
-from Anilist.query.media_list import MediaListQuery
+from Anilist.query import MediaEntryQuery
+from Anilist.query import MediaListQuery
 
 import logging
 
 from Anilist.vars.vars import Vars
 
 class QueryClient(Client):
-
-    def __init__(self, level=logging.INFO):
-        Client.__init__(self, None, level)
+    """
+    A hub that creates various interfaces that interact with the Anilist API
+    """
+
+    def __init__(self, level=logging.INFO, **kwargs):
+        """
+        Parameters
+        ----------
+        level : int
+            The logging level for this client
+        """
+        Client.__init__(self, None, level, **kwargs)
 
     def _query_type(self):
         return "query"
 
-    def media_list(self, *, username, per_page: int=10, starting_page: int=1, languages=["english"], sizes=["extraLarge"]):
-        return MediaListQuery(
-            client=self,
-            username=username, 
-            per_page=per_page, 
-            starting_page=starting_page, 
-            languages=languages, 
-            sizes=sizes
-        )
+    def media_list(self, *, languages=["english"], sizes=["extraLarge"]):
+        return MediaListQuery(client=self, languages=languages, sizes=sizes)
+    
+    def media_entry(self, *, languages=["english"], sizes=["extraLarge"]):
+        return MediaEntryQuery(client=self, languages=languages, sizes=sizes)
```

### Comparing `Anilist-0.5.0/Anilist/errors/request.py` & `Anilist-0.8.0/Anilist/errors/request.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.5.0/Anilist/scheme/scheme.py` & `Anilist-0.8.0/Anilist/scheme/scheme.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,26 @@
     
     def __call__(self, **kwargs):
         d = dict(**kwargs)
         if d != {}:
             self._up[self._layers[-1]] = f"{self._layers[-1]} ({', '.join([f'{k}: {v}' for k, v in d.items()])})"
         return self
     
+    def _replace_head(self, pat, r):
+        self._layers[0] = str(self._layers[0]).replace(pat, r)
+        tch = []
+        for k, v in self._up.items():
+            if k == pat:
+                tch.append(k)
+
+        for k in tch:
+            self._up[r] = str(self._up.pop(k)).replace(pat, r)
+
+        return self
+    
     @classmethod
     def _construct(cls, *schs):
         d = {k: v for sch in schs for k, v in sch._up.items()}
         return construct_query_as_string(construct_query(list(schs)), d)
     
     @classmethod
     def _combine(cls, scha, schb):
```

### Comparing `Anilist-0.5.0/Anilist/utils/logging.py` & `Anilist-0.8.0/Anilist/utils/logging.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.5.0/Anilist/utils/object.py` & `Anilist-0.8.0/Anilist/utils/object.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,12 +9,15 @@
                 self.__dict[k] = [AnilistObject(el) if type(el) is dict else el for el in v]
             else:
                 self.__dict[k] = v
 
     def __getattr__(self, k):
         return self.__dict[k]
     
+    def __getitem__(self, k):
+        return self.__dict[k]
+    
     def __str__(self):
         return str(self.__dict)
     
     def __repr__(self):
         return str(self)
```

### Comparing `Anilist-0.5.0/Anilist.egg-info/PKG-INFO` & `Anilist-0.8.0/Anilist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Anilist
-Version: 0.5.0
+Version: 0.8.0
 Summary: Anilist API wrapper
 Author-email: Ann Mauduy-Decius <ann.mauduy.decius@gmail.com>
 Project-URL: Homepage, https://github.com/xxxAnn/Anilist.py
 Project-URL: Bug Tracker, https://github.com/xxxAnn/Anilist.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Anilist-0.5.0/Anilist.egg-info/SOURCES.txt` & `Anilist-0.8.0/Anilist.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 Anilist/client/client.py
 Anilist/client/mutation.py
 Anilist/client/query.py
 Anilist/errors/__init__.py
 Anilist/errors/request.py
 Anilist/mutation/__init__.py
 Anilist/mutation/media_list.py
+Anilist/mutation/mutable.py
 Anilist/query/__init__.py
 Anilist/query/media_entry.py
 Anilist/query/media_list.py
+Anilist/query/query.py
 Anilist/scheme/__init__.py
 Anilist/scheme/media_scheme.py
 Anilist/scheme/scheme.py
 Anilist/utils/__init__.py
 Anilist/utils/consts.py
 Anilist/utils/logging.py
 Anilist/utils/object.py
```

### Comparing `Anilist-0.5.0/LICENSE` & `Anilist-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Anilist-0.5.0/PKG-INFO` & `Anilist-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Anilist
-Version: 0.5.0
+Version: 0.8.0
 Summary: Anilist API wrapper
 Author-email: Ann Mauduy-Decius <ann.mauduy.decius@gmail.com>
 Project-URL: Homepage, https://github.com/xxxAnn/Anilist.py
 Project-URL: Bug Tracker, https://github.com/xxxAnn/Anilist.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Anilist-0.5.0/pyproject.toml` & `Anilist-0.8.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Anilist"
-version = "0.5.0"
+version = "0.8.0"
 authors = [
   { name="Ann Mauduy-Decius", email="ann.mauduy.decius@gmail.com" },
 ]
 description = "Anilist API wrapper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

