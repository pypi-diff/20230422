# Comparing `tmp/secucPy-0.1.tar.gz` & `tmp/secucPy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secucPy-0.1.tar", last modified: Fri Apr 21 02:52:39 2023, max compression
+gzip compressed data, was "secucPy-0.2.tar", last modified: Sat Apr 22 20:30:26 2023, max compression
```

## Comparing `secucPy-0.1.tar` & `secucPy-0.2.tar`

### file list

```diff
@@ -1,16 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 02:52:39.251708 secucPy-0.1/
--rw-rw-rw-   0        0        0      203 2023-04-21 02:52:39.252695 secucPy-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       62 2023-04-20 21:05:57.000000 secucPy-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 02:52:39.213033 secucPy-0.1/secucpy/
-drwxrwxrwx   0        0        0        0 2023-04-21 02:52:39.224606 secucPy-0.1/secucpy/client/
--rw-rw-rw-   0        0        0        0 2023-04-20 20:52:54.000000 secucPy-0.1/secucpy/client/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-20 20:53:08.000000 secucPy-0.1/secucpy/client/__main__.py
--rw-rw-rw-   0        0        0     2825 2023-04-20 22:49:16.000000 secucPy-0.1/secucpy/client/transfer.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:52:39.249493 secucPy-0.1/secucpy/secucPy.egg-info/
--rw-rw-rw-   0        0        0      203 2023-04-21 02:52:39.000000 secucPy-0.1/secucpy/secucPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-21 02:52:39.000000 secucPy-0.1/secucpy/secucPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 02:52:39.000000 secucPy-0.1/secucpy/secucPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-21 02:52:39.000000 secucPy-0.1/secucpy/secucPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 02:52:39.000000 secucPy-0.1/secucpy/secucPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-04-21 02:52:39.254691 secucPy-0.1/setup.cfg
--rw-rw-rw-   0        0        0      409 2023-04-21 02:51:56.000000 secucPy-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 20:30:26.228955 secucPy-0.2/
+-rw-rw-rw-   0        0        0      203 2023-04-22 20:30:26.228955 secucPy-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-04-21 20:00:38.000000 secucPy-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 20:30:26.210946 secucPy-0.2/secucpy/
+drwxrwxrwx   0        0        0        0 2023-04-22 20:30:26.226954 secucPy-0.2/secucpy/secucPy.egg-info/
+-rw-rw-rw-   0        0        0      203 2023-04-22 20:30:26.000000 secucPy-0.2/secucpy/secucPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-04-22 20:30:26.000000 secucPy-0.2/secucpy/secucPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 20:30:26.000000 secucPy-0.2/secucpy/secucPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-22 20:30:26.000000 secucPy-0.2/secucpy/secucPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 20:30:26.000000 secucPy-0.2/secucpy/secucPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-04-22 20:30:26.229954 secucPy-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      450 2023-04-22 20:30:14.000000 secucPy-0.2/setup.py
```

