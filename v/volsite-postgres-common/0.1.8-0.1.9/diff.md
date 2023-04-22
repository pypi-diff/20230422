# Comparing `tmp/volsite_postgres_common-0.1.8.tar.gz` & `tmp/volsite_postgres_common-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volsite_postgres_common-0.1.8.tar", last modified: Thu Jan 26 08:53:53 2023, max compression
+gzip compressed data, was "volsite_postgres_common-0.1.9.tar", last modified: Thu Jan 26 09:21:45 2023, max compression
```

## Comparing `volsite_postgres_common-0.1.8.tar` & `volsite_postgres_common-0.1.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 08:53:53.287222 volsite_postgres_common-0.1.8/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      234 2023-01-26 08:53:53.287222 volsite_postgres_common-0.1.8/PKG-INFO
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       31 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/README.rst
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      107 2023-01-26 08:53:53.287222 volsite_postgres_common-0.1.8/setup.cfg
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      378 2023-01-26 08:53:50.000000 volsite_postgres_common-0.1.8/setup.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 08:53:53.207220 volsite_postgres_common-0.1.8/src/
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 08:53:53.283222 volsite_postgres_common-0.1.8/src/volsite_postgres_common/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      259 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/Base64Utf8.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 08:53:53.283222 volsite_postgres_common-0.1.8/src/volsite_postgres_common/api/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     3222 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/api/CA.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/api/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 08:53:53.283222 volsite_postgres_common-0.1.8/src/volsite_postgres_common/api/enum/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/api/enum/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       77 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/api/enum/common_error_code.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      658 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/api/enum/enum.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 08:53:53.283222 volsite_postgres_common-0.1.8/src/volsite_postgres_common/db/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     2082 2023-01-26 08:53:32.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/db/BFn.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      681 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/db/CC.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1037 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/db/CFn.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      410 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/db/FnT.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/db/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      192 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/db/migration.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 08:53:53.283222 volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      513 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/AInsertFunction.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     3114 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/function.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1431 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/general.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     2450 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/id.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      133 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/insert.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     5160 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/json.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1486 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/sql_segments.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 08:53:53.287222 volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/title_description/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1527 2023-01-26 08:28:07.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/title_description/APFnUpsertDescription.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1291 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/title_description/APFnUpsertTitle.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     2410 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/title_description/APFnUpsertTitleDescriptionB64.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/title_description/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 08:53:53.287222 volsite_postgres_common-0.1.8/src/volsite_postgres_common/table/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/table/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1203 2023-01-26 07:39:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/table/create_table_descriptions.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1293 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/table/create_table_titles.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      595 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/table/description.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      802 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/table/series.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      951 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/table/text.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 08:53:53.287222 volsite_postgres_common-0.1.8/src/volsite_postgres_common/test/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      515 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/test/Timer.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/test/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      787 2023-01-23 23:33:26.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/test/assert_util.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 08:53:53.287222 volsite_postgres_common-0.1.8/src/volsite_postgres_common/test/db/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      154 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/test/db/ATestDb.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      282 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/test/db/ATestSetUser.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/test/db/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      885 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common/test/dokuwiki.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 08:53:53.283222 volsite_postgres_common-0.1.8/src/volsite_postgres_common.egg-info/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      234 2023-01-26 08:53:52.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common.egg-info/PKG-INFO
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     2092 2023-01-26 08:53:53.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common.egg-info/SOURCES.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        1 2023-01-26 08:53:52.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common.egg-info/dependency_links.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       15 2023-01-26 08:53:53.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common.egg-info/requires.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       24 2023-01-26 08:53:53.000000 volsite_postgres_common-0.1.8/src/volsite_postgres_common.egg-info/top_level.txt
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 09:21:45.311820 volsite_postgres_common-0.1.9/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      234 2023-01-26 09:21:45.311820 volsite_postgres_common-0.1.9/PKG-INFO
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       31 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/README.rst
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      107 2023-01-26 09:21:45.311820 volsite_postgres_common-0.1.9/setup.cfg
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      378 2023-01-26 09:21:40.000000 volsite_postgres_common-0.1.9/setup.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 09:21:45.303820 volsite_postgres_common-0.1.9/src/
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 09:21:45.303820 volsite_postgres_common-0.1.9/src/volsite_postgres_common/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      259 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/Base64Utf8.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 09:21:45.307819 volsite_postgres_common-0.1.9/src/volsite_postgres_common/api/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     3222 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/api/CA.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/api/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 09:21:45.307819 volsite_postgres_common-0.1.9/src/volsite_postgres_common/api/enum/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/api/enum/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       77 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/api/enum/common_error_code.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      658 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/api/enum/enum.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 09:21:45.307819 volsite_postgres_common-0.1.9/src/volsite_postgres_common/db/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     2124 2023-01-26 09:19:47.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/db/BFn.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      681 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/db/CC.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1037 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/db/CFn.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      410 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/db/FnT.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/db/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      192 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/db/migration.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 09:21:45.307819 volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      513 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/AInsertFunction.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     3114 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/function.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1431 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/general.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     2450 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/id.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      133 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/insert.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     5160 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/json.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1486 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/sql_segments.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 09:21:45.307819 volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/title_description/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1527 2023-01-26 08:28:07.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/title_description/APFnUpsertDescription.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1291 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/title_description/APFnUpsertTitle.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     2410 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/title_description/APFnUpsertTitleDescriptionB64.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/title_description/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 09:21:45.307819 volsite_postgres_common-0.1.9/src/volsite_postgres_common/table/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/table/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1203 2023-01-26 07:39:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/table/create_table_descriptions.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1293 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/table/create_table_titles.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      595 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/table/description.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      802 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/table/series.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      951 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/table/text.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 09:21:45.307819 volsite_postgres_common-0.1.9/src/volsite_postgres_common/test/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      515 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/test/Timer.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/test/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      787 2023-01-23 23:33:26.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/test/assert_util.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 09:21:45.311820 volsite_postgres_common-0.1.9/src/volsite_postgres_common/test/db/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      154 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/test/db/ATestDb.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      282 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/test/db/ATestSetUser.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/test/db/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      885 2023-01-22 07:41:08.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common/test/dokuwiki.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-01-26 09:21:45.307819 volsite_postgres_common-0.1.9/src/volsite_postgres_common.egg-info/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      234 2023-01-26 09:21:45.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common.egg-info/PKG-INFO
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     2092 2023-01-26 09:21:45.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        1 2023-01-26 09:21:45.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       15 2023-01-26 09:21:45.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common.egg-info/requires.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       24 2023-01-26 09:21:45.000000 volsite_postgres_common-0.1.9/src/volsite_postgres_common.egg-info/top_level.txt
```

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/api/CA.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/api/CA.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/api/enum/enum.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/api/enum/enum.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/db/BFn.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/db/BFn.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     quote_ident: Final[str] = 'quote_ident'
 
     jsonb_agg: Final[str] = 'jsonb_agg'
     jsonb_array_elements: Final[str] = 'jsonb_array_elements'
     jsonb_array_elements_text: Final[str] = 'jsonb_array_elements_text'
     jsonb_build_array: Final[str] = 'jsonb_build_array'
     jsonb_build_object: Final[str] = 'jsonb_build_object'
+    jsonb_each: Final[str] = 'jsonb_each'
     jsonb_object_agg: Final[str] = 'jsonb_object_agg'
     jsonb_object_keys: Final[str] = 'jsonb_object_keys'
     jsonb_strip_nulls: Final[str] = 'jsonb_strip_nulls'
 
     length: Final[str] = 'length'
 
     nextval: Final[str] = 'nextval'
```

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/db/CC.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/db/CC.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/db/CFn.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/db/CFn.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/AInsertFunction.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/AInsertFunction.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/function.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/function.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/general.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/general.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/id.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/id.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/json.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/json.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/sql_segments.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/sql_segments.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/title_description/APFnUpsertDescription.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/title_description/APFnUpsertDescription.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/title_description/APFnUpsertTitle.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/title_description/APFnUpsertTitle.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/fn/title_description/APFnUpsertTitleDescriptionB64.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/fn/title_description/APFnUpsertTitleDescriptionB64.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/table/create_table_descriptions.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/table/create_table_descriptions.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/table/create_table_titles.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/table/create_table_titles.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/table/description.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/table/description.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/table/series.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/table/series.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/table/text.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/table/text.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/test/Timer.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/test/Timer.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/test/assert_util.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/test/assert_util.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common/test/dokuwiki.py` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common/test/dokuwiki.py`

 * *Files identical despite different names*

### Comparing `volsite_postgres_common-0.1.8/src/volsite_postgres_common.egg-info/SOURCES.txt` & `volsite_postgres_common-0.1.9/src/volsite_postgres_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

