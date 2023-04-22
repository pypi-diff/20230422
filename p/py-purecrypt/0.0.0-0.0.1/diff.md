# Comparing `tmp/py-purecrypt-0.0.0.tar.gz` & `tmp/py-purecrypt-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-purecrypt-0.0.0.tar", last modified: Sat Apr 22 17:54:00 2023, max compression
+gzip compressed data, was "py-purecrypt-0.0.1.tar", last modified: Sat Apr 22 17:59:24 2023, max compression
```

## Comparing `py-purecrypt-0.0.0.tar` & `py-purecrypt-0.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 17:54:00.216581 py-purecrypt-0.0.0/
--rw-r--r--   0 ceharris   (501) staff       (20)     1066 2023-04-22 14:54:21.000000 py-purecrypt-0.0.0/LICENSE
--rw-r--r--   0 ceharris   (501) staff       (20)     2124 2023-04-22 17:54:00.216824 py-purecrypt-0.0.0/PKG-INFO
--rw-r--r--   0 ceharris   (501) staff       (20)     1587 2023-04-22 17:50:03.000000 py-purecrypt-0.0.0/README.md
--rw-r--r--   0 ceharris   (501) staff       (20)       41 2023-04-21 18:22:43.000000 py-purecrypt-0.0.0/pyproject.toml
--rw-r--r--   0 ceharris   (501) staff       (20)      720 2023-04-22 17:54:00.217898 py-purecrypt-0.0.0/setup.cfg
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 17:54:00.206731 py-purecrypt-0.0.0/src/
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 17:54:00.206890 py-purecrypt-0.0.0/src/main/
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 17:54:00.207349 py-purecrypt-0.0.0/src/main/python/
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 17:54:00.213672 py-purecrypt-0.0.0/src/main/python/purecrypt/
--rw-r--r--   0 ceharris   (501) staff       (20)       52 2023-04-22 16:52:31.000000 py-purecrypt-0.0.0/src/main/python/purecrypt/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)      923 2023-04-22 17:14:35.000000 py-purecrypt-0.0.0/src/main/python/purecrypt/__main__.py
--rw-r--r--   0 ceharris   (501) staff       (20)      292 2023-04-22 15:51:49.000000 py-purecrypt-0.0.0/src/main/python/purecrypt/b64.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1640 2023-04-22 17:33:12.000000 py-purecrypt-0.0.0/src/main/python/purecrypt/crypt.py
--rw-r--r--   0 ceharris   (501) staff       (20)     3740 2023-04-22 17:40:48.000000 py-purecrypt-0.0.0/src/main/python/purecrypt/crypt_md5.py
--rw-r--r--   0 ceharris   (501) staff       (20)     6513 2023-04-22 17:33:12.000000 py-purecrypt-0.0.0/src/main/python/purecrypt/crypt_sha2.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1045 2023-04-22 17:03:31.000000 py-purecrypt-0.0.0/src/main/python/purecrypt/crypt_sha256.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1855 2023-04-22 17:03:31.000000 py-purecrypt-0.0.0/src/main/python/purecrypt/crypt_sha512.py
--rw-r--r--   0 ceharris   (501) staff       (20)       51 2023-04-22 15:42:49.000000 py-purecrypt-0.0.0/src/main/python/purecrypt/limits.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1346 2023-04-22 17:33:12.000000 py-purecrypt-0.0.0/src/main/python/purecrypt/method.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1126 2023-04-22 15:42:25.000000 py-purecrypt-0.0.0/src/main/python/purecrypt/salt.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 17:54:00.216247 py-purecrypt-0.0.0/src/main/python/py_purecrypt.egg-info/
--rw-r--r--   0 ceharris   (501) staff       (20)     2124 2023-04-22 17:54:00.000000 py-purecrypt-0.0.0/src/main/python/py_purecrypt.egg-info/PKG-INFO
--rw-r--r--   0 ceharris   (501) staff       (20)      714 2023-04-22 17:54:00.000000 py-purecrypt-0.0.0/src/main/python/py_purecrypt.egg-info/SOURCES.txt
--rw-r--r--   0 ceharris   (501) staff       (20)        1 2023-04-22 17:54:00.000000 py-purecrypt-0.0.0/src/main/python/py_purecrypt.egg-info/dependency_links.txt
--rw-r--r--   0 ceharris   (501) staff       (20)       13 2023-04-22 17:54:00.000000 py-purecrypt-0.0.0/src/main/python/py_purecrypt.egg-info/requires.txt
--rw-r--r--   0 ceharris   (501) staff       (20)       10 2023-04-22 17:54:00.000000 py-purecrypt-0.0.0/src/main/python/py_purecrypt.egg-info/top_level.txt
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 17:59:24.980319 py-purecrypt-0.0.1/
+-rw-r--r--   0 ceharris   (501) staff       (20)     1066 2023-04-22 14:54:21.000000 py-purecrypt-0.0.1/LICENSE
+-rw-r--r--   0 ceharris   (501) staff       (20)     2272 2023-04-22 17:59:24.980551 py-purecrypt-0.0.1/PKG-INFO
+-rw-r--r--   0 ceharris   (501) staff       (20)     1744 2023-04-22 17:57:58.000000 py-purecrypt-0.0.1/README.md
+-rw-r--r--   0 ceharris   (501) staff       (20)       41 2023-04-21 18:22:43.000000 py-purecrypt-0.0.1/pyproject.toml
+-rw-r--r--   0 ceharris   (501) staff       (20)      711 2023-04-22 17:59:24.981283 py-purecrypt-0.0.1/setup.cfg
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 17:59:24.971522 py-purecrypt-0.0.1/src/
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 17:59:24.971717 py-purecrypt-0.0.1/src/main/
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 17:59:24.972123 py-purecrypt-0.0.1/src/main/python/
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 17:59:24.977923 py-purecrypt-0.0.1/src/main/python/purecrypt/
+-rw-r--r--   0 ceharris   (501) staff       (20)       52 2023-04-22 16:52:31.000000 py-purecrypt-0.0.1/src/main/python/purecrypt/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)      923 2023-04-22 17:14:35.000000 py-purecrypt-0.0.1/src/main/python/purecrypt/__main__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)      292 2023-04-22 15:51:49.000000 py-purecrypt-0.0.1/src/main/python/purecrypt/b64.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1640 2023-04-22 17:33:12.000000 py-purecrypt-0.0.1/src/main/python/purecrypt/crypt.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     3740 2023-04-22 17:40:48.000000 py-purecrypt-0.0.1/src/main/python/purecrypt/crypt_md5.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     6513 2023-04-22 17:33:12.000000 py-purecrypt-0.0.1/src/main/python/purecrypt/crypt_sha2.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1045 2023-04-22 17:03:31.000000 py-purecrypt-0.0.1/src/main/python/purecrypt/crypt_sha256.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1855 2023-04-22 17:03:31.000000 py-purecrypt-0.0.1/src/main/python/purecrypt/crypt_sha512.py
+-rw-r--r--   0 ceharris   (501) staff       (20)       51 2023-04-22 15:42:49.000000 py-purecrypt-0.0.1/src/main/python/purecrypt/limits.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1346 2023-04-22 17:33:12.000000 py-purecrypt-0.0.1/src/main/python/purecrypt/method.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1126 2023-04-22 15:42:25.000000 py-purecrypt-0.0.1/src/main/python/purecrypt/salt.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 17:59:24.980005 py-purecrypt-0.0.1/src/main/python/py_purecrypt.egg-info/
+-rw-r--r--   0 ceharris   (501) staff       (20)     2272 2023-04-22 17:59:24.000000 py-purecrypt-0.0.1/src/main/python/py_purecrypt.egg-info/PKG-INFO
+-rw-r--r--   0 ceharris   (501) staff       (20)      714 2023-04-22 17:59:24.000000 py-purecrypt-0.0.1/src/main/python/py_purecrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 ceharris   (501) staff       (20)        1 2023-04-22 17:59:24.000000 py-purecrypt-0.0.1/src/main/python/py_purecrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 ceharris   (501) staff       (20)       13 2023-04-22 17:59:24.000000 py-purecrypt-0.0.1/src/main/python/py_purecrypt.egg-info/requires.txt
+-rw-r--r--   0 ceharris   (501) staff       (20)       10 2023-04-22 17:59:24.000000 py-purecrypt-0.0.1/src/main/python/py_purecrypt.egg-info/top_level.txt
```

### Comparing `py-purecrypt-0.0.0/LICENSE` & `py-purecrypt-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-purecrypt-0.0.0/PKG-INFO` & `py-purecrypt-0.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: py-purecrypt
-Version: 0.0.0
-Summary: A pure Python implementation of common UNIX password encryption
+Version: 0.0.1
+Summary: A pure Python implementation of crypt(3) from GNU libc
 Home-page: https://gitlab.com/soulwing/py-purecrypt
 Author: Carl Harris
 Author-email: ceharris414@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/soulwing/py-purecrypt
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,21 @@
 [cryptography](https://pypi.org/project/cryptography/) package, it should 
 run on any platform supported by Python.
 
 This implementation is not fast. If you're looking for speed, I suggest you
 consider alternatives such as [bcrypt](https://pypi.org/project/bcrypt/).
 
 
+Installation
+------------
+
+Install `py-purecrypt` from [PyPI](https://pypi.org/project/py-purecrypt)
+using `pip` or your preferred Python package manager.
+
+
 Usage
 -----
 
 This section shows basic usage examples.
 
 ### Encrypt a password
```

### Comparing `py-purecrypt-0.0.0/README.md` & `py-purecrypt-0.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 [cryptography](https://pypi.org/project/cryptography/) package, it should 
 run on any platform supported by Python.
 
 This implementation is not fast. If you're looking for speed, I suggest you
 consider alternatives such as [bcrypt](https://pypi.org/project/bcrypt/).
 
 
+Installation
+------------
+
+Install `py-purecrypt` from [PyPI](https://pypi.org/project/py-purecrypt)
+using `pip` or your preferred Python package manager.
+
+
 Usage
 -----
 
 This section shows basic usage examples.
 
 ### Encrypt a password
```

### Comparing `py-purecrypt-0.0.0/setup.cfg` & `py-purecrypt-0.0.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = py-purecrypt
-version = 0.0.0
+version = 0.0.1
 author = Carl Harris
 author_email = ceharris414@gmail.com
-description = A pure Python implementation of common UNIX password encryption
+description = A pure Python implementation of crypt(3) from GNU libc
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/soulwing/py-purecrypt
 project_urls = 
 	Bug Tracker = https://gitlab.com/soulwing/py-purecrypt
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `py-purecrypt-0.0.0/src/main/python/purecrypt/__main__.py` & `py-purecrypt-0.0.1/src/main/python/purecrypt/__main__.py`

 * *Files identical despite different names*

### Comparing `py-purecrypt-0.0.0/src/main/python/purecrypt/crypt.py` & `py-purecrypt-0.0.1/src/main/python/purecrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `py-purecrypt-0.0.0/src/main/python/purecrypt/crypt_md5.py` & `py-purecrypt-0.0.1/src/main/python/purecrypt/crypt_md5.py`

 * *Files identical despite different names*

### Comparing `py-purecrypt-0.0.0/src/main/python/purecrypt/crypt_sha2.py` & `py-purecrypt-0.0.1/src/main/python/purecrypt/crypt_sha2.py`

 * *Files identical despite different names*

### Comparing `py-purecrypt-0.0.0/src/main/python/purecrypt/crypt_sha256.py` & `py-purecrypt-0.0.1/src/main/python/purecrypt/crypt_sha256.py`

 * *Files identical despite different names*

### Comparing `py-purecrypt-0.0.0/src/main/python/purecrypt/crypt_sha512.py` & `py-purecrypt-0.0.1/src/main/python/purecrypt/crypt_sha512.py`

 * *Files identical despite different names*

### Comparing `py-purecrypt-0.0.0/src/main/python/purecrypt/method.py` & `py-purecrypt-0.0.1/src/main/python/purecrypt/method.py`

 * *Files identical despite different names*

### Comparing `py-purecrypt-0.0.0/src/main/python/purecrypt/salt.py` & `py-purecrypt-0.0.1/src/main/python/purecrypt/salt.py`

 * *Files identical despite different names*

### Comparing `py-purecrypt-0.0.0/src/main/python/py_purecrypt.egg-info/PKG-INFO` & `py-purecrypt-0.0.1/src/main/python/py_purecrypt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: py-purecrypt
-Version: 0.0.0
-Summary: A pure Python implementation of common UNIX password encryption
+Version: 0.0.1
+Summary: A pure Python implementation of crypt(3) from GNU libc
 Home-page: https://gitlab.com/soulwing/py-purecrypt
 Author: Carl Harris
 Author-email: ceharris414@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/soulwing/py-purecrypt
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,21 @@
 [cryptography](https://pypi.org/project/cryptography/) package, it should 
 run on any platform supported by Python.
 
 This implementation is not fast. If you're looking for speed, I suggest you
 consider alternatives such as [bcrypt](https://pypi.org/project/bcrypt/).
 
 
+Installation
+------------
+
+Install `py-purecrypt` from [PyPI](https://pypi.org/project/py-purecrypt)
+using `pip` or your preferred Python package manager.
+
+
 Usage
 -----
 
 This section shows basic usage examples.
 
 ### Encrypt a password
```

### Comparing `py-purecrypt-0.0.0/src/main/python/py_purecrypt.egg-info/SOURCES.txt` & `py-purecrypt-0.0.1/src/main/python/py_purecrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

