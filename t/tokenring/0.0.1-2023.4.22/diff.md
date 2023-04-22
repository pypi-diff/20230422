# Comparing `tmp/tokenring-0.0.1.tar.gz` & `tmp/tokenring-2023.4.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenring-0.0.1.tar", last modified: Tue Apr 11 18:54:28 2023, max compression
+gzip compressed data, was "tokenring-2023.4.22.tar", last modified: Sat Apr 22 16:38:08 2023, max compression
```

## Comparing `tokenring-0.0.1.tar` & `tokenring-2023.4.22.tar`

### file list

```diff
@@ -1,9 +1,25 @@
-drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-04-11 18:54:28.751868 tokenring-0.0.1/
--rw-r--r--   0 glyph      (501) staff       (20)      210 2023-04-11 18:54:28.751766 tokenring-0.0.1/PKG-INFO
--rw-r--r--   0 glyph      (501) staff       (20)       38 2023-04-11 18:54:28.751903 tokenring-0.0.1/setup.cfg
--rw-r--r--   0 glyph      (501) staff       (20)      312 2023-04-11 18:54:04.000000 tokenring-0.0.1/setup.py
-drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-04-11 18:54:28.751633 tokenring-0.0.1/tokenring.egg-info/
--rw-r--r--   0 glyph      (501) staff       (20)      210 2023-04-11 18:54:28.000000 tokenring-0.0.1/tokenring.egg-info/PKG-INFO
--rw-r--r--   0 glyph      (501) staff       (20)      140 2023-04-11 18:54:28.000000 tokenring-0.0.1/tokenring.egg-info/SOURCES.txt
--rw-r--r--   0 glyph      (501) staff       (20)        1 2023-04-11 18:54:28.000000 tokenring-0.0.1/tokenring.egg-info/dependency_links.txt
--rw-r--r--   0 glyph      (501) staff       (20)        1 2023-04-11 18:54:28.000000 tokenring-0.0.1/tokenring.egg-info/top_level.txt
+drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-04-22 16:38:08.397535 tokenring-2023.4.22/
+-rw-r--r--   0 glyph      (501) staff       (20)       77 2023-04-22 16:38:08.397420 tokenring-2023.4.22/PKG-INFO
+-rw-r--r--   0 glyph      (501) staff       (20)     4956 2023-04-13 07:28:45.000000 tokenring-2023.4.22/README.rst
+-rw-r--r--   0 glyph      (501) staff       (20)      993 2023-04-22 15:03:11.000000 tokenring-2023.4.22/pyproject.toml
+-rw-r--r--   0 glyph      (501) staff       (20)       38 2023-04-22 16:38:08.397569 tokenring-2023.4.22/setup.cfg
+drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-04-22 16:38:08.393876 tokenring-2023.4.22/src/
+drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-04-22 16:38:08.395915 tokenring-2023.4.22/src/tokenring/
+-rw-r--r--   0 glyph      (501) staff       (20)        0 2023-04-11 05:37:16.000000 tokenring-2023.4.22/src/tokenring/__init__.py
+drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-04-22 16:38:08.397281 tokenring-2023.4.22/src/tokenring/agent/
+-rw-r--r--   0 glyph      (501) staff       (20)     2481 2023-04-11 18:39:19.000000 tokenring-2023.4.22/src/tokenring/agent/_admin_pipe.py
+-rw-r--r--   0 glyph      (501) staff       (20)     2392 2023-04-22 02:15:48.000000 tokenring-2023.4.22/src/tokenring/agent/client.py
+-rw-r--r--   0 glyph      (501) staff       (20)      669 2023-04-12 03:50:18.000000 tokenring-2023.4.22/src/tokenring/agent/common.py
+-rw-r--r--   0 glyph      (501) staff       (20)     3225 2023-04-13 07:15:03.000000 tokenring-2023.4.22/src/tokenring/cli.py
+-rw-r--r--   0 glyph      (501) staff       (20)     2234 2023-04-12 03:50:49.000000 tokenring-2023.4.22/src/tokenring/fidoclient.py
+-rw-r--r--   0 glyph      (501) staff       (20)     6909 2023-04-12 03:50:49.000000 tokenring-2023.4.22/src/tokenring/handles.py
+-rw-r--r--   0 glyph      (501) staff       (20)     3655 2023-04-12 04:08:16.000000 tokenring-2023.4.22/src/tokenring/interaction.py
+-rw-r--r--   0 glyph      (501) staff       (20)     1366 2023-04-12 03:50:49.000000 tokenring-2023.4.22/src/tokenring/local.py
+-rw-r--r--   0 glyph      (501) staff       (20)     6262 2023-04-22 02:18:20.000000 tokenring-2023.4.22/src/tokenring/vault.py
+drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-04-22 16:38:08.396561 tokenring-2023.4.22/src/tokenring.egg-info/
+-rw-r--r--   0 glyph      (501) staff       (20)       77 2023-04-22 16:38:08.000000 tokenring-2023.4.22/src/tokenring.egg-info/PKG-INFO
+-rw-r--r--   0 glyph      (501) staff       (20)      519 2023-04-22 16:38:08.000000 tokenring-2023.4.22/src/tokenring.egg-info/SOURCES.txt
+-rw-r--r--   0 glyph      (501) staff       (20)        1 2023-04-22 16:38:08.000000 tokenring-2023.4.22/src/tokenring.egg-info/dependency_links.txt
+-rw-r--r--   0 glyph      (501) staff       (20)      143 2023-04-22 16:38:08.000000 tokenring-2023.4.22/src/tokenring.egg-info/entry_points.txt
+-rw-r--r--   0 glyph      (501) staff       (20)       99 2023-04-22 16:38:08.000000 tokenring-2023.4.22/src/tokenring.egg-info/requires.txt
+-rw-r--r--   0 glyph      (501) staff       (20)       10 2023-04-22 16:38:08.000000 tokenring-2023.4.22/src/tokenring.egg-info/top_level.txt
```

