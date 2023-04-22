# Comparing `tmp/pyhtml_desktop-1.1.2.tar.gz` & `tmp/pyhtml_desktop-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtml_desktop-1.1.2.tar", last modified: Sat Apr 22 20:07:55 2023, max compression
+gzip compressed data, was "pyhtml_desktop-1.1.3.tar", last modified: Sat Apr 22 20:14:35 2023, max compression
```

## Comparing `pyhtml_desktop-1.1.2.tar` & `pyhtml_desktop-1.1.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 kellanbutler52  (1000) kellanbutler52  (1000)        0 2023-04-22 20:07:55.896760 pyhtml_desktop-1.1.2/
--rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      545 2023-04-22 20:07:55.895760 pyhtml_desktop-1.1.2/PKG-INFO
-drwxr-xr-x   0 kellanbutler52  (1000) kellanbutler52  (1000)        0 2023-04-22 20:07:55.891760 pyhtml_desktop-1.1.2/pyhtml_desktop/
--rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)     3994 2023-04-22 20:07:19.000000 pyhtml_desktop-1.1.2/pyhtml_desktop/__init__.py
-drwxr-xr-x   0 kellanbutler52  (1000) kellanbutler52  (1000)        0 2023-04-22 20:07:55.894760 pyhtml_desktop-1.1.2/pyhtml_desktop.egg-info/
--rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      545 2023-04-22 20:07:55.000000 pyhtml_desktop-1.1.2/pyhtml_desktop.egg-info/PKG-INFO
--rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      187 2023-04-22 20:07:55.000000 pyhtml_desktop-1.1.2/pyhtml_desktop.egg-info/SOURCES.txt
--rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)        1 2023-04-22 20:07:55.000000 pyhtml_desktop-1.1.2/pyhtml_desktop.egg-info/dependency_links.txt
--rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)       15 2023-04-22 20:07:55.000000 pyhtml_desktop-1.1.2/pyhtml_desktop.egg-info/top_level.txt
--rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)       38 2023-04-22 20:07:55.896760 pyhtml_desktop-1.1.2/setup.cfg
--rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      842 2023-04-22 20:07:31.000000 pyhtml_desktop-1.1.2/setup.py
+drwxr-xr-x   0 kellanbutler52  (1000) kellanbutler52  (1000)        0 2023-04-22 20:14:35.142343 pyhtml_desktop-1.1.3/
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      545 2023-04-22 20:14:35.141343 pyhtml_desktop-1.1.3/PKG-INFO
+drwxr-xr-x   0 kellanbutler52  (1000) kellanbutler52  (1000)        0 2023-04-22 20:14:35.136343 pyhtml_desktop-1.1.3/pyhtml_desktop/
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)     3994 2023-04-22 20:07:19.000000 pyhtml_desktop-1.1.3/pyhtml_desktop/__init__.py
+drwxr-xr-x   0 kellanbutler52  (1000) kellanbutler52  (1000)        0 2023-04-22 20:14:35.140343 pyhtml_desktop-1.1.3/pyhtml_desktop.egg-info/
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      545 2023-04-22 20:14:34.000000 pyhtml_desktop-1.1.3/pyhtml_desktop.egg-info/PKG-INFO
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      224 2023-04-22 20:14:35.000000 pyhtml_desktop-1.1.3/pyhtml_desktop.egg-info/SOURCES.txt
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)        1 2023-04-22 20:14:34.000000 pyhtml_desktop-1.1.3/pyhtml_desktop.egg-info/dependency_links.txt
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)       15 2023-04-22 20:14:34.000000 pyhtml_desktop-1.1.3/pyhtml_desktop.egg-info/requires.txt
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)       15 2023-04-22 20:14:34.000000 pyhtml_desktop-1.1.3/pyhtml_desktop.egg-info/top_level.txt
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)       38 2023-04-22 20:14:35.142343 pyhtml_desktop-1.1.3/setup.cfg
+-rw-r--r--   0 kellanbutler52  (1000) kellanbutler52  (1000)      858 2023-04-22 20:14:23.000000 pyhtml_desktop-1.1.3/setup.py
```

### Comparing `pyhtml_desktop-1.1.2/PKG-INFO` & `pyhtml_desktop-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pyhtml_desktop
-Version: 1.1.2
+Version: 1.1.3
 Summary: build desktop apps with Python and HTML
 Home-page: UNKNOWN
 Author: Kellan Butler
 Author-email: kellanbutler52@gmail.com
 License: UNKNOWN
 Project-URL: Github, https://github.com/kellantech/pyhtmldesktop/
 Description: build desktop apps with Python and HTML
```

### Comparing `pyhtml_desktop-1.1.2/pyhtml_desktop/__init__.py` & `pyhtml_desktop-1.1.3/pyhtml_desktop/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhtml_desktop-1.1.2/pyhtml_desktop.egg-info/PKG-INFO` & `pyhtml_desktop-1.1.3/pyhtml_desktop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pyhtml-desktop
-Version: 1.1.2
+Version: 1.1.3
 Summary: build desktop apps with Python and HTML
 Home-page: UNKNOWN
 Author: Kellan Butler
 Author-email: kellanbutler52@gmail.com
 License: UNKNOWN
 Project-URL: Github, https://github.com/kellantech/pyhtmldesktop/
 Description: build desktop apps with Python and HTML
```

### Comparing `pyhtml_desktop-1.1.2/setup.py` & `pyhtml_desktop-1.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.2' 
+VERSION = '1.1.3' 
 DESCRIPTION = 'build desktop apps with Python and HTML'
 LONG_DESCRIPTION = 'build desktop apps with Python and HTML'
 setup(
         name="pyhtml_desktop", 
         version=VERSION,
         author="Kellan Butler",
         author_email="kellanbutler52@gmail.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=[], 
+        install_requires=['beautifulsoup4'], 
         
         keywords=['python', 'html'],
         classifiers= [
             "Development Status :: 4 - Beta",
             "Intended Audience :: Developers",
             "Programming Language :: Python :: 3",
             "Operating System :: POSIX :: Linux",
```

