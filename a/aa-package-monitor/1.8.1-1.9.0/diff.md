# Comparing `tmp/aa-package-monitor-1.8.1.tar.gz` & `tmp/aa_package_monitor-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-package-monitor-1.8.1.tar", last modified: Wed Jan  4 20:51:22 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aa-package-monitor-1.8.1.tar` & `aa_package_monitor-1.9.0.tar`

### file list

```diff
@@ -1,60 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 20:51:22.371293 aa-package-monitor-1.8.1/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2020-10-24 19:41:16.000000 aa-package-monitor-1.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      204 2021-07-20 18:35:59.000000 aa-package-monitor-1.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9835 2023-01-04 20:51:22.371293 aa-package-monitor-1.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8873 2022-09-15 18:48:32.000000 aa-package-monitor-1.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 20:51:22.363293 aa-package-monitor-1.8.1/aa_package_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9835 2023-01-04 20:51:22.000000 aa-package-monitor-1.8.1/aa_package_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1581 2023-01-04 20:51:22.000000 aa-package-monitor-1.8.1/aa_package_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-04 20:51:22.000000 aa-package-monitor-1.8.1/aa_package_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-01-04 20:51:22.000000 aa-package-monitor-1.8.1/aa_package_monitor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-01-04 20:51:22.000000 aa-package-monitor-1.8.1/aa_package_monitor.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 20:51:22.367293 aa-package-monitor-1.8.1/package_monitor/
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-01-04 19:18:13.000000 aa-package-monitor-1.8.1/package_monitor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1102 2022-09-12 17:45:36.000000 aa-package-monitor-1.8.1/package_monitor/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2021-07-20 18:35:59.000000 aa-package-monitor-1.8.1/package_monitor/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2022-08-30 16:33:16.000000 aa-package-monitor-1.8.1/package_monitor/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     9431 2023-01-04 19:18:13.000000 aa-package-monitor-1.8.1/package_monitor/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 20:51:22.359293 aa-package-monitor-1.8.1/package_monitor/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 20:51:22.367293 aa-package-monitor-1.8.1/package_monitor/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)     1149 2022-08-30 16:33:16.000000 aa-package-monitor-1.8.1/package_monitor/management/commands/package_monitor_refresh.py
--rw-rw-rw-   0 root         (0) root         (0)     6031 2022-09-15 18:48:32.000000 aa-package-monitor-1.8.1/package_monitor/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 20:51:22.367293 aa-package-monitor-1.8.1/package_monitor/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     3861 2020-10-24 19:41:16.000000 aa-package-monitor-1.8.1/package_monitor/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1694 2022-08-30 18:08:53.000000 aa-package-monitor-1.8.1/package_monitor/migrations/0002_add_editable_and_refactor_json_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      857 2022-09-12 17:45:36.000000 aa-package-monitor-1.8.1/package_monitor/migrations/0003_add_update_notifications.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-24 19:41:16.000000 aa-package-monitor-1.8.1/package_monitor/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2640 2022-09-12 17:45:36.000000 aa-package-monitor-1.8.1/package_monitor/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 20:51:22.359293 aa-package-monitor-1.8.1/package_monitor/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 20:51:22.363293 aa-package-monitor-1.8.1/package_monitor/static/package_monitor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 20:51:22.367293 aa-package-monitor-1.8.1/package_monitor/static/package_monitor/css/
--rw-rw-rw-   0 root         (0) root         (0)     1302 2020-11-05 15:15:38.000000 aa-package-monitor-1.8.1/package_monitor/static/package_monitor/css/global.css
--rw-rw-rw-   0 root         (0) root         (0)      392 2020-11-05 15:15:38.000000 aa-package-monitor-1.8.1/package_monitor/static/package_monitor/css/package_list.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 20:51:22.367293 aa-package-monitor-1.8.1/package_monitor/static/package_monitor/images/
--rw-rw-rw-   0 root         (0) root         (0)    43262 2020-11-05 15:15:38.000000 aa-package-monitor-1.8.1/package_monitor/static/package_monitor/images/Spinner-1s-64px-dark.gif
--rw-rw-rw-   0 root         (0) root         (0)    43381 2020-11-05 15:15:38.000000 aa-package-monitor-1.8.1/package_monitor/static/package_monitor/images/Spinner-1s-64px-light.gif
--rw-rw-rw-   0 root         (0) root         (0)      358 2021-07-20 18:35:59.000000 aa-package-monitor-1.8.1/package_monitor/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 20:51:22.363293 aa-package-monitor-1.8.1/package_monitor/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 20:51:22.367293 aa-package-monitor-1.8.1/package_monitor/templates/package_monitor/
--rw-rw-rw-   0 root         (0) root         (0)      285 2020-11-05 15:15:38.000000 aa-package-monitor-1.8.1/package_monitor/templates/package_monitor/base.html
--rw-rw-rw-   0 root         (0) root         (0)     8704 2022-08-02 12:15:31.000000 aa-package-monitor-1.8.1/package_monitor/templates/package_monitor/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 20:51:22.371293 aa-package-monitor-1.8.1/package_monitor/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-24 19:41:16.000000 aa-package-monitor-1.8.1/package_monitor/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5848 2022-09-12 17:45:36.000000 aa-package-monitor-1.8.1/package_monitor/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2021-07-20 18:35:59.000000 aa-package-monitor-1.8.1/package_monitor/tests/test_commands.py
--rw-rw-rw-   0 root         (0) root         (0)    13381 2023-01-04 20:01:19.000000 aa-package-monitor-1.8.1/package_monitor/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2022-09-12 17:45:36.000000 aa-package-monitor-1.8.1/package_monitor/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)    18043 2022-09-12 20:58:48.000000 aa-package-monitor-1.8.1/package_monitor/tests/test_managers.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2022-09-12 17:45:36.000000 aa-package-monitor-1.8.1/package_monitor/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)      359 2022-08-30 16:33:16.000000 aa-package-monitor-1.8.1/package_monitor/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3975 2022-09-12 17:45:36.000000 aa-package-monitor-1.8.1/package_monitor/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2021-07-20 18:35:59.000000 aa-package-monitor-1.8.1/package_monitor/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     4881 2022-09-12 17:45:36.000000 aa-package-monitor-1.8.1/package_monitor/views.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-04 20:51:22.371293 aa-package-monitor-1.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1683 2023-01-03 14:03:30.000000 aa-package-monitor-1.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 20:51:22.371293 aa-package-monitor-1.8.1/testauth/
--rw-rw-rw-   0 root         (0) root         (0)       46 2020-10-24 19:41:16.000000 aa-package-monitor-1.8.1/testauth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2021-07-20 18:35:59.000000 aa-package-monitor-1.8.1/testauth/celery.py
--rw-rw-rw-   0 root         (0) root         (0)     9863 2021-10-30 13:11:21.000000 aa-package-monitor-1.8.1/testauth/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2021-07-20 18:35:59.000000 aa-package-monitor-1.8.1/testauth/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2020-10-24 19:41:16.000000 aa-package-monitor-1.8.1/testauth/wsgi.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/app_settings.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/apps.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/auth_hooks.py
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/core.py
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/managers.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/models.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tasks.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/urls.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/views.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/django.pot
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/management/commands/package_monitor_refresh.py
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/migrations/0002_add_editable_and_refactor_json_fields.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/migrations/0003_add_update_notifications.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/migrations/__init__.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/static/package_monitor/css/global.css
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/static/package_monitor/css/package_list.css
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/static/package_monitor/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/static/package_monitor/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/templates/package_monitor/base.html
+-rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/templates/package_monitor/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/__init__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/test_commands.py
+-rw-r--r--   0        0        0    15922 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/test_core.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/test_integration.py
+-rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/test_managers.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/test_models.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/test_tasks.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/test_views.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/factories/__init__.py
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/factories/factories.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/factories/stubs.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/factories/tests.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/LICENSE
+-rw-r--r--   0        0        0     8873 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/README.md
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10220 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/PKG-INFO
```

### Comparing `aa-package-monitor-1.8.1/LICENSE` & `aa_package_monitor-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-package-monitor-1.8.1/PKG-INFO` & `aa_package_monitor-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: aa-package-monitor
-Version: 1.8.1
+Version: 1.9.0
 Summary: An app that helps keep track of installed packages and outstanding updates for Alliance Auth
-Home-page: https://gitlab.com/ErikKalkoken/aa-package-monitor
-Author: Erik Kalkoken
-Author-email: kalkoken87@gmail.com
-License: MIT
-Platform: UNKNOWN
+Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-package-monitor
+Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-package-monitor
+Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-package-monitor/-/blob/master/CHANGELOG.md
+Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-package-monitor/-/issues
+Author-email: Erik Kalkoken <kalkoken87@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.8
+Requires-Python: >=3.8
+Requires-Dist: allianceauth-app-utils>=1.8
+Requires-Dist: allianceauth>=3
+Requires-Dist: importlib-metadata
+Requires-Dist: requests
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Package Monitor
 
 An app for keeping track of installed packages and outstanding updates with Alliance Auth.
 
 [![release](https://img.shields.io/pypi/v/aa-package-monitor?label=release)](https://pypi.org/project/aa-package-monitor/)
 [![python](https://img.shields.io/pypi/pyversions/aa-package-monitor)](https://pypi.org/project/aa-package-monitor/)
@@ -199,9 +204,7 @@
 ## Management Commands
 
 The following management commands are included in this app:
 
 Command | Description
 -- | --
 `package_monitor_refresh`| Refreshes all data about distribution packages. This command does functionally the same as the hourly update and is helpful to use after you have completed updating outdated packages to quickly see the result of your actions on the website.
-
-
```

### Comparing `aa-package-monitor-1.8.1/README.md` & `aa_package_monitor-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aa-package-monitor-1.8.1/package_monitor/app_settings.py` & `aa_package_monitor-1.9.0/package_monitor/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa-package-monitor-1.8.1/package_monitor/auth_hooks.py` & `aa_package_monitor-1.9.0/package_monitor/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-package-monitor-1.8.1/package_monitor/core.py` & `aa_package_monitor-1.9.0/package_monitor/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import concurrent.futures
+import json
 import os
 import sys
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional
 
 import importlib_metadata
 import requests
@@ -62,39 +63,58 @@
         for a specific distribution package and are thus storing
         all needed information about that package in our new object.
         Should additional information be needed sometimes it should be fetched here too.
         """
         obj = cls(
             name=dist.name,
             current=dist.version,
-            is_editable=cls._calc_is_editable(dist.name),
+            is_editable=_is_distribution_editable(dist),
             requirements=_parse_requirements(dist.requires),
-            homepage_url=dist_metadata_value(dist, "Home-page"),
             summary=dist_metadata_value(dist, "Summary"),
         )
         dist_files = [
             "/" + str(f) for f in dist.files if str(f).endswith("__init__.py")
         ]
         if not disable_app_check:
             for dist_file in dist_files:
                 for app in django_apps.get_app_configs():
                     my_file = app.module.__file__
                     if my_file.endswith(dist_file):
                         obj.apps.append(app.name)
                         break
         return obj
 
-    @staticmethod
-    def _calc_is_editable(dist_name: str) -> bool:
-        """Is distribution an editable install?"""
-        for path_item in sys.path:
-            egg_link = os.path.join(path_item, dist_name + ".egg-link")
-            if os.path.isfile(egg_link):
-                return True
-        return False
+
+# def _determine_homepage_url(dist: importlib_metadata.Distribution) -> str:
+#     if url := dist_metadata_value(dist, "Home-page"):
+#         return url
+#     values = dist.metadata.get_all("Project-URL")
+#     while values:
+#         k, v = [o.strip() for o in values.pop(0).split(",")]
+#         if k.lower() == "homepage":
+#             return v
+#     return ""
+
+
+def _is_distribution_editable(dist: importlib_metadata.Distribution) -> bool:
+    """Determine if a distribution is an editable install?"""
+    # method for new packages conforming with pep 660
+    direct_url_json = dist.read_text("direct_url.json")
+    if direct_url_json:
+        direct_url = json.loads(direct_url_json)
+        if "dir_info" in direct_url and direct_url["dir_info"].get("editable") is True:
+            return True
+
+    # method for old packages
+    for path_item in sys.path:
+        egg_link = os.path.join(path_item, dist.name + ".egg-link")
+        if os.path.isfile(egg_link):
+            return True
+
+    return False
 
 
 def gather_distribution_packages() -> Dict[str, DistributionPackage]:
     """Gather distribution packages and detect Django apps."""
     packages = [
         DistributionPackage.create_from_distribution(dist)
         for dist in importlib_metadata.distributions()
@@ -150,103 +170,117 @@
     def thread_update_latest_from_pypi(package_name: str) -> None:
         """Retrieves latest valid version from PyPI and updates packages
 
         Note: This inner function can run as thread
         """
         nonlocal packages
 
-        current_python_version = version_parse(
-            f"{sys.version_info.major}.{sys.version_info.minor}"
-            f".{sys.version_info.micro}"
+        consolidated_requirements = _calc_consolidated_requirements(
+            package_name, requirements
+        )
+        latest, pypi_url = _fetch_data_from_pypi(
+            packages[package_name], consolidated_requirements
         )
+        packages[package_name].latest = latest
+        packages[package_name].homepage_url = pypi_url
+
+    def _calc_consolidated_requirements(package_name, requirements):
         consolidated_requirements = SpecifierSet()
         if package_name in requirements:
             for _, specifier in requirements[package_name].items():
                 consolidated_requirements &= specifier
+        return consolidated_requirements
 
-        package = packages[package_name]
+    def _fetch_data_from_pypi(package, consolidated_requirements):
+        """Fetch data for a package from PyPI."""
+        current_python_version = version_parse(
+            f"{sys.version_info.major}.{sys.version_info.minor}"
+            f".{sys.version_info.micro}"
+        )
         current_version = version_parse(package.current)
         current_is_prerelease = (
             str(current_version) == str(package.current)
             and current_version.is_prerelease
         )
         logger.info(
-            f"Fetching info for distribution package '{package.name}' " "from PyPI"
+            f"Fetching info for distribution package '{package.name}' from PyPI"
         )
+
         r = requests.get(f"https://pypi.org/pypi/{package.name}/json", timeout=(5, 30))
-        if r.status_code == requests.codes.ok:
-            pypi_info = r.json()
-            latest = ""
-            for release, release_details in pypi_info["releases"].items():
-                try:
-                    release_detail = (
-                        release_details[-1] if len(release_details) > 0 else None
-                    )
-                    if release_detail:
-                        if release_detail["yanked"]:
-                            continue
-                        if (
-                            requires_python := release_detail.get("requires_python")
-                        ) and current_python_version not in SpecifierSet(
-                            requires_python
-                        ):
-                            continue
-
-                    my_release = version_parse(release)
-                    if str(my_release) == str(release) and (
-                        current_is_prerelease or not my_release.is_prerelease
-                    ):
-                        if len(consolidated_requirements) > 0:
-                            is_valid = my_release in consolidated_requirements
-                        else:
-                            is_valid = True
-
-                        if is_valid and (
-                            not latest or my_release > version_parse(latest)
-                        ):
-                            latest = release
-                except InvalidVersion:
-                    logger.warning(
-                        "%s: Ignoring release with invalid version: %s",
-                        package.name,
-                        release,
-                    )
-                except InvalidSpecifier:
-                    logger.warning(
-                        "%s: Ignoring release with invalid requires_python: %s",
-                        package.name,
-                        requires_python,
-                    )
-            if not latest:
-                logger.warning(
-                    f"Could not find a release of '{package.name}' "
-                    f"that matches all requirements: '{consolidated_requirements}''"
-                )
-        else:
+        if r.status_code != requests.codes.ok:
             if r.status_code == 404:
                 logger.info(f"Package '{package.name}' is not registered in PyPI")
             else:
                 logger.warning(
                     "Failed to retrieve infos from PyPI for "
                     f"package '{package.name}'. "
                     f"Status code: {r.status_code}, "
                     f"response: {r.content}"
                 )
-            latest = ""
+            return "", ""
 
-        packages[package_name].latest = latest
+        pypi_data = r.json()
+        latest = ""
+        pypi_info = pypi_data.get("info")
+        pypi_url = pypi_info.get("project_url", "") if pypi_info else ""
+        for release, release_details in pypi_data["releases"].items():
+            try:
+                release_detail = (
+                    release_details[-1] if len(release_details) > 0 else None
+                )
+                if release_detail:
+                    if release_detail["yanked"]:
+                        continue
+                    if (
+                        requires_python := release_detail.get("requires_python")
+                    ) and current_python_version not in SpecifierSet(requires_python):
+                        continue
+
+                my_release = version_parse(release)
+                if str(my_release) == str(release) and (
+                    current_is_prerelease or not my_release.is_prerelease
+                ):
+                    if len(consolidated_requirements) > 0:
+                        is_valid = my_release in consolidated_requirements
+                    else:
+                        is_valid = True
+
+                    if is_valid and (not latest or my_release > version_parse(latest)):
+                        latest = release
+            except InvalidVersion:
+                logger.warning(
+                    "%s: Ignoring release with invalid version: %s",
+                    package.name,
+                    release,
+                )
+            except InvalidSpecifier:
+                logger.warning(
+                    "%s: Ignoring release with invalid requires_python: %s",
+                    package.name,
+                    requires_python,
+                )
+        if not latest:
+            logger.warning(
+                f"Could not find a release of '{package.name}' "
+                f"that matches all requirements: '{consolidated_requirements}''"
+            )
+        return latest, pypi_url
 
     if use_threads:
         with concurrent.futures.ThreadPoolExecutor(
             max_workers=MAX_THREAD_WORKERS
         ) as executor:
             executor.map(thread_update_latest_from_pypi, packages.keys())
     else:
         for package_name in packages.keys():
             thread_update_latest_from_pypi(package_name)
 
 
 def dist_metadata_value(dist: importlib_metadata.Distribution, prop: str) -> str:
-    """Metadata value from distribution or empty string."""
-    if dist and dist.metadata[prop] and dist.metadata[prop] != "UNKNOWN":
-        return dist.metadata[prop]
+    """Metadata value from distribution or empty string.
+
+    Note: metadata can contain multiple values for the same key.
+    This method will return the first only!
+    """
+    if dist and (value := dist.metadata.get(prop)) and value != "UNKNOWN":
+        return value
     return ""
```

### Comparing `aa-package-monitor-1.8.1/package_monitor/management/commands/package_monitor_refresh.py` & `aa_package_monitor-1.9.0/package_monitor/management/commands/package_monitor_refresh.py`

 * *Files identical despite different names*

### Comparing `aa-package-monitor-1.8.1/package_monitor/managers.py` & `aa_package_monitor-1.9.0/package_monitor/managers.py`

 * *Files identical despite different names*

### Comparing `aa-package-monitor-1.8.1/package_monitor/migrations/0001_initial.py` & `aa_package_monitor-1.9.0/package_monitor/migrations/0001_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2.16 on 2020-09-16 18:39
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="General",
```

### Comparing `aa-package-monitor-1.8.1/package_monitor/migrations/0002_add_editable_and_refactor_json_fields.py` & `aa_package_monitor-1.9.0/package_monitor/migrations/0002_add_editable_and_refactor_json_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.0.7 on 2022-08-30 16:47
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("package_monitor", "0001_initial"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="distribution",
```

### Comparing `aa-package-monitor-1.8.1/package_monitor/migrations/0003_add_update_notifications.py` & `aa_package_monitor-1.9.0/package_monitor/migrations/0003_add_update_notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.0.7 on 2022-09-12 15:03
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("package_monitor", "0002_add_editable_and_refactor_json_fields"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="distribution",
```

### Comparing `aa-package-monitor-1.8.1/package_monitor/models.py` & `aa_package_monitor-1.9.0/package_monitor/models.py`

 * *Files identical despite different names*

### Comparing `aa-package-monitor-1.8.1/package_monitor/static/package_monitor/css/global.css` & `aa_package_monitor-1.9.0/package_monitor/static/package_monitor/css/global.css`

 * *Files identical despite different names*

### Comparing `aa-package-monitor-1.8.1/package_monitor/static/package_monitor/images/Spinner-1s-64px-dark.gif` & `aa_package_monitor-1.9.0/package_monitor/static/package_monitor/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa-package-monitor-1.8.1/package_monitor/static/package_monitor/images/Spinner-1s-64px-light.gif` & `aa_package_monitor-1.9.0/package_monitor/static/package_monitor/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa-package-monitor-1.8.1/package_monitor/tests/test_commands.py` & `aa_package_monitor-1.9.0/package_monitor/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa-package-monitor-1.8.1/package_monitor/tests/test_core.py` & `aa_package_monitor-1.9.0/package_monitor/tests/test_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import requests_mock
 from packaging.specifiers import SpecifierSet
 
 from app_utils.testing import NoSocketsTestCase
 
 from package_monitor.core import (
     DistributionPackage,
+    _is_distribution_editable,
     compile_package_requirements,
     dist_metadata_value,
     gather_distribution_packages,
     update_packages_from_pypi,
 )
 
 from .factories import (
@@ -48,15 +49,15 @@
         # then
         self.assertEqual(obj.name, "Alpha")
         self.assertEqual(obj.name_normalized, "alpha")
         self.assertEqual(obj.current, "1.2.3")
         self.assertEqual(obj.latest, "")
         self.assertListEqual([str(x) for x in obj.requirements], ["bravo>=1.0.0"])
         self.assertEqual(obj.apps, ["alpha_app"])
-        self.assertEqual(obj.homepage_url, "https://www.alpha.com")
+        self.assertEqual(obj.homepage_url, "")
 
     def test_should_not_be_outdated(self):
         # given
         obj = DistributionPackageFactory(current="1.0.0", latest="1.0.0")
         # when/then
         self.assertFalse(obj.is_outdated())
 
@@ -68,27 +69,100 @@
 
     def test_should_return_none_as_outdated(self):
         # given
         obj = DistributionPackageFactory(current="1.0.0", latest=None)
         # when/then
         self.assertIsNone(obj.is_outdated())
 
-    def test_should_not_be_editable(self):
+
+@mock.patch(MODULE_PATH + ".os.path.isfile")
+class TestIsDistributionEditable(NoSocketsTestCase):
+    def test_should_not_be_editable(self, mock_isfile):
         # given
-        obj = DistributionPackageFactory(name="alpha")
+        mock_isfile.return_value = False
+        obj = ImportlibDistributionStubFactory(name="alpha")
         # when/then
-        self.assertFalse(obj._calc_is_editable("alpha"))
+        self.assertFalse(_is_distribution_editable(obj))
 
-    @mock.patch(MODULE_PATH + ".os.path.isfile")
-    def test_should_be_editable(self, mock_isfile):
+    def test_should_be_editable_old_version(self, mock_isfile):
         # given
         mock_isfile.return_value = True
-        obj = DistributionPackageFactory(name="alpha")
+        obj = ImportlibDistributionStubFactory(name="alpha")
+        # when/then
+        self.assertTrue(_is_distribution_editable(obj))
+
+    def test_should_be_editable_pep660(self, mock_isfile):
+        # given
+        mock_isfile.return_value = False
+
+        obj = ImportlibDistributionStubFactory(name="alpha")
+        obj._files_content = {
+            "direct_url.json": '{"dir_info": {"editable": true}, "url": "xxx"}'
+        }
+        # when/then
+        self.assertTrue(_is_distribution_editable(obj))
+
+    def test_should_not_be_editable_pep660(self, mock_isfile):
+        # given
+        mock_isfile.return_value = False
+
+        obj = ImportlibDistributionStubFactory(name="alpha")
+        obj._files_content = {
+            "direct_url.json": '{"dir_info": {"editable": false}, "url": "xxx"}'
+        }
         # when/then
-        self.assertTrue(obj._calc_is_editable("alpha"))
+        self.assertFalse(_is_distribution_editable(obj))
+
+
+# class TestDetermineHomePageUrl(NoSocketsTestCase):
+#     def test_should_identify_homepage_old_style(self):
+#         # given
+#         dist = ImportlibDistributionStubFactory(homepage_url="my-homepage-url")
+#         # when
+#         url = _determine_homepage_url(dist)
+#         # then
+#         self.assertEqual(url, "my-homepage-url")
+
+#     def test_should_identify_homepage_pep_621_style(self):
+#         # given
+#         dist = ImportlibDistributionStubFactory(homepage_url="")
+#         for v in [
+#             "Documentation, other-url",
+#             "Homepage, my-homepage-url",
+#             "Issues, other-url",
+#         ]:
+#             dist.metadata["Project-URL"] = v
+#         # when
+#         url = _determine_homepage_url(dist)
+#         # then
+#         self.assertEqual(url, "my-homepage-url")
+
+#     def test_should_identify_homepage_pep_621_style_other_case(self):
+#         # given
+#         dist = ImportlibDistributionStubFactory(homepage_url="")
+#         for v in [
+#             "Documentation, other-url",
+#             "homepage, my-homepage-url",
+#             "Issues, other-url",
+#         ]:
+#             dist.metadata["Project-URL"] = v
+#         # when
+#         url = _determine_homepage_url(dist)
+#         # then
+#         self.assertEqual(url, "my-homepage-url")
+
+#     def test_should_return_empty_string_when_no_url_found_with_pep_621(self):
+#         # given
+#         dist = ImportlibDistributionStubFactory(homepage_url="")
+#         for v in ["Documentation, other-url", "Issues, other-url"]:
+#             dist.metadata["Project-URL"] = v
+#         # when
+#         url = _determine_homepage_url(dist)
+#         # then
+#         self.assertEqual(url, "")
 
 
 @mock.patch(MODULE_PATH + ".importlib_metadata.distributions", spec=True)
 class TestFetchRelevantPackages(NoSocketsTestCase):
     def test_should_fetch_all_packages(self, mock_distributions):
         # given
         dist_alpha = ImportlibDistributionStubFactory(name="alpha")
@@ -170,14 +244,17 @@
         )
         # when
         update_packages_from_pypi(
             packages=packages, requirements=requirements, use_threads=False
         )
         # then
         self.assertEqual(packages["alpha"].latest, "1.1.0")
+        self.assertEqual(
+            packages["alpha"].homepage_url, "https://pypi.org/project/alpha/"
+        )
 
     def test_should_ignore_prereleases_when_stable(self, requests_mocker):
         # given
         dist_alpha = DistributionPackageFactory(name="alpha", current="1.0.0")
         packages = make_packages(dist_alpha)
         requirements = {}
         pypi_alpha = PypiFactory(distribution=dist_alpha)
@@ -280,19 +357,15 @@
         # when
         update_packages_from_pypi(
             packages=packages, requirements=requirements, use_threads=False
         )
         # then
         self.assertEqual(packages["alpha"].latest, "1.0.0")
 
-    """
-    This test breaks with packaging<22, which is currently required by Auth.
-    Die App is build to work with packaging>=22.0 though and this test should
-    be enabled once the Auth patch for updating this requirement is released.
-    """
+    # TODO: This test breaks with packaging<22, which is currently required by Auth.
 
     # def test_should_ignore_invalid_python_release_spec(self, requests_mocker):
     #     # given
     #     dist_alpha = DistributionPackageFactory(name="alpha", current="1.0.0")
     #     packages = make_packages(dist_alpha)
     #     requirements = {}
     #     pypi_alpha = PypiFactory(distribution=dist_alpha)
@@ -311,20 +384,19 @@
 class TestDistMetadataValue(NoSocketsTestCase):
     def test_should_return_value_when_exists(self):
         # given
         dist = ImportlibDistributionStubFactory(name="Alpha")
         # when/then
         self.assertEqual(dist_metadata_value(dist, "Name"), "Alpha")
 
-    def test_should_raise_error_when_prop_does_not_exist(self):
+    def test_should_return_empty_string_when_prop_does_not_exist(self):
         # given
         dist = ImportlibDistributionStubFactory(name="Alpha")
         # when/then
-        with self.assertRaises(KeyError):
-            dist_metadata_value(dist, "XXX")
+        self.assertEqual(dist_metadata_value(dist, "XXX"), "")
 
     def test_should_return_name(self):
         # given
         dist = ImportlibDistributionStubFactory(name="Alpha")
         # when/then
         self.assertEqual(dist_metadata_value(dist, "Name"), "Alpha")
```

### Comparing `aa-package-monitor-1.8.1/package_monitor/tests/test_integration.py` & `aa_package_monitor-1.9.0/package_monitor/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa-package-monitor-1.8.1/package_monitor/tests/test_managers.py` & `aa_package_monitor-1.9.0/package_monitor/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `aa-package-monitor-1.8.1/package_monitor/tests/test_models.py` & `aa_package_monitor-1.9.0/package_monitor/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa-package-monitor-1.8.1/package_monitor/tests/test_views.py` & `aa_package_monitor-1.9.0/package_monitor/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa-package-monitor-1.8.1/package_monitor/views.py` & `aa_package_monitor-1.9.0/package_monitor/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.contrib.auth.decorators import login_required, permission_required
 from django.http import HttpResponse, JsonResponse
 from django.shortcuts import render
 from django.utils.html import format_html
+from django.utils.translation import gettext_lazy as _
 
-from app_utils.views import link_html, no_wrap_html, yesno_str
+from app_utils.views import link_html, yesno_str
 
 from . import __title__
 from .app_settings import (
     PACKAGE_MONITOR_INCLUDE_PACKAGES,
     PACKAGE_MONITOR_SHOW_ALL_PACKAGES,
 )
 from .models import Distribution
@@ -29,15 +30,15 @@
         Distribution.objects.filter_visible()
         .filter(is_outdated=True)
         .order_by("name")
         .build_install_command()
     )
     context = {
         "app_title": __title__,
-        "page_title": "Distribution packages",
+        "page_title": _("Distribution packages"),
         "updated_at": updated_at,
         "filter": filter,
         "all_count": distributions_qs.count(),
         "current_count": distributions_qs.filter(is_outdated=False).count(),
         "outdated_count": distributions_qs.outdated_count(),
         "unknown_count": distributions_qs.filter(is_outdated__isnull=True).count(),
         "include_packages": PACKAGE_MONITOR_INCLUDE_PACKAGES,
@@ -60,22 +61,26 @@
     elif my_filter == "current":
         distributions_qs = distributions_qs.filter(is_outdated=False)
     elif my_filter == "unknown":
         distributions_qs = distributions_qs.filter(is_outdated__isnull=True)
 
     data = list()
     for dist in distributions_qs.order_by("name"):
+        dist: Distribution
         name_link_html = (
             link_html(dist.website_url, dist.name) if dist.website_url else dist.name
         )
         if dist.is_outdated:
-            name_link_html += '&nbsp;<i class="fas fa-exclamation-circle" title="Update available"></i>'
+            name_link_html += (
+                '&nbsp;<i class="fas fa-exclamation-circle" '
+                f'title="{_("Update available")}"></i>'
+            )
 
         if dist.apps:
-            _lst = [no_wrap_html(row) for row in dist.apps]
+            _lst = [row for row in dist.apps]
             apps_html = "<br>".join(_lst) if _lst else "-"
         else:
             apps_html = ""
 
         if dist.used_by:
             used_by_sorted = sorted(dist.used_by, key=lambda k: k["name"])
             used_by_html = "<br>".join(
@@ -95,33 +100,36 @@
         else:
             used_by_html = ""
 
         if not dist.latest_version:
             latest_html = "?"
         else:
             command = f"pip install {dist.pip_install_version}"
-            latest_html = no_wrap_html(
+            latest_html = (
                 f'<span class="copy_to_clipboard" '
                 f'title="{command}"'
                 f' data-clipboard-text="{command}">'
                 f"{dist.latest_version}"
                 '&nbsp;&nbsp;<i class="far fa-copy"></i></span>'
             )
 
+        description = dist.description
+        if dist.is_editable:
+            description += f" [{_('EDITABLE')}]"
         data.append(
             {
                 "name": dist.name,
-                "name_link": no_wrap_html(name_link_html),
+                "name_link": name_link_html,
                 "apps": apps_html,
                 "used_by": used_by_html,
                 "current": dist.installed_version,
                 "latest": latest_html,
                 "is_outdated": dist.is_outdated,
                 "is_outdated_str": yesno_str(dist.is_outdated),
-                "description": dist.description,
+                "description": description,
             }
         )
 
     return JsonResponse(data, safe=False)
 
 
 @login_required
```

