# Comparing `tmp/hagis-0.3.1.tar.gz` & `tmp/hagis-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.3.1.tar", last modified: Thu Apr 20 00:35:24 2023, max compression
+gzip compressed data, was "hagis-0.3.2.tar", last modified: Sat Apr 22 03:03:30 2023, max compression
```

## Comparing `hagis-0.3.1.tar` & `hagis-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 00:35:24.333327 hagis-0.3.1/
--rw-rw-rw-   0        0        0      941 2023-04-20 00:35:24.328545 hagis-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 00:35:24.287274 hagis-0.3.1/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.3.1/hagis/__init__.py
--rw-rw-rw-   0        0        0    13056 2023-04-20 00:34:48.000000 hagis-0.3.1/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-20 00:35:24.315546 hagis-0.3.1/hagis.egg-info/
--rw-rw-rw-   0        0        0      941 2023-04-20 00:35:24.000000 hagis-0.3.1/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-20 00:35:24.000000 hagis-0.3.1/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 00:35:24.000000 hagis-0.3.1/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 00:35:24.000000 hagis-0.3.1/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-20 00:34:33.000000 hagis-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-20 00:35:24.333327 hagis-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-22 03:03:30.870926 hagis-0.3.2/
+-rw-rw-rw-   0        0        0      923 2023-04-22 03:03:30.862928 hagis-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-04-22 02:10:21.000000 hagis-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 03:03:30.822360 hagis-0.3.2/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.3.2/hagis/__init__.py
+-rw-rw-rw-   0        0        0    13057 2023-04-22 03:01:48.000000 hagis-0.3.2/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-22 03:03:30.854939 hagis-0.3.2/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-04-22 03:03:30.000000 hagis-0.3.2/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-22 03:03:30.000000 hagis-0.3.2/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 03:03:30.000000 hagis-0.3.2/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-22 03:03:30.000000 hagis-0.3.2/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-22 02:59:04.000000 hagis-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-22 03:03:30.870926 hagis-0.3.2/setup.cfg
```

### Comparing `hagis-0.3.1/PKG-INFO` & `hagis-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.3.1
+Version: 0.3.2
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Hagis
 
-A high availability GIS client
+A GIS client
 
 ```python
 from hagis import Layer, Point
 
 class City:
     objectid: int
     areaname: str
```

### Comparing `hagis-0.3.1/hagis/hagis.py` & `hagis-0.3.2/hagis/hagis.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
             else:
                 attributes[field] = value
 
         return dictionary
 
     def _post(self, url: str, **kwargs: Any) -> SimpleNamespace:
         kwargs["f"] = "json"
-        response = post(url, timeout=2, data=kwargs)
+        response = post(url, data=kwargs, timeout=10)
         obj = loads(response.text, object_hook=lambda x: SimpleNamespace(**x))
 
         if hasattr(obj, "error"):
             raise RuntimeError(obj.error.message)
 
         return obj
```

### Comparing `hagis-0.3.1/hagis.egg-info/PKG-INFO` & `hagis-0.3.2/hagis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.3.1
+Version: 0.3.2
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Hagis
 
-A high availability GIS client
+A GIS client
 
 ```python
 from hagis import Layer, Point
 
 class City:
     objectid: int
     areaname: str
```

### Comparing `hagis-0.3.1/pyproject.toml` & `hagis-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

