# Comparing `tmp/pybricks_jedi-1.7.0.tar.gz` & `tmp/pybricks_jedi-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybricks_jedi-1.7.0.tar", max compression
+gzip compressed data, was "pybricks_jedi-1.8.0.tar", max compression
```

## Comparing `pybricks_jedi-1.7.0.tar` & `pybricks_jedi-1.8.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     1077 2022-12-28 22:10:31.332337 pybricks_jedi-1.7.0/LICENSE
--rw-r--r--   0        0        0      612 2022-12-28 22:10:31.332337 pybricks_jedi-1.7.0/pyproject.toml
--rw-r--r--   0        0        0    14717 2022-12-28 22:10:31.332337 pybricks_jedi-1.7.0/src/pybricks_jedi/__init__.py
--rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 pybricks_jedi-1.7.0/setup.py
--rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 pybricks_jedi-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-21 22:27:39.399066 pybricks_jedi-1.8.0/LICENSE
+-rw-r--r--   0        0        0      612 2023-04-21 22:27:39.399066 pybricks_jedi-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0    14663 2023-04-21 22:27:39.399066 pybricks_jedi-1.8.0/src/pybricks_jedi/__init__.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 pybricks_jedi-1.8.0/PKG-INFO
```

### Comparing `pybricks_jedi-1.7.0/LICENSE` & `pybricks_jedi-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybricks_jedi-1.7.0/pyproject.toml` & `pybricks_jedi-1.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "pybricks_jedi"
-version = "1.7.0"
+version = "1.8.0"
 description = "Code completion for Pybricks."
 authors = ["The Pybricks Authors <team@pybricks.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = ">= 3.10, < 3.11"
-pybricks = "3.2.0c1"
+python = ">= 3.10, < 3.12"
+pybricks = "3.3.0a4"
 jedi = "0.18.1"
 typing-extensions = "4.2.0"
 docstring-parser = "0.14.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 black = "^22.3.0"
```

### Comparing `pybricks_jedi-1.7.0/src/pybricks_jedi/__init__.py` & `pybricks_jedi-1.8.0/src/pybricks_jedi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from jedi.api.classes import BaseName, Completion, Name, ParamName, Signature
 from typing_extensions import NotRequired, TypedDict
 
 # Packages included in Pybricks firmware that ships with Pybricks Code.
 PYBRICKS_CODE_PACKAGES = {
     "micropython",
     "pybricks",
-    "pybricks.geometry",
     "pybricks.hubs",
     "pybricks.iodevices",
     "pybricks.parameters",
     "pybricks.pupdevices",
     "pybricks.robotics",
     "pybricks.tools",
     "uerrno",
@@ -485,15 +484,14 @@
     jedi.preload_module(
         "typing",
         "enum",
         "micropython",
         "pybricks._common",
         "pybricks.ev3dev",
         "pybricks.ev3dev.speaker",
-        "pybricks.geometry",
         "pybricks.hubs",
         "pybricks.iodevices",
         "pybricks.parameters",
         "pybricks.pupdevices",
         "pybricks.robotics",
         "pybricks.tools",
         "pybricks",
```

