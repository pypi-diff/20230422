# Comparing `tmp/buildington-1.2.tar.gz` & `tmp/buildington-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildington-1.2.tar", last modified: Sat Apr 22 13:11:56 2023, max compression
+gzip compressed data, was "buildington-1.3.tar", last modified: Sat Apr 22 13:22:55 2023, max compression
```

## Comparing `buildington-1.2.tar` & `buildington-1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 13:11:56.600556 buildington-1.2/
--rw-rw-rw-   0        0        0      482 2023-04-22 13:11:56.600556 buildington-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-22 13:11:56.553683 buildington-1.2/buildington/
--rw-rw-rw-   0        0        0     3552 2023-04-22 13:11:18.000000 buildington-1.2/buildington/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 13:11:56.600556 buildington-1.2/buildington.egg-info/
--rw-rw-rw-   0        0        0      482 2023-04-22 13:11:56.000000 buildington-1.2/buildington.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-04-22 13:11:56.000000 buildington-1.2/buildington.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 13:11:56.000000 buildington-1.2/buildington.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-22 13:11:56.000000 buildington-1.2/buildington.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-22 13:11:56.000000 buildington-1.2/buildington.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 13:11:56.600556 buildington-1.2/setup.cfg
--rw-rw-rw-   0        0        0      556 2023-04-22 13:11:31.000000 buildington-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:22:55.245676 buildington-1.3/
+-rw-rw-rw-   0        0        0      482 2023-04-22 13:22:55.245676 buildington-1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-22 13:22:55.198811 buildington-1.3/buildington/
+-rw-rw-rw-   0        0        0     3573 2023-04-22 13:22:36.000000 buildington-1.3/buildington/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:22:55.245676 buildington-1.3/buildington.egg-info/
+-rw-rw-rw-   0        0        0      482 2023-04-22 13:22:54.000000 buildington-1.3/buildington.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-04-22 13:22:55.000000 buildington-1.3/buildington.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 13:22:54.000000 buildington-1.3/buildington.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-22 13:22:54.000000 buildington-1.3/buildington.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-22 13:22:54.000000 buildington-1.3/buildington.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 13:22:55.245676 buildington-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-04-22 13:22:50.000000 buildington-1.3/setup.py
```

### Comparing `buildington-1.2/buildington/__init__.py` & `buildington-1.3/buildington/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,21 +81,22 @@
 			endpnt = globals()["PAGES"][count]
 			if endpnt[0] == path:
 				foundEndpnt = True
 				break
 			count += 1
 		if not foundEndpnt:
 			return flask.abort(404) # Page not found!!1
-		endpntMets = endpnt[2]["met"]
+		endpntMets = []
 		count = 0
-		for met in endpntMets:
-			endpntMets[count] = "GET" if met == GETMET else ("POST" if met == POSTMET else None)
+		for met in endpnt[2]["met"]:
+			endpntMets.append("GET" if met == GETMET else ("POST" if met == POSTMET else None))
 			count += 1
 		if flask.request.method.upper() not in endpntMets:
 			return flask.abort(405)
+		del locals()["endpntMets"]
 		bdRes = endpnt[1]()
 		def escapeHTML(txt):
 			res = ""
 			for char in txt:
 				res += "&#" + str(ord(char)) + ";"
 			return res
 		count = 0
```

### Comparing `buildington-1.2/setup.py` & `buildington-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
 	name="buildington",
-	version="1.2",
+	version="1.3",
 	author="RixTheTyrunt",
 	author_email="rixthetyrunt@gmail.com",
 	description="Building websites like React, and hosting 'em like Flask!",
 	packages=["buildington"],
 	classifiers=[
 		"Environment :: Console",
 		"Framework :: Flask",
```

