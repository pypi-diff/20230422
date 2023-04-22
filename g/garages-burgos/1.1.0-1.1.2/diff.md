# Comparing `tmp/garages_burgos-1.1.0.tar.gz` & `tmp/garages_burgos-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garages_burgos-1.1.0.tar", max compression
+gzip compressed data, was "garages_burgos-1.1.2.tar", max compression
```

## Comparing `garages_burgos-1.1.0.tar` & `garages_burgos-1.1.2.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0      340 2021-06-19 11:05:50.047064 garages_burgos-1.1.0/README.md
--rw-r--r--   0        0        0     1969 2021-06-19 11:05:50.047064 garages_burgos-1.1.0/garages_burgos/__init__.py
--rw-r--r--   0        0        0     1132 2021-06-19 11:06:20.759255 garages_burgos-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1092 2021-06-19 11:06:21.356644 garages_burgos-1.1.0/setup.py
--rw-r--r--   0        0        0     1328 2021-06-19 11:06:21.356919 garages_burgos-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      340 2023-04-22 10:47:56.134356 garages_burgos-1.1.2/README.md
+-rw-r--r--   0        0        0     1599 2023-04-22 10:47:56.134356 garages_burgos-1.1.2/garages_burgos/__init__.py
+-rw-r--r--   0        0        0     1101 2023-04-22 10:48:23.190792 garages_burgos-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 garages_burgos-1.1.2/PKG-INFO
```

### Comparing `garages_burgos-1.1.0/pyproject.toml` & `garages_burgos-1.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "garages_burgos"
-version = "1.1.0"
+version = "1.1.2"
 description = "Asynchronous Python client for getting garage occupancy in Burgos"
 authors = ["ricveal <ricveal@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ricveal/garages_burgos"
 repository = "https://github.com/ricveal/garages_burgos"
 keywords = ["garages", "burgos", "occupancy", "api", "async", "client"]
@@ -19,16 +19,14 @@
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 aiohttp = "^3.0.0"
-bs4 = "^0.0.1"
-lxml = "^4.6.3"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^3.9.2"
 pytest = "^6.2.4"
 black = "^21.6b0"
 pytest-watch = "^4.2.0"
 pytest-mock = "^3.6.1"
```

