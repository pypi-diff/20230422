# Comparing `tmp/hk_utils-1.1.6-py3-none-any.whl.zip` & `tmp/hk_utils-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4800 bytes, number of entries: 7
--rw-r--r--  2.0 unx     5288 b- defN 23-Apr-10 10:25 hk_utils/AttrDict.py
--rw-r--r--  2.0 unx       93 b- defN 23-Mar-31 17:26 hk_utils/__init__.py
--rw-r--r--  2.0 unx     7020 b- defN 23-Mar-31 17:11 hk_utils/hk_print.py
--rw-r--r--  2.0 unx     2199 b- defN 23-Apr-10 10:25 hk_utils-1.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 10:25 hk_utils-1.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-10 10:25 hk_utils-1.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      530 b- defN 23-Apr-10 10:25 hk_utils-1.1.6.dist-info/RECORD
-7 files, 15231 bytes uncompressed, 3862 bytes compressed:  74.6%
+Zip file size: 4777 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     5192 b- defN 23-Apr-22 13:27 hk_utils/AttrDict.py
+-rw-rw-r--  2.0 unx       93 b- defN 23-Apr-22 13:20 hk_utils/__init__.py
+-rw-rw-r--  2.0 unx     7020 b- defN 23-Apr-22 13:20 hk_utils/hk_print.py
+-rw-rw-r--  2.0 unx     2180 b- defN 23-Apr-22 13:27 hk_utils-1.1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-22 13:27 hk_utils-1.1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Apr-22 13:27 hk_utils-1.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      530 b- defN 23-Apr-22 13:27 hk_utils-1.1.7.dist-info/RECORD
+7 files, 15116 bytes uncompressed, 3839 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: hk_utils/__init__.py
 Comment: 
 
 Filename: hk_utils/hk_print.py
 Comment: 
 
-Filename: hk_utils-1.1.6.dist-info/METADATA
+Filename: hk_utils-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: hk_utils-1.1.6.dist-info/WHEEL
+Filename: hk_utils-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: hk_utils-1.1.6.dist-info/top_level.txt
+Filename: hk_utils-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: hk_utils-1.1.6.dist-info/RECORD
+Filename: hk_utils-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hk_utils/AttrDict.py

```diff
@@ -39,26 +39,22 @@
         return cls(input)
     
     def __getattr__(self, key):
         return None # fallback to None if key not exists in self.__dict__
     
     def __setattr__(self, key, value):
         assert type(key) in [int, str], f"invalid key type {type(key)} : only int, str are available"
-        if type(value) == dict:
-            value = AttrDict(value)
-        self.__dict__[key] = value
+        self.__dict__[key] = self._deep_convert(value)
         
     def __getitem__(self, key):
         return self.__dict__[key] if key in self.__dict__ else None
     
     def __setitem__(self, key, value):
         assert type(key) in [int, str], f"invalid key type {type(key)} : only int, str are available"
-        if type(value) == dict:
-            value = AttrDict(value)
-        self.__dict__[key] = value
+        self.__dict__[key] = self._deep_convert(value)
         
     def __delitem__(self, key):
         del self.__dict__[key]
     
     def __repr__(self):
         dict_str = [ repr(key) + ": " + repr(value) for key, value in self.__dict__.items() ]
         return "{" + ', '.join(dict_str) + "}"
```

## Comparing `hk_utils-1.1.6.dist-info/METADATA` & `hk_utils-1.1.7.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: hk-utils
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python utilities by Heekang Park
 Home-page: https://github.com/HeekangPark/hk-utils
 Author: Heekang Park
 Author-email: park.heekang33@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # hk_utils [PYTHON]
@@ -100,8 +99,7 @@
 
 - 최초 버전
 - `hk_print` 모듈 추가
 
 ### v1.1
 
 - `AttrDict` 모듈 추가
-
```

