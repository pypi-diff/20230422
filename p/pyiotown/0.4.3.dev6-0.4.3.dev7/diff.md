# Comparing `tmp/pyiotown-0.4.3.dev6-py3-none-any.whl.zip` & `tmp/pyiotown-0.4.3.dev7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6639 bytes, number of entries: 10
+Zip file size: 6660 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-05 08:55 pyiotown/__init__.py
 -rw-r--r--  2.0 unx     3416 b- defN 23-Apr-18 05:32 pyiotown/get.py
 -rw-r--r--  2.0 unx     3794 b- defN 23-Apr-18 05:32 pyiotown/post.py
--rw-r--r--  2.0 unx     6794 b- defN 23-Apr-18 05:57 pyiotown/post_process.py
--rw-r--r--  2.0 unx     1053 b- defN 23-Apr-18 06:00 pyiotown-0.4.3.dev6.dist-info/LICENSE
--rw-r--r--  2.0 unx      693 b- defN 23-Apr-18 06:00 pyiotown-0.4.3.dev6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 06:00 pyiotown-0.4.3.dev6.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Apr-18 06:00 pyiotown-0.4.3.dev6.dist-info/pbr.json
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-18 06:00 pyiotown-0.4.3.dev6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      807 b- defN 23-Apr-18 06:00 pyiotown-0.4.3.dev6.dist-info/RECORD
-10 files, 16705 bytes uncompressed, 5253 bytes compressed:  68.6%
+-rw-r--r--  2.0 unx     6865 b- defN 23-Apr-22 06:39 pyiotown/post_process.py
+-rw-r--r--  2.0 unx     1053 b- defN 23-Apr-22 06:41 pyiotown-0.4.3.dev7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      693 b- defN 23-Apr-22 06:41 pyiotown-0.4.3.dev7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 06:41 pyiotown-0.4.3.dev7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Apr-22 06:41 pyiotown-0.4.3.dev7.dist-info/pbr.json
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-22 06:41 pyiotown-0.4.3.dev7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      807 b- defN 23-Apr-22 06:41 pyiotown-0.4.3.dev7.dist-info/RECORD
+10 files, 16776 bytes uncompressed, 5274 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: pyiotown/post.py
 Comment: 
 
 Filename: pyiotown/post_process.py
 Comment: 
 
-Filename: pyiotown-0.4.3.dev6.dist-info/LICENSE
+Filename: pyiotown-0.4.3.dev7.dist-info/LICENSE
 Comment: 
 
-Filename: pyiotown-0.4.3.dev6.dist-info/METADATA
+Filename: pyiotown-0.4.3.dev7.dist-info/METADATA
 Comment: 
 
-Filename: pyiotown-0.4.3.dev6.dist-info/WHEEL
+Filename: pyiotown-0.4.3.dev7.dist-info/WHEEL
 Comment: 
 
-Filename: pyiotown-0.4.3.dev6.dist-info/pbr.json
+Filename: pyiotown-0.4.3.dev7.dist-info/pbr.json
 Comment: 
 
-Filename: pyiotown-0.4.3.dev6.dist-info/top_level.txt
+Filename: pyiotown-0.4.3.dev7.dist-info/top_level.txt
 Comment: 
 
-Filename: pyiotown-0.4.3.dev6.dist-info/RECORD
+Filename: pyiotown-0.4.3.dev7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyiotown/post_process.py

```diff
@@ -40,15 +40,15 @@
             client.publish('iotown/proc-done', json.dumps(message), 1)
         return
 
     if userdata['dry'] == True:
         result = None
     
     if type(result) is dict and 'data' in result.keys():
-        result = post_files(result, userdata['url'], userdata['token'])
+        result = post_files(result, userdata['url'], userdata['token'], userdata['verify'])
         message['data'] = result['data']
         client.publish('iotown/proc-done', json.dumps(message), 1)
     elif result is None:
         print(f"Discard the message")
     else:
         print(f"CALLBACK FUNCTION TYPE ERROR {type(result)} must [ dict ]", file=sys.stderr)
         client.publish('iotown/proc-done', msg.payload, 1)
@@ -119,14 +119,15 @@
     client.on_message = on_message
     client.user_data_set({
         "url": url,
         "token": token,
         "func": func,
         "group": group,
         "name": name,
+        "verify": verify,
         "dry": dry_run,
     })
 
     if mqtt_url is None:
         mqtt_host = urlparse(url).hostname
         mqtt_port = 8883
 
@@ -171,14 +172,15 @@
     client.on_message = on_message
     client.user_data_set({
         "url": url,
         "token": token,
         "func": func,
         "group": "common",
         "name": topic,
+        "verify": False,
         "dry": dry_run,
     })
 
     if mqtt_url is None:
         mqtt_host = urlparse(url).hostname
         mqtt_port = 8883
     else:
```

## Comparing `pyiotown-0.4.3.dev6.dist-info/LICENSE` & `pyiotown-0.4.3.dev7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyiotown-0.4.3.dev6.dist-info/METADATA` & `pyiotown-0.4.3.dev7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiotown
-Version: 0.4.3.dev6
+Version: 0.4.3.dev7
 Summary: IoT.own Library
 Home-page: https://github.com/CoXlabInc/pyiotow
 Author: CoXlab Inc.
 Author-email: support@coxlab.kr
 Maintainer: Jongsoo Jeong
 Maintainer-email: jsjeong@coxlab.k
 License: MIT
```

## Comparing `pyiotown-0.4.3.dev6.dist-info/RECORD` & `pyiotown-0.4.3.dev7.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pyiotown/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyiotown/get.py,sha256=025Eg17ZnS2VttWiaNgc-6lz1eaKRFsj5kz6hJxMh3U,3416
 pyiotown/post.py,sha256=qdeb2G74anHc8ceymjSSQ7ZnNpO1iQMFghbWYjbj2ms,3794
-pyiotown/post_process.py,sha256=4xUmshk-s5x-slaKMfSKuAoLjas79jr1nHDoHWv7dQY,6794
-pyiotown-0.4.3.dev6.dist-info/LICENSE,sha256=hf-g3asB2eVCMfAdxFSFlGUmBqk8KhH3U04FUvwOFGU,1053
-pyiotown-0.4.3.dev6.dist-info/METADATA,sha256=TStArJIBGoVxMeGhEICf836Fh_vKvtOt1_vFu4C2OZ0,693
-pyiotown-0.4.3.dev6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyiotown-0.4.3.dev6.dist-info/pbr.json,sha256=NVi9f5uTIbn6SHsiDiF3mx5vEBJc5hnFM8BeQldYstI,47
-pyiotown-0.4.3.dev6.dist-info/top_level.txt,sha256=7C_yB2E4KedHWqWClKpbaMmv2nYswwQ19MHhsBDr6kk,9
-pyiotown-0.4.3.dev6.dist-info/RECORD,,
+pyiotown/post_process.py,sha256=p4_XO0NDPd0Q3csHIbsXh4_XO3splFI8gMy33li6n9U,6865
+pyiotown-0.4.3.dev7.dist-info/LICENSE,sha256=hf-g3asB2eVCMfAdxFSFlGUmBqk8KhH3U04FUvwOFGU,1053
+pyiotown-0.4.3.dev7.dist-info/METADATA,sha256=x77a64d3itDnT3PzvbK6GwBWbKw4I8kLC18SUrRgv74,693
+pyiotown-0.4.3.dev7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyiotown-0.4.3.dev7.dist-info/pbr.json,sha256=kc6ciLY88_Yu39zFSPymNBFrUwpb9p90BPvr6VtpTyo,47
+pyiotown-0.4.3.dev7.dist-info/top_level.txt,sha256=7C_yB2E4KedHWqWClKpbaMmv2nYswwQ19MHhsBDr6kk,9
+pyiotown-0.4.3.dev7.dist-info/RECORD,,
```

