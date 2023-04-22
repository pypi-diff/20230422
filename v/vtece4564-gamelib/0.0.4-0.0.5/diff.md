# Comparing `tmp/vtece4564-gamelib-0.0.4.tar.gz` & `tmp/vtece4564-gamelib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtece4564-gamelib-0.0.4.tar", last modified: Fri Apr 21 20:05:54 2023, max compression
+gzip compressed data, was "vtece4564-gamelib-0.0.5.tar", last modified: Sat Apr 22 19:24:53 2023, max compression
```

## Comparing `vtece4564-gamelib-0.0.4.tar` & `vtece4564-gamelib-0.0.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 20:05:54.923939 vtece4564-gamelib-0.0.4/
--rw-r--r--   0 ceharris   (501) staff       (20)      940 2023-04-21 20:05:54.924170 vtece4564-gamelib-0.0.4/PKG-INFO
--rw-r--r--   0 ceharris   (501) staff       (20)      435 2023-04-21 18:13:29.000000 vtece4564-gamelib-0.0.4/README.md
--rw-r--r--   0 ceharris   (501) staff       (20)       41 2023-04-21 18:22:43.000000 vtece4564-gamelib-0.0.4/pyproject.toml
--rw-r--r--   0 ceharris   (501) staff       (20)      737 2023-04-21 20:05:54.924896 vtece4564-gamelib-0.0.4/setup.cfg
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 20:05:54.907159 vtece4564-gamelib-0.0.4/src/
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 20:05:54.907252 vtece4564-gamelib-0.0.4/src/main/
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 20:05:54.908933 vtece4564-gamelib-0.0.4/src/main/python/
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 20:05:54.912862 vtece4564-gamelib-0.0.4/src/main/python/gameauth/
--rw-r--r--   0 ceharris   (501) staff       (20)      210 2023-04-20 13:57:00.000000 vtece4564-gamelib-0.0.4/src/main/python/gameauth/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     2004 2023-04-19 17:45:40.000000 vtece4564-gamelib-0.0.4/src/main/python/gameauth/__main__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1515 2023-04-19 17:39:08.000000 vtece4564-gamelib-0.0.4/src/main/python/gameauth/key_util.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1385 2023-04-19 17:39:08.000000 vtece4564-gamelib-0.0.4/src/main/python/gameauth/password.py
--rw-r--r--   0 ceharris   (501) staff       (20)      260 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.4/src/main/python/gameauth/token.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1861 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.4/src/main/python/gameauth/token_generator.py
--rw-r--r--   0 ceharris   (501) staff       (20)     2155 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.4/src/main/python/gameauth/token_validator.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 20:05:54.913236 vtece4564-gamelib-0.0.4/src/main/python/gamecomm/
--rw-r--r--   0 ceharris   (501) staff       (20)        0 2023-04-19 19:21:49.000000 vtece4564-gamelib-0.0.4/src/main/python/gamecomm/__init__.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 20:05:54.914988 vtece4564-gamelib-0.0.4/src/main/python/gamecomm/client/
--rw-r--r--   0 ceharris   (501) staff       (20)      188 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.4/src/main/python/gamecomm/client/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     4949 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.4/src/main/python/gamecomm/client/game_client.py
--rw-r--r--   0 ceharris   (501) staff       (20)      348 2023-04-20 10:13:04.000000 vtece4564-gamelib-0.0.4/src/main/python/gamecomm/client/game_connection.py
--rw-r--r--   0 ceharris   (501) staff       (20)     3914 2023-04-21 19:49:31.000000 vtece4564-gamelib-0.0.4/src/main/python/gamecomm/client/tcp_connection.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1596 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.4/src/main/python/gamecomm/client/ws_connection.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 20:05:54.916749 vtece4564-gamelib-0.0.4/src/main/python/gamecomm/server/
--rw-r--r--   0 ceharris   (501) staff       (20)      187 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.4/src/main/python/gamecomm/server/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     7178 2023-04-21 16:16:01.000000 vtece4564-gamelib-0.0.4/src/main/python/gamecomm/server/game_connection.py
--rw-r--r--   0 ceharris   (501) staff       (20)     3489 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.4/src/main/python/gamecomm/server/tcp_listener.py
--rw-r--r--   0 ceharris   (501) staff       (20)     3835 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.4/src/main/python/gamecomm/server/ws_listener.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 20:05:54.918408 vtece4564-gamelib-0.0.4/src/main/python/gamedb/
--rw-r--r--   0 ceharris   (501) staff       (20)      156 2023-04-19 10:45:29.000000 vtece4564-gamelib-0.0.4/src/main/python/gamedb/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)      884 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.4/src/main/python/gamedb/game_repository.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 20:05:54.919859 vtece4564-gamelib-0.0.4/src/main/python/gamedb/json/
--rw-r--r--   0 ceharris   (501) staff       (20)      130 2023-04-21 14:47:05.000000 vtece4564-gamelib-0.0.4/src/main/python/gamedb/json/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     2154 2023-04-21 19:23:56.000000 vtece4564-gamelib-0.0.4/src/main/python/gamedb/json/game_repository.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1473 2023-04-21 19:24:11.000000 vtece4564-gamelib-0.0.4/src/main/python/gamedb/json/json_db.py
--rw-r--r--   0 ceharris   (501) staff       (20)     2299 2023-04-21 19:28:13.000000 vtece4564-gamelib-0.0.4/src/main/python/gamedb/json/user_repository.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 20:05:54.921148 vtece4564-gamelib-0.0.4/src/main/python/gamedb/mongo/
--rw-r--r--   0 ceharris   (501) staff       (20)       98 2023-04-21 14:47:05.000000 vtece4564-gamelib-0.0.4/src/main/python/gamedb/mongo/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1936 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.4/src/main/python/gamedb/mongo/game_repository.py
--rw-r--r--   0 ceharris   (501) staff       (20)     2344 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.4/src/main/python/gamedb/mongo/user_repository.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1085 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.4/src/main/python/gamedb/user_repository.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 20:05:54.923525 vtece4564-gamelib-0.0.4/src/main/python/vtece4564_gamelib.egg-info/
--rw-r--r--   0 ceharris   (501) staff       (20)      940 2023-04-21 20:05:54.000000 vtece4564-gamelib-0.0.4/src/main/python/vtece4564_gamelib.egg-info/PKG-INFO
--rw-r--r--   0 ceharris   (501) staff       (20)     1485 2023-04-21 20:05:54.000000 vtece4564-gamelib-0.0.4/src/main/python/vtece4564_gamelib.egg-info/SOURCES.txt
--rw-r--r--   0 ceharris   (501) staff       (20)        1 2023-04-21 20:05:54.000000 vtece4564-gamelib-0.0.4/src/main/python/vtece4564_gamelib.egg-info/dependency_links.txt
--rw-r--r--   0 ceharris   (501) staff       (20)       38 2023-04-21 20:05:54.000000 vtece4564-gamelib-0.0.4/src/main/python/vtece4564_gamelib.egg-info/requires.txt
--rw-r--r--   0 ceharris   (501) staff       (20)       25 2023-04-21 20:05:54.000000 vtece4564-gamelib-0.0.4/src/main/python/vtece4564_gamelib.egg-info/top_level.txt
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 19:24:53.509199 vtece4564-gamelib-0.0.5/
+-rw-r--r--   0 ceharris   (501) staff       (20)     1262 2023-04-22 19:24:53.509395 vtece4564-gamelib-0.0.5/PKG-INFO
+-rw-r--r--   0 ceharris   (501) staff       (20)      757 2023-04-22 19:06:37.000000 vtece4564-gamelib-0.0.5/README.md
+-rw-r--r--   0 ceharris   (501) staff       (20)       41 2023-04-21 18:22:43.000000 vtece4564-gamelib-0.0.5/pyproject.toml
+-rw-r--r--   0 ceharris   (501) staff       (20)      737 2023-04-22 19:24:53.510448 vtece4564-gamelib-0.0.5/setup.cfg
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 19:24:53.487912 vtece4564-gamelib-0.0.5/src/
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 19:24:53.488041 vtece4564-gamelib-0.0.5/src/main/
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 19:24:53.489376 vtece4564-gamelib-0.0.5/src/main/python/
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 19:24:53.493451 vtece4564-gamelib-0.0.5/src/main/python/gameauth/
+-rw-r--r--   0 ceharris   (501) staff       (20)      210 2023-04-20 13:57:00.000000 vtece4564-gamelib-0.0.5/src/main/python/gameauth/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     2004 2023-04-19 17:45:40.000000 vtece4564-gamelib-0.0.5/src/main/python/gameauth/__main__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1515 2023-04-19 17:39:08.000000 vtece4564-gamelib-0.0.5/src/main/python/gameauth/key_util.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1285 2023-04-22 18:42:22.000000 vtece4564-gamelib-0.0.5/src/main/python/gameauth/password.py
+-rw-r--r--   0 ceharris   (501) staff       (20)      260 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.5/src/main/python/gameauth/token.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1861 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.5/src/main/python/gameauth/token_generator.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     2155 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.5/src/main/python/gameauth/token_validator.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 19:24:53.494109 vtece4564-gamelib-0.0.5/src/main/python/gamecomm/
+-rw-r--r--   0 ceharris   (501) staff       (20)        0 2023-04-19 19:21:49.000000 vtece4564-gamelib-0.0.5/src/main/python/gamecomm/__init__.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 19:24:53.496350 vtece4564-gamelib-0.0.5/src/main/python/gamecomm/client/
+-rw-r--r--   0 ceharris   (501) staff       (20)      188 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.5/src/main/python/gamecomm/client/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     4949 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.5/src/main/python/gamecomm/client/game_client.py
+-rw-r--r--   0 ceharris   (501) staff       (20)      348 2023-04-20 10:13:04.000000 vtece4564-gamelib-0.0.5/src/main/python/gamecomm/client/game_connection.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     3914 2023-04-21 19:49:31.000000 vtece4564-gamelib-0.0.5/src/main/python/gamecomm/client/tcp_connection.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1596 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.5/src/main/python/gamecomm/client/ws_connection.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 19:24:53.498188 vtece4564-gamelib-0.0.5/src/main/python/gamecomm/server/
+-rw-r--r--   0 ceharris   (501) staff       (20)      187 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.5/src/main/python/gamecomm/server/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     7178 2023-04-21 16:16:01.000000 vtece4564-gamelib-0.0.5/src/main/python/gamecomm/server/game_connection.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     3489 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.5/src/main/python/gamecomm/server/tcp_listener.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     3835 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.5/src/main/python/gamecomm/server/ws_listener.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 19:24:53.499912 vtece4564-gamelib-0.0.5/src/main/python/gamedb/
+-rw-r--r--   0 ceharris   (501) staff       (20)      156 2023-04-19 10:45:29.000000 vtece4564-gamelib-0.0.5/src/main/python/gamedb/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)      884 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.5/src/main/python/gamedb/game_repository.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 19:24:53.501613 vtece4564-gamelib-0.0.5/src/main/python/gamedb/json/
+-rw-r--r--   0 ceharris   (501) staff       (20)      130 2023-04-21 14:47:05.000000 vtece4564-gamelib-0.0.5/src/main/python/gamedb/json/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     2154 2023-04-21 19:23:56.000000 vtece4564-gamelib-0.0.5/src/main/python/gamedb/json/game_repository.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1473 2023-04-21 19:24:11.000000 vtece4564-gamelib-0.0.5/src/main/python/gamedb/json/json_db.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     2299 2023-04-21 19:28:13.000000 vtece4564-gamelib-0.0.5/src/main/python/gamedb/json/user_repository.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 19:24:53.503677 vtece4564-gamelib-0.0.5/src/main/python/gamedb/mongo/
+-rw-r--r--   0 ceharris   (501) staff       (20)       98 2023-04-21 14:47:05.000000 vtece4564-gamelib-0.0.5/src/main/python/gamedb/mongo/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1936 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.5/src/main/python/gamedb/mongo/game_repository.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     2344 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.5/src/main/python/gamedb/mongo/user_repository.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1085 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.5/src/main/python/gamedb/user_repository.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 19:24:53.508792 vtece4564-gamelib-0.0.5/src/main/python/vtece4564_gamelib.egg-info/
+-rw-r--r--   0 ceharris   (501) staff       (20)     1262 2023-04-22 19:24:53.000000 vtece4564-gamelib-0.0.5/src/main/python/vtece4564_gamelib.egg-info/PKG-INFO
+-rw-r--r--   0 ceharris   (501) staff       (20)     1485 2023-04-22 19:24:53.000000 vtece4564-gamelib-0.0.5/src/main/python/vtece4564_gamelib.egg-info/SOURCES.txt
+-rw-r--r--   0 ceharris   (501) staff       (20)        1 2023-04-22 19:24:53.000000 vtece4564-gamelib-0.0.5/src/main/python/vtece4564_gamelib.egg-info/dependency_links.txt
+-rw-r--r--   0 ceharris   (501) staff       (20)       38 2023-04-22 19:24:53.000000 vtece4564-gamelib-0.0.5/src/main/python/vtece4564_gamelib.egg-info/requires.txt
+-rw-r--r--   0 ceharris   (501) staff       (20)       25 2023-04-22 19:24:53.000000 vtece4564-gamelib-0.0.5/src/main/python/vtece4564_gamelib.egg-info/top_level.txt
```

### Comparing `vtece4564-gamelib-0.0.4/PKG-INFO` & `vtece4564-gamelib-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: vtece4564-gamelib
-Version: 0.0.4
-Summary: A support library for the ECE 4564 Final Project
-Home-page: https://code.vt.edu/ece4564/gamelib
-Author: Carl Harris
-Author-email: ceharris414@gmail.com
-Project-URL: Bug Tracker, https://code.vt.edu/ece4564/gamelib/-/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 gamelib
 =======
 
 The project provides a Python library teams may use for
 satisfying various aspects of the final project for ECE 4564.
 It contains the following packages:
 
 * [gameauth](src/main/python/gameauth/README.md) -- authentication and authorization support
 * [gamecomm](src/main/python/gamecomm/README.md) -- client and server communication support
 * [gamedb](src/main/python/gamedb/README.md) -- user and game database support
+
+Installation
+------------
+
+To use this library in your project, install it into your virtual environment
+using `pip`. **First, activate your virtual environment**. Then install as
+follows.
+
+```bash
+pip install vtece4564-gamelib
+```
+
+This will install the library and all of its dependencies in your 
+virtual environment.
```

### Comparing `vtece4564-gamelib-0.0.4/setup.cfg` & `vtece4564-gamelib-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vtece4564-gamelib
-version = 0.0.4
+version = 0.0.5
 author = Carl Harris
 author_email = ceharris414@gmail.com
 description = A support library for the ECE 4564 Final Project
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://code.vt.edu/ece4564/gamelib
 project_urls =
```

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gameauth/__main__.py` & `vtece4564-gamelib-0.0.5/src/main/python/gameauth/__main__.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gameauth/key_util.py` & `vtece4564-gamelib-0.0.5/src/main/python/gameauth/key_util.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gameauth/password.py` & `vtece4564-gamelib-0.0.5/src/main/python/gameauth/password.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-import crypt
+from purecrypt import Crypt, Method
 
-_CRYPT_METHOD = crypt.METHOD_SHA512
+_CRYPT_METHOD = Method.SHA512
 _CRYPT_ROUNDS = 10000
 
 
 def encrypt(plaintext_password: str, salt: str = None):
     """
     Encrypts a password for storage or comparison.
     :param plaintext_password: plaintext password
     :param salt: salt to use in the encryption; specify None to generate a new salt, or specify the salt of the
         password to be compared (only that substring that represents a salt will be used)
     :return: the encyrpted password
     """
     # Generate a temporary salt so that we know the length of the salt
-    temp_salt = crypt.mksalt(_CRYPT_METHOD, rounds=_CRYPT_ROUNDS)
+    temp_salt = Crypt.generate_salt(_CRYPT_METHOD, rounds=_CRYPT_ROUNDS)
     if salt is not None:
         # Extract the salt from whatever else is in the string
         salt = salt[:len(temp_salt)]
     else:
         # Use the generated salt
         salt = temp_salt
 
-    crypto = crypt.crypt(plaintext_password, salt)
-    return f"{salt}{crypto}"
+    ciphertext_password = Crypt.encrypt(plaintext_password, salt)
+    return ciphertext_password
 
 
 def is_valid(plaintext_password: str, encrypted_password: str):
     """
     Tests whether a plaintext password matches an encrypted password.
     :param plaintext_password: the password to be test
     :param encrypted_password: the basis for the comparison
     :return: s
     """
-    # encrypt the plaintext password using the salt of the encrypted password
-    pw = encrypt(plaintext_password, encrypted_password)
-    # compare the resulting strings
-    return pw == encrypted_password
+    return Crypt.is_valid(plaintext_password, encrypted_password)
```

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gameauth/token_generator.py` & `vtece4564-gamelib-0.0.5/src/main/python/gameauth/token_generator.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gameauth/token_validator.py` & `vtece4564-gamelib-0.0.5/src/main/python/gameauth/token_validator.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gamecomm/client/game_client.py` & `vtece4564-gamelib-0.0.5/src/main/python/gamecomm/client/game_client.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gamecomm/client/tcp_connection.py` & `vtece4564-gamelib-0.0.5/src/main/python/gamecomm/client/tcp_connection.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gamecomm/client/ws_connection.py` & `vtece4564-gamelib-0.0.5/src/main/python/gamecomm/client/ws_connection.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gamecomm/server/game_connection.py` & `vtece4564-gamelib-0.0.5/src/main/python/gamecomm/server/game_connection.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gamecomm/server/tcp_listener.py` & `vtece4564-gamelib-0.0.5/src/main/python/gamecomm/server/tcp_listener.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gamecomm/server/ws_listener.py` & `vtece4564-gamelib-0.0.5/src/main/python/gamecomm/server/ws_listener.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gamedb/game_repository.py` & `vtece4564-gamelib-0.0.5/src/main/python/gamedb/game_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gamedb/json/game_repository.py` & `vtece4564-gamelib-0.0.5/src/main/python/gamedb/json/game_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gamedb/json/json_db.py` & `vtece4564-gamelib-0.0.5/src/main/python/gamedb/json/json_db.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gamedb/json/user_repository.py` & `vtece4564-gamelib-0.0.5/src/main/python/gamedb/json/user_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gamedb/mongo/game_repository.py` & `vtece4564-gamelib-0.0.5/src/main/python/gamedb/mongo/game_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gamedb/mongo/user_repository.py` & `vtece4564-gamelib-0.0.5/src/main/python/gamedb/mongo/user_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/gamedb/user_repository.py` & `vtece4564-gamelib-0.0.5/src/main/python/gamedb/user_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.4/src/main/python/vtece4564_gamelib.egg-info/SOURCES.txt` & `vtece4564-gamelib-0.0.5/src/main/python/vtece4564_gamelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

