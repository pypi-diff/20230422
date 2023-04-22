# Comparing `tmp/gqylpy_datastruct-2.2.3-py3-none-any.whl.zip` & `tmp/gqylpy_datastruct-2.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 17148 bytes, number of entries: 7
--rw-r--r--  2.0 unx     7474 b- defN 23-Mar-05 03:20 gqylpy_datastruct/__init__.py
--rw-r--r--  2.0 unx    34228 b- defN 23-Mar-05 03:20 gqylpy_datastruct/g datastruct.py
--rw-r--r--  2.0 unx    11389 b- defN 23-Mar-05 03:20 gqylpy_datastruct-2.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     8071 b- defN 23-Mar-05 03:20 gqylpy_datastruct-2.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-05 03:20 gqylpy_datastruct-2.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Mar-05 03:20 gqylpy_datastruct-2.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      614 b- defN 23-Mar-05 03:20 gqylpy_datastruct-2.2.3.dist-info/RECORD
-7 files, 61886 bytes uncompressed, 16052 bytes compressed:  74.1%
+Zip file size: 17200 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     7474 b- defN 23-Apr-22 03:40 gqylpy_datastruct/__init__.py
+-rw-r--r--  2.0 unx    34341 b- defN 23-Apr-22 03:40 gqylpy_datastruct/g datastruct.py
+-rw-r--r--  2.0 unx    11389 b- defN 23-Apr-22 03:41 gqylpy_datastruct-2.2.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8064 b- defN 23-Apr-22 03:41 gqylpy_datastruct-2.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 03:41 gqylpy_datastruct-2.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Apr-22 03:41 gqylpy_datastruct-2.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      614 b- defN 23-Apr-22 03:41 gqylpy_datastruct-2.2.4.dist-info/RECORD
+7 files, 61992 bytes uncompressed, 16104 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: gqylpy_datastruct/__init__.py
 Comment: 
 
 Filename: gqylpy_datastruct/g datastruct.py
 Comment: 
 
-Filename: gqylpy_datastruct-2.2.3.dist-info/LICENSE
+Filename: gqylpy_datastruct-2.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: gqylpy_datastruct-2.2.3.dist-info/METADATA
+Filename: gqylpy_datastruct-2.2.4.dist-info/METADATA
 Comment: 
 
-Filename: gqylpy_datastruct-2.2.3.dist-info/WHEEL
+Filename: gqylpy_datastruct-2.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: gqylpy_datastruct-2.2.3.dist-info/top_level.txt
+Filename: gqylpy_datastruct-2.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: gqylpy_datastruct-2.2.3.dist-info/RECORD
+Filename: gqylpy_datastruct-2.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gqylpy_datastruct/__init__.py

```diff
@@ -2,15 +2,15 @@
 Create a blueprint to draw the data structure of your program, and then use this
 blueprint to verify that the incoming data is correct.
 
     >>> from gqylpy_datastruct import DataStruct
     >>> datastruct = DataStruct({'name': {type: str}})
     >>> err = datastruct.verify({'name': 'Alpha'})
 
-    @version: 2.2.3
+    @version: 2.2.4
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/gqylpy-datastruct
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

## gqylpy_datastruct/g datastruct.py

```diff
@@ -17,15 +17,15 @@
 import re
 import sys
 import copy
 import inspect
 import decimal
 import datetime
 
-from typing import Union, Callable, Generator, Any
+from typing import Union, Pattern, Callable, Generator, Any
 
 import gqylpy_exception as ge
 
 unique = b'GQYLPY, \xe6\x94\xb9\xe5\x8f\x98\xe4\xb8\x96\xe7\x95\x8c\xe3\x80\x82'
 
 coerces_supported = (
     int, float, bytes, str, tuple, list, set, frozenset, dict, bool
@@ -440,15 +440,15 @@
             })
         blueprint[key] = tuple(value)
 
     def verify_verify(
             self,
             keypath:    str,
             key:        str,
-            value:      Union[str, Callable, re.Pattern, tuple, list],
+            value:      Union[str, Callable, Pattern, tuple, list],
             blueprint:  dict,
             *,
             full_value: Union[tuple, list] = None
     ) -> None:
         value_type: type = value.__class__
 
         if value_type in (tuple, list) and not full_value:
@@ -809,15 +809,15 @@
                 }
             value = data[key] = [value]
         return 1, value
 
     def verify_verify(
             self,
             keypath:     str,
-            verify:      Union[re.Pattern, Callable, list, tuple],
+            verify:      Union[Pattern, Callable, list, tuple],
             value:       Any,
             _, __,
     ) -> tuple:
         if verify.__class__ in (list, tuple):
             mode = any if verify.__class__ is list else all
             results = [self.verify_verify(
                 keypath, v, value, _, __
@@ -832,15 +832,16 @@
                     'keypath': keypath,
                     'value': value,
                     'verify': verify_string,
                     'msg': 'verify failed.',
                     'hint': '"tuple" will be execute in "and" mode, '
                             '"list" will be execute in "or" mode.'
                 }
-        elif verify.__class__ is re.Pattern:
+        elif (sys.version_info >= (3, 8) and verify.__class__ is re.Pattern) \
+                or (str(verify.__class__) == "<class '_sre.SRE_Pattern'>"):
             if value.__class__ in (int, float):
                 value = str(value)
             try:
                 result = verify.search(value)
             except TypeError as e:
                 return 0, {
                     'title': 'VerifyError',
```

## Comparing `gqylpy_datastruct-2.2.3.dist-info/LICENSE` & `gqylpy_datastruct-2.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gqylpy_datastruct-2.2.3.dist-info/METADATA` & `gqylpy_datastruct-2.2.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqylpy-datastruct
-Version: 2.2.3
+Version: 2.2.4
 Summary: 创建一张蓝图来规划好程序需要的数据结构，并在之后使用该蓝图去校验到来的数据是否如期。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-datastruct
 Classifier: Environment :: Web Environment
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: gqylpy-exception (<2.0,>=1.3.2)
+Requires-Dist: gqylpy-exception (>=2.0)
 
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-datastruct.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-datastruct/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_datastruct)](https://pypi.org/project/gqylpy_datastruct)
 [![License](https://img.shields.io/pypi/l/gqylpy_datastruct)](https://github.com/gqylpy/gqylpy-datastruct/blob/master/LICENSE)
 [![Downloads](https://pepy.tech/badge/gqylpy_datastruct/month)](https://pepy.tech/project/gqylpy_datastruct)
```

