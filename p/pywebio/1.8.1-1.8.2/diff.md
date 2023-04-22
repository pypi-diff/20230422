# Comparing `tmp/pywebio-1.8.1.tar.gz` & `tmp/pywebio-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywebio-1.8.1.tar", last modified: Sun Apr 16 03:43:36 2023, max compression
+gzip compressed data, was "dist/pywebio-1.8.2.tar", last modified: Sat Apr 22 05:38:28 2023, max compression
```

## Comparing `pywebio-1.8.1.tar` & `pywebio-1.8.2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-16 03:43:06.000000 pywebio-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-16 03:43:36.000000 pywebio-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-16 03:43:06.000000 pywebio-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/demos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:06.000000 pywebio-1.8.1/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-16 03:43:06.000000 pywebio-1.8.1/demos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-16 03:43:06.000000 pywebio-1.8.1/demos/bmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-16 03:43:06.000000 pywebio-1.8.1/demos/bokeh_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-16 03:43:06.000000 pywebio-1.8.1/demos/chat_room.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-16 03:43:06.000000 pywebio-1.8.1/demos/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-16 03:43:06.000000 pywebio-1.8.1/demos/doc_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-16 03:43:06.000000 pywebio-1.8.1/demos/gomoku_game.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-16 03:43:06.000000 pywebio-1.8.1/demos/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-16 03:43:06.000000 pywebio-1.8.1/demos/input_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-16 03:43:06.000000 pywebio-1.8.1/demos/markdown_previewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-04-16 03:43:06.000000 pywebio-1.8.1/demos/output_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-16 03:43:06.000000 pywebio-1.8.1/demos/set_env_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13864 2023-04-16 03:43:06.000000 pywebio-1.8.1/demos/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio/html/codemirror/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/codemirror/active-line.js
--rw-r--r--   0 runner    (1001) docker     (123)    29098 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/codemirror/addons.js
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/codemirror/autorefresh.js
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/codemirror/loadmode.js
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/codemirror/matchbrackets.js
--rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/codemirror/python.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio/html/css/
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/css/app.css
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/css/bootstrap-select.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio/html/css/bs-theme/
--rw-r--r--   0 runner    (1001) docker     (123)   183536 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/css/bs-theme/dark.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   162100 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/css/bs-theme/default.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   166623 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/css/bs-theme/minty.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   167654 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/css/bs-theme/sketchy.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   169188 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/css/bs-theme/yeti.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/css/codemirror.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    16294 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/css/markdown.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/css/toastify.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio/html/image/
--rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/image/apple-touch-icon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      265 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/image/favicon_closed_16.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/image/favicon_closed_32.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      251 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/image/favicon_open_16.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      466 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/image/favicon_open_32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio/html/js/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2611 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/js/FileSaver.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    53596 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/js/bootstrap-select.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    60010 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/js/bs-custom-file-input.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   169793 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/js/codemirror.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    88145 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/js/jquery.min.js
--rwxr-xr-x   0 runner    (1001) docker     (123)    11143 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/js/mustache.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/js/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    74085 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/js/prism.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    17886 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/js/purify.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   129423 2023-04-16 03:43:29.000000 pywebio-1.8.1/pywebio/html/js/pywebio.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/js/require.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/html/js/toastify.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    37649 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/input.py
--rw-r--r--   0 runner    (1001) docker     (123)    14584 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/io_ctrl.py
--rw-r--r--   0 runner    (1001) docker     (123)    92960 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    17511 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/pin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio/platform/
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio/platform/adaptor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15561 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/adaptor/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/adaptor/ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/bokeh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/path_deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio/platform/pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/pyinstaller/hook-pywebio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/remote_access.py
--rw-r--r--   0 runner    (1001) docker     (123)    18817 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/tornado.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/tornado_http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio/platform/tpl/
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/tpl/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/platform/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio/session/
--rw-r--r--   0 runner    (1001) docker     (123)    21572 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/session/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/session/coroutinebased.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/session/threadbased.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-04-16 03:43:06.000000 pywebio-1.8.1/pywebio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 03:43:36.000000 pywebio-1.8.1/pywebio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 03:43:36.000000 pywebio-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-16 03:43:06.000000 pywebio-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:43:36.000000 pywebio-1.8.1/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-16 03:43:06.000000 pywebio-1.8.1/tools/pywebio-path-deploy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-22 05:37:57.000000 pywebio-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-22 05:38:28.000000 pywebio-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-22 05:37:57.000000 pywebio-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 05:37:57.000000 pywebio-1.8.2/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-22 05:37:57.000000 pywebio-1.8.2/demos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-22 05:37:57.000000 pywebio-1.8.2/demos/bmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-22 05:37:57.000000 pywebio-1.8.2/demos/bokeh_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-22 05:37:57.000000 pywebio-1.8.2/demos/chat_room.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-22 05:37:57.000000 pywebio-1.8.2/demos/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-22 05:37:57.000000 pywebio-1.8.2/demos/doc_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-22 05:37:57.000000 pywebio-1.8.2/demos/gomoku_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-22 05:37:57.000000 pywebio-1.8.2/demos/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-22 05:37:57.000000 pywebio-1.8.2/demos/input_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-22 05:37:57.000000 pywebio-1.8.2/demos/markdown_previewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-04-22 05:37:57.000000 pywebio-1.8.2/demos/output_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-22 05:37:57.000000 pywebio-1.8.2/demos/set_env_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13864 2023-04-22 05:37:57.000000 pywebio-1.8.2/demos/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio/html/codemirror/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/codemirror/active-line.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29098 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/codemirror/addons.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/codemirror/autorefresh.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/codemirror/loadmode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/codemirror/matchbrackets.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/codemirror/python.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio/html/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/css/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/css/bootstrap-select.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio/html/css/bs-theme/
+-rw-r--r--   0 runner    (1001) docker     (123)   183536 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/css/bs-theme/dark.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   162100 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/css/bs-theme/default.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   166623 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/css/bs-theme/minty.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   167654 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/css/bs-theme/sketchy.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   169188 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/css/bs-theme/yeti.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/css/codemirror.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16294 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/css/markdown.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/css/toastify.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio/html/image/
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/image/apple-touch-icon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      265 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/image/favicon_closed_16.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/image/favicon_closed_32.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      251 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/image/favicon_open_16.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      466 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/image/favicon_open_32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio/html/js/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2611 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/js/FileSaver.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    53596 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/js/bootstrap-select.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    60010 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/js/bs-custom-file-input.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   169793 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/js/codemirror.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    88145 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/js/jquery.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11143 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/js/mustache.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/js/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    74085 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/js/prism.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17886 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/js/purify.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   129639 2023-04-22 05:38:20.000000 pywebio-1.8.2/pywebio/html/js/pywebio.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/js/require.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/html/js/toastify.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    37649 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14584 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/io_ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93229 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17511 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/pin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio/platform/adaptor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15561 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/adaptor/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/adaptor/ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/bokeh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/path_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio/platform/pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/pyinstaller/hook-pywebio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/remote_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18817 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/tornado_http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio/platform/tpl/
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/tpl/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/platform/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio/session/
+-rw-r--r--   0 runner    (1001) docker     (123)    21572 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/session/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/session/coroutinebased.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/session/threadbased.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-04-22 05:37:57.000000 pywebio-1.8.2/pywebio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-22 05:38:28.000000 pywebio-1.8.2/pywebio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 05:38:28.000000 pywebio-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-22 05:37:57.000000 pywebio-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:38:28.000000 pywebio-1.8.2/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-22 05:37:57.000000 pywebio-1.8.2/tools/pywebio-path-deploy
```

### Comparing `pywebio-1.8.1/PKG-INFO` & `pywebio-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebio
-Version: 1.8.1
+Version: 1.8.2
 Summary: Write interactive web app in script way.
 Home-page: https://pywebio.readthedocs.io
 Author: WangWeimin
 Author-email: wang0.618@qq.com
 License: MIT
 Project-URL: Documentation, https://pywebio.readthedocs.io
 Project-URL: Source, https://github.com/wang0618/PyWebIO
```

### Comparing `pywebio-1.8.1/README.md` & `pywebio-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/demos/bmi.py` & `pywebio-1.8.2/demos/bmi.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/demos/bokeh_app.py` & `pywebio-1.8.2/demos/bokeh_app.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/demos/chat_room.py` & `pywebio-1.8.2/demos/chat_room.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/demos/doc_demo.py` & `pywebio-1.8.2/demos/doc_demo.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/demos/gomoku_game.py` & `pywebio-1.8.2/demos/gomoku_game.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/demos/index.py` & `pywebio-1.8.2/demos/index.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/demos/input_usage.py` & `pywebio-1.8.2/demos/input_usage.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/demos/markdown_previewer.py` & `pywebio-1.8.2/demos/markdown_previewer.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/demos/output_usage.py` & `pywebio-1.8.2/demos/output_usage.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/demos/set_env_demo.py` & `pywebio-1.8.2/demos/set_env_demo.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/demos/theme.py` & `pywebio-1.8.2/demos/theme.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/__init__.py` & `pywebio-1.8.2/pywebio/__init__.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/codemirror/active-line.js` & `pywebio-1.8.2/pywebio/html/codemirror/active-line.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/codemirror/addons.js` & `pywebio-1.8.2/pywebio/html/codemirror/addons.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/codemirror/autorefresh.js` & `pywebio-1.8.2/pywebio/html/codemirror/autorefresh.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/codemirror/loadmode.js` & `pywebio-1.8.2/pywebio/html/codemirror/loadmode.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/codemirror/matchbrackets.js` & `pywebio-1.8.2/pywebio/html/codemirror/matchbrackets.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/codemirror/python.js` & `pywebio-1.8.2/pywebio/html/codemirror/python.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/css/app.css` & `pywebio-1.8.2/pywebio/html/css/app.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/css/bootstrap-select.min.css` & `pywebio-1.8.2/pywebio/html/css/bootstrap-select.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/css/bs-theme/dark.min.css` & `pywebio-1.8.2/pywebio/html/css/bs-theme/dark.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/css/bs-theme/default.min.css` & `pywebio-1.8.2/pywebio/html/css/bs-theme/default.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/css/bs-theme/minty.min.css` & `pywebio-1.8.2/pywebio/html/css/bs-theme/minty.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/css/bs-theme/sketchy.min.css` & `pywebio-1.8.2/pywebio/html/css/bs-theme/sketchy.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/css/bs-theme/yeti.min.css` & `pywebio-1.8.2/pywebio/html/css/bs-theme/yeti.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/css/codemirror.min.css` & `pywebio-1.8.2/pywebio/html/css/codemirror.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/css/markdown.min.css` & `pywebio-1.8.2/pywebio/html/css/markdown.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/css/toastify.min.css` & `pywebio-1.8.2/pywebio/html/css/toastify.min.css`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/image/apple-touch-icon.png` & `pywebio-1.8.2/pywebio/html/image/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/image/favicon_closed_32.png` & `pywebio-1.8.2/pywebio/html/image/favicon_closed_32.png`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/js/FileSaver.min.js` & `pywebio-1.8.2/pywebio/html/js/FileSaver.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/js/bootstrap-select.min.js` & `pywebio-1.8.2/pywebio/html/js/bootstrap-select.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/js/bootstrap.min.js` & `pywebio-1.8.2/pywebio/html/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/js/bs-custom-file-input.min.js` & `pywebio-1.8.2/pywebio/html/js/bs-custom-file-input.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/js/codemirror.min.js` & `pywebio-1.8.2/pywebio/html/js/codemirror.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/js/jquery.min.js` & `pywebio-1.8.2/pywebio/html/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/js/mustache.min.js` & `pywebio-1.8.2/pywebio/html/js/mustache.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/js/popper.min.js` & `pywebio-1.8.2/pywebio/html/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/js/prism.min.js` & `pywebio-1.8.2/pywebio/html/js/prism.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/js/purify.min.js` & `pywebio-1.8.2/pywebio/html/js/purify.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/js/pywebio.min.js` & `pywebio-1.8.2/pywebio/html/js/pywebio.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2413,26 +2413,31 @@
                     return t.data[o(e.id_field)]
                 });
                 var v = null,
                     g = new Promise((function(e, t) {
                         v = e
                     }));
                 e.instance_id && (window["ag_grid_" + e.instance_id + "_promise"] = g);
-                var b = Object.assign(Object.assign(Object.assign({}, p), e.grid_args), {
+                var b = e.field_args && Object.keys(e.field_args).some((function(t) {
+                        return e.field_args[t].flex
+                    })) || e.path_args && e.path_args.some((function(e) {
+                        return e[1].flex
+                    })) || (e.grid_args.defaultColDef || {}).flex,
+                    y = Object.assign(Object.assign(Object.assign({}, p), e.grid_args), {
                         path2field: o,
                         field2path: s,
                         spec: e,
                         flatten_row: c,
                         getRowId: m,
                         rowData: _.rowData,
                         columnDefs: _.columnDefs,
-                        rowSelection: e.actions.length > 0 && (e.multiple_select ? "multiple" : "single"),
+                        rowSelection: (e.actions.length > 0 || e.on_select) && (e.multiple_select ? "multiple" : "single"),
                         defaultColDef: Object.assign(Object.assign({}, h), e.grid_args.defaultColDef || {}),
                         getSelectedRowIDs: function() {
-                            var t = b.api.getSelectedNodes(),
+                            var t = y.api.getSelectedNodes(),
                                 n = [],
                                 i = !0,
                                 r = !1,
                                 a = void 0;
                             try {
                                 for (var o, s = t[Symbol.iterator](); !(i = (o = s.next()).done); i = !0) {
                                     var l = o.value;
@@ -2448,62 +2453,64 @@
                                 }
                             }
                             return e.id_field || (n = n.map((function(e) {
                                 return parseInt(e)
                             }))), n
                         },
                         onGridReady: function(t) {
-                            v(b), f && b.api.setDomLayout("autoHeight");
+                            v(y), f && y.api.setDomLayout("autoHeight");
                             var i = n.find(".ag-grid")[0],
                                 r = Promise.resolve();
                             0 === i.clientWidth && (r = new Promise((function(e) {
                                 new ResizeObserver((function(t, n) {
                                     i.clientWidth > 0 && (n.disconnect(), e())
                                 })).observe(i)
                             }))), r.then((function() {
-                                b.columnApi.autoSizeAllColumns();
-                                var e = 0;
-                                b.columnApi.getColumns().forEach((function(t) {
-                                    t.getColDef().hide || (e += t.getActualWidth())
-                                })), e < i.clientWidth && b.api.sizeColumnsToFit()
+                                if (!b) {
+                                    y.columnApi.autoSizeAllColumns();
+                                    var e = 0;
+                                    y.columnApi.getColumns().forEach((function(t) {
+                                        t.getColDef().hide || (e += t.getActualWidth())
+                                    })), e < i.clientWidth && y.api.sizeColumnsToFit()
+                                }
                             })), e.actions.length > 0 && n.find(".ag-grid-tools").css("opacity", 1), n.find(".grid-unselect .act-btn").on("click", (function() {
-                                return b.api.deselectAll()
+                                return y.api.deselectAll()
                             }));
                             var o = function(t) {
                                 var i = e.actions[t];
                                 if (null === i) n.find(".grid-actions").append('<div class="sep"></div>');
                                 else {
                                     var r = $('<div class="act-btn">' + i + "</div>");
                                     r.on("click", (function() {
                                         a.pushData({
                                             btn: parseInt(t),
-                                            rows: b.getSelectedRowIDs()
+                                            rows: y.getSelectedRowIDs()
                                         }, e.callback_id)
                                     })), n.find(".grid-actions").append(r)
                                 }
                             };
                             for (var s in e.actions) o(s);
                             d("agGrid.onGridReady()", e.grid_args.onGridReady, t)
                         },
                         onCellFocused: function(t) {
-                            var i = b.api.getDisplayedRowAtIndex(t.rowIndex),
-                                r = b.api.getValue(t.column, i);
+                            var i = y.api.getDisplayedRowAtIndex(t.rowIndex),
+                                r = y.api.getValue(t.column, i);
                             (void 0 === r && (r = ""), e.cell_content_bar) && n.find(".ag-grid-cell-bar").text(r).show();
                             d("agGrid.onCellFocused()", e.grid_args.onCellFocused, t)
                         },
                         onSelectionChanged: function(t) {
-                            var i = b.getSelectedRowIDs();
+                            var i = y.getSelectedRowIDs();
                             e.on_select && i.length > 0 && a.pushData({
                                 rows: i
                             }, e.callback_id), n.find(".ag-grid-row-count").text(i.length), n.find(".ag-grid-row-unit").text(i.length > 1 ? "rows" : "row"), 0 === i.length && n.find(".ag-grid-tools .grid-unselect, .ag-grid-tools .grid-actions").hide(), i.length >= 1 && n.find(".ag-grid-tools .grid-unselect, .ag-grid-tools .grid-actions").fadeIn(200), d("agGrid.onSelectionChanged()", e.grid_args.onSelectionChanged, t)
                         }
                     }),
-                    y = e.enterprise_key ? "ag-grid-enterprise" : "ag-grid";
-                return requirejs([y], (function(t) {
-                    n.find(".grid-loading").remove(), new t.Grid(n.find(".ag-grid")[0], b), e.instance_id && (window["ag_grid_" + e.instance_id] = b)
+                    k = e.enterprise_key ? "ag-grid-enterprise" : "ag-grid";
+                return requirejs([k], (function(t) {
+                    n.find(".grid-loading").remove(), new t.Grid(n.find(".ag-grid")[0], y), e.instance_id && (window["ag_grid_" + e.instance_id] = y)
                 })), n
             }
         }
     }, {
         "../session": 25
     }],
     14: [function(e, t, n) {
```

### Comparing `pywebio-1.8.1/pywebio/html/js/require.min.js` & `pywebio-1.8.2/pywebio/html/js/require.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/html/js/toastify.min.js` & `pywebio-1.8.2/pywebio/html/js/toastify.min.js`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/input.py` & `pywebio-1.8.2/pywebio/input.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/io_ctrl.py` & `pywebio-1.8.2/pywebio/io_ctrl.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/output.py` & `pywebio-1.8.2/pywebio/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1490,15 +1490,15 @@
         id_field: str = None,
         height: Union[str, int] = 600,
         theme: "Literal['alpine', 'alpine-dark', 'balham', 'balham-dark', 'material']" = 'balham',
         cell_content_bar=True,
         instance_id='',
         column_order: Union[SequenceType[str], MappingType] = None,
         column_args: MappingType[Union[str, Tuple], MappingType] = None,
-        grid_args: MappingType[str, MappingType] = None,
+        grid_args: MappingType[str, Any] = None,
         enterprise_key='',
         scope: str = None,
         position: int = OutputPosition.BOTTOM
 ) -> Output:
     """
     Output a datatable.
 
@@ -1536,14 +1536,15 @@
         Default is ``True``.
     :param str instance_id: Assign a unique ID to the datatable, so that you can refer this datatable in
         `datatable_update()`, `datatable_insert()` and `datatable_remove()` functions.
 
     :param list column_order: column order, the order of the column names in the list will be used as the column order.
         If not provided, the column order will be the same as the order of the keys in the first row of ``records``.
         When provided, the column not in the list will not be shown.
+        Note that ``column_order`` must be specified when ``records`` is empty.
 
         .. collapse:: Notes when the row record is nested dict
 
            Since the ``dict`` in python is ordered after py3.7, you can use dict to specify the column order when the
            row record is nested dict. For example::
 
                 column_order = {'a': {'b': {'c': None, 'd': None}, 'e': None}, 'f': None}
@@ -1627,37 +1628,28 @@
         The implement of `datatable_update()`, `datatable_insert` and `datatable_remove` functions are good examples
         to show how to interact with ag-grid in Javascript.
     """
     actions = actions or []
     column_args = column_args or {}
     grid_args = grid_args or {}
 
+    if not records and not column_order:
+        raise ValueError('`column_order` must be specified when `records` is empty')
+
     if isinstance(height, int):
         height = f"{height}px"
     if height == 'auto' and len(records) > 1000:
         height = '600px'
         logger.warning("put_datatable: numbers of rows are too large to use auto height, use fix height instead")
 
     if isinstance(id_field, str):
         id_field = [id_field]
 
     js_func_key = random_str(10)
 
-    def json_encoder(obj):
-        if isinstance(obj, JSFunction):
-            return dict(
-                __pywebio_js_function__=js_func_key,
-                params=obj.params,
-                body=obj.body,
-            )
-        raise TypeError
-
-    column_args = json.loads(json.dumps(column_args, default=json_encoder))
-    grid_args = json.loads(json.dumps(grid_args, default=json_encoder))
-
     def callback(data: Dict):
         rows = data['rows'] if multiple_select else data['rows'][0]
 
         if "btn" not in data and onselect is not None:
             return onselect(rows)
 
         _, cb = actions[data['btn']]
@@ -1667,14 +1659,27 @@
     if actions or onselect:
         callback_id = output_register_callback(callback)
 
     action_labels = [a[0] if a else None for a in actions]
     field_args = {k: v for k, v in column_args.items() if isinstance(k, str)}
     path_args = [(k, v) for k, v in column_args.items() if not isinstance(k, str)]
 
+    def json_encoder(obj):
+        if isinstance(obj, JSFunction):
+            return dict(
+                __pywebio_js_function__=js_func_key,
+                params=obj.params,
+                body=obj.body,
+            )
+        raise TypeError
+
+    field_args = json.loads(json.dumps(field_args, default=json_encoder))
+    path_args = json.loads(json.dumps(path_args, default=json_encoder))
+    grid_args = json.loads(json.dumps(grid_args, default=json_encoder))
+
     if isinstance(column_order, (list, tuple)):
         column_order = {k: None for k in column_order}
 
     spec = _get_output_spec(
         'datatable',
         records=records, callback_id=callback_id, actions=action_labels, on_select=onselect is not None,
         id_field=id_field, column_order=column_order,
```

### Comparing `pywebio-1.8.1/pywebio/pin.py` & `pywebio-1.8.2/pywebio/pin.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/platform/__init__.py` & `pywebio-1.8.2/pywebio/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/platform/adaptor/http.py` & `pywebio-1.8.2/pywebio/platform/adaptor/http.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/platform/adaptor/ws.py` & `pywebio-1.8.2/pywebio/platform/adaptor/ws.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/platform/aiohttp.py` & `pywebio-1.8.2/pywebio/platform/aiohttp.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/platform/bokeh.py` & `pywebio-1.8.2/pywebio/platform/bokeh.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/platform/django.py` & `pywebio-1.8.2/pywebio/platform/django.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/platform/fastapi.py` & `pywebio-1.8.2/pywebio/platform/fastapi.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/platform/flask.py` & `pywebio-1.8.2/pywebio/platform/flask.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/platform/page.py` & `pywebio-1.8.2/pywebio/platform/page.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/platform/path_deploy.py` & `pywebio-1.8.2/pywebio/platform/path_deploy.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/platform/remote_access.py` & `pywebio-1.8.2/pywebio/platform/remote_access.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/platform/tornado.py` & `pywebio-1.8.2/pywebio/platform/tornado.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/platform/tornado_http.py` & `pywebio-1.8.2/pywebio/platform/tornado_http.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/platform/tpl/index.html` & `pywebio-1.8.2/pywebio/platform/tpl/index.html`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/platform/utils.py` & `pywebio-1.8.2/pywebio/platform/utils.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/session/__init__.py` & `pywebio-1.8.2/pywebio/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/session/base.py` & `pywebio-1.8.2/pywebio/session/base.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/session/coroutinebased.py` & `pywebio-1.8.2/pywebio/session/coroutinebased.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/session/threadbased.py` & `pywebio-1.8.2/pywebio/session/threadbased.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio/utils.py` & `pywebio-1.8.2/pywebio/utils.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/pywebio.egg-info/PKG-INFO` & `pywebio-1.8.2/pywebio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebio
-Version: 1.8.1
+Version: 1.8.2
 Summary: Write interactive web app in script way.
 Home-page: https://pywebio.readthedocs.io
 Author: WangWeimin
 Author-email: wang0.618@qq.com
 License: MIT
 Project-URL: Documentation, https://pywebio.readthedocs.io
 Project-URL: Source, https://github.com/wang0618/PyWebIO
```

### Comparing `pywebio-1.8.1/pywebio.egg-info/SOURCES.txt` & `pywebio-1.8.2/pywebio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/setup.py` & `pywebio-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `pywebio-1.8.1/tools/pywebio-path-deploy` & `pywebio-1.8.2/tools/pywebio-path-deploy`

 * *Files identical despite different names*

