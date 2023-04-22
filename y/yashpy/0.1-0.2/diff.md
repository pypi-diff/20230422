# Comparing `tmp/yashpy-0.1.tar.gz` & `tmp/yashpy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yashpy-0.1.tar", last modified: Sat Apr 22 04:45:26 2023, max compression
+gzip compressed data, was "yashpy-0.2.tar", last modified: Sat Apr 22 05:11:40 2023, max compression
```

## Comparing `yashpy-0.1.tar` & `yashpy-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 04:45:26.675771 yashpy-0.1/
--rw-rw-rw-   0        0        0      175 2023-04-22 04:45:26.675579 yashpy-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-22 04:03:48.000000 yashpy-0.1/licence.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 04:45:26.676768 yashpy-0.1/setup.cfg
--rw-rw-rw-   0        0        0      245 2023-04-22 04:43:23.000000 yashpy-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 04:45:26.628971 yashpy-0.1/yashpy/
--rw-rw-rw-   0        0        0       97 2023-04-22 04:44:05.000000 yashpy-0.1/yashpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 04:45:26.673497 yashpy-0.1/yashpy.egg-info/
--rw-rw-rw-   0        0        0      175 2023-04-22 04:45:26.000000 yashpy-0.1/yashpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-04-22 04:45:26.000000 yashpy-0.1/yashpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 04:45:26.000000 yashpy-0.1/yashpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-22 04:45:26.000000 yashpy-0.1/yashpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 05:11:39.690033 yashpy-0.2/
+-rw-rw-rw-   0        0        0      175 2023-04-22 05:11:39.690033 yashpy-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-22 04:03:48.000000 yashpy-0.2/licence.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 05:11:39.691177 yashpy-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      245 2023-04-22 05:10:09.000000 yashpy-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 05:11:39.669537 yashpy-0.2/yashpy/
+-rw-rw-rw-   0        0        0       97 2023-04-22 05:10:26.000000 yashpy-0.2/yashpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 05:11:39.689056 yashpy-0.2/yashpy.egg-info/
+-rw-rw-rw-   0        0        0      175 2023-04-22 05:11:39.000000 yashpy-0.2/yashpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-04-22 05:11:39.000000 yashpy-0.2/yashpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 05:11:39.000000 yashpy-0.2/yashpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-22 05:11:39.000000 yashpy-0.2/yashpy.egg-info/top_level.txt
```

