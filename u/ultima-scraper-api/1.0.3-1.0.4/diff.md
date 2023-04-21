# Comparing `tmp/ultima_scraper_api-1.0.3.tar.gz` & `tmp/ultima_scraper_api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_api-1.0.3.tar", max compression
+gzip compressed data, was "ultima_scraper_api-1.0.4.tar", max compression
```

## Comparing `ultima_scraper_api-1.0.3.tar` & `ultima_scraper_api-1.0.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1030 2023-04-21 19:40:07.507003 ultima_scraper_api-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-1.0.3/ultima_scraper_api/.readthedocs.yaml
--rw-r--r--   0        0        0     2140 2023-03-26 20:22:06.588147 ultima_scraper_api-1.0.3/ultima_scraper_api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-1.0.3/ultima_scraper_api/__main__.py
--rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/__init__.py
--rw-r--r--   0        0        0     6799 2023-03-25 23:19:49.924231 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/api_helper.py
--rw-r--r--   0        0        0     1694 2023-03-13 07:53:19.528681 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/api_streamliner.py
--rw-r--r--   0        0        0      696 2022-12-02 16:36:46.812390 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/background_tasks.py
--rw-r--r--   0        0        0     2842 2023-04-09 16:10:08.954446 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/__init__.py
--rw-r--r--   0        0        0      164 2023-03-26 17:40:00.484637 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/__init__.py
--rw-r--r--   0        0        0    19219 2023-04-10 14:08:37.807384 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/auth_model.py
--rw-r--r--   0        0        0     6511 2023-04-10 15:12:02.910813 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/collection_model.py
--rw-r--r--   0        0        0    11370 2023-04-11 14:57:48.165435 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/extras.py
--rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
--rw-r--r--   0        0        0     6216 2023-04-11 15:11:13.965757 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/message_model.py
--rw-r--r--   0        0        0     6918 2023-04-09 17:42:13.567826 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/post_model.py
--rw-r--r--   0        0        0     3212 2023-03-26 19:02:31.325107 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/story_model.py
--rw-r--r--   0        0        0    27819 2023-04-21 19:38:11.534003 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/decorators/decorators.py
--rw-r--r--   0        0        0     3783 2023-04-11 14:58:58.366956 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/fansly.py
--rw-r--r--   0        0        0     2505 2023-04-09 16:10:03.007639 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/__init__.py
--rw-r--r--   0        0        0      153 2023-03-26 20:30:17.157147 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/__init__.py
--rw-r--r--   0        0        0    19791 2023-04-21 03:37:28.750604 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
--rw-r--r--   0        0        0    10554 2023-03-21 11:26:19.768761 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/extras.py
--rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
--rw-r--r--   0        0        0     2748 2023-03-27 06:43:37.105523 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/message_model.py
--rw-r--r--   0        0        0     3375 2023-03-27 00:23:55.042753 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/post_model.py
--rw-r--r--   0        0        0     1318 2023-04-09 10:09:44.773447 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/story_model.py
--rw-r--r--   0        0        0    26435 2023-04-21 19:37:21.105693 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
--rw-r--r--   0        0        0     3980 2023-03-28 02:35:06.221154 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/onlyfans.py
--rw-r--r--   0        0        0     2678 2023-03-12 07:58:39.963131 ultima_scraper_api-1.0.3/ultima_scraper_api/apis/user_streamliner.py
--rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-1.0.3/ultima_scraper_api/classes/__init__.py
--rw-r--r--   0        0        0    13187 2023-03-24 22:26:49.870986 ultima_scraper_api-1.0.3/ultima_scraper_api/classes/make_settings.py
--rw-r--r--   0        0        0     3977 2023-03-12 11:46:35.721289 ultima_scraper_api-1.0.3/ultima_scraper_api/classes/prepare_directories.py
--rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.3/ultima_scraper_api/classes/prepare_download.py
--rw-r--r--   0        0        0    13595 2023-04-11 15:12:54.204494 ultima_scraper_api-1.0.3/ultima_scraper_api/classes/prepare_metadata.py
--rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.3/ultima_scraper_api/classes/prepare_webhooks.py
--rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-1.0.3/ultima_scraper_api/docs/Makefile
--rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-1.0.3/ultima_scraper_api/docs/make.bat
--rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-1.0.3/ultima_scraper_api/docs/requirements.txt
--rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-1.0.3/ultima_scraper_api/docs/source/conf.py
--rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-1.0.3/ultima_scraper_api/docs/source/index.rst
--rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-1.0.3/ultima_scraper_api/helpers/__init__.py
--rw-r--r--   0        0        0    11469 2023-04-09 08:48:21.278550 ultima_scraper_api-1.0.3/ultima_scraper_api/helpers/main_helper.py
--rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-1.0.3/ultima_scraper_api/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-1.0.3/ultima_scraper_api/managers/job_manager/__init__.py
--rw-r--r--   0        0        0     1791 2023-03-04 03:36:24.985587 ultima_scraper_api-1.0.3/ultima_scraper_api/managers/job_manager/job_manager.py
--rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-1.0.3/ultima_scraper_api/managers/job_manager/jobs/__init__.py
--rw-r--r--   0        0        0      704 2023-03-24 22:51:29.186132 ultima_scraper_api-1.0.3/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
--rw-r--r--   0        0        0     2181 2023-03-27 18:00:12.375116 ultima_scraper_api-1.0.3/ultima_scraper_api/managers/scrape_manager.py
--rw-r--r--   0        0        0    14981 2023-04-21 12:41:49.451546 ultima_scraper_api-1.0.3/ultima_scraper_api/managers/session_manager.py
--rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-1.0.3/ultima_scraper_api/py.typed
--rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 ultima_scraper_api-1.0.3/setup.py
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 ultima_scraper_api-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-04-21 22:24:37.351086 ultima_scraper_api-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-1.0.4/ultima_scraper_api/.readthedocs.yaml
+-rw-r--r--   0        0        0     2140 2023-03-26 20:22:06.588147 ultima_scraper_api-1.0.4/ultima_scraper_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-1.0.4/ultima_scraper_api/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/__init__.py
+-rw-r--r--   0        0        0     6799 2023-03-25 23:19:49.924231 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/api_helper.py
+-rw-r--r--   0        0        0     1694 2023-03-13 07:53:19.528681 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/api_streamliner.py
+-rw-r--r--   0        0        0      696 2022-12-02 16:36:46.812390 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/background_tasks.py
+-rw-r--r--   0        0        0     2842 2023-04-09 16:10:08.954446 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/__init__.py
+-rw-r--r--   0        0        0      164 2023-03-26 17:40:00.484637 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/__init__.py
+-rw-r--r--   0        0        0    19219 2023-04-10 14:08:37.807384 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/auth_model.py
+-rw-r--r--   0        0        0     6511 2023-04-10 15:12:02.910813 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/collection_model.py
+-rw-r--r--   0        0        0    11370 2023-04-11 14:57:48.165435 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/extras.py
+-rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
+-rw-r--r--   0        0        0     6216 2023-04-11 15:11:13.965757 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/message_model.py
+-rw-r--r--   0        0        0     6918 2023-04-09 17:42:13.567826 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/post_model.py
+-rw-r--r--   0        0        0     3212 2023-03-26 19:02:31.325107 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/story_model.py
+-rw-r--r--   0        0        0    27819 2023-04-21 19:38:11.534003 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/decorators/decorators.py
+-rw-r--r--   0        0        0     3783 2023-04-11 14:58:58.366956 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/fansly.py
+-rw-r--r--   0        0        0     2505 2023-04-09 16:10:03.007639 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/__init__.py
+-rw-r--r--   0        0        0      153 2023-03-26 20:30:17.157147 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/classes/__init__.py
+-rw-r--r--   0        0        0    19791 2023-04-21 03:37:28.750604 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
+-rw-r--r--   0        0        0    10554 2023-03-21 11:26:19.768761 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/classes/extras.py
+-rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
+-rw-r--r--   0        0        0     2748 2023-03-27 06:43:37.105523 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/classes/message_model.py
+-rw-r--r--   0        0        0     3375 2023-03-27 00:23:55.042753 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/classes/post_model.py
+-rw-r--r--   0        0        0     1318 2023-04-09 10:09:44.773447 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/classes/story_model.py
+-rw-r--r--   0        0        0    26435 2023-04-21 19:37:21.105693 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
+-rw-r--r--   0        0        0     3980 2023-03-28 02:35:06.221154 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/onlyfans.py
+-rw-r--r--   0        0        0     2678 2023-03-12 07:58:39.963131 ultima_scraper_api-1.0.4/ultima_scraper_api/apis/user_streamliner.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-1.0.4/ultima_scraper_api/classes/__init__.py
+-rw-r--r--   0        0        0    13187 2023-03-24 22:26:49.870986 ultima_scraper_api-1.0.4/ultima_scraper_api/classes/make_settings.py
+-rw-r--r--   0        0        0     3977 2023-03-12 11:46:35.721289 ultima_scraper_api-1.0.4/ultima_scraper_api/classes/prepare_directories.py
+-rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.4/ultima_scraper_api/classes/prepare_download.py
+-rw-r--r--   0        0        0    13595 2023-04-11 15:12:54.204494 ultima_scraper_api-1.0.4/ultima_scraper_api/classes/prepare_metadata.py
+-rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.4/ultima_scraper_api/classes/prepare_webhooks.py
+-rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-1.0.4/ultima_scraper_api/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-1.0.4/ultima_scraper_api/docs/make.bat
+-rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-1.0.4/ultima_scraper_api/docs/requirements.txt
+-rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-1.0.4/ultima_scraper_api/docs/source/conf.py
+-rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-1.0.4/ultima_scraper_api/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-1.0.4/ultima_scraper_api/helpers/__init__.py
+-rw-r--r--   0        0        0    11368 2023-04-21 22:22:23.096800 ultima_scraper_api-1.0.4/ultima_scraper_api/helpers/main_helper.py
+-rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-1.0.4/ultima_scraper_api/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-1.0.4/ultima_scraper_api/managers/job_manager/__init__.py
+-rw-r--r--   0        0        0     1791 2023-03-04 03:36:24.985587 ultima_scraper_api-1.0.4/ultima_scraper_api/managers/job_manager/job_manager.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-1.0.4/ultima_scraper_api/managers/job_manager/jobs/__init__.py
+-rw-r--r--   0        0        0      704 2023-03-24 22:51:29.186132 ultima_scraper_api-1.0.4/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
+-rw-r--r--   0        0        0     2181 2023-03-27 18:00:12.375116 ultima_scraper_api-1.0.4/ultima_scraper_api/managers/scrape_manager.py
+-rw-r--r--   0        0        0    14981 2023-04-21 12:41:49.451546 ultima_scraper_api-1.0.4/ultima_scraper_api/managers/session_manager.py
+-rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-1.0.4/ultima_scraper_api/py.typed
+-rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 ultima_scraper_api-1.0.4/setup.py
+-rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 ultima_scraper_api-1.0.4/PKG-INFO
```

### Comparing `ultima_scraper_api-1.0.3/pyproject.toml` & `ultima_scraper_api-1.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ultima-scraper-api"
-version = "1.0.3"
+version = "1.0.4"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_api"}]
 include = ["ultima_scraper_api/py.typed"]
 
@@ -22,14 +22,15 @@
 aiofiles = "^22.1.0"
 beautifulsoup4 = "^4.11.1"
 Sphinx = "^5.3.0"
 sphinx-autoapi = "^2.0.0"
 sphinx-rtd-theme = "^1.1.1"
 mypy = "^0.991"
 lxml =  "^4.9.1"
+win32-setctime = {version="^1.1.0", platform = 'win32'}
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.2"
 
 [tool.semantic_release]
 version_toml = "pyproject.toml:tool.poetry.version"
```

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/__init__.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/api_helper.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/api_helper.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/api_streamliner.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/api_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/background_tasks.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/__init__.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/auth_model.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/auth_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/collection_model.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/collection_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/extras.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/extras.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/message_model.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/message_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/post_model.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/story_model.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/classes/user_model.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/classes/user_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/fansly/fansly.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/fansly/fansly.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/__init__.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/auth_model.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/classes/auth_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/extras.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/classes/extras.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/message_model.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/classes/message_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/post_model.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/story_model.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/classes/user_model.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/classes/user_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/onlyfans/onlyfans.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/onlyfans/onlyfans.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/apis/user_streamliner.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/apis/user_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/classes/make_settings.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/classes/make_settings.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/classes/prepare_directories.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/classes/prepare_directories.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/classes/prepare_metadata.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/classes/prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/classes/prepare_webhooks.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/classes/prepare_webhooks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/docs/Makefile` & `ultima_scraper_api-1.0.4/ultima_scraper_api/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/docs/make.bat` & `ultima_scraper_api-1.0.4/ultima_scraper_api/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/docs/source/conf.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/helpers/main_helper.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/helpers/main_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 import shutil
 import subprocess
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, BinaryIO, Literal
 
 import orjson
 import requests
-import ultima_scraper_api
-import ultima_scraper_api.classes.make_settings as make_settings
-import ultima_scraper_api.classes.prepare_webhooks as prepare_webhooks
 from aiofiles import os as async_os
 from bs4 import BeautifulSoup
 from mergedeep import Strategy, merge  # type: ignore
 
+import ultima_scraper_api
+import ultima_scraper_api.classes.make_settings as make_settings
+import ultima_scraper_api.classes.prepare_webhooks as prepare_webhooks
+
 if TYPE_CHECKING:
     pass
 
 api_types = ultima_scraper_api.api_types
 auth_types = ultima_scraper_api.auth_types
 user_types = ultima_scraper_api.user_types
 
@@ -106,24 +107,21 @@
         merged.pop("directories")
     return merged
 
 
 async def format_image(filepath: Path, timestamp: float, reformat_media: bool):
     if reformat_media:
         while True:
-            try:
-                if os_name == "Windows":
-                    from win32_setctime import setctime
-
-                    setctime(filepath, timestamp)
-                    # print(f"Updated Creation Time {filepath}")
-                os.utime(filepath, (timestamp, timestamp))
-                # print(f"Updated Modification Time {filepath}")
-            except Exception as _e:
-                continue
+            if os_name == "Windows":
+                from win32_setctime import setctime
+
+                setctime(filepath, timestamp)
+                # print(f"Updated Creation Time {filepath}")
+            os.utime(filepath, (timestamp, timestamp))
+            # print(f"Updated Modification Time {filepath}")
             break
 
 
 def check_space(
     download_paths: list[Path],
     min_size: int = 0,
     priority: str = "download",
```

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/managers/job_manager/job_manager.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/managers/job_manager/job_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/managers/job_manager/jobs/custom_job.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/managers/job_manager/jobs/custom_job.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/managers/scrape_manager.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/managers/scrape_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/ultima_scraper_api/managers/session_manager.py` & `ultima_scraper_api-1.0.4/ultima_scraper_api/managers/session_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.3/setup.py` & `ultima_scraper_api-1.0.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,25 +34,29 @@
  'python-dateutil>=2.8.2,<3.0.0',
  'python-socks[asyncio]==2.2.0',
  'requests[socks]==2.28.2',
  'sphinx-autoapi>=2.0.0,<3.0.0',
  'sphinx-rtd-theme>=1.1.1,<2.0.0',
  'user-agent>=0.1.10,<0.2.0']
 
+extras_require = \
+{':sys_platform == "win32"': ['win32-setctime>=1.1.0,<2.0.0']}
+
 setup_kwargs = {
     'name': 'ultima-scraper-api',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': '',
     'long_description': 'None',
     'author': 'DIGITALCRIMINALS',
     'author_email': '89371864+digitalcriminals@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `ultima_scraper_api-1.0.3/PKG-INFO` & `ultima_scraper_api-1.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-api
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -20,7 +20,8 @@
 Requires-Dist: orjson (>=3.8.3,<4.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-socks[asyncio] (==2.2.0)
 Requires-Dist: requests[socks] (==2.28.2)
 Requires-Dist: sphinx-autoapi (>=2.0.0,<3.0.0)
 Requires-Dist: sphinx-rtd-theme (>=1.1.1,<2.0.0)
 Requires-Dist: user-agent (>=0.1.10,<0.2.0)
+Requires-Dist: win32-setctime (>=1.1.0,<2.0.0); sys_platform == "win32"
```

