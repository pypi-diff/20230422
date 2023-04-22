# Comparing `tmp/jupylite_duckdb-0.0.8-py3-none-any.whl.zip` & `tmp/jupylite_duckdb-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6292 bytes, number of entries: 10
+Zip file size: 6289 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat      128 b- defN 23-Apr-21 01:44 jupylite_duckdb/__init__.py
--rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-22 15:25 jupylite_duckdb/_version.py
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-22 15:30 jupylite_duckdb/_version.py
 -rw-rw-rw-  2.0 fat     8758 b- defN 23-Apr-22 15:22 jupylite_duckdb/jdw.py
--rw-rw-rw-  2.0 fat     1040 b- defN 23-Apr-22 15:25 jupylite_duckdb/jdw_magic.py
+-rw-rw-rw-  2.0 fat     1040 b- defN 23-Apr-22 15:29 jupylite_duckdb/jdw_magic.py
 -rw-rw-rw-  2.0 fat      979 b- defN 23-Apr-22 14:33 jupylite_duckdb/magic.py
--rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-22 15:25 jupylite_duckdb-0.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1323 b- defN 23-Apr-22 15:25 jupylite_duckdb-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 15:25 jupylite_duckdb-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-22 15:25 jupylite_duckdb-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      835 b- defN 23-Apr-22 15:25 jupylite_duckdb-0.0.8.dist-info/RECORD
-10 files, 14687 bytes uncompressed, 4856 bytes compressed:  66.9%
+-rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-22 15:30 jupylite_duckdb-0.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1323 b- defN 23-Apr-22 15:30 jupylite_duckdb-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 15:30 jupylite_duckdb-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-22 15:30 jupylite_duckdb-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      835 b- defN 23-Apr-22 15:30 jupylite_duckdb-0.0.9.dist-info/RECORD
+10 files, 14687 bytes uncompressed, 4853 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: jupylite_duckdb/jdw_magic.py
 Comment: 
 
 Filename: jupylite_duckdb/magic.py
 Comment: 
 
-Filename: jupylite_duckdb-0.0.8.dist-info/LICENSE
+Filename: jupylite_duckdb-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: jupylite_duckdb-0.0.8.dist-info/METADATA
+Filename: jupylite_duckdb-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: jupylite_duckdb-0.0.8.dist-info/WHEEL
+Filename: jupylite_duckdb-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: jupylite_duckdb-0.0.8.dist-info/top_level.txt
+Filename: jupylite_duckdb-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: jupylite_duckdb-0.0.8.dist-info/RECORD
+Filename: jupylite_duckdb-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jupylite_duckdb/_version.py

```diff
@@ -1 +1 @@
-__version__="0.0.8"
+__version__="0.0.9"
```

## Comparing `jupylite_duckdb-0.0.8.dist-info/LICENSE` & `jupylite_duckdb-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jupylite_duckdb-0.0.8.dist-info/METADATA` & `jupylite_duckdb-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupylite-duckdb
-Version: 0.0.8
+Version: 0.0.9
 Summary: Testing
 Home-page: https://github.com/iqmo-org/
 Author: iqmo
 Author-email: info@iqmo.com
 Keywords: jupyterlite duckdb wasm
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `jupylite_duckdb-0.0.8.dist-info/RECORD` & `jupylite_duckdb-0.0.9.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 jupylite_duckdb/__init__.py,sha256=-Z_P6KBbWKDsMsnvKal14k3bbGljgWmFQPEvz7zrLVU,128
-jupylite_duckdb/_version.py,sha256=W7a04jdOnTfeGJknta42tPwNi1GSvvq850YgU9hC9Mw,21
+jupylite_duckdb/_version.py,sha256=-on8kltkEYjKmDF-4wTSGQBIMW_PSbpQaefFmKIAaiE,21
 jupylite_duckdb/jdw.py,sha256=A70AWJ3dYWuK0bQy1OR72tOUUQp6SPbCNGrdFRk_ORE,8758
 jupylite_duckdb/jdw_magic.py,sha256=j_uca93dDtk4LpJHbxAvR124XICQQVD0q3BpdlgfX18,1040
 jupylite_duckdb/magic.py,sha256=okWgdHbcu0ul2BOYNdu9NHwRSoyAG_0m6RiGnw2Bj_k,979
-jupylite_duckdb-0.0.8.dist-info/LICENSE,sha256=WJMtiY9u9JD8FJ18a6_psLMXvrOIA7F-mYphCuyGFvw,1495
-jupylite_duckdb-0.0.8.dist-info/METADATA,sha256=iYoGcVRun_trCOE_T-6heFiXqhzzVuGMoHGc4woC2fc,1323
-jupylite_duckdb-0.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-jupylite_duckdb-0.0.8.dist-info/top_level.txt,sha256=y1GybQE7FyRTQPGLf2lE9dStC--h8ZozxhgXQRxz490,16
-jupylite_duckdb-0.0.8.dist-info/RECORD,,
+jupylite_duckdb-0.0.9.dist-info/LICENSE,sha256=WJMtiY9u9JD8FJ18a6_psLMXvrOIA7F-mYphCuyGFvw,1495
+jupylite_duckdb-0.0.9.dist-info/METADATA,sha256=rkpXarbcELh3SCpeg_xSbtxJtHH9YCgbmM98f5HuzUc,1323
+jupylite_duckdb-0.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+jupylite_duckdb-0.0.9.dist-info/top_level.txt,sha256=y1GybQE7FyRTQPGLf2lE9dStC--h8ZozxhgXQRxz490,16
+jupylite_duckdb-0.0.9.dist-info/RECORD,,
```

