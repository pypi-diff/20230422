# Comparing `tmp/dragonfile-1.0.0-py3-none-any.whl.zip` & `tmp/dragonfile-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3214 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     4045 b- defN 23-Apr-22 04:32 dragonfile/__init__.py
+Zip file size: 3223 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat     4083 b- defN 23-Apr-22 04:56 dragonfile/__init__.py
 -rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-22 04:26 tests/__init__.py
--rw-rw-rw-  2.0 fat     1086 b- defN 23-Apr-22 04:36 dragonfile-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      773 b- defN 23-Apr-22 04:36 dragonfile-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 04:36 dragonfile-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Apr-22 04:36 dragonfile-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      550 b- defN 23-Apr-22 04:36 dragonfile-1.0.0.dist-info/RECORD
-7 files, 6571 bytes uncompressed, 2234 bytes compressed:  66.0%
+-rw-rw-rw-  2.0 fat     1086 b- defN 23-Apr-22 04:56 dragonfile-1.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      773 b- defN 23-Apr-22 04:56 dragonfile-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 04:56 dragonfile-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Apr-22 04:56 dragonfile-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      550 b- defN 23-Apr-22 04:56 dragonfile-1.0.1.dist-info/RECORD
+7 files, 6609 bytes uncompressed, 2243 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: dragonfile/__init__.py
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
-Filename: dragonfile-1.0.0.dist-info/LICENSE
+Filename: dragonfile-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: dragonfile-1.0.0.dist-info/METADATA
+Filename: dragonfile-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: dragonfile-1.0.0.dist-info/WHEEL
+Filename: dragonfile-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: dragonfile-1.0.0.dist-info/top_level.txt
+Filename: dragonfile-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: dragonfile-1.0.0.dist-info/RECORD
+Filename: dragonfile-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dragonfile/__init__.py

```diff
@@ -1,15 +1,16 @@
 import csv
 
 class dragonfile:
-    def __init__ (self, dFile, nColumn, dSep=",", coding="utf-8"):
+    def __init__ (self, dFile, nColumn, dSep=",", coding="utf-8", dictD={}):
         self.dFile = dFile
         self.nColumn = nColumn
         self.dSep = dSep
         self.coding = coding
+        self.dictD = dictD
     
     def readFile(self):
         columns = []
 
         with open(self.dFile, encoding=self.coding) as file:
             reader = csv.reader(file, delimiter=self.dSep)
             header = next(reader)
```

## Comparing `dragonfile-1.0.0.dist-info/LICENSE` & `dragonfile-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dragonfile-1.0.0.dist-info/METADATA` & `dragonfile-1.0.1.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfile
-Version: 1.0.0
+Version: 1.0.1
 Summary: Read CSV - Version Test
 Author: Gabriel Arantd Felipe
 Author-email: grantd.ctt@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `dragonfile-1.0.0.dist-info/RECORD` & `dragonfile-1.0.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-dragonfile/__init__.py,sha256=RfRWiLOwqi83HwEue11k_YhkXh47Po6t65pIKPqZ4sY,4045
+dragonfile/__init__.py,sha256=-d7yqScBK8gZ-gGv2lm0gXiNPj9FzlhNsRHU3lqnFM0,4083
 tests/__init__.py,sha256=_45vlcIypa2b18N8SC7zcRrUliWSOUQ-UBaMp1Pih7w,8
-dragonfile-1.0.0.dist-info/LICENSE,sha256=02eOcGvYICXgBPMIM3vlF_VGi_CiLCBR_vsDUpfZ1I4,1086
-dragonfile-1.0.0.dist-info/METADATA,sha256=kY1PrDFsZmv_VXbhnqR5VwOuNV26A1t6IpYmuDWdGyc,773
-dragonfile-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-dragonfile-1.0.0.dist-info/top_level.txt,sha256=8ckXgjHS0EofdYIFBWxygj6OaGisVypLa_ly4uRJIBc,17
-dragonfile-1.0.0.dist-info/RECORD,,
+dragonfile-1.0.1.dist-info/LICENSE,sha256=02eOcGvYICXgBPMIM3vlF_VGi_CiLCBR_vsDUpfZ1I4,1086
+dragonfile-1.0.1.dist-info/METADATA,sha256=AjD7p41N0PwOGOaN8LMOCakeNzYtoPHopxeRhQd-3LE,773
+dragonfile-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+dragonfile-1.0.1.dist-info/top_level.txt,sha256=8ckXgjHS0EofdYIFBWxygj6OaGisVypLa_ly4uRJIBc,17
+dragonfile-1.0.1.dist-info/RECORD,,
```

