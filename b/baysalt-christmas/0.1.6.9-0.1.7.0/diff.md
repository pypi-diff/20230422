# Comparing `tmp/baysalt_christmas-0.1.6.9.tar.gz` & `tmp/baysalt_christmas-0.1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.6.9.tar", last modified: Thu Apr 20 15:23:14 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.7.0.tar", last modified: Sat Apr 22 08:23:23 2023, max compression
```

## Comparing `baysalt_christmas-0.1.6.9.tar` & `baysalt_christmas-0.1.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-20 15:23:14.695692 baysalt_christmas-0.1.6.9/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-04-19 08:43:20.000000 baysalt_christmas-0.1.6.9/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.6.9/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-20 15:23:14.695533 baysalt_christmas-0.1.6.9/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.6.9/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-20 15:23:14.690268 baysalt_christmas-0.1.6.9/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-20 15:23:14.000000 baysalt_christmas-0.1.6.9/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      725 2023-04-20 15:23:14.000000 baysalt_christmas-0.1.6.9/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-04-20 15:23:14.000000 baysalt_christmas-0.1.6.9/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       21 2023-04-20 15:23:14.000000 baysalt_christmas-0.1.6.9/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-04-20 15:23:14.000000 baysalt_christmas-0.1.6.9/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-20 15:23:14.691939 baysalt_christmas-0.1.6.9/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    18765 2023-04-20 15:22:34.000000 baysalt_christmas-0.1.6.9/christmas/Blog.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.6.9/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      441 2023-04-13 14:13:51.000000 baysalt_christmas-0.1.6.9/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4094 2023-04-20 13:28:55.000000 baysalt_christmas-0.1.6.9/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.6.9/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-20 15:23:14.694045 baysalt_christmas-0.1.6.9/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.6.9/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.6.9/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.6.9/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-20 15:23:14.695182 baysalt_christmas-0.1.6.9/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.6.9/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.6.9/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.6.9/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.6.9/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.6.9/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.6.9/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-04-13 06:21:12.000000 baysalt_christmas-0.1.6.9/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.6.9/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.6.9/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-04-20 15:23:14.695748 baysalt_christmas-0.1.6.9/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-04-20 15:23:13.000000 baysalt_christmas-0.1.6.9/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-22 08:23:23.793805 baysalt_christmas-0.1.7.0/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-04-19 08:43:20.000000 baysalt_christmas-0.1.7.0/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.0/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-22 08:23:23.793668 baysalt_christmas-0.1.7.0/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.0/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-22 08:23:23.788643 baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-22 08:23:23.000000 baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      725 2023-04-22 08:23:23.000000 baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-04-22 08:23:23.000000 baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       21 2023-04-22 08:23:23.000000 baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-04-22 08:23:23.000000 baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-22 08:23:23.789921 baysalt_christmas-0.1.7.0/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    18741 2023-04-22 08:22:21.000000 baysalt_christmas-0.1.7.0/christmas/Blog.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.0/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      441 2023-04-13 14:13:51.000000 baysalt_christmas-0.1.7.0/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4094 2023-04-20 13:28:55.000000 baysalt_christmas-0.1.7.0/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.0/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-22 08:23:23.791300 baysalt_christmas-0.1.7.0/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-22 08:23:23.793323 baysalt_christmas-0.1.7.0/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.0/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-04-13 06:21:12.000000 baysalt_christmas-0.1.7.0/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.0/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.0/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-04-22 08:23:23.793854 baysalt_christmas-0.1.7.0/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-04-22 08:23:15.000000 baysalt_christmas-0.1.7.0/setup.py
```

### Comparing `baysalt_christmas-0.1.6.9/.DS_Store` & `baysalt_christmas-0.1.7.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.9/PKG-INFO` & `baysalt_christmas-0.1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.6.9
+Version: 0.1.7.0
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.6.9/README.md` & `baysalt_christmas-0.1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.9/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.6.9
+Version: 0.1.7.0
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.6.9/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.9/christmas/Blog.py` & `baysalt_christmas-0.1.7.0/christmas/Blog.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,16 +139,14 @@
             rmfiles(self.__all_log_path,
                     self.__error_plus_log_path,
                     self.debug_log_filename,
                     self.info_log_filename,
                     self.warning_log_filename,
                     self.error_log_filename,
                     self.critical_log_filename)
-
-        self.console()
     
     def __init_logger_handler(self, logfile_path, Rotating='time', when='H', interval=1):
         # sourcery skip: inline-immediately-returned-variable
         """
         创建日志记录器handler，用于收集日志
         :param logfile_path: 日志文件路径
         :return: 日志记录器
```

### Comparing `baysalt_christmas-0.1.6.9/christmas/S_DateTime.py` & `baysalt_christmas-0.1.7.0/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.9/christmas/commonCode.py` & `baysalt_christmas-0.1.7.0/christmas/commonCode.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.9/christmas/cprintf.py` & `baysalt_christmas-0.1.7.0/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.9/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.7.0/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.9/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.7.0/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.9/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.7.0/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.9/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.7.0/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.9/christmas/mncPy/common.py` & `baysalt_christmas-0.1.7.0/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.9/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.7.0/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.9/christmas/processBar.py` & `baysalt_christmas-0.1.7.0/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.9/christmas/read_conf.py` & `baysalt_christmas-0.1.7.0/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.9/christmas/server_info.py` & `baysalt_christmas-0.1.7.0/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.6.9/setup.py` & `baysalt_christmas-0.1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.6.9",
+    version="0.1.7.0",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

