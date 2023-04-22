# Comparing `tmp/medium-api-0.5.2.tar.gz` & `tmp/medium-api-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium-api-0.5.2.tar", last modified: Sat Apr 22 17:30:48 2023, max compression
+gzip compressed data, was "medium-api-0.5.3.tar", last modified: Sat Apr 22 19:02:18 2023, max compression
```

## Comparing `medium-api-0.5.2.tar` & `medium-api-0.5.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 17:30:48.386204 medium-api-0.5.2/
--rw-r--r--   0 sanskar    (501) staff       (20)     1069 2022-01-02 12:36:51.000000 medium-api-0.5.2/LICENSE
--rw-r--r--   0 sanskar    (501) staff       (20)      232 2022-01-21 06:51:28.000000 medium-api-0.5.2/MANIFEST.in
--rw-r--r--   0 sanskar    (501) staff       (20)     6221 2023-04-22 17:30:48.386330 medium-api-0.5.2/PKG-INFO
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 17:30:48.359871 medium-api-0.5.2/docs/
--rw-r--r--   0 sanskar    (501) staff       (20)      611 2022-02-27 09:33:04.000000 medium-api-0.5.2/docs/Makefile
--rw-r--r--   0 sanskar    (501) staff       (20)     5287 2023-01-28 20:04:36.000000 medium-api-0.5.2/docs/README.rst
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 17:30:48.351778 medium-api-0.5.2/docs/_build/
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 17:30:48.351852 medium-api-0.5.2/docs/_build/html/
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 17:30:48.363593 medium-api-0.5.2/docs/_build/html/_static/
--rw-r--r--   0 sanskar    (501) staff       (20)   378551 2022-02-28 09:45:28.000000 medium-api-0.5.2/docs/_build/html/_static/MediumAPI-Banner.png
--rw-r--r--   0 sanskar    (501) staff       (20)   116988 2022-04-10 13:29:20.000000 medium-api-0.5.2/docs/_build/html/_static/MediumAPI-GettingStarted-Thumbnail.png
--rw-r--r--   0 sanskar    (501) staff       (20)      286 2022-01-17 09:33:23.000000 medium-api-0.5.2/docs/_build/html/_static/file.png
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 17:30:48.367210 medium-api-0.5.2/docs/_build/html/_static/logos/
--rw-r--r--   0 sanskar    (501) staff       (20)    26295 2022-02-04 15:57:31.000000 medium-api-0.5.2/docs/_build/html/_static/logos/Logo-encircled-no-background.png
--rw-r--r--   0 sanskar    (501) staff       (20)   275759 2022-02-04 15:54:27.000000 medium-api-0.5.2/docs/_build/html/_static/logos/Logo-encircled.png
--rw-r--r--   0 sanskar    (501) staff       (20)    25218 2022-02-28 05:20:48.000000 medium-api-0.5.2/docs/_build/html/_static/logos/Logo-with_name-no_background.png
--rw-r--r--   0 sanskar    (501) staff       (20)   303096 2022-02-28 05:20:07.000000 medium-api-0.5.2/docs/_build/html/_static/logos/Logo-with_name.png
--rw-r--r--   0 sanskar    (501) staff       (20)    16128 2022-02-04 15:08:14.000000 medium-api-0.5.2/docs/_build/html/_static/logos/Logo.png
--rw-r--r--   0 sanskar    (501) staff       (20)       90 2022-01-17 09:33:23.000000 medium-api-0.5.2/docs/_build/html/_static/minus.png
--rw-r--r--   0 sanskar    (501) staff       (20)       90 2022-01-17 09:33:23.000000 medium-api-0.5.2/docs/_build/html/_static/plus.png
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 17:30:48.369358 medium-api-0.5.2/docs/_static/
--rw-r--r--   0 sanskar    (501) staff       (20)   378551 2022-02-28 09:45:28.000000 medium-api-0.5.2/docs/_static/MediumAPI-Banner.png
--rw-r--r--   0 sanskar    (501) staff       (20)   116988 2022-04-10 13:29:20.000000 medium-api-0.5.2/docs/_static/MediumAPI-GettingStarted-Thumbnail.png
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 17:30:48.375891 medium-api-0.5.2/docs/_static/logos/
--rw-rw-rw-   0 sanskar    (501) staff       (20)    26295 2022-02-04 15:57:31.000000 medium-api-0.5.2/docs/_static/logos/Logo-encircled-no-background.png
--rw-rw-rw-   0 sanskar    (501) staff       (20)   275759 2022-02-04 15:54:27.000000 medium-api-0.5.2/docs/_static/logos/Logo-encircled.png
--rw-r--r--   0 sanskar    (501) staff       (20)    25218 2022-02-28 05:20:48.000000 medium-api-0.5.2/docs/_static/logos/Logo-with_name-no_background.png
--rw-r--r--   0 sanskar    (501) staff       (20)   303096 2022-02-28 05:20:07.000000 medium-api-0.5.2/docs/_static/logos/Logo-with_name.png
--rw-r--r--   0 sanskar    (501) staff       (20)    16128 2022-02-04 15:08:14.000000 medium-api-0.5.2/docs/_static/logos/Logo.png
--rw-r--r--   0 sanskar    (501) staff       (20)      154 2022-02-28 10:17:36.000000 medium-api-0.5.2/docs/authors.rst
--rwxr-xr-x   0 sanskar    (501) staff       (20)     5256 2022-02-28 10:04:39.000000 medium-api-0.5.2/docs/conf.py
--rw-r--r--   0 sanskar    (501) staff       (20)     3501 2022-02-27 09:29:20.000000 medium-api-0.5.2/docs/contributing.rst
--rw-r--r--   0 sanskar    (501) staff       (20)      855 2023-04-02 23:24:30.000000 medium-api-0.5.2/docs/documentation.rst
--rw-r--r--   0 sanskar    (501) staff       (20)      420 2022-02-07 11:18:24.000000 medium-api-0.5.2/docs/index.rst
--rw-r--r--   0 sanskar    (501) staff       (20)     1158 2022-02-27 09:18:02.000000 medium-api-0.5.2/docs/installation.rst
--rw-r--r--   0 sanskar    (501) staff       (20)      772 2022-02-27 09:32:51.000000 medium-api-0.5.2/docs/make.bat
--rw-r--r--   0 sanskar    (501) staff       (20)    34500 2022-02-27 09:32:17.000000 medium-api-0.5.2/docs/terms_of_use.rst
--rw-r--r--   0 sanskar    (501) staff       (20)    10462 2023-04-12 09:28:54.000000 medium-api-0.5.2/docs/usage.rst
--rw-r--r--   0 sanskar    (501) staff       (20)       89 2022-01-16 18:16:53.000000 medium-api-0.5.2/pyproject.toml
--rw-r--r--   0 sanskar    (501) staff       (20)       33 2022-02-01 20:42:59.000000 medium-api-0.5.2/requirements-dev.txt
--rw-r--r--   0 sanskar    (501) staff       (20)        0 2023-01-26 20:03:14.000000 medium-api-0.5.2/requirements.txt
--rw-r--r--   0 sanskar    (501) staff       (20)     1045 2023-04-22 17:30:48.386893 medium-api-0.5.2/setup.cfg
--rw-r--r--   0 sanskar    (501) staff       (20)       61 2022-01-16 19:30:09.000000 medium-api-0.5.2/setup.py
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 17:30:48.352448 medium-api-0.5.2/src/
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 17:30:48.379304 medium-api-0.5.2/src/medium_api/
--rw-r--r--   0 sanskar    (501) staff       (20)      157 2023-04-22 17:30:48.000000 medium-api-0.5.2/src/medium_api/__init__.py
--rw-r--r--   0 sanskar    (501) staff       (20)    15261 2023-04-12 09:31:29.000000 medium-api-0.5.2/src/medium_api/_article.py
--rw-r--r--   0 sanskar    (501) staff       (20)     3013 2023-03-30 10:20:57.000000 medium-api-0.5.2/src/medium_api/_latestposts.py
--rw-r--r--   0 sanskar    (501) staff       (20)     8382 2023-04-02 21:00:13.000000 medium-api-0.5.2/src/medium_api/_medium_list.py
--rw-r--r--   0 sanskar    (501) staff       (20)    11527 2023-03-30 10:20:44.000000 medium-api-0.5.2/src/medium_api/_publication.py
--rw-r--r--   0 sanskar    (501) staff       (20)     2450 2023-03-30 10:20:19.000000 medium-api-0.5.2/src/medium_api/_top_writers.py
--rw-r--r--   0 sanskar    (501) staff       (20)     3076 2023-03-30 10:21:46.000000 medium-api-0.5.2/src/medium_api/_topfeeds.py
--rw-r--r--   0 sanskar    (501) staff       (20)    16315 2023-04-02 21:02:22.000000 medium-api-0.5.2/src/medium_api/_user.py
--rw-r--r--   0 sanskar    (501) staff       (20)    26743 2023-04-22 17:29:30.000000 medium-api-0.5.2/src/medium_api/medium.py
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 17:30:48.380595 medium-api-0.5.2/src/medium_api.egg-info/
--rw-r--r--   0 sanskar    (501) staff       (20)     6221 2023-04-22 17:30:48.000000 medium-api-0.5.2/src/medium_api.egg-info/PKG-INFO
--rw-r--r--   0 sanskar    (501) staff       (20)     1740 2023-04-22 17:30:48.000000 medium-api-0.5.2/src/medium_api.egg-info/SOURCES.txt
--rw-r--r--   0 sanskar    (501) staff       (20)        1 2023-04-22 17:30:48.000000 medium-api-0.5.2/src/medium_api.egg-info/dependency_links.txt
--rw-r--r--   0 sanskar    (501) staff       (20)       11 2023-04-22 17:30:48.000000 medium-api-0.5.2/src/medium_api.egg-info/top_level.txt
--rw-r--r--   0 sanskar    (501) staff       (20)        1 2022-07-27 13:19:52.000000 medium-api-0.5.2/src/medium_api.egg-info/zip-safe
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 17:30:48.385831 medium-api-0.5.2/tests/
--rw-r--r--   0 sanskar    (501) staff       (20)     6148 2022-02-27 12:41:15.000000 medium-api-0.5.2/tests/.DS_Store
--rw-r--r--   0 sanskar    (501) staff       (20)        0 2022-01-16 17:06:47.000000 medium-api-0.5.2/tests/__init__.py
--rw-r--r--   0 sanskar    (501) staff       (20)     3578 2023-04-12 09:09:51.000000 medium-api-0.5.2/tests/test_article.py
--rw-r--r--   0 sanskar    (501) staff       (20)     1161 2022-07-22 09:09:55.000000 medium-api-0.5.2/tests/test_latestposts.py
--rw-r--r--   0 sanskar    (501) staff       (20)     2255 2023-03-28 12:57:03.000000 medium-api-0.5.2/tests/test_medium_list.py
--rw-r--r--   0 sanskar    (501) staff       (20)     2610 2022-11-30 08:22:20.000000 medium-api-0.5.2/tests/test_publication.py
--rw-r--r--   0 sanskar    (501) staff       (20)     1230 2023-03-30 19:21:06.000000 medium-api-0.5.2/tests/test_search.py
--rw-r--r--   0 sanskar    (501) staff       (20)      710 2023-04-02 23:13:37.000000 medium-api-0.5.2/tests/test_tag.py
--rw-r--r--   0 sanskar    (501) staff       (20)      877 2023-02-17 11:23:49.000000 medium-api-0.5.2/tests/test_top_writers.py
--rw-r--r--   0 sanskar    (501) staff       (20)     1010 2023-02-14 17:43:26.000000 medium-api-0.5.2/tests/test_topfeeds.py
--rw-r--r--   0 sanskar    (501) staff       (20)     4162 2023-03-30 10:58:55.000000 medium-api-0.5.2/tests/test_user.py
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.856478 medium-api-0.5.3/
+-rw-r--r--   0 sanskar    (501) staff       (20)     1069 2022-01-02 12:36:51.000000 medium-api-0.5.3/LICENSE
+-rw-r--r--   0 sanskar    (501) staff       (20)      232 2022-01-21 06:51:28.000000 medium-api-0.5.3/MANIFEST.in
+-rw-r--r--   0 sanskar    (501) staff       (20)     6221 2023-04-22 19:02:18.856590 medium-api-0.5.3/PKG-INFO
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.823637 medium-api-0.5.3/docs/
+-rw-r--r--   0 sanskar    (501) staff       (20)      611 2022-02-27 09:33:04.000000 medium-api-0.5.3/docs/Makefile
+-rw-r--r--   0 sanskar    (501) staff       (20)     5287 2023-01-28 20:04:36.000000 medium-api-0.5.3/docs/README.rst
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.816239 medium-api-0.5.3/docs/_build/
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.816287 medium-api-0.5.3/docs/_build/html/
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.827598 medium-api-0.5.3/docs/_build/html/_static/
+-rw-r--r--   0 sanskar    (501) staff       (20)   378551 2022-02-28 09:45:28.000000 medium-api-0.5.3/docs/_build/html/_static/MediumAPI-Banner.png
+-rw-r--r--   0 sanskar    (501) staff       (20)   116988 2022-04-10 13:29:20.000000 medium-api-0.5.3/docs/_build/html/_static/MediumAPI-GettingStarted-Thumbnail.png
+-rw-r--r--   0 sanskar    (501) staff       (20)      286 2022-01-17 09:33:23.000000 medium-api-0.5.3/docs/_build/html/_static/file.png
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.830605 medium-api-0.5.3/docs/_build/html/_static/logos/
+-rw-r--r--   0 sanskar    (501) staff       (20)    26295 2022-02-04 15:57:31.000000 medium-api-0.5.3/docs/_build/html/_static/logos/Logo-encircled-no-background.png
+-rw-r--r--   0 sanskar    (501) staff       (20)   275759 2022-02-04 15:54:27.000000 medium-api-0.5.3/docs/_build/html/_static/logos/Logo-encircled.png
+-rw-r--r--   0 sanskar    (501) staff       (20)    25218 2022-02-28 05:20:48.000000 medium-api-0.5.3/docs/_build/html/_static/logos/Logo-with_name-no_background.png
+-rw-r--r--   0 sanskar    (501) staff       (20)   303096 2022-02-28 05:20:07.000000 medium-api-0.5.3/docs/_build/html/_static/logos/Logo-with_name.png
+-rw-r--r--   0 sanskar    (501) staff       (20)    16128 2022-02-04 15:08:14.000000 medium-api-0.5.3/docs/_build/html/_static/logos/Logo.png
+-rw-r--r--   0 sanskar    (501) staff       (20)       90 2022-01-17 09:33:23.000000 medium-api-0.5.3/docs/_build/html/_static/minus.png
+-rw-r--r--   0 sanskar    (501) staff       (20)       90 2022-01-17 09:33:23.000000 medium-api-0.5.3/docs/_build/html/_static/plus.png
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.832046 medium-api-0.5.3/docs/_static/
+-rw-r--r--   0 sanskar    (501) staff       (20)   378551 2022-02-28 09:45:28.000000 medium-api-0.5.3/docs/_static/MediumAPI-Banner.png
+-rw-r--r--   0 sanskar    (501) staff       (20)   116988 2022-04-10 13:29:20.000000 medium-api-0.5.3/docs/_static/MediumAPI-GettingStarted-Thumbnail.png
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.843136 medium-api-0.5.3/docs/_static/logos/
+-rw-rw-rw-   0 sanskar    (501) staff       (20)    26295 2022-02-04 15:57:31.000000 medium-api-0.5.3/docs/_static/logos/Logo-encircled-no-background.png
+-rw-rw-rw-   0 sanskar    (501) staff       (20)   275759 2022-02-04 15:54:27.000000 medium-api-0.5.3/docs/_static/logos/Logo-encircled.png
+-rw-r--r--   0 sanskar    (501) staff       (20)    25218 2022-02-28 05:20:48.000000 medium-api-0.5.3/docs/_static/logos/Logo-with_name-no_background.png
+-rw-r--r--   0 sanskar    (501) staff       (20)   303096 2022-02-28 05:20:07.000000 medium-api-0.5.3/docs/_static/logos/Logo-with_name.png
+-rw-r--r--   0 sanskar    (501) staff       (20)    16128 2022-02-04 15:08:14.000000 medium-api-0.5.3/docs/_static/logos/Logo.png
+-rw-r--r--   0 sanskar    (501) staff       (20)      154 2022-02-28 10:17:36.000000 medium-api-0.5.3/docs/authors.rst
+-rwxr-xr-x   0 sanskar    (501) staff       (20)     5256 2022-02-28 10:04:39.000000 medium-api-0.5.3/docs/conf.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     3501 2022-02-27 09:29:20.000000 medium-api-0.5.3/docs/contributing.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)      855 2023-04-02 23:24:30.000000 medium-api-0.5.3/docs/documentation.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)      420 2022-02-07 11:18:24.000000 medium-api-0.5.3/docs/index.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)     1158 2022-02-27 09:18:02.000000 medium-api-0.5.3/docs/installation.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)      772 2022-02-27 09:32:51.000000 medium-api-0.5.3/docs/make.bat
+-rw-r--r--   0 sanskar    (501) staff       (20)    34500 2022-02-27 09:32:17.000000 medium-api-0.5.3/docs/terms_of_use.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)    10462 2023-04-12 09:28:54.000000 medium-api-0.5.3/docs/usage.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)       89 2022-01-16 18:16:53.000000 medium-api-0.5.3/pyproject.toml
+-rw-r--r--   0 sanskar    (501) staff       (20)       33 2022-02-01 20:42:59.000000 medium-api-0.5.3/requirements-dev.txt
+-rw-r--r--   0 sanskar    (501) staff       (20)        0 2023-01-26 20:03:14.000000 medium-api-0.5.3/requirements.txt
+-rw-r--r--   0 sanskar    (501) staff       (20)     1045 2023-04-22 19:02:18.858886 medium-api-0.5.3/setup.cfg
+-rw-r--r--   0 sanskar    (501) staff       (20)       61 2022-01-16 19:30:09.000000 medium-api-0.5.3/setup.py
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.816674 medium-api-0.5.3/src/
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.846115 medium-api-0.5.3/src/medium_api/
+-rw-r--r--   0 sanskar    (501) staff       (20)      157 2023-04-22 19:02:18.000000 medium-api-0.5.3/src/medium_api/__init__.py
+-rw-r--r--   0 sanskar    (501) staff       (20)    15261 2023-04-12 09:31:29.000000 medium-api-0.5.3/src/medium_api/_article.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     3013 2023-03-30 10:20:57.000000 medium-api-0.5.3/src/medium_api/_latestposts.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     8382 2023-04-02 21:00:13.000000 medium-api-0.5.3/src/medium_api/_medium_list.py
+-rw-r--r--   0 sanskar    (501) staff       (20)    11527 2023-03-30 10:20:44.000000 medium-api-0.5.3/src/medium_api/_publication.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     2450 2023-03-30 10:20:19.000000 medium-api-0.5.3/src/medium_api/_top_writers.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     3076 2023-03-30 10:21:46.000000 medium-api-0.5.3/src/medium_api/_topfeeds.py
+-rw-r--r--   0 sanskar    (501) staff       (20)    16393 2023-04-22 17:34:09.000000 medium-api-0.5.3/src/medium_api/_user.py
+-rw-r--r--   0 sanskar    (501) staff       (20)    26743 2023-04-22 19:01:46.000000 medium-api-0.5.3/src/medium_api/medium.py
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.848402 medium-api-0.5.3/src/medium_api.egg-info/
+-rw-r--r--   0 sanskar    (501) staff       (20)     6221 2023-04-22 19:02:18.000000 medium-api-0.5.3/src/medium_api.egg-info/PKG-INFO
+-rw-r--r--   0 sanskar    (501) staff       (20)     1740 2023-04-22 19:02:18.000000 medium-api-0.5.3/src/medium_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sanskar    (501) staff       (20)        1 2023-04-22 19:02:18.000000 medium-api-0.5.3/src/medium_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sanskar    (501) staff       (20)       11 2023-04-22 19:02:18.000000 medium-api-0.5.3/src/medium_api.egg-info/top_level.txt
+-rw-r--r--   0 sanskar    (501) staff       (20)        1 2022-07-27 13:19:52.000000 medium-api-0.5.3/src/medium_api.egg-info/zip-safe
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.856133 medium-api-0.5.3/tests/
+-rw-r--r--   0 sanskar    (501) staff       (20)     6148 2022-02-27 12:41:15.000000 medium-api-0.5.3/tests/.DS_Store
+-rw-r--r--   0 sanskar    (501) staff       (20)        0 2022-01-16 17:06:47.000000 medium-api-0.5.3/tests/__init__.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     3578 2023-04-12 09:09:51.000000 medium-api-0.5.3/tests/test_article.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     1161 2022-07-22 09:09:55.000000 medium-api-0.5.3/tests/test_latestposts.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     2255 2023-03-28 12:57:03.000000 medium-api-0.5.3/tests/test_medium_list.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     2610 2022-11-30 08:22:20.000000 medium-api-0.5.3/tests/test_publication.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     1230 2023-03-30 19:21:06.000000 medium-api-0.5.3/tests/test_search.py
+-rw-r--r--   0 sanskar    (501) staff       (20)      710 2023-04-02 23:13:37.000000 medium-api-0.5.3/tests/test_tag.py
+-rw-r--r--   0 sanskar    (501) staff       (20)      877 2023-02-17 11:23:49.000000 medium-api-0.5.3/tests/test_top_writers.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     1010 2023-02-14 17:43:26.000000 medium-api-0.5.3/tests/test_topfeeds.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     4162 2023-03-30 10:58:55.000000 medium-api-0.5.3/tests/test_user.py
```

### Comparing `medium-api-0.5.2/LICENSE` & `medium-api-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/PKG-INFO` & `medium-api-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medium-api
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python Wrapper on top of Medium API to quickly extract data from https://medium.com.
 Home-page: https://github.com/weeping-angel/medium-api
 Author: Nishu Jain
 Author-email: nishujain1997.19@gmail.com
 License: MIT
 Platform: unix
 Platform: linux
```

### Comparing `medium-api-0.5.2/docs/Makefile` & `medium-api-0.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/README.rst` & `medium-api-0.5.3/docs/README.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/_build/html/_static/MediumAPI-Banner.png` & `medium-api-0.5.3/docs/_build/html/_static/MediumAPI-Banner.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/_build/html/_static/MediumAPI-GettingStarted-Thumbnail.png` & `medium-api-0.5.3/docs/_build/html/_static/MediumAPI-GettingStarted-Thumbnail.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/_build/html/_static/logos/Logo-encircled-no-background.png` & `medium-api-0.5.3/docs/_build/html/_static/logos/Logo-encircled-no-background.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/_build/html/_static/logos/Logo-encircled.png` & `medium-api-0.5.3/docs/_build/html/_static/logos/Logo-encircled.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/_build/html/_static/logos/Logo-with_name-no_background.png` & `medium-api-0.5.3/docs/_build/html/_static/logos/Logo-with_name-no_background.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/_build/html/_static/logos/Logo-with_name.png` & `medium-api-0.5.3/docs/_build/html/_static/logos/Logo-with_name.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/_build/html/_static/logos/Logo.png` & `medium-api-0.5.3/docs/_build/html/_static/logos/Logo.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/_static/MediumAPI-Banner.png` & `medium-api-0.5.3/docs/_static/MediumAPI-Banner.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/_static/MediumAPI-GettingStarted-Thumbnail.png` & `medium-api-0.5.3/docs/_static/MediumAPI-GettingStarted-Thumbnail.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/_static/logos/Logo-encircled-no-background.png` & `medium-api-0.5.3/docs/_static/logos/Logo-encircled-no-background.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/_static/logos/Logo-encircled.png` & `medium-api-0.5.3/docs/_static/logos/Logo-encircled.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/_static/logos/Logo-with_name-no_background.png` & `medium-api-0.5.3/docs/_static/logos/Logo-with_name-no_background.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/_static/logos/Logo-with_name.png` & `medium-api-0.5.3/docs/_static/logos/Logo-with_name.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/_static/logos/Logo.png` & `medium-api-0.5.3/docs/_static/logos/Logo.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/conf.py` & `medium-api-0.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/contributing.rst` & `medium-api-0.5.3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/documentation.rst` & `medium-api-0.5.3/docs/documentation.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/installation.rst` & `medium-api-0.5.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/make.bat` & `medium-api-0.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/terms_of_use.rst` & `medium-api-0.5.3/docs/terms_of_use.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/docs/usage.rst` & `medium-api-0.5.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/setup.cfg` & `medium-api-0.5.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = medium-api
 description = Python Wrapper on top of Medium API to quickly extract data from https://medium.com.
-version = 0.5.2
+version = 0.5.3
 long_description = file: docs/README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/weeping-angel/medium-api
 author = Nishu Jain
 author_email = nishujain1997.19@gmail.com
 platforms = unix, linux, osx, win32, cygwin
 description_file = README.rst
```

### Comparing `medium-api-0.5.2/src/medium_api/_article.py` & `medium-api-0.5.3/src/medium_api/_article.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/src/medium_api/_latestposts.py` & `medium-api-0.5.3/src/medium_api/_latestposts.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/src/medium_api/_medium_list.py` & `medium-api-0.5.3/src/medium_api/_medium_list.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/src/medium_api/_publication.py` & `medium-api-0.5.3/src/medium_api/_publication.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/src/medium_api/_top_writers.py` & `medium-api-0.5.3/src/medium_api/_top_writers.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/src/medium_api/_topfeeds.py` & `medium-api-0.5.3/src/medium_api/_topfeeds.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/src/medium_api/_user.py` & `medium-api-0.5.3/src/medium_api/_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,14 +361,16 @@
                 - ``user.username``
                 - ``user.followers_count``
                 - ``user.following_count``
                 - ``user.bio``
                 - ``user.twitter_username``
                 - ``user.is_writer_program_enrolled``
                 - ``user.is_suspended``
+                - ``user.has_list``
+                - ``user.is_book_author``
                 - ``user.allow_notes``
                 - ``user.medium_member_at``
                 - ``user.top_writer_in``
                 - ``user.image_url``
         """
         user = self.info
```

### Comparing `medium-api-0.5.2/src/medium_api/medium.py` & `medium-api-0.5.3/src/medium_api/medium.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,15 +566,15 @@
                 the article as well. Otherwise, default is `False`
 
         Returns:
             None: This method doesn't return anything since it fills the values in the passed
             list of Article(s) objects itself.
 
         """
-        with ThreadPoolExecutor(max_workers=20) as executor:
+        with ThreadPoolExecutor(max_workers=10) as executor:
             future_to_url = [executor.submit(article.save_info) for article in articles if article.title is None]
             if content:
                 future_to_url += [executor.submit(article.save_content) for article in articles]
 
             for future in as_completed(future_to_url):
                 future.result()
     
@@ -591,15 +591,15 @@
             publications (list[Publication]): List of (empty) Publications objects to fill information into it.
 
         Returns:
             None: This method doesn't return anything since it fills the values in the passed
             list of Publication(s) objects itself.
 
         """
-        with ThreadPoolExecutor(max_workers=20) as executor:
+        with ThreadPoolExecutor(max_workers=10) as executor:
             future_to_url = [executor.submit(publication.save_info) for publication in publications if publication.name is None]
 
             for future in as_completed(future_to_url):
                 future.result()
 
     def fetch_lists(self, medium_lists:list):
         """To quickly fetch Medium List related info using multithreading
@@ -614,15 +614,15 @@
             medium_lists (list[MediumList]): An array of (empty) `MediumList` objects to fill information into it.
 
         Returns:
             None: This method doesn't return anything since it fills the values in the passed
             array of MediumList(s) objects itself.
 
         """
-        with ThreadPoolExecutor(max_workers=20) as executor:
+        with ThreadPoolExecutor(max_workers=10) as executor:
             future_to_url = [executor.submit(medium_list.save_info) 
                              for medium_list in medium_lists 
                              if medium_list.name is None]
 
             for future in as_completed(future_to_url):
                 future.result()
 
@@ -639,15 +639,15 @@
             users (list[User]): List of (empty) User objects to fill information into it.
 
         Returns:
             None: This method doesn't return anything since it fills the values into the 
             passed list of User(s) objects itself.
 
         """
-        with ThreadPoolExecutor(max_workers=20) as executor:
+        with ThreadPoolExecutor(max_workers=10) as executor:
             future_to_url = (executor.submit(user.save_info) for user in users if user.fullname is None)
 
             for future in as_completed(future_to_url):
                 future.result()
 
     def extract_article_id(self, article_url:str):
         """To get `article_id` from the Article's URL
```

### Comparing `medium-api-0.5.2/src/medium_api.egg-info/PKG-INFO` & `medium-api-0.5.3/src/medium_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medium-api
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python Wrapper on top of Medium API to quickly extract data from https://medium.com.
 Home-page: https://github.com/weeping-angel/medium-api
 Author: Nishu Jain
 Author-email: nishujain1997.19@gmail.com
 License: MIT
 Platform: unix
 Platform: linux
```

### Comparing `medium-api-0.5.2/src/medium_api.egg-info/SOURCES.txt` & `medium-api-0.5.3/src/medium_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/tests/.DS_Store` & `medium-api-0.5.3/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/tests/test_article.py` & `medium-api-0.5.3/tests/test_article.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/tests/test_latestposts.py` & `medium-api-0.5.3/tests/test_latestposts.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/tests/test_medium_list.py` & `medium-api-0.5.3/tests/test_medium_list.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/tests/test_publication.py` & `medium-api-0.5.3/tests/test_publication.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/tests/test_search.py` & `medium-api-0.5.3/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/tests/test_tag.py` & `medium-api-0.5.3/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/tests/test_top_writers.py` & `medium-api-0.5.3/tests/test_top_writers.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/tests/test_topfeeds.py` & `medium-api-0.5.3/tests/test_topfeeds.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.2/tests/test_user.py` & `medium-api-0.5.3/tests/test_user.py`

 * *Files identical despite different names*

