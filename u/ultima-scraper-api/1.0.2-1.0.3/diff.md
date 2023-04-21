# Comparing `tmp/ultima_scraper_api-1.0.2.tar.gz` & `tmp/ultima_scraper_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_api-1.0.2.tar", max compression
+gzip compressed data, was "ultima_scraper_api-1.0.3.tar", max compression
```

## Comparing `ultima_scraper_api-1.0.2.tar` & `ultima_scraper_api-1.0.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1030 2023-04-21 13:32:00.033065 ultima_scraper_api-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-1.0.2/ultima_scraper_api/.readthedocs.yaml
--rw-r--r--   0        0        0     2140 2023-03-26 20:22:06.588147 ultima_scraper_api-1.0.2/ultima_scraper_api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-1.0.2/ultima_scraper_api/__main__.py
--rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/__init__.py
--rw-r--r--   0        0        0     6799 2023-03-25 23:19:49.924231 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/api_helper.py
--rw-r--r--   0        0        0     1694 2023-03-13 07:53:19.528681 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/api_streamliner.py
--rw-r--r--   0        0        0      696 2022-12-02 16:36:46.812390 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/background_tasks.py
--rw-r--r--   0        0        0     2842 2023-04-09 16:10:08.954446 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/__init__.py
--rw-r--r--   0        0        0      164 2023-03-26 17:40:00.484637 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/__init__.py
--rw-r--r--   0        0        0    19219 2023-04-10 14:08:37.807384 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/auth_model.py
--rw-r--r--   0        0        0     6511 2023-04-10 15:12:02.910813 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/collection_model.py
--rw-r--r--   0        0        0    11370 2023-04-11 14:57:48.165435 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/extras.py
--rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
--rw-r--r--   0        0        0     6216 2023-04-11 15:11:13.965757 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/message_model.py
--rw-r--r--   0        0        0     6918 2023-04-09 17:42:13.567826 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/post_model.py
--rw-r--r--   0        0        0     3212 2023-03-26 19:02:31.325107 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/story_model.py
--rw-r--r--   0        0        0    28334 2023-04-21 13:30:48.828644 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/decorators/decorators.py
--rw-r--r--   0        0        0     3783 2023-04-11 14:58:58.366956 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/fansly.py
--rw-r--r--   0        0        0     2505 2023-04-09 16:10:03.007639 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/__init__.py
--rw-r--r--   0        0        0      153 2023-03-26 20:30:17.157147 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/classes/__init__.py
--rw-r--r--   0        0        0    19791 2023-04-21 03:37:28.750604 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
--rw-r--r--   0        0        0    10554 2023-03-21 11:26:19.768761 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/classes/extras.py
--rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
--rw-r--r--   0        0        0     2748 2023-03-27 06:43:37.105523 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/classes/message_model.py
--rw-r--r--   0        0        0     3375 2023-03-27 00:23:55.042753 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/classes/post_model.py
--rw-r--r--   0        0        0     1318 2023-04-09 10:09:44.773447 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/classes/story_model.py
--rw-r--r--   0        0        0    27351 2023-04-21 13:26:46.711662 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
--rw-r--r--   0        0        0     3980 2023-03-28 02:35:06.221154 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/onlyfans.py
--rw-r--r--   0        0        0     2678 2023-03-12 07:58:39.963131 ultima_scraper_api-1.0.2/ultima_scraper_api/apis/user_streamliner.py
--rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-1.0.2/ultima_scraper_api/classes/__init__.py
--rw-r--r--   0        0        0    13187 2023-03-24 22:26:49.870986 ultima_scraper_api-1.0.2/ultima_scraper_api/classes/make_settings.py
--rw-r--r--   0        0        0     3977 2023-03-12 11:46:35.721289 ultima_scraper_api-1.0.2/ultima_scraper_api/classes/prepare_directories.py
--rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.2/ultima_scraper_api/classes/prepare_download.py
--rw-r--r--   0        0        0    13595 2023-04-11 15:12:54.204494 ultima_scraper_api-1.0.2/ultima_scraper_api/classes/prepare_metadata.py
--rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.2/ultima_scraper_api/classes/prepare_webhooks.py
--rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-1.0.2/ultima_scraper_api/docs/Makefile
--rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-1.0.2/ultima_scraper_api/docs/make.bat
--rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-1.0.2/ultima_scraper_api/docs/requirements.txt
--rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-1.0.2/ultima_scraper_api/docs/source/conf.py
--rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-1.0.2/ultima_scraper_api/docs/source/index.rst
--rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-1.0.2/ultima_scraper_api/helpers/__init__.py
--rw-r--r--   0        0        0    11469 2023-04-09 08:48:21.278550 ultima_scraper_api-1.0.2/ultima_scraper_api/helpers/main_helper.py
--rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-1.0.2/ultima_scraper_api/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-1.0.2/ultima_scraper_api/managers/job_manager/__init__.py
--rw-r--r--   0        0        0     1791 2023-03-04 03:36:24.985587 ultima_scraper_api-1.0.2/ultima_scraper_api/managers/job_manager/job_manager.py
--rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-1.0.2/ultima_scraper_api/managers/job_manager/jobs/__init__.py
--rw-r--r--   0        0        0      704 2023-03-24 22:51:29.186132 ultima_scraper_api-1.0.2/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
--rw-r--r--   0        0        0     2181 2023-03-27 18:00:12.375116 ultima_scraper_api-1.0.2/ultima_scraper_api/managers/scrape_manager.py
--rw-r--r--   0        0        0    14981 2023-04-21 12:41:49.451546 ultima_scraper_api-1.0.2/ultima_scraper_api/managers/session_manager.py
--rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-1.0.2/ultima_scraper_api/py.typed
--rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 ultima_scraper_api-1.0.2/setup.py
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 ultima_scraper_api-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1030 2023-04-21 19:40:07.507003 ultima_scraper_api-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-1.0.3/ultima_scraper_api/.readthedocs.yaml
+-rw-r--r--   0        0        0     2140 2023-03-26 20:22:06.588147 ultima_scraper_api-1.0.3/ultima_scraper_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-1.0.3/ultima_scraper_api/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/__init__.py
+-rw-r--r--   0        0        0     6799 2023-03-25 23:19:49.924231 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/api_helper.py
+-rw-r--r--   0        0        0     1694 2023-03-13 07:53:19.528681 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/api_streamliner.py
+-rw-r--r--   0        0        0      696 2022-12-02 16:36:46.812390 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/background_tasks.py
+-rw-r--r--   0        0        0     2842 2023-04-09 16:10:08.954446 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/__init__.py
+-rw-r--r--   0        0        0      164 2023-03-26 17:40:00.484637 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/__init__.py
+-rw-r--r--   0        0        0    19219 2023-04-10 14:08:37.807384 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/auth_model.py
+-rw-r--r--   0        0        0     6511 2023-04-10 15:12:02.910813 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/collection_model.py
+-rw-r--r--   0        0        0    11370 2023-04-11 14:57:48.165435 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/extras.py
+-rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
+-rw-r--r--   0        0        0     6216 2023-04-11 15:11:13.965757 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/message_model.py
+-rw-r--r--   0        0        0     6918 2023-04-09 17:42:13.567826 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/post_model.py
+-rw-r--r--   0        0        0     3212 2023-03-26 19:02:31.325107 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/story_model.py
+-rw-r--r--   0        0        0    27819 2023-04-21 19:38:11.534003 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/decorators/decorators.py
+-rw-r--r--   0        0        0     3783 2023-04-11 14:58:58.366956 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/fansly.py
+-rw-r--r--   0        0        0     2505 2023-04-09 16:10:03.007639 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/__init__.py
+-rw-r--r--   0        0        0      153 2023-03-26 20:30:17.157147 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/__init__.py
+-rw-r--r--   0        0        0    19791 2023-04-21 03:37:28.750604 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
+-rw-r--r--   0        0        0    10554 2023-03-21 11:26:19.768761 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/extras.py
+-rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
+-rw-r--r--   0        0        0     2748 2023-03-27 06:43:37.105523 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/message_model.py
+-rw-r--r--   0        0        0     3375 2023-03-27 00:23:55.042753 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/post_model.py
+-rw-r--r--   0        0        0     1318 2023-04-09 10:09:44.773447 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/story_model.py
+-rw-r--r--   0        0        0    26435 2023-04-21 19:37:21.105693 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
+-rw-r--r--   0        0        0     3980 2023-03-28 02:35:06.221154 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/onlyfans.py
+-rw-r--r--   0        0        0     2678 2023-03-12 07:58:39.963131 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/user_streamliner.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-1.0.3/ultima_scraper_api/classes/__init__.py
+-rw-r--r--   0        0        0    13187 2023-03-24 22:26:49.870986 ultima_scraper_api-1.0.3/ultima_scraper_api/classes/make_settings.py
+-rw-r--r--   0        0        0     3977 2023-03-12 11:46:35.721289 ultima_scraper_api-1.0.3/ultima_scraper_api/classes/prepare_directories.py
+-rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.3/ultima_scraper_api/classes/prepare_download.py
+-rw-r--r--   0        0        0    13595 2023-04-11 15:12:54.204494 ultima_scraper_api-1.0.3/ultima_scraper_api/classes/prepare_metadata.py
+-rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.3/ultima_scraper_api/classes/prepare_webhooks.py
+-rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-1.0.3/ultima_scraper_api/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-1.0.3/ultima_scraper_api/docs/make.bat
+-rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-1.0.3/ultima_scraper_api/docs/requirements.txt
+-rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-1.0.3/ultima_scraper_api/docs/source/conf.py
+-rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-1.0.3/ultima_scraper_api/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-1.0.3/ultima_scraper_api/helpers/__init__.py
+-rw-r--r--   0        0        0    11469 2023-04-09 08:48:21.278550 ultima_scraper_api-1.0.3/ultima_scraper_api/helpers/main_helper.py
+-rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-1.0.3/ultima_scraper_api/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-1.0.3/ultima_scraper_api/managers/job_manager/__init__.py
+-rw-r--r--   0        0        0     1791 2023-03-04 03:36:24.985587 ultima_scraper_api-1.0.3/ultima_scraper_api/managers/job_manager/job_manager.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-1.0.3/ultima_scraper_api/managers/job_manager/jobs/__init__.py
+-rw-r--r--   0        0        0      704 2023-03-24 22:51:29.186132 ultima_scraper_api-1.0.3/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
+-rw-r--r--   0        0        0     2181 2023-03-27 18:00:12.375116 ultima_scraper_api-1.0.3/ultima_scraper_api/managers/scrape_manager.py
+-rw-r--r--   0        0        0    14981 2023-04-21 12:41:49.451546 ultima_scraper_api-1.0.3/ultima_scraper_api/managers/session_manager.py
+-rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-1.0.3/ultima_scraper_api/py.typed
+-rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 ultima_scraper_api-1.0.3/setup.py
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 ultima_scraper_api-1.0.3/PKG-INFO
```

### Comparing `ultima_scraper_api-1.0.2/pyproject.toml` & `ultima_scraper_api-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ultima-scraper-api"
-version = "1.0.2"
+version = "1.0.3"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_api"}]
 include = ["ultima_scraper_api/py.typed"]
```

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/__init__.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/api_helper.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/api_helper.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/api_streamliner.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/api_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/background_tasks.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/__init__.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/auth_model.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/auth_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/collection_model.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/collection_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/extras.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/extras.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/message_model.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/message_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/post_model.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/story_model.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/classes/user_model.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/user_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,15 +315,15 @@
             temp_results.append(data)
         results = api_helper.merge_dictionaries(temp_results)
         final_results = []
         if results:
             final_results = [
                 post_model.create_post(x, self, results) for x in results["posts"]
             ]
-            self.temp_scraped.Posts = final_results
+            self.scrape_manager.scraped.Posts = final_results
         return final_results
 
     async def get_post(
         self, identifier: Optional[int | str] = None, limit: int = 10, offset: int = 0
     ) -> Union[create_post, ErrorDetails]:
         if not identifier:
             identifier = self.id
@@ -399,15 +399,15 @@
                 final_results.extend(results2)
             if not inside_loop:
                 final_results = [
                     message_model.create_message(x, self, extras)
                     for x in final_results
                     if x
                 ]
-            self.temp_scraped.Messages = final_results
+            self.scrape_manager.scraped.Messages = final_results
         return final_results
 
     async def get_message_by_id(
         self, user_id=None, message_id=None, refresh=True, limit=10, offset=0
     ):
         if not user_id:
             user_id = self.id
@@ -579,28 +579,14 @@
 
     async def match_identifiers(self, identifiers: list[int | str]):
         if self.id in identifiers or self.username in identifiers:
             return True
         else:
             return False
 
-    async def find_duplicate_media(self):
-        for post in self.scraped.Posts:
-            for media in post["medias"]:
-                a = [
-                    media_2
-                    for post_2 in self.scraped.Posts
-                    for media_2 in post_2["medias"]
-                    if media["media_id"] != media_2["media_id"]
-                    and media["filename"] == media_2["filename"]
-                ]
-                if a:
-                    self.duplicate_media.extend(a)
-        return self.duplicate_media
-
     async def get_collections(self):
         link = endpoint_links(identifier=self.id).collections_api
         results = await self.get_session_manager().json_request(link)
         return results["response"]
 
     async def get_collection_content(self, collection: dict[str, Any], offset: int = 0):
         temp_responses: list[dict[str, Any]] = []
```

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/fansly/fansly.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/fansly.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/__init__.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/classes/auth_model.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/auth_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/classes/extras.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/extras.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/classes/message_model.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/message_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/classes/post_model.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/classes/story_model.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/classes/user_model.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/user_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -554,31 +554,14 @@
 
     async def match_identifiers(self, identifiers: list[int | str]):
         if self.id in identifiers or self.username in identifiers:
             return True
         else:
             return False
 
-    async def find_duplicate_media(self):
-        # A user had 10 photos but only 5 were downloaded, this was because some media on OnlyFans have the same filename but an invalid link.
-        # Even if the link returns a 404, OnlyFans still counts it as a valid media when providing model statistics.
-        # I'll have to create a diagnosis function that checks if any media fails to download and return the reason why.
-        for post in self.scraped.Posts:
-            for media in post["medias"]:
-                a = [
-                    media_2
-                    for post_2 in self.scraped.Posts
-                    for media_2 in post_2["medias"]
-                    if media["media_id"] != media_2["media_id"]
-                    and media["filename"] == media_2["filename"]
-                ]
-                if a:
-                    self.duplicate_media.extend(a)
-        return self.duplicate_media
-
     async def get_avatar(self):
         return self.avatar
 
     async def get_header(self):
         return self.header
 
     async def is_subscribed(self):
```

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/onlyfans/onlyfans.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/onlyfans.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/apis/user_streamliner.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/user_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/classes/make_settings.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/classes/make_settings.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/classes/prepare_directories.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/classes/prepare_directories.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/classes/prepare_metadata.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/classes/prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/classes/prepare_webhooks.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/classes/prepare_webhooks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/docs/Makefile` & `ultima_scraper_api-1.0.3/ultima_scraper_api/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/docs/make.bat` & `ultima_scraper_api-1.0.3/ultima_scraper_api/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/docs/source/conf.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/helpers/main_helper.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/helpers/main_helper.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/managers/job_manager/job_manager.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/managers/job_manager/job_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/managers/job_manager/jobs/custom_job.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/managers/job_manager/jobs/custom_job.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/managers/scrape_manager.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/managers/scrape_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/ultima_scraper_api/managers/session_manager.py` & `ultima_scraper_api-1.0.3/ultima_scraper_api/managers/session_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.2/setup.py` & `ultima_scraper_api-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
  'requests[socks]==2.28.2',
  'sphinx-autoapi>=2.0.0,<3.0.0',
  'sphinx-rtd-theme>=1.1.1,<2.0.0',
  'user-agent>=0.1.10,<0.2.0']
 
 setup_kwargs = {
     'name': 'ultima-scraper-api',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': '',
     'long_description': 'None',
     'author': 'DIGITALCRIMINALS',
     'author_email': '89371864+digitalcriminals@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ultima_scraper_api-1.0.2/PKG-INFO` & `ultima_scraper_api-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

