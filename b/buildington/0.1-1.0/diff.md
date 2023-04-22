# Comparing `tmp/buildington-0.1.tar.gz` & `tmp/buildington-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildington-0.1.tar", last modified: Sat Apr 22 11:15:39 2023, max compression
+gzip compressed data, was "buildington-1.0.tar", last modified: Sat Apr 22 11:02:58 2023, max compression
```

## Comparing `buildington-0.1.tar` & `buildington-1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 11:15:39.786949 buildington-0.1/
--rw-rw-rw-   0        0        0      482 2023-04-22 11:15:39.771327 buildington-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-22 11:15:39.708823 buildington-0.1/buildington/
--rw-rw-rw-   0        0        0     3544 2023-04-22 11:14:56.000000 buildington-0.1/buildington/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 11:15:39.771327 buildington-0.1/buildington.egg-info/
--rw-rw-rw-   0        0        0      482 2023-04-22 11:15:39.000000 buildington-0.1/buildington.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-04-22 11:15:39.000000 buildington-0.1/buildington.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 11:15:39.000000 buildington-0.1/buildington.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-22 11:15:39.000000 buildington-0.1/buildington.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-22 11:15:39.000000 buildington-0.1/buildington.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 11:15:39.786949 buildington-0.1/setup.cfg
--rw-rw-rw-   0        0        0      556 2023-04-22 11:15:02.000000 buildington-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 11:02:58.830696 buildington-1.0/
+-rw-rw-rw-   0        0        0      482 2023-04-22 11:02:58.830696 buildington-1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-22 11:02:58.768183 buildington-1.0/buildington/
+-rw-rw-rw-   0        0        0     3538 2023-04-22 10:49:35.000000 buildington-1.0/buildington/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 11:02:58.830696 buildington-1.0/buildington.egg-info/
+-rw-rw-rw-   0        0        0      482 2023-04-22 11:02:58.000000 buildington-1.0/buildington.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-04-22 11:02:58.000000 buildington-1.0/buildington.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 11:02:58.000000 buildington-1.0/buildington.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-22 11:02:58.000000 buildington-1.0/buildington.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-22 11:02:58.000000 buildington-1.0/buildington.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 11:02:58.830696 buildington-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-04-22 11:00:57.000000 buildington-1.0/setup.py
```

### Comparing `buildington-0.1/buildington/__init__.py` & `buildington-1.0/buildington/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 			return flask.abort(404) # Page not found!!1
 		endpntMets = endpnt[2]["met"]
 		count = 0
 		for met in endpntMets:
 			endpntMets[count] = "GET" if met == GETMET else ("POST" if met == POSTMET else None)
 			count += 1
 		if flask.request.method not in endpntMets:
-			return flask.abort(405)
+			return abort(405)
 		bdRes = endpnt[1]()
 		def escapeHTML(txt):
 			res = ""
 			for char in txt:
 				res += "&#" + str(ord(char)) + ";"
 			return res
 		count = 0
```

### Comparing `buildington-0.1/setup.py` & `buildington-1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
 	name="buildington",
-	version="0.1",
+	version="1.0",
 	author="RixTheTyrunt",
 	author_email="rixthetyrunt@gmail.com",
 	description="Building websites like React, and hosting 'em like Flask!",
 	packages=["buildington"],
 	classifiers=[
 		"Environment :: Console",
 		"Framework :: Flask",
```

