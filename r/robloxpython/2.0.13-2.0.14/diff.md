# Comparing `tmp/robloxpython-2.0.13.tar.gz` & `tmp/robloxpython-2.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robloxpython-2.0.13.tar", last modified: Sat Apr 22 01:35:18 2023, max compression
+gzip compressed data, was "robloxpython-2.0.14.tar", last modified: Sat Apr 22 19:47:48 2023, max compression
```

## Comparing `robloxpython-2.0.13.tar` & `robloxpython-2.0.14.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 01:35:18.130019 robloxpython-2.0.13/
--rw-rw-rw-   0        0        0      278 2023-04-22 01:35:18.129016 robloxpython-2.0.13/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-22 01:35:18.130532 robloxpython-2.0.13/setup.cfg
--rw-rw-rw-   0        0        0     1527 2023-04-22 01:35:06.000000 robloxpython-2.0.13/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 01:35:18.059019 robloxpython-2.0.13/src/
-drwxrwxrwx   0        0        0        0 2023-04-22 01:35:18.083521 robloxpython-2.0.13/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2021-11-15 19:17:04.000000 robloxpython-2.0.13/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2021-11-16 19:32:04.000000 robloxpython-2.0.13/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2021-11-16 19:32:06.000000 robloxpython-2.0.13/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2021-11-16 19:54:36.000000 robloxpython-2.0.13/src/roblox_api_wrapper/message.py
-drwxrwxrwx   0        0        0        0 2023-04-22 01:35:18.123516 robloxpython-2.0.13/src/robloxpython.egg-info/
--rw-rw-rw-   0        0        0      278 2023-04-22 01:35:17.000000 robloxpython-2.0.13/src/robloxpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-22 01:35:17.000000 robloxpython-2.0.13/src/robloxpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 01:35:17.000000 robloxpython-2.0.13/src/robloxpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-22 01:35:17.000000 robloxpython-2.0.13/src/robloxpython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 19:47:48.291296 robloxpython-2.0.14/
+-rw-rw-rw-   0        0        0      278 2023-04-22 19:47:48.290293 robloxpython-2.0.14/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-22 19:47:48.291793 robloxpython-2.0.14/setup.cfg
+-rw-rw-rw-   0        0        0     1527 2023-04-22 19:47:33.000000 robloxpython-2.0.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 19:47:48.210794 robloxpython-2.0.14/src/
+drwxrwxrwx   0        0        0        0 2023-04-22 19:47:48.252293 robloxpython-2.0.14/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2021-11-15 19:17:04.000000 robloxpython-2.0.14/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2021-11-16 19:32:04.000000 robloxpython-2.0.14/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2021-11-16 19:32:06.000000 robloxpython-2.0.14/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2021-11-16 19:54:36.000000 robloxpython-2.0.14/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2023-04-22 19:47:48.284791 robloxpython-2.0.14/src/robloxpython.egg-info/
+-rw-rw-rw-   0        0        0      278 2023-04-22 19:47:47.000000 robloxpython-2.0.14/src/robloxpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-22 19:47:47.000000 robloxpython-2.0.14/src/robloxpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 19:47:47.000000 robloxpython-2.0.14/src/robloxpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-22 19:47:47.000000 robloxpython-2.0.14/src/robloxpython.egg-info/top_level.txt
```

### Comparing `robloxpython-2.0.13/setup.py` & `robloxpython-2.0.14/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools, base64
 
 
 setuptools.setup(
     name="robloxpython",
-    version="2.0.13",
+    version="2.0.14",
     author="robloxpython",
     #description="Official wrapper for the Roblox API",
     description="robloxpython",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

