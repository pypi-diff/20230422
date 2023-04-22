# Comparing `tmp/buildington-1.1.tar.gz` & `tmp/buildington-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildington-1.1.tar", last modified: Sat Apr 22 11:18:29 2023, max compression
+gzip compressed data, was "buildington-1.2.tar", last modified: Sat Apr 22 13:11:56 2023, max compression
```

## Comparing `buildington-1.1.tar` & `buildington-1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 11:18:29.287921 buildington-1.1/
--rw-rw-rw-   0        0        0      482 2023-04-22 11:18:29.287921 buildington-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-22 11:18:29.256673 buildington-1.1/buildington/
--rw-rw-rw-   0        0        0     3544 2023-04-22 11:14:56.000000 buildington-1.1/buildington/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 11:18:29.287921 buildington-1.1/buildington.egg-info/
--rw-rw-rw-   0        0        0      482 2023-04-22 11:18:28.000000 buildington-1.1/buildington.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-04-22 11:18:29.000000 buildington-1.1/buildington.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 11:18:29.000000 buildington-1.1/buildington.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-22 11:18:29.000000 buildington-1.1/buildington.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-22 11:18:29.000000 buildington-1.1/buildington.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 11:18:29.287921 buildington-1.1/setup.cfg
--rw-rw-rw-   0        0        0      556 2023-04-22 11:18:21.000000 buildington-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:11:56.600556 buildington-1.2/
+-rw-rw-rw-   0        0        0      482 2023-04-22 13:11:56.600556 buildington-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-22 13:11:56.553683 buildington-1.2/buildington/
+-rw-rw-rw-   0        0        0     3552 2023-04-22 13:11:18.000000 buildington-1.2/buildington/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:11:56.600556 buildington-1.2/buildington.egg-info/
+-rw-rw-rw-   0        0        0      482 2023-04-22 13:11:56.000000 buildington-1.2/buildington.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-04-22 13:11:56.000000 buildington-1.2/buildington.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 13:11:56.000000 buildington-1.2/buildington.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-22 13:11:56.000000 buildington-1.2/buildington.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-22 13:11:56.000000 buildington-1.2/buildington.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 13:11:56.600556 buildington-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-04-22 13:11:31.000000 buildington-1.2/setup.py
```

### Comparing `buildington-1.1/buildington/__init__.py` & `buildington-1.2/buildington/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 		if not foundEndpnt:
 			return flask.abort(404) # Page not found!!1
 		endpntMets = endpnt[2]["met"]
 		count = 0
 		for met in endpntMets:
 			endpntMets[count] = "GET" if met == GETMET else ("POST" if met == POSTMET else None)
 			count += 1
-		if flask.request.method not in endpntMets:
+		if flask.request.method.upper() not in endpntMets:
 			return flask.abort(405)
 		bdRes = endpnt[1]()
 		def escapeHTML(txt):
 			res = ""
 			for char in txt:
 				res += "&#" + str(ord(char)) + ";"
 			return res
```

### Comparing `buildington-1.1/setup.py` & `buildington-1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
 	name="buildington",
-	version="1.1",
+	version="1.2",
 	author="RixTheTyrunt",
 	author_email="rixthetyrunt@gmail.com",
 	description="Building websites like React, and hosting 'em like Flask!",
 	packages=["buildington"],
 	classifiers=[
 		"Environment :: Console",
 		"Framework :: Flask",
```

