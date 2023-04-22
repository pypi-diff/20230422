# Comparing `tmp/pmserializer-1.0.1.tar.gz` & `tmp/pmserializer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmserializer-1.0.1.tar", last modified: Fri Apr 21 16:05:53 2023, max compression
+gzip compressed data, was "pmserializer-2.0.0.tar", last modified: Sat Apr 22 05:30:45 2023, max compression
```

## Comparing `pmserializer-1.0.1.tar` & `pmserializer-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 16:05:53.415856 pmserializer-1.0.1/
--rw-rw-rw-   0        0        0      221 2023-04-21 16:05:53.413488 pmserializer-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 16:05:53.344017 pmserializer-1.0.1/lab3/
--rw-rw-rw-   0        0        0     4534 2023-04-21 14:44:58.000000 pmserializer-1.0.1/lab3/DeserializerJson.py
--rw-rw-rw-   0        0        0     3857 2023-04-21 14:39:00.000000 pmserializer-1.0.1/lab3/DeserializerYaml.py
--rw-rw-rw-   0        0        0      641 2023-04-21 14:44:58.000000 pmserializer-1.0.1/lab3/Json.py
--rw-rw-rw-   0        0        0      367 2023-04-21 14:44:58.000000 pmserializer-1.0.1/lab3/SerializerFactory.py
--rw-rw-rw-   0        0        0     7068 2023-04-21 14:44:58.000000 pmserializer-1.0.1/lab3/SerializerJson.py
--rw-rw-rw-   0        0        0     5514 2023-04-21 14:44:58.000000 pmserializer-1.0.1/lab3/SerializerYaml.py
--rw-rw-rw-   0        0        0      689 2023-04-21 14:44:58.000000 pmserializer-1.0.1/lab3/Toml.py
--rw-rw-rw-   0        0        0      676 2023-04-21 14:44:58.000000 pmserializer-1.0.1/lab3/Yaml.py
--rw-rw-rw-   0        0        0        0 2023-04-21 14:39:00.000000 pmserializer-1.0.1/lab3/__init__.py
--rw-rw-rw-   0        0        0      279 2023-04-21 14:39:00.000000 pmserializer-1.0.1/lab3/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-21 16:05:53.409583 pmserializer-1.0.1/pmserializer.egg-info/
--rw-rw-rw-   0        0        0      221 2023-04-21 16:05:53.000000 pmserializer-1.0.1/pmserializer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-21 16:05:53.000000 pmserializer-1.0.1/pmserializer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 16:05:53.000000 pmserializer-1.0.1/pmserializer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-21 16:05:53.000000 pmserializer-1.0.1/pmserializer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-21 16:05:53.000000 pmserializer-1.0.1/pmserializer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 16:05:53.416387 pmserializer-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      311 2023-04-21 16:01:17.000000 pmserializer-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 05:30:45.537287 pmserializer-2.0.0/
+-rw-rw-rw-   0        0        0      221 2023-04-22 05:30:45.536290 pmserializer-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-22 05:30:45.509958 pmserializer-2.0.0/lab3/
+-rw-rw-rw-   0        0        0     4534 2023-04-21 14:44:58.000000 pmserializer-2.0.0/lab3/DeserializerJson.py
+-rw-rw-rw-   0        0        0     3857 2023-04-21 14:39:00.000000 pmserializer-2.0.0/lab3/DeserializerYaml.py
+-rw-rw-rw-   0        0        0      641 2023-04-21 14:44:58.000000 pmserializer-2.0.0/lab3/Json.py
+-rw-rw-rw-   0        0        0      367 2023-04-21 14:44:58.000000 pmserializer-2.0.0/lab3/SerializerFactory.py
+-rw-rw-rw-   0        0        0     7068 2023-04-21 14:44:58.000000 pmserializer-2.0.0/lab3/SerializerJson.py
+-rw-rw-rw-   0        0        0     5514 2023-04-21 14:44:58.000000 pmserializer-2.0.0/lab3/SerializerYaml.py
+-rw-rw-rw-   0        0        0      689 2023-04-21 14:44:58.000000 pmserializer-2.0.0/lab3/Toml.py
+-rw-rw-rw-   0        0        0      676 2023-04-21 14:44:58.000000 pmserializer-2.0.0/lab3/Yaml.py
+-rw-rw-rw-   0        0        0      112 2023-04-22 05:30:24.000000 pmserializer-2.0.0/lab3/__init__.py
+-rw-rw-rw-   0        0        0      279 2023-04-21 14:39:00.000000 pmserializer-2.0.0/lab3/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-22 05:30:45.534295 pmserializer-2.0.0/pmserializer.egg-info/
+-rw-rw-rw-   0        0        0      221 2023-04-22 05:30:45.000000 pmserializer-2.0.0/pmserializer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-04-22 05:30:45.000000 pmserializer-2.0.0/pmserializer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 05:30:45.000000 pmserializer-2.0.0/pmserializer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-22 05:30:45.000000 pmserializer-2.0.0/pmserializer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-22 05:30:45.000000 pmserializer-2.0.0/pmserializer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 05:30:45.537287 pmserializer-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      311 2023-04-22 05:30:24.000000 pmserializer-2.0.0/setup.py
```

### Comparing `pmserializer-1.0.1/lab3/DeserializerJson.py` & `pmserializer-2.0.0/lab3/DeserializerJson.py`

 * *Files identical despite different names*

### Comparing `pmserializer-1.0.1/lab3/DeserializerYaml.py` & `pmserializer-2.0.0/lab3/DeserializerYaml.py`

 * *Files identical despite different names*

### Comparing `pmserializer-1.0.1/lab3/Json.py` & `pmserializer-2.0.0/lab3/Json.py`

 * *Files identical despite different names*

### Comparing `pmserializer-1.0.1/lab3/SerializerJson.py` & `pmserializer-2.0.0/lab3/SerializerJson.py`

 * *Files identical despite different names*

### Comparing `pmserializer-1.0.1/lab3/SerializerYaml.py` & `pmserializer-2.0.0/lab3/SerializerYaml.py`

 * *Files identical despite different names*

### Comparing `pmserializer-1.0.1/lab3/Toml.py` & `pmserializer-2.0.0/lab3/Toml.py`

 * *Files identical despite different names*

### Comparing `pmserializer-1.0.1/lab3/Yaml.py` & `pmserializer-2.0.0/lab3/Yaml.py`

 * *Files identical despite different names*

