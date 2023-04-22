# Comparing `tmp/ripandtear-0.9.3.tar.gz` & `tmp/ripandtear-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ripandtear-0.9.3.tar", last modified: Tue Apr 11 15:17:30 2023, max compression
+gzip compressed data, was "ripandtear-0.9.4.tar", last modified: Sat Apr 22 16:04:06 2023, max compression
```

## Comparing `ripandtear-0.9.3.tar` & `ripandtear-0.9.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-11 15:17:30.308816 ripandtear-0.9.3/
--rw-rw-r--   0 beard     (1000) beard     (1000)    35064 2023-02-18 23:42:30.000000 ripandtear-0.9.3/LICENSE
--rw-rw-r--   0 beard     (1000) beard     (1000)    16917 2023-04-11 15:17:30.308816 ripandtear-0.9.3/PKG-INFO
--rw-rw-r--   0 beard     (1000) beard     (1000)    16527 2023-02-28 03:34:50.000000 ripandtear-0.9.3/README.md
--rw-rw-r--   0 beard     (1000) beard     (1000)       90 2023-02-20 00:52:42.000000 ripandtear-0.9.3/pyproject.toml
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-11 15:17:30.300816 ripandtear-0.9.3/ripandtear/
--rw-rw-r--   0 beard     (1000) beard     (1000)       22 2023-03-09 22:35:04.000000 ripandtear-0.9.3/ripandtear/__init__.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8025 2023-02-28 02:57:32.000000 ripandtear-0.9.3/ripandtear/__main__.py
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-11 15:17:30.304816 ripandtear-0.9.3/ripandtear/extractors/
--rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 22:50:13.000000 ripandtear-0.9.3/ripandtear/extractors/__init__.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    13425 2023-04-02 21:19:42.000000 ripandtear-0.9.3/ripandtear/extractors/bunkr.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8646 2023-02-28 02:57:32.000000 ripandtear-0.9.3/ripandtear/extractors/common.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6740 2023-03-20 18:38:53.000000 ripandtear-0.9.3/ripandtear/extractors/coomer.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     5143 2023-04-02 22:53:26.000000 ripandtear-0.9.3/ripandtear/extractors/cyberdrop.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2451 2023-03-12 23:21:36.000000 ripandtear-0.9.3/ripandtear/extractors/gfycat.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     5370 2023-03-12 23:22:37.000000 ripandtear-0.9.3/ripandtear/extractors/gofile.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     7926 2023-03-12 23:23:07.000000 ripandtear-0.9.3/ripandtear/extractors/imgur.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8128 2023-04-02 19:55:36.000000 ripandtear-0.9.3/ripandtear/extractors/jpg.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    18471 2023-03-31 03:36:45.000000 ripandtear-0.9.3/ripandtear/extractors/reddit.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6506 2023-03-12 16:08:32.000000 ripandtear-0.9.3/ripandtear/extractors/redgifs.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6065 2023-03-12 23:25:25.000000 ripandtear-0.9.3/ripandtear/extractors/tiktits.py
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-11 15:17:30.308816 ripandtear-0.9.3/ripandtear/utils/
--rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 04:04:14.000000 ripandtear-0.9.3/ripandtear/utils/__init__.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    10060 2023-02-28 02:57:32.000000 ripandtear-0.9.3/ripandtear/utils/cli_arguments.py
--rw-rw-r--   0 beard     (1000) beard     (1000)      708 2023-02-27 19:25:42.000000 ripandtear-0.9.3/ripandtear/utils/color.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6767 2023-04-02 18:45:08.000000 ripandtear-0.9.3/ripandtear/utils/conductor.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     7198 2023-03-02 23:14:20.000000 ripandtear-0.9.3/ripandtear/utils/content_finder.py
--rw-rw-r--   0 beard     (1000) beard     (1000)      870 2023-02-27 19:25:42.000000 ripandtear-0.9.3/ripandtear/utils/custom_types.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8474 2023-04-02 04:30:56.000000 ripandtear-0.9.3/ripandtear/utils/downloader.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2847 2023-02-20 00:52:42.000000 ripandtear-0.9.3/ripandtear/utils/file_hasher.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2369 2023-03-12 15:20:35.000000 ripandtear-0.9.3/ripandtear/utils/file_sorter.py
--rw-rw-r--   0 beard     (1000) beard     (1000)      467 2023-02-27 19:25:42.000000 ripandtear-0.9.3/ripandtear/utils/logger.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2196 2023-02-27 19:25:42.000000 ripandtear-0.9.3/ripandtear/utils/progress.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    11036 2023-02-28 02:58:35.000000 ripandtear-0.9.3/ripandtear/utils/rat_info.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     4775 2023-02-27 19:25:42.000000 ripandtear-0.9.3/ripandtear/utils/rat_interaction.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     4961 2023-04-02 05:10:23.000000 ripandtear-0.9.3/ripandtear/utils/tracker.py
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-11 15:17:30.300816 ripandtear-0.9.3/ripandtear.egg-info/
--rw-rw-r--   0 beard     (1000) beard     (1000)    16917 2023-04-11 15:17:30.000000 ripandtear-0.9.3/ripandtear.egg-info/PKG-INFO
--rw-rw-r--   0 beard     (1000) beard     (1000)     1111 2023-04-11 15:17:30.000000 ripandtear-0.9.3/ripandtear.egg-info/SOURCES.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)        1 2023-04-11 15:17:30.000000 ripandtear-0.9.3/ripandtear.egg-info/dependency_links.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)       58 2023-04-11 15:17:30.000000 ripandtear-0.9.3/ripandtear.egg-info/entry_points.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)      405 2023-04-11 15:17:30.000000 ripandtear-0.9.3/ripandtear.egg-info/requires.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)       11 2023-04-11 15:17:30.000000 ripandtear-0.9.3/ripandtear.egg-info/top_level.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)     1058 2023-04-11 15:17:30.308816 ripandtear-0.9.3/setup.cfg
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 16:04:06.606638 ripandtear-0.9.4/
+-rw-rw-r--   0 beard     (1000) beard     (1000)    35064 2023-02-18 23:42:30.000000 ripandtear-0.9.4/LICENSE
+-rw-rw-r--   0 beard     (1000) beard     (1000)    17207 2023-04-22 16:04:06.606638 ripandtear-0.9.4/PKG-INFO
+-rw-rw-r--   0 beard     (1000) beard     (1000)    16817 2023-04-22 16:03:38.000000 ripandtear-0.9.4/README.md
+-rw-rw-r--   0 beard     (1000) beard     (1000)       90 2023-02-20 00:52:42.000000 ripandtear-0.9.4/pyproject.toml
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 16:04:06.598638 ripandtear-0.9.4/ripandtear/
+-rw-rw-r--   0 beard     (1000) beard     (1000)       22 2023-04-22 15:55:11.000000 ripandtear-0.9.4/ripandtear/__init__.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8025 2023-02-28 02:57:32.000000 ripandtear-0.9.4/ripandtear/__main__.py
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 16:04:06.602638 ripandtear-0.9.4/ripandtear/extractors/
+-rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 22:50:13.000000 ripandtear-0.9.4/ripandtear/extractors/__init__.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    13425 2023-04-11 15:19:35.000000 ripandtear-0.9.4/ripandtear/extractors/bunkr.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8646 2023-02-28 02:57:32.000000 ripandtear-0.9.4/ripandtear/extractors/common.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6740 2023-04-11 15:19:35.000000 ripandtear-0.9.4/ripandtear/extractors/coomer.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     5143 2023-04-11 15:19:35.000000 ripandtear-0.9.4/ripandtear/extractors/cyberdrop.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2451 2023-04-11 15:19:35.000000 ripandtear-0.9.4/ripandtear/extractors/gfycat.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     5370 2023-04-11 15:19:35.000000 ripandtear-0.9.4/ripandtear/extractors/gofile.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     7926 2023-04-11 15:19:35.000000 ripandtear-0.9.4/ripandtear/extractors/imgur.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8128 2023-04-11 15:19:35.000000 ripandtear-0.9.4/ripandtear/extractors/jpg.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    18471 2023-04-11 15:19:35.000000 ripandtear-0.9.4/ripandtear/extractors/reddit.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     9383 2023-04-22 15:55:11.000000 ripandtear-0.9.4/ripandtear/extractors/redgifs.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6065 2023-04-11 15:19:35.000000 ripandtear-0.9.4/ripandtear/extractors/tiktits.py
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 16:04:06.606638 ripandtear-0.9.4/ripandtear/utils/
+-rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 04:04:14.000000 ripandtear-0.9.4/ripandtear/utils/__init__.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    10060 2023-02-28 02:57:32.000000 ripandtear-0.9.4/ripandtear/utils/cli_arguments.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)      708 2023-02-27 19:25:42.000000 ripandtear-0.9.4/ripandtear/utils/color.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6767 2023-04-11 15:19:35.000000 ripandtear-0.9.4/ripandtear/utils/conductor.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     7198 2023-03-02 23:14:20.000000 ripandtear-0.9.4/ripandtear/utils/content_finder.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)      870 2023-02-27 19:25:42.000000 ripandtear-0.9.4/ripandtear/utils/custom_types.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8474 2023-04-11 15:19:35.000000 ripandtear-0.9.4/ripandtear/utils/downloader.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2847 2023-02-20 00:52:42.000000 ripandtear-0.9.4/ripandtear/utils/file_hasher.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2369 2023-04-11 15:19:35.000000 ripandtear-0.9.4/ripandtear/utils/file_sorter.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)      467 2023-02-27 19:25:42.000000 ripandtear-0.9.4/ripandtear/utils/logger.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2196 2023-02-27 19:25:42.000000 ripandtear-0.9.4/ripandtear/utils/progress.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    11036 2023-02-28 02:58:35.000000 ripandtear-0.9.4/ripandtear/utils/rat_info.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     4775 2023-02-27 19:25:42.000000 ripandtear-0.9.4/ripandtear/utils/rat_interaction.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     4961 2023-04-11 15:19:35.000000 ripandtear-0.9.4/ripandtear/utils/tracker.py
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 16:04:06.602638 ripandtear-0.9.4/ripandtear.egg-info/
+-rw-rw-r--   0 beard     (1000) beard     (1000)    17207 2023-04-22 16:04:06.000000 ripandtear-0.9.4/ripandtear.egg-info/PKG-INFO
+-rw-rw-r--   0 beard     (1000) beard     (1000)     1111 2023-04-22 16:04:06.000000 ripandtear-0.9.4/ripandtear.egg-info/SOURCES.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)        1 2023-04-22 16:04:06.000000 ripandtear-0.9.4/ripandtear.egg-info/dependency_links.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)       58 2023-04-22 16:04:06.000000 ripandtear-0.9.4/ripandtear.egg-info/entry_points.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)      405 2023-04-22 16:04:06.000000 ripandtear-0.9.4/ripandtear.egg-info/requires.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)       11 2023-04-22 16:04:06.000000 ripandtear-0.9.4/ripandtear.egg-info/top_level.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)     1058 2023-04-22 16:04:06.606638 ripandtear-0.9.4/setup.cfg
```

### Comparing `ripandtear-0.9.3/LICENSE` & `ripandtear-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/PKG-INFO` & `ripandtear-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ripandtear
-Version: 0.9.3
+Version: 0.9.4
 Summary: An asynchronous file archival program
 Home-page: https://gitlab.com/johnny_barracuda/ripandtear/
 Author: Johnny-Barracuda
 Author-email: johnny_barracuda@protonmail.ch
 Project-URL: Bug Tracker, https://gitlab.com/johnny_barracuda/ripandtear/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -35,14 +35,21 @@
 
 `pip install ripandtear`
 
 (Windows)
 
 `py -m pip install ripandtear`
 
+### Additional Downloads
+After downloading ripandtear from your command line run
+
+`playwright install`
+
+Playwright is a webdevelopment tool that opens up a browser in the background. Ripandtear uses this for certain websites to interact with javascript in order to find and download links
+
 
 ## Current Supported Sites
 
 **Bunkr.su**
 
 **Coomer.party**
```

### Comparing `ripandtear-0.9.3/README.md` & `ripandtear-0.9.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,21 @@
 
 `pip install ripandtear`
 
 (Windows)
 
 `py -m pip install ripandtear`
 
+### Additional Downloads
+After downloading ripandtear from your command line run
+
+`playwright install`
+
+Playwright is a webdevelopment tool that opens up a browser in the background. Ripandtear uses this for certain websites to interact with javascript in order to find and download links
+
 
 ## Current Supported Sites
 
 **Bunkr.su**
 
 **Coomer.party**
```

### Comparing `ripandtear-0.9.3/ripandtear/__main__.py` & `ripandtear-0.9.4/ripandtear/__main__.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/extractors/bunkr.py` & `ripandtear-0.9.4/ripandtear/extractors/bunkr.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/extractors/common.py` & `ripandtear-0.9.4/ripandtear/extractors/common.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/extractors/coomer.py` & `ripandtear-0.9.4/ripandtear/extractors/coomer.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/extractors/cyberdrop.py` & `ripandtear-0.9.4/ripandtear/extractors/cyberdrop.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/extractors/gfycat.py` & `ripandtear-0.9.4/ripandtear/extractors/gfycat.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/extractors/gofile.py` & `ripandtear-0.9.4/ripandtear/extractors/gofile.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/extractors/imgur.py` & `ripandtear-0.9.4/ripandtear/extractors/imgur.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/extractors/jpg.py` & `ripandtear-0.9.4/ripandtear/extractors/jpg.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/extractors/reddit.py` & `ripandtear-0.9.4/ripandtear/extractors/reddit.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/extractors/redgifs.py` & `ripandtear-0.9.4/ripandtear/extractors/redgifs.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 prefix = "redgifs"
 url_root = "https://www.redgifs.com/"
 url_root_v3 = "https://v3.redgifs.com/"
 
 single_uid_api = "https://api.redgifs.com/v2/gifs/"
 
+re_tag_url = re.compile(r"(https?://)(\w+\.)(redgifs\.com/)gifs\/(.*)")
+
 re_extension = re.compile(
     r"(https?://)(\w+\.)(redgifs.com/)(\w+)(-\w+)?\.(\w+)")
 
 re_watch_uid = re.compile(
     r"(/watch/)(\w+)#")
 
 # 'https://i.redgifs.com/i/kosherpurehairstreak.jpg'
@@ -73,14 +75,93 @@
 
         elif re_user.match(url_dictionary['url']):
 
             log.debug("User found. Sending to user_download_v3")
             await self.user_download_v3(re_user.match(
                 url_dictionary['url']).group(6), url_dictionary.copy())
 
+        elif re_tag_url.match(url_dictionary['url']):
+
+            log.debug("Tags url found. Preparing download")
+            await self.tag_download(url_dictionary.copy())
+
+    async def tag_download(self, url_dictionary: UrlDictionary) -> None:
+
+        log.info(f"Found Tag. Preparing download")
+
+        async with async_playwright() as pw:
+
+            try:
+                browser = await pw.chromium.launch()
+                page = await browser.new_page()
+                await page.goto(url_dictionary['url'])
+
+                log.info("Searching for videos")
+                content = await page.query_selector_all('a.tile')
+
+                while True:
+
+                    for x in range(5):
+                        await page.keyboard.down('PageDown')
+                        await page.wait_for_timeout(200)
+
+                    new_content = await page.query_selector_all('a.tile')
+
+                    if len(new_content) > len(content):
+
+                        content = new_content
+                        log.info(f"Gifs found: {len(new_content)}")
+
+                    else:
+                        content = new_content
+                        break
+
+                if page.locator('div.gifList'):
+                    html = await page.locator('div.gifList').inner_html()
+
+                elif page.locator('div.tileFeed'):
+                    html = await page.locator('div.tileFeed').inner_html()
+
+                soup = BeautifulSoup(html, features='html.parser')
+
+                already_downloaded_urls = rat_info.get_downloaded_urls()
+
+                tasks = []
+                for link in soup.find_all('a'):
+
+                    href = link.get('href').split('#')[0]
+
+                    url = f"https://v3.redgifs.com{href}"
+
+                    if url in already_downloaded_urls and url_dictionary['download'] is True:
+                        log.info(f"Already downloaded: {url}")
+                        continue
+
+                    elif url not in already_downloaded_urls and url_dictionary['download'] is True:
+                        log.info(f"Creating task out of {url}")
+
+                        url_dictionary['url'] = url
+                        tasks.append(asyncio.create_task(
+                            self.run(url_dictionary.copy())))
+
+                    elif url_dictionary['download'] is False:
+                        url_dictionary['url_to_download'] = url
+                        continue
+
+                log.info("Executing tasks")
+                await asyncio.gather(*tasks)
+
+            except Exception:
+                log.exception("Problem getting gifs from tag url")
+                await self.common_failed_attempt(url_dictionary.copy())
+
+            finally:
+                await page.close()
+                await browser.close()
+
     async def single_download(self, uid: str, url_dictionary: UrlDictionary) -> None:
 
         async with sem:
 
             log.debug("Single image given. Attempting download")
 
             async with httpx.AsyncClient() as client:
```

### Comparing `ripandtear-0.9.3/ripandtear/extractors/tiktits.py` & `ripandtear-0.9.4/ripandtear/extractors/tiktits.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/utils/cli_arguments.py` & `ripandtear-0.9.4/ripandtear/utils/cli_arguments.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/utils/color.py` & `ripandtear-0.9.4/ripandtear/utils/color.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/utils/conductor.py` & `ripandtear-0.9.4/ripandtear/utils/conductor.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/utils/content_finder.py` & `ripandtear-0.9.4/ripandtear/utils/content_finder.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/utils/custom_types.py` & `ripandtear-0.9.4/ripandtear/utils/custom_types.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/utils/downloader.py` & `ripandtear-0.9.4/ripandtear/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/utils/file_hasher.py` & `ripandtear-0.9.4/ripandtear/utils/file_hasher.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/utils/file_sorter.py` & `ripandtear-0.9.4/ripandtear/utils/file_sorter.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/utils/progress.py` & `ripandtear-0.9.4/ripandtear/utils/progress.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/utils/rat_info.py` & `ripandtear-0.9.4/ripandtear/utils/rat_info.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/utils/rat_interaction.py` & `ripandtear-0.9.4/ripandtear/utils/rat_interaction.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear/utils/tracker.py` & `ripandtear-0.9.4/ripandtear/utils/tracker.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/ripandtear.egg-info/PKG-INFO` & `ripandtear-0.9.4/ripandtear.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ripandtear
-Version: 0.9.3
+Version: 0.9.4
 Summary: An asynchronous file archival program
 Home-page: https://gitlab.com/johnny_barracuda/ripandtear/
 Author: Johnny-Barracuda
 Author-email: johnny_barracuda@protonmail.ch
 Project-URL: Bug Tracker, https://gitlab.com/johnny_barracuda/ripandtear/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -35,14 +35,21 @@
 
 `pip install ripandtear`
 
 (Windows)
 
 `py -m pip install ripandtear`
 
+### Additional Downloads
+After downloading ripandtear from your command line run
+
+`playwright install`
+
+Playwright is a webdevelopment tool that opens up a browser in the background. Ripandtear uses this for certain websites to interact with javascript in order to find and download links
+
 
 ## Current Supported Sites
 
 **Bunkr.su**
 
 **Coomer.party**
```

### Comparing `ripandtear-0.9.3/ripandtear.egg-info/SOURCES.txt` & `ripandtear-0.9.4/ripandtear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.3/setup.cfg` & `ripandtear-0.9.4/setup.cfg`

 * *Files identical despite different names*

