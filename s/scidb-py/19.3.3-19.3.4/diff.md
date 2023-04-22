# Comparing `tmp/scidb-py-19.3.3.tar.gz` & `tmp/scidb-py-19.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scidb-py-19.3.3.tar", last modified: Fri Mar 13 18:33:22 2020, max compression
+gzip compressed data, was "dist/scidb-py-19.3.4.tar", last modified: Fri Aug 21 17:17:23 2020, max compression
```

## Comparing `scidb-py-19.3.3.tar` & `scidb-py-19.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx------   0 rares     (1000) rares     (1000)        0 2020-03-13 18:33:22.000000 scidb-py-19.3.3/
--rw-------   0 rares     (1000) rares     (1000)     4343 2020-03-13 18:33:22.000000 scidb-py-19.3.3/PKG-INFO
--rw-------   0 rares     (1000) rares     (1000)     2726 2019-06-01 02:16:02.000000 scidb-py-19.3.3/README.rst
-drwx------   0 rares     (1000) rares     (1000)        0 2020-03-13 18:33:22.000000 scidb-py-19.3.3/scidb_py.egg-info/
--rw-------   0 rares     (1000) rares     (1000)     4343 2020-03-13 18:33:22.000000 scidb-py-19.3.3/scidb_py.egg-info/PKG-INFO
--rw-------   0 rares     (1000) rares     (1000)      256 2020-03-13 18:33:22.000000 scidb-py-19.3.3/scidb_py.egg-info/SOURCES.txt
--rw-------   0 rares     (1000) rares     (1000)        1 2020-03-13 18:33:22.000000 scidb-py-19.3.3/scidb_py.egg-info/dependency_links.txt
--rw-------   0 rares     (1000) rares     (1000)      144 2020-03-13 18:33:22.000000 scidb-py-19.3.3/scidb_py.egg-info/requires.txt
--rw-------   0 rares     (1000) rares     (1000)        8 2020-03-13 18:33:22.000000 scidb-py-19.3.3/scidb_py.egg-info/top_level.txt
-drwx------   0 rares     (1000) rares     (1000)        0 2020-03-13 18:33:22.000000 scidb-py-19.3.3/scidbpy/
--rw-------   0 rares     (1000) rares     (1000)    26336 2020-03-13 18:21:15.000000 scidb-py-19.3.3/scidbpy/__init__.py
--rw-------   0 rares     (1000) rares     (1000)    31554 2020-03-11 23:32:46.000000 scidb-py-19.3.3/scidbpy/db.py
--rw-------   0 rares     (1000) rares     (1000)     2620 2018-02-03 05:26:53.000000 scidb-py-19.3.3/scidbpy/meta.py
--rw-------   0 rares     (1000) rares     (1000)    26728 2019-06-01 02:15:40.000000 scidb-py-19.3.3/scidbpy/schema.py
--rw-------   0 rares     (1000) rares     (1000)       67 2020-03-13 18:33:22.000000 scidb-py-19.3.3/setup.cfg
--rw-------   0 rares     (1000) rares     (1000)     1505 2019-07-08 02:29:08.000000 scidb-py-19.3.3/setup.py
+drwx------   0 vernica  (21736907) users      (100)        0 2020-08-21 17:17:23.654081 scidb-py-19.3.4/
+-rw-------   0 vernica  (21736907) users      (100)     4343 2020-08-21 17:17:23.654081 scidb-py-19.3.4/PKG-INFO
+-rw-------   0 vernica  (21736907) users      (100)     2726 2020-08-21 16:45:41.000000 scidb-py-19.3.4/README.rst
+drwx------   0 vernica  (21736907) users      (100)        0 2020-08-21 17:17:23.652081 scidb-py-19.3.4/scidb_py.egg-info/
+-rw-r--r--   0 vernica  (21736907) users      (100)     4343 2020-08-21 17:17:23.000000 scidb-py-19.3.4/scidb_py.egg-info/PKG-INFO
+-rw-r--r--   0 vernica  (21736907) users      (100)      256 2020-08-21 17:17:23.000000 scidb-py-19.3.4/scidb_py.egg-info/SOURCES.txt
+-rw-r--r--   0 vernica  (21736907) users      (100)        1 2020-08-21 17:17:23.000000 scidb-py-19.3.4/scidb_py.egg-info/dependency_links.txt
+-rw-r--r--   0 vernica  (21736907) users      (100)      144 2020-08-21 17:17:23.000000 scidb-py-19.3.4/scidb_py.egg-info/requires.txt
+-rw-r--r--   0 vernica  (21736907) users      (100)        8 2020-08-21 17:17:23.000000 scidb-py-19.3.4/scidb_py.egg-info/top_level.txt
+drwx------   0 vernica  (21736907) users      (100)        0 2020-08-21 17:17:23.654081 scidb-py-19.3.4/scidbpy/
+-rw-------   0 vernica  (21736907) users      (100)    26336 2020-08-21 17:02:57.000000 scidb-py-19.3.4/scidbpy/__init__.py
+-rw-------   0 vernica  (21736907) users      (100)    31776 2020-08-21 16:45:59.000000 scidb-py-19.3.4/scidbpy/db.py
+-rw-r--r--   0 vernica  (21736907) users      (100)     2620 2018-12-22 08:56:07.000000 scidb-py-19.3.4/scidbpy/meta.py
+-rw-------   0 vernica  (21736907) users      (100)    26728 2020-08-21 16:45:41.000000 scidb-py-19.3.4/scidbpy/schema.py
+-rw-r--r--   0 vernica  (21736907) users      (100)       67 2020-08-21 17:17:23.655081 scidb-py-19.3.4/setup.cfg
+-rw-------   0 vernica  (21736907) users      (100)     1505 2020-08-21 16:45:41.000000 scidb-py-19.3.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scidb-py-19.3.3/PKG-INFO` & `scidb-py-19.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scidb-py
-Version: 19.3.3
+Version: 19.3.4
 Summary: Python library for SciDB
 Home-page: UNKNOWN
 Author: Rares Vernica
 Author-email: rvernica@gmail.com
 License: AGPL-3.0
 Download-URL: http://github.com/Paradigm4/SciDB-Py
 Description: SciDB-Py: Python Interface to SciDB
```

### Comparing `scidb-py-19.3.3/README.rst` & `scidb-py-19.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `scidb-py-19.3.3/scidb_py.egg-info/PKG-INFO` & `scidb-py-19.3.4/scidb_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scidb-py
-Version: 19.3.3
+Version: 19.3.4
 Summary: Python library for SciDB
 Home-page: UNKNOWN
 Author: Rares Vernica
 Author-email: rvernica@gmail.com
 License: AGPL-3.0
 Download-URL: http://github.com/Paradigm4/SciDB-Py
 Description: SciDB-Py: Python Interface to SciDB
```

### Comparing `scidb-py-19.3.3/scidbpy/__init__.py` & `scidb-py-19.3.4/scidbpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1036,8 +1036,8 @@
 no_ops            = False
 
 """
 
 from .db import connect, iquery, Array
 from .schema import Attribute, Dimension, Schema
 
-__version__ = '19.3.3'
+__version__ = '19.3.4'
```

### Comparing `scidb-py-19.3.3/scidbpy/db.py` & `scidb-py-19.3.4/scidbpy/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     url = requests.compat.urljoin(scidb_url, Shim.release_session.value)
     req = requests.get(
         url,
         params={'id': id},
         auth=http_auth,
         verify=verify)
     req.reason = req.content
+    req.url = _sanitize_url(req.url)
     req.raise_for_status()
 
 
 class DB(object):
     """SciDB Shim connection object.
 
     >>> DB()
@@ -553,14 +554,15 @@
                     auth=self._http_auth,
                     verify=self.verify)
             except KeyboardInterrupt as e:
                 self._cleanup(endpoint)
                 raise e
 
         req.reason = req.content
+        req.url = _sanitize_url(req.url)
         try:
             req.raise_for_status()
         except Exception as e:
             self._cleanup(endpoint)
             raise e
         return req
 
@@ -889,14 +891,21 @@
     def schema(self):
         if self.is_lazy:
             return Schema.fromstring(
                 self.db.iquery_readlines(
                     "show('{}', 'afl')".format(self))[0][0])
 
 
+_sanitize_url_re = re.compile('((user)|(password))=[^&]*(?=(&|$))')
+
+
+def _sanitize_url(url):
+    return _sanitize_url_re.sub('\\1=...', url)
+
+
 connect = DB
 iquery = DB.iquery
 
 
 if __name__ == "__main__":
     # logging.basicConfig(level=logging.DEBUG)
     import doctest
```

### Comparing `scidb-py-19.3.3/scidbpy/meta.py` & `scidb-py-19.3.4/scidbpy/meta.py`

 * *Files identical despite different names*

### Comparing `scidb-py-19.3.3/scidbpy/schema.py` & `scidb-py-19.3.4/scidbpy/schema.py`

 * *Files identical despite different names*

### Comparing `scidb-py-19.3.3/setup.py` & `scidb-py-19.3.4/setup.py`

 * *Files identical despite different names*

