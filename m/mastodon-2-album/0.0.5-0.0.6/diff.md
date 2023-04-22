# Comparing `tmp/mastodon_2_album-0.0.5.tar.gz` & `tmp/mastodon_2_album-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mastodon_2_album-0.0.5.tar", last modified: Thu Feb 23 02:50:42 2023, max compression
+gzip compressed data, was "mastodon_2_album-0.0.6.tar", last modified: Sat Apr 22 00:56:07 2023, max compression
```

## Comparing `mastodon_2_album-0.0.5.tar` & `mastodon_2_album-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-02-23 02:50:42.000000 mastodon_2_album-0.0.5/
--rw-r--r--   0 user       (501) staff       (20)     1071 2023-02-22 14:28:17.000000 mastodon_2_album-0.0.5/LICENSE
--rw-r--r--   0 user       (501) staff       (20)      749 2023-02-23 02:50:42.000000 mastodon_2_album-0.0.5/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      238 2023-02-22 14:32:02.000000 mastodon_2_album-0.0.5/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-02-23 02:50:42.000000 mastodon_2_album-0.0.5/mastodon_2_album/
--rw-r--r--   0 user       (501) staff       (20)     4487 2023-02-23 02:50:14.000000 mastodon_2_album-0.0.5/mastodon_2_album/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-02-23 02:50:42.000000 mastodon_2_album-0.0.5/mastodon_2_album.egg-info/
--rw-r--r--   0 user       (501) staff       (20)      749 2023-02-23 02:50:42.000000 mastodon_2_album-0.0.5/mastodon_2_album.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      254 2023-02-23 02:50:42.000000 mastodon_2_album-0.0.5/mastodon_2_album.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-02-23 02:50:42.000000 mastodon_2_album-0.0.5/mastodon_2_album.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       18 2023-02-23 02:50:42.000000 mastodon_2_album-0.0.5/mastodon_2_album.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       17 2023-02-23 02:50:42.000000 mastodon_2_album-0.0.5/mastodon_2_album.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)       38 2023-02-23 02:50:42.000000 mastodon_2_album-0.0.5/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      759 2023-02-23 02:50:40.000000 mastodon_2_album-0.0.5/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-04-22 00:56:07.000000 mastodon_2_album-0.0.6/
+-rw-r--r--   0 user       (501) staff       (20)     1071 2023-02-22 14:28:17.000000 mastodon_2_album-0.0.6/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)      749 2023-04-22 00:56:07.000000 mastodon_2_album-0.0.6/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      238 2023-02-22 14:32:02.000000 mastodon_2_album-0.0.6/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-04-22 00:56:07.000000 mastodon_2_album-0.0.6/mastodon_2_album/
+-rw-r--r--   0 user       (501) staff       (20)     4659 2023-04-22 00:54:40.000000 mastodon_2_album-0.0.6/mastodon_2_album/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-04-22 00:56:07.000000 mastodon_2_album-0.0.6/mastodon_2_album.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)      749 2023-04-22 00:56:07.000000 mastodon_2_album-0.0.6/mastodon_2_album.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      254 2023-04-22 00:56:07.000000 mastodon_2_album-0.0.6/mastodon_2_album.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-04-22 00:56:07.000000 mastodon_2_album-0.0.6/mastodon_2_album.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       18 2023-04-22 00:56:07.000000 mastodon_2_album-0.0.6/mastodon_2_album.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       17 2023-04-22 00:56:07.000000 mastodon_2_album-0.0.6/mastodon_2_album.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-04-22 00:56:07.000000 mastodon_2_album-0.0.6/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      759 2023-04-22 00:56:05.000000 mastodon_2_album-0.0.6/setup.py
```

### Comparing `mastodon_2_album-0.0.5/LICENSE` & `mastodon_2_album-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mastodon_2_album-0.0.5/PKG-INFO` & `mastodon_2_album-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mastodon_2_album
-Version: 0.0.5
+Version: 0.0.6
 Summary: Return photo list and caption (markdown format) from mastodon.
 Home-page: https://github.com/gaoyunzhi/mastodon_2_album
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mastodon_2_album-0.0.5/mastodon_2_album/__init__.py` & `mastodon_2_album-0.0.6/mastodon_2_album/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,20 @@
     r = Result()
     r.imgs = getImages(status)
     r.video = getVideo(status)
     r.cap_html_v2 = getCap(status)
     r.url = getUrl(status)
     return r
 
+def getFromUrl(mastodon, url):
+    for status in mastodon.search_v2(url)['statuses']:
+        if getUrl(status) == url:
+            return get(status)
+    return Result()
+
 def getHash(status):
     cap = getContentText(status)
     origin_cap = getOriginCap(status)
     raw_content = origin_cap + cap
     raw_content += ''.join(getImages(status))
     raw_content += str(getVideo(status))
     result = []
```

### Comparing `mastodon_2_album-0.0.5/mastodon_2_album.egg-info/PKG-INFO` & `mastodon_2_album-0.0.6/mastodon_2_album.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mastodon-2-album
-Version: 0.0.5
+Version: 0.0.6
 Summary: Return photo list and caption (markdown format) from mastodon.
 Home-page: https://github.com/gaoyunzhi/mastodon_2_album
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mastodon_2_album-0.0.5/setup.py` & `mastodon_2_album-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mastodon_2_album",
-    version="0.0.5",
+    version="0.0.6",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Return photo list and caption (markdown format) from mastodon.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/mastodon_2_album",
     packages=setuptools.find_packages(),
```

