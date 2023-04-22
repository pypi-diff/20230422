# Comparing `tmp/df_websockets-1.0.2.tar.gz` & `tmp/df_websockets-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "df_websockets-1.0.2.tar", last modified: Sat Apr 22 15:09:48 2023, max compression
+gzip compressed data, was "df_websockets-1.0.3.tar", last modified: Sat Apr 22 16:50:05 2023, max compression
```

## Comparing `df_websockets-1.0.2.tar` & `df_websockets-1.0.3.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 15:09:48.375904 df_websockets-1.0.2/
--rw-r--r--   0 flanker    (501) staff       (20)     3094 2023-04-22 13:39:52.000000 df_websockets-1.0.2/.gitignore
--rw-r--r--   0 flanker    (501) staff       (20)      478 2021-03-25 18:53:48.000000 df_websockets-1.0.2/.travis.yml
--rw-r--r--   0 flanker    (501) staff       (20)    21393 2020-11-04 09:00:51.000000 df_websockets-1.0.2/LICENSE
--rw-r--r--   0 flanker    (501) staff       (20)      105 2020-11-04 09:00:51.000000 df_websockets-1.0.2/MANIFEST.in
--rw-r--r--   0 flanker    (501) staff       (20)    19654 2023-04-22 15:09:48.376362 df_websockets-1.0.2/PKG-INFO
--rw-r--r--   0 flanker    (501) staff       (20)    18404 2023-04-22 13:38:39.000000 df_websockets-1.0.2/README.md
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 15:09:48.303044 df_websockets-1.0.2/demo_df_websockets/
--rw-r--r--   0 flanker    (501) staff       (20)        0 2023-01-28 22:42:08.000000 df_websockets-1.0.2/demo_df_websockets/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     5682 2023-01-28 22:42:08.000000 df_websockets-1.0.2/demo_df_websockets/settings.py
--rw-r--r--   0 flanker    (501) staff       (20)     5475 2023-01-28 22:42:08.000000 df_websockets-1.0.2/demo_df_websockets/signals.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 15:09:48.304973 df_websockets-1.0.2/demo_df_websockets/static/
--rw-r--r--   0 flanker    (501) staff       (20)      224 2023-01-28 22:42:08.000000 df_websockets-1.0.2/demo_df_websockets/static/demo.css
--rw-r--r--   0 flanker    (501) staff       (20)      329 2023-01-28 22:42:08.000000 df_websockets-1.0.2/demo_df_websockets/static/demo.js
--rw-r--r--   0 flanker    (501) staff       (20)    15390 2021-03-22 07:04:44.000000 df_websockets-1.0.2/demo_df_websockets/static/image.png
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 15:09:48.305864 df_websockets-1.0.2/demo_df_websockets/templates/
--rw-r--r--   0 flanker    (501) staff       (20)    29153 2022-08-29 19:52:16.000000 df_websockets-1.0.2/demo_df_websockets/templates/index.html
--rw-r--r--   0 flanker    (501) staff       (20)      769 2023-01-28 22:42:08.000000 df_websockets-1.0.2/demo_df_websockets/urls.py
--rw-r--r--   0 flanker    (501) staff       (20)      215 2023-01-28 22:42:08.000000 df_websockets-1.0.2/demo_df_websockets/views.py
--rwxr-xr-x   0 flanker    (501) staff       (20)      334 2023-01-28 22:42:08.000000 df_websockets-1.0.2/demo_manage.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 15:09:48.315822 df_websockets-1.0.2/df_websockets/
--rw-r--r--   0 flanker    (501) staff       (20)     1237 2023-04-22 15:09:11.000000 df_websockets-1.0.2/df_websockets/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)      301 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/apps.py
--rw-r--r--   0 flanker    (501) staff       (20)     2900 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/celery.py
--rw-r--r--   0 flanker    (501) staff       (20)     1414 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/checks.py
--rw-r--r--   0 flanker    (501) staff       (20)     1471 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/constants.py
--rw-r--r--   0 flanker    (501) staff       (20)     8285 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/consumers.py
--rw-r--r--   0 flanker    (501) staff       (20)    13765 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/decorators.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 15:09:48.339676 df_websockets-1.0.2/df_websockets/management/
--rw-r--r--   0 flanker    (501) staff       (20)     1215 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/management/__init__.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 15:09:48.343044 df_websockets-1.0.2/df_websockets/management/commands/
--rw-r--r--   0 flanker    (501) staff       (20)     1215 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/management/commands/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     1685 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/management/commands/celery.py
--rw-r--r--   0 flanker    (501) staff       (20)     3489 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/management/commands/worker.py
--rw-r--r--   0 flanker    (501) staff       (20)     3829 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/middleware.py
--rw-r--r--   0 flanker    (501) staff       (20)     1989 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/routing.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 15:09:48.293547 df_websockets-1.0.2/df_websockets/static/
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 15:09:48.344817 df_websockets-1.0.2/df_websockets/static/js/
--rw-r--r--   0 flanker    (501) staff       (20)     7866 2022-08-29 19:52:16.000000 df_websockets-1.0.2/df_websockets/static/js/df_websockets.min.js
--rw-r--r--   0 flanker    (501) staff       (20)    44971 2022-08-29 19:52:16.000000 df_websockets-1.0.2/df_websockets/static/js/df_websockets.min.js.map
--rw-r--r--   0 flanker    (501) staff       (20)    16911 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/tasks.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 15:09:48.347782 df_websockets-1.0.2/df_websockets/templatetags/
--rw-r--r--   0 flanker    (501) staff       (20)     1215 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/templatetags/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     2579 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/templatetags/websockets.py
--rw-r--r--   0 flanker    (501) staff       (20)     5424 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/testing.py
--rw-r--r--   0 flanker    (501) staff       (20)     3039 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/topics.py
--rw-r--r--   0 flanker    (501) staff       (20)     6143 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/utils.py
--rw-r--r--   0 flanker    (501) staff       (20)     5736 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/window_info.py
--rw-r--r--   0 flanker    (501) staff       (20)    11754 2023-01-28 22:42:08.000000 df_websockets-1.0.2/df_websockets/ws_middleware.py
--rw-r--r--   0 flanker    (501) staff       (20)     3554 2023-04-22 13:58:56.000000 df_websockets-1.0.2/df_websockets/ws_settings.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 15:09:48.338981 df_websockets-1.0.2/df_websockets.egg-info/
--rw-r--r--   0 flanker    (501) staff       (20)    19654 2023-04-22 15:09:48.000000 df_websockets-1.0.2/df_websockets.egg-info/PKG-INFO
--rw-r--r--   0 flanker    (501) staff       (20)     1806 2023-04-22 15:09:48.000000 df_websockets-1.0.2/df_websockets.egg-info/SOURCES.txt
--rw-r--r--   0 flanker    (501) staff       (20)        1 2023-04-22 15:09:48.000000 df_websockets-1.0.2/df_websockets.egg-info/dependency_links.txt
--rw-r--r--   0 flanker    (501) staff       (20)        1 2020-11-21 14:07:31.000000 df_websockets-1.0.2/df_websockets.egg-info/not-zip-safe
--rw-r--r--   0 flanker    (501) staff       (20)       45 2023-04-22 15:09:48.000000 df_websockets-1.0.2/df_websockets.egg-info/requires.txt
--rw-r--r--   0 flanker    (501) staff       (20)       52 2023-04-22 15:09:48.000000 df_websockets-1.0.2/df_websockets.egg-info/top_level.txt
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 15:09:48.355486 df_websockets-1.0.2/npm/
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 15:09:48.368100 df_websockets-1.0.2/npm/df_websockets/
--rw-r--r--   0 flanker    (501) staff       (20)     5253 2023-01-28 22:42:08.000000 df_websockets-1.0.2/npm/df_websockets/app.js
--rw-r--r--   0 flanker    (501) staff       (20)    13295 2023-01-28 22:42:08.000000 df_websockets-1.0.2/npm/df_websockets/base.js
--rw-r--r--   0 flanker    (501) staff       (20)    10672 2023-01-28 22:42:08.000000 df_websockets-1.0.2/npm/df_websockets/forms.ts
--rw-r--r--   0 flanker    (501) staff       (20)     4494 2023-01-28 22:42:08.000000 df_websockets-1.0.2/npm/df_websockets/html.js
--rw-r--r--   0 flanker    (501) staff       (20)   112499 2022-08-29 19:52:16.000000 df_websockets-1.0.2/npm/package-lock.json
--rw-r--r--   0 flanker    (501) staff       (20)      475 2021-03-25 21:22:08.000000 df_websockets-1.0.2/npm/package.json
--rw-r--r--   0 flanker    (501) staff       (20)      256 2021-03-23 20:46:59.000000 df_websockets-1.0.2/npm/tsconfig.json
--rw-r--r--   0 flanker    (501) staff       (20)     1963 2023-01-28 22:42:08.000000 df_websockets-1.0.2/npm/webpack.config.js
--rwxr-xr-x   0 flanker    (501) staff       (20)     1250 2023-01-28 22:42:08.000000 df_websockets-1.0.2/pre-commit.sh
--rw-r--r--   0 flanker    (501) staff       (20)     2700 2023-04-22 15:09:48.378382 df_websockets-1.0.2/setup.cfg
--rw-r--r--   0 flanker    (501) staff       (20)     1254 2023-01-28 22:42:08.000000 df_websockets-1.0.2/setup.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 15:09:48.374703 df_websockets-1.0.2/test_df_websockets/
--rw-r--r--   0 flanker    (501) staff       (20)        0 2023-01-28 22:42:08.000000 df_websockets-1.0.2/test_df_websockets/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     5824 2023-01-28 22:42:08.000000 df_websockets-1.0.2/test_df_websockets/test_consumers.py
--rw-r--r--   0 flanker    (501) staff       (20)     1339 2023-01-28 22:42:08.000000 df_websockets-1.0.2/test_df_websockets/test_decorators.py
--rw-r--r--   0 flanker    (501) staff       (20)     3350 2023-01-28 22:42:08.000000 df_websockets-1.0.2/test_df_websockets/test_middleware.py
--rw-r--r--   0 flanker    (501) staff       (20)     1834 2023-01-28 22:42:08.000000 df_websockets-1.0.2/test_df_websockets/test_testing.py
--rw-r--r--   0 flanker    (501) staff       (20)      414 2023-01-28 22:42:08.000000 df_websockets-1.0.2/test_df_websockets/test_utils.py
--rw-r--r--   0 flanker    (501) staff       (20)      998 2023-01-28 22:42:08.000000 df_websockets-1.0.2/test_df_websockets/test_window_info.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.638219 df_websockets-1.0.3/
+-rw-r--r--   0 flanker    (501) staff       (20)     3094 2023-04-22 16:43:51.000000 df_websockets-1.0.3/.gitignore
+-rw-r--r--   0 flanker    (501) staff       (20)      478 2021-03-25 18:53:48.000000 df_websockets-1.0.3/.travis.yml
+-rw-r--r--   0 flanker    (501) staff       (20)    21393 2020-11-04 09:00:51.000000 df_websockets-1.0.3/LICENSE
+-rw-r--r--   0 flanker    (501) staff       (20)      105 2020-11-04 09:00:51.000000 df_websockets-1.0.3/MANIFEST.in
+-rw-r--r--   0 flanker    (501) staff       (20)    19848 2023-04-22 16:50:05.638555 df_websockets-1.0.3/PKG-INFO
+-rw-r--r--   0 flanker    (501) staff       (20)    18598 2023-04-22 16:43:51.000000 df_websockets-1.0.3/README.md
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.577858 df_websockets-1.0.3/demo_df_websockets/
+-rw-r--r--   0 flanker    (501) staff       (20)        0 2023-01-28 22:42:08.000000 df_websockets-1.0.3/demo_df_websockets/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5682 2023-04-22 16:43:51.000000 df_websockets-1.0.3/demo_df_websockets/settings.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5475 2023-04-22 16:43:51.000000 df_websockets-1.0.3/demo_df_websockets/signals.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.579933 df_websockets-1.0.3/demo_df_websockets/static/
+-rw-r--r--   0 flanker    (501) staff       (20)      224 2023-01-28 22:42:08.000000 df_websockets-1.0.3/demo_df_websockets/static/demo.css
+-rw-r--r--   0 flanker    (501) staff       (20)      329 2023-01-28 22:42:08.000000 df_websockets-1.0.3/demo_df_websockets/static/demo.js
+-rw-r--r--   0 flanker    (501) staff       (20)    15390 2021-03-22 07:04:44.000000 df_websockets-1.0.3/demo_df_websockets/static/image.png
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.580826 df_websockets-1.0.3/demo_df_websockets/templates/
+-rw-r--r--   0 flanker    (501) staff       (20)    29153 2023-04-22 16:43:51.000000 df_websockets-1.0.3/demo_df_websockets/templates/index.html
+-rw-r--r--   0 flanker    (501) staff       (20)      769 2023-01-28 22:42:08.000000 df_websockets-1.0.3/demo_df_websockets/urls.py
+-rw-r--r--   0 flanker    (501) staff       (20)      215 2023-01-28 22:42:08.000000 df_websockets-1.0.3/demo_df_websockets/views.py
+-rwxr-xr-x   0 flanker    (501) staff       (20)      334 2023-01-28 22:42:08.000000 df_websockets-1.0.3/demo_manage.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.610794 df_websockets-1.0.3/df_websockets/
+-rw-r--r--   0 flanker    (501) staff       (20)     1237 2023-04-22 16:49:52.000000 df_websockets-1.0.3/df_websockets/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)      301 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/apps.py
+-rw-r--r--   0 flanker    (501) staff       (20)     2900 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/celery.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1414 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/checks.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1471 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/constants.py
+-rw-r--r--   0 flanker    (501) staff       (20)     8285 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/consumers.py
+-rw-r--r--   0 flanker    (501) staff       (20)    13765 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/decorators.py
+-rw-r--r--   0 flanker    (501) staff       (20)      217 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/load.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.616988 df_websockets-1.0.3/df_websockets/management/
+-rw-r--r--   0 flanker    (501) staff       (20)     1215 2023-01-28 22:42:08.000000 df_websockets-1.0.3/df_websockets/management/__init__.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.619643 df_websockets-1.0.3/df_websockets/management/commands/
+-rw-r--r--   0 flanker    (501) staff       (20)     1215 2023-01-28 22:42:08.000000 df_websockets-1.0.3/df_websockets/management/commands/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1685 2023-01-28 22:42:08.000000 df_websockets-1.0.3/df_websockets/management/commands/celery.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3489 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/management/commands/worker.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3829 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/middleware.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1989 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/routing.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.566543 df_websockets-1.0.3/df_websockets/static/
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.621103 df_websockets-1.0.3/df_websockets/static/js/
+-rw-r--r--   0 flanker    (501) staff       (20)     7866 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/static/js/df_websockets.min.js
+-rw-r--r--   0 flanker    (501) staff       (20)    44971 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/static/js/df_websockets.min.js.map
+-rw-r--r--   0 flanker    (501) staff       (20)    16911 2023-04-22 16:47:25.000000 df_websockets-1.0.3/df_websockets/tasks.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.623127 df_websockets-1.0.3/df_websockets/templatetags/
+-rw-r--r--   0 flanker    (501) staff       (20)     1215 2023-01-28 22:42:08.000000 df_websockets-1.0.3/df_websockets/templatetags/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     2579 2023-01-28 22:42:08.000000 df_websockets-1.0.3/df_websockets/templatetags/websockets.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5424 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/testing.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3039 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/topics.py
+-rw-r--r--   0 flanker    (501) staff       (20)     6143 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/utils.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5736 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/window_info.py
+-rw-r--r--   0 flanker    (501) staff       (20)    11796 2023-04-22 16:48:31.000000 df_websockets-1.0.3/df_websockets/ws_middleware.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3547 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/ws_settings.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.616209 df_websockets-1.0.3/df_websockets.egg-info/
+-rw-r--r--   0 flanker    (501) staff       (20)    19848 2023-04-22 16:50:05.000000 df_websockets-1.0.3/df_websockets.egg-info/PKG-INFO
+-rw-r--r--   0 flanker    (501) staff       (20)     1828 2023-04-22 16:50:05.000000 df_websockets-1.0.3/df_websockets.egg-info/SOURCES.txt
+-rw-r--r--   0 flanker    (501) staff       (20)        1 2023-04-22 16:50:05.000000 df_websockets-1.0.3/df_websockets.egg-info/dependency_links.txt
+-rw-r--r--   0 flanker    (501) staff       (20)        1 2020-11-21 14:07:31.000000 df_websockets-1.0.3/df_websockets.egg-info/not-zip-safe
+-rw-r--r--   0 flanker    (501) staff       (20)       45 2023-04-22 16:50:05.000000 df_websockets-1.0.3/df_websockets.egg-info/requires.txt
+-rw-r--r--   0 flanker    (501) staff       (20)       52 2023-04-22 16:50:05.000000 df_websockets-1.0.3/df_websockets.egg-info/top_level.txt
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.628277 df_websockets-1.0.3/npm/
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.631419 df_websockets-1.0.3/npm/df_websockets/
+-rw-r--r--   0 flanker    (501) staff       (20)     5253 2023-01-28 22:42:08.000000 df_websockets-1.0.3/npm/df_websockets/app.js
+-rw-r--r--   0 flanker    (501) staff       (20)    13295 2023-01-28 22:42:08.000000 df_websockets-1.0.3/npm/df_websockets/base.js
+-rw-r--r--   0 flanker    (501) staff       (20)    10672 2023-01-28 22:42:08.000000 df_websockets-1.0.3/npm/df_websockets/forms.ts
+-rw-r--r--   0 flanker    (501) staff       (20)     4494 2023-01-28 22:42:08.000000 df_websockets-1.0.3/npm/df_websockets/html.js
+-rw-r--r--   0 flanker    (501) staff       (20)   112499 2023-04-22 16:45:55.000000 df_websockets-1.0.3/npm/package-lock.json
+-rw-r--r--   0 flanker    (501) staff       (20)      475 2021-03-25 21:22:08.000000 df_websockets-1.0.3/npm/package.json
+-rw-r--r--   0 flanker    (501) staff       (20)      256 2021-03-23 20:46:59.000000 df_websockets-1.0.3/npm/tsconfig.json
+-rw-r--r--   0 flanker    (501) staff       (20)     1963 2023-01-28 22:42:08.000000 df_websockets-1.0.3/npm/webpack.config.js
+-rwxr-xr-x   0 flanker    (501) staff       (20)     1250 2023-01-28 22:42:08.000000 df_websockets-1.0.3/pre-commit.sh
+-rw-r--r--   0 flanker    (501) staff       (20)     2700 2023-04-22 16:50:05.640344 df_websockets-1.0.3/setup.cfg
+-rw-r--r--   0 flanker    (501) staff       (20)     1254 2023-01-28 22:42:08.000000 df_websockets-1.0.3/setup.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.637521 df_websockets-1.0.3/test_df_websockets/
+-rw-r--r--   0 flanker    (501) staff       (20)        0 2023-01-28 22:42:08.000000 df_websockets-1.0.3/test_df_websockets/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5824 2023-04-22 16:43:51.000000 df_websockets-1.0.3/test_df_websockets/test_consumers.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1339 2023-04-22 16:43:51.000000 df_websockets-1.0.3/test_df_websockets/test_decorators.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3350 2023-04-22 16:43:51.000000 df_websockets-1.0.3/test_df_websockets/test_middleware.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1834 2023-04-22 16:43:51.000000 df_websockets-1.0.3/test_df_websockets/test_testing.py
+-rw-r--r--   0 flanker    (501) staff       (20)      414 2023-04-22 16:43:51.000000 df_websockets-1.0.3/test_df_websockets/test_utils.py
+-rw-r--r--   0 flanker    (501) staff       (20)      998 2023-04-22 16:43:51.000000 df_websockets-1.0.3/test_df_websockets/test_window_info.py
```

### Comparing `df_websockets-1.0.2/.gitignore` & `df_websockets-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/LICENSE` & `df_websockets-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/PKG-INFO` & `df_websockets-1.0.3/df_websockets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: df_websockets
-Version: 1.0.2
+Name: df-websockets
+Version: 1.0.3
 Summary: Websocket integration for Django
 Home-page: https://github.com/d9pouces/df_websockets
 Author: Matthieu Gallet
 Author-email: github@19pouces.net
 Maintainer: Matthieu Gallet
 Maintainer-email: github@19pouces.net
 License: CeCILL-B
@@ -50,21 +50,23 @@
 Requirements
 ------------
 
 `df_websockets` works with:
 
   * [Python](https://www.python.org) >= 3.6,
   * [django](https://pypi.org/project/Django/) >= 2.0,
-  * [channels](https://pypi.org/project/channels/) >= 2.0.
+  * [channels](https://pypi.org/project/channels/) >= 2.0,
+  * [daphne](https://pypi.python.org/pypi/daphne) >= 2.0.
 
 
 For production use or any multiprocess setup (even in development mode), you also need:
 
   * [redis](https://redis.io) >= 5.0,
-  * [channels_redis](https://pypi.org/project/channels-redis/) >= 3.3.
+  * [channels_redis](https://pypi.org/project/channels-redis/) >= 3.3,
+  * [daphne](https://pypi.python.org/pypi/daphne) >= 2.0.
 
 If you want to process signals in Celery tasks rather in Channel workers, you need to setup a Celery infrastructure:
 [Celery setup](https://docs.celeryproject.org/en/stable/django/first-steps-with-django.html).
 
 Installation
 ------------
 
@@ -74,15 +76,15 @@
 
 In your settings, you must add the following values:
 ```python
 # the ASGI application to use with gunicorn or daphne
 ASGI_APPLICATION = "df_websockets.routing.application"
 # add the required Middleware
 MIDDLEWARES = [..., "df_websockets.middleware.WebsocketMiddleware", ...]
-INSTALLED_APPS = [..., "channels", "df_websockets", ...]
+INSTALLED_APPS = [..., "channels", "daphne", "df_websockets", ...]
 WEBSOCKET_WORKERS = "thread"
 # a channel layer, required by channels_redis
 CHANNEL_LAYERS = {
     'default': {
         'BACKEND': 'channels_redis.core.RedisChannelLayer',
         'CONFIG': {
             "hosts": [('localhost', 6379)],
@@ -97,14 +99,15 @@
 A bidirectionnal websocket connection will be established in your page.
 
 You can start the development server:
 ```bash
 python manage.py runserver
 ```
 
+_`daphne` must be present in `INSTALLED_APPS` with `channels>=4.0`_
 
 If you use Channels workers (WEBSOCKET_WORKERS = "channels"), you also need to start a Channel worker:
 ```bash
 python manage.py run_worker celery
 ```
 If you use Celery (WEBSOCKET_WORKERS = "celery"), you also need to start a Celery worker:
 ```bash
```

### Comparing `df_websockets-1.0.2/README.md` & `df_websockets-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,23 @@
 Requirements
 ------------
 
 `df_websockets` works with:
 
   * [Python](https://www.python.org) >= 3.6,
   * [django](https://pypi.org/project/Django/) >= 2.0,
-  * [channels](https://pypi.org/project/channels/) >= 2.0.
+  * [channels](https://pypi.org/project/channels/) >= 2.0,
+  * [daphne](https://pypi.python.org/pypi/daphne) >= 2.0.
 
 
 For production use or any multiprocess setup (even in development mode), you also need:
 
   * [redis](https://redis.io) >= 5.0,
-  * [channels_redis](https://pypi.org/project/channels-redis/) >= 3.3.
+  * [channels_redis](https://pypi.org/project/channels-redis/) >= 3.3,
+  * [daphne](https://pypi.python.org/pypi/daphne) >= 2.0.
 
 If you want to process signals in Celery tasks rather in Channel workers, you need to setup a Celery infrastructure:
 [Celery setup](https://docs.celeryproject.org/en/stable/django/first-steps-with-django.html).
 
 Installation
 ------------
 
@@ -43,15 +45,15 @@
 
 In your settings, you must add the following values:
 ```python
 # the ASGI application to use with gunicorn or daphne
 ASGI_APPLICATION = "df_websockets.routing.application"
 # add the required Middleware
 MIDDLEWARES = [..., "df_websockets.middleware.WebsocketMiddleware", ...]
-INSTALLED_APPS = [..., "channels", "df_websockets", ...]
+INSTALLED_APPS = [..., "channels", "daphne", "df_websockets", ...]
 WEBSOCKET_WORKERS = "thread"
 # a channel layer, required by channels_redis
 CHANNEL_LAYERS = {
     'default': {
         'BACKEND': 'channels_redis.core.RedisChannelLayer',
         'CONFIG': {
             "hosts": [('localhost', 6379)],
@@ -66,14 +68,15 @@
 A bidirectionnal websocket connection will be established in your page.
 
 You can start the development server:
 ```bash
 python manage.py runserver
 ```
 
+_`daphne` must be present in `INSTALLED_APPS` with `channels>=4.0`_
 
 If you use Channels workers (WEBSOCKET_WORKERS = "channels"), you also need to start a Channel worker:
 ```bash
 python manage.py run_worker celery
 ```
 If you use Celery (WEBSOCKET_WORKERS = "celery"), you also need to start a Celery worker:
 ```bash
```

### Comparing `df_websockets-1.0.2/demo_df_websockets/settings.py` & `df_websockets-1.0.3/demo_df_websockets/settings.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/demo_df_websockets/signals.py` & `df_websockets-1.0.3/demo_df_websockets/signals.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/demo_df_websockets/static/image.png` & `df_websockets-1.0.3/demo_df_websockets/static/image.png`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/demo_df_websockets/templates/index.html` & `df_websockets-1.0.3/demo_df_websockets/templates/index.html`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/demo_df_websockets/urls.py` & `df_websockets-1.0.3/demo_df_websockets/urls.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/__init__.py` & `df_websockets-1.0.3/df_websockets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #                                                                              #
 #  You should have received a copy of the CeCILL-B license with                #
 #  this file. If not, please visit:                                            #
 #  https://cecill.info/licences/Licence_CeCILL-B_V1-en.txt (English)           #
 #  or https://cecill.info/licences/Licence_CeCILL-B_V1-fr.txt (French)         #
 #                                                                              #
 # ##############################################################################
-__version__ = "1.0.2"
+__version__ = "1.0.3"
```

### Comparing `df_websockets-1.0.2/df_websockets/celery.py` & `df_websockets-1.0.3/df_websockets/celery.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/checks.py` & `df_websockets-1.0.3/df_websockets/checks.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/constants.py` & `df_websockets-1.0.3/df_websockets/constants.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/consumers.py` & `df_websockets-1.0.3/df_websockets/consumers.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/decorators.py` & `df_websockets-1.0.3/df_websockets/decorators.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/management/__init__.py` & `df_websockets-1.0.3/df_websockets/management/__init__.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/management/commands/__init__.py` & `df_websockets-1.0.3/df_websockets/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/management/commands/celery.py` & `df_websockets-1.0.3/df_websockets/management/commands/celery.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/management/commands/worker.py` & `df_websockets-1.0.3/df_websockets/management/commands/worker.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/middleware.py` & `df_websockets-1.0.3/df_websockets/middleware.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/routing.py` & `df_websockets-1.0.3/df_websockets/routing.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/static/js/df_websockets.min.js` & `df_websockets-1.0.3/df_websockets/static/js/df_websockets.min.js`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/static/js/df_websockets.min.js.map` & `df_websockets-1.0.3/df_websockets/static/js/df_websockets.min.js.map`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/tasks.py` & `df_websockets-1.0.3/df_websockets/tasks.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/templatetags/__init__.py` & `df_websockets-1.0.3/df_websockets/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/templatetags/websockets.py` & `df_websockets-1.0.3/df_websockets/templatetags/websockets.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/testing.py` & `df_websockets-1.0.3/df_websockets/testing.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/topics.py` & `df_websockets-1.0.3/df_websockets/topics.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/utils.py` & `df_websockets-1.0.3/df_websockets/utils.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/window_info.py` & `df_websockets-1.0.3/df_websockets/window_info.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/df_websockets/ws_middleware.py` & `df_websockets-1.0.3/df_websockets/ws_middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,8 +291,9 @@
         return {
             "LANGUAGES": settings.LANGUAGES,
             "LANGUAGE_CODE": window_info.language_code,
             "LANGUAGE_BIDI": translation.get_language_bidi(),
         }
 
     def before_process(self, window_info):
-        activate(window_info.language_code)
+        if window_info.language_code:
+            activate(window_info.language_code)
```

### Comparing `df_websockets-1.0.2/df_websockets/ws_settings.py` & `df_websockets-1.0.3/df_websockets/ws_settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 from df_websockets.constants import RemovedInDfWebsockets2Warning
 
 CELERY_APP = getattr(settings, "CELERY_APP", "df_websockets")
 
 
 def compatibility_setting(new_name, old_name, default):
     if hasattr(settings, new_name):
-        return settings.WEBSOCKET_DEFAULT_QUEUE
+        return getattr(settings, new_name)
     elif hasattr(settings, old_name):
         warnings.warn(
             f"{old_name} settings is replaced by {new_name}.",
             category=RemovedInDfWebsockets2Warning,
             stacklevel=2,
         )
-        return settings.CELERY_DEFAULT_QUEUE
+        return getattr(settings, old_name)
     else:
         return default
 
 
 WEBSOCKET_DEFAULT_QUEUE = compatibility_setting(
     "WEBSOCKET_DEFAULT_QUEUE", "CELERY_DEFAULT_QUEUE", "celery"
 )
```

### Comparing `df_websockets-1.0.2/df_websockets.egg-info/PKG-INFO` & `df_websockets-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: df-websockets
-Version: 1.0.2
+Name: df_websockets
+Version: 1.0.3
 Summary: Websocket integration for Django
 Home-page: https://github.com/d9pouces/df_websockets
 Author: Matthieu Gallet
 Author-email: github@19pouces.net
 Maintainer: Matthieu Gallet
 Maintainer-email: github@19pouces.net
 License: CeCILL-B
@@ -50,21 +50,23 @@
 Requirements
 ------------
 
 `df_websockets` works with:
 
   * [Python](https://www.python.org) >= 3.6,
   * [django](https://pypi.org/project/Django/) >= 2.0,
-  * [channels](https://pypi.org/project/channels/) >= 2.0.
+  * [channels](https://pypi.org/project/channels/) >= 2.0,
+  * [daphne](https://pypi.python.org/pypi/daphne) >= 2.0.
 
 
 For production use or any multiprocess setup (even in development mode), you also need:
 
   * [redis](https://redis.io) >= 5.0,
-  * [channels_redis](https://pypi.org/project/channels-redis/) >= 3.3.
+  * [channels_redis](https://pypi.org/project/channels-redis/) >= 3.3,
+  * [daphne](https://pypi.python.org/pypi/daphne) >= 2.0.
 
 If you want to process signals in Celery tasks rather in Channel workers, you need to setup a Celery infrastructure:
 [Celery setup](https://docs.celeryproject.org/en/stable/django/first-steps-with-django.html).
 
 Installation
 ------------
 
@@ -74,15 +76,15 @@
 
 In your settings, you must add the following values:
 ```python
 # the ASGI application to use with gunicorn or daphne
 ASGI_APPLICATION = "df_websockets.routing.application"
 # add the required Middleware
 MIDDLEWARES = [..., "df_websockets.middleware.WebsocketMiddleware", ...]
-INSTALLED_APPS = [..., "channels", "df_websockets", ...]
+INSTALLED_APPS = [..., "channels", "daphne", "df_websockets", ...]
 WEBSOCKET_WORKERS = "thread"
 # a channel layer, required by channels_redis
 CHANNEL_LAYERS = {
     'default': {
         'BACKEND': 'channels_redis.core.RedisChannelLayer',
         'CONFIG': {
             "hosts": [('localhost', 6379)],
@@ -97,14 +99,15 @@
 A bidirectionnal websocket connection will be established in your page.
 
 You can start the development server:
 ```bash
 python manage.py runserver
 ```
 
+_`daphne` must be present in `INSTALLED_APPS` with `channels>=4.0`_
 
 If you use Channels workers (WEBSOCKET_WORKERS = "channels"), you also need to start a Channel worker:
 ```bash
 python manage.py run_worker celery
 ```
 If you use Celery (WEBSOCKET_WORKERS = "celery"), you also need to start a Celery worker:
 ```bash
```

### Comparing `df_websockets-1.0.2/df_websockets.egg-info/SOURCES.txt` & `df_websockets-1.0.3/df_websockets.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 df_websockets/__init__.py
 df_websockets/apps.py
 df_websockets/celery.py
 df_websockets/checks.py
 df_websockets/constants.py
 df_websockets/consumers.py
 df_websockets/decorators.py
+df_websockets/load.py
 df_websockets/middleware.py
 df_websockets/routing.py
 df_websockets/tasks.py
 df_websockets/testing.py
 df_websockets/topics.py
 df_websockets/utils.py
 df_websockets/window_info.py
```

### Comparing `df_websockets-1.0.2/npm/df_websockets/app.js` & `df_websockets-1.0.3/npm/df_websockets/app.js`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/npm/df_websockets/base.js` & `df_websockets-1.0.3/npm/df_websockets/base.js`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/npm/df_websockets/forms.ts` & `df_websockets-1.0.3/npm/df_websockets/forms.ts`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/npm/df_websockets/html.js` & `df_websockets-1.0.3/npm/df_websockets/html.js`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/npm/package-lock.json` & `df_websockets-1.0.3/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/npm/webpack.config.js` & `df_websockets-1.0.3/npm/webpack.config.js`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/pre-commit.sh` & `df_websockets-1.0.3/pre-commit.sh`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/setup.cfg` & `df_websockets-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/setup.py` & `df_websockets-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/test_df_websockets/test_consumers.py` & `df_websockets-1.0.3/test_df_websockets/test_consumers.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/test_df_websockets/test_decorators.py` & `df_websockets-1.0.3/test_df_websockets/test_decorators.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/test_df_websockets/test_middleware.py` & `df_websockets-1.0.3/test_df_websockets/test_middleware.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/test_df_websockets/test_testing.py` & `df_websockets-1.0.3/test_df_websockets/test_testing.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.2/test_df_websockets/test_window_info.py` & `df_websockets-1.0.3/test_df_websockets/test_window_info.py`

 * *Files identical despite different names*

