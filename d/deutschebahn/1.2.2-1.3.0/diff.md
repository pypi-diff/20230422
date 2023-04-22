# Comparing `tmp/deutschebahn-1.2.2.tar.gz` & `tmp/deutschebahn-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\deutschebahn-1.2.2.tar", last modified: Mon Jan 10 17:14:56 2022, max compression
+gzip compressed data, was "deutschebahn-1.3.0.tar", last modified: Sat Apr 22 12:12:55 2023, max compression
```

## Comparing `deutschebahn-1.2.2.tar` & `deutschebahn-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-01-10 17:14:56.000000 deutschebahn-1.2.2/
--rw-rw-rw-   0        0        0      657 2022-01-10 17:14:56.000000 deutschebahn-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      428 2020-05-20 20:13:46.000000 deutschebahn-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2022-01-10 17:14:56.000000 deutschebahn-1.2.2/deutschebahn/
--rw-rw-rw-   0        0        0      782 2020-05-20 19:48:38.000000 deutschebahn-1.2.2/deutschebahn/__init__.py
--rw-rw-rw-   0        0        0     3977 2022-01-10 17:11:09.000000 deutschebahn-1.2.2/deutschebahn/db_infoscreen.py
--rw-rw-rw-   0        0        0  1670305 2020-05-20 19:28:43.000000 deutschebahn-1.2.2/deutschebahn/ds100.csv
--rw-rw-rw-   0        0        0     2232 2020-05-20 20:24:29.000000 deutschebahn-1.2.2/deutschebahn/ds100.py
--rw-rw-rw-   0        0        0      642 2022-01-10 17:12:48.000000 deutschebahn-1.2.2/deutschebahn/metadata.py
-drwxrwxrwx   0        0        0        0 2022-01-10 17:14:56.000000 deutschebahn-1.2.2/deutschebahn.egg-info/
--rw-rw-rw-   0        0        0      657 2022-01-10 17:14:56.000000 deutschebahn-1.2.2/deutschebahn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2022-01-10 17:14:56.000000 deutschebahn-1.2.2/deutschebahn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-10 17:14:56.000000 deutschebahn-1.2.2/deutschebahn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-01-10 17:14:56.000000 deutschebahn-1.2.2/deutschebahn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-01-10 17:14:56.000000 deutschebahn-1.2.2/deutschebahn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-01-10 17:14:56.000000 deutschebahn-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      561 2020-05-20 20:36:43.000000 deutschebahn-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 12:12:55.580300 deutschebahn-1.3.0/
+-rw-rw-rw-   0        0        0    35823 2023-04-22 12:06:56.000000 deutschebahn-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0      669 2023-04-22 12:12:55.580300 deutschebahn-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-04-22 12:06:56.000000 deutschebahn-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 12:12:55.573294 deutschebahn-1.3.0/deutschebahn/
+-rw-rw-rw-   0        0        0      821 2023-04-22 12:08:02.000000 deutschebahn-1.3.0/deutschebahn/__init__.py
+-rw-rw-rw-   0        0        0     3977 2023-04-22 12:06:56.000000 deutschebahn-1.3.0/deutschebahn/db_infoscreen.py
+-rw-rw-rw-   0        0        0  1670305 2023-04-22 12:06:56.000000 deutschebahn-1.3.0/deutschebahn/ds100.csv
+-rw-rw-rw-   0        0        0     2237 2023-04-22 12:06:56.000000 deutschebahn-1.3.0/deutschebahn/ds100.py
+-rw-rw-rw-   0        0        0     3035 2023-04-22 12:06:56.000000 deutschebahn-1.3.0/deutschebahn/fahrplan.py
+-rw-rw-rw-   0        0        0      642 2023-04-22 12:11:00.000000 deutschebahn-1.3.0/deutschebahn/metadata.py
+drwxrwxrwx   0        0        0        0 2023-04-22 12:12:55.579299 deutschebahn-1.3.0/deutschebahn/utils/
+-rw-rw-rw-   0        0        0      691 2023-04-22 12:09:01.000000 deutschebahn-1.3.0/deutschebahn/utils/__init__.py
+-rw-rw-rw-   0        0        0     1697 2023-04-22 12:10:37.000000 deutschebahn-1.3.0/deutschebahn/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-22 12:12:55.577297 deutschebahn-1.3.0/deutschebahn.egg-info/
+-rw-rw-rw-   0        0        0      669 2023-04-22 12:12:55.000000 deutschebahn-1.3.0/deutschebahn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-04-22 12:12:55.000000 deutschebahn-1.3.0/deutschebahn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 12:12:55.000000 deutschebahn-1.3.0/deutschebahn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-22 12:12:55.000000 deutschebahn-1.3.0/deutschebahn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-22 12:12:55.000000 deutschebahn-1.3.0/deutschebahn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 12:12:55.580300 deutschebahn-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-04-22 12:06:56.000000 deutschebahn-1.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `deutschebahn-1.2.2/PKG-INFO` & `deutschebahn-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: deutschebahn
-Version: 1.2.2
-Summary: Collection of utilities related to German train operator Deutsche Bahn.
-Includes bindings for https://github.com/derf/db-fakedisplay, coach order API, list of stations, and more.
-Includes unmodified DS 100 station data, licensed under CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/deed), created by Deutsche Bahn AG.
+Version: 1.3.0
+Summary: Collection of utilities related to German train operator Deutsche Bahn. Includes bindings for https://github.com/derf/db-fakedisplay, coach order API, list of stations, and more. Includes unmodified DS 100 station data, licensed under CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/deed), created by Deutsche Bahn AG.
 Home-page: https://github.com/Mezgrman/pyDeutscheBahn
 Author: Julian Metzler
 Author-email: git@mezgr.de
 License: GPLv3
-Description: UNKNOWN
 Keywords: train web api json departure arrival times coach order station list db deutsche bahn
 Platform: UNKNOWN
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `deutschebahn-1.2.2/deutschebahn/__init__.py` & `deutschebahn-1.3.0/deutschebahn/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020 Julian Metzler
+Copyright 2020-2022 Julian Metzler
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -14,8 +14,9 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from .metadata import version as __version__
 
 from .db_infoscreen import DBInfoscreen
-from .ds100 import DS100
+from .ds100 import DS100
+from .fahrplan import Fahrplan
```

### Comparing `deutschebahn-1.2.2/deutschebahn/db_infoscreen.py` & `deutschebahn-1.3.0/deutschebahn/db_infoscreen.py`

 * *Files identical despite different names*

### Comparing `deutschebahn-1.2.2/deutschebahn/ds100.csv` & `deutschebahn-1.3.0/deutschebahn/ds100.csv`

 * *Files identical despite different names*

### Comparing `deutschebahn-1.2.2/deutschebahn/ds100.py` & `deutschebahn-1.3.0/deutschebahn/ds100.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020 Julian Metzler
+Copyright 2020-2022 Julian Metzler
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `deutschebahn-1.2.2/deutschebahn/metadata.py` & `deutschebahn-1.3.0/deutschebahn/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name = "deutschebahn"
-version = "1.2.2"
+version = "1.3.0"
 description = """Collection of utilities related to German train operator Deutsche Bahn.
 Includes bindings for https://github.com/derf/db-fakedisplay, coach order API, list of stations, and more.
 Includes unmodified DS 100 station data, licensed under CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/deed), created by Deutsche Bahn AG."""
 license = "GPLv3"
 author = "Julian Metzler"
 author_email = "git@mezgr.de"
 requires = ['requests']
```

### Comparing `deutschebahn-1.2.2/deutschebahn.egg-info/PKG-INFO` & `deutschebahn-1.3.0/deutschebahn.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: deutschebahn
-Version: 1.2.2
-Summary: Collection of utilities related to German train operator Deutsche Bahn.
-Includes bindings for https://github.com/derf/db-fakedisplay, coach order API, list of stations, and more.
-Includes unmodified DS 100 station data, licensed under CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/deed), created by Deutsche Bahn AG.
+Version: 1.3.0
+Summary: Collection of utilities related to German train operator Deutsche Bahn. Includes bindings for https://github.com/derf/db-fakedisplay, coach order API, list of stations, and more. Includes unmodified DS 100 station data, licensed under CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/deed), created by Deutsche Bahn AG.
 Home-page: https://github.com/Mezgrman/pyDeutscheBahn
 Author: Julian Metzler
 Author-email: git@mezgr.de
 License: GPLv3
-Description: UNKNOWN
 Keywords: train web api json departure arrival times coach order station list db deutsche bahn
 Platform: UNKNOWN
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `deutschebahn-1.2.2/setup.py` & `deutschebahn-1.3.0/setup.py`

 * *Files identical despite different names*

