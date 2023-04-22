# Comparing `tmp/styledlogger-0.0.1.tar.gz` & `tmp/styledlogger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "styledlogger-0.0.1.tar", last modified: Sat Apr 22 09:49:47 2023, max compression
+gzip compressed data, was "styledlogger-0.0.3.tar", last modified: Sat Apr 22 10:06:34 2023, max compression
```

## Comparing `styledlogger-0.0.1.tar` & `styledlogger-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-22 09:49:47.249944 styledlogger-0.0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1338 2023-04-20 07:54:38.000000 styledlogger-0.0.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      703 2023-04-22 09:49:47.249944 styledlogger-0.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      202 2023-04-21 11:42:00.000000 styledlogger-0.0.1/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-22 09:49:47.249944 styledlogger-0.0.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      998 2023-04-22 09:48:33.000000 styledlogger-0.0.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-22 09:49:47.241944 styledlogger-0.0.1/styledlogger/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      104 2023-04-22 09:45:32.000000 styledlogger-0.0.1/styledlogger/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-22 09:49:47.249944 styledlogger-0.0.1/styledlogger/classes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-21 11:27:07.000000 styledlogger-0.0.1/styledlogger/classes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      821 2023-04-21 11:27:07.000000 styledlogger-0.0.1/styledlogger/classes/printcolors.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      296 2023-04-21 11:27:07.000000 styledlogger-0.0.1/styledlogger/classes/printtypes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2988 2023-04-21 11:27:07.000000 styledlogger-0.0.1/styledlogger/classes/styleconfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2182 2023-04-21 11:30:14.000000 styledlogger-0.0.1/styledlogger/logger.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-22 09:49:47.249944 styledlogger-0.0.1/styledlogger.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      703 2023-04-22 09:49:47.000000 styledlogger-0.0.1/styledlogger.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      393 2023-04-22 09:49:47.000000 styledlogger-0.0.1/styledlogger.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-22 09:49:47.000000 styledlogger-0.0.1/styledlogger.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       61 2023-04-22 09:49:47.000000 styledlogger-0.0.1/styledlogger.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-04-22 09:49:47.000000 styledlogger-0.0.1/styledlogger.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-22 10:06:34.932707 styledlogger-0.0.3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1338 2023-04-20 07:54:38.000000 styledlogger-0.0.3/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1547 2023-04-22 10:06:34.932707 styledlogger-0.0.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1045 2023-04-22 10:04:56.000000 styledlogger-0.0.3/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-22 10:06:34.932707 styledlogger-0.0.3/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      998 2023-04-22 10:06:19.000000 styledlogger-0.0.3/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-22 10:06:34.928707 styledlogger-0.0.3/styledlogger/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      104 2023-04-22 09:45:32.000000 styledlogger-0.0.3/styledlogger/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-22 10:06:34.932707 styledlogger-0.0.3/styledlogger/classes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-21 11:27:07.000000 styledlogger-0.0.3/styledlogger/classes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      821 2023-04-21 11:27:07.000000 styledlogger-0.0.3/styledlogger/classes/printcolors.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      296 2023-04-21 11:27:07.000000 styledlogger-0.0.3/styledlogger/classes/printtypes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2988 2023-04-22 09:59:27.000000 styledlogger-0.0.3/styledlogger/classes/styleconfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2182 2023-04-21 11:30:14.000000 styledlogger-0.0.3/styledlogger/logger.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-22 10:06:34.928707 styledlogger-0.0.3/styledlogger.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1547 2023-04-22 10:06:34.000000 styledlogger-0.0.3/styledlogger.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      393 2023-04-22 10:06:34.000000 styledlogger-0.0.3/styledlogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-22 10:06:34.000000 styledlogger-0.0.3/styledlogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       61 2023-04-22 10:06:34.000000 styledlogger-0.0.3/styledlogger.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-04-22 10:06:34.000000 styledlogger-0.0.3/styledlogger.egg-info/top_level.txt
```

### Comparing `styledlogger-0.0.1/LICENSE` & `styledlogger-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `styledlogger-0.0.1/setup.py` & `styledlogger-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     # Basics
     name='styledlogger',
-    version='0.0.1',
+    version='0.0.3',
     description='A simple, styled logging library.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     
     # Author
     author='ImAlek (splayzdk)',
     author_email='alek@imalek.me',
```

### Comparing `styledlogger-0.0.1/styledlogger/classes/printcolors.py` & `styledlogger-0.0.3/styledlogger/classes/printcolors.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.0.1/styledlogger/classes/styleconfig.py` & `styledlogger-0.0.3/styledlogger/classes/styleconfig.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.0.1/styledlogger/logger.py` & `styledlogger-0.0.3/styledlogger/logger.py`

 * *Files identical despite different names*

