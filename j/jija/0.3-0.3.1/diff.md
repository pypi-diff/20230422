# Comparing `tmp/jija-0.3.tar.gz` & `tmp/jija-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jija-0.3.tar", last modified: Sat Apr 22 10:51:19 2023, max compression
+gzip compressed data, was "jija-0.3.1.tar", last modified: Sat Apr 22 11:43:09 2023, max compression
```

## Comparing `jija-0.3.tar` & `jija-0.3.1.tar`

### file list

```diff
@@ -1,41 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:51:19.156313 jija-0.3/
--rw-r--r--   0 root         (0) root         (0)      256 2023-04-22 10:51:19.156313 jija-0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:51:19.146313 jija-0.3/jija/
--rwxr-xr-x   0 root         (0) root         (0)      308 2023-04-20 16:55:27.000000 jija-0.3/jija/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6316 2023-04-22 10:21:56.000000 jija-0.3/jija/app.py
--rwxr-xr-x   0 root         (0) root         (0)     4247 2023-04-20 22:18:05.000000 jija-0.3/jija/apps.py
--rwxr-xr-x   0 root         (0) root         (0)      513 2023-04-20 22:16:18.000000 jija-0.3/jija/collector.py
--rwxr-xr-x   0 root         (0) root         (0)      456 2022-11-19 22:00:09.000000 jija-0.3/jija/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:51:19.156313 jija-0.3/jija/config/
--rwxr-xr-x   0 root         (0) root         (0)      136 2023-04-20 15:42:10.000000 jija-0.3/jija/config/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1162 2023-01-23 14:19:45.000000 jija-0.3/jija/config/base.py
--rwxr-xr-x   0 root         (0) root         (0)      685 2023-04-20 10:04:29.000000 jija-0.3/jija/config/dev.py
--rwxr-xr-x   0 root         (0) root         (0)      928 2023-04-20 15:19:31.000000 jija-0.3/jija/config/drivers.py
--rwxr-xr-x   0 root         (0) root         (0)      290 2023-04-20 13:46:57.000000 jija-0.3/jija/config/network.py
--rwxr-xr-x   0 root         (0) root         (0)     1280 2023-04-20 13:50:19.000000 jija-0.3/jija/config/structute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:51:19.156313 jija-0.3/jija/drivers/
--rwxr-xr-x   0 root         (0) root         (0)       90 2023-04-20 14:55:05.000000 jija-0.3/jija/drivers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      163 2023-04-20 15:18:55.000000 jija-0.3/jija/drivers/base.py
--rwxr-xr-x   0 root         (0) root         (0)      270 2023-04-20 15:29:36.000000 jija-0.3/jija/drivers/database.py
--rwxr-xr-x   0 root         (0) root         (0)       72 2023-04-20 14:28:01.000000 jija-0.3/jija/drivers/docs.py
--rwxr-xr-x   0 root         (0) root         (0)      171 2023-01-22 17:43:04.000000 jija-0.3/jija/exceptions.py
--rwxr-xr-x   0 root         (0) root         (0)      270 2023-01-22 17:43:04.000000 jija-0.3/jija/middleware.py
--rwxr-xr-x   0 root         (0) root         (0)     1829 2023-04-20 10:04:29.000000 jija-0.3/jija/reloader.py
--rwxr-xr-x   0 root         (0) root         (0)     1370 2023-01-22 17:43:04.000000 jija-0.3/jija/response.py
--rwxr-xr-x   0 root         (0) root         (0)     2281 2023-04-20 21:45:15.000000 jija-0.3/jija/router.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:51:19.156313 jija-0.3/jija/serializers/
--rwxr-xr-x   0 root         (0) root         (0)      138 2023-01-22 17:43:04.000000 jija-0.3/jija/serializers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      310 2023-01-22 17:43:04.000000 jija-0.3/jija/serializers/exceptions.py
--rwxr-xr-x   0 root         (0) root         (0)     3305 2023-04-20 13:50:19.000000 jija-0.3/jija/serializers/fields.py
--rwxr-xr-x   0 root         (0) root         (0)     1283 2023-04-20 11:10:56.000000 jija-0.3/jija/serializers/serializer.py
--rwxr-xr-x   0 root         (0) root         (0)     3220 2023-04-20 13:50:19.000000 jija-0.3/jija/serializers/validators.py
--rwxr-xr-x   0 root         (0) root         (0)     6044 2023-04-20 14:13:13.000000 jija-0.3/jija/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:51:19.156313 jija-0.3/jija.egg-info/
--rw-r--r--   0 root         (0) root         (0)      256 2023-04-22 10:51:19.000000 jija-0.3/jija.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      726 2023-04-22 10:51:19.000000 jija-0.3/jija.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 10:51:19.000000 jija-0.3/jija.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 10:51:19.000000 jija-0.3/jija.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       83 2023-04-22 10:51:19.000000 jija-0.3/jija.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-22 10:51:19.000000 jija-0.3/jija.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 10:51:19.156313 jija-0.3/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      522 2023-04-22 10:51:00.000000 jija-0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-22 11:43:09.187370 jija-0.3.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/
+-rwxr-xr-x   0 root         (0) root         (0)      308 2023-04-20 16:55:27.000000 jija-0.3.1/jija/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6316 2023-04-22 10:21:56.000000 jija-0.3.1/jija/app.py
+-rwxr-xr-x   0 root         (0) root         (0)     4247 2023-04-20 22:18:05.000000 jija-0.3.1/jija/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/base_app/
+-rwxr-xr-x   0 root         (0) root         (0)      198 2023-04-20 21:51:13.000000 jija-0.3.1/jija/base_app/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/base_app/commands/
+-rwxr-xr-x   0 root         (0) root         (0)      165 2023-04-20 15:29:36.000000 jija-0.3.1/jija/base_app/commands/migrate.py
+-rwxr-xr-x   0 root         (0) root         (0)     1366 2023-04-18 13:14:24.000000 jija-0.3.1/jija/base_app/commands/run.py
+-rwxr-xr-x   0 root         (0) root         (0)      299 2023-02-26 05:34:17.000000 jija-0.3.1/jija/base_app/commands/runprocess.py
+-rwxr-xr-x   0 root         (0) root         (0)      163 2023-04-20 15:30:36.000000 jija-0.3.1/jija/base_app/commands/update.py
+-rwxr-xr-x   0 root         (0) root         (0)      966 2022-11-05 14:37:03.000000 jija-0.3.1/jija/base_app/middlewares.py
+-rwxr-xr-x   0 root         (0) root         (0)      513 2023-04-20 22:16:18.000000 jija-0.3.1/jija/collector.py
+-rwxr-xr-x   0 root         (0) root         (0)      456 2022-11-19 22:00:09.000000 jija-0.3.1/jija/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/config/
+-rwxr-xr-x   0 root         (0) root         (0)      136 2023-04-20 15:42:10.000000 jija-0.3.1/jija/config/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1162 2023-01-23 14:19:45.000000 jija-0.3.1/jija/config/base.py
+-rwxr-xr-x   0 root         (0) root         (0)      685 2023-04-20 10:04:29.000000 jija-0.3.1/jija/config/dev.py
+-rwxr-xr-x   0 root         (0) root         (0)      928 2023-04-20 15:19:31.000000 jija-0.3.1/jija/config/drivers.py
+-rwxr-xr-x   0 root         (0) root         (0)      290 2023-04-20 13:46:57.000000 jija-0.3.1/jija/config/network.py
+-rwxr-xr-x   0 root         (0) root         (0)     1280 2023-04-20 13:50:19.000000 jija-0.3.1/jija/config/structute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/contrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/contrib/auth/
+-rwxr-xr-x   0 root         (0) root         (0)      488 2023-04-20 13:48:49.000000 jija-0.3.1/jija/contrib/auth/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/contrib/jija_orm/
+-rwxr-xr-x   0 root         (0) root         (0)     2238 2023-04-22 11:38:34.000000 jija-0.3.1/jija/contrib/jija_orm/driver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/contrib/swagger/
+-rwxr-xr-x   0 root         (0) root         (0)     1481 2023-04-20 14:28:01.000000 jija-0.3.1/jija/contrib/swagger/driver.py
+-rwxr-xr-x   0 root         (0) root         (0)     4723 2023-04-20 14:10:00.000000 jija-0.3.1/jija/contrib/swagger/processor.py
+-rwxr-xr-x   0 root         (0) root         (0)      234 2023-04-20 14:05:10.000000 jija-0.3.1/jija/contrib/swagger/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/drivers/
+-rwxr-xr-x   0 root         (0) root         (0)       90 2023-04-20 14:55:05.000000 jija-0.3.1/jija/drivers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      163 2023-04-20 15:18:55.000000 jija-0.3.1/jija/drivers/base.py
+-rwxr-xr-x   0 root         (0) root         (0)      270 2023-04-20 15:29:36.000000 jija-0.3.1/jija/drivers/database.py
+-rwxr-xr-x   0 root         (0) root         (0)       72 2023-04-20 14:28:01.000000 jija-0.3.1/jija/drivers/docs.py
+-rwxr-xr-x   0 root         (0) root         (0)      171 2023-01-22 17:43:04.000000 jija-0.3.1/jija/exceptions.py
+-rwxr-xr-x   0 root         (0) root         (0)      270 2023-01-22 17:43:04.000000 jija-0.3.1/jija/middleware.py
+-rwxr-xr-x   0 root         (0) root         (0)     1829 2023-04-20 10:04:29.000000 jija-0.3.1/jija/reloader.py
+-rwxr-xr-x   0 root         (0) root         (0)     1370 2023-01-22 17:43:04.000000 jija-0.3.1/jija/response.py
+-rwxr-xr-x   0 root         (0) root         (0)     2281 2023-04-20 21:45:15.000000 jija-0.3.1/jija/router.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija/serializers/
+-rwxr-xr-x   0 root         (0) root         (0)      138 2023-01-22 17:43:04.000000 jija-0.3.1/jija/serializers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      310 2023-01-22 17:43:04.000000 jija-0.3.1/jija/serializers/exceptions.py
+-rwxr-xr-x   0 root         (0) root         (0)     3305 2023-04-20 13:50:19.000000 jija-0.3.1/jija/serializers/fields.py
+-rwxr-xr-x   0 root         (0) root         (0)     1283 2023-04-20 11:10:56.000000 jija-0.3.1/jija/serializers/serializer.py
+-rwxr-xr-x   0 root         (0) root         (0)     3220 2023-04-20 13:50:19.000000 jija-0.3.1/jija/serializers/validators.py
+-rwxr-xr-x   0 root         (0) root         (0)     6044 2023-04-20 14:13:13.000000 jija-0.3.1/jija/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:43:09.187370 jija-0.3.1/jija.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-22 11:43:09.000000 jija-0.3.1/jija.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-04-22 11:43:09.000000 jija-0.3.1/jija.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 11:43:09.000000 jija-0.3.1/jija.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 11:43:09.000000 jija-0.3.1/jija.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-22 11:43:09.000000 jija-0.3.1/jija.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-22 11:43:09.000000 jija-0.3.1/jija.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 11:43:09.187370 jija-0.3.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      718 2023-04-22 11:43:07.000000 jija-0.3.1/setup.py
```

### Comparing `jija-0.3/jija/app.py` & `jija-0.3.1/jija/app.py`

 * *Files identical despite different names*

### Comparing `jija-0.3/jija/apps.py` & `jija-0.3.1/jija/apps.py`

 * *Files identical despite different names*

### Comparing `jija-0.3/jija/collector.py` & `jija-0.3.1/jija/collector.py`

 * *Files identical despite different names*

### Comparing `jija-0.3/jija/config/base.py` & `jija-0.3.1/jija/config/base.py`

 * *Files identical despite different names*

### Comparing `jija-0.3/jija/config/dev.py` & `jija-0.3.1/jija/config/dev.py`

 * *Files identical despite different names*

### Comparing `jija-0.3/jija/config/drivers.py` & `jija-0.3.1/jija/config/drivers.py`

 * *Files identical despite different names*

### Comparing `jija-0.3/jija/config/structute.py` & `jija-0.3.1/jija/config/structute.py`

 * *Files identical despite different names*

### Comparing `jija-0.3/jija/reloader.py` & `jija-0.3.1/jija/reloader.py`

 * *Files identical despite different names*

### Comparing `jija-0.3/jija/response.py` & `jija-0.3.1/jija/response.py`

 * *Files identical despite different names*

### Comparing `jija-0.3/jija/router.py` & `jija-0.3.1/jija/router.py`

 * *Files identical despite different names*

### Comparing `jija-0.3/jija/serializers/fields.py` & `jija-0.3.1/jija/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `jija-0.3/jija/serializers/serializer.py` & `jija-0.3.1/jija/serializers/serializer.py`

 * *Files identical despite different names*

### Comparing `jija-0.3/jija/serializers/validators.py` & `jija-0.3.1/jija/serializers/validators.py`

 * *Files identical despite different names*

### Comparing `jija-0.3/jija/views.py` & `jija-0.3.1/jija/views.py`

 * *Files identical despite different names*

