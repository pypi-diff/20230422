# Comparing `tmp/maxilearn-0.5.0.tar.gz` & `tmp/maxilearn-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxilearn-0.5.0.tar", last modified: Fri Apr 21 16:49:06 2023, max compression
+gzip compressed data, was "maxilearn-4.1.tar", last modified: Sat Apr 22 17:15:37 2023, max compression
```

## Comparing `maxilearn-0.5.0.tar` & `maxilearn-4.1.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 16:49:06.060713 maxilearn-0.5.0/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 maxilearn-0.5.0/LICENSE
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      243 2023-04-21 16:49:06.060538 maxilearn-0.5.0/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 maxilearn-0.5.0/README.md
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 16:49:06.060284 maxilearn-0.5.0/maxilearn.egg-info/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      243 2023-04-21 16:49:06.000000 maxilearn-0.5.0/maxilearn.egg-info/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      190 2023-04-21 16:49:06.000000 maxilearn-0.5.0/maxilearn.egg-info/SOURCES.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-21 16:49:06.000000 maxilearn-0.5.0/maxilearn.egg-info/dependency_links.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       36 2023-04-21 16:49:06.000000 maxilearn-0.5.0/maxilearn.egg-info/requires.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-21 16:49:06.000000 maxilearn-0.5.0/maxilearn.egg-info/top_level.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       38 2023-04-21 16:49:06.060773 maxilearn-0.5.0/setup.cfg
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      406 2023-04-21 16:48:52.000000 maxilearn-0.5.0/setup.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-22 17:15:37.403842 maxilearn-4.1/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 maxilearn-4.1/LICENSE
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-22 17:15:37.403946 maxilearn-4.1/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 maxilearn-4.1/README.md
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-22 17:15:37.397660 maxilearn-4.1/maxilearn/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       74 2023-04-22 16:51:44.000000 maxilearn-4.1/maxilearn/__init__.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    15015 2023-04-22 07:51:57.000000 maxilearn-4.1/maxilearn/classificators.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 maxilearn-4.1/maxilearn/regressors.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-22 17:15:37.403626 maxilearn-4.1/maxilearn.egg-info/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-22 17:15:37.000000 maxilearn-4.1/maxilearn.egg-info/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      274 2023-04-22 17:15:37.000000 maxilearn-4.1/maxilearn.egg-info/SOURCES.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-22 17:15:37.000000 maxilearn-4.1/maxilearn.egg-info/dependency_links.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       45 2023-04-22 17:15:37.000000 maxilearn-4.1/maxilearn.egg-info/requires.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       10 2023-04-22 17:15:37.000000 maxilearn-4.1/maxilearn.egg-info/top_level.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-22 17:15:37.404271 maxilearn-4.1/setup.cfg
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      854 2023-04-22 17:14:12.000000 maxilearn-4.1/setup.py
```

### Comparing `maxilearn-0.5.0/LICENSE` & `maxilearn-4.1/LICENSE`

 * *Files identical despite different names*

