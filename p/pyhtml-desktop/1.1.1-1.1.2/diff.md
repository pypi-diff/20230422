# Comparing `tmp/pyhtml_desktop-1.1.1.tar.gz` & `tmp/pyhtml_desktop-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtml_desktop-1.1.1.tar", last modified: Sat Apr 22 20:06:07 2023, max compression
+gzip compressed data, was "pyhtml_desktop-1.1.2.tar", last modified: Sat Apr 22 20:07:55 2023, max compression
```

## Comparing `pyhtml_desktop-1.1.1.tar` & `pyhtml_desktop-1.1.2.tar`

### file list

```diff
@@ -1,9 +1,11 @@
-drwxr-xr-x   0 kellanbutler52  (1000) kellanbutler52  (1000)        0 2023-04-22 20:06:07.524760 pyhtml_desktop-1.1.1/
--rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      545 2023-04-22 20:06:07.522760 pyhtml_desktop-1.1.1/PKG-INFO
-drwxr-xr-x   0 kellanbutler52  (1000) kellanbutler52  (1000)        0 2023-04-22 20:06:07.521760 pyhtml_desktop-1.1.1/pyhtml_desktop.egg-info/
--rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      545 2023-04-22 20:06:07.000000 pyhtml_desktop-1.1.1/pyhtml_desktop.egg-info/PKG-INFO
--rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      160 2023-04-22 20:06:07.000000 pyhtml_desktop-1.1.1/pyhtml_desktop.egg-info/SOURCES.txt
--rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)        1 2023-04-22 20:06:07.000000 pyhtml_desktop-1.1.1/pyhtml_desktop.egg-info/dependency_links.txt
--rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)        1 2023-04-22 20:06:07.000000 pyhtml_desktop-1.1.1/pyhtml_desktop.egg-info/top_level.txt
--rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)       38 2023-04-22 20:06:07.524760 pyhtml_desktop-1.1.1/setup.cfg
--rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      842 2023-04-22 20:05:23.000000 pyhtml_desktop-1.1.1/setup.py
+drwxr-xr-x   0 kellanbutler52  (1000) kellanbutler52  (1000)        0 2023-04-22 20:07:55.896760 pyhtml_desktop-1.1.2/
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      545 2023-04-22 20:07:55.895760 pyhtml_desktop-1.1.2/PKG-INFO
+drwxr-xr-x   0 kellanbutler52  (1000) kellanbutler52  (1000)        0 2023-04-22 20:07:55.891760 pyhtml_desktop-1.1.2/pyhtml_desktop/
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)     3994 2023-04-22 20:07:19.000000 pyhtml_desktop-1.1.2/pyhtml_desktop/__init__.py
+drwxr-xr-x   0 kellanbutler52  (1000) kellanbutler52  (1000)        0 2023-04-22 20:07:55.894760 pyhtml_desktop-1.1.2/pyhtml_desktop.egg-info/
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      545 2023-04-22 20:07:55.000000 pyhtml_desktop-1.1.2/pyhtml_desktop.egg-info/PKG-INFO
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      187 2023-04-22 20:07:55.000000 pyhtml_desktop-1.1.2/pyhtml_desktop.egg-info/SOURCES.txt
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)        1 2023-04-22 20:07:55.000000 pyhtml_desktop-1.1.2/pyhtml_desktop.egg-info/dependency_links.txt
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)       15 2023-04-22 20:07:55.000000 pyhtml_desktop-1.1.2/pyhtml_desktop.egg-info/top_level.txt
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)       38 2023-04-22 20:07:55.896760 pyhtml_desktop-1.1.2/setup.cfg
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      842 2023-04-22 20:07:31.000000 pyhtml_desktop-1.1.2/setup.py
```

### Comparing `pyhtml_desktop-1.1.1/PKG-INFO` & `pyhtml_desktop-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pyhtml_desktop
-Version: 1.1.1
+Version: 1.1.2
 Summary: build desktop apps with Python and HTML
 Home-page: UNKNOWN
 Author: Kellan Butler
 Author-email: kellanbutler52@gmail.com
 License: UNKNOWN
 Project-URL: Github, https://github.com/kellantech/pyhtmldesktop/
 Description: build desktop apps with Python and HTML
```

### Comparing `pyhtml_desktop-1.1.1/pyhtml_desktop.egg-info/PKG-INFO` & `pyhtml_desktop-1.1.2/pyhtml_desktop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pyhtml-desktop
-Version: 1.1.1
+Version: 1.1.2
 Summary: build desktop apps with Python and HTML
 Home-page: UNKNOWN
 Author: Kellan Butler
 Author-email: kellanbutler52@gmail.com
 License: UNKNOWN
 Project-URL: Github, https://github.com/kellantech/pyhtmldesktop/
 Description: build desktop apps with Python and HTML
```

### Comparing `pyhtml_desktop-1.1.1/setup.py` & `pyhtml_desktop-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.1' 
+VERSION = '1.1.2' 
 DESCRIPTION = 'build desktop apps with Python and HTML'
 LONG_DESCRIPTION = 'build desktop apps with Python and HTML'
 setup(
         name="pyhtml_desktop", 
         version=VERSION,
         author="Kellan Butler",
         author_email="kellanbutler52@gmail.com",
```

