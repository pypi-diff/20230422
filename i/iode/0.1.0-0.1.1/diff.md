# Comparing `tmp/iode-0.1.0-py3-none-any.whl.zip` & `tmp/iode-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4153 bytes, number of entries: 8
+Zip file size: 4154 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat       19 b- defN 23-Apr-22 14:43 iode/__init__.py
--rw-rw-rw-  2.0 fat     4369 b- defN 23-Apr-22 15:09 iode/iode.py
--rw-rw-rw-  2.0 fat     1081 b- defN 23-Apr-22 15:10 iode-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2148 b- defN 23-Apr-22 15:10 iode-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 15:10 iode-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       41 b- defN 23-Apr-22 15:10 iode-0.1.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-22 15:10 iode-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      602 b- defN 23-Apr-22 15:10 iode-0.1.0.dist-info/RECORD
-8 files, 8357 bytes uncompressed, 3105 bytes compressed:  62.8%
+-rw-rw-rw-  2.0 fat     4373 b- defN 23-Apr-22 15:11 iode/iode.py
+-rw-rw-rw-  2.0 fat     1081 b- defN 23-Apr-22 15:11 iode-0.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2148 b- defN 23-Apr-22 15:11 iode-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 15:11 iode-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       41 b- defN 23-Apr-22 15:11 iode-0.1.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-22 15:11 iode-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      602 b- defN 23-Apr-22 15:11 iode-0.1.1.dist-info/RECORD
+8 files, 8361 bytes uncompressed, 3106 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: iode/__init__.py
 Comment: 
 
 Filename: iode/iode.py
 Comment: 
 
-Filename: iode-0.1.0.dist-info/LICENSE
+Filename: iode-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: iode-0.1.0.dist-info/METADATA
+Filename: iode-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: iode-0.1.0.dist-info/WHEEL
+Filename: iode-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: iode-0.1.0.dist-info/entry_points.txt
+Filename: iode-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: iode-0.1.0.dist-info/top_level.txt
+Filename: iode-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: iode-0.1.0.dist-info/RECORD
+Filename: iode-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iode/iode.py

```diff
@@ -5,15 +5,15 @@
 # Created Date: Aug 10, 2021
 # =============================================================================
 import os
 import shutil
 import argparse
 import configparser
 
-version = '0.1.0'
+version = '0.1.1'
 
 iode_run_cmd = 'code' # 'code' or 'code-insider' 
 iode_dir_path = os.path.join(os.path.expanduser('~'), '.iode')
 iode_conf_path = os.path.join(os.path.expanduser('~'), '.iodeconfig')
 
 def _list(args):
     global iode_dir_path
@@ -103,16 +103,16 @@
         with open(iode_conf_path, "w") as fp:
             config_parser.write(fp)
     else:
         config_parser = configparser.ConfigParser()
         config_parser.read(iode_conf_path)
         iode_run_cmd = config_parser['setting']['iode_run']
         iode_dir_path = config_parser['setting']['iode_dir']
-        print(f'run_cmd = {iode_run_cmd}')
-        print(f'dir_path = {iode_dir_path}')
+        # print(f'run_cmd = {iode_run_cmd}')
+        # print(f'dir_path = {iode_dir_path}')
   
     if not os.path.exists(iode_dir_path):
         os.makedirs(iode_dir_path)
     
     arg_parser = argparse.ArgumentParser()
     arg_parser.add_argument('-v', '--version', action='version', version=f'IODE v{version}')
```

## Comparing `iode-0.1.0.dist-info/LICENSE` & `iode-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `iode-0.1.0.dist-info/METADATA` & `iode-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iode
-Version: 0.1.0
+Version: 0.1.1
 Summary: Isolate your vscode environment and keep it simple!
 Home-page: https://github.com/jugangdae/iode
 Author: Gangdae Ju
 Author-email: jugangdae@gamil.com
 License: MIT
 Keywords: iode,manage,isolated,vscode,environment,simple,cli,tool
 Platform: UNKNOWN
```

## Comparing `iode-0.1.0.dist-info/RECORD` & `iode-0.1.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 iode/__init__.py,sha256=ZuzR5pXkT9jOgkKLn-qfqOjClOaA6uM73tuWsWqdqaA,19
-iode/iode.py,sha256=ltbdj5LEXW6rrvdgOiIU7LLHsMvQh14j77eOMsIQWuw,4369
-iode-0.1.0.dist-info/LICENSE,sha256=fruW1UBnviAjamLyt_7ulIZcaYZhv8bJ170H2Q7sTOk,1081
-iode-0.1.0.dist-info/METADATA,sha256=671UopFfnn_E97zupcxh6tTbK1_ZCuPkLircCSRog3c,2148
-iode-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-iode-0.1.0.dist-info/entry_points.txt,sha256=weNuBGfvg0bzpAtol0fmrJphH0cO-rcLKGypYiLbMzo,41
-iode-0.1.0.dist-info/top_level.txt,sha256=IMEMaDgAA7knwFgUlWf-9ZOzQWizYC4tCVaecumz-kA,5
-iode-0.1.0.dist-info/RECORD,,
+iode/iode.py,sha256=eCppVjOL47FLZbR64J2Cuf6tDxWdwTtnR5tS6dCiRGw,4373
+iode-0.1.1.dist-info/LICENSE,sha256=fruW1UBnviAjamLyt_7ulIZcaYZhv8bJ170H2Q7sTOk,1081
+iode-0.1.1.dist-info/METADATA,sha256=f_be27RgBrFNYBfiuAjEP6ZHx8j-eSqWPBkxIbQxr40,2148
+iode-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+iode-0.1.1.dist-info/entry_points.txt,sha256=weNuBGfvg0bzpAtol0fmrJphH0cO-rcLKGypYiLbMzo,41
+iode-0.1.1.dist-info/top_level.txt,sha256=IMEMaDgAA7knwFgUlWf-9ZOzQWizYC4tCVaecumz-kA,5
+iode-0.1.1.dist-info/RECORD,,
```

