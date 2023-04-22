# Comparing `tmp/StringFix-0.6.8.tar.gz` & `tmp/StringFix-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StringFix-0.6.8.tar", last modified: Sat Apr 22 05:29:11 2023, max compression
+gzip compressed data, was "StringFix-0.6.9.tar", last modified: Sat Apr 22 05:33:17 2023, max compression
```

## Comparing `StringFix-0.6.8.tar` & `StringFix-0.6.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-04-22 05:29:11.708037 StringFix-0.6.8/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-04-20 03:05:32.000000 StringFix-0.6.8/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-04-20 03:25:54.000000 StringFix-0.6.8/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      676 2023-04-22 05:29:11.708037 StringFix-0.6.8/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      111 2023-04-20 03:25:54.000000 StringFix-0.6.8/README.md
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-04-22 05:29:11.708037 StringFix-0.6.8/StringFix/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-04-20 05:42:13.000000 StringFix-0.6.8/StringFix/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   598129 2023-04-22 05:28:21.000000 StringFix-0.6.8/StringFix/core.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    53685 2023-04-22 02:22:03.000000 StringFix-0.6.8/StringFix/pybam.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     7641 2023-04-22 03:48:29.000000 StringFix-0.6.8/StringFix/run_sfix.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-04-22 05:29:11.708037 StringFix-0.6.8/StringFix.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      676 2023-04-22 05:29:11.000000 StringFix-0.6.8/StringFix.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      325 2023-04-22 05:29:11.000000 StringFix-0.6.8/StringFix.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-04-22 05:29:11.000000 StringFix-0.6.8/StringFix.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-04-22 05:29:11.000000 StringFix-0.6.8/StringFix.egg-info/not-zip-safe
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-04-22 05:29:11.000000 StringFix-0.6.8/StringFix.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       10 2023-04-22 05:29:11.000000 StringFix-0.6.8/StringFix.egg-info/top_level.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-04-22 05:29:11.708037 StringFix-0.6.8/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     2669 2023-04-22 05:28:55.000000 StringFix-0.6.8/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-04-22 05:33:17.494445 StringFix-0.6.9/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-04-20 03:05:32.000000 StringFix-0.6.9/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-04-20 03:25:54.000000 StringFix-0.6.9/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      676 2023-04-22 05:33:17.494445 StringFix-0.6.9/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      111 2023-04-20 03:25:54.000000 StringFix-0.6.9/README.md
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-04-22 05:33:17.494445 StringFix-0.6.9/StringFix/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-04-20 05:42:13.000000 StringFix-0.6.9/StringFix/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   598129 2023-04-22 05:28:21.000000 StringFix-0.6.9/StringFix/core.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    53685 2023-04-22 02:22:03.000000 StringFix-0.6.9/StringFix/pybam.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     7641 2023-04-22 05:31:54.000000 StringFix-0.6.9/StringFix/run_sfix.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-04-22 05:33:17.494445 StringFix-0.6.9/StringFix.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      676 2023-04-22 05:33:17.000000 StringFix-0.6.9/StringFix.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      325 2023-04-22 05:33:17.000000 StringFix-0.6.9/StringFix.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-04-22 05:33:17.000000 StringFix-0.6.9/StringFix.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-04-22 05:33:17.000000 StringFix-0.6.9/StringFix.egg-info/not-zip-safe
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-04-22 05:33:17.000000 StringFix-0.6.9/StringFix.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       10 2023-04-22 05:33:17.000000 StringFix-0.6.9/StringFix.egg-info/top_level.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-04-22 05:33:17.494445 StringFix-0.6.9/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     2669 2023-04-22 05:32:30.000000 StringFix-0.6.9/setup.py
```

### Comparing `StringFix-0.6.8/LICENSE` & `StringFix-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `StringFix-0.6.8/PKG-INFO` & `StringFix-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StringFix
-Version: 0.6.8
+Version: 0.6.9
 Summary: Annotation guided transcriptome assembly program.
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Joongho Lee, Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi StringFix
 Classifier: Programming Language :: Python :: 3
```

### Comparing `StringFix-0.6.8/StringFix/core.py` & `StringFix-0.6.9/StringFix/core.py`

 * *Files identical despite different names*

### Comparing `StringFix-0.6.8/StringFix/pybam.py` & `StringFix-0.6.9/StringFix/pybam.py`

 * *Files identical despite different names*

### Comparing `StringFix-0.6.8/StringFix/run_sfix.py` & `StringFix-0.6.9/StringFix/run_sfix.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     args = parser.parse_args()
     return args, parser
 
 
 def main():
 
     print('+------------------------------+')
-    print('|      Stringfix v.0.6.6       |')
+    print('|      Stringfix v.0.6.9       |')
     print('+------------------------------+')
 
     args, parser = get_args()
 
     if (args.input is None): # | (args.gtf is None) | (args.gnm is None):
         parser.print_help()
         return
```

### Comparing `StringFix-0.6.8/StringFix.egg-info/PKG-INFO` & `StringFix-0.6.9/StringFix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StringFix
-Version: 0.6.8
+Version: 0.6.9
 Summary: Annotation guided transcriptome assembly program.
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Joongho Lee, Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi StringFix
 Classifier: Programming Language :: Python :: 3
```

### Comparing `StringFix-0.6.8/setup.py` & `StringFix-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     # 배포할 패키지의 이름을 적어줍니다. setup.py파일을 가지는 폴더 이름과 동일하게 합니다.
     name                = 'StringFix',
     # 배포할 패키지의 버전을 적어줍니다. 첫 등록이므로 0.1 또는 0.0.1을 사용합니다.
-    version             = '0.6.8',
+    version             = '0.6.9',
     # 배포할 패키지에 대한 설명을 작성합니다.
     description         = 'Annotation guided transcriptome assembly program.',
     # 배포하는 사람의 이름을 작성합니다.
     author              = 'Joongho Lee, Seokhyun Yoon',
     # 배포하는 사람의 메일주소를 작성합니다.
     author_email        = 'syoon@dku.edu',
     # 배포하는 패키지의 url을 적어줍니다. 보통 github 링크를 적습니다.
```

