# Comparing `tmp/django-marina-23.1.tar.gz` & `tmp/django-marina-23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-marina-23.1.tar", last modified: Fri Apr 14 10:26:51 2023, max compression
+gzip compressed data, was "django-marina-23.2.tar", last modified: Sat Apr 22 11:17:04 2023, max compression
```

## Comparing `django-marina-23.1.tar` & `django-marina-23.2.tar`

### file list

```diff
@@ -1,106 +1,48 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-14 10:26:51.054757 django-marina-23.1/
--rw-r--r--   0 dylan      (501) staff       (20)     1456 2019-04-27 05:10:10.000000 django-marina-23.1/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)      263 2021-04-09 08:41:59.000000 django-marina-23.1/MANIFEST.in
--rw-r--r--   0 dylan      (501) staff       (20)     1786 2023-04-14 10:26:51.054625 django-marina-23.1/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      666 2020-10-31 06:45:14.000000 django-marina-23.1/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-14 10:26:51.045351 django-marina-23.1/docs/
--rw-r--r--   0 dylan      (501) staff       (20)       30 2020-06-14 04:57:27.000000 django-marina-23.1/docs/changelog.rst
--rw-r--r--   0 dylan      (501) staff       (20)      878 2021-04-28 07:12:56.000000 django-marina-23.1/docs/conf.py
--rw-r--r--   0 dylan      (501) staff       (20)      217 2021-12-04 17:34:31.000000 django-marina-23.1/docs/db.rst
--rw-r--r--   0 dylan      (501) staff       (20)      152 2020-06-15 12:42:52.000000 django-marina-23.1/docs/index.rst
--rw-r--r--   0 dylan      (501) staff       (20)      104 2023-04-14 10:12:52.000000 django-marina-23.1/docs/requirements.txt
--rw-r--r--   0 dylan      (501) staff       (20)      220 2022-01-03 06:11:13.000000 django-marina-23.1/docs/test.rst
--rwxr-xr-x   0 dylan      (501) staff       (20)      252 2021-04-09 08:10:13.000000 django-marina-23.1/manage.py
--rw-r--r--   0 dylan      (501) staff       (20)     1148 2022-03-31 10:40:02.000000 django-marina-23.1/pyproject.toml
--rw-r--r--   0 dylan      (501) staff       (20)       38 2023-04-14 10:26:51.054789 django-marina-23.1/setup.cfg
--rw-r--r--   0 dylan      (501) staff       (20)     1689 2023-04-14 10:25:14.000000 django-marina-23.1/setup.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-14 10:26:51.043494 django-marina-23.1/src/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-14 10:26:51.045545 django-marina-23.1/src/django_marina/
--rw-r--r--   0 dylan      (501) staff       (20)      264 2020-11-02 05:49:45.000000 django-marina-23.1/src/django_marina/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-14 10:26:51.046616 django-marina-23.1/src/django_marina/db/
--rw-r--r--   0 dylan      (501) staff       (20)      138 2020-06-15 08:02:46.000000 django-marina-23.1/src/django_marina/db/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)      717 2020-06-15 12:42:52.000000 django-marina-23.1/src/django_marina/db/migrations.py
--rw-r--r--   0 dylan      (501) staff       (20)     1998 2021-05-31 06:50:39.000000 django-marina-23.1/src/django_marina/db/models.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-14 10:26:51.046991 django-marina-23.1/src/django_marina/test/
--rw-r--r--   0 dylan      (501) staff       (20)      127 2021-12-04 17:34:31.000000 django-marina-23.1/src/django_marina/test/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     1908 2021-07-01 04:27:53.000000 django-marina-23.1/src/django_marina/test/clients.py
--rw-r--r--   0 dylan      (501) staff       (20)     9273 2021-12-04 17:34:51.000000 django-marina-23.1/src/django_marina/test/test_cases.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-14 10:26:51.046285 django-marina-23.1/src/django_marina.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     1786 2023-04-14 10:26:51.000000 django-marina-23.1/src/django_marina.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     3435 2023-04-14 10:26:51.000000 django-marina-23.1/src/django_marina.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2023-04-14 10:26:51.000000 django-marina-23.1/src/django_marina.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2021-04-09 08:22:42.000000 django-marina-23.1/src/django_marina.egg-info/not-zip-safe
--rw-r--r--   0 dylan      (501) staff       (20)       82 2023-04-14 10:26:51.000000 django-marina-23.1/src/django_marina.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)       14 2023-04-14 10:26:51.000000 django-marina-23.1/src/django_marina.egg-info/top_level.txt
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-14 10:26:51.047824 django-marina-23.1/tests/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2020-06-11 08:49:17.000000 django-marina-23.1/tests/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-14 10:26:51.051801 django-marina-23.1/tests/__pycache__/
--rw-r--r--   0 dylan      (501) staff       (20)      146 2022-01-03 12:11:48.000000 django-marina-23.1/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      162 2023-04-14 06:45:30.000000 django-marina-23.1/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      140 2022-01-03 12:10:08.000000 django-marina-23.1/tests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      144 2022-01-03 12:10:29.000000 django-marina-23.1/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      144 2022-01-03 12:11:10.000000 django-marina-23.1/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      967 2022-01-03 12:11:48.000000 django-marina-23.1/tests/__pycache__/models.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1455 2023-04-14 06:45:30.000000 django-marina-23.1/tests/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      972 2022-01-03 12:10:08.000000 django-marina-23.1/tests/__pycache__/models.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      987 2022-01-03 12:10:29.000000 django-marina-23.1/tests/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      987 2022-01-03 12:11:10.000000 django-marina-23.1/tests/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2761 2022-01-03 12:11:48.000000 django-marina-23.1/tests/__pycache__/test_db.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     4776 2023-04-14 06:45:30.000000 django-marina-23.1/tests/__pycache__/test_db.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2783 2022-01-03 12:10:08.000000 django-marina-23.1/tests/__pycache__/test_db.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2769 2022-01-03 12:10:29.000000 django-marina-23.1/tests/__pycache__/test_db.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2809 2022-01-03 12:11:10.000000 django-marina-23.1/tests/__pycache__/test_db.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1196 2022-01-03 12:11:48.000000 django-marina-23.1/tests/__pycache__/test_extended_client.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1960 2023-04-14 06:45:30.000000 django-marina-23.1/tests/__pycache__/test_extended_client.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1184 2022-01-03 12:10:08.000000 django-marina-23.1/tests/__pycache__/test_extended_client.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1192 2022-01-03 12:10:29.000000 django-marina-23.1/tests/__pycache__/test_extended_client.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1192 2022-01-03 12:11:10.000000 django-marina-23.1/tests/__pycache__/test_extended_client.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     7702 2022-01-03 12:11:48.000000 django-marina-23.1/tests/__pycache__/test_extended_test_case.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)    20300 2023-04-14 06:45:30.000000 django-marina-23.1/tests/__pycache__/test_extended_test_case.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     7334 2022-01-03 12:10:09.000000 django-marina-23.1/tests/__pycache__/test_extended_test_case.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     7274 2022-01-03 12:10:30.000000 django-marina-23.1/tests/__pycache__/test_extended_test_case.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     7908 2022-01-03 12:11:10.000000 django-marina-23.1/tests/__pycache__/test_extended_test_case.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1332 2022-01-03 12:11:48.000000 django-marina-23.1/tests/__pycache__/test_imports.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1740 2023-04-14 06:45:30.000000 django-marina-23.1/tests/__pycache__/test_imports.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1386 2022-01-03 12:10:09.000000 django-marina-23.1/tests/__pycache__/test_imports.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1414 2022-01-03 12:10:30.000000 django-marina-23.1/tests/__pycache__/test_imports.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1414 2022-01-03 12:11:10.000000 django-marina-23.1/tests/__pycache__/test_imports.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      674 2022-01-03 12:11:48.000000 django-marina-23.1/tests/__pycache__/test_version.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      964 2023-04-14 06:45:30.000000 django-marina-23.1/tests/__pycache__/test_version.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      658 2022-01-03 12:10:09.000000 django-marina-23.1/tests/__pycache__/test_version.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      670 2022-01-03 12:10:30.000000 django-marina-23.1/tests/__pycache__/test_version.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      670 2022-01-03 12:11:10.000000 django-marina-23.1/tests/__pycache__/test_version.cpython-39.pyc
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-14 10:26:51.052248 django-marina-23.1/tests/app/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2020-06-13 09:16:54.000000 django-marina-23.1/tests/app/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-14 10:26:51.054458 django-marina-23.1/tests/app/__pycache__/
--rw-r--r--   0 dylan      (501) staff       (20)      150 2022-01-03 12:11:48.000000 django-marina-23.1/tests/app/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      166 2023-04-14 06:45:30.000000 django-marina-23.1/tests/app/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      144 2022-01-03 12:10:08.000000 django-marina-23.1/tests/app/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      148 2022-01-03 12:10:29.000000 django-marina-23.1/tests/app/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      148 2022-01-03 12:11:10.000000 django-marina-23.1/tests/app/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1308 2022-01-03 12:11:48.000000 django-marina-23.1/tests/app/__pycache__/settings.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1404 2023-04-14 06:45:30.000000 django-marina-23.1/tests/app/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1322 2022-01-03 12:10:08.000000 django-marina-23.1/tests/app/__pycache__/settings.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1334 2022-01-03 12:10:29.000000 django-marina-23.1/tests/app/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1306 2022-01-03 12:11:10.000000 django-marina-23.1/tests/app/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      686 2022-01-03 12:11:49.000000 django-marina-23.1/tests/app/__pycache__/urls.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1207 2023-04-14 06:45:31.000000 django-marina-23.1/tests/app/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      678 2022-01-03 12:10:09.000000 django-marina-23.1/tests/app/__pycache__/urls.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      684 2022-01-03 12:10:30.000000 django-marina-23.1/tests/app/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      684 2022-01-03 12:11:10.000000 django-marina-23.1/tests/app/__pycache__/urls.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3058 2022-01-03 12:11:49.000000 django-marina-23.1/tests/app/__pycache__/views.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     4537 2023-04-14 06:45:31.000000 django-marina-23.1/tests/app/__pycache__/views.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3207 2022-01-03 12:10:09.000000 django-marina-23.1/tests/app/__pycache__/views.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3166 2022-01-03 12:10:30.000000 django-marina-23.1/tests/app/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3166 2022-01-03 12:11:10.000000 django-marina-23.1/tests/app/__pycache__/views.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1525 2021-04-28 07:14:00.000000 django-marina-23.1/tests/app/settings.py
--rw-r--r--   0 dylan      (501) staff       (20)      616 2021-04-28 07:14:00.000000 django-marina-23.1/tests/app/urls.py
--rw-r--r--   0 dylan      (501) staff       (20)     1832 2021-04-28 07:14:00.000000 django-marina-23.1/tests/app/views.py
--rw-r--r--   0 dylan      (501) staff       (20)      617 2021-04-13 10:45:33.000000 django-marina-23.1/tests/models.py
--rw-r--r--   0 dylan      (501) staff       (20)     1995 2021-04-23 08:20:35.000000 django-marina-23.1/tests/test_db.py
--rw-r--r--   0 dylan      (501) staff       (20)      694 2020-07-20 04:35:29.000000 django-marina-23.1/tests/test_extended_client.py
--rw-r--r--   0 dylan      (501) staff       (20)     8518 2021-12-04 17:34:51.000000 django-marina-23.1/tests/test_extended_test_case.py
--rw-r--r--   0 dylan      (501) staff       (20)      547 2020-06-15 08:02:46.000000 django-marina-23.1/tests/test_imports.py
--rw-r--r--   0 dylan      (501) staff       (20)      303 2021-12-04 17:34:51.000000 django-marina-23.1/tests/test_version.py
--rw-r--r--   0 dylan      (501) staff       (20)      768 2019-06-10 07:50:32.000000 django-marina-23.1/tests/urls.py
--rw-r--r--   0 dylan      (501) staff       (20)     2323 2023-04-14 10:12:52.000000 django-marina-23.1/tox.ini
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.011949 django-marina-23.2/
+-rw-r--r--   0 dylan      (501) staff       (20)     1456 2019-04-27 05:10:10.000000 django-marina-23.2/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)      278 2023-04-22 11:05:50.000000 django-marina-23.2/MANIFEST.in
+-rw-r--r--   0 dylan      (501) staff       (20)     1786 2023-04-22 11:17:04.012023 django-marina-23.2/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      666 2020-10-31 06:45:14.000000 django-marina-23.2/README.md
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.007255 django-marina-23.2/docs/
+-rw-r--r--   0 dylan      (501) staff       (20)       30 2020-06-14 04:57:27.000000 django-marina-23.2/docs/changelog.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      905 2023-04-22 08:41:12.000000 django-marina-23.2/docs/conf.py
+-rw-r--r--   0 dylan      (501) staff       (20)      217 2021-12-04 17:34:31.000000 django-marina-23.2/docs/db.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      152 2020-06-15 12:42:52.000000 django-marina-23.2/docs/index.rst
+-rw-r--r--   0 dylan      (501) staff       (20)       62 2023-04-22 08:41:12.000000 django-marina-23.2/docs/requirements.txt
+-rw-r--r--   0 dylan      (501) staff       (20)      220 2022-01-03 06:11:13.000000 django-marina-23.2/docs/test.rst
+-rwxr-xr-x   0 dylan      (501) staff       (20)      252 2021-04-09 08:10:13.000000 django-marina-23.2/manage.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1148 2022-03-31 10:40:02.000000 django-marina-23.2/pyproject.toml
+-rw-r--r--   0 dylan      (501) staff       (20)     1217 2023-04-22 11:17:04.012278 django-marina-23.2/setup.cfg
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.004782 django-marina-23.2/src/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.007844 django-marina-23.2/src/django_marina/
+-rw-r--r--   0 dylan      (501) staff       (20)      264 2020-11-02 05:49:45.000000 django-marina-23.2/src/django_marina/__init__.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.009144 django-marina-23.2/src/django_marina/db/
+-rw-r--r--   0 dylan      (501) staff       (20)      138 2020-06-15 08:02:46.000000 django-marina-23.2/src/django_marina/db/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)      717 2020-06-15 12:42:52.000000 django-marina-23.2/src/django_marina/db/migrations.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1998 2021-05-31 06:50:39.000000 django-marina-23.2/src/django_marina/db/models.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.009490 django-marina-23.2/src/django_marina/test/
+-rw-r--r--   0 dylan      (501) staff       (20)      127 2021-12-04 17:34:31.000000 django-marina-23.2/src/django_marina/test/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1908 2021-07-01 04:27:53.000000 django-marina-23.2/src/django_marina/test/clients.py
+-rw-r--r--   0 dylan      (501) staff       (20)     9271 2023-04-22 08:41:12.000000 django-marina-23.2/src/django_marina/test/test_cases.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.008806 django-marina-23.2/src/django_marina.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)     1786 2023-04-22 11:17:03.000000 django-marina-23.2/src/django_marina.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      899 2023-04-22 11:17:04.000000 django-marina-23.2/src/django_marina.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2023-04-22 11:17:03.000000 django-marina-23.2/src/django_marina.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2021-04-09 08:22:42.000000 django-marina-23.2/src/django_marina.egg-info/not-zip-safe
+-rw-r--r--   0 dylan      (501) staff       (20)       80 2023-04-22 11:17:03.000000 django-marina-23.2/src/django_marina.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       14 2023-04-22 11:17:03.000000 django-marina-23.2/src/django_marina.egg-info/top_level.txt
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.011054 django-marina-23.2/tests/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2020-06-11 08:49:17.000000 django-marina-23.2/tests/__init__.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.011808 django-marina-23.2/tests/app/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2020-06-13 09:16:54.000000 django-marina-23.2/tests/app/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1525 2021-04-28 07:14:00.000000 django-marina-23.2/tests/app/settings.py
+-rw-r--r--   0 dylan      (501) staff       (20)      616 2021-04-28 07:14:00.000000 django-marina-23.2/tests/app/urls.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1832 2021-04-28 07:14:00.000000 django-marina-23.2/tests/app/views.py
+-rw-r--r--   0 dylan      (501) staff       (20)      617 2021-04-13 10:45:33.000000 django-marina-23.2/tests/models.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1995 2021-04-23 08:20:35.000000 django-marina-23.2/tests/test_db.py
+-rw-r--r--   0 dylan      (501) staff       (20)      694 2020-07-20 04:35:29.000000 django-marina-23.2/tests/test_extended_client.py
+-rw-r--r--   0 dylan      (501) staff       (20)     8518 2021-12-04 17:34:51.000000 django-marina-23.2/tests/test_extended_test_case.py
+-rw-r--r--   0 dylan      (501) staff       (20)      547 2020-06-15 08:02:46.000000 django-marina-23.2/tests/test_imports.py
+-rw-r--r--   0 dylan      (501) staff       (20)      303 2021-12-04 17:34:51.000000 django-marina-23.2/tests/test_version.py
+-rw-r--r--   0 dylan      (501) staff       (20)      768 2019-06-10 07:50:32.000000 django-marina-23.2/tests/urls.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2323 2023-04-14 10:12:52.000000 django-marina-23.2/tox.ini
```

### Comparing `django-marina-23.1/LICENSE` & `django-marina-23.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-marina-23.1/PKG-INFO` & `django-marina-23.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-marina
-Version: 23.1
+Version: 23.2
 Summary: Django extensions by Zostera
 Home-page: https://github.com/zostera/django-marina
 Author: Dylan Verheul
 Author-email: dylan@dyve.net
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-marina-23.1/README.md` & `django-marina-23.2/README.md`

 * *Files identical despite different names*

### Comparing `django-marina-23.1/docs/conf.py` & `django-marina-23.2/docs/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 copyright = f"2020, {author}"
 
 # The full version, including alpha/beta/rc tags, in x.y.z.misc format
 release = project_metadata["version"]
 # The short X.Y version.
 version = ".".join(release.split(".")[:2])
 
-extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode", "m2r2"]
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.viewcode",
+    "sphinx_mdinclude",
+]
 pygments_style = "sphinx"
 htmlhelp_basename = f"{PROJECT_NAME}-doc"
 
 if not on_rtd:  # only import and set the theme if we're building docs locally
     import sphinx_rtd_theme
 
     html_theme = "sphinx_rtd_theme"
```

### Comparing `django-marina-23.1/pyproject.toml` & `django-marina-23.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-marina-23.1/src/django_marina/db/migrations.py` & `django-marina-23.2/src/django_marina/db/migrations.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.1/src/django_marina/db/models.py` & `django-marina-23.2/src/django_marina/db/models.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.1/src/django_marina/test/clients.py` & `django-marina-23.2/src/django_marina/test/clients.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.1/src/django_marina/test/test_cases.py` & `django-marina-23.2/src/django_marina/test/test_cases.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,30 +137,28 @@
         :param response: Response object
         :param message: Full text of message to check for
         """
         self.assertIn(message, [m.message for m in get_messages(response.wsgi_request)])
 
     def _get_soup_num_results(self, response, soup_method, soup_args, soup_kwargs):
         """Get number of results in response for BeautifulSoup query."""
-
         # Extract string kwarg for selectors since soup does not implement it
         string = soup_kwargs.pop("string", None) if soup_method == "select" else None
 
         method = getattr(response.soup, soup_method)
         results = method(*soup_args, **soup_kwargs)
 
         # Search with string kwarg for selectors, by applying it to found tags
         if string is not None:
             results = [result for result in results if result.find(string=string)]
 
         return len(results)
 
     def _assert_soup(self, response, soup_method, soup_args, soup_kwargs, status_code, count, msg_prefix):
         """Handle assertions that use BeautifulSoup, with interface similar to assertContains and assertNotContains."""
-
         self.assertEqual(
             response.status_code,
             status_code,
             _msg_prefix_add(
                 msg_prefix,
                 f"Couldn't retrieve content: Response code was {response.status_code} (expected {status_code}).",
             ),
```

### Comparing `django-marina-23.1/src/django_marina.egg-info/PKG-INFO` & `django-marina-23.2/src/django_marina.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-marina
-Version: 23.1
+Version: 23.2
 Summary: Django extensions by Zostera
 Home-page: https://github.com/zostera/django-marina
 Author: Dylan Verheul
 Author-email: dylan@dyve.net
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-marina-23.1/tests/app/settings.py` & `django-marina-23.2/tests/app/settings.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.1/tests/app/urls.py` & `django-marina-23.2/tests/app/urls.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.1/tests/app/views.py` & `django-marina-23.2/tests/app/views.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.1/tests/models.py` & `django-marina-23.2/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.1/tests/test_db.py` & `django-marina-23.2/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.1/tests/test_extended_client.py` & `django-marina-23.2/tests/test_extended_client.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.1/tests/test_extended_test_case.py` & `django-marina-23.2/tests/test_extended_test_case.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.1/tests/test_imports.py` & `django-marina-23.2/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.1/tests/urls.py` & `django-marina-23.2/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.1/tox.ini` & `django-marina-23.2/tox.ini`

 * *Files identical despite different names*

