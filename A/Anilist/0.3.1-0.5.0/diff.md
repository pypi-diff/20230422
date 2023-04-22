# Comparing `tmp/Anilist-0.3.1.tar.gz` & `tmp/Anilist-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Anilist-0.3.1.tar", last modified: Fri Apr 21 03:22:07 2023, max compression
+gzip compressed data, was "Anilist-0.5.0.tar", last modified: Fri Apr 21 07:32:04 2023, max compression
```

## Comparing `Anilist-0.3.1.tar` & `Anilist-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.211926 Anilist-0.3.1/
-drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.124981 Anilist-0.3.1/Anilist/
--rw-rw-rw-   0        0        0      127 2023-04-21 03:20:18.000000 Anilist-0.3.1/Anilist/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.160957 Anilist-0.3.1/Anilist/auth/
--rw-rw-rw-   0        0        0      719 2023-04-19 21:58:46.000000 Anilist-0.3.1/Anilist/auth/auth.py
--rw-rw-rw-   0        0        0     1007 2023-04-19 23:18:58.000000 Anilist-0.3.1/Anilist/auth/code.py
--rw-rw-rw-   0        0        0      497 2023-04-19 21:18:07.000000 Anilist-0.3.1/Anilist/auth/token.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.197934 Anilist-0.3.1/Anilist/client/
--rw-rw-rw-   0        0        0       96 2023-04-21 03:19:41.000000 Anilist-0.3.1/Anilist/client/__init__.py
--rw-rw-rw-   0        0        0     1383 2023-04-21 03:20:24.000000 Anilist-0.3.1/Anilist/client/client.py
--rw-rw-rw-   0        0        0      365 2023-04-21 03:19:10.000000 Anilist-0.3.1/Anilist/client/mutation.py
--rw-rw-rw-   0        0        0      577 2023-04-21 03:20:31.000000 Anilist-0.3.1/Anilist/client/query.py
--rw-rw-rw-   0        0        0      190 2023-04-21 03:11:45.000000 Anilist-0.3.1/Anilist/consts.py
--rw-rw-rw-   0        0        0     1571 2023-04-20 22:06:18.000000 Anilist-0.3.1/Anilist/logging.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.199933 Anilist-0.3.1/Anilist/mutation/
--rw-rw-rw-   0        0        0        0 2023-04-19 21:32:11.000000 Anilist-0.3.1/Anilist/mutation/__init__.py
--rw-rw-rw-   0        0        0     1302 2023-04-19 23:39:31.000000 Anilist-0.3.1/Anilist/mutation/media_list.py
--rw-rw-rw-   0        0        0      599 2023-04-20 21:27:29.000000 Anilist-0.3.1/Anilist/object.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.203930 Anilist-0.3.1/Anilist/query/
--rw-rw-rw-   0        0        0        0 2023-04-19 23:42:28.000000 Anilist-0.3.1/Anilist/query/__init__.py
--rw-rw-rw-   0        0        0     1933 2023-04-21 00:03:00.000000 Anilist-0.3.1/Anilist/query/media_list.py
--rw-rw-rw-   0        0        0     2007 2023-04-21 03:14:07.000000 Anilist-0.3.1/Anilist/scheme.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.152962 Anilist-0.3.1/Anilist.egg-info/
--rw-rw-rw-   0        0        0      563 2023-04-21 03:22:07.000000 Anilist-0.3.1/Anilist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-04-21 03:22:07.000000 Anilist-0.3.1/Anilist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 03:22:07.000000 Anilist-0.3.1/Anilist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 03:22:07.000000 Anilist-0.3.1/Anilist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2023-04-20 22:07:52.000000 Anilist-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      563 2023-04-21 03:22:07.210926 Anilist-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-20 21:05:02.000000 Anilist-0.3.1/README.md
--rw-rw-rw-   0        0        0      601 2023-04-21 03:07:29.000000 Anilist-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 03:22:07.211926 Anilist-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.208928 Anilist-0.3.1/tests/
--rw-rw-rw-   0        0        0      383 2023-04-21 03:16:41.000000 Anilist-0.3.1/tests/test_base.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.647638 Anilist-0.5.0/
+drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.575798 Anilist-0.5.0/Anilist/
+-rw-rw-rw-   0        0        0      164 2023-04-21 07:31:24.000000 Anilist-0.5.0/Anilist/__init__.py
+-rw-rw-rw-   0        0        0      702 2023-04-21 07:19:11.000000 Anilist-0.5.0/Anilist/anilist_types.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.599784 Anilist-0.5.0/Anilist/auth/
+-rw-rw-rw-   0        0        0       22 2023-04-21 03:25:44.000000 Anilist-0.5.0/Anilist/auth/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-04-19 21:58:46.000000 Anilist-0.5.0/Anilist/auth/auth.py
+-rw-rw-rw-   0        0        0     1007 2023-04-19 23:18:58.000000 Anilist-0.5.0/Anilist/auth/code.py
+-rw-rw-rw-   0        0        0      503 2023-04-21 03:30:49.000000 Anilist-0.5.0/Anilist/auth/token.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.605785 Anilist-0.5.0/Anilist/client/
+-rw-rw-rw-   0        0        0       98 2023-04-21 03:31:08.000000 Anilist-0.5.0/Anilist/client/__init__.py
+-rw-rw-rw-   0        0        0     1870 2023-04-21 07:28:07.000000 Anilist-0.5.0/Anilist/client/client.py
+-rw-rw-rw-   0        0        0      457 2023-04-21 07:26:48.000000 Anilist-0.5.0/Anilist/client/mutation.py
+-rw-rw-rw-   0        0        0      690 2023-04-21 07:24:53.000000 Anilist-0.5.0/Anilist/client/query.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.610783 Anilist-0.5.0/Anilist/errors/
+-rw-rw-rw-   0        0        0       55 2023-04-21 04:04:44.000000 Anilist-0.5.0/Anilist/errors/__init__.py
+-rw-rw-rw-   0        0        0      998 2023-04-21 04:21:59.000000 Anilist-0.5.0/Anilist/errors/request.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.620776 Anilist-0.5.0/Anilist/mutation/
+-rw-rw-rw-   0        0        0       41 2023-04-21 03:30:29.000000 Anilist-0.5.0/Anilist/mutation/__init__.py
+-rw-rw-rw-   0        0        0     1302 2023-04-19 23:39:31.000000 Anilist-0.5.0/Anilist/mutation/media_list.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.625774 Anilist-0.5.0/Anilist/query/
+-rw-rw-rw-   0        0        0       38 2023-04-21 03:30:22.000000 Anilist-0.5.0/Anilist/query/__init__.py
+-rw-rw-rw-   0        0        0       70 2023-04-21 06:25:57.000000 Anilist-0.5.0/Anilist/query/media_entry.py
+-rw-rw-rw-   0        0        0     1844 2023-04-21 07:23:57.000000 Anilist-0.5.0/Anilist/query/media_list.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.631987 Anilist-0.5.0/Anilist/scheme/
+-rw-rw-rw-   0        0        0       65 2023-04-21 03:27:28.000000 Anilist-0.5.0/Anilist/scheme/__init__.py
+-rw-rw-rw-   0        0        0      149 2023-04-21 03:27:33.000000 Anilist-0.5.0/Anilist/scheme/media_scheme.py
+-rw-rw-rw-   0        0        0     1900 2023-04-21 07:10:08.000000 Anilist-0.5.0/Anilist/scheme/scheme.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.638643 Anilist-0.5.0/Anilist/utils/
+-rw-rw-rw-   0        0        0       92 2023-04-21 03:29:38.000000 Anilist-0.5.0/Anilist/utils/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-04-21 03:11:45.000000 Anilist-0.5.0/Anilist/utils/consts.py
+-rw-rw-rw-   0        0        0     1571 2023-04-20 22:06:18.000000 Anilist-0.5.0/Anilist/utils/logging.py
+-rw-rw-rw-   0        0        0      584 2023-04-21 03:28:31.000000 Anilist-0.5.0/Anilist/utils/object.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.642640 Anilist-0.5.0/Anilist/vars/
+-rw-rw-rw-   0        0        0       22 2023-04-21 06:57:34.000000 Anilist-0.5.0/Anilist/vars/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-04-21 07:19:48.000000 Anilist-0.5.0/Anilist/vars/vars.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.592789 Anilist-0.5.0/Anilist.egg-info/
+-rw-rw-rw-   0        0        0      563 2023-04-21 07:32:04.000000 Anilist-0.5.0/Anilist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      836 2023-04-21 07:32:04.000000 Anilist-0.5.0/Anilist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 07:32:04.000000 Anilist-0.5.0/Anilist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 07:32:04.000000 Anilist-0.5.0/Anilist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2023-04-20 22:07:52.000000 Anilist-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0      563 2023-04-21 07:32:04.645639 Anilist-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-20 21:05:02.000000 Anilist-0.5.0/README.md
+-rw-rw-rw-   0        0        0      601 2023-04-21 07:31:33.000000 Anilist-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 07:32:04.647638 Anilist-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 07:32:04.643640 Anilist-0.5.0/tests/
+-rw-rw-rw-   0        0        0      383 2023-04-21 07:15:50.000000 Anilist-0.5.0/tests/test_base.py
```

### Comparing `Anilist-0.3.1/Anilist/auth/auth.py` & `Anilist-0.5.0/Anilist/auth/auth.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.3.1/Anilist/auth/code.py` & `Anilist-0.5.0/Anilist/auth/code.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.3.1/Anilist/client/query.py` & `Anilist-0.5.0/Anilist/client/query.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,25 @@
     
 from Anilist.client import Client
 from Anilist.query.media_list import MediaListQuery
 
+import logging
+
+from Anilist.vars.vars import Vars
 
 class QueryClient(Client):
 
-    def __init__(self, level):
+    def __init__(self, level=logging.INFO):
         Client.__init__(self, None, level)
 
+    def _query_type(self):
+        return "query"
+
     def media_list(self, *, username, per_page: int=10, starting_page: int=1, languages=["english"], sizes=["extraLarge"]):
         return MediaListQuery(
             client=self,
             username=username, 
             per_page=per_page, 
             starting_page=starting_page, 
             languages=languages, 
             sizes=sizes
         )
-
-
```

### Comparing `Anilist-0.3.1/Anilist/logging.py` & `Anilist-0.5.0/Anilist/utils/logging.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.3.1/Anilist/mutation/media_list.py` & `Anilist-0.5.0/Anilist/mutation/media_list.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.3.1/Anilist/object.py` & `Anilist-0.5.0/Anilist/utils/object.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import json
-
 class AnilistObject:
     
     def __init__(self, json_object):
         self.__dict = {}
         for k, v in json_object.items():
             if type(v) is dict:
                 self.__dict[k] = AnilistObject(v)
```

### Comparing `Anilist-0.3.1/Anilist/query/media_list.py` & `Anilist-0.5.0/Anilist/query/media_list.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from Anilist.scheme import MediaScheme, Scheme
+from Anilist.vars.vars import Vars
 class MediaListQuery:
     
     def __init__(self, client, username: str, per_page: int=10, starting_page: int = 1, languages=["english"], sizes=["extraLarge"]):
         self._username = username
         self._per_page = per_page
         self._starting_page = starting_page
         self._languages = languages
@@ -10,15 +11,16 @@
         self._sizes = sizes
         self._media_entries = []
         self.DEFAULT_QUERY = [
             MediaScheme().id, 
             *[MediaScheme().title[lang] for lang in self._languages], 
             *[MediaScheme().coverImage[size] for size in self._sizes]
         ]
-        # load a few important values
+        self.DEFAULT_VARS = Vars(usr=self._username, page=self._starting_page, perPage=self._per_page)
+        # load default values
         self._base_query()
 
     @property
     def entries(self):
         return self._media_entries
     
     def query(self, *schs, default=True):
@@ -26,42 +28,34 @@
         if default:
             schs = list(schs)
             schs.extend(self.DEFAULT_QUERY)
 
         return self._query(*schs)
     
     def _query(self, *schs):
-        query = """
-        query ($usr: String, $page: Int, $perPage: Int) {{
-            Page (page: $page, perPage: $perPage) {{
-                mediaList (userName: $usr) {{
-                    {0}
-                }}
-            }}
-        }}
-        """.format(Scheme._construct(*schs))
-
-        vars = {
-            "usr": self._username,
-            "page": self._starting_page,
-            "perPage": self._per_page
-        }
+
+        head_sch = Scheme().Page(page="$page", perPage="$perPage").mediaList(userName="$usr")
+
+        query = self._client._create_query(self.DEFAULT_VARS, *schs, head_sch=head_sch)
 
         pg = self._starting_page
+        
+        vals = self.DEFAULT_VARS._json
+
         temp = []
 
         while True:
-            resp = self._client._request(query, vars=vars)
+            resp = self._client._request(query, vars=vals)
             data = ([v.media for v in resp.Page.mediaList])
 
             temp.extend(data)
 
             if data == []:
                 break
 
             pg += 1
-            vars["page"] = pg
+            vals["page"] = pg
 
         self._media_entries = temp
 
     def _base_query(self):
-        self.query(default=True)
+        self.query()
```

### Comparing `Anilist-0.3.1/Anilist/scheme.py` & `Anilist-0.5.0/Anilist/scheme/scheme.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 class Scheme:
+
     def __init__(self):
         self._layers = []
         self._up = {}
 
     def __getattr__(self, k):
         return self[k]
     
@@ -14,16 +15,23 @@
         d = dict(**kwargs)
         if d != {}:
             self._up[self._layers[-1]] = f"{self._layers[-1]} ({', '.join([f'{k}: {v}' for k, v in d.items()])})"
         return self
     
     @classmethod
     def _construct(cls, *schs):
-        return construct_query_as_string(construct_query(list(schs)), [sch._up for sch in schs])
+        d = {k: v for sch in schs for k, v in sch._up.items()}
+        return construct_query_as_string(construct_query(list(schs)), d)
     
+    @classmethod
+    def _combine(cls, scha, schb):
+        n = cls()
+        n._layers = scha._layers + schb._layers
+        n._up = scha._up | schb._up
+        return n
     
 def construct_query(schs: list[Scheme]):
     temp = {}
 
     for sch in schs:
         sch = sch._layers
         if not sch[0] in temp:
@@ -31,33 +39,29 @@
         for i in range(1, len(sch)):
             if not sch[i] in get_nest_list(get_numbers_up_to(i), temp, i, sch):
                 get_nest_list(get_numbers_up_to(i), temp, i, sch)[sch[i]] = {}
 
     
     return temp
 
-REPLACE = "__SPECIAL_KEY_REPLACE__"
 
 def construct_query_as_string(d, l, ss=""):
     if type(d) != dict:
         return str(d)
+    
     s = ""
+
     for k, v in d.items():
+        nk = k if k not in l else l[k]
         if v == {}:
-            s = f"{s}{ss}{REPLACE}{k}\n"
+            s = f"{s}{ss}{nk}\n"
         else:
             t = construct_query_as_string(v, l, f'{ss}  ')
             t = t[0:-1]
-            s = f"{s}{ss}{REPLACE}{k} {{\n{t}\n{ss}}}\n"
-
-    if ss == "":
-        for dic in l:
-            for k, v in dic.items():
-                s = s.replace(f"{REPLACE}{k}", f"{v}")
-        s = s.replace(f"{REPLACE}", "")
+            s = f"{s}{ss}{nk} {{\n{t}\n{ss}}}\n"
 
     return s
 
 
 def get_numbers_up_to(i):
     l = []
     n = i
@@ -69,13 +73,7 @@
 
 def get_nest_list(n, l, m, sch):
     prev = l
     for i in n:
         prev = prev[sch[m-i]]
     return prev
     
-    # a b e
-    # a d v
-class MediaScheme(Scheme):
-    def __init__(self):
-        super().__init__()
-        self._layers.append("media")
```

### Comparing `Anilist-0.3.1/Anilist.egg-info/PKG-INFO` & `Anilist-0.5.0/Anilist.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Anilist
-Version: 0.3.1
+Version: 0.5.0
 Summary: Anilist API wrapper
 Author-email: Ann Mauduy-Decius <ann.mauduy.decius@gmail.com>
 Project-URL: Homepage, https://github.com/xxxAnn/Anilist.py
 Project-URL: Bug Tracker, https://github.com/xxxAnn/Anilist.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Anilist-0.3.1/Anilist.egg-info/SOURCES.txt` & `Anilist-0.5.0/Anilist.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 LICENSE
 README.md
 pyproject.toml
 Anilist/__init__.py
-Anilist/consts.py
-Anilist/logging.py
-Anilist/object.py
-Anilist/scheme.py
+Anilist/anilist_types.py
 Anilist.egg-info/PKG-INFO
 Anilist.egg-info/SOURCES.txt
 Anilist.egg-info/dependency_links.txt
 Anilist.egg-info/top_level.txt
+Anilist/auth/__init__.py
 Anilist/auth/auth.py
 Anilist/auth/code.py
 Anilist/auth/token.py
 Anilist/client/__init__.py
 Anilist/client/client.py
 Anilist/client/mutation.py
 Anilist/client/query.py
+Anilist/errors/__init__.py
+Anilist/errors/request.py
 Anilist/mutation/__init__.py
 Anilist/mutation/media_list.py
 Anilist/query/__init__.py
+Anilist/query/media_entry.py
 Anilist/query/media_list.py
+Anilist/scheme/__init__.py
+Anilist/scheme/media_scheme.py
+Anilist/scheme/scheme.py
+Anilist/utils/__init__.py
+Anilist/utils/consts.py
+Anilist/utils/logging.py
+Anilist/utils/object.py
+Anilist/vars/__init__.py
+Anilist/vars/vars.py
 tests/test_base.py
```

### Comparing `Anilist-0.3.1/LICENSE` & `Anilist-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Anilist-0.3.1/PKG-INFO` & `Anilist-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Anilist
-Version: 0.3.1
+Version: 0.5.0
 Summary: Anilist API wrapper
 Author-email: Ann Mauduy-Decius <ann.mauduy.decius@gmail.com>
 Project-URL: Homepage, https://github.com/xxxAnn/Anilist.py
 Project-URL: Bug Tracker, https://github.com/xxxAnn/Anilist.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Anilist-0.3.1/pyproject.toml` & `Anilist-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Anilist"
-version = "0.3.1"
+version = "0.5.0"
 authors = [
   { name="Ann Mauduy-Decius", email="ann.mauduy.decius@gmail.com" },
 ]
 description = "Anilist API wrapper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

