# Comparing `tmp/pyrew-0.4.1.tar.gz` & `tmp/pyrew-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrew-0.4.1.tar", last modified: Sat Apr 22 05:44:20 2023, max compression
+gzip compressed data, was "pyrew-0.5.1.tar", last modified: Sat Apr 22 05:54:30 2023, max compression
```

## Comparing `pyrew-0.4.1.tar` & `pyrew-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 05:44:20.789080 pyrew-0.4.1/
--rw-rw-rw-   0        0        0      357 2023-04-22 05:44:20.785729 pyrew-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-04-22 05:25:08.000000 pyrew-0.4.1/README.md
--rw-rw-rw-   0        0        0       91 2023-04-22 04:22:49.000000 pyrew-0.4.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-22 05:44:20.780547 pyrew-0.4.1/pyrew.egg-info/
--rw-rw-rw-   0        0        0      357 2023-04-22 05:44:20.000000 pyrew-0.4.1/pyrew.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-22 05:44:20.000000 pyrew-0.4.1/pyrew.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 05:44:20.000000 pyrew-0.4.1/pyrew.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-22 05:44:20.000000 pyrew-0.4.1/pyrew.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6185 2023-04-22 04:50:28.000000 pyrew-0.4.1/pyrew.py
--rw-rw-rw-   0        0        0       42 2023-04-22 05:44:20.791087 pyrew-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0      525 2023-04-22 05:43:19.000000 pyrew-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 05:54:30.063939 pyrew-0.5.1/
+-rw-rw-rw-   0        0        0      705 2023-04-22 05:54:30.062948 pyrew-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2023-04-22 05:54:13.000000 pyrew-0.5.1/README.rst
+-rw-rw-rw-   0        0        0       91 2023-04-22 04:22:49.000000 pyrew-0.5.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-22 05:54:30.060025 pyrew-0.5.1/pyrew.egg-info/
+-rw-rw-rw-   0        0        0      705 2023-04-22 05:54:29.000000 pyrew-0.5.1/pyrew.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-04-22 05:54:29.000000 pyrew-0.5.1/pyrew.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 05:54:29.000000 pyrew-0.5.1/pyrew.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-22 05:54:29.000000 pyrew-0.5.1/pyrew.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6185 2023-04-22 05:54:18.000000 pyrew-0.5.1/pyrew.py
+-rw-rw-rw-   0        0        0       42 2023-04-22 05:54:30.064940 pyrew-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      497 2023-04-22 05:54:14.000000 pyrew-0.5.1/setup.py
```

### Comparing `pyrew-0.4.1/pyrew.py` & `pyrew-0.5.1/pyrew.py`

 * *Files identical despite different names*

