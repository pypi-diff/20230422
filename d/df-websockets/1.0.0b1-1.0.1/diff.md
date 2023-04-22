# Comparing `tmp/df_websockets-1.0.0b1.tar.gz` & `tmp/df_websockets-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/df_websockets-1.0.0b1.tar", last modified: Mon Aug 29 19:52:24 2022, max compression
+gzip compressed data, was "df_websockets-1.0.1.tar", last modified: Sat Apr 22 14:01:34 2023, max compression
```

## Comparing `df_websockets-1.0.0b1.tar` & `df_websockets-1.0.1.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2022-08-29 19:52:24.310690 df_websockets-1.0.0b1/
--rw-r--r--   0 flanker    (501) staff       (20)      935 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/.gitignore
--rw-r--r--   0 flanker    (501) staff       (20)      478 2021-03-25 18:53:48.000000 df_websockets-1.0.0b1/.travis.yml
--rw-r--r--   0 flanker    (501) staff       (20)    21393 2020-11-04 09:00:51.000000 df_websockets-1.0.0b1/LICENSE
--rw-r--r--   0 flanker    (501) staff       (20)      105 2020-11-04 09:00:51.000000 df_websockets-1.0.0b1/MANIFEST.in
--rw-r--r--   0 flanker    (501) staff       (20)    19164 2022-08-29 19:52:24.310947 df_websockets-1.0.0b1/PKG-INFO
--rw-r--r--   0 flanker    (501) staff       (20)    17893 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/README.md
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2022-08-29 19:52:24.274325 df_websockets-1.0.0b1/demo_df_websockets/
--rw-r--r--   0 flanker    (501) staff       (20)        0 2021-03-21 22:05:43.000000 df_websockets-1.0.0b1/demo_df_websockets/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     5682 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/demo_df_websockets/settings.py
--rw-r--r--   0 flanker    (501) staff       (20)     5475 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/demo_df_websockets/signals.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2022-08-29 19:52:24.276386 df_websockets-1.0.0b1/demo_df_websockets/static/
--rw-r--r--   0 flanker    (501) staff       (20)      224 2021-03-23 21:50:25.000000 df_websockets-1.0.0b1/demo_df_websockets/static/demo.css
--rw-r--r--   0 flanker    (501) staff       (20)      329 2021-03-21 23:06:30.000000 df_websockets-1.0.0b1/demo_df_websockets/static/demo.js
--rw-r--r--   0 flanker    (501) staff       (20)    15390 2021-03-22 07:04:44.000000 df_websockets-1.0.0b1/demo_df_websockets/static/image.png
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2022-08-29 19:52:24.277069 df_websockets-1.0.0b1/demo_df_websockets/templates/
--rw-r--r--   0 flanker    (501) staff       (20)    29153 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/demo_df_websockets/templates/index.html
--rw-r--r--   0 flanker    (501) staff       (20)      769 2021-03-22 21:11:59.000000 df_websockets-1.0.0b1/demo_df_websockets/urls.py
--rw-r--r--   0 flanker    (501) staff       (20)      215 2021-03-22 21:12:10.000000 df_websockets-1.0.0b1/demo_df_websockets/views.py
--rwxr-xr-x   0 flanker    (501) staff       (20)      334 2021-03-22 21:12:59.000000 df_websockets-1.0.0b1/demo_manage.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2022-08-29 19:52:24.283121 df_websockets-1.0.0b1/df_websockets/
--rw-r--r--   0 flanker    (501) staff       (20)     1239 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     2900 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/celery.py
--rw-r--r--   0 flanker    (501) staff       (20)     1471 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/constants.py
--rw-r--r--   0 flanker    (501) staff       (20)     8228 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/consumers.py
--rw-r--r--   0 flanker    (501) staff       (20)    13765 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/decorators.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2022-08-29 19:52:24.286510 df_websockets-1.0.0b1/df_websockets/management/
--rw-r--r--   0 flanker    (501) staff       (20)     1215 2022-01-09 14:49:12.000000 df_websockets-1.0.0b1/df_websockets/management/__init__.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2022-08-29 19:52:24.289241 df_websockets-1.0.0b1/df_websockets/management/commands/
--rw-r--r--   0 flanker    (501) staff       (20)     1215 2022-01-09 14:49:12.000000 df_websockets-1.0.0b1/df_websockets/management/commands/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     1685 2022-01-09 14:49:12.000000 df_websockets-1.0.0b1/df_websockets/management/commands/celery.py
--rw-r--r--   0 flanker    (501) staff       (20)     3489 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/management/commands/worker.py
--rw-r--r--   0 flanker    (501) staff       (20)     3829 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/middleware.py
--rw-r--r--   0 flanker    (501) staff       (20)     1989 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/routing.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2022-08-29 19:52:24.266568 df_websockets-1.0.0b1/df_websockets/static/
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2022-08-29 19:52:24.290403 df_websockets-1.0.0b1/df_websockets/static/js/
--rw-r--r--   0 flanker    (501) staff       (20)     7866 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/static/js/df_websockets.min.js
--rw-r--r--   0 flanker    (501) staff       (20)    44971 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/static/js/df_websockets.min.js.map
--rw-r--r--   0 flanker    (501) staff       (20)    16854 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/tasks.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2022-08-29 19:52:24.291934 df_websockets-1.0.0b1/df_websockets/templatetags/
--rw-r--r--   0 flanker    (501) staff       (20)     1215 2022-01-09 14:49:12.000000 df_websockets-1.0.0b1/df_websockets/templatetags/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     2579 2022-01-09 14:49:12.000000 df_websockets-1.0.0b1/df_websockets/templatetags/websockets.py
--rw-r--r--   0 flanker    (501) staff       (20)     5424 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/testing.py
--rw-r--r--   0 flanker    (501) staff       (20)     3039 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/topics.py
--rw-r--r--   0 flanker    (501) staff       (20)     6143 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/utils.py
--rw-r--r--   0 flanker    (501) staff       (20)     5736 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/window_info.py
--rw-r--r--   0 flanker    (501) staff       (20)    11754 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/ws_middleware.py
--rw-r--r--   0 flanker    (501) staff       (20)     3316 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/df_websockets/ws_settings.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2022-08-29 19:52:24.286037 df_websockets-1.0.0b1/df_websockets.egg-info/
--rw-r--r--   0 flanker    (501) staff       (20)    19164 2022-08-29 19:52:23.000000 df_websockets-1.0.0b1/df_websockets.egg-info/PKG-INFO
--rw-r--r--   0 flanker    (501) staff       (20)     1760 2022-08-29 19:52:23.000000 df_websockets-1.0.0b1/df_websockets.egg-info/SOURCES.txt
--rw-r--r--   0 flanker    (501) staff       (20)        1 2022-08-29 19:52:23.000000 df_websockets-1.0.0b1/df_websockets.egg-info/dependency_links.txt
--rw-r--r--   0 flanker    (501) staff       (20)        1 2020-11-21 14:07:31.000000 df_websockets-1.0.0b1/df_websockets.egg-info/not-zip-safe
--rw-r--r--   0 flanker    (501) staff       (20)       78 2022-08-29 19:52:23.000000 df_websockets-1.0.0b1/df_websockets.egg-info/requires.txt
--rw-r--r--   0 flanker    (501) staff       (20)       52 2022-08-29 19:52:23.000000 df_websockets-1.0.0b1/df_websockets.egg-info/top_level.txt
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2022-08-29 19:52:24.295162 df_websockets-1.0.0b1/npm/
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2022-08-29 19:52:24.298342 df_websockets-1.0.0b1/npm/df_websockets/
--rw-r--r--   0 flanker    (501) staff       (20)     5253 2020-11-22 08:17:24.000000 df_websockets-1.0.0b1/npm/df_websockets/app.js
--rw-r--r--   0 flanker    (501) staff       (20)    13295 2022-08-29 15:15:37.000000 df_websockets-1.0.0b1/npm/df_websockets/base.js
--rw-r--r--   0 flanker    (501) staff       (20)    10672 2022-08-29 15:11:10.000000 df_websockets-1.0.0b1/npm/df_websockets/forms.ts
--rw-r--r--   0 flanker    (501) staff       (20)     4494 2021-03-21 21:26:55.000000 df_websockets-1.0.0b1/npm/df_websockets/html.js
--rw-r--r--   0 flanker    (501) staff       (20)   112499 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/npm/package-lock.json
--rw-r--r--   0 flanker    (501) staff       (20)      475 2021-03-25 21:22:08.000000 df_websockets-1.0.0b1/npm/package.json
--rw-r--r--   0 flanker    (501) staff       (20)      256 2021-03-23 20:46:59.000000 df_websockets-1.0.0b1/npm/tsconfig.json
--rw-r--r--   0 flanker    (501) staff       (20)     1963 2020-11-13 20:54:20.000000 df_websockets-1.0.0b1/npm/webpack.config.js
--rwxr-xr-x   0 flanker    (501) staff       (20)     1250 2020-11-04 09:00:51.000000 df_websockets-1.0.0b1/pre-commit.sh
--rw-r--r--   0 flanker    (501) staff       (20)     2736 2022-08-29 19:52:24.312402 df_websockets-1.0.0b1/setup.cfg
--rw-r--r--   0 flanker    (501) staff       (20)     1254 2021-03-24 18:46:39.000000 df_websockets-1.0.0b1/setup.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2022-08-29 19:52:24.310312 df_websockets-1.0.0b1/test_df_websockets/
--rw-r--r--   0 flanker    (501) staff       (20)        0 2020-11-04 09:00:51.000000 df_websockets-1.0.0b1/test_df_websockets/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     5824 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/test_df_websockets/test_consumers.py
--rw-r--r--   0 flanker    (501) staff       (20)     1339 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/test_df_websockets/test_decorators.py
--rw-r--r--   0 flanker    (501) staff       (20)     3350 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/test_df_websockets/test_middleware.py
--rw-r--r--   0 flanker    (501) staff       (20)     1834 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/test_df_websockets/test_testing.py
--rw-r--r--   0 flanker    (501) staff       (20)      414 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/test_df_websockets/test_utils.py
--rw-r--r--   0 flanker    (501) staff       (20)      998 2022-08-29 19:52:16.000000 df_websockets-1.0.0b1/test_df_websockets/test_window_info.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 14:01:34.562182 df_websockets-1.0.1/
+-rw-r--r--   0 flanker    (501) staff       (20)     3094 2023-04-22 13:39:52.000000 df_websockets-1.0.1/.gitignore
+-rw-r--r--   0 flanker    (501) staff       (20)      478 2021-03-25 18:53:48.000000 df_websockets-1.0.1/.travis.yml
+-rw-r--r--   0 flanker    (501) staff       (20)    21393 2020-11-04 09:00:51.000000 df_websockets-1.0.1/LICENSE
+-rw-r--r--   0 flanker    (501) staff       (20)      105 2020-11-04 09:00:51.000000 df_websockets-1.0.1/MANIFEST.in
+-rw-r--r--   0 flanker    (501) staff       (20)    19654 2023-04-22 14:01:34.562489 df_websockets-1.0.1/PKG-INFO
+-rw-r--r--   0 flanker    (501) staff       (20)    18404 2023-04-22 13:38:39.000000 df_websockets-1.0.1/README.md
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 14:01:34.502075 df_websockets-1.0.1/demo_df_websockets/
+-rw-r--r--   0 flanker    (501) staff       (20)        0 2023-01-28 22:42:08.000000 df_websockets-1.0.1/demo_df_websockets/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5682 2023-01-28 22:42:08.000000 df_websockets-1.0.1/demo_df_websockets/settings.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5475 2023-01-28 22:42:08.000000 df_websockets-1.0.1/demo_df_websockets/signals.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 14:01:34.504662 df_websockets-1.0.1/demo_df_websockets/static/
+-rw-r--r--   0 flanker    (501) staff       (20)      224 2023-01-28 22:42:08.000000 df_websockets-1.0.1/demo_df_websockets/static/demo.css
+-rw-r--r--   0 flanker    (501) staff       (20)      329 2023-01-28 22:42:08.000000 df_websockets-1.0.1/demo_df_websockets/static/demo.js
+-rw-r--r--   0 flanker    (501) staff       (20)    15390 2021-03-22 07:04:44.000000 df_websockets-1.0.1/demo_df_websockets/static/image.png
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 14:01:34.505703 df_websockets-1.0.1/demo_df_websockets/templates/
+-rw-r--r--   0 flanker    (501) staff       (20)    29153 2022-08-29 19:52:16.000000 df_websockets-1.0.1/demo_df_websockets/templates/index.html
+-rw-r--r--   0 flanker    (501) staff       (20)      769 2023-01-28 22:42:08.000000 df_websockets-1.0.1/demo_df_websockets/urls.py
+-rw-r--r--   0 flanker    (501) staff       (20)      215 2023-01-28 22:42:08.000000 df_websockets-1.0.1/demo_df_websockets/views.py
+-rwxr-xr-x   0 flanker    (501) staff       (20)      334 2023-01-28 22:42:08.000000 df_websockets-1.0.1/demo_manage.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 14:01:34.539019 df_websockets-1.0.1/df_websockets/
+-rw-r--r--   0 flanker    (501) staff       (20)     1237 2023-04-22 13:39:37.000000 df_websockets-1.0.1/df_websockets/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)      301 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/apps.py
+-rw-r--r--   0 flanker    (501) staff       (20)     2900 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/celery.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1414 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/checks.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1471 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/constants.py
+-rw-r--r--   0 flanker    (501) staff       (20)     8285 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/consumers.py
+-rw-r--r--   0 flanker    (501) staff       (20)    13765 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/decorators.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 14:01:34.544215 df_websockets-1.0.1/df_websockets/management/
+-rw-r--r--   0 flanker    (501) staff       (20)     1215 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/management/__init__.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 14:01:34.546711 df_websockets-1.0.1/df_websockets/management/commands/
+-rw-r--r--   0 flanker    (501) staff       (20)     1215 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/management/commands/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1685 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/management/commands/celery.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3489 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/management/commands/worker.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3829 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/middleware.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1989 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/routing.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 14:01:34.484450 df_websockets-1.0.1/df_websockets/static/
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 14:01:34.548550 df_websockets-1.0.1/df_websockets/static/js/
+-rw-r--r--   0 flanker    (501) staff       (20)     7866 2022-08-29 19:52:16.000000 df_websockets-1.0.1/df_websockets/static/js/df_websockets.min.js
+-rw-r--r--   0 flanker    (501) staff       (20)    44971 2022-08-29 19:52:16.000000 df_websockets-1.0.1/df_websockets/static/js/df_websockets.min.js.map
+-rw-r--r--   0 flanker    (501) staff       (20)    16911 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/tasks.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 14:01:34.550130 df_websockets-1.0.1/df_websockets/templatetags/
+-rw-r--r--   0 flanker    (501) staff       (20)     1215 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/templatetags/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     2579 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/templatetags/websockets.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5424 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/testing.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3039 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/topics.py
+-rw-r--r--   0 flanker    (501) staff       (20)     6143 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/utils.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5736 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/window_info.py
+-rw-r--r--   0 flanker    (501) staff       (20)    11754 2023-01-28 22:42:08.000000 df_websockets-1.0.1/df_websockets/ws_middleware.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3554 2023-04-22 13:58:56.000000 df_websockets-1.0.1/df_websockets/ws_settings.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 14:01:34.543618 df_websockets-1.0.1/df_websockets.egg-info/
+-rw-r--r--   0 flanker    (501) staff       (20)    19654 2023-04-22 14:01:34.000000 df_websockets-1.0.1/df_websockets.egg-info/PKG-INFO
+-rw-r--r--   0 flanker    (501) staff       (20)     1806 2023-04-22 14:01:34.000000 df_websockets-1.0.1/df_websockets.egg-info/SOURCES.txt
+-rw-r--r--   0 flanker    (501) staff       (20)        1 2023-04-22 14:01:34.000000 df_websockets-1.0.1/df_websockets.egg-info/dependency_links.txt
+-rw-r--r--   0 flanker    (501) staff       (20)        1 2020-11-21 14:07:31.000000 df_websockets-1.0.1/df_websockets.egg-info/not-zip-safe
+-rw-r--r--   0 flanker    (501) staff       (20)       78 2023-04-22 14:01:34.000000 df_websockets-1.0.1/df_websockets.egg-info/requires.txt
+-rw-r--r--   0 flanker    (501) staff       (20)       52 2023-04-22 14:01:34.000000 df_websockets-1.0.1/df_websockets.egg-info/top_level.txt
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 14:01:34.554551 df_websockets-1.0.1/npm/
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 14:01:34.557380 df_websockets-1.0.1/npm/df_websockets/
+-rw-r--r--   0 flanker    (501) staff       (20)     5253 2023-01-28 22:42:08.000000 df_websockets-1.0.1/npm/df_websockets/app.js
+-rw-r--r--   0 flanker    (501) staff       (20)    13295 2023-01-28 22:42:08.000000 df_websockets-1.0.1/npm/df_websockets/base.js
+-rw-r--r--   0 flanker    (501) staff       (20)    10672 2023-01-28 22:42:08.000000 df_websockets-1.0.1/npm/df_websockets/forms.ts
+-rw-r--r--   0 flanker    (501) staff       (20)     4494 2023-01-28 22:42:08.000000 df_websockets-1.0.1/npm/df_websockets/html.js
+-rw-r--r--   0 flanker    (501) staff       (20)   112499 2022-08-29 19:52:16.000000 df_websockets-1.0.1/npm/package-lock.json
+-rw-r--r--   0 flanker    (501) staff       (20)      475 2021-03-25 21:22:08.000000 df_websockets-1.0.1/npm/package.json
+-rw-r--r--   0 flanker    (501) staff       (20)      256 2021-03-23 20:46:59.000000 df_websockets-1.0.1/npm/tsconfig.json
+-rw-r--r--   0 flanker    (501) staff       (20)     1963 2023-01-28 22:42:08.000000 df_websockets-1.0.1/npm/webpack.config.js
+-rwxr-xr-x   0 flanker    (501) staff       (20)     1250 2023-01-28 22:42:08.000000 df_websockets-1.0.1/pre-commit.sh
+-rw-r--r--   0 flanker    (501) staff       (20)     2736 2023-04-22 14:01:34.564122 df_websockets-1.0.1/setup.cfg
+-rw-r--r--   0 flanker    (501) staff       (20)     1254 2023-01-28 22:42:08.000000 df_websockets-1.0.1/setup.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 14:01:34.561654 df_websockets-1.0.1/test_df_websockets/
+-rw-r--r--   0 flanker    (501) staff       (20)        0 2023-01-28 22:42:08.000000 df_websockets-1.0.1/test_df_websockets/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5824 2023-01-28 22:42:08.000000 df_websockets-1.0.1/test_df_websockets/test_consumers.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1339 2023-01-28 22:42:08.000000 df_websockets-1.0.1/test_df_websockets/test_decorators.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3350 2023-01-28 22:42:08.000000 df_websockets-1.0.1/test_df_websockets/test_middleware.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1834 2023-01-28 22:42:08.000000 df_websockets-1.0.1/test_df_websockets/test_testing.py
+-rw-r--r--   0 flanker    (501) staff       (20)      414 2023-01-28 22:42:08.000000 df_websockets-1.0.1/test_df_websockets/test_utils.py
+-rw-r--r--   0 flanker    (501) staff       (20)      998 2023-01-28 22:42:08.000000 df_websockets-1.0.1/test_df_websockets/test_window_info.py
```

### Comparing `df_websockets-1.0.0b1/LICENSE` & `df_websockets-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/PKG-INFO` & `df_websockets-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: df_websockets
-Version: 1.0.0b1
+Version: 1.0.1
 Summary: Websocket integration for Django
 Home-page: https://github.com/d9pouces/df_websockets
 Author: Matthieu Gallet
 Author-email: github@19pouces.net
 Maintainer: Matthieu Gallet
 Maintainer-email: github@19pouces.net
 License: CeCILL-B
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
@@ -44,16 +43,16 @@
 Signals are exchanged between the browser window and the server using a single websocket.
 Signals that are triggered by the browser on the server are processed as background tasks (so the websocket endpoint does almost nothing).
 Signals that are triggered by the server can be processed as background tasks on the serveur and as Javascript functions on the browser.
 
 Background processes can use [celery](https://docs.celeryproject.org/en/stable/), [channels](https://pypi.org/project/channels/) workers, or simply different processes or threads.
 
 
-Requirements and installation
------------------------------
+Requirements
+------------
 
 `df_websockets` works with:
 
   * [Python](https://www.python.org) >= 3.6,
   * [django](https://pypi.org/project/Django/) >= 2.0,
   * [channels](https://pypi.org/project/channels/) >= 2.0.
 
@@ -62,14 +61,17 @@
 
   * [redis](https://redis.io) >= 5.0,
   * [channels_redis](https://pypi.org/project/channels-redis/) >= 3.3.
 
 If you want to process signals in Celery tasks rather in Channel workers, you need to setup a Celery infrastructure:
 [Celery setup](https://docs.celeryproject.org/en/stable/django/first-steps-with-django.html).
 
+Installation
+------------
+
 ```bash
 python -m pip install df_websockets
 ```
 
 In your settings, you must add the following values:
 ```python
 # the ASGI application to use with gunicorn or daphne
@@ -172,34 +174,37 @@
 When you trigger a signal on the server, you can target any set topic. All windows featuring this topic will receive this signal.
 
 _For example, assume that multiple clients open a specific article on a blog. At any time, you can open Python shell in a terminal and trigger a signal on all these windows._  
 
 
 ```python
 from df_websockets.tasks import set_websocket_topics
+from django.contrib.auth.models import Group
+from django.template.response import TemplateResponse
 
 def any_view(request):  # this is a standard Django view
     # useful code
-    obj1 = MyModel.objects.get(id=42)
+    obj1 = Group.objects.get(id=42)
     set_websocket_topics(request, [obj1])
     return TemplateResponse("my/template.html", {})  # do not forget to add `js/df_websockets.min.js` to this HTML
 ```
 
 `obj1` must be a Python object that is handled by the `WEBSOCKET_TOPIC_SERIALIZER` function. By default, any string and Django models are valid.
 Each window also has a unique identifier that is automatically added to this list, as well as the connected user id and the `BROADCAST`.
 
 The following code will call the JS function on every browser window having the `obj` topic and to the displayed window.
 ```python
 from df_websockets.tasks import WINDOW, trigger
 from df_websockets.tasks import set_websocket_topics
-
+from django.contrib.auth.models import Group
+from django.http.response import HttpResponse
 def another_view(request, obj_id):
-    obj = MyModel.objects.get(id=42)
+    obj = Group.objects.get(id=42)
     trigger(request, 'myproject.first_signal', to=[WINDOW, obj], content="hello from a view")
-    set_websocket_topics(request, [other_topics])
+    set_websocket_topics(request, ["other topics"])
     return HttpResponse()
 ```
 
 There are three special values:
 
 * `df_websockets.tasks.WINDOW`: the original browser window,
 * `df_websockets.tasks.USER`: all windows currently displayed by the connected user,
@@ -213,19 +218,20 @@
 settings
 --------
 
 There are a few settings:
 
 - `WEBSOCKET_WORKERS`: one of "celery" (use Celery tasks), "channels" (use Channels workers), "multithread" (process signals in threads), "multiprocess" (process signals in new processes).
   The first two choices require at least one valid worker. 
-- `CELERY_DEFAULT_QUEUE` the default queue for signals (`"celery"` by default)
+- `WEBSOCKET_DEFAULT_QUEUE` the default queue for signals (`"celery"` by default)
 
 Other settings are:
-- `WEBSOCKET_REDIS_EXPIRE`: the validity of the association between a websocket connection and the associated topics
-- `WEBSOCKET_REDIS_PREFIX`: prefix of keys used to cache data
+- `WEBSOCKET_CACHE_EXPIRE`: the validity of the association between a websocket connection and the associated topics
+- `WEBSOCKET_CACHE_PREFIX`: prefix of keys used to cache data
+- `WEBSOCKET_CACHE_BACKEND`: the cache backend (`default` by default) — you cannot use LocMemCache with Celery or Channels workers, nor DummyCache with any kind of workers 
 - `WEBSOCKET_SIGNAL_ENCODER`: the JSON encoder to encode signal arguments 
 - `WEBSOCKET_SIGNAL_DECODER`: the JSON decoder to decode signal arguments
 - `WEBSOCKET_TOPIC_SERIALIZER`: the function used to transform Python topics into valid topic names  
 - `WEBSOCKET_POOL_SIZES`: a dict associating a queue name to a number of threads (or processes)
 - `WINDOW_INFO_MIDDLEWARES`: a list of middlewares for transforming a HttpRequest to a WindowInfo 
 - `WEBSOCKET_URL`: URL prefix (`/ws/` by default)
 - `ASGI_APPLICATION`: the ASGI application 
@@ -345,14 +351,16 @@
 ```
 
 JavaScript signals
 ------------------
 
 Many [JS signals](https://github.com/d9pouces/df_websockets/blob/master/npm/df_websockets/base.js) are available out-of-the-box.
 These signals can be triggered either by the JS code or by the Python code.
+
+Signals must be defined in a Python file that is imported during Django's startup, or in any `signals.py` file inside a Django app (like `models.py`). 
 For example, you can update the content of a HTML node with the following lines:
 
 ```python
 from df_websockets.tasks import trigger, WINDOW
 from df_websockets.decorators import signal
 
 @signal(path='test.signal', queue='demo-queue')
@@ -486,8 +494,7 @@
             "propagate": False,
         },
     },
     "root": {"handlers": ["stdout.info"], "level": "DEBUG"},
 }
 
 ```
-
```

### Comparing `df_websockets-1.0.0b1/README.md` & `df_websockets-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 Signals are exchanged between the browser window and the server using a single websocket.
 Signals that are triggered by the browser on the server are processed as background tasks (so the websocket endpoint does almost nothing).
 Signals that are triggered by the server can be processed as background tasks on the serveur and as Javascript functions on the browser.
 
 Background processes can use [celery](https://docs.celeryproject.org/en/stable/), [channels](https://pypi.org/project/channels/) workers, or simply different processes or threads.
 
 
-Requirements and installation
------------------------------
+Requirements
+------------
 
 `df_websockets` works with:
 
   * [Python](https://www.python.org) >= 3.6,
   * [django](https://pypi.org/project/Django/) >= 2.0,
   * [channels](https://pypi.org/project/channels/) >= 2.0.
 
@@ -30,14 +30,17 @@
 
   * [redis](https://redis.io) >= 5.0,
   * [channels_redis](https://pypi.org/project/channels-redis/) >= 3.3.
 
 If you want to process signals in Celery tasks rather in Channel workers, you need to setup a Celery infrastructure:
 [Celery setup](https://docs.celeryproject.org/en/stable/django/first-steps-with-django.html).
 
+Installation
+------------
+
 ```bash
 python -m pip install df_websockets
 ```
 
 In your settings, you must add the following values:
 ```python
 # the ASGI application to use with gunicorn or daphne
@@ -140,34 +143,37 @@
 When you trigger a signal on the server, you can target any set topic. All windows featuring this topic will receive this signal.
 
 _For example, assume that multiple clients open a specific article on a blog. At any time, you can open Python shell in a terminal and trigger a signal on all these windows._  
 
 
 ```python
 from df_websockets.tasks import set_websocket_topics
+from django.contrib.auth.models import Group
+from django.template.response import TemplateResponse
 
 def any_view(request):  # this is a standard Django view
     # useful code
-    obj1 = MyModel.objects.get(id=42)
+    obj1 = Group.objects.get(id=42)
     set_websocket_topics(request, [obj1])
     return TemplateResponse("my/template.html", {})  # do not forget to add `js/df_websockets.min.js` to this HTML
 ```
 
 `obj1` must be a Python object that is handled by the `WEBSOCKET_TOPIC_SERIALIZER` function. By default, any string and Django models are valid.
 Each window also has a unique identifier that is automatically added to this list, as well as the connected user id and the `BROADCAST`.
 
 The following code will call the JS function on every browser window having the `obj` topic and to the displayed window.
 ```python
 from df_websockets.tasks import WINDOW, trigger
 from df_websockets.tasks import set_websocket_topics
-
+from django.contrib.auth.models import Group
+from django.http.response import HttpResponse
 def another_view(request, obj_id):
-    obj = MyModel.objects.get(id=42)
+    obj = Group.objects.get(id=42)
     trigger(request, 'myproject.first_signal', to=[WINDOW, obj], content="hello from a view")
-    set_websocket_topics(request, [other_topics])
+    set_websocket_topics(request, ["other topics"])
     return HttpResponse()
 ```
 
 There are three special values:
 
 * `df_websockets.tasks.WINDOW`: the original browser window,
 * `df_websockets.tasks.USER`: all windows currently displayed by the connected user,
@@ -181,19 +187,20 @@
 settings
 --------
 
 There are a few settings:
 
 - `WEBSOCKET_WORKERS`: one of "celery" (use Celery tasks), "channels" (use Channels workers), "multithread" (process signals in threads), "multiprocess" (process signals in new processes).
   The first two choices require at least one valid worker. 
-- `CELERY_DEFAULT_QUEUE` the default queue for signals (`"celery"` by default)
+- `WEBSOCKET_DEFAULT_QUEUE` the default queue for signals (`"celery"` by default)
 
 Other settings are:
-- `WEBSOCKET_REDIS_EXPIRE`: the validity of the association between a websocket connection and the associated topics
-- `WEBSOCKET_REDIS_PREFIX`: prefix of keys used to cache data
+- `WEBSOCKET_CACHE_EXPIRE`: the validity of the association between a websocket connection and the associated topics
+- `WEBSOCKET_CACHE_PREFIX`: prefix of keys used to cache data
+- `WEBSOCKET_CACHE_BACKEND`: the cache backend (`default` by default) — you cannot use LocMemCache with Celery or Channels workers, nor DummyCache with any kind of workers 
 - `WEBSOCKET_SIGNAL_ENCODER`: the JSON encoder to encode signal arguments 
 - `WEBSOCKET_SIGNAL_DECODER`: the JSON decoder to decode signal arguments
 - `WEBSOCKET_TOPIC_SERIALIZER`: the function used to transform Python topics into valid topic names  
 - `WEBSOCKET_POOL_SIZES`: a dict associating a queue name to a number of threads (or processes)
 - `WINDOW_INFO_MIDDLEWARES`: a list of middlewares for transforming a HttpRequest to a WindowInfo 
 - `WEBSOCKET_URL`: URL prefix (`/ws/` by default)
 - `ASGI_APPLICATION`: the ASGI application 
@@ -313,14 +320,16 @@
 ```
 
 JavaScript signals
 ------------------
 
 Many [JS signals](https://github.com/d9pouces/df_websockets/blob/master/npm/df_websockets/base.js) are available out-of-the-box.
 These signals can be triggered either by the JS code or by the Python code.
+
+Signals must be defined in a Python file that is imported during Django's startup, or in any `signals.py` file inside a Django app (like `models.py`). 
 For example, you can update the content of a HTML node with the following lines:
 
 ```python
 from df_websockets.tasks import trigger, WINDOW
 from df_websockets.decorators import signal
 
 @signal(path='test.signal', queue='demo-queue')
```

### Comparing `df_websockets-1.0.0b1/demo_df_websockets/settings.py` & `df_websockets-1.0.1/demo_df_websockets/settings.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/demo_df_websockets/signals.py` & `df_websockets-1.0.1/demo_df_websockets/signals.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/demo_df_websockets/static/image.png` & `df_websockets-1.0.1/demo_df_websockets/static/image.png`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/demo_df_websockets/templates/index.html` & `df_websockets-1.0.1/demo_df_websockets/templates/index.html`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/demo_df_websockets/urls.py` & `df_websockets-1.0.1/demo_df_websockets/urls.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/__init__.py` & `df_websockets-1.0.1/df_websockets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #                                                                              #
 #  You should have received a copy of the CeCILL-B license with                #
 #  this file. If not, please visit:                                            #
 #  https://cecill.info/licences/Licence_CeCILL-B_V1-en.txt (English)           #
 #  or https://cecill.info/licences/Licence_CeCILL-B_V1-fr.txt (French)         #
 #                                                                              #
 # ##############################################################################
-__version__ = "1.0.0b1"
+__version__ = "1.0.1"
```

### Comparing `df_websockets-1.0.0b1/df_websockets/celery.py` & `df_websockets-1.0.1/df_websockets/celery.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/constants.py` & `df_websockets-1.0.1/df_websockets/constants.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/consumers.py` & `df_websockets-1.0.1/df_websockets/consumers.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from typing import Optional, Union
 
 from asgiref.compatibility import guarantee_single_callable
 from asgiref.sync import async_to_sync
 from channels.consumer import SyncConsumer
 from channels.generic.websocket import WebsocketConsumer
 from channels.routing import ChannelNameRouter
-from django.core import cache
+from django.core.cache import caches
 from django.core.exceptions import ImproperlyConfigured
 from django.core.handlers.base import BaseHandler
 from django.http import HttpRequest, HttpResponse, QueryDict
 from django.utils.module_loading import import_string
 
 from df_websockets import tasks, ws_settings
 from df_websockets.constants import WEBSOCKET_KEY_COOKIE_NAME
@@ -44,15 +44,16 @@
     if not hasattr(request, "window_key"):
         return []
     # noinspection PyUnresolvedReferences
     cache_key = "%s%s" % (
         ws_settings.WEBSOCKET_CACHE_PREFIX,
         request.window_key,
     )
-    topic_string = cache.cache.get(cache_key, "[]")
+    cache = caches[ws_settings.WEBSOCKET_CACHE_BACKEND]
+    topic_string = cache.get(cache_key, "[]")
     logger.debug("websocket %s is bound to topics %s", cache_key, topic_string)
     return [valid_topic_name(x) for x in json.loads(topic_string)]
 
 
 class WebsocketHandler(BaseHandler):
     def _get_response(self, request):
         return HttpResponse(status=200)
```

### Comparing `df_websockets-1.0.0b1/df_websockets/decorators.py` & `df_websockets-1.0.1/df_websockets/decorators.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/management/__init__.py` & `df_websockets-1.0.1/df_websockets/management/__init__.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/management/commands/__init__.py` & `df_websockets-1.0.1/df_websockets/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/management/commands/celery.py` & `df_websockets-1.0.1/df_websockets/management/commands/celery.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/management/commands/worker.py` & `df_websockets-1.0.1/df_websockets/management/commands/worker.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/middleware.py` & `df_websockets-1.0.1/df_websockets/middleware.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/routing.py` & `df_websockets-1.0.1/df_websockets/routing.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/static/js/df_websockets.min.js` & `df_websockets-1.0.1/df_websockets/static/js/df_websockets.min.js`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/static/js/df_websockets.min.js.map` & `df_websockets-1.0.1/df_websockets/static/js/df_websockets.min.js.map`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/tasks.py` & `df_websockets-1.0.1/df_websockets/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,24 +33,24 @@
 import uuid
 from functools import lru_cache
 from importlib import import_module
 from typing import Dict, List
 
 import django
 from asgiref.sync import async_to_sync
+from django.core.cache import caches
 
 try:
     from celery import shared_task as celery_shared_task
 except ImportError:
     celery_shared_task = None
 
 from channels import DEFAULT_CHANNEL_LAYER
 from channels.layers import get_channel_layer
 from django.apps import apps
-from django.core import cache
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.module_loading import import_string
 
 from df_websockets import ws_settings
 from df_websockets.constants import (
     WORKER_CELERY,
     WORKER_CHANNEL,
@@ -112,15 +112,16 @@
     if getattr(request, "user", None) and request.user.is_authenticated:
         topic_strings.add(_topic_serializer(request, USER))
     topic_strings.add(_topic_serializer(request, WINDOW))
     topic_strings.add(_topic_serializer(request, BROADCAST))
     topic_string = json.dumps(list(topic_strings))
     # noinspection PyUnresolvedReferences
     cache_key = "%s%s" % (ws_settings.WEBSOCKET_CACHE_PREFIX, request.window_key)
-    cache.cache.set(cache_key, topic_string, ws_settings.WEBSOCKET_CACHE_EXPIRE)
+    cache = caches[ws_settings.WEBSOCKET_CACHE_BACKEND]
+    cache.set(cache_key, topic_string, ws_settings.WEBSOCKET_CACHE_EXPIRE)
     logger.debug("websocket %s is now bound to topics %s", cache_key, topic_string)
 
 
 def trigger(window_info, signal_name, to=None, **kwargs):
     """Shortcut to :meth:`df_websockets.tasks.call`, allowing to directly pass arguments of the signal to this function.
     Your signal cannot use `window_info`, `signal_name` and `to` as argument names.
```

### Comparing `df_websockets-1.0.0b1/df_websockets/templatetags/__init__.py` & `df_websockets-1.0.1/df_websockets/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/templatetags/websockets.py` & `df_websockets-1.0.1/df_websockets/templatetags/websockets.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/testing.py` & `df_websockets-1.0.1/df_websockets/testing.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/topics.py` & `df_websockets-1.0.1/df_websockets/topics.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/utils.py` & `df_websockets-1.0.1/df_websockets/utils.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/window_info.py` & `df_websockets-1.0.1/df_websockets/window_info.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/ws_middleware.py` & `df_websockets-1.0.1/df_websockets/ws_middleware.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/df_websockets/ws_settings.py` & `df_websockets-1.0.1/df_websockets/ws_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,26 +42,32 @@
 )
 WEBSOCKET_CACHE_EXPIRE = compatibility_setting(
     "WEBSOCKET_CACHE_EXPIRE", "WEBSOCKET_REDIS_EXPIRE", 36000
 )
 WEBSOCKET_CACHE_PREFIX = compatibility_setting(
     "WEBSOCKET_CACHE_PREFIX", "WEBSOCKET_REDIS_PREFIX", "df_ws"
 )
+WEBSOCKET_CACHE_BACKEND = getattr(settings, "WEBSOCKET_CACHE_BACKEND", "default")
 WEBSOCKET_SIGNAL_DECODER = getattr(
     settings, "WEBSOCKET_SIGNAL_DECODER", "json.JSONDecoder"
 )
 WEBSOCKET_SIGNAL_ENCODER = getattr(
     settings,
     "WEBSOCKET_SIGNAL_ENCODER",
     "django.core.serializers.json.DjangoJSONEncoder",
 )
 WEBSOCKET_TOPIC_SERIALIZER = getattr(
     settings, "WEBSOCKET_TOPIC_SERIALIZER", "df_websockets.topics.serialize_topic"
 )
 WEBSOCKET_WORKERS = getattr(settings, "WEBSOCKET_WORKERS", constants.WORKER_CELERY)
+if WEBSOCKET_WORKERS == constants.WORKER_CELERY:
+    try:
+        import celery
+    except ImportError:
+        WEBSOCKET_WORKERS = constants.WORKER_THREAD
 # "celery", "channels", "multithread", "multiprocess"
 WEBSOCKET_POOL_SIZES = getattr(settings, "WEBSOCKET_POOL_SIZES", {None: 10})
 WINDOW_INFO_MIDDLEWARES = getattr(
     settings,
     "WINDOW_INFO_MIDDLEWARES",
     [
         "df_websockets.ws_middleware.WindowKeyMiddleware",
```

### Comparing `df_websockets-1.0.0b1/df_websockets.egg-info/PKG-INFO` & `df_websockets-1.0.1/df_websockets.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: df-websockets
-Version: 1.0.0b1
+Version: 1.0.1
 Summary: Websocket integration for Django
 Home-page: https://github.com/d9pouces/df_websockets
 Author: Matthieu Gallet
 Author-email: github@19pouces.net
 Maintainer: Matthieu Gallet
 Maintainer-email: github@19pouces.net
 License: CeCILL-B
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
@@ -44,16 +43,16 @@
 Signals are exchanged between the browser window and the server using a single websocket.
 Signals that are triggered by the browser on the server are processed as background tasks (so the websocket endpoint does almost nothing).
 Signals that are triggered by the server can be processed as background tasks on the serveur and as Javascript functions on the browser.
 
 Background processes can use [celery](https://docs.celeryproject.org/en/stable/), [channels](https://pypi.org/project/channels/) workers, or simply different processes or threads.
 
 
-Requirements and installation
------------------------------
+Requirements
+------------
 
 `df_websockets` works with:
 
   * [Python](https://www.python.org) >= 3.6,
   * [django](https://pypi.org/project/Django/) >= 2.0,
   * [channels](https://pypi.org/project/channels/) >= 2.0.
 
@@ -62,14 +61,17 @@
 
   * [redis](https://redis.io) >= 5.0,
   * [channels_redis](https://pypi.org/project/channels-redis/) >= 3.3.
 
 If you want to process signals in Celery tasks rather in Channel workers, you need to setup a Celery infrastructure:
 [Celery setup](https://docs.celeryproject.org/en/stable/django/first-steps-with-django.html).
 
+Installation
+------------
+
 ```bash
 python -m pip install df_websockets
 ```
 
 In your settings, you must add the following values:
 ```python
 # the ASGI application to use with gunicorn or daphne
@@ -172,34 +174,37 @@
 When you trigger a signal on the server, you can target any set topic. All windows featuring this topic will receive this signal.
 
 _For example, assume that multiple clients open a specific article on a blog. At any time, you can open Python shell in a terminal and trigger a signal on all these windows._  
 
 
 ```python
 from df_websockets.tasks import set_websocket_topics
+from django.contrib.auth.models import Group
+from django.template.response import TemplateResponse
 
 def any_view(request):  # this is a standard Django view
     # useful code
-    obj1 = MyModel.objects.get(id=42)
+    obj1 = Group.objects.get(id=42)
     set_websocket_topics(request, [obj1])
     return TemplateResponse("my/template.html", {})  # do not forget to add `js/df_websockets.min.js` to this HTML
 ```
 
 `obj1` must be a Python object that is handled by the `WEBSOCKET_TOPIC_SERIALIZER` function. By default, any string and Django models are valid.
 Each window also has a unique identifier that is automatically added to this list, as well as the connected user id and the `BROADCAST`.
 
 The following code will call the JS function on every browser window having the `obj` topic and to the displayed window.
 ```python
 from df_websockets.tasks import WINDOW, trigger
 from df_websockets.tasks import set_websocket_topics
-
+from django.contrib.auth.models import Group
+from django.http.response import HttpResponse
 def another_view(request, obj_id):
-    obj = MyModel.objects.get(id=42)
+    obj = Group.objects.get(id=42)
     trigger(request, 'myproject.first_signal', to=[WINDOW, obj], content="hello from a view")
-    set_websocket_topics(request, [other_topics])
+    set_websocket_topics(request, ["other topics"])
     return HttpResponse()
 ```
 
 There are three special values:
 
 * `df_websockets.tasks.WINDOW`: the original browser window,
 * `df_websockets.tasks.USER`: all windows currently displayed by the connected user,
@@ -213,19 +218,20 @@
 settings
 --------
 
 There are a few settings:
 
 - `WEBSOCKET_WORKERS`: one of "celery" (use Celery tasks), "channels" (use Channels workers), "multithread" (process signals in threads), "multiprocess" (process signals in new processes).
   The first two choices require at least one valid worker. 
-- `CELERY_DEFAULT_QUEUE` the default queue for signals (`"celery"` by default)
+- `WEBSOCKET_DEFAULT_QUEUE` the default queue for signals (`"celery"` by default)
 
 Other settings are:
-- `WEBSOCKET_REDIS_EXPIRE`: the validity of the association between a websocket connection and the associated topics
-- `WEBSOCKET_REDIS_PREFIX`: prefix of keys used to cache data
+- `WEBSOCKET_CACHE_EXPIRE`: the validity of the association between a websocket connection and the associated topics
+- `WEBSOCKET_CACHE_PREFIX`: prefix of keys used to cache data
+- `WEBSOCKET_CACHE_BACKEND`: the cache backend (`default` by default) — you cannot use LocMemCache with Celery or Channels workers, nor DummyCache with any kind of workers 
 - `WEBSOCKET_SIGNAL_ENCODER`: the JSON encoder to encode signal arguments 
 - `WEBSOCKET_SIGNAL_DECODER`: the JSON decoder to decode signal arguments
 - `WEBSOCKET_TOPIC_SERIALIZER`: the function used to transform Python topics into valid topic names  
 - `WEBSOCKET_POOL_SIZES`: a dict associating a queue name to a number of threads (or processes)
 - `WINDOW_INFO_MIDDLEWARES`: a list of middlewares for transforming a HttpRequest to a WindowInfo 
 - `WEBSOCKET_URL`: URL prefix (`/ws/` by default)
 - `ASGI_APPLICATION`: the ASGI application 
@@ -345,14 +351,16 @@
 ```
 
 JavaScript signals
 ------------------
 
 Many [JS signals](https://github.com/d9pouces/df_websockets/blob/master/npm/df_websockets/base.js) are available out-of-the-box.
 These signals can be triggered either by the JS code or by the Python code.
+
+Signals must be defined in a Python file that is imported during Django's startup, or in any `signals.py` file inside a Django app (like `models.py`). 
 For example, you can update the content of a HTML node with the following lines:
 
 ```python
 from df_websockets.tasks import trigger, WINDOW
 from df_websockets.decorators import signal
 
 @signal(path='test.signal', queue='demo-queue')
@@ -486,8 +494,7 @@
             "propagate": False,
         },
     },
     "root": {"handlers": ["stdout.info"], "level": "DEBUG"},
 }
 
 ```
-
```

### Comparing `df_websockets-1.0.0b1/df_websockets.egg-info/SOURCES.txt` & `df_websockets-1.0.1/df_websockets.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 demo_df_websockets/urls.py
 demo_df_websockets/views.py
 demo_df_websockets/static/demo.css
 demo_df_websockets/static/demo.js
 demo_df_websockets/static/image.png
 demo_df_websockets/templates/index.html
 df_websockets/__init__.py
+df_websockets/apps.py
 df_websockets/celery.py
+df_websockets/checks.py
 df_websockets/constants.py
 df_websockets/consumers.py
 df_websockets/decorators.py
 df_websockets/middleware.py
 df_websockets/routing.py
 df_websockets/tasks.py
 df_websockets/testing.py
```

### Comparing `df_websockets-1.0.0b1/npm/df_websockets/app.js` & `df_websockets-1.0.1/npm/df_websockets/app.js`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/npm/df_websockets/base.js` & `df_websockets-1.0.1/npm/df_websockets/base.js`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/npm/df_websockets/forms.ts` & `df_websockets-1.0.1/npm/df_websockets/forms.ts`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/npm/df_websockets/html.js` & `df_websockets-1.0.1/npm/df_websockets/html.js`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/npm/package-lock.json` & `df_websockets-1.0.1/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/npm/webpack.config.js` & `df_websockets-1.0.1/npm/webpack.config.js`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/pre-commit.sh` & `df_websockets-1.0.1/pre-commit.sh`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/setup.cfg` & `df_websockets-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/setup.py` & `df_websockets-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/test_df_websockets/test_consumers.py` & `df_websockets-1.0.1/test_df_websockets/test_consumers.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/test_df_websockets/test_decorators.py` & `df_websockets-1.0.1/test_df_websockets/test_decorators.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/test_df_websockets/test_middleware.py` & `df_websockets-1.0.1/test_df_websockets/test_middleware.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/test_df_websockets/test_testing.py` & `df_websockets-1.0.1/test_df_websockets/test_testing.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.0b1/test_df_websockets/test_window_info.py` & `df_websockets-1.0.1/test_df_websockets/test_window_info.py`

 * *Files identical despite different names*

