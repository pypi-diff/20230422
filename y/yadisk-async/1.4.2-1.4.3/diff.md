# Comparing `tmp/yadisk-async-1.4.2.tar.gz` & `tmp/yadisk-async-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yadisk-async-1.4.2.tar", last modified: Mon Mar 20 12:45:48 2023, max compression
+gzip compressed data, was "yadisk-async-1.4.3.tar", last modified: Sat Apr 22 10:21:31 2023, max compression
```

## Comparing `yadisk-async-1.4.2.tar` & `yadisk-async-1.4.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-03-20 12:45:48.183045 yadisk-async-1.4.2/
--rw-r--r--   0 ivan      (1000) ivan      (1000)    35147 2019-07-04 16:39:24.000000 yadisk-async-1.4.2/COPYING
--rw-r--r--   0 ivan      (1000) ivan      (1000)     7649 2019-07-04 16:39:24.000000 yadisk-async-1.4.2/COPYING.lesser
--rw-r--r--   0 ivan      (1000) ivan      (1000)      132 2023-01-30 14:53:45.000000 yadisk-async-1.4.2/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)    14931 2023-03-20 12:45:48.183045 yadisk-async-1.4.2/PKG-INFO
--rw-r--r--   0 ivan      (1000) ivan      (1000)    10610 2023-03-20 12:37:45.000000 yadisk-async-1.4.2/README.en.rst
--rw-r--r--   0 ivan      (1000) ivan      (1000)    13597 2023-03-20 12:37:37.000000 yadisk-async-1.4.2/README.rst
--rw-r--r--   0 ivan      (1000) ivan      (1000)    13599 2023-03-20 12:36:12.000000 yadisk-async-1.4.2/README.ru.rst
--rw-r--r--   0 ivan      (1000) ivan      (1000)       38 2023-03-20 12:45:48.183045 yadisk-async-1.4.2/setup.cfg
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1819 2023-03-20 12:18:58.000000 yadisk-async-1.4.2/setup.py
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-03-20 12:45:48.180045 yadisk-async-1.4.2/yadisk_async/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      121 2023-03-20 12:19:06.000000 yadisk-async-1.4.2/yadisk_async/__init__.py
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-03-20 12:45:48.181044 yadisk-async-1.4.2/yadisk_async/api/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      177 2019-07-04 16:39:24.000000 yadisk-async-1.4.2/yadisk_async/api/__init__.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     4966 2023-01-30 14:53:45.000000 yadisk-async-1.4.2/yadisk_async/api/api_request.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     4973 2023-01-30 14:53:45.000000 yadisk-async-1.4.2/yadisk_async/api/auth.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1221 2023-01-30 14:53:45.000000 yadisk-async-1.4.2/yadisk_async/api/disk.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     2005 2023-01-30 14:53:45.000000 yadisk-async-1.4.2/yadisk_async/api/operations.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)    44431 2023-01-30 14:53:45.000000 yadisk-async-1.4.2/yadisk_async/api/resources.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     5214 2023-03-20 12:30:27.000000 yadisk-async-1.4.2/yadisk_async/common.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      739 2023-01-30 14:53:45.000000 yadisk-async-1.4.2/yadisk_async/compat.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     4754 2023-01-30 14:53:45.000000 yadisk-async-1.4.2/yadisk_async/exceptions.py
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-03-20 12:45:48.182045 yadisk-async-1.4.2/yadisk_async/objects/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      207 2019-07-04 16:39:24.000000 yadisk-async-1.4.2/yadisk_async/objects/__init__.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1722 2023-01-30 14:53:45.000000 yadisk-async-1.4.2/yadisk_async/objects/auth.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     6780 2023-01-30 14:53:45.000000 yadisk-async-1.4.2/yadisk_async/objects/disk.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      692 2019-07-04 16:39:24.000000 yadisk-async-1.4.2/yadisk_async/objects/error_object.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1293 2023-01-30 14:53:45.000000 yadisk-async-1.4.2/yadisk_async/objects/operations.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)    72830 2023-02-28 14:33:26.000000 yadisk-async-1.4.2/yadisk_async/objects/resources.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     4082 2023-01-30 14:53:45.000000 yadisk-async-1.4.2/yadisk_async/objects/yadisk_object.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)        0 2023-01-30 14:53:45.000000 yadisk-async-1.4.2/yadisk_async/py.typed
--rw-r--r--   0 ivan      (1000) ivan      (1000)      821 2021-07-10 09:57:54.000000 yadisk-async-1.4.2/yadisk_async/session.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      711 2019-07-05 16:26:08.000000 yadisk-async-1.4.2/yadisk_async/settings.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     4023 2023-01-30 14:53:45.000000 yadisk-async-1.4.2/yadisk_async/utils.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)    76122 2023-03-20 12:16:44.000000 yadisk-async-1.4.2/yadisk_async/yadisk.py
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-03-20 12:45:48.181044 yadisk-async-1.4.2/yadisk_async.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)    14931 2023-03-20 12:45:48.000000 yadisk-async-1.4.2/yadisk_async.egg-info/PKG-INFO
--rw-r--r--   0 ivan      (1000) ivan      (1000)      882 2023-03-20 12:45:48.000000 yadisk-async-1.4.2/yadisk_async.egg-info/SOURCES.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)        1 2023-03-20 12:45:48.000000 yadisk-async-1.4.2/yadisk_async.egg-info/dependency_links.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)       17 2023-03-20 12:45:48.000000 yadisk-async-1.4.2/yadisk_async.egg-info/requires.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)       13 2023-03-20 12:45:48.000000 yadisk-async-1.4.2/yadisk_async.egg-info/top_level.txt
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-04-22 10:21:31.583838 yadisk-async-1.4.3/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    35147 2019-07-04 16:39:24.000000 yadisk-async-1.4.3/COPYING
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     7649 2019-07-04 16:39:24.000000 yadisk-async-1.4.3/COPYING.lesser
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      132 2023-01-30 14:53:45.000000 yadisk-async-1.4.3/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    15072 2023-04-22 10:21:31.582837 yadisk-async-1.4.3/PKG-INFO
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    10707 2023-04-22 10:21:08.000000 yadisk-async-1.4.3/README.en.rst
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    13738 2023-04-22 10:21:08.000000 yadisk-async-1.4.3/README.rst
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    13738 2023-04-22 10:21:08.000000 yadisk-async-1.4.3/README.ru.rst
+-rw-r--r--   0 ivan      (1000) ivan      (1000)       38 2023-04-22 10:21:31.583838 yadisk-async-1.4.3/setup.cfg
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1819 2023-04-22 10:21:08.000000 yadisk-async-1.4.3/setup.py
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-04-22 10:21:31.580838 yadisk-async-1.4.3/yadisk_async/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      121 2023-04-22 10:21:08.000000 yadisk-async-1.4.3/yadisk_async/__init__.py
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-04-22 10:21:31.581838 yadisk-async-1.4.3/yadisk_async/api/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      177 2019-07-04 16:39:24.000000 yadisk-async-1.4.3/yadisk_async/api/__init__.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     4966 2023-01-30 14:53:45.000000 yadisk-async-1.4.3/yadisk_async/api/api_request.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     4973 2023-01-30 14:53:45.000000 yadisk-async-1.4.3/yadisk_async/api/auth.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1221 2023-01-30 14:53:45.000000 yadisk-async-1.4.3/yadisk_async/api/disk.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     2005 2023-01-30 14:53:45.000000 yadisk-async-1.4.3/yadisk_async/api/operations.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    44431 2023-01-30 14:53:45.000000 yadisk-async-1.4.3/yadisk_async/api/resources.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     5271 2023-04-22 10:21:08.000000 yadisk-async-1.4.3/yadisk_async/common.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      739 2023-01-30 14:53:45.000000 yadisk-async-1.4.3/yadisk_async/compat.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     4754 2023-01-30 14:53:45.000000 yadisk-async-1.4.3/yadisk_async/exceptions.py
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-04-22 10:21:31.582837 yadisk-async-1.4.3/yadisk_async/objects/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      207 2019-07-04 16:39:24.000000 yadisk-async-1.4.3/yadisk_async/objects/__init__.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1722 2023-01-30 14:53:45.000000 yadisk-async-1.4.3/yadisk_async/objects/auth.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     6780 2023-01-30 14:53:45.000000 yadisk-async-1.4.3/yadisk_async/objects/disk.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      692 2019-07-04 16:39:24.000000 yadisk-async-1.4.3/yadisk_async/objects/error_object.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1293 2023-01-30 14:53:45.000000 yadisk-async-1.4.3/yadisk_async/objects/operations.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    72830 2023-02-28 14:33:26.000000 yadisk-async-1.4.3/yadisk_async/objects/resources.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     4082 2023-01-30 14:53:45.000000 yadisk-async-1.4.3/yadisk_async/objects/yadisk_object.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)        0 2023-01-30 14:53:45.000000 yadisk-async-1.4.3/yadisk_async/py.typed
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      821 2021-07-10 09:57:54.000000 yadisk-async-1.4.3/yadisk_async/session.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      711 2019-07-05 16:26:08.000000 yadisk-async-1.4.3/yadisk_async/settings.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     4023 2023-01-30 14:53:45.000000 yadisk-async-1.4.3/yadisk_async/utils.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    76122 2023-03-20 12:47:32.000000 yadisk-async-1.4.3/yadisk_async/yadisk.py
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-04-22 10:21:31.580838 yadisk-async-1.4.3/yadisk_async.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)    15072 2023-04-22 10:21:31.000000 yadisk-async-1.4.3/yadisk_async.egg-info/PKG-INFO
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      882 2023-04-22 10:21:31.000000 yadisk-async-1.4.3/yadisk_async.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)        1 2023-04-22 10:21:31.000000 yadisk-async-1.4.3/yadisk_async.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)       17 2023-04-22 10:21:31.000000 yadisk-async-1.4.3/yadisk_async.egg-info/requires.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)       13 2023-04-22 10:21:31.000000 yadisk-async-1.4.3/yadisk_async.egg-info/top_level.txt
```

### Comparing `yadisk-async-1.4.2/COPYING` & `yadisk-async-1.4.3/COPYING`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/COPYING.lesser` & `yadisk-async-1.4.3/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/PKG-INFO` & `yadisk-async-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yadisk-async
-Version: 1.4.2
+Version: 1.4.3
 Summary: Библиотека-клиент REST API Яндекс.Диска с поддержкой async/await / Yandex.Disk REST API client library with async/await support
 Home-page: https://github.com/ivknv/yadisk-async
 Author: Ivan Konovalov
 Author-email: ivknv0@gmail.com
 License: LGPLv3
 Project-URL: Source code, https://github.com/ivknv/yadisk-async
 Project-URL: Documentation (EN), https://yadisk-async.readthedocs.io/en/latest
@@ -114,14 +114,18 @@
 .. _PR #1: https://github.com/ivknv/yadisk-async/pull/1
 .. _issue #23: https://github.com/ivknv/yadisk/issues/23
 .. _PR #6: https://github.com/ivknv/yadisk-async/pull/6
 .. _issue #26: https://github.com/ivknv/yadisk/issues/26
 .. _issue #28: https://github.com/ivknv/yadisk/issues/28
 .. _issue #29: https://github.com/ivknv/yadisk/issues/29
 
+* **Release 1.4.3 (2023-04-22)**
+
+  * Пути вида :code:`app:/` теперь работают правильно (см. `issue #26`_)
+
 * **Release 1.4.2 (2023-03-20)**
 
   * Исправлено `issue #29`_: TypeError: 'type' object is not subscriptable
   * Исправлена ошибка (Python <3.9): TypeError: Too many parameters for typing.AsyncIterable; actual 2, expected 1
 
 * **Release 1.4.1 (2023-02-28)**
```

### Comparing `yadisk-async-1.4.2/README.en.rst` & `yadisk-async-1.4.3/README.en.rst`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,18 @@
 .. _PR #1: https://github.com/ivknv/yadisk-async/pull/1
 .. _issue #23: https://github.com/ivknv/yadisk/issues/23
 .. _PR #6: https://github.com/ivknv/yadisk-async/pull/6
 .. _issue #26: https://github.com/ivknv/yadisk/issues/26
 .. _issue #28: https://github.com/ivknv/yadisk/issues/28
 .. _issue #29: https://github.com/ivknv/yadisk/issues/29
 
+* **Release 1.4.3 (2023-04-22)**
+
+  * :code:`app:/` paths now work correctly (see `issue #26`_)
+
 * **Release 1.4.2 (2023-03-20)**
 
   * Fixed `issue #29`_: TypeError: 'type' object is not subscriptable
   * Fixed a bug affecting Python <3.9: TypeError: Too many parameters for typing.AsyncIterable; actual 2, expected 1
 
 * **Release 1.4.1 (2023-02-28)**
```

### Comparing `yadisk-async-1.4.2/README.rst` & `yadisk-async-1.4.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,18 @@
 .. _PR #1: https://github.com/ivknv/yadisk-async/pull/1
 .. _issue #23: https://github.com/ivknv/yadisk/issues/23
 .. _PR #6: https://github.com/ivknv/yadisk-async/pull/6
 .. _issue #26: https://github.com/ivknv/yadisk/issues/26
 .. _issue #28: https://github.com/ivknv/yadisk/issues/28
 .. _issue #29: https://github.com/ivknv/yadisk/issues/29
 
+* **Release 1.4.3 (2023-04-22)**
+
+  * Пути вида :code:`app:/` теперь работают правильно (см. `issue #26`_)
+
 * **Release 1.4.2 (2023-03-20)**
 
   * Исправлено `issue #29`_: TypeError: 'type' object is not subscriptable
   * Исправлена ошибка (Python <3.9): TypeError: Too many parameters for typing.AsyncIterable; actual 2, expected 1
 
 * **Release 1.4.1 (2023-02-28)**
```

### Comparing `yadisk-async-1.4.2/README.ru.rst` & `yadisk-async-1.4.3/README.ru.rst`

 * *Files 2% similar despite different names*

```diff
@@ -87,18 +87,22 @@
 .. _PR #1: https://github.com/ivknv/yadisk-async/pull/1
 .. _issue #23: https://github.com/ivknv/yadisk/issues/23
 .. _PR #6: https://github.com/ivknv/yadisk-async/pull/6
 .. _issue #26: https://github.com/ivknv/yadisk/issues/26
 .. _issue #28: https://github.com/ivknv/yadisk/issues/28
 .. _issue #29: https://github.com/ivknv/yadisk/issues/29
 
+* **Release 1.4.3 (2023-04-22)**
+
+  * Пути вида :code:`app:/` теперь работают правильно (см. `issue #26`_)
+
 * **Release 1.4.2 (2023-03-20)**
 
   * Исправлено `issue #29`_: TypeError: 'type' object is not subscriptable
-  * Исправлена ошибка (Python <3.9): `TypeError: Too many parameters for typing.AsyncIterable; actual 2, expected 1`
+  * Исправлена ошибка (Python <3.9): TypeError: Too many parameters for typing.AsyncIterable; actual 2, expected 1
 
 * **Release 1.4.1 (2023-02-28)**
 
   * Исправлено `issue #28`_: :code:`TypeError` при вызове :code:`download_public()` с параметром :code:`path`
   * Исправлено :code:`AttributeError` при вызове :code:`ResourceLinkObject.public_listdir()`
 
 * **Release 1.4.0 (2023-01-30)**
```

### Comparing `yadisk-async-1.4.2/setup.py` & `yadisk-async-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 module_dir = os.path.dirname(__file__)
 
 with codecs.open(os.path.join(module_dir, "README.rst"), encoding="utf8") as f:
     long_description = f.read()
 
 setup(name="yadisk-async",
-      version="1.4.2",
+      version="1.4.3",
       packages=find_packages(exclude=("tests",)),
       description="Библиотека-клиент REST API Яндекс.Диска с поддержкой async/await / Yandex.Disk REST API client library with async/await support",
       long_description=long_description,
       author="Ivan Konovalov",
       author_email="ivknv0@gmail.com",
       license="LGPLv3",
       python_requires=">=3.8",
```

### Comparing `yadisk-async-1.4.2/yadisk_async/api/api_request.py` & `yadisk-async-1.4.3/yadisk_async/api/api_request.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/api/auth.py` & `yadisk-async-1.4.3/yadisk_async/api/auth.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/api/disk.py` & `yadisk-async-1.4.3/yadisk_async/api/disk.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/api/operations.py` & `yadisk-async-1.4.3/yadisk_async/api/operations.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/api/resources.py` & `yadisk-async-1.4.3/yadisk_async/api/resources.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/common.py` & `yadisk-async-1.4.3/yadisk_async/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,27 +76,29 @@
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
 
 class AsyncFileLike(Protocol):
     async def read(self, size: int = ..., /) -> Union[str, bytes]: ...
     async def write(self, buffer: Any, /) -> int: ...
     async def seek(self, pos: int, whence: int = ..., /) -> int: ...
     async def tell(self) -> int: ...
```

### Comparing `yadisk-async-1.4.2/yadisk_async/compat.py` & `yadisk-async-1.4.3/yadisk_async/compat.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/exceptions.py` & `yadisk-async-1.4.3/yadisk_async/exceptions.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/objects/auth.py` & `yadisk-async-1.4.3/yadisk_async/objects/auth.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/objects/disk.py` & `yadisk-async-1.4.3/yadisk_async/objects/disk.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/objects/error_object.py` & `yadisk-async-1.4.3/yadisk_async/objects/error_object.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/objects/operations.py` & `yadisk-async-1.4.3/yadisk_async/objects/operations.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/objects/resources.py` & `yadisk-async-1.4.3/yadisk_async/objects/resources.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/objects/yadisk_object.py` & `yadisk-async-1.4.3/yadisk_async/objects/yadisk_object.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/session.py` & `yadisk-async-1.4.3/yadisk_async/session.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/settings.py` & `yadisk-async-1.4.3/yadisk_async/settings.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/utils.py` & `yadisk-async-1.4.3/yadisk_async/utils.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async/yadisk.py` & `yadisk-async-1.4.3/yadisk_async/yadisk.py`

 * *Files identical despite different names*

### Comparing `yadisk-async-1.4.2/yadisk_async.egg-info/PKG-INFO` & `yadisk-async-1.4.3/yadisk_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yadisk-async
-Version: 1.4.2
+Version: 1.4.3
 Summary: Библиотека-клиент REST API Яндекс.Диска с поддержкой async/await / Yandex.Disk REST API client library with async/await support
 Home-page: https://github.com/ivknv/yadisk-async
 Author: Ivan Konovalov
 Author-email: ivknv0@gmail.com
 License: LGPLv3
 Project-URL: Source code, https://github.com/ivknv/yadisk-async
 Project-URL: Documentation (EN), https://yadisk-async.readthedocs.io/en/latest
@@ -114,14 +114,18 @@
 .. _PR #1: https://github.com/ivknv/yadisk-async/pull/1
 .. _issue #23: https://github.com/ivknv/yadisk/issues/23
 .. _PR #6: https://github.com/ivknv/yadisk-async/pull/6
 .. _issue #26: https://github.com/ivknv/yadisk/issues/26
 .. _issue #28: https://github.com/ivknv/yadisk/issues/28
 .. _issue #29: https://github.com/ivknv/yadisk/issues/29
 
+* **Release 1.4.3 (2023-04-22)**
+
+  * Пути вида :code:`app:/` теперь работают правильно (см. `issue #26`_)
+
 * **Release 1.4.2 (2023-03-20)**
 
   * Исправлено `issue #29`_: TypeError: 'type' object is not subscriptable
   * Исправлена ошибка (Python <3.9): TypeError: Too many parameters for typing.AsyncIterable; actual 2, expected 1
 
 * **Release 1.4.1 (2023-02-28)**
```

### Comparing `yadisk-async-1.4.2/yadisk_async.egg-info/SOURCES.txt` & `yadisk-async-1.4.3/yadisk_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

