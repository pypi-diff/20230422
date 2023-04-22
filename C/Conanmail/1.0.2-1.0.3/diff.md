# Comparing `tmp/Conanmail-1.0.2-py3-none-any.whl.zip` & `tmp/Conanmail-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 4718 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat     1502 b- defN 23-Apr-21 19:13 conan/IMAP.json
 -rw-rw-rw-  2.0 fat      800 b- defN 23-Apr-22 20:29 conan/config.py
 -rw-rw-rw-  2.0 fat     1027 b- defN 23-Apr-22 20:29 conan/main.py
 -rw-rw-rw-  2.0 fat     5435 b- defN 23-Apr-22 20:30 conan/utils.py
--rw-rw-rw-  2.0 fat      308 b- defN 23-Apr-22 21:09 Conanmail-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 21:09 Conanmail-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       42 b- defN 23-Apr-22 21:09 Conanmail-1.0.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-22 21:09 Conanmail-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      685 b- defN 23-Apr-22 21:09 Conanmail-1.0.2.dist-info/RECORD
+-rw-rw-rw-  2.0 fat      308 b- defN 23-Apr-22 21:16 Conanmail-1.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 21:16 Conanmail-1.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       42 b- defN 23-Apr-22 21:16 Conanmail-1.0.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-22 21:16 Conanmail-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      685 b- defN 23-Apr-22 21:16 Conanmail-1.0.3.dist-info/RECORD
 9 files, 9897 bytes uncompressed, 3542 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: conan/main.py
 Comment: 
 
 Filename: conan/utils.py
 Comment: 
 
-Filename: Conanmail-1.0.2.dist-info/METADATA
+Filename: Conanmail-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: Conanmail-1.0.2.dist-info/WHEEL
+Filename: Conanmail-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: Conanmail-1.0.2.dist-info/entry_points.txt
+Filename: Conanmail-1.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: Conanmail-1.0.2.dist-info/top_level.txt
+Filename: Conanmail-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: Conanmail-1.0.2.dist-info/RECORD
+Filename: Conanmail-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `Conanmail-1.0.2.dist-info/RECORD` & `Conanmail-1.0.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 conan/IMAP.json,sha256=yuuSZctIhU2_w4ETO5xMk-U9W_md5ujuXyFMs4GDREM,1502
 conan/config.py,sha256=L00BaYVpffndVIj26Nefvy5CkolGMSHBJYBXSyRKk9E,800
 conan/main.py,sha256=bfSOriG8qtjUqQYUfS7DY6ie_ECq-Bex_QX-3uS45oE,1027
 conan/utils.py,sha256=ZYf0LOezFoFZiWFADhwB5hMWvprnEwjFyKmzekovLo0,5435
-Conanmail-1.0.2.dist-info/METADATA,sha256=6O-p8Ja4pdG90Xp6h6XeuG_P_g3mYUSegfsLXT4Qagg,308
-Conanmail-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-Conanmail-1.0.2.dist-info/entry_points.txt,sha256=3UrXVyVTgZifIQHDrU5mSfB2HUponF5XrT6ZPbUK5Zk,42
-Conanmail-1.0.2.dist-info/top_level.txt,sha256=sM4lgXKfCbokMqE3Up5iIqdHl_SXyHTxz_scRtSarSw,6
-Conanmail-1.0.2.dist-info/RECORD,,
+Conanmail-1.0.3.dist-info/METADATA,sha256=suRR1HYFg9Y-d0R1zNj1dAuR4cpwVW94ry-vC1oST0o,308
+Conanmail-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+Conanmail-1.0.3.dist-info/entry_points.txt,sha256=3UrXVyVTgZifIQHDrU5mSfB2HUponF5XrT6ZPbUK5Zk,42
+Conanmail-1.0.3.dist-info/top_level.txt,sha256=sM4lgXKfCbokMqE3Up5iIqdHl_SXyHTxz_scRtSarSw,6
+Conanmail-1.0.3.dist-info/RECORD,,
```

