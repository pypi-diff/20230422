# Comparing `tmp/deutschebahn-1.3.1.tar.gz` & `tmp/deutschebahn-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deutschebahn-1.3.1.tar", last modified: Sat Apr 22 16:16:45 2023, max compression
+gzip compressed data, was "deutschebahn-1.3.2.tar", last modified: Sat Apr 22 16:23:02 2023, max compression
```

## Comparing `deutschebahn-1.3.1.tar` & `deutschebahn-1.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 16:16:45.602492 deutschebahn-1.3.1/
--rw-rw-rw-   0        0        0    35823 2023-04-22 12:06:56.000000 deutschebahn-1.3.1/LICENSE
--rw-rw-rw-   0        0        0      669 2023-04-22 16:16:45.602492 deutschebahn-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-04-22 12:06:56.000000 deutschebahn-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 16:16:45.595486 deutschebahn-1.3.1/deutschebahn/
--rw-rw-rw-   0        0        0      821 2023-04-22 12:08:02.000000 deutschebahn-1.3.1/deutschebahn/__init__.py
--rw-rw-rw-   0        0        0     3977 2023-04-22 12:06:56.000000 deutschebahn-1.3.1/deutschebahn/db_infoscreen.py
--rw-rw-rw-   0        0        0  1670305 2023-04-22 12:06:56.000000 deutschebahn-1.3.1/deutschebahn/ds100.csv
--rw-rw-rw-   0        0        0     2237 2023-04-22 12:06:56.000000 deutschebahn-1.3.1/deutschebahn/ds100.py
--rw-rw-rw-   0        0        0     3035 2023-04-22 12:06:56.000000 deutschebahn-1.3.1/deutschebahn/fahrplan.py
--rw-rw-rw-   0        0        0      642 2023-04-22 16:15:32.000000 deutschebahn-1.3.1/deutschebahn/metadata.py
-drwxrwxrwx   0        0        0        0 2023-04-22 16:16:45.601492 deutschebahn-1.3.1/deutschebahn/utils/
--rw-rw-rw-   0        0        0      691 2023-04-22 12:09:01.000000 deutschebahn-1.3.1/deutschebahn/utils/__init__.py
--rw-rw-rw-   0        0        0     1705 2023-04-22 16:16:16.000000 deutschebahn-1.3.1/deutschebahn/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-22 16:16:45.599490 deutschebahn-1.3.1/deutschebahn.egg-info/
--rw-rw-rw-   0        0        0      669 2023-04-22 16:16:45.000000 deutschebahn-1.3.1/deutschebahn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-04-22 16:16:45.000000 deutschebahn-1.3.1/deutschebahn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 16:16:45.000000 deutschebahn-1.3.1/deutschebahn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-22 16:16:45.000000 deutschebahn-1.3.1/deutschebahn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-22 16:16:45.000000 deutschebahn-1.3.1/deutschebahn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 16:16:45.602492 deutschebahn-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-04-22 12:06:56.000000 deutschebahn-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:23:02.355085 deutschebahn-1.3.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-22 12:06:56.000000 deutschebahn-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0      669 2023-04-22 16:23:02.354084 deutschebahn-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-04-22 12:06:56.000000 deutschebahn-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 16:23:02.346076 deutschebahn-1.3.2/deutschebahn/
+-rw-rw-rw-   0        0        0      821 2023-04-22 12:08:02.000000 deutschebahn-1.3.2/deutschebahn/__init__.py
+-rw-rw-rw-   0        0        0     3977 2023-04-22 12:06:56.000000 deutschebahn-1.3.2/deutschebahn/db_infoscreen.py
+-rw-rw-rw-   0        0        0  1670305 2023-04-22 12:06:56.000000 deutschebahn-1.3.2/deutschebahn/ds100.csv
+-rw-rw-rw-   0        0        0     2237 2023-04-22 12:06:56.000000 deutschebahn-1.3.2/deutschebahn/ds100.py
+-rw-rw-rw-   0        0        0     3035 2023-04-22 12:06:56.000000 deutschebahn-1.3.2/deutschebahn/fahrplan.py
+-rw-rw-rw-   0        0        0      642 2023-04-22 16:22:49.000000 deutschebahn-1.3.2/deutschebahn/metadata.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:23:02.353083 deutschebahn-1.3.2/deutschebahn/utils/
+-rw-rw-rw-   0        0        0      691 2023-04-22 12:09:01.000000 deutschebahn-1.3.2/deutschebahn/utils/__init__.py
+-rw-rw-rw-   0        0        0     2673 2023-04-22 16:22:17.000000 deutschebahn-1.3.2/deutschebahn/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:23:02.352082 deutschebahn-1.3.2/deutschebahn.egg-info/
+-rw-rw-rw-   0        0        0      669 2023-04-22 16:23:02.000000 deutschebahn-1.3.2/deutschebahn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-04-22 16:23:02.000000 deutschebahn-1.3.2/deutschebahn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 16:23:02.000000 deutschebahn-1.3.2/deutschebahn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-22 16:23:02.000000 deutschebahn-1.3.2/deutschebahn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-22 16:23:02.000000 deutschebahn-1.3.2/deutschebahn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 16:23:02.355085 deutschebahn-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-04-22 12:06:56.000000 deutschebahn-1.3.2/setup.py
```

### Comparing `deutschebahn-1.3.1/LICENSE` & `deutschebahn-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deutschebahn-1.3.1/PKG-INFO` & `deutschebahn-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deutschebahn
-Version: 1.3.1
+Version: 1.3.2
 Summary: Collection of utilities related to German train operator Deutsche Bahn. Includes bindings for https://github.com/derf/db-fakedisplay, coach order API, list of stations, and more. Includes unmodified DS 100 station data, licensed under CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/deed), created by Deutsche Bahn AG.
 Home-page: https://github.com/Mezgrman/pyDeutscheBahn
 Author: Julian Metzler
 Author-email: git@mezgr.de
 License: GPLv3
 Keywords: train web api json departure arrival times coach order station list db deutsche bahn
 Platform: UNKNOWN
```

### Comparing `deutschebahn-1.3.1/deutschebahn/__init__.py` & `deutschebahn-1.3.2/deutschebahn/__init__.py`

 * *Files identical despite different names*

### Comparing `deutschebahn-1.3.1/deutschebahn/db_infoscreen.py` & `deutschebahn-1.3.2/deutschebahn/db_infoscreen.py`

 * *Files identical despite different names*

### Comparing `deutschebahn-1.3.1/deutschebahn/ds100.csv` & `deutschebahn-1.3.2/deutschebahn/ds100.csv`

 * *Files identical despite different names*

### Comparing `deutschebahn-1.3.1/deutschebahn/ds100.py` & `deutschebahn-1.3.2/deutschebahn/ds100.py`

 * *Files identical despite different names*

### Comparing `deutschebahn-1.3.1/deutschebahn/fahrplan.py` & `deutschebahn-1.3.2/deutschebahn/fahrplan.py`

 * *Files identical despite different names*

### Comparing `deutschebahn-1.3.1/deutschebahn/metadata.py` & `deutschebahn-1.3.2/deutschebahn/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name = "deutschebahn"
-version = "1.3.1"
+version = "1.3.2"
 description = """Collection of utilities related to German train operator Deutsche Bahn.
 Includes bindings for https://github.com/derf/db-fakedisplay, coach order API, list of stations, and more.
 Includes unmodified DS 100 station data, licensed under CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/deed), created by Deutsche Bahn AG."""
 license = "GPLv3"
 author = "Julian Metzler"
 author_email = "git@mezgr.de"
 requires = ['requests']
```

### Comparing `deutschebahn-1.3.1/deutschebahn/utils/__init__.py` & `deutschebahn-1.3.2/deutschebahn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deutschebahn-1.3.1/deutschebahn.egg-info/PKG-INFO` & `deutschebahn-1.3.2/deutschebahn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deutschebahn
-Version: 1.3.1
+Version: 1.3.2
 Summary: Collection of utilities related to German train operator Deutsche Bahn. Includes bindings for https://github.com/derf/db-fakedisplay, coach order API, list of stations, and more. Includes unmodified DS 100 station data, licensed under CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/deed), created by Deutsche Bahn AG.
 Home-page: https://github.com/Mezgrman/pyDeutscheBahn
 Author: Julian Metzler
 Author-email: git@mezgr.de
 License: GPLv3
 Keywords: train web api json departure arrival times coach order station list db deutsche bahn
 Platform: UNKNOWN
```

### Comparing `deutschebahn-1.3.1/setup.py` & `deutschebahn-1.3.2/setup.py`

 * *Files identical despite different names*

