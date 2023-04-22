# Comparing `tmp/torrent-hound-2.0.tar.gz` & `tmp/torrent-hound-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torrent-hound-2.0.tar", last modified: Sat Apr 22 01:15:39 2023, max compression
+gzip compressed data, was "torrent-hound-2.0.1.tar", last modified: Sat Apr 22 01:33:21 2023, max compression
```

## Comparing `torrent-hound-2.0.tar` & `torrent-hound-2.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yashovardhan   (501) staff       (20)        0 2023-04-22 01:15:39.585668 torrent-hound-2.0/
--rw-r--r--   0 yashovardhan   (501) staff       (20)       18 2018-06-15 03:26:44.000000 torrent-hound-2.0/MANIFEST.in
--rw-r--r--   0 yashovardhan   (501) staff       (20)     2245 2023-04-22 01:15:39.584923 torrent-hound-2.0/PKG-INFO
--rw-r--r--   0 yashovardhan   (501) staff       (20)     1976 2018-12-11 21:30:12.000000 torrent-hound-2.0/README.rst
--rw-r--r--   0 yashovardhan   (501) staff       (20)       38 2023-04-22 01:15:39.585858 torrent-hound-2.0/setup.cfg
--rw-r--r--   0 yashovardhan   (501) staff       (20)      828 2023-04-22 01:13:10.000000 torrent-hound-2.0/setup.py
--rwxr--r--   0 yashovardhan   (501) staff       (20)    52365 2023-04-22 01:14:00.000000 torrent-hound-2.0/torrent-hound
-drwxr-xr-x   0 yashovardhan   (501) staff       (20)        0 2023-04-22 01:15:39.501730 torrent-hound-2.0/torrent_hound.egg-info/
--rw-r--r--   0 yashovardhan   (501) staff       (20)     2245 2023-04-22 01:15:37.000000 torrent-hound-2.0/torrent_hound.egg-info/PKG-INFO
--rw-r--r--   0 yashovardhan   (501) staff       (20)      229 2023-04-22 01:15:39.000000 torrent-hound-2.0/torrent_hound.egg-info/SOURCES.txt
--rw-r--r--   0 yashovardhan   (501) staff       (20)        1 2023-04-22 01:15:37.000000 torrent-hound-2.0/torrent_hound.egg-info/dependency_links.txt
--rw-r--r--   0 yashovardhan   (501) staff       (20)       63 2023-04-22 01:15:38.000000 torrent-hound-2.0/torrent_hound.egg-info/requires.txt
--rw-r--r--   0 yashovardhan   (501) staff       (20)        1 2023-04-22 01:15:38.000000 torrent-hound-2.0/torrent_hound.egg-info/top_level.txt
+drwxr-xr-x   0 yashovardhan   (501) staff       (20)        0 2023-04-22 01:33:21.971453 torrent-hound-2.0.1/
+-rw-r--r--   0 yashovardhan   (501) staff       (20)       18 2018-06-15 03:26:44.000000 torrent-hound-2.0.1/MANIFEST.in
+-rw-r--r--   0 yashovardhan   (501) staff       (20)     2245 2023-04-22 01:33:21.968036 torrent-hound-2.0.1/PKG-INFO
+-rw-r--r--   0 yashovardhan   (501) staff       (20)     1974 2023-04-22 01:31:31.000000 torrent-hound-2.0.1/README.rst
+-rw-r--r--   0 yashovardhan   (501) staff       (20)       38 2023-04-22 01:33:21.974193 torrent-hound-2.0.1/setup.cfg
+-rw-r--r--   0 yashovardhan   (501) staff       (20)      830 2023-04-22 01:24:27.000000 torrent-hound-2.0.1/setup.py
+-rwxr--r--   0 yashovardhan   (501) staff       (20)    52365 2023-04-22 01:14:00.000000 torrent-hound-2.0.1/torrent-hound
+drwxr-xr-x   0 yashovardhan   (501) staff       (20)        0 2023-04-22 01:33:21.966190 torrent-hound-2.0.1/torrent_hound.egg-info/
+-rw-r--r--   0 yashovardhan   (501) staff       (20)     2245 2023-04-22 01:33:21.000000 torrent-hound-2.0.1/torrent_hound.egg-info/PKG-INFO
+-rw-r--r--   0 yashovardhan   (501) staff       (20)      229 2023-04-22 01:33:21.000000 torrent-hound-2.0.1/torrent_hound.egg-info/SOURCES.txt
+-rw-r--r--   0 yashovardhan   (501) staff       (20)        1 2023-04-22 01:33:21.000000 torrent-hound-2.0.1/torrent_hound.egg-info/dependency_links.txt
+-rw-r--r--   0 yashovardhan   (501) staff       (20)       63 2023-04-22 01:33:21.000000 torrent-hound-2.0.1/torrent_hound.egg-info/requires.txt
+-rw-r--r--   0 yashovardhan   (501) staff       (20)        1 2023-04-22 01:33:21.000000 torrent-hound-2.0.1/torrent_hound.egg-info/top_level.txt
```

### Comparing `torrent-hound-2.0/PKG-INFO` & `torrent-hound-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torrent-hound
-Version: 2.0
+Version: 2.0.1
 Summary: Search torrents from multiple websites via the CLI
 Home-page: https://github.com/baddymaster/torrent-hound
 Author: Yashovardhan Sharma
 Author-email: yash.s@tuta.io
 License: AGPL-3.0
 Requires-Python: >=3
 
@@ -12,15 +12,15 @@
 =============
 
 Search torrents from multiple websites via the CLI
 
 Requirements
 ~~~~~~~~~~~~
 
--  Python 2.7
+-  Python 3
 -  bs4
 -  clint
 -  pyperclip
 -  humanize
 -  VeryPrettyTable
 -  cfscrape
```

### Comparing `torrent-hound-2.0/README.rst` & `torrent-hound-2.0.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 =============
 
 Search torrents from multiple websites via the CLI
 
 Requirements
 ~~~~~~~~~~~~
 
--  Python 2.7
+-  Python 3
 -  bs4
 -  clint
 -  pyperclip
 -  humanize
 -  VeryPrettyTable
 -  cfscrape
```

### Comparing `torrent-hound-2.0/setup.py` & `torrent-hound-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='torrent-hound',          # This is the name of your PyPI-package.
-    version='2.0',                 # Update the version number for new releases
+    version='2.0.1',                 # Update the version number for new releases
     scripts=['torrent-hound'],     # The name of your scipt, and also the command you'll be using for calling it
     description='Search torrents from multiple websites via the CLI',
     long_description=readme(),
     python_requires = '>=3',
     url='https://github.com/baddymaster/torrent-hound',
     install_requires=[
         'bs4',
```

### Comparing `torrent-hound-2.0/torrent-hound` & `torrent-hound-2.0.1/torrent-hound`

 * *Files identical despite different names*

### Comparing `torrent-hound-2.0/torrent_hound.egg-info/PKG-INFO` & `torrent-hound-2.0.1/torrent_hound.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torrent-hound
-Version: 2.0
+Version: 2.0.1
 Summary: Search torrents from multiple websites via the CLI
 Home-page: https://github.com/baddymaster/torrent-hound
 Author: Yashovardhan Sharma
 Author-email: yash.s@tuta.io
 License: AGPL-3.0
 Requires-Python: >=3
 
@@ -12,15 +12,15 @@
 =============
 
 Search torrents from multiple websites via the CLI
 
 Requirements
 ~~~~~~~~~~~~
 
--  Python 2.7
+-  Python 3
 -  bs4
 -  clint
 -  pyperclip
 -  humanize
 -  VeryPrettyTable
 -  cfscrape
```

