# Comparing `tmp/sosse-0.dev4.tar.gz` & `tmp/sosse-0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosse-0.dev4.tar", last modified: Sat Apr 22 09:36:56 2023, max compression
+gzip compressed data, was "sosse-0.dev5.tar", last modified: Sat Apr 22 10:24:48 2023, max compression
```

## Comparing `sosse-0.dev4.tar` & `sosse-0.dev5.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:36:56.498721 sosse-0.dev4/
--rw-r--r--   0 root         (0) root         (0)    34523 2022-10-02 17:55:35.000000 sosse-0.dev4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       94 2023-04-22 08:58:29.000000 sosse-0.dev4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2785 2023-04-22 09:36:56.498721 sosse-0.dev4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2392 2023-04-21 16:16:29.000000 sosse-0.dev4/README.md
--rw-r--r--   0 root         (0) root         (0)      892 2023-04-20 13:26:25.000000 sosse-0.dev4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      129 2022-10-18 20:27:33.000000 sosse-0.dev4/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:36:56.438720 sosse-0.dev4/se/
--rw-r--r--   0 root         (0) root         (0)        0 2020-07-14 21:23:14.000000 sosse-0.dev4/se/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19185 2020-07-14 21:23:14.000000 sosse-0.dev4/se/admin.py
--rw-r--r--   0 root         (0) root         (0)      996 2020-07-14 21:23:14.000000 sosse-0.dev4/se/apps.py
--rw-r--r--   0 root         (0) root         (0)     4119 2020-07-14 21:23:14.000000 sosse-0.dev4/se/atom.py
--rw-r--r--   0 root         (0) root         (0)    24133 2020-07-14 21:23:14.000000 sosse-0.dev4/se/browser.py
--rw-r--r--   0 root         (0) root         (0)     2804 2020-07-14 21:23:14.000000 sosse-0.dev4/se/cached.py
--rw-r--r--   0 root         (0) root         (0)     4314 2020-07-14 21:23:14.000000 sosse-0.dev4/se/forms.py
--rw-r--r--   0 root         (0) root         (0)     1150 2020-07-14 21:23:14.000000 sosse-0.dev4/se/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:36:56.442720 sosse-0.dev4/se/management/
--rw-r--r--   0 root         (0) root         (0)        0 2020-07-14 21:23:14.000000 sosse-0.dev4/se/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:36:56.446720 sosse-0.dev4/se/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2020-07-14 21:23:14.000000 sosse-0.dev4/se/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4063 2020-07-14 21:23:14.000000 sosse-0.dev4/se/management/commands/crawl.py
--rw-r--r--   0 root         (0) root         (0)     1343 2020-07-14 21:23:14.000000 sosse-0.dev4/se/management/commands/default_admin.py
--rw-r--r--   0 root         (0) root         (0)      951 2020-07-14 21:23:14.000000 sosse-0.dev4/se/management/commands/default_conf.py
--rw-r--r--   0 root         (0) root         (0)      951 2020-07-14 21:23:14.000000 sosse-0.dev4/se/management/commands/default_conf2.py
--rw-r--r--   0 root         (0) root         (0)     2363 2023-04-21 19:46:35.000000 sosse-0.dev4/se/management/commands/extract_doc.py
--rw-r--r--   0 root         (0) root         (0)     1162 2020-07-14 21:23:14.000000 sosse-0.dev4/se/management/commands/generate_secret.py
--rw-r--r--   0 root         (0) root         (0)     1082 2020-07-14 21:23:14.000000 sosse-0.dev4/se/management/commands/load_se.py
--rw-r--r--   0 root         (0) root         (0)     1543 2023-04-22 09:34:05.000000 sosse-0.dev4/se/management/commands/update_se.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:36:56.446720 sosse-0.dev4/se/migrations/
--rw-r--r--   0 root         (0) root         (0)    13875 2020-07-14 21:23:14.000000 sosse-0.dev4/se/migrations/0001_initial.py
--rwxr-xr-x   0 root         (0) root         (0)     2976 2020-07-14 21:23:14.000000 sosse-0.dev4/se/migrations/0002_search_vector.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-07-14 21:23:14.000000 sosse-0.dev4/se/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54928 2020-07-14 21:23:14.000000 sosse-0.dev4/se/models.py
--rw-r--r--   0 root         (0) root         (0)     1941 2020-07-14 21:23:14.000000 sosse-0.dev4/se/screenshot.py
--rw-r--r--   0 root         (0) root         (0)     6607 2020-07-14 21:23:14.000000 sosse-0.dev4/se/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:36:56.410720 sosse-0.dev4/se/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:36:56.458720 sosse-0.dev4/se/static/se/
--rw-r--r--   0 root         (0) root         (0)    19511 2020-07-14 21:23:14.000000 sosse-0.dev4/se/static/se/admin-base.css
--rw-r--r--   0 root         (0) root         (0)     8810 2020-07-14 21:23:14.000000 sosse-0.dev4/se/static/se/admin-forms.css
--rw-r--r--   0 root         (0) root         (0)     2005 2020-07-14 21:23:14.000000 sosse-0.dev4/se/static/se/base.js
--rw-r--r--   0 root         (0) root         (0)     2435 2020-07-14 21:23:14.000000 sosse-0.dev4/se/static/se/icon-atom.svg
--rw-r--r--   0 root         (0) root         (0)     2196 2020-07-14 21:23:14.000000 sosse-0.dev4/se/static/se/icon-clear.svg
--rw-r--r--   0 root         (0) root         (0)     3722 2020-07-14 21:23:14.000000 sosse-0.dev4/se/static/se/icon-cog.svg
--rw-r--r--   0 root         (0) root         (0)     6887 2020-07-14 21:23:14.000000 sosse-0.dev4/se/static/se/icon-search.svg
--rw-r--r--   0 root         (0) root         (0)     2488 2020-07-14 21:23:14.000000 sosse-0.dev4/se/static/se/icon-stats.svg
--rw-r--r--   0 root         (0) root         (0)     3644 2020-07-14 21:23:14.000000 sosse-0.dev4/se/static/se/icon-trash.svg
--rw-r--r--   0 root         (0) root         (0)     2771 2020-07-14 21:23:14.000000 sosse-0.dev4/se/static/se/icon-user.svg
--rw-r--r--   0 root         (0) root         (0)     9798 2020-07-14 21:23:14.000000 sosse-0.dev4/se/static/se/index.js
--rw-r--r--   0 root         (0) root         (0)     9908 2020-07-14 21:23:14.000000 sosse-0.dev4/se/static/se/logo.svg
--rw-r--r--   0 root         (0) root         (0)     5967 2020-07-14 21:23:14.000000 sosse-0.dev4/se/static/se/pygal-tooltips.min.js
--rw-r--r--   0 root         (0) root         (0)      982 2020-07-14 21:23:14.000000 sosse-0.dev4/se/static/se/screenshot.js
--rw-r--r--   0 root         (0) root         (0)     2522 2020-07-14 21:23:14.000000 sosse-0.dev4/se/static/se/style.css
--rw-r--r--   0 root         (0) root         (0)     8567 2020-07-14 21:23:14.000000 sosse-0.dev4/se/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:36:56.410720 sosse-0.dev4/se/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:36:56.466720 sosse-0.dev4/se/templates/admin/
--rw-r--r--   0 root         (0) root         (0)     3427 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/admin/add_to_queue.html
--rw-r--r--   0 root         (0) root         (0)     2518 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/admin/app_list.html
--rw-r--r--   0 root         (0) root         (0)     2270 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/admin/base.html
--rw-r--r--   0 root         (0) root         (0)      105 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/admin/base_site.html
--rw-r--r--   0 root         (0) root         (0)      677 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/admin/change_form.html
--rw-r--r--   0 root         (0) root         (0)      905 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/admin/crawl_status.html
--rw-r--r--   0 root         (0) root         (0)     2710 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/admin/crawl_status_content.html
--rw-r--r--   0 root         (0) root         (0)       69 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/admin/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:36:56.486720 sosse-0.dev4/se/templates/se/
--rw-r--r--   0 root         (0) root         (0)      661 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/se/about.html
--rw-r--r--   0 root         (0) root         (0)     1473 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/se/base.html
--rw-r--r--   0 root         (0) root         (0)     2256 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/se/cached.html
--rw-r--r--   0 root         (0) root         (0)     1870 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/se/history.html
--rw-r--r--   0 root         (0) root         (0)     8099 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/se/index.html
--rw-r--r--   0 root         (0) root         (0)     1320 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/se/main_menu.html
--rw-r--r--   0 root         (0) root         (0)      545 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/se/opensearch.xml
--rw-r--r--   0 root         (0) root         (0)      761 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/se/pagination.html
--rw-r--r--   0 root         (0) root         (0)     2242 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/se/prefs.html
--rw-r--r--   0 root         (0) root         (0)     1706 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/se/screenshot.html
--rw-r--r--   0 root         (0) root         (0)     1523 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/se/search_redirect.html
--rw-r--r--   0 root         (0) root         (0)     1547 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/se/stats.html
--rw-r--r--   0 root         (0) root         (0)      741 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/se/unknown_url.html
--rw-r--r--   0 root         (0) root         (0)      474 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/se/words.html
--rw-r--r--   0 root         (0) root         (0)      361 2020-07-14 21:23:14.000000 sosse-0.dev4/se/templates/se/www.html
--rw-r--r--   0 root         (0) root         (0)     5979 2020-07-14 21:23:14.000000 sosse-0.dev4/se/test_cookie.py
--rw-r--r--   0 root         (0) root         (0)    13928 2020-07-14 21:23:14.000000 sosse-0.dev4/se/test_crawl.py
--rw-r--r--   0 root         (0) root         (0)     9545 2020-07-14 21:23:14.000000 sosse-0.dev4/se/test_functionals.py
--rw-r--r--   0 root         (0) root         (0)     1459 2020-07-14 21:23:14.000000 sosse-0.dev4/se/test_misc.py
--rw-r--r--   0 root         (0) root         (0)     4659 2020-07-14 21:23:14.000000 sosse-0.dev4/se/test_parser.py
--rw-r--r--   0 root         (0) root         (0)     2133 2020-07-14 21:23:14.000000 sosse-0.dev4/se/test_redirect.py
--rw-r--r--   0 root         (0) root         (0)     1600 2020-07-14 21:23:14.000000 sosse-0.dev4/se/test_requests.py
--rw-r--r--   0 root         (0) root         (0)     9547 2020-07-14 21:23:14.000000 sosse-0.dev4/se/test_search.py
--rw-r--r--   0 root         (0) root         (0)     2612 2020-07-14 21:23:14.000000 sosse-0.dev4/se/test_url.py
--rw-r--r--   0 root         (0) root         (0)     6286 2020-07-14 21:23:14.000000 sosse-0.dev4/se/test_views.py
--rw-r--r--   0 root         (0) root         (0)     3101 2020-07-14 21:23:14.000000 sosse-0.dev4/se/utils.py
--rw-r--r--   0 root         (0) root         (0)     7784 2020-07-14 21:23:14.000000 sosse-0.dev4/se/views.py
--rw-r--r--   0 root         (0) root         (0)     1587 2020-07-14 21:23:14.000000 sosse-0.dev4/se/words.py
--rw-r--r--   0 root         (0) root         (0)     2805 2020-07-14 21:23:14.000000 sosse-0.dev4/se/www.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 09:36:56.502721 sosse-0.dev4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:36:56.494721 sosse-0.dev4/sosse/
--rw-r--r--   0 root         (0) root         (0)        0 2020-07-14 21:23:14.000000 sosse-0.dev4/sosse/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16218 2023-04-21 22:28:27.000000 sosse-0.dev4/sosse/conf.py
--rw-r--r--   0 root         (0) root         (0)     7379 2023-04-22 09:36:19.000000 sosse-0.dev4/sosse/settings.py
--rwxr-xr-x   0 root         (0) root         (0)     1328 2023-04-21 16:16:29.000000 sosse-0.dev4/sosse/sosse_admin.py
--rw-r--r--   0 root         (0) root         (0)     2548 2020-07-14 21:23:14.000000 sosse-0.dev4/sosse/urls.py
--rw-r--r--   0 root         (0) root         (0)     1089 2020-07-14 21:23:14.000000 sosse-0.dev4/sosse/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:36:56.498721 sosse-0.dev4/sosse.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2785 2023-04-22 09:36:56.000000 sosse-0.dev4/sosse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2293 2023-04-22 09:36:56.000000 sosse-0.dev4/sosse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 09:36:56.000000 sosse-0.dev4/sosse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-22 09:36:56.000000 sosse-0.dev4/sosse.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      129 2023-04-22 09:36:56.000000 sosse-0.dev4/sosse.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-22 09:36:56.000000 sosse-0.dev4/sosse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:24:48.045176 sosse-0.dev5/
+-rw-r--r--   0 root         (0) root         (0)    34523 2022-10-02 17:55:35.000000 sosse-0.dev5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      112 2023-04-22 10:24:18.000000 sosse-0.dev5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-04-22 10:24:48.045176 sosse-0.dev5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2392 2023-04-21 16:16:29.000000 sosse-0.dev5/README.md
+-rw-r--r--   0 root         (0) root         (0)      892 2023-04-20 13:26:25.000000 sosse-0.dev5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      129 2022-10-18 20:27:33.000000 sosse-0.dev5/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:24:48.013175 sosse-0.dev5/se/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-07-14 21:23:14.000000 sosse-0.dev5/se/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19185 2020-07-14 21:23:14.000000 sosse-0.dev5/se/admin.py
+-rw-r--r--   0 root         (0) root         (0)      996 2020-07-14 21:23:14.000000 sosse-0.dev5/se/apps.py
+-rw-r--r--   0 root         (0) root         (0)     4119 2020-07-14 21:23:14.000000 sosse-0.dev5/se/atom.py
+-rw-r--r--   0 root         (0) root         (0)    24133 2020-07-14 21:23:14.000000 sosse-0.dev5/se/browser.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2020-07-14 21:23:14.000000 sosse-0.dev5/se/cached.py
+-rw-r--r--   0 root         (0) root         (0)     4314 2020-07-14 21:23:14.000000 sosse-0.dev5/se/forms.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2020-07-14 21:23:14.000000 sosse-0.dev5/se/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:24:48.013175 sosse-0.dev5/se/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-07-14 21:23:14.000000 sosse-0.dev5/se/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:24:48.017175 sosse-0.dev5/se/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-07-14 21:23:14.000000 sosse-0.dev5/se/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4063 2020-07-14 21:23:14.000000 sosse-0.dev5/se/management/commands/crawl.py
+-rw-r--r--   0 root         (0) root         (0)     1343 2020-07-14 21:23:14.000000 sosse-0.dev5/se/management/commands/default_admin.py
+-rw-r--r--   0 root         (0) root         (0)      951 2020-07-14 21:23:14.000000 sosse-0.dev5/se/management/commands/default_conf.py
+-rw-r--r--   0 root         (0) root         (0)      951 2020-07-14 21:23:14.000000 sosse-0.dev5/se/management/commands/default_conf2.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2023-04-21 19:46:35.000000 sosse-0.dev5/se/management/commands/extract_doc.py
+-rw-r--r--   0 root         (0) root         (0)     1162 2020-07-14 21:23:14.000000 sosse-0.dev5/se/management/commands/generate_secret.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2020-07-14 21:23:14.000000 sosse-0.dev5/se/management/commands/load_se.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-04-22 09:41:23.000000 sosse-0.dev5/se/management/commands/update_se.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:24:48.017175 sosse-0.dev5/se/migrations/
+-rw-r--r--   0 root         (0) root         (0)    13875 2020-07-14 21:23:14.000000 sosse-0.dev5/se/migrations/0001_initial.py
+-rwxr-xr-x   0 root         (0) root         (0)     2976 2020-07-14 21:23:14.000000 sosse-0.dev5/se/migrations/0002_search_vector.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-07-14 21:23:14.000000 sosse-0.dev5/se/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54928 2020-07-14 21:23:14.000000 sosse-0.dev5/se/models.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2020-07-14 21:23:14.000000 sosse-0.dev5/se/screenshot.py
+-rw-r--r--   0 root         (0) root         (0)     6607 2020-07-14 21:23:14.000000 sosse-0.dev5/se/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:24:47.993175 sosse-0.dev5/se/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:24:48.025175 sosse-0.dev5/se/static/se/
+-rw-r--r--   0 root         (0) root         (0)    19511 2020-07-14 21:23:14.000000 sosse-0.dev5/se/static/se/admin-base.css
+-rw-r--r--   0 root         (0) root         (0)     8810 2020-07-14 21:23:14.000000 sosse-0.dev5/se/static/se/admin-forms.css
+-rw-r--r--   0 root         (0) root         (0)     2005 2020-07-14 21:23:14.000000 sosse-0.dev5/se/static/se/base.js
+-rw-r--r--   0 root         (0) root         (0)     2435 2020-07-14 21:23:14.000000 sosse-0.dev5/se/static/se/icon-atom.svg
+-rw-r--r--   0 root         (0) root         (0)     2196 2020-07-14 21:23:14.000000 sosse-0.dev5/se/static/se/icon-clear.svg
+-rw-r--r--   0 root         (0) root         (0)     3722 2020-07-14 21:23:14.000000 sosse-0.dev5/se/static/se/icon-cog.svg
+-rw-r--r--   0 root         (0) root         (0)     6887 2020-07-14 21:23:14.000000 sosse-0.dev5/se/static/se/icon-search.svg
+-rw-r--r--   0 root         (0) root         (0)     2488 2020-07-14 21:23:14.000000 sosse-0.dev5/se/static/se/icon-stats.svg
+-rw-r--r--   0 root         (0) root         (0)     3644 2020-07-14 21:23:14.000000 sosse-0.dev5/se/static/se/icon-trash.svg
+-rw-r--r--   0 root         (0) root         (0)     2771 2020-07-14 21:23:14.000000 sosse-0.dev5/se/static/se/icon-user.svg
+-rw-r--r--   0 root         (0) root         (0)     9798 2020-07-14 21:23:14.000000 sosse-0.dev5/se/static/se/index.js
+-rw-r--r--   0 root         (0) root         (0)     9908 2020-07-14 21:23:14.000000 sosse-0.dev5/se/static/se/logo.svg
+-rw-r--r--   0 root         (0) root         (0)     5967 2020-07-14 21:23:14.000000 sosse-0.dev5/se/static/se/pygal-tooltips.min.js
+-rw-r--r--   0 root         (0) root         (0)      982 2020-07-14 21:23:14.000000 sosse-0.dev5/se/static/se/screenshot.js
+-rw-r--r--   0 root         (0) root         (0)     2522 2020-07-14 21:23:14.000000 sosse-0.dev5/se/static/se/style.css
+-rw-r--r--   0 root         (0) root         (0)     8567 2020-07-14 21:23:14.000000 sosse-0.dev5/se/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:24:47.997175 sosse-0.dev5/se/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:24:48.029175 sosse-0.dev5/se/templates/admin/
+-rw-r--r--   0 root         (0) root         (0)     3427 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/admin/add_to_queue.html
+-rw-r--r--   0 root         (0) root         (0)     2518 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/admin/app_list.html
+-rw-r--r--   0 root         (0) root         (0)     2270 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/admin/base.html
+-rw-r--r--   0 root         (0) root         (0)      105 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/admin/base_site.html
+-rw-r--r--   0 root         (0) root         (0)      677 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/admin/change_form.html
+-rw-r--r--   0 root         (0) root         (0)      905 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/admin/crawl_status.html
+-rw-r--r--   0 root         (0) root         (0)     2710 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/admin/crawl_status_content.html
+-rw-r--r--   0 root         (0) root         (0)       69 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/admin/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:24:48.037176 sosse-0.dev5/se/templates/se/
+-rw-r--r--   0 root         (0) root         (0)      661 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/se/about.html
+-rw-r--r--   0 root         (0) root         (0)     1473 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/se/base.html
+-rw-r--r--   0 root         (0) root         (0)     2256 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/se/cached.html
+-rw-r--r--   0 root         (0) root         (0)     1870 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/se/history.html
+-rw-r--r--   0 root         (0) root         (0)     8099 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/se/index.html
+-rw-r--r--   0 root         (0) root         (0)     1320 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/se/main_menu.html
+-rw-r--r--   0 root         (0) root         (0)      545 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/se/opensearch.xml
+-rw-r--r--   0 root         (0) root         (0)      761 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/se/pagination.html
+-rw-r--r--   0 root         (0) root         (0)     2242 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/se/prefs.html
+-rw-r--r--   0 root         (0) root         (0)     1706 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/se/screenshot.html
+-rw-r--r--   0 root         (0) root         (0)     1523 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/se/search_redirect.html
+-rw-r--r--   0 root         (0) root         (0)     1547 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/se/stats.html
+-rw-r--r--   0 root         (0) root         (0)      741 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/se/unknown_url.html
+-rw-r--r--   0 root         (0) root         (0)      474 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/se/words.html
+-rw-r--r--   0 root         (0) root         (0)      361 2020-07-14 21:23:14.000000 sosse-0.dev5/se/templates/se/www.html
+-rw-r--r--   0 root         (0) root         (0)     5979 2020-07-14 21:23:14.000000 sosse-0.dev5/se/test_cookie.py
+-rw-r--r--   0 root         (0) root         (0)    13928 2020-07-14 21:23:14.000000 sosse-0.dev5/se/test_crawl.py
+-rw-r--r--   0 root         (0) root         (0)     9545 2020-07-14 21:23:14.000000 sosse-0.dev5/se/test_functionals.py
+-rw-r--r--   0 root         (0) root         (0)     1459 2020-07-14 21:23:14.000000 sosse-0.dev5/se/test_misc.py
+-rw-r--r--   0 root         (0) root         (0)     4659 2020-07-14 21:23:14.000000 sosse-0.dev5/se/test_parser.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2020-07-14 21:23:14.000000 sosse-0.dev5/se/test_redirect.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2020-07-14 21:23:14.000000 sosse-0.dev5/se/test_requests.py
+-rw-r--r--   0 root         (0) root         (0)     9547 2020-07-14 21:23:14.000000 sosse-0.dev5/se/test_search.py
+-rw-r--r--   0 root         (0) root         (0)     2612 2020-07-14 21:23:14.000000 sosse-0.dev5/se/test_url.py
+-rw-r--r--   0 root         (0) root         (0)     6286 2020-07-14 21:23:14.000000 sosse-0.dev5/se/test_views.py
+-rw-r--r--   0 root         (0) root         (0)     3101 2020-07-14 21:23:14.000000 sosse-0.dev5/se/utils.py
+-rw-r--r--   0 root         (0) root         (0)     7784 2020-07-14 21:23:14.000000 sosse-0.dev5/se/views.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2020-07-14 21:23:14.000000 sosse-0.dev5/se/words.py
+-rw-r--r--   0 root         (0) root         (0)     2805 2020-07-14 21:23:14.000000 sosse-0.dev5/se/www.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 10:24:48.045176 sosse-0.dev5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:24:48.041175 sosse-0.dev5/sosse/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-07-14 21:23:14.000000 sosse-0.dev5/sosse/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16218 2023-04-21 22:28:27.000000 sosse-0.dev5/sosse/conf.py
+-rw-r--r--   0 root         (0) root         (0)    18486 2023-04-02 19:20:51.000000 sosse-0.dev5/sosse/search_engines.json
+-rw-r--r--   0 root         (0) root         (0)     7379 2023-04-22 09:42:36.000000 sosse-0.dev5/sosse/settings.py
+-rwxr-xr-x   0 root         (0) root         (0)     1328 2023-04-21 16:16:29.000000 sosse-0.dev5/sosse/sosse_admin.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2020-07-14 21:23:14.000000 sosse-0.dev5/sosse/urls.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2020-07-14 21:23:14.000000 sosse-0.dev5/sosse/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:24:48.045176 sosse-0.dev5/sosse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-04-22 10:24:47.000000 sosse-0.dev5/sosse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-04-22 10:24:47.000000 sosse-0.dev5/sosse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 10:24:47.000000 sosse-0.dev5/sosse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-22 10:24:47.000000 sosse-0.dev5/sosse.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      129 2023-04-22 10:24:47.000000 sosse-0.dev5/sosse.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-22 10:24:47.000000 sosse-0.dev5/sosse.egg-info/top_level.txt
```

### Comparing `sosse-0.dev4/LICENSE` & `sosse-0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/PKG-INFO` & `sosse-0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosse
-Version: 0.dev4
+Version: 0.dev5
 Summary: Selenium Open Source Search Engine
 Author-email: Laurent Defert <laurent_defert@yahoo.fr>
 License: GNU Affero General Public License v3
 Keywords: search engine,crawler
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `sosse-0.dev4/README.md` & `sosse-0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/pyproject.toml` & `sosse-0.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/admin.py` & `sosse-0.dev5/se/admin.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/apps.py` & `sosse-0.dev5/se/apps.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/atom.py` & `sosse-0.dev5/se/atom.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/browser.py` & `sosse-0.dev5/se/browser.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/cached.py` & `sosse-0.dev5/se/cached.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/forms.py` & `sosse-0.dev5/se/forms.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/login.py` & `sosse-0.dev5/se/login.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/management/commands/crawl.py` & `sosse-0.dev5/se/management/commands/crawl.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/management/commands/default_admin.py` & `sosse-0.dev5/se/management/commands/default_admin.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/management/commands/default_conf.py` & `sosse-0.dev5/se/management/commands/default_conf.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/management/commands/default_conf2.py` & `sosse-0.dev5/se/management/commands/default_conf2.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/management/commands/extract_doc.py` & `sosse-0.dev5/se/management/commands/extract_doc.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/management/commands/generate_secret.py` & `sosse-0.dev5/se/management/commands/generate_secret.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/management/commands/load_se.py` & `sosse-0.dev5/se/management/commands/load_se.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/management/commands/update_se.py` & `sosse-0.dev5/se/management/commands/update_se.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 # the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License along with SOSSE.
 # If not, see <https://www.gnu.org/licenses/>.
 
 import json
+import os
 
+from django.conf import settings
 from django.core.management.base import BaseCommand
 
 from ...models import SearchEngine
 
 
-SE_FILE = 'sosse/search_engine.json'
+SE_FILE = 'sosse/search_engines.json'
 
 
 class Command(BaseCommand):
     help = 'Update Search engine shortcuts'
 
     def handle(self, *args, **options):
         count = 0
```

### Comparing `sosse-0.dev4/se/migrations/0001_initial.py` & `sosse-0.dev5/se/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/migrations/0002_search_vector.py` & `sosse-0.dev5/se/migrations/0002_search_vector.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/models.py` & `sosse-0.dev5/se/models.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/screenshot.py` & `sosse-0.dev5/se/screenshot.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/search.py` & `sosse-0.dev5/se/search.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/static/se/admin-base.css` & `sosse-0.dev5/se/static/se/admin-base.css`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/static/se/admin-forms.css` & `sosse-0.dev5/se/static/se/admin-forms.css`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/static/se/base.js` & `sosse-0.dev5/se/static/se/base.js`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/static/se/icon-atom.svg` & `sosse-0.dev5/se/static/se/icon-atom.svg`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/static/se/icon-clear.svg` & `sosse-0.dev5/se/static/se/icon-clear.svg`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/static/se/icon-cog.svg` & `sosse-0.dev5/se/static/se/icon-cog.svg`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/static/se/icon-search.svg` & `sosse-0.dev5/se/static/se/icon-search.svg`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/static/se/icon-stats.svg` & `sosse-0.dev5/se/static/se/icon-stats.svg`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/static/se/icon-trash.svg` & `sosse-0.dev5/se/static/se/icon-trash.svg`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/static/se/icon-user.svg` & `sosse-0.dev5/se/static/se/icon-user.svg`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/static/se/index.js` & `sosse-0.dev5/se/static/se/index.js`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/static/se/logo.svg` & `sosse-0.dev5/se/static/se/logo.svg`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/static/se/pygal-tooltips.min.js` & `sosse-0.dev5/se/static/se/pygal-tooltips.min.js`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/static/se/screenshot.js` & `sosse-0.dev5/se/static/se/screenshot.js`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/static/se/style.css` & `sosse-0.dev5/se/static/se/style.css`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/stats.py` & `sosse-0.dev5/se/stats.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/admin/add_to_queue.html` & `sosse-0.dev5/se/templates/admin/add_to_queue.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/admin/app_list.html` & `sosse-0.dev5/se/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/admin/base.html` & `sosse-0.dev5/se/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/admin/change_form.html` & `sosse-0.dev5/se/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/admin/crawl_status.html` & `sosse-0.dev5/se/templates/admin/crawl_status.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/admin/crawl_status_content.html` & `sosse-0.dev5/se/templates/admin/crawl_status_content.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/se/about.html` & `sosse-0.dev5/se/templates/se/about.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/se/base.html` & `sosse-0.dev5/se/templates/se/base.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/se/cached.html` & `sosse-0.dev5/se/templates/se/cached.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/se/history.html` & `sosse-0.dev5/se/templates/se/history.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/se/index.html` & `sosse-0.dev5/se/templates/se/index.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/se/main_menu.html` & `sosse-0.dev5/se/templates/se/main_menu.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/se/opensearch.xml` & `sosse-0.dev5/se/templates/se/opensearch.xml`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/se/pagination.html` & `sosse-0.dev5/se/templates/se/pagination.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/se/prefs.html` & `sosse-0.dev5/se/templates/se/prefs.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/se/screenshot.html` & `sosse-0.dev5/se/templates/se/screenshot.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/se/search_redirect.html` & `sosse-0.dev5/se/templates/se/search_redirect.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/se/stats.html` & `sosse-0.dev5/se/templates/se/stats.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/templates/se/unknown_url.html` & `sosse-0.dev5/se/templates/se/unknown_url.html`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/test_cookie.py` & `sosse-0.dev5/se/test_cookie.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/test_crawl.py` & `sosse-0.dev5/se/test_crawl.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/test_functionals.py` & `sosse-0.dev5/se/test_functionals.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/test_misc.py` & `sosse-0.dev5/se/test_misc.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/test_parser.py` & `sosse-0.dev5/se/test_parser.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/test_redirect.py` & `sosse-0.dev5/se/test_redirect.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/test_requests.py` & `sosse-0.dev5/se/test_requests.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/test_search.py` & `sosse-0.dev5/se/test_search.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/test_url.py` & `sosse-0.dev5/se/test_url.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/test_views.py` & `sosse-0.dev5/se/test_views.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/utils.py` & `sosse-0.dev5/se/utils.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/views.py` & `sosse-0.dev5/se/views.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/words.py` & `sosse-0.dev5/se/words.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/se/www.py` & `sosse-0.dev5/se/www.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/sosse/conf.py` & `sosse-0.dev5/sosse/conf.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/sosse/settings.py` & `sosse-0.dev5/sosse/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,9 +323,9 @@
         'name': 'chinese',
         'flag': '🇹🇼'
     }
 }
 
 globals().update(Conf.get())
 
-SOSSE_VERSION_TAG = '0.dev4'
+SOSSE_VERSION_TAG = '0.dev5'
 SOSSE_VERSION_COMMIT = ''
```

### Comparing `sosse-0.dev4/sosse/sosse_admin.py` & `sosse-0.dev5/sosse/sosse_admin.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/sosse/urls.py` & `sosse-0.dev5/sosse/urls.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/sosse/wsgi.py` & `sosse-0.dev5/sosse/wsgi.py`

 * *Files identical despite different names*

### Comparing `sosse-0.dev4/sosse.egg-info/PKG-INFO` & `sosse-0.dev5/sosse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosse
-Version: 0.dev4
+Version: 0.dev5
 Summary: Selenium Open Source Search Engine
 Author-email: Laurent Defert <laurent_defert@yahoo.fr>
 License: GNU Affero General Public License v3
 Keywords: search engine,crawler
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `sosse-0.dev4/sosse.egg-info/SOURCES.txt` & `sosse-0.dev5/sosse.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 se/templates/se/search_redirect.html
 se/templates/se/stats.html
 se/templates/se/unknown_url.html
 se/templates/se/words.html
 se/templates/se/www.html
 sosse/__init__.py
 sosse/conf.py
+sosse/search_engines.json
 sosse/settings.py
 sosse/sosse_admin.py
 sosse/urls.py
 sosse/wsgi.py
 sosse.egg-info/PKG-INFO
 sosse.egg-info/SOURCES.txt
 sosse.egg-info/dependency_links.txt
```

