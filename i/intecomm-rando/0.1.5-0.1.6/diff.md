# Comparing `tmp/intecomm-rando-0.1.5.tar.gz` & `tmp/intecomm-rando-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intecomm-rando-0.1.5.tar", last modified: Fri Mar 31 00:48:50 2023, max compression
+gzip compressed data, was "intecomm-rando-0.1.6.tar", last modified: Sat Apr 22 18:11:51 2023, max compression
```

## Comparing `intecomm-rando-0.1.5.tar` & `intecomm-rando-0.1.6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 00:48:50.897046 intecomm-rando-0.1.5/
--rw-r--r--   0 erikvw     (501) staff       (20)       64 2022-11-18 01:20:32.000000 intecomm-rando-0.1.5/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-18 01:20:32.000000 intecomm-rando-0.1.5/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 00:48:50.887466 intecomm-rando-0.1.5/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 00:48:50.890932 intecomm-rando-0.1.5/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1645 2023-03-31 00:48:41.000000 intecomm-rando-0.1.5/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-11-20 14:10:06.000000 intecomm-rando-0.1.5/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-03-31 00:48:41.000000 intecomm-rando-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-18 01:20:32.000000 intecomm-rando-0.1.5/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)      243 2022-11-18 01:20:32.000000 intecomm-rando-0.1.5/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       29 2022-11-18 01:20:32.000000 intecomm-rando-0.1.5/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-18 00:53:59.000000 intecomm-rando-0.1.5/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-11-18 01:20:32.000000 intecomm-rando-0.1.5/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-03-31 00:48:50.897156 intecomm-rando-0.1.5/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      825 2022-11-18 01:20:32.000000 intecomm-rando-0.1.5/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-18 01:20:32.000000 intecomm-rando-0.1.5/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 00:48:50.892660 intecomm-rando-0.1.5/intecomm_rando/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:17:21.000000 intecomm-rando-0.1.5/intecomm_rando/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-11-18 01:20:32.000000 intecomm-rando-0.1.5/intecomm_rando/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)       72 2023-01-25 03:01:52.000000 intecomm-rando-0.1.5/intecomm_rando/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)      103 2022-11-23 01:14:40.000000 intecomm-rando-0.1.5/intecomm_rando/exceptions.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2749 2023-03-31 00:48:41.000000 intecomm-rando-0.1.5/intecomm_rando/group_eligibility.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1116 2022-11-20 02:31:32.000000 intecomm-rando-0.1.5/intecomm_rando/group_identifier.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 00:48:50.893888 intecomm-rando-0.1.5/intecomm_rando/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    24521 2023-03-31 00:48:41.000000 intecomm-rando-0.1.5/intecomm_rando/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3304 2023-03-31 00:48:41.000000 intecomm-rando-0.1.5/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:31:32.000000 intecomm-rando-0.1.5/intecomm_rando/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 00:48:50.894491 intecomm-rando-0.1.5/intecomm_rando/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      154 2023-01-23 15:17:57.000000 intecomm-rando-0.1.5/intecomm_rando/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      524 2023-03-31 00:48:41.000000 intecomm-rando-0.1.5/intecomm_rando/models/randomization_list.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1849 2023-03-31 00:48:41.000000 intecomm-rando-0.1.5/intecomm_rando/models/registered_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2269 2023-03-31 00:48:41.000000 intecomm-rando-0.1.5/intecomm_rando/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4942 2023-03-31 00:48:41.000000 intecomm-rando-0.1.5/intecomm_rando/randomize_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1320 2023-01-25 03:01:52.000000 intecomm-rando-0.1.5/intecomm_rando/randomizers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 00:48:50.894848 intecomm-rando-0.1.5/intecomm_rando/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:16:20.000000 intecomm-rando-0.1.5/intecomm_rando/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 00:48:50.896691 intecomm-rando-0.1.5/intecomm_rando/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      391 2023-01-25 03:01:52.000000 intecomm-rando-0.1.5/intecomm_rando/tests/etc/randomization_list.csv
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.5/intecomm_rando/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.5/intecomm_rando/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-20 14:10:06.000000 intecomm-rando-0.1.5/intecomm_rando/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.5/intecomm_rando/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-20 14:10:06.000000 intecomm-rando-0.1.5/intecomm_rando/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.5/intecomm_rando/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.5/intecomm_rando/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.5/intecomm_rando/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      303 2023-03-31 00:48:41.000000 intecomm-rando-0.1.5/intecomm_rando/tests/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      294 2022-11-20 02:31:32.000000 intecomm-rando-0.1.5/intecomm_rando/tests/sites.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 00:48:50.896936 intecomm-rando-0.1.5/intecomm_rando/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-23 01:14:40.000000 intecomm-rando-0.1.5/intecomm_rando/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    12424 2023-03-31 00:48:41.000000 intecomm-rando-0.1.5/intecomm_rando/tests/tests/test_rando_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-18 01:20:32.000000 intecomm-rando-0.1.5/intecomm_rando/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-03-31 00:48:50.893473 intecomm-rando-0.1.5/intecomm_rando.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-03-31 00:48:50.000000 intecomm-rando-0.1.5/intecomm_rando.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1605 2023-03-31 00:48:50.000000 intecomm-rando-0.1.5/intecomm_rando.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-03-31 00:48:50.000000 intecomm-rando-0.1.5/intecomm_rando.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-18 01:20:40.000000 intecomm-rando-0.1.5/intecomm_rando.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       15 2023-03-31 00:48:50.000000 intecomm-rando-0.1.5/intecomm_rando.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1753 2023-03-31 00:48:41.000000 intecomm-rando-0.1.5/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1711 2023-03-31 00:48:41.000000 intecomm-rando-0.1.5/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1159 2023-03-31 00:48:50.897526 intecomm-rando-0.1.5/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.311874 intecomm-rando-0.1.6/
+-rw-r--r--   0 erikvw     (501) staff       (20)       64 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.302187 intecomm-rando-0.1.6/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.305549 intecomm-rando-0.1.6/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1645 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-04-22 18:11:43.000000 intecomm-rando-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)      243 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       29 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-18 00:53:59.000000 intecomm-rando-0.1.6/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-04-22 18:11:51.311957 intecomm-rando-0.1.6/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      825 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.307379 intecomm-rando-0.1.6/intecomm_rando/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:17:21.000000 intecomm-rando-0.1.6/intecomm_rando/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/intecomm_rando/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       72 2023-01-25 03:01:52.000000 intecomm-rando-0.1.6/intecomm_rando/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      103 2022-11-23 01:14:40.000000 intecomm-rando-0.1.6/intecomm_rando/exceptions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2749 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/group_eligibility.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1116 2022-11-20 02:31:32.000000 intecomm-rando-0.1.6/intecomm_rando/group_identifier.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.308785 intecomm-rando-0.1.6/intecomm_rando/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    24521 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3304 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:31:32.000000 intecomm-rando-0.1.6/intecomm_rando/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.309440 intecomm-rando-0.1.6/intecomm_rando/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      154 2023-01-23 15:17:57.000000 intecomm-rando-0.1.6/intecomm_rando/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      524 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/models/randomization_list.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1849 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/models/registered_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2269 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4942 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/randomize_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1320 2023-01-25 03:01:52.000000 intecomm-rando-0.1.6/intecomm_rando/randomizers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.309829 intecomm-rando-0.1.6/intecomm_rando/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:16:20.000000 intecomm-rando-0.1.6/intecomm_rando/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.311505 intecomm-rando-0.1.6/intecomm_rando/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      391 2023-01-25 03:01:52.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/randomization_list.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      303 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/tests/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      294 2022-11-20 02:31:32.000000 intecomm-rando-0.1.6/intecomm_rando/tests/sites.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.311751 intecomm-rando-0.1.6/intecomm_rando/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-23 01:14:40.000000 intecomm-rando-0.1.6/intecomm_rando/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12293 2023-04-22 18:11:43.000000 intecomm-rando-0.1.6/intecomm_rando/tests/tests/test_rando_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/intecomm_rando/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.308306 intecomm-rando-0.1.6/intecomm_rando.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-04-22 18:11:51.000000 intecomm-rando-0.1.6/intecomm_rando.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1605 2023-04-22 18:11:51.000000 intecomm-rando-0.1.6/intecomm_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-04-22 18:11:51.000000 intecomm-rando-0.1.6/intecomm_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-18 01:20:40.000000 intecomm-rando-0.1.6/intecomm_rando.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       15 2023-04-22 18:11:51.000000 intecomm-rando-0.1.6/intecomm_rando.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1753 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1711 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1159 2023-04-22 18:11:51.312288 intecomm-rando-0.1.6/setup.cfg
```

### Comparing `intecomm-rando-0.1.5/.github/workflows/build.yml` & `intecomm-rando-0.1.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/.gitignore` & `intecomm-rando-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/.pre-commit-config.yaml` & `intecomm-rando-0.1.6/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ---
 exclude: tests/etc/user-*
 
 repos:
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3.10
 
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
@@ -37,13 +37,18 @@
       - id: fix-byte-order-marker
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
+  - repo: https://github.com/rstcheck/rstcheck
+    rev: v6.1.2
+    hooks:
+      - id: rstcheck
+
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.29.0
+    rev: v1.30.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `intecomm-rando-0.1.5/LICENSE` & `intecomm-rando-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/PKG-INFO` & `intecomm-rando-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-rando
-Version: 0.1.5
+Version: 0.1.6
 Summary: INTECOMM EDC randomization
 Home-page: https://github.com/intecomm-trial/intecomm-rando
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC randomization,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `intecomm-rando-0.1.5/README.rst` & `intecomm-rando-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/intecomm_rando/group_eligibility.py` & `intecomm-rando-0.1.6/intecomm_rando/group_eligibility.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/intecomm_rando/group_identifier.py` & `intecomm-rando-0.1.6/intecomm_rando/group_identifier.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/intecomm_rando/migrations/0001_initial.py` & `intecomm-rando-0.1.6/intecomm_rando/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py` & `intecomm-rando-0.1.6/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/intecomm_rando/models/randomization_list.py` & `intecomm-rando-0.1.6/intecomm_rando/models/randomization_list.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/intecomm_rando/models/registered_group.py` & `intecomm-rando-0.1.6/intecomm_rando/models/registered_group.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/intecomm_rando/models/signals.py` & `intecomm-rando-0.1.6/intecomm_rando/models/signals.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/intecomm_rando/randomize_group.py` & `intecomm-rando-0.1.6/intecomm_rando/randomize_group.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/intecomm_rando/randomizers.py` & `intecomm-rando-0.1.6/intecomm_rando/randomizers.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/intecomm_rando/tests/etc/user-rsa-local-private.pem` & `intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/intecomm_rando/tests/etc/user-rsa-restricted-private.pem` & `intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/intecomm_rando/tests/tests/test_rando_group.py` & `intecomm-rando-0.1.6/intecomm_rando/tests/tests/test_rando_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from uuid import uuid4
 
 from django.conf import settings
 from django.contrib.sites.models import Site
 from django.core.exceptions import ObjectDoesNotExist
-from django.test import override_settings, tag
+from django.test import override_settings
 from django_mock_queries.query import MockSet
 from edc_constants.constants import COMPLETE, NO, UUID_PATTERN, YES
 from edc_randomization.site_randomizers import site_randomizers
 from edc_registration.models import RegisteredSubject
 from edc_sites.add_or_update_django_sites import add_or_update_django_sites
 from intecomm_form_validators.tests.mock_models import PatientGroupMockModel
 from intecomm_form_validators.tests.test_case_mixin import TestCaseMixin
@@ -44,15 +44,14 @@
         site_randomizers.register(Randomizer)
 
     @classmethod
     def setUpTestData(cls):
         for country, sites in all_sites.items():
             add_or_update_django_sites(sites=sites, verbose=False)
 
-    @tag("1")
     @override_settings(SITE_ID=101)
     def test_ok(self):
         group_identifier_as_pk = str(uuid4())
         patients = self.get_mock_patients(
             dm=10,
             htn=0,
             hiv=4,
@@ -91,15 +90,14 @@
             self.fail("ObjectDoesNotExist unexpectedly raised (RegisteredGroup)")
 
         try:
             RandomizationList.objects.get(group_identifier=patient_group.group_identifier)
         except ObjectDoesNotExist:
             self.fail("ObjectDoesNotExist unexpectedly raised (RandomizationList)")
 
-    @tag("1")
     @override_settings(SITE_ID=101)
     def test_already_randomized(self):
         patients = self.get_mock_patients(
             dm=10,
             htn=0,
             hiv=4,
             stable=True,
@@ -117,15 +115,14 @@
             patients=MockSet(*patients),
             site=Site.objects.get(id=settings.SITE_ID),
         )
         randomizer = RandomizeGroup(patient_group)
         self.assertTrue(patient_group.randomized)
         self.assertRaises(GroupAlreadyRandomized, randomizer.randomize_group)
 
-    @tag("1")
     @override_settings(SITE_ID=101)
     def test_incomplete_group(self):
         patients = self.get_mock_patients(
             dm=10,
             htn=0,
             hiv=4,
             stable=True,
@@ -144,15 +141,14 @@
             patients=MockSet(*patients),
             site=Site.objects.get(id=settings.SITE_ID),
         )
         randomizer = RandomizeGroup(patient_group)
         self.assertRaises(GroupRandomizationError, randomizer.randomize_group)
         self.assertFalse(patient_group.randomized)
 
-    @tag("1")
     @override_settings(SITE_ID=101)
     def test_complete_group_but_not_enough_members(self):
         patients = self.get_mock_patients(
             dm=3,
             htn=0,
             hiv=4,
             stable=True,
@@ -173,15 +169,14 @@
         )
         randomizer = RandomizeGroup(patient_group)
         with self.assertRaises(GroupRandomizationError) as cm:
             randomizer.randomize_group()
         self.assertIn("Patient group must have at least", str(cm.exception))
         self.assertFalse(patient_group.randomized)
 
-    @tag("1")
     @override_settings(SITE_ID=101)
     def test_complete_group_enough_members_not_screened(self):
         patients = self.get_mock_patients(
             dm=4,
             htn=4,
             hiv=4,
             stable=True,
@@ -202,15 +197,14 @@
         )
         randomizer = RandomizeGroup(patient_group)
         with self.assertRaises(GroupRandomizationError) as cm:
             randomizer.randomize_group()
         self.assertIn("Patient has not screened", str(cm.exception))
         self.assertFalse(patient_group.randomized)
 
-    @tag("1")
     @override_settings(SITE_ID=101)
     def test_complete_group_enough_members_not_consented(self):
         patients = self.get_mock_patients(
             dm=4,
             htn=4,
             hiv=4,
             stable=True,
@@ -231,15 +225,14 @@
         )
         randomizer = RandomizeGroup(patient_group)
         with self.assertRaises(GroupRandomizationError) as cm:
             randomizer.randomize_group()
         self.assertIn("Patient has not consented", str(cm.exception))
         self.assertFalse(patient_group.randomized)
 
-    @tag("1")
     @override_settings(SITE_ID=101)
     def test_complete_group_enough_members_all_consented(self):
         group_identifier_as_pk = str(uuid4())
         patients = self.get_mock_patients(
             dm=5,
             htn=5,
             hiv=4,
@@ -264,15 +257,14 @@
         randomizer = RandomizeGroup(patient_group)
         try:
             randomizer.randomize_group()
         except GroupRandomizationError as e:
             self.fail(f"GroupRandomizationError unexpectedly raised. Got {e}")
         self.assertTrue(patient_group.randomized)
 
-    @tag("1")
     @override_settings(SITE_ID=101)
     def test_complete_group_but_randomize_now_is_no(self):
         group_identifier_as_pk = str(uuid4())
         patients = self.get_mock_patients(
             dm=5,
             htn=5,
             hiv=4,
@@ -297,15 +289,14 @@
         randomize_group = RandomizeGroup(patient_group)
         try:
             randomize_group.randomize_group()
         except GroupRandomizationError:
             self.fail("GroupRandomizationError unexpectedly raised.")
         self.assertTrue(patient_group.randomized)
 
-    @tag("1")
     @override_settings(SITE_ID=101)
     def test_complete_group_enough_members_all_consented_func(self):
         group_identifier_as_pk = str(uuid4())
         patients = self.get_mock_patients(
             dm=5,
             htn=5,
             hiv=4,
```

### Comparing `intecomm-rando-0.1.5/intecomm_rando.egg-info/PKG-INFO` & `intecomm-rando-0.1.6/intecomm_rando.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-rando
-Version: 0.1.5
+Version: 0.1.6
 Summary: INTECOMM EDC randomization
 Home-page: https://github.com/intecomm-trial/intecomm-rando
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC randomization,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `intecomm-rando-0.1.5/intecomm_rando.egg-info/SOURCES.txt` & `intecomm-rando-0.1.6/intecomm_rando.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/pyproject.toml` & `intecomm-rando-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/runtests.py` & `intecomm-rando-0.1.6/runtests.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.5/setup.cfg` & `intecomm-rando-0.1.6/setup.cfg`

 * *Files identical despite different names*

