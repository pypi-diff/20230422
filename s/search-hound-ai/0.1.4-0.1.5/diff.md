# Comparing `tmp/search_hound_ai-0.1.4.tar.gz` & `tmp/search_hound_ai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "search_hound_ai-0.1.4.tar", max compression
+gzip compressed data, was "search_hound_ai-0.1.5.tar", max compression
```

## Comparing `search_hound_ai-0.1.4.tar` & `search_hound_ai-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-04-22 00:47:36.079460 search_hound_ai-0.1.4/LICENSE
--rw-r--r--   0        0        0     1434 2023-04-22 00:47:36.079460 search_hound_ai-0.1.4/README.md
--rw-r--r--   0        0        0      541 2023-04-22 00:47:36.083461 search_hound_ai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      504 2023-04-22 00:47:36.083461 search_hound_ai-0.1.4/search_hound_ai/__init__.py
--rwxr-xr-x   0        0        0      530 2023-04-22 00:47:36.083461 search_hound_ai-0.1.4/search_hound_ai/app.py
--rw-r--r--   0        0        0      369 2023-04-22 00:47:36.083461 search_hound_ai-0.1.4/search_hound_ai/app_test.py
--rw-r--r--   0        0        0      392 2023-04-22 00:47:36.083461 search_hound_ai-0.1.4/search_hound_ai/hound_client_commands.py
--rw-r--r--   0        0        0     1146 2023-04-22 00:47:36.083461 search_hound_ai-0.1.4/search_hound_ai/openai_lib.py
--rw-r--r--   0        0        0      465 2023-04-22 00:47:36.083461 search_hound_ai-0.1.4/search_hound_ai/search_hound_lib.py
--rw-r--r--   0        0        0     1902 1970-01-01 00:00:00.000000 search_hound_ai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-22 04:01:13.611708 search_hound_ai-0.1.5/LICENSE
+-rw-r--r--   0        0        0      912 2023-04-22 04:01:13.611708 search_hound_ai-0.1.5/README.md
+-rw-r--r--   0        0        0      534 2023-04-22 04:01:13.611708 search_hound_ai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      504 2023-04-22 04:01:13.611708 search_hound_ai-0.1.5/search_hound_ai/__init__.py
+-rwxr-xr-x   0        0        0      530 2023-04-22 04:01:13.611708 search_hound_ai-0.1.5/search_hound_ai/app.py
+-rw-r--r--   0        0        0      369 2023-04-22 04:01:13.611708 search_hound_ai-0.1.5/search_hound_ai/app_test.py
+-rw-r--r--   0        0        0      392 2023-04-22 04:01:13.611708 search_hound_ai-0.1.5/search_hound_ai/hound_client_commands.py
+-rw-r--r--   0        0        0     1146 2023-04-22 04:01:13.611708 search_hound_ai-0.1.5/search_hound_ai/openai_lib.py
+-rw-r--r--   0        0        0      465 2023-04-22 04:01:13.611708 search_hound_ai-0.1.5/search_hound_ai/search_hound_lib.py
+-rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 search_hound_ai-0.1.5/PKG-INFO
```

### Comparing `search_hound_ai-0.1.4/LICENSE` & `search_hound_ai-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `search_hound_ai-0.1.4/pyproject.toml` & `search_hound_ai-0.1.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "search-hound-ai"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Martin Patino <martin@sibipro.com>"]
 readme = "README.md"
 packages = [{include = "search_hound_ai"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -17,8 +17,8 @@
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-search-hound = "search_hound_ai.app:main"
+hound = "search_hound_ai.app:main"
```

### Comparing `search_hound_ai-0.1.4/search_hound_ai/app.py` & `search_hound_ai-0.1.5/search_hound_ai/app.py`

 * *Files identical despite different names*

### Comparing `search_hound_ai-0.1.4/search_hound_ai/openai_lib.py` & `search_hound_ai-0.1.5/search_hound_ai/openai_lib.py`

 * *Files identical despite different names*

