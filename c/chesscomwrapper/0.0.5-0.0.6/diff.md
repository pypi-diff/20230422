# Comparing `tmp/chesscomwrapper-0.0.5.tar.gz` & `tmp/chesscomwrapper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chesscomwrapper-0.0.5.tar", last modified: Sat Apr 22 16:57:23 2023, max compression
+gzip compressed data, was "chesscomwrapper-0.0.6.tar", last modified: Sat Apr 22 17:01:02 2023, max compression
```

## Comparing `chesscomwrapper-0.0.5.tar` & `chesscomwrapper-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:57:23.720376 chesscomwrapper-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-22 16:57:23.720376 chesscomwrapper-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:57:23.716375 chesscomwrapper-0.0.5/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:57:23.716375 chesscomwrapper-0.0.5/app/chesscomwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:57:23.720376 chesscomwrapper-0.0.5/app/chesscomwrapper/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/apimanager.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/chessclub.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/chesscountry.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/chessleaderboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/chessplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/chessstreamer.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/chessteammatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/chesstournament.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/chesswrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/dailypuzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/lazy_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/playerarchive.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/teammatchboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/tournamentround.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/src/tournamentroundgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/app/chesscomwrapper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:57:23.716375 chesscomwrapper-0.0.5/app/chesscomwrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-22 16:57:23.000000 chesscomwrapper-0.0.5/app/chesscomwrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-22 16:57:23.000000 chesscomwrapper-0.0.5/app/chesscomwrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 16:57:23.000000 chesscomwrapper-0.0.5/app/chesscomwrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-22 16:57:23.000000 chesscomwrapper-0.0.5/app/chesscomwrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 16:57:23.000000 chesscomwrapper-0.0.5/app/chesscomwrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 16:57:23.720376 chesscomwrapper-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:57:23.720376 chesscomwrapper-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-04-22 16:57:12.000000 chesscomwrapper-0.0.5/tests/test_chesswrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:02.468727 chesscomwrapper-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-22 17:01:02.468727 chesscomwrapper-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:02.460727 chesscomwrapper-0.0.6/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:02.464727 chesscomwrapper-0.0.6/app/chesscomwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:02.468727 chesscomwrapper-0.0.6/app/chesscomwrapper/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/apimanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chessclub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chesscountry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chessleaderboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chessplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chessstreamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chessteammatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chesstournament.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chesswrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/dailypuzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/lazy_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/playerarchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/teammatchboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/tournamentround.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/tournamentroundgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:02.464727 chesscomwrapper-0.0.6/app/chesscomwrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-22 17:01:02.000000 chesscomwrapper-0.0.6/app/chesscomwrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-22 17:01:02.000000 chesscomwrapper-0.0.6/app/chesscomwrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:01:02.000000 chesscomwrapper-0.0.6/app/chesscomwrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 17:01:02.000000 chesscomwrapper-0.0.6/app/chesscomwrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 17:01:02.000000 chesscomwrapper-0.0.6/app/chesscomwrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 17:01:02.468727 chesscomwrapper-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:02.468727 chesscomwrapper-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/tests/test_chesswrapper.py
```

### Comparing `chesscomwrapper-0.0.5/LICENSE.txt` & `chesscomwrapper-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.5/PKG-INFO` & `chesscomwrapper-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chesscomwrapper
-Version: 0.0.5
+Version: 0.0.6
 Summary: A wrapper for the chess.com API
 Home-page: https://github.com/nicpanozzo/chesscom-api-wrapper
 Author: Nicola Panozzo
 Author-email: nicolapanoz@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chesscomwrapper-0.0.5/app/chesscomwrapper/src/apimanager.py` & `chesscomwrapper-0.0.6/app/chesscomwrapper/src/apimanager.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.5/app/chesscomwrapper/src/chessclub.py` & `chesscomwrapper-0.0.6/app/chesscomwrapper/src/chessclub.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.5/app/chesscomwrapper/src/chesscountry.py` & `chesscomwrapper-0.0.6/app/chesscomwrapper/src/chesscountry.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.5/app/chesscomwrapper/src/chessplayer.py` & `chesscomwrapper-0.0.6/app/chesscomwrapper/src/chessplayer.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.5/app/chesscomwrapper/src/chesswrapper.py` & `chesscomwrapper-0.0.6/app/chesscomwrapper/src/chesswrapper.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.5/app/chesscomwrapper/src/playerarchive.py` & `chesscomwrapper-0.0.6/app/chesscomwrapper/src/playerarchive.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.5/app/chesscomwrapper.egg-info/PKG-INFO` & `chesscomwrapper-0.0.6/app/chesscomwrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chesscomwrapper
-Version: 0.0.5
+Version: 0.0.6
 Summary: A wrapper for the chess.com API
 Home-page: https://github.com/nicpanozzo/chesscom-api-wrapper
 Author: Nicola Panozzo
 Author-email: nicolapanoz@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chesscomwrapper-0.0.5/app/chesscomwrapper.egg-info/SOURCES.txt` & `chesscomwrapper-0.0.6/app/chesscomwrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.5/setup.py` & `chesscomwrapper-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,15 @@
     author='Nicola Panozzo',
     author_email='nicolapanoz@gmail.com',
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3'
         ],
-    install_requires=['requests',
-                      'functools'],
+    install_requires=['requests'],
     extras_require={
         'dev': [
             'pytest>=3.7',
             'twine>=1.11.0',
         ],
     },
     python_requires='>=3.6',
```

### Comparing `chesscomwrapper-0.0.5/tests/test_chesswrapper.py` & `chesscomwrapper-0.0.6/tests/test_chesswrapper.py`

 * *Files identical despite different names*

