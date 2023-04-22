# Comparing `tmp/xhs-0.1.3.tar.gz` & `tmp/xhs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhs-0.1.3.tar", last modified: Sat Apr 15 14:43:28 2023, max compression
+gzip compressed data, was "xhs-0.1.4.tar", last modified: Sat Apr 22 15:40:18 2023, max compression
```

## Comparing `xhs-0.1.3.tar` & `xhs-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:43:28.262915 xhs-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-15 14:43:16.000000 xhs-0.1.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-15 14:43:16.000000 xhs-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 14:43:16.000000 xhs-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-15 14:43:28.262915 xhs-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-15 14:43:16.000000 xhs-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-15 14:43:16.000000 xhs-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-15 14:43:28.262915 xhs-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-15 14:43:16.000000 xhs-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:43:28.262915 xhs-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-15 14:43:16.000000 xhs-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-15 14:43:16.000000 xhs-0.1.3/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-15 14:43:16.000000 xhs-0.1.3/tests/test_xhs.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-15 14:43:16.000000 xhs-0.1.3/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:43:28.262915 xhs-0.1.3/xhs/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-15 14:43:16.000000 xhs-0.1.3/xhs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-15 14:43:16.000000 xhs-0.1.3/xhs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19541 2023-04-15 14:43:16.000000 xhs-0.1.3/xhs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 14:43:16.000000 xhs-0.1.3/xhs/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-15 14:43:16.000000 xhs-0.1.3/xhs/help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:43:28.262915 xhs-0.1.3/xhs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-15 14:43:28.000000 xhs-0.1.3/xhs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-15 14:43:28.000000 xhs-0.1.3/xhs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 14:43:28.000000 xhs-0.1.3/xhs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 14:43:28.000000 xhs-0.1.3/xhs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 14:43:28.000000 xhs-0.1.3/xhs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 14:43:28.000000 xhs-0.1.3/xhs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:40:18.186189 xhs-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-22 15:40:06.000000 xhs-0.1.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-22 15:40:06.000000 xhs-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-22 15:40:06.000000 xhs-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-22 15:40:18.186189 xhs-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-22 15:40:06.000000 xhs-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-22 15:40:06.000000 xhs-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-22 15:40:18.186189 xhs-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-22 15:40:06.000000 xhs-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:40:18.186189 xhs-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-22 15:40:06.000000 xhs-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-22 15:40:06.000000 xhs-0.1.4/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-22 15:40:06.000000 xhs-0.1.4/tests/test_xhs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-22 15:40:06.000000 xhs-0.1.4/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:40:18.186189 xhs-0.1.4/xhs/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-22 15:40:06.000000 xhs-0.1.4/xhs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-22 15:40:06.000000 xhs-0.1.4/xhs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20070 2023-04-22 15:40:06.000000 xhs-0.1.4/xhs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-22 15:40:06.000000 xhs-0.1.4/xhs/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-22 15:40:06.000000 xhs-0.1.4/xhs/help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:40:18.186189 xhs-0.1.4/xhs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-22 15:40:18.000000 xhs-0.1.4/xhs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-22 15:40:18.000000 xhs-0.1.4/xhs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 15:40:18.000000 xhs-0.1.4/xhs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 15:40:18.000000 xhs-0.1.4/xhs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-22 15:40:18.000000 xhs-0.1.4/xhs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-22 15:40:18.000000 xhs-0.1.4/xhs.egg-info/top_level.txt
```

### Comparing `xhs-0.1.3/CHANGELOG.md` & `xhs-0.1.4/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 ## dev
 
 - Improve documentation
 - Add more test function
 
+## 0.1.4
+
+### ADD
+
+- add get user like notes
+- add get user collect notes
+
 ## 0.1.3
 
 ### ADD
 
 - add get note comments
 - add get note sub comments
 - add get note all comments
```

### Comparing `xhs-0.1.3/LICENSE` & `xhs-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xhs-0.1.3/PKG-INFO` & `xhs-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.1.3
+Version: 0.1.4
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xhs-0.1.3/README.md` & `xhs-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `xhs-0.1.3/setup.py` & `xhs-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.3/tests/test_help.py` & `xhs-0.1.4/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.3/tests/test_xhs.py` & `xhs-0.1.4/tests/test_xhs.py`

 * *Files 10% similar despite different names*

```diff
@@ -148,7 +148,23 @@
 @pytest.mark.parametrize("note_id", [
     "639a7064000000001f0098a8",
     "635d06790000000015020497"
 ])
 @pytest.mark.skip()
 def test_save_files_from_note_id_invalid_title(xhs_client: XhsClient, note_id):
     xhs_client.save_files_from_note_id(note_id, r"C:\Users\ReaJason\Desktop")
+
+
+# @pytest.mark.skip()
+def test_get_user_collect_notes(xhs_client: XhsClient):
+    notes = xhs_client.get_user_collect_notes(
+        user_id="63273a77000000002303cc9b")["notes"]
+    beauty_print(notes)
+    assert len(notes) == 1
+
+
+# @pytest.mark.skip()
+def test_get_user_like_notes(xhs_client: XhsClient):
+    notes = xhs_client.get_user_like_notes(
+        user_id="63273a77000000002303cc9b")["notes"]
+    beauty_print(notes)
+    assert len(notes) == 2
```

### Comparing `xhs-0.1.3/xhs/core.py` & `xhs-0.1.4/xhs/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 
         new_dir_path = os.path.join(dir_path, title)
         if not os.path.exists(new_dir_path):
             os.mkdir(new_dir_path)
 
         if note["type"] == NoteType.VIDEO.value:
             video_url = self._get_video_url_from_note(note)
-            video_filename = os.path.join(new_dir_path, f"{title}.mp4")
+            video_filename = os.path.join(new_dir_path, f"{title}.mov")
             download_file(video_url, video_filename)
         else:
             img_urls = self._get_img_urls_from_note(note)
             for index, img_url in enumerate(img_urls):
                 img_file_name = os.path.join(new_dir_path, f"{title}{index}.png")
                 download_file(img_url, img_file_name)
 
@@ -228,16 +228,15 @@
         :param note: note info
         :type note: dict
         :return: video url
         :rtype: str
         """
         if not note.get("video"):
             return ""
-        video = next(filter(lambda value: len(value), note["video"]["media"]["stream"].values()))[0]
-        return video["master_url"]
+        return f"http://sns-video-bd.xhscdn.com/{note['video']['consumer']['origin_video_key']}"
 
     def get_self_info(self):
         uri = "/api/sns/web/v1/user/selfinfo"
         res = self.get(uri)
         return res
 
     def get_user_info(self, user_id: str):
@@ -538,7 +537,25 @@
     def check_qrcode(self, qr_id: str, code: str):
         uri = "/api/sns/web/v1/login/qrcode/status"
         params = {
             "qr_id": qr_id,
             "code": code
         }
         return self.get(uri, params)
+
+    def get_user_collect_notes(self, user_id: str, num: int = 30, cursor: str = ""):
+        uri = "/api/sns/web/v2/note/collect/page"
+        params = {
+            "user_id": user_id,
+            "num": num,
+            "cursor": cursor
+        }
+        return self.get(uri, params)
+
+    def get_user_like_notes(self, user_id: str, num: int = 30, cursor: str = ""):
+        uri = "/api/sns/web/v1/note/like/page"
+        params = {
+            "user_id": user_id,
+            "num": num,
+            "cursor": cursor
+        }
+        return self.get(uri, params)
```

### Comparing `xhs-0.1.3/xhs/help.py` & `xhs-0.1.4/xhs/help.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.3/xhs.egg-info/PKG-INFO` & `xhs-0.1.4/xhs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.1.3
+Version: 0.1.4
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
```

