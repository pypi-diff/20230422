# Comparing `tmp/yadisk-1.3.2.tar.gz` & `tmp/yadisk-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yadisk-1.3.2.tar", last modified: Mon Mar 20 12:44:34 2023, max compression
+gzip compressed data, was "yadisk-1.3.3.tar", last modified: Sat Apr 22 10:19:42 2023, max compression
```

## Comparing `yadisk-1.3.2.tar` & `yadisk-1.3.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-03-20 12:44:34.845604 yadisk-1.3.2/
--rw-r--r--   0 ivan      (1000) ivan      (1000)    35147 2022-08-16 16:14:20.000000 yadisk-1.3.2/COPYING
--rw-r--r--   0 ivan      (1000) ivan      (1000)     7649 2022-08-16 16:14:20.000000 yadisk-1.3.2/COPYING.lesser
--rw-r--r--   0 ivan      (1000) ivan      (1000)      126 2023-01-30 14:51:04.000000 yadisk-1.3.2/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)    13716 2023-03-20 12:44:34.845604 yadisk-1.3.2/PKG-INFO
--rw-r--r--   0 ivan      (1000) ivan      (1000)     9727 2023-03-20 12:03:24.000000 yadisk-1.3.2/README.en.rst
--rw-r--r--   0 ivan      (1000) ivan      (1000)    12485 2023-03-20 12:03:47.000000 yadisk-1.3.2/README.rst
--rw-r--r--   0 ivan      (1000) ivan      (1000)    12485 2023-03-20 12:03:39.000000 yadisk-1.3.2/README.ru.rst
--rw-r--r--   0 ivan      (1000) ivan      (1000)       38 2023-03-20 12:44:34.845604 yadisk-1.3.2/setup.cfg
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1705 2023-03-20 12:01:36.000000 yadisk-1.3.2/setup.py
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-03-20 12:44:34.842604 yadisk-1.3.2/yadisk/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      121 2023-03-20 12:01:43.000000 yadisk-1.3.2/yadisk/__init__.py
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-03-20 12:44:34.844604 yadisk-1.3.2/yadisk/api/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      177 2022-08-16 16:14:20.000000 yadisk-1.3.2/yadisk/api/__init__.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     4887 2023-01-30 14:51:04.000000 yadisk-1.3.2/yadisk/api/api_request.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     4944 2023-01-30 14:51:04.000000 yadisk-1.3.2/yadisk/api/auth.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1212 2023-01-30 14:51:04.000000 yadisk-1.3.2/yadisk/api/disk.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1996 2023-01-30 14:51:04.000000 yadisk-1.3.2/yadisk/api/operations.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)    44614 2023-01-30 14:51:04.000000 yadisk-1.3.2/yadisk/api/resources.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     2990 2023-01-30 14:51:04.000000 yadisk-1.3.2/yadisk/common.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      357 2023-01-30 14:51:04.000000 yadisk-1.3.2/yadisk/compat.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     4744 2023-01-30 14:51:04.000000 yadisk-1.3.2/yadisk/exceptions.py
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-03-20 12:44:34.845604 yadisk-1.3.2/yadisk/objects/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      207 2022-08-16 16:14:20.000000 yadisk-1.3.2/yadisk/objects/__init__.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1722 2023-01-30 14:51:04.000000 yadisk-1.3.2/yadisk/objects/auth.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     6780 2023-01-30 14:51:04.000000 yadisk-1.3.2/yadisk/objects/disk.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      761 2023-01-30 14:51:04.000000 yadisk-1.3.2/yadisk/objects/error_object.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1293 2023-01-30 14:51:04.000000 yadisk-1.3.2/yadisk/objects/operations.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)    71422 2023-02-28 14:35:09.000000 yadisk-1.3.2/yadisk/objects/resources.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     4082 2023-01-30 14:51:04.000000 yadisk-1.3.2/yadisk/objects/yadisk_object.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)        0 2023-01-30 14:51:04.000000 yadisk-1.3.2/yadisk/py.typed
--rw-r--r--   0 ivan      (1000) ivan      (1000)      651 2022-08-16 16:14:20.000000 yadisk-1.3.2/yadisk/settings.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     3935 2023-01-30 14:51:04.000000 yadisk-1.3.2/yadisk/utils.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)    69945 2023-03-20 11:58:17.000000 yadisk-1.3.2/yadisk/yadisk.py
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-03-20 12:44:34.843604 yadisk-1.3.2/yadisk.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)    13716 2023-03-20 12:44:34.000000 yadisk-1.3.2/yadisk.egg-info/PKG-INFO
--rw-r--r--   0 ivan      (1000) ivan      (1000)      702 2023-03-20 12:44:34.000000 yadisk-1.3.2/yadisk.egg-info/SOURCES.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)        1 2023-03-20 12:44:34.000000 yadisk-1.3.2/yadisk.egg-info/dependency_links.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)        9 2023-03-20 12:44:34.000000 yadisk-1.3.2/yadisk.egg-info/requires.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)        7 2023-03-20 12:44:34.000000 yadisk-1.3.2/yadisk.egg-info/top_level.txt
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-04-22 10:19:42.112524 yadisk-1.3.3/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    35147 2022-08-16 16:14:20.000000 yadisk-1.3.3/COPYING
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     7649 2022-08-16 16:14:20.000000 yadisk-1.3.3/COPYING.lesser
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      126 2023-01-30 14:51:04.000000 yadisk-1.3.3/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    13857 2023-04-22 10:19:42.112524 yadisk-1.3.3/PKG-INFO
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     9824 2023-04-22 10:18:42.000000 yadisk-1.3.3/README.en.rst
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    12626 2023-04-22 10:18:42.000000 yadisk-1.3.3/README.rst
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    12626 2023-04-22 10:18:42.000000 yadisk-1.3.3/README.ru.rst
+-rw-r--r--   0 ivan      (1000) ivan      (1000)       38 2023-04-22 10:19:42.112524 yadisk-1.3.3/setup.cfg
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1705 2023-04-22 10:18:42.000000 yadisk-1.3.3/setup.py
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-04-22 10:19:42.109524 yadisk-1.3.3/yadisk/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      121 2023-04-22 10:18:42.000000 yadisk-1.3.3/yadisk/__init__.py
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-04-22 10:19:42.111524 yadisk-1.3.3/yadisk/api/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      177 2022-08-16 16:14:20.000000 yadisk-1.3.3/yadisk/api/__init__.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     4887 2023-01-30 14:51:04.000000 yadisk-1.3.3/yadisk/api/api_request.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     4944 2023-01-30 14:51:04.000000 yadisk-1.3.3/yadisk/api/auth.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1212 2023-01-30 14:51:04.000000 yadisk-1.3.3/yadisk/api/disk.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1996 2023-01-30 14:51:04.000000 yadisk-1.3.3/yadisk/api/operations.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    44614 2023-01-30 14:51:04.000000 yadisk-1.3.3/yadisk/api/resources.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     3047 2023-04-22 10:18:42.000000 yadisk-1.3.3/yadisk/common.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      357 2023-01-30 14:51:04.000000 yadisk-1.3.3/yadisk/compat.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     4744 2023-01-30 14:51:04.000000 yadisk-1.3.3/yadisk/exceptions.py
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-04-22 10:19:42.112524 yadisk-1.3.3/yadisk/objects/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      207 2022-08-16 16:14:20.000000 yadisk-1.3.3/yadisk/objects/__init__.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1722 2023-01-30 14:51:04.000000 yadisk-1.3.3/yadisk/objects/auth.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     6780 2023-01-30 14:51:04.000000 yadisk-1.3.3/yadisk/objects/disk.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      761 2023-01-30 14:51:04.000000 yadisk-1.3.3/yadisk/objects/error_object.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1293 2023-01-30 14:51:04.000000 yadisk-1.3.3/yadisk/objects/operations.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    71422 2023-02-28 14:35:09.000000 yadisk-1.3.3/yadisk/objects/resources.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     4082 2023-01-30 14:51:04.000000 yadisk-1.3.3/yadisk/objects/yadisk_object.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)        0 2023-01-30 14:51:04.000000 yadisk-1.3.3/yadisk/py.typed
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      651 2022-08-16 16:14:20.000000 yadisk-1.3.3/yadisk/settings.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     3935 2023-01-30 14:51:04.000000 yadisk-1.3.3/yadisk/utils.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    69945 2023-03-20 12:48:10.000000 yadisk-1.3.3/yadisk/yadisk.py
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-04-22 10:19:42.110524 yadisk-1.3.3/yadisk.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    13857 2023-04-22 10:19:42.000000 yadisk-1.3.3/yadisk.egg-info/PKG-INFO
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      702 2023-04-22 10:19:42.000000 yadisk-1.3.3/yadisk.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)        1 2023-04-22 10:19:42.000000 yadisk-1.3.3/yadisk.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)        9 2023-04-22 10:19:42.000000 yadisk-1.3.3/yadisk.egg-info/requires.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)        7 2023-04-22 10:19:42.000000 yadisk-1.3.3/yadisk.egg-info/top_level.txt
```

### Comparing `yadisk-1.3.2/COPYING` & `yadisk-1.3.3/COPYING`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/COPYING.lesser` & `yadisk-1.3.3/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/PKG-INFO` & `yadisk-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yadisk
-Version: 1.3.2
+Version: 1.3.3
 Summary: Библиотека-клиент REST API Яндекс.Диска / Yandex.Disk REST API client library
 Home-page: https://github.com/ivknv/yadisk
 Author: Ivan Konovalov
 Author-email: ivknv0@gmail.com
 License: LGPLv3
 Project-URL: Source code, https://github.com/ivknv/yadisk
 Project-URL: Documentation (EN), https://yadisk.readthedocs.io/en/latest
@@ -102,14 +102,18 @@
 .. _issue #4: https://github.com/ivknv/yadisk/issues/4
 .. _issue #7: https://github.com/ivknv/yadisk/issues/7
 .. _issue #23: https://github.com/ivknv/yadisk/issues/23
 .. _issue #26: https://github.com/ivknv/yadisk/issues/26
 .. _issue #28: https://github.com/ivknv/yadisk/issues/28
 .. _issue #29: https://github.com/ivknv/yadisk/issues/29
 
+* **Release 1.3.3 (2023-04-22)**
+
+  * Пути вида :code:`app:/` теперь работают правильно (см. `issue #26`_)
+
 * **Release 1.3.2 (2023-03-20)**
 
   * Исправлено `issue #29`_: TypeError: 'type' object is not subscriptable
 
 * **Release 1.3.1 (2023-02-28)**
 
   * Исправлено `issue #28`_: :code:`TypeError` при вызове :code:`download_public()` с параметром :code:`path`
```

### Comparing `yadisk-1.3.2/README.en.rst` & `yadisk-1.3.3/README.en.rst`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,18 @@
 .. _issue #4: https://github.com/ivknv/yadisk/issues/4
 .. _issue #7: https://github.com/ivknv/yadisk/issues/7
 .. _issue #23: https://github.com/ivknv/yadisk/issues/23
 .. _issue #26: https://github.com/ivknv/yadisk/issues/26
 .. _issue #28: https://github.com/ivknv/yadisk/issues/28
 .. _issue #29: https://github.com/ivknv/yadisk/issues/29
 
+* **Release 1.3.3 (2023-04-22)**
+
+  * :code:`app:/` paths now work correctly (see `issue #26`_)
+
 * **Release 1.3.2 (2023-03-20)**
 
   * Fixed `issue #29`_: TypeError: 'type' object is not subscriptable
 
 * **Release 1.3.1 (2023-02-28)**
 
   * Fixed `issue #28`_: calling :code:`download_public()` with :code:`path` keyword argument raises :code:`TypeError`
```

### Comparing `yadisk-1.3.2/README.rst` & `yadisk-1.3.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,18 @@
 .. _issue #4: https://github.com/ivknv/yadisk/issues/4
 .. _issue #7: https://github.com/ivknv/yadisk/issues/7
 .. _issue #23: https://github.com/ivknv/yadisk/issues/23
 .. _issue #26: https://github.com/ivknv/yadisk/issues/26
 .. _issue #28: https://github.com/ivknv/yadisk/issues/28
 .. _issue #29: https://github.com/ivknv/yadisk/issues/29
 
+* **Release 1.3.3 (2023-04-22)**
+
+  * Пути вида :code:`app:/` теперь работают правильно (см. `issue #26`_)
+
 * **Release 1.3.2 (2023-03-20)**
 
   * Исправлено `issue #29`_: TypeError: 'type' object is not subscriptable
 
 * **Release 1.3.1 (2023-02-28)**
 
   * Исправлено `issue #28`_: :code:`TypeError` при вызове :code:`download_public()` с параметром :code:`path`
```

### Comparing `yadisk-1.3.2/README.ru.rst` & `yadisk-1.3.3/README.ru.rst`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,18 @@
 .. _issue #4: https://github.com/ivknv/yadisk/issues/4
 .. _issue #7: https://github.com/ivknv/yadisk/issues/7
 .. _issue #23: https://github.com/ivknv/yadisk/issues/23
 .. _issue #26: https://github.com/ivknv/yadisk/issues/26
 .. _issue #28: https://github.com/ivknv/yadisk/issues/28
 .. _issue #29: https://github.com/ivknv/yadisk/issues/29
 
+* **Release 1.3.3 (2023-04-22)**
+
+  * Пути вида :code:`app:/` теперь работают правильно (см. `issue #26`_)
+
 * **Release 1.3.2 (2023-03-20)**
 
   * Исправлено `issue #29`_: TypeError: 'type' object is not subscriptable
 
 * **Release 1.3.1 (2023-02-28)**
 
   * Исправлено `issue #28`_: :code:`TypeError` при вызове :code:`download_public()` с параметром :code:`path`
```

### Comparing `yadisk-1.3.2/setup.py` & `yadisk-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 module_dir = os.path.dirname(__file__)
 
 with codecs.open(os.path.join(module_dir, "README.rst"), encoding="utf8") as f:
     long_description = f.read()
 
 setup(name="yadisk",
-      version="1.3.2",
+      version="1.3.3",
       packages=find_packages(exclude=("tests",)),
       description="Библиотека-клиент REST API Яндекс.Диска / Yandex.Disk REST API client library",
       long_description=long_description,
       author="Ivan Konovalov",
       author_email="ivknv0@gmail.com",
       license="LGPLv3",
       python_requires=">=3.8",
```

### Comparing `yadisk-1.3.2/yadisk/api/api_request.py` & `yadisk-1.3.3/yadisk/api/api_request.py`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/yadisk/api/auth.py` & `yadisk-1.3.3/yadisk/api/auth.py`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/yadisk/api/disk.py` & `yadisk-1.3.3/yadisk/api/disk.py`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/yadisk/api/operations.py` & `yadisk-1.3.3/yadisk/api/operations.py`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/yadisk/api/resources.py` & `yadisk-1.3.3/yadisk/api/resources.py`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/yadisk/common.py` & `yadisk-1.3.3/yadisk/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,21 +75,23 @@
     if url.startswith("https://cloud-api.yandex.net/v1/disk/public/resources?"):
         return True
 
     # Check also for HTTP version
     return url.startswith("http://cloud-api.yandex.net/v1/disk/public/resources?")
 
 def ensure_path_has_schema(path: str, default_schema: str = "disk") -> str:
-    # Modifies path to always have a schema (disk:/ or trash:/).
+    # Modifies path to always have a schema (disk:/, trash:/ or app:/).
     # Without the schema Yandex.Disk won't let you upload filenames with the ':' character.
     # See https://github.com/ivknv/yadisk/issues/26 for more details
 
-    if path in ("disk:", "trash:"):
-        return default_schema + ":/" + path
+    KNOWN_SCHEMAS = ("disk:", "trash:", "app:")
 
-    if path.startswith("disk:/") or path.startswith("trash:/"):
-        return path
+    if path in KNOWN_SCHEMAS:
+        return default_schema + ":/" + path
 
     if path.startswith("/"):
         return default_schema + ":" + path
 
+    if any(path.startswith(schema + "/") for schema in KNOWN_SCHEMAS):
+        return path
+
     return default_schema + ":/" + path
```

### Comparing `yadisk-1.3.2/yadisk/exceptions.py` & `yadisk-1.3.3/yadisk/exceptions.py`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/yadisk/objects/auth.py` & `yadisk-1.3.3/yadisk/objects/auth.py`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/yadisk/objects/disk.py` & `yadisk-1.3.3/yadisk/objects/disk.py`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/yadisk/objects/error_object.py` & `yadisk-1.3.3/yadisk/objects/error_object.py`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/yadisk/objects/operations.py` & `yadisk-1.3.3/yadisk/objects/operations.py`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/yadisk/objects/resources.py` & `yadisk-1.3.3/yadisk/objects/resources.py`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/yadisk/objects/yadisk_object.py` & `yadisk-1.3.3/yadisk/objects/yadisk_object.py`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/yadisk/settings.py` & `yadisk-1.3.3/yadisk/settings.py`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/yadisk/utils.py` & `yadisk-1.3.3/yadisk/utils.py`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/yadisk/yadisk.py` & `yadisk-1.3.3/yadisk/yadisk.py`

 * *Files identical despite different names*

### Comparing `yadisk-1.3.2/yadisk.egg-info/PKG-INFO` & `yadisk-1.3.3/yadisk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yadisk
-Version: 1.3.2
+Version: 1.3.3
 Summary: Библиотека-клиент REST API Яндекс.Диска / Yandex.Disk REST API client library
 Home-page: https://github.com/ivknv/yadisk
 Author: Ivan Konovalov
 Author-email: ivknv0@gmail.com
 License: LGPLv3
 Project-URL: Source code, https://github.com/ivknv/yadisk
 Project-URL: Documentation (EN), https://yadisk.readthedocs.io/en/latest
@@ -102,14 +102,18 @@
 .. _issue #4: https://github.com/ivknv/yadisk/issues/4
 .. _issue #7: https://github.com/ivknv/yadisk/issues/7
 .. _issue #23: https://github.com/ivknv/yadisk/issues/23
 .. _issue #26: https://github.com/ivknv/yadisk/issues/26
 .. _issue #28: https://github.com/ivknv/yadisk/issues/28
 .. _issue #29: https://github.com/ivknv/yadisk/issues/29
 
+* **Release 1.3.3 (2023-04-22)**
+
+  * Пути вида :code:`app:/` теперь работают правильно (см. `issue #26`_)
+
 * **Release 1.3.2 (2023-03-20)**
 
   * Исправлено `issue #29`_: TypeError: 'type' object is not subscriptable
 
 * **Release 1.3.1 (2023-02-28)**
 
   * Исправлено `issue #28`_: :code:`TypeError` при вызове :code:`download_public()` с параметром :code:`path`
```

### Comparing `yadisk-1.3.2/yadisk.egg-info/SOURCES.txt` & `yadisk-1.3.3/yadisk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

