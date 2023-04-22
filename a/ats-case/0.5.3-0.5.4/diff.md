# Comparing `tmp/ats_case-0.5.3.tar.gz` & `tmp/ats_case-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.5.3.tar", last modified: Sat Apr 22 08:02:59 2023, max compression
+gzip compressed data, was "ats_case-0.5.4.tar", last modified: Sat Apr 22 08:11:42 2023, max compression
```

## Comparing `ats_case-0.5.3.tar` & `ats_case-0.5.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 08:02:59.181251 ats_case-0.5.3/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.3/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-22 08:02:59.178886 ats_case-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 08:02:58.791593 ats_case-0.5.3/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.3/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 08:02:59.008314 ats_case-0.5.3/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.3/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17443 2023-04-22 08:02:29.000000 ats_case-0.5.3/ats_case/case/command.py
--rw-rw-rw-   0        0        0     9683 2023-04-20 08:35:14.000000 ats_case-0.5.3/ats_case/case/context.py
--rw-rw-rw-   0        0        0     6309 2023-04-21 03:45:03.000000 ats_case-0.5.3/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5593 2023-04-21 02:33:28.000000 ats_case-0.5.3/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-22 08:02:59.073215 ats_case-0.5.3/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.3/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.3/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.3/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-22 08:02:59.134561 ats_case-0.5.3/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.3/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.3/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.3/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-22 08:02:59.168482 ats_case-0.5.3/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.3/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.3/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-22 08:02:58.883204 ats_case-0.5.3/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-22 08:02:58.000000 ats_case-0.5.3/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-22 08:02:58.000000 ats_case-0.5.3/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 08:02:58.000000 ats_case-0.5.3/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-22 08:02:58.000000 ats_case-0.5.3/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-22 08:02:58.000000 ats_case-0.5.3/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 08:02:59.181251 ats_case-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-22 08:02:46.000000 ats_case-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 08:11:42.079189 ats_case-0.5.4/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.4/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-22 08:11:42.077187 ats_case-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 08:11:41.701257 ats_case-0.5.4/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.4/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 08:11:41.900642 ats_case-0.5.4/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.4/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17443 2023-04-22 08:02:29.000000 ats_case-0.5.4/ats_case/case/command.py
+-rw-rw-rw-   0        0        0     9683 2023-04-20 08:35:14.000000 ats_case-0.5.4/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     6309 2023-04-21 03:45:03.000000 ats_case-0.5.4/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5593 2023-04-21 02:33:28.000000 ats_case-0.5.4/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-22 08:11:41.969703 ats_case-0.5.4/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.4/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.4/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.4/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-22 08:11:42.029850 ats_case-0.5.4/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.4/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.4/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.4/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-22 08:11:42.060725 ats_case-0.5.4/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.4/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.4/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-22 08:11:41.787209 ats_case-0.5.4/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-22 08:11:41.000000 ats_case-0.5.4/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-22 08:11:41.000000 ats_case-0.5.4/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 08:11:41.000000 ats_case-0.5.4/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-22 08:11:41.000000 ats_case-0.5.4/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-22 08:11:41.000000 ats_case-0.5.4/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 08:11:42.079189 ats_case-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-22 08:11:37.000000 ats_case-0.5.4/setup.py
```

### Comparing `ats_case-0.5.3/PKG-INFO` & `ats_case-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.5.3
+Version: 0.5.4
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.3/README.md` & `ats_case-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.3/ats_case/case/command.py` & `ats_case-0.5.4/ats_case/case/command.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.3/ats_case/case/context.py` & `ats_case-0.5.4/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.3/ats_case/case/executor.py` & `ats_case-0.5.4/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.3/ats_case/case/translator.py` & `ats_case-0.5.4/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.3/ats_case/common/error.py` & `ats_case-0.5.4/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.3/ats_case/manage/core.py` & `ats_case-0.5.4/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.3/ats_case/manage/start.py` & `ats_case-0.5.4/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.3/ats_case/template/testcase_v1.tmp` & `ats_case-0.5.4/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.3/ats_case.egg-info/PKG-INFO` & `ats_case-0.5.4/ats_case.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.5.3
+Version: 0.5.4
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.3/ats_case.egg-info/SOURCES.txt` & `ats_case-0.5.4/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.3/setup.py` & `ats_case-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.5.3",
+    version="0.5.4",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

