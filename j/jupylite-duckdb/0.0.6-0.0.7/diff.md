# Comparing `tmp/jupylite_duckdb-0.0.6-py3-none-any.whl.zip` & `tmp/jupylite_duckdb-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5610 bytes, number of entries: 9
+Zip file size: 5611 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      128 b- defN 23-Apr-21 01:44 jupylite_duckdb/__init__.py
--rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-22 15:13 jupylite_duckdb/_version.py
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-22 15:17 jupylite_duckdb/_version.py
 -rw-rw-rw-  2.0 fat     8757 b- defN 23-Apr-22 15:13 jupylite_duckdb/jdw.py
 -rw-rw-rw-  2.0 fat      979 b- defN 23-Apr-22 14:33 jupylite_duckdb/magic.py
--rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-22 15:13 jupylite_duckdb-0.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1296 b- defN 23-Apr-22 15:13 jupylite_duckdb-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 15:13 jupylite_duckdb-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-22 15:13 jupylite_duckdb-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      750 b- defN 23-Apr-22 15:13 jupylite_duckdb-0.0.6.dist-info/RECORD
-9 files, 13534 bytes uncompressed, 4306 bytes compressed:  68.2%
+-rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-22 15:17 jupylite_duckdb-0.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1296 b- defN 23-Apr-22 15:17 jupylite_duckdb-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 15:17 jupylite_duckdb-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-22 15:17 jupylite_duckdb-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      750 b- defN 23-Apr-22 15:17 jupylite_duckdb-0.0.7.dist-info/RECORD
+9 files, 13534 bytes uncompressed, 4307 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: jupylite_duckdb/jdw.py
 Comment: 
 
 Filename: jupylite_duckdb/magic.py
 Comment: 
 
-Filename: jupylite_duckdb-0.0.6.dist-info/LICENSE
+Filename: jupylite_duckdb-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: jupylite_duckdb-0.0.6.dist-info/METADATA
+Filename: jupylite_duckdb-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: jupylite_duckdb-0.0.6.dist-info/WHEEL
+Filename: jupylite_duckdb-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: jupylite_duckdb-0.0.6.dist-info/top_level.txt
+Filename: jupylite_duckdb-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: jupylite_duckdb-0.0.6.dist-info/RECORD
+Filename: jupylite_duckdb-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jupylite_duckdb/_version.py

```diff
@@ -1 +1 @@
-__version__="0.0.6"
+__version__="0.0.7"
```

## Comparing `jupylite_duckdb-0.0.6.dist-info/LICENSE` & `jupylite_duckdb-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jupylite_duckdb-0.0.6.dist-info/METADATA` & `jupylite_duckdb-0.0.7.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupylite-duckdb
-Version: 0.0.6
+Version: 0.0.7
 Summary: Testing
 Home-page: https://github.com/iqmo-org/
 Author: iqmo
 Author-email: info@iqmo.com
 Keywords: jupyterlite duckdb wasm
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `jupylite_duckdb-0.0.6.dist-info/RECORD` & `jupylite_duckdb-0.0.7.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 jupylite_duckdb/__init__.py,sha256=-Z_P6KBbWKDsMsnvKal14k3bbGljgWmFQPEvz7zrLVU,128
-jupylite_duckdb/_version.py,sha256=niArccs46aAShkIemAhMOaWl6PSyU7kClcvLnu4wpOM,21
+jupylite_duckdb/_version.py,sha256=yVpnvh3CICAkroQTNidsV9p--h4xzLc0YVEAgibVefI,21
 jupylite_duckdb/jdw.py,sha256=dqy0jOx65GV3mXGG7NlFKKQ6BZQ5_qzmbZ3i622nWL8,8757
 jupylite_duckdb/magic.py,sha256=okWgdHbcu0ul2BOYNdu9NHwRSoyAG_0m6RiGnw2Bj_k,979
-jupylite_duckdb-0.0.6.dist-info/LICENSE,sha256=WJMtiY9u9JD8FJ18a6_psLMXvrOIA7F-mYphCuyGFvw,1495
-jupylite_duckdb-0.0.6.dist-info/METADATA,sha256=Ka30J24ChI7_tyo8Co63KjwNWMCxX6Jun9IjNBD21lA,1296
-jupylite_duckdb-0.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-jupylite_duckdb-0.0.6.dist-info/top_level.txt,sha256=y1GybQE7FyRTQPGLf2lE9dStC--h8ZozxhgXQRxz490,16
-jupylite_duckdb-0.0.6.dist-info/RECORD,,
+jupylite_duckdb-0.0.7.dist-info/LICENSE,sha256=WJMtiY9u9JD8FJ18a6_psLMXvrOIA7F-mYphCuyGFvw,1495
+jupylite_duckdb-0.0.7.dist-info/METADATA,sha256=53sLQb1U65EBTGFvgGkLCiz5HIAiRbgV4P8UDYQn8p8,1296
+jupylite_duckdb-0.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+jupylite_duckdb-0.0.7.dist-info/top_level.txt,sha256=y1GybQE7FyRTQPGLf2lE9dStC--h8ZozxhgXQRxz490,16
+jupylite_duckdb-0.0.7.dist-info/RECORD,,
```

