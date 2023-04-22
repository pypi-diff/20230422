# Comparing `tmp/yerbamate-0.9.21.tar.gz` & `tmp/yerbamate-0.9.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yerbamate-0.9.21.tar", last modified: Mon Feb 13 21:23:10 2023, max compression
+gzip compressed data, was "yerbamate-0.9.22.tar", last modified: Sat Apr 22 15:21:21 2023, max compression
```

## Comparing `yerbamate-0.9.21.tar` & `yerbamate-0.9.22.tar`

### file list

```diff
@@ -1,104 +1,88 @@
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.109751 yerbamate-0.9.21/
--rw-r--r--   0 al        (1000) al        (1000)     1079 2023-02-09 13:54:17.000000 yerbamate-0.9.21/LICENSE
--rw-r--r--   0 al        (1000) al        (1000)       29 2022-09-29 23:08:07.000000 yerbamate-0.9.21/MANIFEST.in
--rw-r--r--   0 al        (1000) al        (1000)     7580 2023-02-13 21:23:10.109751 yerbamate-0.9.21/PKG-INFO
--rw-r--r--   0 al        (1000) al        (1000)     6948 2023-02-13 21:22:00.000000 yerbamate-0.9.21/README.md
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.104751 yerbamate-0.9.21/packages/
--rw-r--r--   0 al        (1000) al        (1000)      114 2023-02-09 14:07:17.000000 yerbamate-0.9.21/packages/requirements.txt
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.104751 yerbamate-0.9.21/packages/yerbamate/
--rw-r--r--   0 al        (1000) al        (1000)      130 2023-02-09 15:48:38.000000 yerbamate-0.9.21/packages/yerbamate/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.105751 yerbamate-0.9.21/packages/yerbamate/__pycache__/
--rw-r--r--   0 al        (1000) al        (1000)      291 2023-02-09 15:49:09.000000 yerbamate-0.9.21/packages/yerbamate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)      404 2023-02-06 16:05:23.000000 yerbamate-0.9.21/packages/yerbamate/__pycache__/backbone_type.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     4417 2023-02-10 22:30:34.000000 yerbamate-0.9.21/packages/yerbamate/__pycache__/environment.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     8361 2023-02-13 21:08:58.000000 yerbamate-0.9.21/packages/yerbamate/__pycache__/mate.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     9435 2023-02-13 21:12:22.000000 yerbamate-0.9.21/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     2779 2023-02-09 12:11:00.000000 yerbamate-0.9.21/packages/yerbamate/__pycache__/mate_config.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     3307 2022-09-29 22:16:27.000000 yerbamate-0.9.21/packages/yerbamate/__pycache__/package.cpython-310.pyc
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.105751 yerbamate-0.9.21/packages/yerbamate/api/
--rw-r--r--   0 al        (1000) al        (1000)        0 2023-02-06 14:44:16.000000 yerbamate-0.9.21/packages/yerbamate/api/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.105751 yerbamate-0.9.21/packages/yerbamate/api/__pycache__/
--rw-r--r--   0 al        (1000) al        (1000)      153 2023-02-06 16:05:23.000000 yerbamate-0.9.21/packages/yerbamate/api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     1514 2023-02-10 22:30:34.000000 yerbamate-0.9.21/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     3316 2022-10-03 15:07:51.000000 yerbamate-0.9.21/packages/yerbamate/api/__pycache__/package.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     1263 2022-10-06 18:00:29.000000 yerbamate-0.9.21/packages/yerbamate/api/__pycache__/package_manager.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     1251 2022-10-07 14:32:28.000000 yerbamate-0.9.21/packages/yerbamate/api/__pycache__/package_repository.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     2834 2022-10-14 20:05:41.000000 yerbamate-0.9.21/packages/yerbamate/api/__pycache__/socket.cpython-310.pyc
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.106751 yerbamate-0.9.21/packages/yerbamate/api/data/
--rw-r--r--   0 al        (1000) al        (1000)       29 2023-02-06 14:44:16.000000 yerbamate-0.9.21/packages/yerbamate/api/data/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.106751 yerbamate-0.9.21/packages/yerbamate/api/data/__pycache__/
--rw-r--r--   0 al        (1000) al        (1000)      197 2023-02-06 16:05:23.000000 yerbamate-0.9.21/packages/yerbamate/api/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     5727 2023-02-12 17:40:02.000000 yerbamate-0.9.21/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)    10886 2023-02-13 20:36:23.000000 yerbamate-0.9.21/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     3316 2023-02-06 16:05:23.000000 yerbamate-0.9.21/packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     3811 2023-02-06 23:26:43.000000 yerbamate-0.9.21/packages/yerbamate/api/data/__pycache__/package_manager.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     6102 2023-02-07 09:47:46.000000 yerbamate-0.9.21/packages/yerbamate/api/data/__pycache__/package_repository.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     9516 2023-02-12 17:39:59.000000 yerbamate-0.9.21/packages/yerbamate/api/data/module_manager.py
--rw-r--r--   0 al        (1000) al        (1000)    12872 2023-02-13 20:36:20.000000 yerbamate-0.9.21/packages/yerbamate/api/data/module_repository.py
--rw-r--r--   0 al        (1000) al        (1000)     3447 2023-02-06 14:44:16.000000 yerbamate-0.9.21/packages/yerbamate/api/data/package.py
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.106751 yerbamate-0.9.21/packages/yerbamate/api/data/sources/
--rw-r--r--   0 al        (1000) al        (1000)        0 2023-02-06 14:44:16.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.106751 yerbamate-0.9.21/packages/yerbamate/api/data/sources/__pycache__/
--rw-r--r--   0 al        (1000) al        (1000)      166 2023-02-06 16:05:23.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     4097 2022-10-05 22:12:32.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/__pycache__/local.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     2125 2022-10-04 13:59:03.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/__pycache__/remote.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     1127 2023-02-06 16:05:23.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.106751 yerbamate-0.9.21/packages/yerbamate/api/data/sources/local/
--rw-r--r--   0 al        (1000) al        (1000)       35 2023-02-06 14:44:16.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/local/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.107751 yerbamate-0.9.21/packages/yerbamate/api/data/sources/local/__pycache__/
--rw-r--r--   0 al        (1000) al        (1000)      217 2023-02-06 16:05:23.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/local/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     5270 2023-02-10 22:30:34.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     5810 2023-02-13 20:59:51.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     2719 2023-02-06 16:05:24.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/local/__pycache__/server.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     5486 2023-02-10 22:21:54.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/local/io.py
--rw-r--r--   0 al        (1000) al        (1000)     5184 2023-02-13 20:59:45.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/local/local.py
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.107751 yerbamate-0.9.21/packages/yerbamate/api/data/sources/remote/
--rw-r--r--   0 al        (1000) al        (1000)       37 2023-02-06 14:44:16.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/remote/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.107751 yerbamate-0.9.21/packages/yerbamate/api/data/sources/remote/__pycache__/
--rw-r--r--   0 al        (1000) al        (1000)      220 2023-02-06 16:05:24.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/remote/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     2132 2023-02-06 16:05:24.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     1078 2023-02-06 14:44:16.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/remote/remote.py
--rw-r--r--   0 al        (1000) al        (1000)      365 2023-02-06 14:44:16.000000 yerbamate-0.9.21/packages/yerbamate/api/data/sources/source.py
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.107751 yerbamate-0.9.21/packages/yerbamate/api/data/utils/
--rw-r--r--   0 al        (1000) al        (1000)        0 2023-02-06 12:35:53.000000 yerbamate-0.9.21/packages/yerbamate/api/data/utils/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.108751 yerbamate-0.9.21/packages/yerbamate/api/data/utils/__pycache__/
--rw-r--r--   0 al        (1000) al        (1000)      164 2023-02-06 13:42:03.000000 yerbamate-0.9.21/packages/yerbamate/api/data/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)      540 2023-02-06 19:52:57.000000 yerbamate-0.9.21/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     1035 2023-02-06 23:30:35.000000 yerbamate-0.9.21/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     4487 2023-02-12 12:12:39.000000 yerbamate-0.9.21/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)      326 2023-02-06 19:48:30.000000 yerbamate-0.9.21/packages/yerbamate/api/data/utils/exp_util.py
--rw-r--r--   0 al        (1000) al        (1000)     1197 2023-02-06 23:30:31.000000 yerbamate-0.9.21/packages/yerbamate/api/data/utils/git_util.py
--rw-r--r--   0 al        (1000) al        (1000)     7395 2023-02-12 12:12:33.000000 yerbamate-0.9.21/packages/yerbamate/api/data/utils/gitdir.py
--rw-r--r--   0 al        (1000) al        (1000)      923 2023-02-10 22:28:52.000000 yerbamate-0.9.21/packages/yerbamate/api/mate_api.py
--rw-r--r--   0 al        (1000) al        (1000)      294 2022-09-29 23:08:07.000000 yerbamate-0.9.21/packages/yerbamate/constants.py
--rw-r--r--   0 al        (1000) al        (1000)     5843 2023-02-10 22:20:55.000000 yerbamate-0.9.21/packages/yerbamate/environment.py
--rw-r--r--   0 al        (1000) al        (1000)     7892 2023-02-13 21:08:56.000000 yerbamate-0.9.21/packages/yerbamate/mate.py
--rw-r--r--   0 al        (1000) al        (1000)    10647 2023-02-13 21:11:01.000000 yerbamate-0.9.21/packages/yerbamate/mate_cli.py
--rw-r--r--   0 al        (1000) al        (1000)     2193 2023-02-09 12:01:35.000000 yerbamate-0.9.21/packages/yerbamate/mate_config.py
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.108751 yerbamate-0.9.21/packages/yerbamate/utils/
--rw-r--r--   0 al        (1000) al        (1000)     1433 2023-02-07 19:44:00.000000 yerbamate-0.9.21/packages/yerbamate/utils/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.108751 yerbamate-0.9.21/packages/yerbamate/utils/__pycache__/
--rw-r--r--   0 al        (1000) al        (1000)     2016 2023-02-07 19:46:03.000000 yerbamate-0.9.21/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     2389 2023-02-06 16:05:23.000000 yerbamate-0.9.21/packages/yerbamate/utils/__pycache__/bunch.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     1557 2022-10-04 13:59:03.000000 yerbamate-0.9.21/packages/yerbamate/utils/__pycache__/git_url_parser.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     3503 2022-09-29 22:16:27.000000 yerbamate-0.9.21/packages/yerbamate/utils/__pycache__/migrator.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     3761 2023-02-06 16:05:23.000000 yerbamate-0.9.21/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1000)     1751 2022-09-29 23:08:07.000000 yerbamate-0.9.21/packages/yerbamate/utils/bunch.py
--rw-r--r--   0 al        (1000) al        (1000)     1386 2022-09-29 23:08:07.000000 yerbamate-0.9.21/packages/yerbamate/utils/git_url_parser.py
--rw-r--r--   0 al        (1000) al        (1000)     4419 2022-09-29 23:08:07.000000 yerbamate-0.9.21/packages/yerbamate/utils/utils.py
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.108751 yerbamate-0.9.21/packages/yerbamate/yerbamate.egg-info/
--rw-r--r--   0 al        (1000) al        (1000)      601 2022-09-29 23:08:07.000000 yerbamate-0.9.21/packages/yerbamate/yerbamate.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) al        (1000)      342 2022-09-29 23:08:07.000000 yerbamate-0.9.21/packages/yerbamate/yerbamate.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) al        (1000)        1 2022-09-29 23:08:07.000000 yerbamate-0.9.21/packages/yerbamate/yerbamate.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) al        (1000)       10 2022-09-29 23:08:07.000000 yerbamate-0.9.21/packages/yerbamate/yerbamate.egg-info/top_level.txt
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.104751 yerbamate-0.9.21/packages/yerbamate.egg-info/
--rw-r--r--   0 al        (1000) al        (1000)     7580 2023-02-13 21:23:09.000000 yerbamate-0.9.21/packages/yerbamate.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) al        (1000)     4169 2023-02-13 21:23:10.000000 yerbamate-0.9.21/packages/yerbamate.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) al        (1000)        1 2023-02-13 21:23:09.000000 yerbamate-0.9.21/packages/yerbamate.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) al        (1000)       73 2023-02-13 21:23:09.000000 yerbamate-0.9.21/packages/yerbamate.egg-info/requires.txt
--rw-r--r--   0 al        (1000) al        (1000)       10 2023-02-13 21:23:09.000000 yerbamate-0.9.21/packages/yerbamate.egg-info/top_level.txt
--rw-r--r--   0 al        (1000) al        (1000)      107 2023-02-13 21:23:10.109751 yerbamate-0.9.21/setup.cfg
--rw-r--r--   0 al        (1000) al        (1000)     1259 2023-02-13 21:23:05.000000 yerbamate-0.9.21/setup.py
-drwxr-xr-x   0 al        (1000) al        (1000)        0 2023-02-13 21:23:10.103751 yerbamate-0.9.21/src/
--rwxr-xr-x   0 al        (1000) al        (1000)      105 2022-09-09 15:58:06.000000 yerbamate-0.9.21/src/mate
--rw-r--r--   0 al        (1000) al        (1000)      115 2023-02-06 12:35:53.000000 yerbamate-0.9.21/src/mateboard
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.553157 yerbamate-0.9.22/
+-rw-r--r--   0 al        (1000) al        (1001)     1079 2023-04-08 19:56:23.000000 yerbamate-0.9.22/LICENSE
+-rw-r--r--   0 al        (1000) al        (1001)       29 2023-04-08 19:56:23.000000 yerbamate-0.9.22/MANIFEST.in
+-rw-r--r--   0 al        (1000) al        (1001)    11581 2023-04-22 15:21:21.553157 yerbamate-0.9.22/PKG-INFO
+-rw-r--r--   0 al        (1000) al        (1001)    10948 2023-04-08 19:56:23.000000 yerbamate-0.9.22/README.md
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.544158 yerbamate-0.9.22/packages/
+-rw-r--r--   0 al        (1000) al        (1001)      112 2023-04-22 15:20:01.000000 yerbamate-0.9.22/packages/requirements.txt
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.544158 yerbamate-0.9.22/packages/yerbamate/
+-rw-r--r--   0 al        (1000) al        (1001)      130 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.545158 yerbamate-0.9.22/packages/yerbamate/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      291 2023-04-08 19:57:52.000000 yerbamate-0.9.22/packages/yerbamate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     4429 2023-04-09 09:45:27.000000 yerbamate-0.9.22/packages/yerbamate/__pycache__/environment.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     8269 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/__pycache__/mate.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     9389 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.546158 yerbamate-0.9.22/packages/yerbamate/api/
+-rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.546158 yerbamate-0.9.22/packages/yerbamate/api/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      153 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1427 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.546158 yerbamate-0.9.22/packages/yerbamate/api/data/
+-rw-r--r--   0 al        (1000) al        (1001)       29 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.548158 yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      197 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5655 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)    11315 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     3316 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     9460 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/module_manager.py
+-rw-r--r--   0 al        (1000) al        (1001)    14686 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/module_repository.py
+-rw-r--r--   0 al        (1000) al        (1001)     3447 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/package.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.548158 yerbamate-0.9.22/packages/yerbamate/api/data/sources/
+-rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.548158 yerbamate-0.9.22/packages/yerbamate/api/data/sources/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      166 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1127 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.548158 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/
+-rw-r--r--   0 al        (1000) al        (1001)       35 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.549158 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      217 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5521 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5734 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5573 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/io.py
+-rw-r--r--   0 al        (1000) al        (1001)     5130 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/local.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.550158 yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/
+-rw-r--r--   0 al        (1000) al        (1001)       37 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.550158 yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      220 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     2132 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1078 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/remote.py
+-rw-r--r--   0 al        (1000) al        (1001)      365 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/source.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.550158 yerbamate-0.9.22/packages/yerbamate/api/data/utils/
+-rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.551158 yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      164 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      540 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1035 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     4487 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      326 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/exp_util.py
+-rw-r--r--   0 al        (1000) al        (1001)     1197 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/git_util.py
+-rw-r--r--   0 al        (1000) al        (1001)     7395 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/gitdir.py
+-rw-r--r--   0 al        (1000) al        (1001)      869 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/mate_api.py
+-rw-r--r--   0 al        (1000) al        (1001)      294 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/constants.py
+-rw-r--r--   0 al        (1000) al        (1001)     5800 2023-04-09 09:45:16.000000 yerbamate-0.9.22/packages/yerbamate/environment.py
+-rw-r--r--   0 al        (1000) al        (1001)     7829 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/mate.py
+-rw-r--r--   0 al        (1000) al        (1001)    10611 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/mate_cli.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.551158 yerbamate-0.9.22/packages/yerbamate/utils/
+-rw-r--r--   0 al        (1000) al        (1001)     1433 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/utils/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.552157 yerbamate-0.9.22/packages/yerbamate/utils/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)     2016 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      814 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/utils/__pycache__/bunch.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     3761 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     2145 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/utils/bunch.py
+-rw-r--r--   0 al        (1000) al        (1001)     1386 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/utils/git_url_parser.py
+-rw-r--r--   0 al        (1000) al        (1001)     4419 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/utils/utils.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.553157 yerbamate-0.9.22/packages/yerbamate/yerbamate.egg-info/
+-rw-r--r--   0 al        (1000) al        (1001)      601 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/yerbamate.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) al        (1001)      342 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/yerbamate.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) al        (1001)        1 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/yerbamate.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) al        (1001)       10 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/yerbamate.egg-info/top_level.txt
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.545158 yerbamate-0.9.22/packages/yerbamate.egg-info/
+-rw-r--r--   0 al        (1000) al        (1001)    11581 2023-04-22 15:21:21.000000 yerbamate-0.9.22/packages/yerbamate.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) al        (1001)     3195 2023-04-22 15:21:21.000000 yerbamate-0.9.22/packages/yerbamate.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) al        (1001)        1 2023-04-22 15:21:21.000000 yerbamate-0.9.22/packages/yerbamate.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) al        (1001)       82 2023-04-22 15:21:21.000000 yerbamate-0.9.22/packages/yerbamate.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) al        (1001)       10 2023-04-22 15:21:21.000000 yerbamate-0.9.22/packages/yerbamate.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) al        (1001)      107 2023-04-22 15:21:21.553157 yerbamate-0.9.22/setup.cfg
+-rw-r--r--   0 al        (1000) al        (1001)     1278 2023-04-22 15:20:20.000000 yerbamate-0.9.22/setup.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.544158 yerbamate-0.9.22/src/
+-rwxr-xr-x   0 al        (1000) al        (1001)       62 2023-04-08 19:56:23.000000 yerbamate-0.9.22/src/mate
```

### Comparing `yerbamate-0.9.21/LICENSE` & `yerbamate-0.9.22/LICENSE`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.21/PKG-INFO` & `yerbamate-0.9.22/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yerbamate
-Version: 0.9.21
+Version: 0.9.22
 Summary:  A python module and experiment manager for deep learning
 Home-page: https://github.com/oalee/yerbamate
 Author: Giulio Zani, Ali Rahimi
 Author-email: yerba.mate.dl@proton.me
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -12,44 +12,51 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1 style="color:green"><span style="color:green">Maté 🧉</span> your friendly AI project and experiment manager</h1>
+<h1 style="color:green"><span style="color:green">Maté 🧉</span> your modular AI project and experiment manager</h1>
 
-Maté is a python project, package and experiment manager. Whether you are a
+<!-- Maté is a python project, package and experiment manager. Whether you are a
 seasoned deep learning researcher or just starting out, Maté provides you with
 the tools to easily add source code and dependencies of models, trainers, and
 data loaders to your projects. With Maté, you can also evaluate, train, and keep
-track of your experiments with ease 🚀
+track of your experiments with ease 🚀 -->
+### Welcome to [Maté](https://github.com/oalee/yerbamate)! 🎉👋🏼
 
-## Features 🎉
+Maté is an open science modular Python framework designed to streamline and simplify the development and management of machine learning projects. It was developed to address the reproducibility crisis in artificial intelligence research by promoting open science and accessible AI. 🌍💻
+
+The framework is built around the best software engineering practices of modularity and separation of concerns, encouraging quality coding, collaboration, and the sharing of models, trainers, data loaders, and knowledge. The modular design and separation of concerns simplify the development and maintenance of machine learning models, leading to an improved developer experience. 🚀💻👨‍💻💬🧠
+
+With Maté, you can easily install the source code of open-source projects and adhere to modularity and separation of concerns, making your models and modules sharable out of the box. This means you can collaborate more effectively with others and easily share your work. 📦💻🤝
 
-- Seamless integration with any installed python library such as PyTorch/Lightning,
-  TensorFlow/Keras, JAX/Flax, Huggingface/transformers.
-- Easy to use interface to add source code of models, trainers, and data loaders
-  to your projects.
-- Support for full customizability and reproducibility of results through the
-  inclusion of dependencies in your project.
-- Modular project structure that enforces a clean and organized codebase.
-- Fully compatible with python. 
-- Convenient environment management through the Maté Environment API.
-- Support for pip and conda for dependency management.
-- Works with Colab.
+Thank you for choosing Maté, and we can't wait to see the amazing machine learning projects you'll create with it! 🎉👨‍💻🌟
+
+## Features 🎉
+- Seamless integration with any python library such as PyTorch/Lightning, TensorFlow/Keras, JAX/Flax, Huggingface/transformers. 🤝🤗🐉
+- Easy to use interface to add source code of models, trainers, and data loaders to your projects. 🎨💻📝
+- Support for full customizability and reproducibility of results through the inclusion of dependencies in your project. 🌟🔍🧪
+- Modular project structure that enforces a clean and organized codebase. 🧱👨‍💻👌
+- Fully compatible with python. No need to use mate commands to run your experiments. 🐍💻🚀
+- Convenient environment management through the Maté Environment API. 🌍👨‍💻🔧
+- Support for pip and conda for dependency management. 📦🔍💻
+- Works with [Colab](https://github.com/oalee/yerbamate/blob/main/deep_learning.ipynb) out of the box.  🎉👌🤖
 
 ## Table of Contents
 
-- [Installation](#installation-🔌)
-- [Quick Start](#quick-start-⚡)
-- [Project Structure](#project-structure-📁)
-- [Example Projects](#example-projects-📚)
-- [Documentation](https://oalee.github.io/yerbamate/)
-- [Contribution](#Contribution-🤝)
+- [Installation](#installation-)
+- [Quick Start](#quick-start-)
+- [Project Structure](#project-structure-)
+- [Example Projects](#example-projects-)
+- [Documentation](#documentation-)
+- [Contribution](#Contribution-)
+- [Guides](#guides-)
+- [Open Science](#open-science-)
 
 ## Installation 🔌
 
 ```bash
 pip install yerbamate
 ```
 
@@ -75,15 +82,15 @@
 |   |-- __init__.py
 ```
 
 ### **Install an experiment**
 
 To install an experiment, you can use `mate install` to install a module and its
 dependencies from a github repository. See
-[docs](https://oalee.github.io/yerbamate/#/?id=install) for more details.
+[docs](https://oalee.github.io/yerbamate/#/?id=mate-install) for more details.
 
 ```bash
 # Short version of GitHub URL https://github.com/oalee/big_transfer/tree/master/big_transfer/experiments/bit
 mate install oalee/big_transfer/experiments/bit -yo pip
 
 # Short version of GitHub URL https://github.com/oalee/deep-vision/tree/main/deepnet/experiments/resnet
 mate install oalee/deep-vision/deepnet/experiments/resnet -yo pip
@@ -100,17 +107,25 @@
 mate install oalee/big_transfer/models/bit -yo pip
 mate install oalee/deep-vision/deepnet/models/vit_pytorch -yo pip
 mate install oalee/deep-vision/deepnet/trainers/classification -yo pip
 ```
 
 ### **Setting up environment**
 
-Take a look at
-[Environment API](https://oalee.github.io/yerbamate#maté-environment-api) and
-set up your environment before running your experiments.
+Set up your environment before running your experiments. This can be done by using shell, or `env.json` file in the root of your project. Maté API requires `results` to be set in the environment. For more information, see [docs](https://oalee.github.io/yerbamate/#/?id=mat%c3%a9-environment-api).
+```bash
+DATA_PATH=/path/to/data
+results=/path/to/results
+```
+```json
+{
+    "DATA_PATH": "/path/to/data",
+    "results": "/path/to/results"
+}
+```
 
 ### **Train a model**
 
 To train a model, you can use the `mate train` command. This command will train
 the model with the specified experiment. For example, to train the an experiment
 called `learn` in the `bit` module, you can use the following command:
 
@@ -121,37 +136,51 @@
 ```
 
 ## Project Structure 📁
 
 Deep learning projects can be organized into the following structure with
 modularity and seperation of concerns in mind. This offers a clean and organized
 codebase that is easy to maintain and is sharable out-of-the-box.
+The modular structure of the framework involves organizing the project directory in a hierarchical tree structure, with an arbitrary name given to the root project directory by the user. The project is then broken down into distinct concerns such as models, data, trainers, experiments, analyzers, and simulators, each with its own subdirectory. Within each concern, modules can be defined with their own subdirectories, such as specific models, trainers, data loaders, data augmentations, or loss functions.
 
 ```bash
-/
-|-- models/
-|   |-- __init__.py
-|-- experiments/
-|   |-- __init__.py
-|-- trainers/
-|   |-- __init__.py
-|-- data/
-|   |-- __init__.py
+└── project_name
+    ├── data
+    │   ├── my_independent_data_loader
+    │   └── __init__.py
+    ├── experiments
+    │   ├── my_awesome_experiment
+    │   └── __init__.py
+    ├── __init__.py
+    ├── models
+    │   ├── awesomenet
+    │   └── __init__.py
+    └── trainers
+        ├── big_brain_trainer
+        └── __init__.py
 ```
 
 ### Modularity
 
 Modularity is a software design principle that focuses on creating
 self-contained, reusable and interchangeable components. In the context of a
 deep learning project, modularity means creating three independent standalone
 modules for models, trainers and data. This allows for a more organized,
 maintainable and sharable project structure. The forth module, experiments, is
 not independent, but rather combines the three modules together to create a
 complete experiment.
 
+### Independent Modules
+
+Yerbamate prioritizes the organization of the project into independent modules when applicable. Independent modules only depend on Python dependencies (such as NumPy, PyTorch, TensorFlow, or Hugging Face), and the code inside the module uses relative imports to import within the module. This makes it an independent module that can be re-used when Python dependencies are installed.
+
+### Non-Independent Modules
+In some cases, a combination of independent modules may be necessary for a particular concern. An example of this is the experiment concern, which imports and combines models, data, and trainers to define and create a specific experiment. In such cases, the module is not independent and is designed to combine the previously defined independent modules. In the case of non-independent modules, Yerbamate creates a dependency list of independent modules that can be used to install the code and Python dependencies. This ensures that the necessary modules are installed, and that the code can be run without issue.
+
+
 ### Sample Modular Project Structure
 
 This structure highlights modularity and seperation of concerns. The `models`,
 `data` and `trainers` modules are independent and can be used in any project.
 The `experiments` module is not independent, but rather combines the three
 modules together to create a complete experiment.
 
@@ -196,33 +225,38 @@
         │   ├── requirements.txt
         │   └── trainer.py
         └── __init__.py
 ```
 
 ## Example Projects 📚
 
-Please check out the [transfer learning](https://github.com/oalee/big-transfer),
+Please check out the [transfer learning](https://github.com/oalee/big_transfer),
 [vision models](https://github.com/oalee/deep-vision), and
 [lightweight gan](https://github.com/oalee/lightweight-gan).
 
 ## Documentation 📚
 
 Please check out the [documentation](https://oalee.github.io/yerbamate).
 
 ## Guides 📖
 
 For more information on modularity, please check out this [guide](https://medium.com/@alee.rmi/the-ultimate-deep-learning-project-structure-a-software-engineers-guide-into-the-land-of-ai-c383f234fd2f).
 
 For running experiments on Google Colab, please check out this
-[example](https://colab.research.google.com/gist/oalee/5f5c2b3bb2da4ec3168f3edd4a52056a/deep-learning.ipynb)
+[example](https://github.com/oalee/yerbamate/blob/main/deep_learning.ipynb)
 
 ## Contribution 🤝
 
 We welcome contributions from the community! Please check out our
 [contributing](https://github.com/oalee/yerbamate/blob/main/CONTRIBUTING.md)
 guide for more information on how to get started.
 
 ## Contact 🤝
 
 For questions please contact:
 
-yerba.mate.dl(at)proton.me
+oalee(at)proton.me
+
+
+## Open Science 📖
+
+As an open science work, Yerbamate strives to promote the principles of transparency and collaboration. To this end, the history of the LaTeX files for work are available on [GitHub](https://github.com/oalee/os-yerbamate). These open science repositories are open to collaboration and encourage participation from the community to enhance the validity, reproducibility, accessibility, and quality of this work.
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/__pycache__/environment.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/__pycache__/environment.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Feb 10 22:20:55 2023 UTC, .py size: 5843 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 47c3 e663 d316 0000  o.......G..c....
+00000000: 6f0d 0d0a 0000 0000 2c89 3264 a816 0000  o.......,.2d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6402 5a05 4700 6403 6404  d.l.Z.d.Z.G.d.d.
 00000060: 8400 6404 6506 8303 5a07 6401 5300 2905  ..d.e...Z.d.S.).
 00000070: e900 0000 004e da03 656e 7663 0000 0000  .....N..envc....
@@ -10,268 +10,268 @@
 00000090: 0000 0000 7344 0000 0065 005a 0164 005a  ....sD...e.Z.d.Z
 000000a0: 0264 0164 0284 005a 0364 0364 0484 005a  .d.d...Z.d.d...Z
 000000b0: 0464 0564 0684 005a 0564 0764 0884 005a  .d.d...Z.d.d...Z
 000000c0: 0664 0964 0a84 005a 0787 0066 0164 0b64  .d.d...Z...f.d.d
 000000d0: 0c84 085a 0887 0004 005a 0953 0029 0dda  ...Z.....Z.S.)..
 000000e0: 0b45 6e76 6972 6f6e 6d65 6e74 6301 0000  .Environmentc...
 000000f0: 0000 0000 0000 0000 0004 0000 0007 0000  ................
-00000100: 0043 0000 0073 2001 0000 6401 7c00 5f00  .C...s ...d.|._.
+00000100: 0043 0000 0073 2e01 0000 6401 7c00 5f00  .C...s....d.|._.
 00000110: 6401 7c00 5f01 6401 7c00 5f02 6401 7c00  d.|._.d.|._.d.|.
-00000120: 5f03 6900 7c00 5f04 7405 7c00 7406 6a07  _.i.|._.t.|.t.j.
-00000130: 6402 1900 6403 8303 0100 7c00 a008 a100  d...d.....|.....
-00000140: 7c00 5f09 7406 6a07 4400 5d1e 7d01 6404  |._.t.j.D.].}.d.
-00000150: 7c01 7601 7227 7120 7c01 a00a 6404 a101  |.v.r'q |...d...
-00000160: 5c02 7d02 7d03 7c00 a00b 7c03 a101 7d03  \.}.}.|...|...}.
-00000170: 7405 7c00 7c02 7c03 8303 0100 7c03 7c00  t.|.|.|.....|.|.
-00000180: 6a04 7c02 3c00 7120 7406 6a07 6405 1900  j.|.<.q t.j.d...
-00000190: 7c00 5f0c 6406 7c00 6a0c 7600 726a 740d  |._.d.|.j.v.rjt.
-000001a0: 6a0e 6a0f 7406 6a07 6407 6408 8502 1900  j.j.t.j.d.d.....
-000001b0: 8e00 7c00 5f10 740d 6a0e a00f 7c00 6a09  ..|._.t.j...|.j.
-000001c0: 6409 7406 6a07 6407 1900 7406 6a07 640a  d.t.j.d...t.j.d.
-000001d0: 1900 640b 1700 a104 7c00 5f0c 6e17 7c00  ..d.....|._.n.|.
-000001e0: 6a0c a00a 640c a101 640d 6400 8502 1900  j...d...d.d.....
-000001f0: 7c00 5f10 740d 6a0e 6a0f 7c00 6a10 8e00  |._.t.j.j.|.j...
-00000200: 6400 640e 8502 1900 7c00 5f10 7c00 a011  d.d.....|._.|...
-00000210: a100 0100 7c00 6a02 728e 7c00 a012 a100  ....|.j.r.|.....
-00000220: 0100 6400 5300 6400 5300 290f 4e46 e901  ..d.S.d.S.).NF..
-00000230: 0000 0054 fa01 3d72 0100 0000 7a08 6269  ...T..=r....z.bi
-00000240: 6e2f 6d61 7465 e902 0000 00e9 0400 0000  n/mate..........
-00000250: 5a0b 6578 7065 7269 6d65 6e74 73e9 0300  Z.experiments...
-00000260: 0000 7a03 2e70 79fa 012f e9fe ffff ffe9  ..z..py../......
-00000270: fdff ffff 2913 5a07 7265 7374 6172 74da  ....).Z.restart.
-00000280: 0474 6573 745a 0574 7261 696e da06 7361  .testZ.train..sa
-00000290: 6d70 6c65 da07 6870 6172 616d 73da 0773  mple..hparams..s
-000002a0: 6574 6174 7472 da03 7379 73da 0461 7267  etattr..sys..arg
-000002b0: 76da 175f 456e 7669 726f 6e6d 656e 745f  v.._Environment_
-000002c0: 5f66 696e 645f 726f 6f74 da05 5f72 6f6f  _find_root.._roo
-000002d0: 74da 0573 706c 6974 da13 636f 6e76 6572  t..split..conver
-000002e0: 745f 7374 725f 746f 5f64 6174 61da 055f  t_str_to_data.._
-000002f0: 7061 7468 da02 6f73 da04 7061 7468 da04  path..os..path..
-00000300: 6a6f 696e da04 6e61 6d65 da15 5f45 6e76  join..name.._Env
-00000310: 6972 6f6e 6d65 6e74 5f5f 7365 745f 656e  ironment__set_en
-00000320: 76da 215f 456e 7669 726f 6e6d 656e 745f  v.!_Environment_
-00000330: 5f67 656e 6572 6174 655f 6578 7065 7269  _generate_experi
-00000340: 6d65 6e74 2904 da04 7365 6c66 da03 6172  ment)...self..ar
-00000350: 67da 036b 6579 da05 7661 6c75 65a9 0072  g..key..value..r
-00000360: 2100 0000 fa3b 2f68 6f6d 652f 616c 2f47  !....;/home/al/G
-00000370: 6974 6875 622f 7965 7262 616d 6174 652f  ithub/yerbamate/
-00000380: 7061 636b 6167 6573 2f79 6572 6261 6d61  packages/yerbama
-00000390: 7465 2f65 6e76 6972 6f6e 6d65 6e74 2e70  te/environment.p
-000003a0: 79da 085f 5f69 6e69 745f 5f0d 0000 0073  y..__init__....s
-000003b0: 3000 0000 0604 0601 0601 0601 0601 1203  0...............
-000003c0: 0a03 0a04 0801 0201 0e01 0a01 0c01 0c01  ................
-000003d0: 0c03 0a01 1801 2801 1603 1801 0802 0602  ......(.........
-000003e0: 0c01 04ff 7a14 456e 7669 726f 6e6d 656e  ....z.Environmen
-000003f0: 742e 5f5f 696e 6974 5f5f 6302 0000 0000  t.__init__c.....
-00000400: 0000 0000 0000 0002 0000 000b 0000 0043  ...............C
-00000410: 0000 0073 6000 0000 7a05 7400 7c01 8301  ...s`...z.t.|...
-00000420: 5700 5300 0400 7401 792f 0100 0100 0100  W.S...t.y/......
-00000430: 7a07 7402 7c01 8301 5700 0600 5900 5300  z.t.|...W...Y.S.
-00000440: 0400 7401 792e 0100 0100 0100 7c01 6401  ..t.y.......|.d.
-00000450: 7600 7222 5900 5900 6402 5300 7c01 6403  v.r"Y.Y.d.S.|.d.
-00000460: 7600 722a 5900 5900 6404 5300 5900 5900  v.r*Y.Y.d.S.Y.Y.
-00000470: 7c01 5300 7700 7700 2905 4e29 02da 0454  |.S.w.w.).N)...T
-00000480: 7275 65da 0474 7275 6554 2902 da05 4661  rue..trueT)...Fa
-00000490: 6c73 65da 0566 616c 7365 4629 03da 0369  lse..falseF)...i
-000004a0: 6e74 da0a 5661 6c75 6545 7272 6f72 da05  nt..ValueError..
-000004b0: 666c 6f61 7429 0272 1d00 0000 da05 696e  float).r......in
-000004c0: 7075 7472 2100 0000 7221 0000 0072 2200  putr!...r!...r".
-000004d0: 0000 7215 0000 0036 0000 0073 1c00 0000  ..r....6...s....
-000004e0: 0201 0a01 0c01 0201 0e01 0c01 0801 0801  ................
-000004f0: 0801 0801 04ff 0403 02fa 02fd 7a1f 456e  ............z.En
-00000500: 7669 726f 6e6d 656e 742e 636f 6e76 6572  vironment.conver
-00000510: 745f 7374 725f 746f 5f64 6174 6163 0100  t_str_to_datac..
-00000520: 0000 0000 0000 0000 0000 0300 0000 0700  ................
-00000530: 0000 4300 0000 734e 0000 0074 00a0 01a1  ..C...sN...t....
-00000540: 007d 0174 006a 02a0 0374 006a 02a0 047c  .}.t.j...t.j...|
-00000550: 0164 01a1 02a1 0172 2574 05a0 0674 0774  .d.....r%t...t.t
-00000560: 006a 02a0 047c 0164 01a1 0264 0283 02a1  .j...|.d...d....
-00000570: 017d 0274 006a 02a0 047c 017c 0264 0319  .}.t.j...|.|.d..
-00000580: 00a1 0253 0064 0053 0029 044e fa09 6d61  ...S.d.S.).N..ma
-00000590: 7465 2e6a 736f 6eda 0172 da07 7072 6f6a  te.json..r..proj
-000005a0: 6563 7429 0872 1700 0000 da06 6765 7463  ect).r......getc
-000005b0: 7764 7218 0000 00da 0665 7869 7374 7372  wdr......existsr
-000005c0: 1900 0000 da04 6a73 6f6e da04 6c6f 6164  ......json..load
-000005d0: da04 6f70 656e 2903 721d 0000 0072 1800  ..open).r....r..
-000005e0: 0000 da04 636f 6e66 7221 0000 0072 2100  ....confr!...r!.
-000005f0: 0000 7222 0000 005a 0b5f 5f66 696e 645f  ..r"...Z.__find_
-00000600: 726f 6f74 4400 0000 730a 0000 0008 0316  rootD...s.......
-00000610: 021a 0112 0204 027a 1745 6e76 6972 6f6e  .......z.Environ
-00000620: 6d65 6e74 2e5f 5f66 696e 645f 726f 6f74  ment.__find_root
-00000630: 6301 0000 0000 0000 0000 0000 0007 0000  c...............
-00000640: 0008 0000 0043 0000 0073 ce00 0000 6700  .....C...s....g.
-00000650: 6401 a201 7d01 6400 7d02 7c01 4400 5d0e  d...}.d.}.|.D.].
-00000660: 7d03 7c03 7c00 6a00 7600 7216 7c00 6a00  }.|.|.j.v.r.|.j.
-00000670: 7c03 1900 7d02 0100 6e01 7108 7c02 6400  |...}...n.q.|.d.
-00000680: 7500 721d 6400 5300 7401 6a02 a003 7c02  u.r.d.S.t.j...|.
-00000690: a101 7328 7401 a004 7c02 a101 0100 7401  ..s(t...|.....t.
-000006a0: 6a02 a005 7c02 6402 a102 7d04 7406 a007  j...|.d...}.t...
-000006b0: 7c00 6a08 7c04 a102 0100 7c00 6a09 6900  |.j.|.....|.j.i.
-000006c0: 6b03 7265 7401 6a02 a005 7c02 6403 a102  k.ret.j...|.d...
-000006d0: 7d05 740a 7c05 6404 8302 8f14 7d06 740b  }.t.|.d.....}.t.
-000006e0: 6a0c 740d 7c00 6a09 8301 7c06 6405 6406  j.t.|.j...|.d.d.
-000006f0: 8d03 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00000700: 6400 5300 3100 735e 7701 0100 0100 0100  d.S.1.s^w.......
-00000710: 5900 0100 6400 5300 6400 5300 2907 4ea9  Y...d.S.d.S.).N.
-00000720: 06da 0772 6573 756c 7473 5a0c 7265 7375  ...resultsZ.resu
-00000730: 6c74 735f 7061 7468 5a0b 7265 7375 6c74  lts_pathZ.result
-00000740: 735f 6469 72da 0473 6176 655a 0973 6176  s_dir..saveZ.sav
-00000750: 655f 7061 7468 5a08 7361 7665 5f64 6972  e_pathZ.save_dir
-00000760: 7a0d 6578 7065 7269 6d65 6e74 2e70 797a  z.experiment.pyz
-00000770: 0f65 7870 6572 696d 656e 742e 6a73 6f6e  .experiment.json
-00000780: da01 7772 0700 0000 a901 da06 696e 6465  ..wr........inde
-00000790: 6e74 290e 7202 0000 0072 1700 0000 7218  nt).r....r....r.
-000007a0: 0000 0072 3000 0000 da08 6d61 6b65 6469  ...r0.....makedi
-000007b0: 7273 7219 0000 00da 0673 6875 7469 6cda  rsr......shutil.
-000007c0: 0863 6f70 7966 696c 6572 1600 0000 720e  .copyfiler....r.
-000007d0: 0000 0072 3300 0000 7231 0000 00da 0464  ...r3...r1.....d
-000007e0: 756d 70da 0464 6963 7429 0772 1d00 0000  ump..dict).r....
-000007f0: 7236 0000 00da 0672 6573 756c 7472 1f00  r6.....resultr..
-00000800: 0000 5a09 7361 7665 5f66 696c 655a 0b70  ..Z.save_fileZ.p
-00000810: 6172 616d 735f 6669 6c65 da01 6672 2100  arams_file..fr!.
-00000820: 0000 7221 0000 0072 2200 0000 5a15 5f5f  ..r!...r"...Z.__
-00000830: 6765 6e65 7261 7465 5f65 7870 6572 696d  generate_experim
-00000840: 656e 7450 0000 0073 2600 0000 0802 0401  entP...s&.......
-00000850: 0801 0a01 0a01 0401 02fe 0803 0401 0c01  ................
-00000860: 0a01 0e02 0e02 0a04 0e01 0c03 1801 22ff  ..............".
-00000870: 04fc 7a21 456e 7669 726f 6e6d 656e 742e  ..z!Environment.
-00000880: 5f5f 6765 6e65 7261 7465 5f65 7870 6572  __generate_exper
-00000890: 696d 656e 7463 0100 0000 0000 0000 0000  imentc..........
-000008a0: 0000 0d00 0000 0900 0000 4300 0000 737a  ..........C...sz
-000008b0: 0200 0074 006a 01a0 0264 01a1 017d 0174  ...t.j...d...}.t
-000008c0: 03a0 0474 057c 0164 0283 02a1 017d 0274  ...t.|.d.....}.t
-000008d0: 006a 01a0 0264 03a1 017d 0374 006a 01a0  .j...d...}.t.j..
-000008e0: 067c 03a1 0173 5074 0764 0483 0101 0074  .|...sPt.d.....t
-000008f0: 087c 0276 0072 297c 0274 0819 00a0 09a1  .|.v.r)|.t......
-00000900: 007d 046e 0364 0567 017d 0464 0664 0784  .}.n.d.g.}.d.d..
-00000910: 007c 0444 0083 017d 0574 057c 0364 0883  .|.D...}.t.|.d..
-00000920: 028f 107d 0674 036a 0a7c 057c 0664 0964  ...}.t.j.|.|.d.d
-00000930: 0a8d 0301 0057 0064 0004 0004 0083 0301  .....W.d........
-00000940: 006e 0831 0073 4b77 0101 0001 0001 0059  .n.1.sKw.......Y
-00000950: 0001 0074 057c 0364 0283 028f 1f7d 067a  ...t.|.d.....}.z
-00000960: 0774 03a0 047c 06a1 017d 0757 006e 0f04  .t...|...}.W.n..
-00000970: 0074 036a 0b6a 0c79 6c01 0001 0001 0064  .t.j.j.yl......d
-00000980: 0564 0b69 017d 0759 006e 0177 0057 0064  .d.i.}.Y.n.w.W.d
-00000990: 0004 0004 0083 0301 006e 0831 0073 7777  .........n.1.sww
-000009a0: 0101 0001 0001 0059 0001 0067 007d 0874  .......Y...g.}.t
-000009b0: 087c 0276 0072 a77c 07a0 0da1 0044 005d  .|.v.r.|.....D.]
-000009c0: 205c 027d 097d 0a7c 077c 0919 0064 0b6b   \.}.}.|.|...d.k
-000009d0: 0272 a67c 0974 006a 0e76 0072 9d74 006a  .r.|.t.j.v.r.t.j
-000009e0: 0e7c 0919 007c 077c 093c 0071 867c 08a0  .|...|.|.<.q.|..
-000009f0: 0f7c 09a1 0101 007c 0a7c 077c 093c 0071  .|.....|.|.|.<.q
-00000a00: 8674 107c 0883 0164 0c6b 0472 d674 0764  .t.|...d.k.r.t.d
-00000a10: 0d83 0101 007c 0844 005d 197d 097c 097c  .....|.D.].}.|.|
-00000a20: 0274 0819 0076 0072 c17c 0274 0819 007c  .t...v.r.|.t...|
-00000a30: 0919 006e 0164 0e7d 0b74 077c 099b 0064  ...n.d.}.t.|...d
-00000a40: 0f7c 0b9b 009d 0383 0101 0071 b374 0764  .|.........q.t.d
-00000a50: 1083 0101 0074 11a0 1264 11a1 0101 0067  .....t...d.....g
-00000a60: 0064 12a2 017d 0c7c 0c44 005d 447d 097c  .d...}.|.D.]D}.|
-00000a70: 097c 0776 0072 fc74 006a 016a 027c 077c  .|.v.r.t.j.j.|.|
-00000a80: 0919 0067 017c 006a 13a0 1464 13a1 01a2  ...g.|.j...d....
-00000a90: 0152 008e 007c 077c 093c 007c 077c 0919  .R...|.|.<.|.|..
-00000aa0: 007c 0764 053c 0001 006e 2574 006a 0ea0  .|.d.<...n%t.j..
-00000ab0: 157c 0964 00a1 0264 0075 0190 0172 2074  .|.d...d.u...r t
-00000ac0: 006a 0ea0 157c 0964 00a1 0264 0b6b 0390  .j...|.d...d.k..
-00000ad0: 0172 2074 006a 0ea0 157c 09a1 017c 077c  .r t.j...|...|.|
-00000ae0: 093c 007c 077c 0919 007c 0764 053c 0001  .<.|.|...|.d.<..
-00000af0: 006e 0171 dc74 107c 0783 0164 0c6b 0290  .n.q.t.|...d.k..
-00000b00: 0172 3574 0764 1483 0101 0074 0764 1083  .r5t.d.....t.d..
-00000b10: 0101 0074 11a0 1264 11a1 0101 0074 167c  ...t...d.....t.|
-00000b20: 0064 157c 0783 0301 0064 0053 0029 164e  .d.|.....d.S.).N
-00000b30: 722c 0000 0072 2d00 0000 7a08 656e 762e  r,...r-...z.env.
-00000b40: 6a73 6f6e 7a40 456e 7669 726f 6e6d 656e  jsonz@Environmen
-00000b50: 7420 6669 6c65 206e 6f74 2066 6f75 6e64  t file not found
-00000b60: 2c20 6372 6561 7469 6e67 206f 6e65 2077  , creating one w
-00000b70: 6974 6820 6465 6661 756c 7473 3a20 656e  ith defaults: en
-00000b80: 762e 6a73 6f6e 7236 0000 0063 0100 0000  v.jsonr6...c....
-00000b90: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000ba0: 5300 0000 7312 0000 0069 007c 005d 057d  S...s....i.|.].}
-00000bb0: 017c 0164 0093 0271 0253 0029 01da 0072  .|.d...q.S.)...r
-00000bc0: 2100 0000 2902 da02 2e30 721f 0000 0072  !...)....0r....r
-00000bd0: 2100 0000 7221 0000 0072 2200 0000 da0a  !...r!...r".....
-00000be0: 3c64 6963 7463 6f6d 703e 7900 0000 7302  <dictcomp>y...s.
-00000bf0: 0000 0012 007a 2945 6e76 6972 6f6e 6d65  .....z)Environme
-00000c00: 6e74 2e5f 5f73 6574 5f65 6e76 2e3c 6c6f  nt.__set_env.<lo
-00000c10: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
-00000c20: 7238 0000 0072 0700 0000 7239 0000 0072  r8...r....r9...r
-00000c30: 4200 0000 7201 0000 007a 4745 6e76 6972  B...r....zGEnvir
-00000c40: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
-00000c50: 206e 6f74 2066 6f75 6e64 2e20 5365 7420   not found. Set 
-00000c60: 7468 656d 2069 6e20 656e 762e 6a73 6f6e  them in env.json
-00000c70: 206f 7220 696e 2079 6f75 7220 7368 656c   or in your shel
-00000c80: 6c2e 7a1d 5265 7175 6972 6564 2065 6e76  l.z.Required env
-00000c90: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00000ca0: 657a 0320 3a20 fa0a 4578 6974 696e 672e  ez. : ..Exiting.
-00000cb0: 2e2e 7204 0000 0072 3500 0000 7209 0000  ..r....r5...r...
-00000cc0: 007a 5972 6573 756c 7473 2f73 6176 655f  .zYresults/save_
-00000cd0: 6469 722f 7361 7665 2065 6e76 6972 6f6e  dir/save environ
-00000ce0: 6d65 6e74 2076 6172 6961 626c 6520 6973  ment variable is
-00000cf0: 2065 6d70 7479 2e20 5365 7420 6974 2069   empty. Set it i
-00000d00: 6e20 656e 762e 6a73 6f6e 206f 7220 696e  n env.json or in
-00000d10: 2079 6f75 7220 7368 656c 6c2e 7202 0000   your shell.r...
-00000d20: 0029 1772 1700 0000 7218 0000 0072 1900  .).r....r....r..
-00000d30: 0000 7231 0000 0072 3200 0000 7233 0000  ..r1...r2...r3..
-00000d40: 0072 3000 0000 da05 7072 696e 74da 0745  .r0.....print..E
-00000d50: 4e56 5f4b 4559 da04 6b65 7973 723e 0000  NV_KEY..keysr>..
-00000d60: 00da 0764 6563 6f64 6572 5a0f 4a53 4f4e  ...decoderZ.JSON
-00000d70: 4465 636f 6465 4572 726f 72da 0569 7465  DecodeError..ite
-00000d80: 6d73 da07 656e 7669 726f 6eda 0661 7070  ms..environ..app
-00000d90: 656e 64da 036c 656e 7210 0000 00da 0465  end..lenr......e
-00000da0: 7869 7472 1a00 0000 7214 0000 00da 0367  xitr....r......g
-00000db0: 6574 720f 0000 0029 0d72 1d00 0000 5a0e  etr....).r....Z.
-00000dc0: 6d61 7465 5f63 6f6e 665f 7061 7468 7234  mate_conf_pathr4
-00000dd0: 0000 005a 0865 6e76 5f70 6174 68da 0d72  ...Z.env_path..r
-00000de0: 6571 7569 7265 645f 6b65 7973 5a0b 6465  equired_keysZ.de
-00000df0: 6675 616c 745f 656e 7672 4100 0000 7202  fualt_envrA...r.
-00000e00: 0000 005a 0d65 6e76 5f6e 6f74 5f66 6f75  ...Z.env_not_fou
-00000e10: 6e64 721f 0000 0072 2000 0000 5a04 6465  ndr....r ...Z.de
-00000e20: 7363 5a0e 7365 6172 6368 5f72 6573 756c  scZ.search_resul
-00000e30: 7473 7221 0000 0072 2100 0000 7222 0000  tsr!...r!...r"..
-00000e40: 005a 095f 5f73 6574 5f65 6e76 6c00 0000  .Z.__set_envl...
-00000e50: 736a 0000 000c 0110 010c 020c 0108 0108  sj..............
-00000e60: 020e 0106 020e 020c 0212 011c ff0c 0402  ................
-00000e70: 010e 0110 0104 0208 ff02 ff02 801c fd04  ................
-00000e80: 0808 0210 010c 010a 0110 010a 0308 0102  ................
-00000e90: 800c 0208 0108 011c 0114 0108 020a 0108  ................
-00000ea0: 0308 0108 0124 010c 0104 0128 0110 010c  .....$.....(....
-00000eb0: 0104 0102 800e 0208 0108 010a 0110 027a  ...............z
-00000ec0: 1545 6e76 6972 6f6e 6d65 6e74 2e5f 5f73  .Environment.__s
-00000ed0: 6574 5f65 6e76 6302 0000 0000 0000 0000  et_envc.........
-00000ee0: 0000 0003 0000 0004 0000 0003 0000 0073  ...............s
-00000ef0: 6e00 0000 7c01 7c00 7601 7231 7c01 7c00  n...|.|.v.r1|.|.
-00000f00: 6a00 7600 720e 7c00 6a00 7c01 1900 5300  j.v.r.|.j.|...S.
-00000f10: 7401 6a02 a003 7c01 6400 a102 7d02 7c02  t.j...|.d...}.|.
-00000f20: 6400 7500 731d 7c02 6401 6b02 722f 7404  d.u.s.|.d.k.r/t.
-00000f30: 6402 7c01 9b00 6403 9d03 8301 0100 7404  d.|...d.......t.
-00000f40: 6404 8301 0100 7405 a006 6405 a101 0100  d.....t...d.....
-00000f50: 6e02 7c02 5300 7407 8300 a008 7c01 a101  n.|.S.t.....|...
-00000f60: 5300 2906 4e72 4200 0000 7a15 456e 7669  S.).NrB...z.Envi
-00000f70: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-00000f80: 207a 3020 6e6f 7420 666f 756e 642e 2053   z0 not found. S
-00000f90: 6574 2069 7420 696e 2065 6e76 2e6a 736f  et it in env.jso
-00000fa0: 6e20 6f72 2069 6e20 796f 7572 2073 6865  n or in your she
-00000fb0: 6c6c 2e72 4500 0000 7204 0000 0029 0972  ll.rE...r....).r
-00000fc0: 0200 0000 7217 0000 0072 4b00 0000 724f  ....r....rK...rO
-00000fd0: 0000 0072 4600 0000 7210 0000 0072 4e00  ...rF...r....rN.
-00000fe0: 0000 da05 7375 7065 72da 0b5f 5f67 6574  ....super..__get
-00000ff0: 6974 656d 5f5f 2903 721d 0000 0072 1f00  item__).r....r..
-00001000: 0000 da03 7265 73a9 01da 095f 5f63 6c61  ....res....__cla
-00001010: 7373 5f5f 7221 0000 0072 2200 0000 7252  ss__r!...r"...rR
-00001020: 0000 00af 0000 0073 1400 0000 0801 0a02  .......s........
-00001030: 0a01 0e01 1002 1001 0801 0c01 0402 0c02  ................
-00001040: 7a17 456e 7669 726f 6e6d 656e 742e 5f5f  z.Environment.__
-00001050: 6765 7469 7465 6d5f 5f29 0ada 085f 5f6e  getitem__)...__n
-00001060: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00001070: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00001080: 2300 0000 7215 0000 0072 1200 0000 721c  #...r....r....r.
-00001090: 0000 0072 1b00 0000 7252 0000 00da 0d5f  ...r....rR....._
-000010a0: 5f63 6c61 7373 6365 6c6c 5f5f 7221 0000  _classcell__r!..
-000010b0: 0072 2100 0000 7254 0000 0072 2200 0000  .r!...rT...r"...
-000010c0: 7203 0000 000b 0000 0073 0e00 0000 0800  r........s......
-000010d0: 0802 0829 080e 080c 081c 1443 7203 0000  ...).......Cr...
-000010e0: 0029 0872 3100 0000 7217 0000 0072 3c00  .).r1...r....r<.
-000010f0: 0000 7210 0000 005a 0469 7064 6272 4700  ..r....Z.ipdbrG.
-00001100: 0000 723f 0000 0072 0300 0000 7221 0000  ..r?...r....r!..
-00001110: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
-00001120: da08 3c6d 6f64 756c 653e 0100 0000 730e  ..<module>....s.
-00001130: 0000 0008 0108 0108 0108 0108 0104 0314  ................
-00001140: 02                                       .
+00000120: 5f03 6900 7c00 5f04 7a0b 7405 7c00 7406  _.i.|._.z.t.|.t.
+00000130: 6a07 6402 1900 6403 8303 0100 5700 6e04  j.d...d.....W.n.
+00000140: 0100 0100 0100 5900 7c00 a008 a100 7c00  ......Y.|.....|.
+00000150: 5f09 7406 6a07 4400 5d1e 7d01 6404 7c01  _.t.j.D.].}.d.|.
+00000160: 7601 722e 7127 7c01 a00a 6404 a101 5c02  v.r.q'|...d...\.
+00000170: 7d02 7d03 7c00 a00b 7c03 a101 7d03 7405  }.}.|...|...}.t.
+00000180: 7c00 7c02 7c03 8303 0100 7c03 7c00 6a04  |.|.|.....|.|.j.
+00000190: 7c02 3c00 7127 7406 6a07 6405 1900 7c00  |.<.q't.j.d...|.
+000001a0: 5f0c 6406 7c00 6a0c 7600 7271 740d 6a0e  _.d.|.j.v.rqt.j.
+000001b0: 6a0f 7406 6a07 6407 6408 8502 1900 8e00  j.t.j.d.d.......
+000001c0: 7c00 5f10 740d 6a0e a00f 7c00 6a09 6409  |._.t.j...|.j.d.
+000001d0: 7406 6a07 6407 1900 7406 6a07 640a 1900  t.j.d...t.j.d...
+000001e0: 640b 1700 a104 7c00 5f0c 6e17 7c00 6a0c  d.....|._.n.|.j.
+000001f0: a00a 640c a101 640d 6400 8502 1900 7c00  ..d...d.d.....|.
+00000200: 5f10 740d 6a0e 6a0f 7c00 6a10 8e00 6400  _.t.j.j.|.j...d.
+00000210: 640e 8502 1900 7c00 5f10 7c00 a011 a100  d.....|._.|.....
+00000220: 0100 7c00 6a02 7295 7c00 a012 a100 0100  ..|.j.r.|.......
+00000230: 6400 5300 6400 5300 290f 4e46 e901 0000  d.S.d.S.).NF....
+00000240: 0054 fa01 3d72 0100 0000 7a08 6269 6e2f  .T..=r....z.bin/
+00000250: 6d61 7465 e902 0000 00e9 0400 0000 5a0b  mate..........Z.
+00000260: 6578 7065 7269 6d65 6e74 73e9 0300 0000  experiments.....
+00000270: 7a03 2e70 79fa 012f e9fe ffff ffe9 fdff  z..py../........
+00000280: ffff 2913 5a07 7265 7374 6172 74da 0474  ..).Z.restart..t
+00000290: 6573 745a 0574 7261 696e da06 7361 6d70  estZ.train..samp
+000002a0: 6c65 da07 6870 6172 616d 73da 0773 6574  le..hparams..set
+000002b0: 6174 7472 da03 7379 73da 0461 7267 76da  attr..sys..argv.
+000002c0: 175f 456e 7669 726f 6e6d 656e 745f 5f66  ._Environment__f
+000002d0: 696e 645f 726f 6f74 da05 5f72 6f6f 74da  ind_root.._root.
+000002e0: 0573 706c 6974 da13 636f 6e76 6572 745f  .split..convert_
+000002f0: 7374 725f 746f 5f64 6174 61da 055f 7061  str_to_data.._pa
+00000300: 7468 da02 6f73 da04 7061 7468 da04 6a6f  th..os..path..jo
+00000310: 696e da04 6e61 6d65 da15 5f45 6e76 6972  in..name.._Envir
+00000320: 6f6e 6d65 6e74 5f5f 7365 745f 656e 76da  onment__set_env.
+00000330: 215f 456e 7669 726f 6e6d 656e 745f 5f67  !_Environment__g
+00000340: 656e 6572 6174 655f 6578 7065 7269 6d65  enerate_experime
+00000350: 6e74 2904 da04 7365 6c66 da03 6172 67da  nt)...self..arg.
+00000360: 036b 6579 da05 7661 6c75 65a9 0072 2100  .key..value..r!.
+00000370: 0000 fa3b 2f68 6f6d 652f 616c 2f47 6974  ...;/home/al/Git
+00000380: 4875 622f 7965 7262 616d 6174 652f 7061  Hub/yerbamate/pa
+00000390: 636b 6167 6573 2f79 6572 6261 6d61 7465  ckages/yerbamate
+000003a0: 2f65 6e76 6972 6f6e 6d65 6e74 2e70 79da  /environment.py.
+000003b0: 085f 5f69 6e69 745f 5f0e 0000 0073 3a00  .__init__....s:.
+000003c0: 0000 0603 0601 0601 0601 0601 0203 1601  ................
+000003d0: 0601 0201 0a02 0a03 0801 0201 0e01 0a01  ................
+000003e0: 0c01 0c01 0c02 0a01 1801 0601 1a01 08ff  ................
+000003f0: 1604 1801 0802 0602 0c01 04ff 7a14 456e  ............z.En
+00000400: 7669 726f 6e6d 656e 742e 5f5f 696e 6974  vironment.__init
+00000410: 5f5f 6302 0000 0000 0000 0000 0000 0002  __c.............
+00000420: 0000 000b 0000 0043 0000 0073 6000 0000  .......C...s`...
+00000430: 7a05 7400 7c01 8301 5700 5300 0400 7401  z.t.|...W.S...t.
+00000440: 792f 0100 0100 0100 7a07 7402 7c01 8301  y/......z.t.|...
+00000450: 5700 0600 5900 5300 0400 7401 792e 0100  W...Y.S...t.y...
+00000460: 0100 0100 7c01 6401 7600 7222 5900 5900  ....|.d.v.r"Y.Y.
+00000470: 6402 5300 7c01 6403 7600 722a 5900 5900  d.S.|.d.v.r*Y.Y.
+00000480: 6404 5300 5900 5900 7c01 5300 7700 7700  d.S.Y.Y.|.S.w.w.
+00000490: 2905 4e29 02da 0454 7275 65da 0474 7275  ).N)...True..tru
+000004a0: 6554 2902 da05 4661 6c73 65da 0566 616c  eT)...False..fal
+000004b0: 7365 4629 03da 0369 6e74 da0a 5661 6c75  seF)...int..Valu
+000004c0: 6545 7272 6f72 da05 666c 6f61 7429 0272  eError..float).r
+000004d0: 1d00 0000 da05 696e 7075 7472 2100 0000  ......inputr!...
+000004e0: 7221 0000 0072 2200 0000 7215 0000 0037  r!...r"...r....7
+000004f0: 0000 0073 1c00 0000 0201 0a01 0c01 0201  ...s............
+00000500: 0e01 0c01 0801 0801 0801 0801 04ff 0403  ................
+00000510: 02fa 02fd 7a1f 456e 7669 726f 6e6d 656e  ....z.Environmen
+00000520: 742e 636f 6e76 6572 745f 7374 725f 746f  t.convert_str_to
+00000530: 5f64 6174 6163 0100 0000 0000 0000 0000  _datac..........
+00000540: 0000 0300 0000 0700 0000 4300 0000 734e  ..........C...sN
+00000550: 0000 0074 00a0 01a1 007d 0174 006a 02a0  ...t.....}.t.j..
+00000560: 0374 006a 02a0 047c 0164 01a1 02a1 0172  .t.j...|.d.....r
+00000570: 2574 05a0 0674 0774 006a 02a0 047c 0164  %t...t.t.j...|.d
+00000580: 01a1 0264 0283 02a1 017d 0274 006a 02a0  ...d.....}.t.j..
+00000590: 047c 017c 0264 0319 00a1 0253 0064 0053  .|.|.d.....S.d.S
+000005a0: 0029 044e fa09 6d61 7465 2e6a 736f 6eda  .).N..mate.json.
+000005b0: 0172 da07 7072 6f6a 6563 7429 0872 1700  .r..project).r..
+000005c0: 0000 da06 6765 7463 7764 7218 0000 00da  ....getcwdr.....
+000005d0: 0665 7869 7374 7372 1900 0000 da04 6a73  .existsr......js
+000005e0: 6f6e da04 6c6f 6164 da04 6f70 656e 2903  on..load..open).
+000005f0: 721d 0000 0072 1800 0000 da04 636f 6e66  r....r......conf
+00000600: 7221 0000 0072 2100 0000 7222 0000 005a  r!...r!...r"...Z
+00000610: 0b5f 5f66 696e 645f 726f 6f74 4500 0000  .__find_rootE...
+00000620: 730a 0000 0008 0316 021a 0112 0204 027a  s..............z
+00000630: 1745 6e76 6972 6f6e 6d65 6e74 2e5f 5f66  .Environment.__f
+00000640: 696e 645f 726f 6f74 6301 0000 0000 0000  ind_rootc.......
+00000650: 0000 0000 0007 0000 0008 0000 0043 0000  .............C..
+00000660: 0073 ce00 0000 6700 6401 a201 7d01 6400  .s....g.d...}.d.
+00000670: 7d02 7c01 4400 5d0e 7d03 7c03 7c00 6a00  }.|.D.].}.|.|.j.
+00000680: 7600 7216 7c00 6a00 7c03 1900 7d02 0100  v.r.|.j.|...}...
+00000690: 6e01 7108 7c02 6400 7500 721d 6400 5300  n.q.|.d.u.r.d.S.
+000006a0: 7401 6a02 a003 7c02 a101 7328 7401 a004  t.j...|...s(t...
+000006b0: 7c02 a101 0100 7401 6a02 a005 7c02 6402  |.....t.j...|.d.
+000006c0: a102 7d04 7406 a007 7c00 6a08 7c04 a102  ..}.t...|.j.|...
+000006d0: 0100 7c00 6a09 6900 6b03 7265 7401 6a02  ..|.j.i.k.ret.j.
+000006e0: a005 7c02 6403 a102 7d05 740a 7c05 6404  ..|.d...}.t.|.d.
+000006f0: 8302 8f14 7d06 740b 6a0c 740d 7c00 6a09  ....}.t.j.t.|.j.
+00000700: 8301 7c06 6405 6406 8d03 0100 5700 6400  ..|.d.d.....W.d.
+00000710: 0400 0400 8303 0100 6400 5300 3100 735e  ........d.S.1.s^
+00000720: 7701 0100 0100 0100 5900 0100 6400 5300  w.......Y...d.S.
+00000730: 6400 5300 2907 4e29 06da 0772 6573 756c  d.S.).N)...resul
+00000740: 7473 5a0c 7265 7375 6c74 735f 7061 7468  tsZ.results_path
+00000750: 5a0b 7265 7375 6c74 735f 6469 72da 0473  Z.results_dir..s
+00000760: 6176 65da 0973 6176 655f 7061 7468 5a08  ave..save_pathZ.
+00000770: 7361 7665 5f64 6972 7a0d 6578 7065 7269  save_dirz.experi
+00000780: 6d65 6e74 2e70 797a 0f65 7870 6572 696d  ment.pyz.experim
+00000790: 656e 742e 6a73 6f6e da01 7772 0700 0000  ent.json..wr....
+000007a0: a901 da06 696e 6465 6e74 290e 7202 0000  ....indent).r...
+000007b0: 0072 1700 0000 7218 0000 0072 3000 0000  .r....r....r0...
+000007c0: da08 6d61 6b65 6469 7273 7219 0000 00da  ..makedirsr.....
+000007d0: 0673 6875 7469 6cda 0863 6f70 7966 696c  .shutil..copyfil
+000007e0: 6572 1600 0000 720e 0000 0072 3300 0000  er....r....r3...
+000007f0: 7231 0000 00da 0464 756d 70da 0464 6963  r1.....dump..dic
+00000800: 7429 0772 1d00 0000 7235 0000 00da 0672  t).r....r5.....r
+00000810: 6573 756c 7472 1f00 0000 5a09 7361 7665  esultr....Z.save
+00000820: 5f66 696c 655a 0b70 6172 616d 735f 6669  _fileZ.params_fi
+00000830: 6c65 da01 6672 2100 0000 7221 0000 0072  le..fr!...r!...r
+00000840: 2200 0000 5a15 5f5f 6765 6e65 7261 7465  "...Z.__generate
+00000850: 5f65 7870 6572 696d 656e 7451 0000 0073  _experimentQ...s
+00000860: 2600 0000 0802 0402 0801 0a01 0a01 0401  &...............
+00000870: 02fe 0803 0401 0c01 0a01 0e02 0e02 0a04  ................
+00000880: 0e01 0c03 1801 22ff 04fc 7a21 456e 7669  ......"...z!Envi
+00000890: 726f 6e6d 656e 742e 5f5f 6765 6e65 7261  ronment.__genera
+000008a0: 7465 5f65 7870 6572 696d 656e 7463 0100  te_experimentc..
+000008b0: 0000 0000 0000 0000 0000 0d00 0000 0900  ................
+000008c0: 0000 4300 0000 7360 0200 0074 006a 01a0  ..C...s`...t.j..
+000008d0: 0264 01a1 017d 0174 03a0 0474 057c 0164  .d...}.t...t.|.d
+000008e0: 0283 02a1 017d 0274 006a 01a0 0264 03a1  .....}.t.j...d..
+000008f0: 017d 0374 006a 01a0 067c 03a1 0173 5074  .}.t.j...|...sPt
+00000900: 0764 0483 0101 0074 087c 0276 0072 297c  .d.....t.|.v.r)|
+00000910: 0274 0819 00a0 09a1 007d 046e 0364 0567  .t.......}.n.d.g
+00000920: 017d 0464 0664 0784 007c 0444 0083 017d  .}.d.d...|.D...}
+00000930: 0574 057c 0364 0883 028f 107d 0674 036a  .t.|.d.....}.t.j
+00000940: 0a7c 057c 0664 0964 0a8d 0301 0057 0064  .|.|.d.d.....W.d
+00000950: 0004 0004 0083 0301 006e 0831 0073 4b77  .........n.1.sKw
+00000960: 0101 0001 0001 0059 0001 0074 057c 0364  .......Y...t.|.d
+00000970: 0283 028f 1f7d 067a 0774 03a0 047c 06a1  .....}.z.t...|..
+00000980: 017d 0757 006e 0f04 0074 036a 0b6a 0c79  .}.W.n...t.j.j.y
+00000990: 6c01 0001 0001 0064 0564 0b69 017d 0759  l......d.d.i.}.Y
+000009a0: 006e 0177 0057 0064 0004 0004 0083 0301  .n.w.W.d........
+000009b0: 006e 0831 0073 7777 0101 0001 0001 0059  .n.1.sww.......Y
+000009c0: 0001 0067 007d 0874 087c 0276 0072 a77c  ...g.}.t.|.v.r.|
+000009d0: 07a0 0da1 0044 005d 205c 027d 097d 0a7c  .....D.] \.}.}.|
+000009e0: 077c 0919 0064 0b6b 0272 a67c 0974 006a  .|...d.k.r.|.t.j
+000009f0: 0e76 0072 9d74 006a 0e7c 0919 007c 077c  .v.r.t.j.|...|.|
+00000a00: 093c 0071 867c 08a0 0f7c 09a1 0101 007c  .<.q.|...|.....|
+00000a10: 0a7c 077c 093c 0071 8674 107c 0883 0164  .|.|.<.q.t.|...d
+00000a20: 0c6b 0472 d674 0764 0d83 0101 007c 0844  .k.r.t.d.....|.D
+00000a30: 005d 197d 097c 097c 0274 0819 0076 0072  .].}.|.|.t...v.r
+00000a40: c17c 0274 0819 007c 0919 006e 0164 0e7d  .|.t...|...n.d.}
+00000a50: 0b74 077c 099b 0064 0f7c 0b9b 009d 0383  .t.|...d.|......
+00000a60: 0101 0071 b374 0764 1083 0101 0074 11a0  ...q.t.d.....t..
+00000a70: 1264 11a1 0101 0064 1267 017d 0c7c 0c44  .d.....d.g.}.|.D
+00000a80: 005d 387d 097c 097c 0776 0072 f574 006a  .]8}.|.|.v.r.t.j
+00000a90: 016a 027c 077c 0919 0067 017c 006a 13a0  .j.|.|...g.|.j..
+00000aa0: 1464 13a1 01a2 0152 008e 007c 077c 093c  .d.....R...|.|.<
+00000ab0: 0001 006e 1f74 006a 0ea0 157c 0964 00a1  ...n.t.j...|.d..
+00000ac0: 0264 0075 0190 0172 1374 006a 0ea0 157c  .d.u...r.t.j...|
+00000ad0: 0964 00a1 0264 0b6b 0390 0172 1374 006a  .d...d.k...r.t.j
+00000ae0: 0ea0 157c 09a1 017c 077c 093c 0001 006e  ...|...|.|.<...n
+00000af0: 0171 db74 107c 0783 0164 0c6b 0290 0172  .q.t.|...d.k...r
+00000b00: 2874 0764 1483 0101 0074 0764 1083 0101  (t.d.....t.d....
+00000b10: 0074 11a0 1264 11a1 0101 0074 167c 0064  .t...d.....t.|.d
+00000b20: 157c 0783 0301 0064 0053 0029 164e 722c  .|.....d.S.).Nr,
+00000b30: 0000 0072 2d00 0000 7a08 656e 762e 6a73  ...r-...z.env.js
+00000b40: 6f6e 7a40 456e 7669 726f 6e6d 656e 7420  onz@Environment 
+00000b50: 6669 6c65 206e 6f74 2066 6f75 6e64 2c20  file not found, 
+00000b60: 6372 6561 7469 6e67 206f 6e65 2077 6974  creating one wit
+00000b70: 6820 6465 6661 756c 7473 3a20 656e 762e  h defaults: env.
+00000b80: 6a73 6f6e 7235 0000 0063 0100 0000 0000  jsonr5...c......
+00000b90: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
+00000ba0: 0000 7312 0000 0069 007c 005d 057d 017c  ..s....i.|.].}.|
+00000bb0: 0164 0093 0271 0253 0029 01da 0072 2100  .d...q.S.)...r!.
+00000bc0: 0000 2902 da02 2e30 721f 0000 0072 2100  ..)....0r....r!.
+00000bd0: 0000 7221 0000 0072 2200 0000 da0a 3c64  ..r!...r".....<d
+00000be0: 6963 7463 6f6d 703e 7900 0000 7302 0000  ictcomp>y...s...
+00000bf0: 0012 007a 2945 6e76 6972 6f6e 6d65 6e74  ...z)Environment
+00000c00: 2e5f 5f73 6574 5f65 6e76 2e3c 6c6f 6361  .__set_env.<loca
+00000c10: 6c73 3e2e 3c64 6963 7463 6f6d 703e 7238  ls>.<dictcomp>r8
+00000c20: 0000 0072 0700 0000 7239 0000 0072 4200  ...r....r9...rB.
+00000c30: 0000 7201 0000 007a 4745 6e76 6972 6f6e  ..r....zGEnviron
+00000c40: 6d65 6e74 2076 6172 6961 626c 6573 206e  ment variables n
+00000c50: 6f74 2066 6f75 6e64 2e20 5365 7420 7468  ot found. Set th
+00000c60: 656d 2069 6e20 656e 762e 6a73 6f6e 206f  em in env.json o
+00000c70: 7220 696e 2079 6f75 7220 7368 656c 6c2e  r in your shell.
+00000c80: 7a1d 5265 7175 6972 6564 2065 6e76 6972  z.Required envir
+00000c90: 6f6e 6d65 6e74 2076 6172 6961 626c 657a  onment variablez
+00000ca0: 0320 3a20 fa0a 4578 6974 696e 672e 2e2e  . : ..Exiting...
+00000cb0: 7204 0000 005a 0961 7574 6f5f 7361 7665  r....Z.auto_save
+00000cc0: 7209 0000 007a 5972 6573 756c 7473 2f73  r....zYresults/s
+00000cd0: 6176 655f 6469 722f 7361 7665 2065 6e76  ave_dir/save env
+00000ce0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+00000cf0: 6520 6973 2065 6d70 7479 2e20 5365 7420  e is empty. Set 
+00000d00: 6974 2069 6e20 656e 762e 6a73 6f6e 206f  it in env.json o
+00000d10: 7220 696e 2079 6f75 7220 7368 656c 6c2e  r in your shell.
+00000d20: 7202 0000 0029 1772 1700 0000 7218 0000  r....).r....r...
+00000d30: 0072 1900 0000 7231 0000 0072 3200 0000  .r....r1...r2...
+00000d40: 7233 0000 0072 3000 0000 da05 7072 696e  r3...r0.....prin
+00000d50: 74da 0745 4e56 5f4b 4559 da04 6b65 7973  t..ENV_KEY..keys
+00000d60: 723e 0000 00da 0764 6563 6f64 6572 da0f  r>.....decoder..
+00000d70: 4a53 4f4e 4465 636f 6465 4572 726f 72da  JSONDecodeError.
+00000d80: 0569 7465 6d73 da07 656e 7669 726f 6eda  .items..environ.
+00000d90: 0661 7070 656e 64da 036c 656e 7210 0000  .append..lenr...
+00000da0: 00da 0465 7869 7472 1a00 0000 7214 0000  ...exitr....r...
+00000db0: 00da 0367 6574 720f 0000 0029 0d72 1d00  ...getr....).r..
+00000dc0: 0000 5a0e 6d61 7465 5f63 6f6e 665f 7061  ..Z.mate_conf_pa
+00000dd0: 7468 7234 0000 005a 0865 6e76 5f70 6174  thr4...Z.env_pat
+00000de0: 68da 0d72 6571 7569 7265 645f 6b65 7973  h..required_keys
+00000df0: 5a0b 6465 6675 616c 745f 656e 7672 4100  Z.defualt_envrA.
+00000e00: 0000 7202 0000 005a 0d65 6e76 5f6e 6f74  ..r....Z.env_not
+00000e10: 5f66 6f75 6e64 721f 0000 0072 2000 0000  _foundr....r ...
+00000e20: da04 6465 7363 5a0e 7365 6172 6368 5f72  ..descZ.search_r
+00000e30: 6573 756c 7473 7221 0000 0072 2100 0000  esultsr!...r!...
+00000e40: 7222 0000 005a 095f 5f73 6574 5f65 6e76  r"...Z.__set_env
+00000e50: 6c00 0000 736e 0000 000c 0110 010c 020c  l...sn..........
+00000e60: 0108 0108 020e 0106 020e 020c 0212 011c  ................
+00000e70: ff0c 0302 010e 0110 0104 0208 ff02 ff02  ................
+00000e80: 801c fd04 0808 0210 010c 010a 0110 010a  ................
+00000e90: 0308 0102 800c 0202 0102 0104 ff08 021c  ................
+00000ea0: 0114 0108 020a 0106 0308 0108 0124 0104  .............$..
+00000eb0: 0228 0110 0104 0202 800e 0202 0102 0104  .(..............
+00000ec0: ff08 020a 0110 027a 1545 6e76 6972 6f6e  .......z.Environ
+00000ed0: 6d65 6e74 2e5f 5f73 6574 5f65 6e76 6302  ment.__set_envc.
+00000ee0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00000ef0: 0000 0003 0000 0073 6e00 0000 7c01 7c00  .......sn...|.|.
+00000f00: 7601 7231 7c01 7c00 6a00 7600 720e 7c00  v.r1|.|.j.v.r.|.
+00000f10: 6a00 7c01 1900 5300 7401 6a02 a003 7c01  j.|...S.t.j...|.
+00000f20: 6400 a102 7d02 7c02 6400 7500 731d 7c02  d...}.|.d.u.s.|.
+00000f30: 6401 6b02 722f 7404 6402 7c01 9b00 6403  d.k.r/t.d.|...d.
+00000f40: 9d03 8301 0100 7404 6404 8301 0100 7405  ......t.d.....t.
+00000f50: a006 6405 a101 0100 6e02 7c02 5300 7407  ..d.....n.|.S.t.
+00000f60: 8300 a008 7c01 a101 5300 2906 4e72 4200  ....|...S.).NrB.
+00000f70: 0000 7a15 456e 7669 726f 6e6d 656e 7420  ..z.Environment 
+00000f80: 7661 7269 6162 6c65 207a 3020 6e6f 7420  variable z0 not 
+00000f90: 666f 756e 642e 2053 6574 2069 7420 696e  found. Set it in
+00000fa0: 2065 6e76 2e6a 736f 6e20 6f72 2069 6e20   env.json or in 
+00000fb0: 796f 7572 2073 6865 6c6c 2e72 4500 0000  your shell.rE...
+00000fc0: 7204 0000 0029 0972 0200 0000 7217 0000  r....).r....r...
+00000fd0: 0072 4c00 0000 7250 0000 0072 4600 0000  .rL...rP...rF...
+00000fe0: 7210 0000 0072 4f00 0000 da05 7375 7065  r....rO.....supe
+00000ff0: 72da 0b5f 5f67 6574 6974 656d 5f5f 2903  r..__getitem__).
+00001000: 721d 0000 0072 1f00 0000 da03 7265 73a9  r....r......res.
+00001010: 01da 095f 5f63 6c61 7373 5f5f 7221 0000  ...__class__r!..
+00001020: 0072 2200 0000 7254 0000 00b0 0000 0073  .r"...rT.......s
+00001030: 1800 0000 0801 0a02 0a01 0e01 1002 0201  ................
+00001040: 0a01 04ff 0802 0c01 0402 0c02 7a17 456e  ............z.En
+00001050: 7669 726f 6e6d 656e 742e 5f5f 6765 7469  vironment.__geti
+00001060: 7465 6d5f 5f29 0ada 085f 5f6e 616d 655f  tem__)...__name_
+00001070: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00001080: 5f71 7561 6c6e 616d 655f 5f72 2300 0000  _qualname__r#...
+00001090: 7215 0000 0072 1200 0000 721c 0000 0072  r....r....r....r
+000010a0: 1b00 0000 7254 0000 00da 0d5f 5f63 6c61  ....rT.....__cla
+000010b0: 7373 6365 6c6c 5f5f 7221 0000 0072 2100  sscell__r!...r!.
+000010c0: 0000 7256 0000 0072 2200 0000 7203 0000  ..rV...r"...r...
+000010d0: 000c 0000 0073 0e00 0000 0800 0802 0829  .....s.........)
+000010e0: 080e 080c 081b 1444 7203 0000 0029 0872  .......Dr....).r
+000010f0: 3100 0000 7217 0000 0072 3c00 0000 7210  1...r....r<...r.
+00001100: 0000 00da 0469 7064 6272 4700 0000 723f  .....ipdbrG...r?
+00001110: 0000 0072 0300 0000 7221 0000 0072 2100  ...r....r!...r!.
+00001120: 0000 7221 0000 0072 2200 0000 da08 3c6d  ..r!...r".....<m
+00001130: 6f64 756c 653e 0100 0000 730e 0000 0008  odule>....s.....
+00001140: 0108 0108 0108 0108 0104 0314 03         .............
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/__pycache__/mate.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/__pycache__/mate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Feb 13 21:08:56 2023 UTC, .py size: 7892 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,523 +1,517 @@
-00000000: 6f0d 0d0a 0000 0000 e8a6 ea63 d41e 0000  o..........c....
+00000000: 6f0d 0d0a 0000 0000 e7c6 3164 951e 0000  o.........1d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
+00000020: 0003 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a04 6400 6403 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6401 6c07 5a07 6400 6401 6c08 5a08 6404  d.l.Z.d.d.l.Z.d.
 00000070: 6405 6c09 6d09 5a09 0100 6400 6401 6c0a  d.l.m.Z...d.d.l.
-00000080: 5a0a 6400 6406 6c0b 6d0c 5a0c 0100 6404  Z.d.d.l.m.Z...d.
-00000090: 6407 6c0d 6d0e 5a0e 0100 4700 6408 6409  d.l.m.Z...G.d.d.
-000000a0: 8400 6409 8302 5a0f 6401 5300 290a e900  ..d...Z.d.S.)...
-000000b0: 0000 004e 2901 da02 696f 2901 da07 4d61  ...N)...io)...Ma
-000000c0: 7465 4150 49e9 0100 0000 2901 da05 7574  teAPI.....)...ut
-000000d0: 696c 7329 01da 084f 7074 696f 6e61 6c29  ils)...Optional)
-000000e0: 01da 0a4d 6174 6543 6f6e 6669 6763 0000  ...MateConfigc..
-000000f0: 0000 0000 0000 0000 0000 0000 0000 0600  ................
-00000100: 0000 4000 0000 73c0 0000 0065 005a 0164  ..@...s....e.Z.d
-00000110: 005a 0264 015a 0364 2864 0364 0484 015a  .Z.d.Z.d(d.d...Z
-00000120: 0465 0564 0565 0666 0264 0664 0784 0483  .e.d.e.f.d.d....
-00000130: 015a 0764 0864 0984 005a 0809 0a09 0b64  .Z.d.d...Z.....d
-00000140: 2964 0c65 0664 0d65 0966 0464 0e64 0f84  )d.e.d.e.f.d.d..
-00000150: 055a 0a64 1065 0666 0264 1164 1284 045a  .Z.d.e.f.d.d...Z
-00000160: 0b64 1364 1484 005a 0c64 1565 0664 1665  .d.d...Z.d.e.d.e
-00000170: 0664 1765 0666 0664 1864 1984 045a 0d64  .d.e.f.d.d...Z.d
-00000180: 1a65 0666 0264 1b64 1c84 045a 0e64 1d65  .e.f.d.d...Z.d.e
-00000190: 0664 1e65 0666 0464 1f64 2084 045a 0f64  .d.e.f.d.d ..Z.d
-000001a0: 1d65 0664 1e65 0666 0464 2164 2284 045a  .e.d.e.f.d!d"..Z
-000001b0: 1064 2365 0666 0264 2464 2584 045a 1164  .d#e.f.d$d%..Z.d
-000001c0: 2664 2784 005a 1264 0a53 0029 2ada 044d  &d'..Z.d.S.)*..M
-000001d0: 6174 657a 310a 2020 2020 4d61 7465 2c20  atez1.    Mate, 
-000001e0: 796f 7572 2066 7269 656e 646c 7920 4d4c  your friendly ML
-000001f0: 2070 726f 6a65 6374 206d 616e 6167 6572   project manager
-00000200: 2e0a 2020 2020 4663 0200 0000 0000 0000  ..    Fc........
-00000210: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-00000220: 733e 0000 0064 017c 005f 0064 017c 005f  s>...d.|._.d.|._
-00000230: 0174 026a 03a0 0474 05a1 017c 005f 0664  .t.j...t...|._.d
-00000240: 007c 005f 077c 00a0 08a1 0001 0074 097c  .|._.|.......t.|
-00000250: 006a 0783 017c 005f 0a64 007c 005f 0b64  .j...|._.d.|._.d
-00000260: 0053 0029 024e da00 290c da0b 726f 6f74  .S.).N..)...root
-00000270: 5f66 6f6c 6465 72da 0973 6176 655f 7061  _folder..save_pa
-00000280: 7468 da02 6f73 da04 7061 7468 da07 6469  th..os..path..di
-00000290: 726e 616d 65da 085f 5f66 696c 655f 5f5a  rname..__file__Z
-000002a0: 0e63 7572 7265 6e74 5f66 6f6c 6465 72da  .current_folder.
-000002b0: 0663 6f6e 6669 67da 0f5f 4d61 7465 5f5f  .config.._Mate__
-000002c0: 6669 6e64 726f 6f74 7203 0000 00da 0361  findrootr......a
-000002d0: 7069 5a0a 7275 6e5f 7061 7261 6d73 2902  piZ.run_params).
-000002e0: da04 7365 6c66 da04 696e 6974 a900 7215  ..self..init..r.
-000002f0: 0000 00fa 342f 686f 6d65 2f61 6c2f 4769  ....4/home/al/Gi
-00000300: 7468 7562 2f79 6572 6261 6d61 7465 2f70  thub/yerbamate/p
-00000310: 6163 6b61 6765 732f 7965 7262 616d 6174  ackages/yerbamat
-00000320: 652f 6d61 7465 2e70 79da 085f 5f69 6e69  e/mate.py..__ini
-00000330: 745f 5f16 0000 0073 0e00 0000 0601 0601  t__....s........
-00000340: 0e01 0601 0801 0c01 0a01 7a0d 4d61 7465  ..........z.Mate
-00000350: 2e5f 5f69 6e69 745f 5fda 0c70 726f 6a65  .__init__..proje
-00000360: 6374 5f6e 616d 6563 0100 0000 0000 0000  ct_namec........
-00000370: 0000 0000 0300 0000 0400 0000 4f00 0000  ............O...
-00000380: 731c 0000 0074 006a 017c 0067 017c 01a2  s....t.j.|.g.|..
-00000390: 0152 0069 007c 02a4 018e 0101 0064 0153  .R.i.|.......d.S
-000003a0: 0029 0261 df01 0000 0a0a 2020 2020 2020  .).a......      
-000003b0: 2020 606d 6174 6520 696e 6974 207b 7072    `mate init {pr
-000003c0: 6f6a 6563 745f 6e61 6d65 7d60 0a0a 2020  oject_name}`..  
-000003d0: 2020 2020 2020 496e 6974 6961 6c69 7a65        Initialize
-000003e0: 7320 6120 6e65 7720 7072 6f6a 6563 742e  s a new project.
-000003f0: 0a20 2020 2020 2020 2054 6869 7320 7769  .        This wi
-00000400: 6c6c 2063 7265 6174 6520 7468 6520 666f  ll create the fo
-00000410: 6c6c 6f77 696e 6720 7374 7275 6374 7572  llowing structur
-00000420: 653a 0a20 2020 2020 2020 2060 6060 0a20  e:.        ```. 
-00000430: 2020 2020 2020 202f 0a20 2020 2020 2020         /.       
-00000440: 207c 2d2d 206d 6f64 656c 732f 0a20 2020   |-- models/.   
-00000450: 2020 2020 207c 2020 207c 2d2d 205f 5f69       |   |-- __i
-00000460: 6e69 745f 5f2e 7079 0a20 2020 2020 2020  nit__.py.       
-00000470: 207c 2d2d 2065 7870 6572 696d 656e 7473   |-- experiments
-00000480: 2f0a 2020 2020 2020 2020 7c20 2020 7c2d  /.        |   |-
-00000490: 2d20 5f5f 696e 6974 5f5f 2e70 790a 2020  - __init__.py.  
-000004a0: 2020 2020 2020 7c2d 2d20 7472 6169 6e65        |-- traine
-000004b0: 7273 2f0a 2020 2020 2020 2020 7c20 2020  rs/.        |   
-000004c0: 7c2d 2d20 5f5f 696e 6974 5f5f 2e70 790a  |-- __init__.py.
-000004d0: 2020 2020 2020 2020 7c2d 2d20 6461 7461          |-- data
-000004e0: 2f0a 2020 2020 2020 2020 7c20 2020 7c2d  /.        |   |-
-000004f0: 2d20 5f5f 696e 6974 5f5f 2e70 790a 2020  - __init__.py.  
-00000500: 2020 2020 2020 6060 600a 0a20 2020 2020        ```..     
-00000510: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00000520: 2020 2020 2070 726f 6a65 6374 5f6e 616d       project_nam
-00000530: 653a 204e 616d 6520 6f66 2074 6865 2070  e: Name of the p
-00000540: 726f 6a65 6374 2e0a 0a20 2020 2020 2020  roject...       
-00000550: 2045 7861 6d70 6c65 3a0a 0a20 2020 2020   Example:..     
-00000560: 2020 2020 2020 2060 6d61 7465 2069 6e69         `mate ini
-00000570: 7420 6d79 5f70 726f 6a65 6374 600a 0a20  t my_project`.. 
-00000580: 2020 2020 2020 204e 2902 7203 0000 005a         N).r....Z
-00000590: 0c69 6e69 745f 7072 6f6a 6563 7429 0372  .init_project).r
-000005a0: 1800 0000 da04 6172 6773 da06 6b77 6172  ......args..kwar
-000005b0: 6773 7215 0000 0072 1500 0000 7216 0000  gsr....r....r...
-000005c0: 0072 1400 0000 1f00 0000 7302 0000 001c  .r........s.....
-000005d0: 1c7a 094d 6174 652e 696e 6974 6301 0000  .z.Mate.initc...
-000005e0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-000005f0: 0043 0000 0073 1000 0000 7c00 6a00 a001  .C...s....|.j...
-00000600: 6401 a101 0100 6402 5300 2903 612b 0200  d.....d.S.).a+..
-00000610: 000a 2020 2020 2020 2020 4765 6e65 7261  ..        Genera
-00000620: 7465 7320 7265 7175 6972 656d 656e 7473  tes requirements
-00000630: 2e74 7874 2c20 6465 7065 6e64 656e 6369  .txt, dependenci
-00000640: 6573 2e6a 736f 6e20 616e 6420 6578 706f  es.json and expo
-00000650: 7274 732e 6d64 2066 6f72 2073 6861 7269  rts.md for shari
-00000660: 6e67 2061 6e64 2072 6570 726f 6475 6369  ng and reproduci
-00000670: 6269 6c69 7479 2e0a 0a20 2020 2020 2020  bility...       
-00000680: 2045 7861 6d70 6c65 3a0a 2020 2020 2020   Example:.      
-00000690: 2020 2020 2020 606d 6174 6520 6578 706f        `mate expo
-000006a0: 7274 600a 0a20 2020 2020 2020 204f 7574  rt`..        Out
-000006b0: 7075 743a 0a20 2020 2020 2020 2020 2020  put:.           
-000006c0: 2060 6060 0a20 2020 2020 2020 2020 2020   ```.           
-000006d0: 2047 656e 6572 6174 6564 2072 6571 7569   Generated requi
-000006e0: 7265 6d65 6e74 732e 7478 7420 666f 7220  rements.txt for 
-000006f0: 6761 6e2f 6d6f 6465 6c73 2f6c 6761 6e0a  gan/models/lgan.
-00000700: 2020 2020 2020 2020 2020 2020 4765 6e65              Gene
-00000710: 7261 7465 6420 6465 7065 6e64 656e 6369  rated dependenci
-00000720: 6573 2e6a 736f 6e20 666f 7220 6761 6e2f  es.json for gan/
-00000730: 6578 7065 7269 6d65 6e74 732f 6c77 6761  experiments/lwga
-00000740: 6e0a 2020 2020 2020 2020 2020 2020 4765  n.            Ge
-00000750: 6e65 7261 7465 6420 7265 7175 6972 656d  nerated requirem
-00000760: 656e 7473 2e74 7874 2066 6f72 2067 616e  ents.txt for gan
-00000770: 2f65 7870 6572 696d 656e 7473 2f6c 7767  /experiments/lwg
-00000780: 616e 0a20 2020 2020 2020 2020 2020 2047  an.            G
-00000790: 656e 6572 6174 6564 2072 6571 7569 7265  enerated require
-000007a0: 6d65 6e74 732e 7478 7420 666f 7220 6761  ments.txt for ga
-000007b0: 6e2f 7472 6169 6e65 7273 2f6c 6761 6e0a  n/trainers/lgan.
-000007c0: 2020 2020 2020 2020 2020 2020 4765 6e65              Gene
-000007d0: 7261 7465 6420 7265 7175 6972 656d 656e  rated requiremen
-000007e0: 7473 2e74 7874 2066 6f72 2067 616e 2f64  ts.txt for gan/d
-000007f0: 6174 612f 6361 7273 0a20 2020 2020 2020  ata/cars.       
-00000800: 2020 2020 2045 7870 6f72 7465 6420 746f       Exported to
-00000810: 2065 7870 6f72 742e 6d64 0a20 2020 2020   export.md.     
-00000820: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00000830: 2020 200a 2020 2020 2020 2020 da06 6578     .        ..ex
-00000840: 706f 7274 4ea9 0272 1200 0000 da04 6175  portN..r......au
-00000850: 746f a901 7213 0000 0072 1500 0000 7215  to..r....r....r.
-00000860: 0000 0072 1600 0000 721b 0000 003d 0000  ...r....r....=..
-00000870: 00f3 0200 0000 1012 7a0b 4d61 7465 2e65  ........z.Mate.e
-00000880: 7870 6f72 744e 54da 0b6d 6f64 756c 655f  xportNT..module_
-00000890: 6e61 6d65 da0b 6f75 7470 7574 5f6a 736f  name..output_jso
-000008a0: 6e63 0300 0000 0000 0000 0000 0000 0400  nc..............
-000008b0: 0000 0500 0000 4300 0000 7332 0000 007c  ......C...s2...|
-000008c0: 006a 00a0 017c 01a1 017d 037c 0272 1374  .j...|...}.|.r.t
-000008d0: 0274 036a 047c 0364 0164 028d 0283 0101  .t.j.|.d.d......
-000008e0: 0064 0353 0074 027c 0383 0101 0064 0353  .d.S.t.|.....d.S
-000008f0: 0029 047a ee0a 0a0a 2020 2020 2020 2020  .).z....        
-00000900: 4c69 7374 7320 616c 6c20 6176 6169 6c61  Lists all availa
-00000910: 626c 6520 6d6f 6475 6c65 732e 0a0a 2020  ble modules...  
-00000920: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00000930: 2020 2020 2020 2020 6d6f 6475 6c65 5f6e          module_n
-00000940: 616d 653a 204e 616d 6520 6f66 2074 6865  ame: Name of the
-00000950: 206d 6f64 756c 6520 746f 206c 6973 742e   module to list.
-00000960: 2049 6620 6e6f 7420 7370 6563 6966 6965   If not specifie
-00000970: 642c 2061 6c6c 206d 6f64 756c 6573 2077  d, all modules w
-00000980: 696c 6c20 6265 206c 6973 7465 642e 0a0a  ill be listed...
-00000990: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
-000009a0: 3a0a 2020 2020 2020 2020 2020 2020 606d  :.            `m
-000009b0: 6174 6520 6c69 7374 206d 6f64 656c 7360  ate list models`
-000009c0: 0a0a 2020 2020 2020 2020 2020 2020 606d  ..            `m
-000009d0: 6174 6520 6c69 7374 600a 0a20 2020 2020  ate list`..     
-000009e0: 2020 20e9 0400 0000 a901 da06 696e 6465     .........inde
-000009f0: 6e74 4e29 0572 1200 0000 da04 6c69 7374  ntN).r......list
-00000a00: da05 7072 696e 74da 046a 736f 6eda 0564  ..print..json..d
-00000a10: 756d 7073 2904 7213 0000 0072 2000 0000  umps).r....r ...
-00000a20: 7221 0000 00da 026c 6972 1500 0000 7215  r!.....lir....r.
-00000a30: 0000 0072 1600 0000 7225 0000 0051 0000  ...r....r%...Q..
-00000a40: 0073 0800 0000 0c14 0401 1601 0c02 7a09  .s............z.
-00000a50: 4d61 7465 2e6c 6973 74da 0763 6f6d 6d61  Mate.list..comma
-00000a60: 6e64 6302 0000 0000 0000 0000 0000 0002  ndc.............
-00000a70: 0000 0003 0000 0043 0000 0073 1000 0000  .......C...s....
-00000a80: 7c00 6a00 a001 7c01 a101 0100 6401 5300  |.j...|.....d.S.
-00000a90: 2902 618e 0100 000a 0a20 2020 2020 2020  ).a......       
-00000aa0: 2060 6d61 7465 2061 7574 6f20 7b63 6f6d   `mate auto {com
-00000ab0: 6d61 6e64 7d60 0a0a 2020 2020 2020 2020  mand}`..        
-00000ac0: 5661 7269 6f75 7320 636f 6d6d 616e 6473  Various commands
-00000ad0: 2074 6f20 6865 6c70 2077 6974 6820 7468   to help with th
-00000ae0: 6520 6465 7665 6c6f 706d 656e 7420 7072  e development pr
-00000af0: 6f63 6573 732e 0a0a 0a20 2020 2020 2020  ocess....       
-00000b00: 2063 6f6d 6d61 6e64 733a 0a20 2020 2020   commands:.     
-00000b10: 2020 202d 2060 6578 706f 7274 603a 2043     - `export`: C
-00000b20: 7265 6174 6573 2061 2072 6571 7569 7265  reates a require
-00000b30: 6d65 6e74 732e 7478 7420 616e 6420 6465  ments.txt and de
-00000b40: 7065 6e64 656e 6369 6573 2e6a 736f 6e20  pendencies.json 
-00000b50: 6669 6c65 7320 666f 7220 7368 6172 696e  files for sharin
-00000b60: 6720 616e 6420 7265 7072 6f64 7563 6962  g and reproducib
-00000b70: 696c 6974 792e 0a20 2020 2020 2020 202d  ility..        -
-00000b80: 2060 696e 6974 603a 2041 7574 6f6d 6174   `init`: Automat
-00000b90: 6963 616c 6c79 2063 7265 6174 6573 2060  ically creates `
-00000ba0: 5f5f 696e 6974 5f5f 2e70 7960 2066 696c  __init__.py` fil
-00000bb0: 6573 2069 6e20 7468 6520 7072 6f6a 6563  es in the projec
-00000bc0: 7420 7374 7275 6374 7572 652e 0a0a 2020  t structure...  
-00000bd0: 2020 2020 2020 4578 616d 706c 653a 0a0a        Example:..
-00000be0: 0a20 2020 2020 2020 2020 2020 2060 6d61  .            `ma
-00000bf0: 7465 2061 7574 6f20 6578 706f 7274 600a  te auto export`.
-00000c00: 2020 2020 2020 2020 2020 2020 606d 6174              `mat
-00000c10: 6520 6175 746f 2069 6e69 7460 0a20 2020  e auto init`.   
-00000c20: 2020 2020 204e 721c 0000 0029 0272 1300       Nr....).r..
-00000c30: 0000 722a 0000 0072 1500 0000 7215 0000  ..r*...r....r...
-00000c40: 0072 1600 0000 721d 0000 006b 0000 0072  .r....r....k...r
-00000c50: 1f00 0000 7a09 4d61 7465 2e61 7574 6f63  ....z.Mate.autoc
-00000c60: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000c70: 0500 0000 4300 0000 731c 0000 0074 0074  ....C...s....t.t
-00000c80: 016a 027c 006a 03a0 04a1 0064 0164 028d  .j.|.j.....d.d..
-00000c90: 0283 0101 0064 0353 0029 047a 4e0a 2020  .....d.S.).zN.  
-00000ca0: 2020 2020 2020 5072 696e 7473 2061 2073        Prints a s
-00000cb0: 756d 6d61 7279 206f 6620 7468 6520 7072  ummary of the pr
-00000cc0: 6f6a 6563 7420 6d6f 6475 6c65 732e 2053  oject modules. S
-00000cd0: 616d 6520 6173 2060 6d61 7465 206c 6973  ame as `mate lis
-00000ce0: 7460 0a20 2020 2020 2020 2072 2200 0000  t`.        r"...
-00000cf0: 7223 0000 004e 2905 7226 0000 0072 2700  r#...N).r&...r'.
-00000d00: 0000 7228 0000 0072 1200 0000 da07 7375  ..r(...r......su
-00000d10: 6d6d 6172 7972 1e00 0000 7215 0000 0072  mmaryr....r....r
-00000d20: 1500 0000 7216 0000 0072 2b00 0000 7f00  ....r....r+.....
-00000d30: 0000 7302 0000 001c 057a 0c4d 6174 652e  ..s......z.Mate.
-00000d40: 7375 6d6d 6172 79da 066d 6f64 756c 65da  summary..module.
-00000d50: 046e 616d 65da 0464 6573 7463 0400 0000  .name..destc....
-00000d60: 0000 0000 0000 0000 0900 0000 0700 0000  ................
-00000d70: 4f00 0000 73ec 0000 0074 006a 01a0 027c  O...s....t.j...|
-00000d80: 006a 037c 017c 02a1 037d 0674 006a 01a0  .j.|.|...}.t.j..
-00000d90: 047c 06a1 0173 1f74 0564 017c 019b 0064  .|...s.t.d.|...d
-00000da0: 027c 029b 0064 039d 0583 0101 0074 06a0  .|...d.......t..
-00000db0: 0764 04a1 0101 0074 006a 01a0 027c 006a  .d.....t.j...|.j
-00000dc0: 037c 017c 03a1 037d 0774 006a 01a0 047c  .|.|...}.t.j...|
-00000dd0: 07a1 0172 6164 057c 0476 0072 3f74 08a0  ...rad.|.v.r?t..
-00000de0: 097c 07a1 0101 0074 0564 067c 079b 009d  .|.....t.d.|....
-00000df0: 0283 0101 006e 2274 0564 077c 039b 0064  .....n"t.d.|...d
-00000e00: 089d 0383 0101 0074 0a64 0983 017d 087c  .......t.d...}.|
-00000e10: 0864 0a6b 0272 5c74 08a0 097c 07a1 0101  .d.k.r\t...|....
-00000e20: 0074 0564 067c 079b 009d 0283 0101 006e  .t.d.|.........n
-00000e30: 0574 06a0 0764 04a1 0101 0074 08a0 0b7c  .t...d.....t...|
-00000e40: 067c 07a1 0201 0074 0564 017c 019b 0064  .|.....t.d.|...d
-00000e50: 027c 029b 0064 0b7c 079b 009d 0683 0101  .|...d.|........
-00000e60: 0064 0c53 0029 0d61 8a01 0000 0a20 2020  .d.S.).a.....   
-00000e70: 2020 2020 2060 6d61 7465 2063 6c6f 6e65       `mate clone
-00000e80: 207b 6d6f 6475 6c65 7d20 7b6e 616d 657d   {module} {name}
-00000e90: 207b 6465 7374 7d20 7b2d 6f7d 600a 0a20   {dest} {-o}`.. 
-00000ea0: 2020 2020 2020 2043 6c6f 6e65 7320 6120         Clones a 
-00000eb0: 736f 7572 6365 2063 6f64 6520 6d6f 6475  source code modu
-00000ec0: 6c65 2074 6f20 6120 6e65 7720 6465 7374  le to a new dest
-00000ed0: 696e 6174 696f 6e2e 0a0a 2020 2020 2020  ination...      
-00000ee0: 2020 4172 6773 3a0a 0a20 2020 2020 2020    Args:..       
-00000ef0: 2020 2020 206d 6f64 756c 653a 204d 6f64       module: Mod
-00000f00: 756c 6520 746f 2063 6c6f 6e65 2e0a 0a20  ule to clone... 
-00000f10: 2020 2020 2020 2020 2020 206e 616d 653a             name:
-00000f20: 204e 616d 6520 6f66 2074 6865 206d 6f64   Name of the mod
-00000f30: 756c 6520 746f 2063 6c6f 6e65 2e0a 0a20  ule to clone... 
-00000f40: 2020 2020 2020 2020 2020 2064 6573 743a             dest:
-00000f50: 2044 6573 7469 6e61 7469 6f6e 2074 6f20   Destination to 
-00000f60: 636c 6f6e 6520 7468 6520 6d6f 6475 6c65  clone the module
-00000f70: 2074 6f2e 0a0a 2020 2020 2020 2020 2020   to...          
-00000f80: 2020 2d6f 3a20 4f76 6572 7772 6974 6520    -o: Overwrite 
-00000f90: 6465 7374 696e 6174 696f 6e20 6966 2069  destination if i
-00000fa0: 7420 6578 6973 7473 2e0a 0a20 2020 2020  t exists...     
-00000fb0: 2020 2045 7861 6d70 6c65 3a0a 0a20 2020     Example:..   
-00000fc0: 2020 2020 2020 2020 2060 6d61 7465 2063           `mate c
-00000fd0: 6c6f 6e65 206d 6f64 656c 7320 746f 7263  lone models torc
-00000fe0: 685f 7669 7420 6d79 5f76 6974 600a 2020  h_vit my_vit`.  
-00000ff0: 2020 2020 2020 7a07 4d6f 6475 6c65 20fa        z.Module .
-00001000: 012f 7a0f 2064 6f65 7320 6e6f 7420 6578  ./z. does not ex
-00001010: 6973 7472 0400 0000 7a02 2d6f 7a08 5265  istr....z.-oz.Re
-00001020: 6d6f 7665 6420 7a0c 4465 7374 696e 6174  moved z.Destinat
-00001030: 696f 6e20 7a07 2065 7869 7374 737a 124f  ion z. existsz.O
-00001040: 7665 7277 7269 7465 3f20 2879 2f6e 293a  verwrite? (y/n):
-00001050: 20da 0179 7a0b 2063 6c6f 6e65 6420 746f   ..yz. cloned to
-00001060: 204e 290c 720c 0000 0072 0d00 0000 da04   N).r....r......
-00001070: 6a6f 696e 720a 0000 00da 0665 7869 7374  joinr......exist
-00001080: 7372 2600 0000 da03 7379 73da 0465 7869  sr&.....sys..exi
-00001090: 74da 0673 6875 7469 6cda 0672 6d74 7265  t..shutil..rmtre
-000010a0: 65da 0569 6e70 7574 da08 636f 7079 7472  e..input..copytr
-000010b0: 6565 2909 7213 0000 0072 2c00 0000 722d  ee).r....r,...r-
-000010c0: 0000 0072 2e00 0000 7219 0000 0072 1a00  ...r....r....r..
-000010d0: 0000 da0b 6d6f 6475 6c65 5f70 6174 685a  ....module_pathZ
-000010e0: 0964 6573 745f 7061 7468 da09 6f76 6572  .dest_path..over
-000010f0: 7772 6974 6572 1500 0000 7215 0000 0072  writer....r....r
-00001100: 1600 0000 da05 636c 6f6e 6586 0000 0073  ......clone....s
-00001110: 2200 0000 1216 0c01 1601 0a01 1203 0c01  "...............
-00001120: 0802 0a01 1001 1002 0801 0801 0a01 1001  ................
-00001130: 0a02 0c03 1e02 7a0a 4d61 7465 2e63 6c6f  ......z.Mate.clo
-00001140: 6e65 da0a 6d6f 6465 6c5f 6e61 6d65 6302  ne..model_namec.
-00001150: 0000 0000 0000 0000 0000 0002 0000 0001  ................
-00001160: 0000 0043 0000 0073 0400 0000 6400 5300  ...C...s....d.S.
-00001170: 2901 4e72 1500 0000 2902 7213 0000 0072  ).Nr....).r....r
-00001180: 3c00 0000 7215 0000 0072 1500 0000 7216  <...r....r....r.
-00001190: 0000 00da 0873 6e61 7073 686f 74b6 0000  .....snapshot...
-000011a0: 0073 0200 0000 0401 7a0d 4d61 7465 2e73  .s......z.Mate.s
-000011b0: 6e61 7073 686f 74da 0a65 7870 5f6d 6f64  napshot..exp_mod
-000011c0: 756c 65da 0365 7870 6303 0000 0000 0000  ule..expc.......
-000011d0: 0000 0000 0007 0000 000a 0000 004f 0000  .............O..
-000011e0: 0073 8800 0000 7c00 6a00 6a01 6401 7c01  .s....|.j.j.d.|.
-000011f0: 7c02 6704 7d05 6402 a002 7c05 a101 7d05  |.g.}.d...|...}.
-00001200: 7a07 7403 7c05 8301 0100 5700 6407 5300  z.t.|.....W.d.S.
-00001210: 0400 7404 7943 0100 7d06 0100 7a23 7405  ..t.yC..}...z#t.
-00001220: 6403 7c01 9b00 6404 7c02 9b00 9d04 8301  d.|...d.|.......
-00001230: 0100 7405 6405 8301 0100 7c00 a006 6401  ..t.d.....|...d.
-00001240: a101 0100 7407 a008 a100 0100 7409 a00a  ....t.......t...
-00001250: 6406 a101 0100 5700 5900 6407 7d06 7e06  d.....W.Y.d.}.~.
-00001260: 6407 5300 6407 7d06 7e06 7701 7700 2908  d.S.d.}.~.w.w.).
-00001270: 61e0 0100 000a 2020 2020 2020 2020 4578  a.....        Ex
-00001280: 6563 7574 6573 2061 6e20 6578 7065 7269  ecutes an experi
-00001290: 6d65 6e74 2e0a 0a20 2020 2020 2020 2055  ment...        U
-000012a0: 7361 6765 3a20 6060 6d61 7465 2074 7261  sage: ``mate tra
-000012b0: 696e 207b 6d6f 6475 6c65 7d20 7b65 7870  in {module} {exp
-000012c0: 6572 696d 656e 747d 6060 0a0a 2020 2020  eriment}``..    
-000012d0: 2020 2020 4172 6773 3a0a 0a20 2020 2020      Args:..     
-000012e0: 2020 2020 2020 2065 7870 5f6d 6f64 756c         exp_modul
-000012f0: 653a 204e 616d 6520 6f66 2074 6865 206d  e: Name of the m
-00001300: 6f64 756c 6520 7768 6572 6520 7468 6520  odule where the 
-00001310: 6578 7065 7269 6d65 6e74 2069 7320 6c6f  experiment is lo
-00001320: 6361 7465 642e 0a0a 2020 2020 2020 2020  cated...        
-00001330: 2020 2020 6578 703a 204e 616d 6520 6f66      exp: Name of
-00001340: 2074 6865 2065 7870 6572 696d 656e 742e   the experiment.
-00001350: 0a0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
-00001360: 653a 0a20 2020 2020 2020 2020 2020 2060  e:.            `
-00001370: 0a20 2020 2020 2020 2020 2020 206d 6174  .            mat
-00001380: 6520 7472 6169 6e20 6578 7065 7269 6d65  e train experime
-00001390: 6e74 7320 6d79 5f65 7870 6572 696d 656e  nts my_experimen
-000013a0: 7460 0a0a 2020 2020 2020 2020 5468 6973  t`..        This
-000013b0: 2077 696c 6c20 7275 6e20 7468 6520 6578   will run the ex
-000013c0: 7065 7269 6d65 6e74 2060 6d79 5f65 7870  periment `my_exp
-000013d0: 6572 696d 656e 7460 206c 6f63 6174 6564  eriment` located
-000013e0: 2069 6e20 7468 6520 6065 7870 6572 696d   in the `experim
-000013f0: 656e 7473 6020 6d6f 6475 6c65 2e0a 0a20  ents` module... 
-00001400: 2020 2020 2020 2045 7175 6976 616c 656e         Equivalen
-00001410: 7420 746f 2060 7079 7468 6f6e 202d 6d20  t to `python -m 
-00001420: 726f 6f74 5f6d 6f64 756c 652e 6578 7065  root_module.expe
-00001430: 7269 6d65 6e74 732e 6d79 5f65 7870 6572  riments.my_exper
-00001440: 696d 656e 7420 7472 6169 6e60 0a20 2020  iment train`.   
-00001450: 2020 2020 20da 0b65 7870 6572 696d 656e       ..experimen
-00001460: 7473 da01 2e7a 1145 7272 6f72 2069 6e20  ts...z.Error in 
-00001470: 6c6f 6164 696e 6720 722f 0000 007a 1641  loading r/...z.A
-00001480: 7661 696c 6162 6c65 2065 7870 6572 696d  vailable experim
-00001490: 656e 7473 3a72 0400 0000 4e29 0b72 1000  ents:r....N).r..
-000014a0: 0000 da07 7072 6f6a 6563 7472 3100 0000  ....projectr1...
-000014b0: da0a 5f5f 696d 706f 7274 5f5f da09 4578  ..__import__..Ex
-000014c0: 6365 7074 696f 6e72 2600 0000 7225 0000  ceptionr&...r%..
-000014d0: 00da 0974 7261 6365 6261 636b da09 7072  ...traceback..pr
-000014e0: 696e 745f 6578 6372 3300 0000 7234 0000  int_excr3...r4..
-000014f0: 0029 0772 1300 0000 723e 0000 0072 3f00  .).r....r>...r?.
-00001500: 0000 7219 0000 0072 1a00 0000 722c 0000  ..r....r....r,..
-00001510: 00da 0165 7215 0000 0072 1500 0000 7216  ...er....r....r.
-00001520: 0000 00da 0574 7261 696e b900 0000 7318  .....train....s.
-00001530: 0000 0010 160a 0102 020e 010e 0114 0108  ................
-00001540: 010a 0108 0118 0308 8002 f97a 0a4d 6174  ...........z.Mat
-00001550: 652e 7472 6169 6e63 0300 0000 0000 0000  e.trainc........
-00001560: 0000 0000 0500 0000 0400 0000 4f00 0000  ............O...
-00001570: 731e 0000 007c 006a 007c 017c 0267 027c  s....|.j.|.|.g.|
-00001580: 03a2 0152 0069 007c 04a4 018e 0101 0064  ...R.i.|.......d
-00001590: 0153 0029 0261 dd01 0000 0a20 2020 2020  .S.).a.....     
-000015a0: 2020 2045 7865 6375 7465 7320 616e 2065     Executes an e
-000015b0: 7870 6572 696d 656e 742e 0a0a 2020 2020  xperiment...    
-000015c0: 2020 2020 5573 6167 653a 2060 606d 6174      Usage: ``mat
-000015d0: 6520 7465 7374 207b 6d6f 6475 6c65 7d20  e test {module} 
-000015e0: 7b65 7870 6572 696d 656e 747d 6060 0a0a  {experiment}``..
-000015f0: 2020 2020 2020 2020 4172 6773 3a0a 0a20          Args:.. 
-00001600: 2020 2020 2020 2020 2020 2065 7870 5f6d             exp_m
-00001610: 6f64 756c 653a 204e 616d 6520 6f66 2074  odule: Name of t
-00001620: 6865 206d 6f64 756c 6520 7768 6572 6520  he module where 
-00001630: 7468 6520 6578 7065 7269 6d65 6e74 2069  the experiment i
-00001640: 7320 6c6f 6361 7465 642e 0a0a 2020 2020  s located...    
-00001650: 2020 2020 2020 2020 6578 703a 204e 616d          exp: Nam
-00001660: 6520 6f66 2074 6865 2065 7870 6572 696d  e of the experim
-00001670: 656e 742e 0a0a 2020 2020 2020 2020 4578  ent...        Ex
-00001680: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
-00001690: 2020 2060 0a20 2020 2020 2020 2020 2020     `.           
-000016a0: 206d 6174 6520 7465 7374 2065 7870 6572   mate test exper
-000016b0: 696d 656e 7473 206d 795f 6578 7065 7269  iments my_experi
-000016c0: 6d65 6e74 600a 0a20 2020 2020 2020 2054  ment`..        T
-000016d0: 6869 7320 7769 6c6c 2072 756e 2074 6865  his will run the
-000016e0: 2065 7870 6572 696d 656e 7420 606d 795f   experiment `my_
-000016f0: 6578 7065 7269 6d65 6e74 6020 6c6f 6361  experiment` loca
-00001700: 7465 6420 696e 2074 6865 2060 6578 7065  ted in the `expe
-00001710: 7269 6d65 6e74 7360 206d 6f64 756c 652e  riments` module.
-00001720: 0a0a 2020 2020 2020 2020 4571 7569 7661  ..        Equiva
-00001730: 6c65 6e74 2074 6f20 6070 7974 686f 6e20  lent to `python 
-00001740: 2d6d 2072 6f6f 745f 6d6f 6475 6c65 2e65  -m root_module.e
-00001750: 7870 6572 696d 656e 7473 2e6d 795f 6578  xperiments.my_ex
-00001760: 7065 7269 6d65 6e74 2074 6573 7460 0a20  periment test`. 
-00001770: 2020 2020 2020 204e 2901 7248 0000 0029         N).rH...)
-00001780: 0572 1300 0000 723e 0000 0072 3f00 0000  .r....r>...r?...
-00001790: 7219 0000 0072 1a00 0000 7215 0000 0072  r....r....r....r
-000017a0: 1500 0000 7216 0000 00da 0474 6573 74dd  ....r......test.
-000017b0: 0000 0073 0200 0000 1e14 7a09 4d61 7465  ...s......z.Mate
-000017c0: 2e74 6573 74da 0375 726c 6302 0000 0000  .test..urlc.....
-000017d0: 0000 0000 0000 0004 0000 0004 0000 004f  ...............O
-000017e0: 0000 0073 1e00 0000 7c00 6a00 6a01 7c01  ...s....|.j.j.|.
-000017f0: 6701 7c02 a201 5200 6900 7c03 a401 8e01  g.|...R.i.|.....
-00001800: 0100 6401 5300 2902 6169 0500 000a 2020  ..d.S.).ai....  
-00001810: 2020 2020 2020 496e 7461 6c6c 7320 6120        Intalls a 
-00001820: 6d6f 6475 6c65 2066 726f 6d20 6120 6769  module from a gi
-00001830: 7420 7265 706f 7369 746f 7279 2e0a 0a20  t repository... 
-00001840: 2020 2020 2020 2055 7361 6765 3a20 6060         Usage: ``
-00001850: 6d61 7465 2069 6e73 7461 6c6c 207b 7572  mate install {ur
-00001860: 6c7d 202d 7b79 7c6e 7c6f 7d20 7b70 6d7d  l} -{y|n|o} {pm}
-00001870: 6060 0a0a 2020 2020 2020 2020 496e 7374  ``..        Inst
-00001880: 616c 6c20 6d6f 6475 6c65 2073 7570 706f  all module suppo
-00001890: 7274 2074 6865 2066 6f6c 6c6f 7769 6e67  rt the following
-000018a0: 2066 6f72 6d61 7473 3a0a 2020 2020 2020   formats:.      
-000018b0: 2020 2d20 6060 6d61 7465 2069 6e73 7461    - ``mate insta
-000018c0: 6c6c 207b 636f 6d70 6c65 7465 5f75 726c  ll {complete_url
-000018d0: 7d60 600a 2020 2020 2020 2020 2d20 6060  }``.        - ``
-000018e0: 6d61 7465 2069 6e73 7461 6c6c 207b 7573  mate install {us
-000018f0: 6572 7d2f 7b72 6570 6f7d 2f7b 726f 6f74  er}/{repo}/{root
-00001900: 5f6d 6f64 756c 657d 2f7b 6d6f 6475 6c65  _module}/{module
-00001910: 7d60 600a 2020 2020 2020 2020 2d20 6060  }``.        - ``
-00001920: 6d61 7465 2069 6e73 7461 6c6c 207b 7573  mate install {us
-00001930: 6572 7d2f 7b72 6570 6f7c 726f 6f74 5f6d  er}/{repo|root_m
-00001940: 6f64 756c 657d 2f7b 6d6f 6475 6c65 7d60  odule}/{module}`
-00001950: 600a 0a20 2020 2020 2020 2041 7267 733a  `..        Args:
-00001960: 0a20 2020 2020 2020 202d 2020 2020 7572  .        -    ur
-00001970: 6c3a 2055 726c 206f 6620 7468 6520 6769  l: Url of the gi
-00001980: 7420 7265 706f 7369 746f 7279 2e0a 2020  t repository..  
-00001990: 2020 2020 2020 2d20 2020 202d 793a 2053        -    -y: S
-000019a0: 6b69 7073 2063 6f6e 6669 726d 6174 696f  kips confirmatio
-000019b0: 6e20 616e 6420 696e 7374 616c 6c73 2070  n and installs p
-000019c0: 7974 686f 6e20 6465 7065 6e64 656e 6369  ython dependenci
-000019d0: 6573 0a20 2020 2020 2020 202d 2020 2020  es.        -    
-000019e0: 2d6e 3a20 536b 6970 7320 696e 7374 616c  -n: Skips instal
-000019f0: 6c69 6e67 2070 7974 686f 6e20 6465 7065  ling python depe
-00001a00: 6e64 656e 6369 6573 0a20 2020 2020 2020  ndencies.       
-00001a10: 202d 2020 2020 2d6f 3a20 4f76 6572 7772   -    -o: Overwr
-00001a20: 6974 6573 2065 7869 7374 696e 6720 636f  ites existing co
-00001a30: 6465 206d 6f64 756c 6573 0a20 2020 2020  de modules.     
-00001a40: 2020 202d 2020 2020 706d 3a20 5061 636b     -    pm: Pack
-00001a50: 6167 6520 6d61 6e61 6765 7220 746f 2075  age manager to u
-00001a60: 7365 2e20 4465 6661 756c 7473 2074 6f20  se. Defaults to 
-00001a70: 6173 6b69 6e67 2074 6865 2075 7365 722e  asking the user.
-00001a80: 0a0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
-00001a90: 6520 496e 7374 616c 6c69 6e67 2061 206d  e Installing a m
-00001aa0: 6f64 756c 6520 6672 6f6d 2073 7472 7563  odule from struc
-00001ab0: 7475 7265 6420 6769 7420 7265 706f 7369  tured git reposi
-00001ac0: 746f 7279 2028 7265 636f 6d6d 656e 6465  tory (recommende
-00001ad0: 6429 3a0a 0a0a 2020 2020 2020 2020 2020  d):...          
-00001ae0: 2020 6d61 7465 2069 6e73 7461 6c6c 206f    mate install o
-00001af0: 616c 6565 2f64 6565 702d 7669 7369 6f6e  alee/deep-vision
-00001b00: 2f64 6565 706e 6574 2f6d 6f64 656c 732f  /deepnet/models/
-00001b10: 746f 7263 685f 7669 7420 2d79 6f20 7069  torch_vit -yo pi
-00001b20: 700a 0a20 2020 2020 2020 2020 2020 2054  p..            T
-00001b30: 6869 7320 7769 6c6c 2069 6e73 7461 6c6c  his will install
-00001b40: 2074 6865 206d 6f64 756c 6520 6074 6f72   the module `tor
-00001b50: 6368 5f76 6974 6020 6672 6f6d 2074 6865  ch_vit` from the
-00001b60: 2072 6570 6f73 6974 6f72 7920 606f 616c   repository `oal
-00001b70: 6565 2f64 6565 702d 7669 7369 6f6e 6020  ee/deep-vision` 
-00001b80: 696e 2074 6f20 796f 7572 2060 6d6f 6465  in to your `mode
-00001b90: 6c73 6020 666f 6c64 6572 2e0a 2020 2020  ls` folder..    
-00001ba0: 2020 2020 2020 2020 5468 6520 6079 6f60          The `yo`
-00001bb0: 2066 6c61 6773 2077 696c 6c20 736b 6970   flags will skip
-00001bc0: 2063 6f6e 6669 726d 6174 696f 6e20 616e   confirmation an
-00001bd0: 6420 696e 7374 616c 6c20 7079 7468 6f6e  d install python
-00001be0: 2064 6570 656e 6465 6e63 6965 7320 7573   dependencies us
-00001bf0: 696e 6720 7069 702e 0a0a 2020 2020 2020  ing pip...      
-00001c00: 2020 4578 616d 706c 6520 496e 7374 616c    Example Instal
-00001c10: 6c69 6e67 2061 206d 6f64 756c 6520 6672  ling a module fr
-00001c20: 6f6d 2075 6e73 7472 7563 7475 7265 6420  om unstructured 
-00001c30: 6769 7420 7265 706f 7369 746f 7279 3a0a  git repository:.
-00001c40: 0a0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
-00001c50: 7465 2069 6e73 7461 6c6c 2068 7474 7073  te install https
-00001c60: 3a2f 2f67 6974 6875 622e 636f 6d2f 7277  ://github.com/rw
-00001c70: 6967 6874 6d61 6e2f 7079 746f 7263 682d  ightman/pytorch-
-00001c80: 696d 6167 652d 6d6f 6465 6c73 2f74 7265  image-models/tre
-00001c90: 652f 6d61 696e 2f74 696d 6d0a 0a0a 2020  e/main/timm...  
-00001ca0: 2020 2020 2020 2020 2020 5468 6973 2077            This w
-00001cb0: 696c 6c20 696e 7374 616c 6c20 7468 6520  ill install the 
-00001cc0: 6d6f 6475 6c65 2060 7469 6d6d 6020 6672  module `timm` fr
-00001cd0: 6f6d 2074 6865 2072 6570 6f73 6974 6f72  om the repositor
-00001ce0: 7920 6173 2061 2073 6973 7465 7220 6d6f  y as a sister mo
-00001cf0: 6475 6c65 2074 6f20 796f 7572 2072 6f6f  dule to your roo
-00001d00: 7420 6d6f 6475 6c65 2e0a 2020 2020 2020  t module..      
-00001d10: 2020 2020 2020 5461 6b65 2069 6e74 6f20        Take into 
-00001d20: 6163 636f 756e 7420 7468 6174 2074 6869  account that thi
-00001d30: 7320 7769 6c6c 2069 6e73 7461 6c6c 206f  s will install o
-00001d40: 6e6c 7920 7468 6520 636f 6465 2061 6e64  nly the code and
-00001d50: 206e 6f74 2074 6865 2070 7974 686f 6e20   not the python 
-00001d60: 6465 7065 6e64 656e 6369 6573 2e0a 2020  dependencies..  
-00001d70: 2020 2020 2020 4e29 0272 1200 0000 5a0b        N).r....Z.
-00001d80: 696e 7374 616c 6c5f 7572 6c29 0472 1300  install_url).r..
-00001d90: 0000 724a 0000 0072 1900 0000 721a 0000  ..rJ...r....r...
-00001da0: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-00001db0: da07 696e 7374 616c 6cf3 0000 0073 0200  ..install....s..
-00001dc0: 0000 1e23 7a0c 4d61 7465 2e69 6e73 7461  ...#z.Mate.insta
-00001dd0: 6c6c 6301 0000 0000 0000 0000 0000 0001  llc.............
-00001de0: 0000 0003 0000 0043 0000 0073 1e00 0000  .......C...s....
-00001df0: 7400 a001 a100 5c02 7c00 5f02 7c00 5f03  t.....\.|._.|._.
-00001e00: 7c00 6a03 6a04 7c00 5f05 6401 5300 2902  |.j.j.|._.d.S.).
-00001e10: 7a71 0a20 2020 2020 2020 204d 6574 686f  zq.        Metho
-00001e20: 6420 696e 2063 6861 7267 6520 6f66 2066  d in charge of f
-00001e30: 696e 6469 6e67 2074 6865 2072 6f6f 7420  inding the root 
-00001e40: 666f 6c64 6572 206f 6620 7468 6520 7072  folder of the pr
-00001e50: 6f6a 6563 7420 616e 6420 7265 6164 696e  oject and readin
-00001e60: 6720 7468 6520 636f 6e74 656e 7420 6f66  g the content of
-00001e70: 206d 6174 652e 6a73 6f6e 0a20 2020 2020   mate.json.     
-00001e80: 2020 204e 2906 7202 0000 005a 0966 696e     N).r....Z.fin
-00001e90: 645f 726f 6f74 720a 0000 0072 1000 0000  d_rootr....r....
-00001ea0: da0e 7265 7375 6c74 735f 666f 6c64 6572  ..results_folder
-00001eb0: 5a10 726f 6f74 5f73 6176 655f 666f 6c64  Z.root_save_fold
-00001ec0: 6572 721e 0000 0072 1500 0000 7215 0000  err....r....r...
-00001ed0: 0072 1600 0000 5a0a 5f5f 6669 6e64 726f  .r....Z.__findro
-00001ee0: 6f74 1801 0000 7304 0000 0010 040e 017a  ot....s........z
-00001ef0: 0f4d 6174 652e 5f5f 6669 6e64 726f 6f74  .Mate.__findroot
-00001f00: 2901 4629 024e 5429 13da 085f 5f6e 616d  ).F).NT)...__nam
-00001f10: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00001f20: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
-00001f30: 5f64 6f63 5f5f 7217 0000 00da 0c73 7461  _doc__r......sta
-00001f40: 7469 636d 6574 686f 64da 0373 7472 7214  ticmethod..strr.
-00001f50: 0000 0072 1b00 0000 da04 626f 6f6c 7225  ...r......boolr%
-00001f60: 0000 0072 1d00 0000 722b 0000 0072 3b00  ...r....r+...r;.
-00001f70: 0000 723d 0000 0072 4800 0000 7249 0000  ..r=...rH...rI..
-00001f80: 0072 4b00 0000 7211 0000 0072 1500 0000  .rK...r....r....
-00001f90: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00001fa0: 0800 0000 1100 0000 732a 0000 0008 0004  ........s*......
-00001fb0: 010a 0402 0910 0108 1d02 1602 0104 fd02  ................
-00001fc0: 0202 fe02 030a fd0e 1a08 1416 070e 3012  ..............0.
-00001fd0: 0312 240e 160c 2572 0800 0000 2910 720c  ..$...%r....).r.
-00001fe0: 0000 0072 4500 0000 5a20 7965 7262 616d  ...rE...Z yerbam
-00001ff0: 6174 652e 6170 692e 6461 7461 2e73 6f75  ate.api.data.sou
-00002000: 7263 6573 2e6c 6f63 616c 7202 0000 0072  rces.localr....r
-00002010: 2700 0000 5a16 7965 7262 616d 6174 652e  '...Z.yerbamate.
-00002020: 6170 692e 6d61 7465 5f61 7069 7203 0000  api.mate_apir...
-00002030: 0072 3300 0000 da04 6970 6462 7205 0000  .r3.....ipdbr...
-00002040: 0072 3500 0000 da06 7479 7069 6e67 7206  .r5.....typingr.
-00002050: 0000 00da 0b6d 6174 655f 636f 6e66 6967  .....mate_config
-00002060: 7207 0000 0072 0800 0000 7215 0000 0072  r....r....r....r
-00002070: 1500 0000 7215 0000 0072 1600 0000 da08  ....r....r......
-00002080: 3c6d 6f64 756c 653e 0100 0000 7318 0000  <module>....s...
-00002090: 0008 0008 010c 0108 010c 0108 0208 020c  ................
-000020a0: 0108 010c 010c 0212 03                   .........
+00000080: 5a0a 6400 6406 6c0b 6d0c 5a0c 0100 4700  Z.d.d.l.m.Z...G.
+00000090: 6407 6408 8400 6408 8302 5a0d 6401 5300  d.d...d...Z.d.S.
+000000a0: 2909 e900 0000 004e 2901 da02 696f 2901  )......N)...io).
+000000b0: da07 4d61 7465 4150 49e9 0100 0000 2901  ..MateAPI.....).
+000000c0: da05 7574 696c 7329 01da 084f 7074 696f  ..utils)...Optio
+000000d0: 6e61 6c63 0000 0000 0000 0000 0000 0000  nalc............
+000000e0: 0000 0000 0600 0000 4000 0000 73c0 0000  ........@...s...
+000000f0: 0065 005a 0164 005a 0264 015a 0364 2864  .e.Z.d.Z.d.Z.d(d
+00000100: 0364 0484 015a 0465 0564 0565 0666 0264  .d...Z.e.d.e.f.d
+00000110: 0664 0784 0483 015a 0764 0864 0984 005a  .d.....Z.d.d...Z
+00000120: 0809 0a09 0b64 2964 0c65 0664 0d65 0966  .....d)d.e.d.e.f
+00000130: 0464 0e64 0f84 055a 0a64 1065 0666 0264  .d.d...Z.d.e.f.d
+00000140: 1164 1284 045a 0b64 1364 1484 005a 0c64  .d...Z.d.d...Z.d
+00000150: 1565 0664 1665 0664 1765 0666 0664 1864  .e.d.e.d.e.f.d.d
+00000160: 1984 045a 0d64 1a65 0666 0264 1b64 1c84  ...Z.d.e.f.d.d..
+00000170: 045a 0e64 1d65 0664 1e65 0666 0464 1f64  .Z.d.e.d.e.f.d.d
+00000180: 2084 045a 0f64 1d65 0664 1e65 0666 0464   ..Z.d.e.d.e.f.d
+00000190: 2164 2284 045a 1064 2365 0666 0264 2464  !d"..Z.d#e.f.d$d
+000001a0: 2584 045a 1164 2664 2784 005a 1264 0a53  %..Z.d&d'..Z.d.S
+000001b0: 0029 2ada 044d 6174 657a 310a 2020 2020  .)*..Matez1.    
+000001c0: 4d61 7465 2c20 796f 7572 2066 7269 656e  Mate, your frien
+000001d0: 646c 7920 4d4c 2070 726f 6a65 6374 206d  dly ML project m
+000001e0: 616e 6167 6572 2e0a 2020 2020 4663 0200  anager..    Fc..
+000001f0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00000200: 0000 4300 0000 733e 0000 0064 017c 005f  ..C...s>...d.|._
+00000210: 0064 017c 005f 0174 026a 03a0 0474 05a1  .d.|._.t.j...t..
+00000220: 017c 005f 0664 007c 005f 077c 00a0 08a1  .|._.d.|._.|....
+00000230: 0001 0074 097c 006a 0783 017c 005f 0a64  ...t.|.j...|._.d
+00000240: 007c 005f 0b64 0053 0029 024e da00 290c  .|._.d.S.).N..).
+00000250: da0b 726f 6f74 5f66 6f6c 6465 72da 0973  ..root_folder..s
+00000260: 6176 655f 7061 7468 da02 6f73 da04 7061  ave_path..os..pa
+00000270: 7468 da07 6469 726e 616d 65da 085f 5f66  th..dirname..__f
+00000280: 696c 655f 5f5a 0e63 7572 7265 6e74 5f66  ile__Z.current_f
+00000290: 6f6c 6465 72da 0663 6f6e 6669 67da 0f5f  older..config.._
+000002a0: 4d61 7465 5f5f 6669 6e64 726f 6f74 7203  Mate__findrootr.
+000002b0: 0000 00da 0361 7069 5a0a 7275 6e5f 7061  .....apiZ.run_pa
+000002c0: 7261 6d73 2902 da04 7365 6c66 da04 696e  rams)...self..in
+000002d0: 6974 a900 7214 0000 00fa 342f 686f 6d65  it..r.....4/home
+000002e0: 2f61 6c2f 4769 7448 7562 2f79 6572 6261  /al/GitHub/yerba
+000002f0: 6d61 7465 2f70 6163 6b61 6765 732f 7965  mate/packages/ye
+00000300: 7262 616d 6174 652f 6d61 7465 2e70 79da  rbamate/mate.py.
+00000310: 085f 5f69 6e69 745f 5f15 0000 0073 0e00  .__init__....s..
+00000320: 0000 0601 0601 0e01 0601 0801 0c01 0a01  ................
+00000330: 7a0d 4d61 7465 2e5f 5f69 6e69 745f 5fda  z.Mate.__init__.
+00000340: 0c70 726f 6a65 6374 5f6e 616d 6563 0100  .project_namec..
+00000350: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00000360: 0000 4f00 0000 731c 0000 0074 006a 017c  ..O...s....t.j.|
+00000370: 0067 017c 01a2 0152 0069 007c 02a4 018e  .g.|...R.i.|....
+00000380: 0101 0064 0153 0029 0261 df01 0000 0a0a  ...d.S.).a......
+00000390: 2020 2020 2020 2020 606d 6174 6520 696e          `mate in
+000003a0: 6974 207b 7072 6f6a 6563 745f 6e61 6d65  it {project_name
+000003b0: 7d60 0a0a 2020 2020 2020 2020 496e 6974  }`..        Init
+000003c0: 6961 6c69 7a65 7320 6120 6e65 7720 7072  ializes a new pr
+000003d0: 6f6a 6563 742e 0a20 2020 2020 2020 2054  oject..        T
+000003e0: 6869 7320 7769 6c6c 2063 7265 6174 6520  his will create 
+000003f0: 7468 6520 666f 6c6c 6f77 696e 6720 7374  the following st
+00000400: 7275 6374 7572 653a 0a20 2020 2020 2020  ructure:.       
+00000410: 2060 6060 0a20 2020 2020 2020 202f 0a20   ```.        /. 
+00000420: 2020 2020 2020 207c 2d2d 206d 6f64 656c         |-- model
+00000430: 732f 0a20 2020 2020 2020 207c 2020 207c  s/.        |   |
+00000440: 2d2d 205f 5f69 6e69 745f 5f2e 7079 0a20  -- __init__.py. 
+00000450: 2020 2020 2020 207c 2d2d 2065 7870 6572         |-- exper
+00000460: 696d 656e 7473 2f0a 2020 2020 2020 2020  iments/.        
+00000470: 7c20 2020 7c2d 2d20 5f5f 696e 6974 5f5f  |   |-- __init__
+00000480: 2e70 790a 2020 2020 2020 2020 7c2d 2d20  .py.        |-- 
+00000490: 7472 6169 6e65 7273 2f0a 2020 2020 2020  trainers/.      
+000004a0: 2020 7c20 2020 7c2d 2d20 5f5f 696e 6974    |   |-- __init
+000004b0: 5f5f 2e70 790a 2020 2020 2020 2020 7c2d  __.py.        |-
+000004c0: 2d20 6461 7461 2f0a 2020 2020 2020 2020  - data/.        
+000004d0: 7c20 2020 7c2d 2d20 5f5f 696e 6974 5f5f  |   |-- __init__
+000004e0: 2e70 790a 2020 2020 2020 2020 6060 600a  .py.        ```.
+000004f0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00000500: 2020 2020 2020 2020 2020 2070 726f 6a65             proje
+00000510: 6374 5f6e 616d 653a 204e 616d 6520 6f66  ct_name: Name of
+00000520: 2074 6865 2070 726f 6a65 6374 2e0a 0a20   the project... 
+00000530: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
+00000540: 0a20 2020 2020 2020 2020 2020 2060 6d61  .            `ma
+00000550: 7465 2069 6e69 7420 6d79 5f70 726f 6a65  te init my_proje
+00000560: 6374 600a 0a20 2020 2020 2020 204e 2902  ct`..        N).
+00000570: 7203 0000 005a 0c69 6e69 745f 7072 6f6a  r....Z.init_proj
+00000580: 6563 7429 0372 1700 0000 da04 6172 6773  ect).r......args
+00000590: da06 6b77 6172 6773 7214 0000 0072 1400  ..kwargsr....r..
+000005a0: 0000 7215 0000 0072 1300 0000 1e00 0000  ..r....r........
+000005b0: 7302 0000 001c 1c7a 094d 6174 652e 696e  s......z.Mate.in
+000005c0: 6974 6301 0000 0000 0000 0000 0000 0001  itc.............
+000005d0: 0000 0003 0000 0043 0000 0073 1000 0000  .......C...s....
+000005e0: 7c00 6a00 a001 6401 a101 0100 6402 5300  |.j...d.....d.S.
+000005f0: 2903 612b 0200 000a 2020 2020 2020 2020  ).a+....        
+00000600: 4765 6e65 7261 7465 7320 7265 7175 6972  Generates requir
+00000610: 656d 656e 7473 2e74 7874 2c20 6465 7065  ements.txt, depe
+00000620: 6e64 656e 6369 6573 2e6a 736f 6e20 616e  ndencies.json an
+00000630: 6420 6578 706f 7274 732e 6d64 2066 6f72  d exports.md for
+00000640: 2073 6861 7269 6e67 2061 6e64 2072 6570   sharing and rep
+00000650: 726f 6475 6369 6269 6c69 7479 2e0a 0a20  roducibility... 
+00000660: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
+00000670: 2020 2020 2020 2020 2020 2020 606d 6174              `mat
+00000680: 6520 6578 706f 7274 600a 0a20 2020 2020  e export`..     
+00000690: 2020 204f 7574 7075 743a 0a20 2020 2020     Output:.     
+000006a0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+000006b0: 2020 2020 2020 2047 656e 6572 6174 6564         Generated
+000006c0: 2072 6571 7569 7265 6d65 6e74 732e 7478   requirements.tx
+000006d0: 7420 666f 7220 6761 6e2f 6d6f 6465 6c73  t for gan/models
+000006e0: 2f6c 6761 6e0a 2020 2020 2020 2020 2020  /lgan.          
+000006f0: 2020 4765 6e65 7261 7465 6420 6465 7065    Generated depe
+00000700: 6e64 656e 6369 6573 2e6a 736f 6e20 666f  ndencies.json fo
+00000710: 7220 6761 6e2f 6578 7065 7269 6d65 6e74  r gan/experiment
+00000720: 732f 6c77 6761 6e0a 2020 2020 2020 2020  s/lwgan.        
+00000730: 2020 2020 4765 6e65 7261 7465 6420 7265      Generated re
+00000740: 7175 6972 656d 656e 7473 2e74 7874 2066  quirements.txt f
+00000750: 6f72 2067 616e 2f65 7870 6572 696d 656e  or gan/experimen
+00000760: 7473 2f6c 7767 616e 0a20 2020 2020 2020  ts/lwgan.       
+00000770: 2020 2020 2047 656e 6572 6174 6564 2072       Generated r
+00000780: 6571 7569 7265 6d65 6e74 732e 7478 7420  equirements.txt 
+00000790: 666f 7220 6761 6e2f 7472 6169 6e65 7273  for gan/trainers
+000007a0: 2f6c 6761 6e0a 2020 2020 2020 2020 2020  /lgan.          
+000007b0: 2020 4765 6e65 7261 7465 6420 7265 7175    Generated requ
+000007c0: 6972 656d 656e 7473 2e74 7874 2066 6f72  irements.txt for
+000007d0: 2067 616e 2f64 6174 612f 6361 7273 0a20   gan/data/cars. 
+000007e0: 2020 2020 2020 2020 2020 2045 7870 6f72             Expor
+000007f0: 7465 6420 746f 2065 7870 6f72 742e 6d64  ted to export.md
+00000800: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
+00000810: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000820: 2020 da06 6578 706f 7274 4ea9 0272 1100    ..exportN..r..
+00000830: 0000 da04 6175 746f a901 7212 0000 0072  ....auto..r....r
+00000840: 1400 0000 7214 0000 0072 1500 0000 721a  ....r....r....r.
+00000850: 0000 003c 0000 00f3 0200 0000 1012 7a0b  ...<..........z.
+00000860: 4d61 7465 2e65 7870 6f72 744e 54da 0b6d  Mate.exportNT..m
+00000870: 6f64 756c 655f 6e61 6d65 da0b 6f75 7470  odule_name..outp
+00000880: 7574 5f6a 736f 6e63 0300 0000 0000 0000  ut_jsonc........
+00000890: 0000 0000 0400 0000 0500 0000 4300 0000  ............C...
+000008a0: 7332 0000 007c 006a 00a0 017c 01a1 017d  s2...|.j...|...}
+000008b0: 037c 0272 1374 0274 036a 047c 0364 0164  .|.r.t.t.j.|.d.d
+000008c0: 028d 0283 0101 0064 0353 0074 027c 0383  .......d.S.t.|..
+000008d0: 0101 0064 0353 0029 047a ee0a 0a0a 2020  ...d.S.).z....  
+000008e0: 2020 2020 2020 4c69 7374 7320 616c 6c20        Lists all 
+000008f0: 6176 6169 6c61 626c 6520 6d6f 6475 6c65  available module
+00000900: 732e 0a0a 2020 2020 2020 2020 4172 6773  s...        Args
+00000910: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
+00000920: 6475 6c65 5f6e 616d 653a 204e 616d 6520  dule_name: Name 
+00000930: 6f66 2074 6865 206d 6f64 756c 6520 746f  of the module to
+00000940: 206c 6973 742e 2049 6620 6e6f 7420 7370   list. If not sp
+00000950: 6563 6966 6965 642c 2061 6c6c 206d 6f64  ecified, all mod
+00000960: 756c 6573 2077 696c 6c20 6265 206c 6973  ules will be lis
+00000970: 7465 642e 0a0a 2020 2020 2020 2020 4578  ted...        Ex
+00000980: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
+00000990: 2020 2020 606d 6174 6520 6c69 7374 206d      `mate list m
+000009a0: 6f64 656c 7360 0a0a 2020 2020 2020 2020  odels`..        
+000009b0: 2020 2020 606d 6174 6520 6c69 7374 600a      `mate list`.
+000009c0: 0a20 2020 2020 2020 20e9 0400 0000 a901  .        .......
+000009d0: da06 696e 6465 6e74 4e29 0572 1100 0000  ..indentN).r....
+000009e0: da04 6c69 7374 da05 7072 696e 74da 046a  ..list..print..j
+000009f0: 736f 6eda 0564 756d 7073 2904 7212 0000  son..dumps).r...
+00000a00: 0072 1f00 0000 7220 0000 00da 026c 6972  .r....r .....lir
+00000a10: 1400 0000 7214 0000 0072 1500 0000 7224  ....r....r....r$
+00000a20: 0000 0050 0000 0073 0800 0000 0c14 0401  ...P...s........
+00000a30: 1601 0c02 7a09 4d61 7465 2e6c 6973 74da  ....z.Mate.list.
+00000a40: 0763 6f6d 6d61 6e64 6302 0000 0000 0000  .commandc.......
+00000a50: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00000a60: 0073 1000 0000 7c00 6a00 a001 7c01 a101  .s....|.j...|...
+00000a70: 0100 6401 5300 2902 618e 0100 000a 0a20  ..d.S.).a...... 
+00000a80: 2020 2020 2020 2060 6d61 7465 2061 7574         `mate aut
+00000a90: 6f20 7b63 6f6d 6d61 6e64 7d60 0a0a 2020  o {command}`..  
+00000aa0: 2020 2020 2020 5661 7269 6f75 7320 636f        Various co
+00000ab0: 6d6d 616e 6473 2074 6f20 6865 6c70 2077  mmands to help w
+00000ac0: 6974 6820 7468 6520 6465 7665 6c6f 706d  ith the developm
+00000ad0: 656e 7420 7072 6f63 6573 732e 0a0a 0a20  ent process.... 
+00000ae0: 2020 2020 2020 2063 6f6d 6d61 6e64 733a         commands:
+00000af0: 0a20 2020 2020 2020 202d 2060 6578 706f  .        - `expo
+00000b00: 7274 603a 2043 7265 6174 6573 2061 2072  rt`: Creates a r
+00000b10: 6571 7569 7265 6d65 6e74 732e 7478 7420  equirements.txt 
+00000b20: 616e 6420 6465 7065 6e64 656e 6369 6573  and dependencies
+00000b30: 2e6a 736f 6e20 6669 6c65 7320 666f 7220  .json files for 
+00000b40: 7368 6172 696e 6720 616e 6420 7265 7072  sharing and repr
+00000b50: 6f64 7563 6962 696c 6974 792e 0a20 2020  oducibility..   
+00000b60: 2020 2020 202d 2060 696e 6974 603a 2041       - `init`: A
+00000b70: 7574 6f6d 6174 6963 616c 6c79 2063 7265  utomatically cre
+00000b80: 6174 6573 2060 5f5f 696e 6974 5f5f 2e70  ates `__init__.p
+00000b90: 7960 2066 696c 6573 2069 6e20 7468 6520  y` files in the 
+00000ba0: 7072 6f6a 6563 7420 7374 7275 6374 7572  project structur
+00000bb0: 652e 0a0a 2020 2020 2020 2020 4578 616d  e...        Exam
+00000bc0: 706c 653a 0a0a 0a20 2020 2020 2020 2020  ple:...         
+00000bd0: 2020 2060 6d61 7465 2061 7574 6f20 6578     `mate auto ex
+00000be0: 706f 7274 600a 2020 2020 2020 2020 2020  port`.          
+00000bf0: 2020 606d 6174 6520 6175 746f 2069 6e69    `mate auto ini
+00000c00: 7460 0a20 2020 2020 2020 204e 721b 0000  t`.        Nr...
+00000c10: 0029 0272 1200 0000 7229 0000 0072 1400  .).r....r)...r..
+00000c20: 0000 7214 0000 0072 1500 0000 721c 0000  ..r....r....r...
+00000c30: 006a 0000 0072 1e00 0000 7a09 4d61 7465  .j...r....z.Mate
+00000c40: 2e61 7574 6f63 0100 0000 0000 0000 0000  .autoc..........
+00000c50: 0000 0100 0000 0500 0000 4300 0000 731c  ..........C...s.
+00000c60: 0000 0074 0074 016a 027c 006a 03a0 04a1  ...t.t.j.|.j....
+00000c70: 0064 0164 028d 0283 0101 0064 0353 0029  .d.d.......d.S.)
+00000c80: 047a 4e0a 2020 2020 2020 2020 5072 696e  .zN.        Prin
+00000c90: 7473 2061 2073 756d 6d61 7279 206f 6620  ts a summary of 
+00000ca0: 7468 6520 7072 6f6a 6563 7420 6d6f 6475  the project modu
+00000cb0: 6c65 732e 2053 616d 6520 6173 2060 6d61  les. Same as `ma
+00000cc0: 7465 206c 6973 7460 0a20 2020 2020 2020  te list`.       
+00000cd0: 2072 2100 0000 7222 0000 004e 2905 7225   r!...r"...N).r%
+00000ce0: 0000 0072 2600 0000 7227 0000 0072 1100  ...r&...r'...r..
+00000cf0: 0000 da07 7375 6d6d 6172 7972 1d00 0000  ....summaryr....
+00000d00: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+00000d10: 2a00 0000 7e00 0000 7302 0000 001c 057a  *...~...s......z
+00000d20: 0c4d 6174 652e 7375 6d6d 6172 79da 066d  .Mate.summary..m
+00000d30: 6f64 756c 65da 046e 616d 65da 0464 6573  odule..name..des
+00000d40: 7463 0400 0000 0000 0000 0000 0000 0900  tc..............
+00000d50: 0000 0700 0000 4f00 0000 73ec 0000 0074  ......O...s....t
+00000d60: 006a 01a0 027c 006a 037c 017c 02a1 037d  .j...|.j.|.|...}
+00000d70: 0674 006a 01a0 047c 06a1 0173 1f74 0564  .t.j...|...s.t.d
+00000d80: 017c 019b 0064 027c 029b 0064 039d 0583  .|...d.|...d....
+00000d90: 0101 0074 06a0 0764 04a1 0101 0074 006a  ...t...d.....t.j
+00000da0: 01a0 027c 006a 037c 017c 03a1 037d 0774  ...|.j.|.|...}.t
+00000db0: 006a 01a0 047c 07a1 0172 6164 057c 0476  .j...|...rad.|.v
+00000dc0: 0072 3f74 08a0 097c 07a1 0101 0074 0564  .r?t...|.....t.d
+00000dd0: 067c 079b 009d 0283 0101 006e 2274 0564  .|.........n"t.d
+00000de0: 077c 039b 0064 089d 0383 0101 0074 0a64  .|...d.......t.d
+00000df0: 0983 017d 087c 0864 0a6b 0272 5c74 08a0  ...}.|.d.k.r\t..
+00000e00: 097c 07a1 0101 0074 0564 067c 079b 009d  .|.....t.d.|....
+00000e10: 0283 0101 006e 0574 06a0 0764 04a1 0101  .....n.t...d....
+00000e20: 0074 08a0 0b7c 067c 07a1 0201 0074 0564  .t...|.|.....t.d
+00000e30: 017c 019b 0064 027c 029b 0064 0b7c 079b  .|...d.|...d.|..
+00000e40: 009d 0683 0101 0064 0c53 0029 0d61 8a01  .......d.S.).a..
+00000e50: 0000 0a20 2020 2020 2020 2060 6d61 7465  ...        `mate
+00000e60: 2063 6c6f 6e65 207b 6d6f 6475 6c65 7d20   clone {module} 
+00000e70: 7b6e 616d 657d 207b 6465 7374 7d20 7b2d  {name} {dest} {-
+00000e80: 6f7d 600a 0a20 2020 2020 2020 2043 6c6f  o}`..        Clo
+00000e90: 6e65 7320 6120 736f 7572 6365 2063 6f64  nes a source cod
+00000ea0: 6520 6d6f 6475 6c65 2074 6f20 6120 6e65  e module to a ne
+00000eb0: 7720 6465 7374 696e 6174 696f 6e2e 0a0a  w destination...
+00000ec0: 2020 2020 2020 2020 4172 6773 3a0a 0a20          Args:.. 
+00000ed0: 2020 2020 2020 2020 2020 206d 6f64 756c             modul
+00000ee0: 653a 204d 6f64 756c 6520 746f 2063 6c6f  e: Module to clo
+00000ef0: 6e65 2e0a 0a20 2020 2020 2020 2020 2020  ne...           
+00000f00: 206e 616d 653a 204e 616d 6520 6f66 2074   name: Name of t
+00000f10: 6865 206d 6f64 756c 6520 746f 2063 6c6f  he module to clo
+00000f20: 6e65 2e0a 0a20 2020 2020 2020 2020 2020  ne...           
+00000f30: 2064 6573 743a 2044 6573 7469 6e61 7469   dest: Destinati
+00000f40: 6f6e 2074 6f20 636c 6f6e 6520 7468 6520  on to clone the 
+00000f50: 6d6f 6475 6c65 2074 6f2e 0a0a 2020 2020  module to...    
+00000f60: 2020 2020 2020 2020 2d6f 3a20 4f76 6572          -o: Over
+00000f70: 7772 6974 6520 6465 7374 696e 6174 696f  write destinatio
+00000f80: 6e20 6966 2069 7420 6578 6973 7473 2e0a  n if it exists..
+00000f90: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+00000fa0: 3a0a 0a20 2020 2020 2020 2020 2020 2060  :..            `
+00000fb0: 6d61 7465 2063 6c6f 6e65 206d 6f64 656c  mate clone model
+00000fc0: 7320 746f 7263 685f 7669 7420 6d79 5f76  s torch_vit my_v
+00000fd0: 6974 600a 2020 2020 2020 2020 7a07 4d6f  it`.        z.Mo
+00000fe0: 6475 6c65 20fa 012f 7a0f 2064 6f65 7320  dule ../z. does 
+00000ff0: 6e6f 7420 6578 6973 7472 0400 0000 7a02  not existr....z.
+00001000: 2d6f 7a08 5265 6d6f 7665 6420 7a0c 4465  -oz.Removed z.De
+00001010: 7374 696e 6174 696f 6e20 7a07 2065 7869  stination z. exi
+00001020: 7374 737a 124f 7665 7277 7269 7465 3f20  stsz.Overwrite? 
+00001030: 2879 2f6e 293a 20da 0179 7a0b 2063 6c6f  (y/n): ..yz. clo
+00001040: 6e65 6420 746f 204e 290c 720b 0000 0072  ned to N).r....r
+00001050: 0c00 0000 da04 6a6f 696e 7209 0000 00da  ......joinr.....
+00001060: 0665 7869 7374 7372 2500 0000 da03 7379  .existsr%.....sy
+00001070: 73da 0465 7869 74da 0673 6875 7469 6cda  s..exit..shutil.
+00001080: 0672 6d74 7265 65da 0569 6e70 7574 da08  .rmtree..input..
+00001090: 636f 7079 7472 6565 2909 7212 0000 0072  copytree).r....r
+000010a0: 2b00 0000 722c 0000 0072 2d00 0000 7218  +...r,...r-...r.
+000010b0: 0000 0072 1900 0000 da0b 6d6f 6475 6c65  ...r......module
+000010c0: 5f70 6174 685a 0964 6573 745f 7061 7468  _pathZ.dest_path
+000010d0: da09 6f76 6572 7772 6974 6572 1400 0000  ..overwriter....
+000010e0: 7214 0000 0072 1500 0000 da05 636c 6f6e  r....r......clon
+000010f0: 6585 0000 0073 2200 0000 1216 0c01 1601  e....s".........
+00001100: 0a01 1203 0c01 0802 0a01 1001 1002 0801  ................
+00001110: 0801 0a01 1001 0a02 0c03 1e02 7a0a 4d61  ............z.Ma
+00001120: 7465 2e63 6c6f 6e65 da0a 6d6f 6465 6c5f  te.clone..model_
+00001130: 6e61 6d65 6302 0000 0000 0000 0000 0000  namec...........
+00001140: 0002 0000 0001 0000 0043 0000 0073 0400  .........C...s..
+00001150: 0000 6400 5300 2901 4e72 1400 0000 2902  ..d.S.).Nr....).
+00001160: 7212 0000 0072 3b00 0000 7214 0000 0072  r....r;...r....r
+00001170: 1400 0000 7215 0000 00da 0873 6e61 7073  ....r......snaps
+00001180: 686f 74b5 0000 0073 0200 0000 0401 7a0d  hot....s......z.
+00001190: 4d61 7465 2e73 6e61 7073 686f 74da 0a65  Mate.snapshot..e
+000011a0: 7870 5f6d 6f64 756c 65da 0365 7870 6303  xp_module..expc.
+000011b0: 0000 0000 0000 0000 0000 0007 0000 000a  ................
+000011c0: 0000 004f 0000 0073 8800 0000 7c00 6a00  ...O...s....|.j.
+000011d0: 6a01 6401 7c01 7c02 6704 7d05 6402 a002  j.d.|.|.g.}.d...
+000011e0: 7c05 a101 7d05 7a07 7403 7c05 8301 0100  |...}.z.t.|.....
+000011f0: 5700 6407 5300 0400 7404 7943 0100 7d06  W.d.S...t.yC..}.
+00001200: 0100 7a23 7405 6403 7c01 9b00 6404 7c02  ..z#t.d.|...d.|.
+00001210: 9b00 9d04 8301 0100 7405 6405 8301 0100  ........t.d.....
+00001220: 7c00 a006 6401 a101 0100 7407 a008 a100  |...d.....t.....
+00001230: 0100 7409 a00a 6406 a101 0100 5700 5900  ..t...d.....W.Y.
+00001240: 6407 7d06 7e06 6407 5300 6407 7d06 7e06  d.}.~.d.S.d.}.~.
+00001250: 7701 7700 2908 61e0 0100 000a 2020 2020  w.w.).a.....    
+00001260: 2020 2020 4578 6563 7574 6573 2061 6e20      Executes an 
+00001270: 6578 7065 7269 6d65 6e74 2e0a 0a20 2020  experiment...   
+00001280: 2020 2020 2055 7361 6765 3a20 6060 6d61       Usage: ``ma
+00001290: 7465 2074 7261 696e 207b 6d6f 6475 6c65  te train {module
+000012a0: 7d20 7b65 7870 6572 696d 656e 747d 6060  } {experiment}``
+000012b0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+000012c0: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
+000012d0: 5f6d 6f64 756c 653a 204e 616d 6520 6f66  _module: Name of
+000012e0: 2074 6865 206d 6f64 756c 6520 7768 6572   the module wher
+000012f0: 6520 7468 6520 6578 7065 7269 6d65 6e74  e the experiment
+00001300: 2069 7320 6c6f 6361 7465 642e 0a0a 2020   is located...  
+00001310: 2020 2020 2020 2020 2020 6578 703a 204e            exp: N
+00001320: 616d 6520 6f66 2074 6865 2065 7870 6572  ame of the exper
+00001330: 696d 656e 742e 0a0a 2020 2020 2020 2020  iment...        
+00001340: 4578 616d 706c 653a 0a20 2020 2020 2020  Example:.       
+00001350: 2020 2020 2060 0a20 2020 2020 2020 2020       `.         
+00001360: 2020 206d 6174 6520 7472 6169 6e20 6578     mate train ex
+00001370: 7065 7269 6d65 6e74 7320 6d79 5f65 7870  periments my_exp
+00001380: 6572 696d 656e 7460 0a0a 2020 2020 2020  eriment`..      
+00001390: 2020 5468 6973 2077 696c 6c20 7275 6e20    This will run 
+000013a0: 7468 6520 6578 7065 7269 6d65 6e74 2060  the experiment `
+000013b0: 6d79 5f65 7870 6572 696d 656e 7460 206c  my_experiment` l
+000013c0: 6f63 6174 6564 2069 6e20 7468 6520 6065  ocated in the `e
+000013d0: 7870 6572 696d 656e 7473 6020 6d6f 6475  xperiments` modu
+000013e0: 6c65 2e0a 0a20 2020 2020 2020 2045 7175  le...        Equ
+000013f0: 6976 616c 656e 7420 746f 2060 7079 7468  ivalent to `pyth
+00001400: 6f6e 202d 6d20 726f 6f74 5f6d 6f64 756c  on -m root_modul
+00001410: 652e 6578 7065 7269 6d65 6e74 732e 6d79  e.experiments.my
+00001420: 5f65 7870 6572 696d 656e 7420 7472 6169  _experiment trai
+00001430: 6e60 0a20 2020 2020 2020 20da 0b65 7870  n`.        ..exp
+00001440: 6572 696d 656e 7473 da01 2e7a 1145 7272  eriments...z.Err
+00001450: 6f72 2069 6e20 6c6f 6164 696e 6720 722e  or in loading r.
+00001460: 0000 007a 1641 7661 696c 6162 6c65 2065  ...z.Available e
+00001470: 7870 6572 696d 656e 7473 3a72 0400 0000  xperiments:r....
+00001480: 4e29 0b72 0f00 0000 da07 7072 6f6a 6563  N).r......projec
+00001490: 7472 3000 0000 da0a 5f5f 696d 706f 7274  tr0.....__import
+000014a0: 5f5f da09 4578 6365 7074 696f 6e72 2500  __..Exceptionr%.
+000014b0: 0000 7224 0000 00da 0974 7261 6365 6261  ..r$.....traceba
+000014c0: 636b da09 7072 696e 745f 6578 6372 3200  ck..print_excr2.
+000014d0: 0000 7233 0000 0029 0772 1200 0000 723d  ..r3...).r....r=
+000014e0: 0000 0072 3e00 0000 7218 0000 0072 1900  ...r>...r....r..
+000014f0: 0000 722b 0000 00da 0165 7214 0000 0072  ..r+.....er....r
+00001500: 1400 0000 7215 0000 00da 0574 7261 696e  ....r......train
+00001510: b800 0000 7318 0000 0010 160a 0102 020e  ....s...........
+00001520: 010e 0114 0108 010a 0108 0118 0308 8002  ................
+00001530: f97a 0a4d 6174 652e 7472 6169 6e63 0300  .z.Mate.trainc..
+00001540: 0000 0000 0000 0000 0000 0500 0000 0400  ................
+00001550: 0000 4f00 0000 731e 0000 007c 006a 007c  ..O...s....|.j.|
+00001560: 017c 0267 027c 03a2 0152 0069 007c 04a4  .|.g.|...R.i.|..
+00001570: 018e 0101 0064 0153 0029 0261 dd01 0000  .....d.S.).a....
+00001580: 0a20 2020 2020 2020 2045 7865 6375 7465  .        Execute
+00001590: 7320 616e 2065 7870 6572 696d 656e 742e  s an experiment.
+000015a0: 0a0a 2020 2020 2020 2020 5573 6167 653a  ..        Usage:
+000015b0: 2060 606d 6174 6520 7465 7374 207b 6d6f   ``mate test {mo
+000015c0: 6475 6c65 7d20 7b65 7870 6572 696d 656e  dule} {experimen
+000015d0: 747d 6060 0a0a 2020 2020 2020 2020 4172  t}``..        Ar
+000015e0: 6773 3a0a 0a20 2020 2020 2020 2020 2020  gs:..           
+000015f0: 2065 7870 5f6d 6f64 756c 653a 204e 616d   exp_module: Nam
+00001600: 6520 6f66 2074 6865 206d 6f64 756c 6520  e of the module 
+00001610: 7768 6572 6520 7468 6520 6578 7065 7269  where the experi
+00001620: 6d65 6e74 2069 7320 6c6f 6361 7465 642e  ment is located.
+00001630: 0a0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+00001640: 703a 204e 616d 6520 6f66 2074 6865 2065  p: Name of the e
+00001650: 7870 6572 696d 656e 742e 0a0a 2020 2020  xperiment...    
+00001660: 2020 2020 4578 616d 706c 653a 0a20 2020      Example:.   
+00001670: 2020 2020 2020 2020 2060 0a20 2020 2020           `.     
+00001680: 2020 2020 2020 206d 6174 6520 7465 7374         mate test
+00001690: 2065 7870 6572 696d 656e 7473 206d 795f   experiments my_
+000016a0: 6578 7065 7269 6d65 6e74 600a 0a20 2020  experiment`..   
+000016b0: 2020 2020 2054 6869 7320 7769 6c6c 2072       This will r
+000016c0: 756e 2074 6865 2065 7870 6572 696d 656e  un the experimen
+000016d0: 7420 606d 795f 6578 7065 7269 6d65 6e74  t `my_experiment
+000016e0: 6020 6c6f 6361 7465 6420 696e 2074 6865  ` located in the
+000016f0: 2060 6578 7065 7269 6d65 6e74 7360 206d   `experiments` m
+00001700: 6f64 756c 652e 0a0a 2020 2020 2020 2020  odule...        
+00001710: 4571 7569 7661 6c65 6e74 2074 6f20 6070  Equivalent to `p
+00001720: 7974 686f 6e20 2d6d 2072 6f6f 745f 6d6f  ython -m root_mo
+00001730: 6475 6c65 2e65 7870 6572 696d 656e 7473  dule.experiments
+00001740: 2e6d 795f 6578 7065 7269 6d65 6e74 2074  .my_experiment t
+00001750: 6573 7460 0a20 2020 2020 2020 204e 2901  est`.        N).
+00001760: 7247 0000 0029 0572 1200 0000 723d 0000  rG...).r....r=..
+00001770: 0072 3e00 0000 7218 0000 0072 1900 0000  .r>...r....r....
+00001780: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+00001790: 0474 6573 74dc 0000 0073 0200 0000 1e14  .test....s......
+000017a0: 7a09 4d61 7465 2e74 6573 74da 0375 726c  z.Mate.test..url
+000017b0: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
+000017c0: 0004 0000 004f 0000 0073 1e00 0000 7c00  .....O...s....|.
+000017d0: 6a00 6a01 7c01 6701 7c02 a201 5200 6900  j.j.|.g.|...R.i.
+000017e0: 7c03 a401 8e01 0100 6401 5300 2902 6169  |.......d.S.).ai
+000017f0: 0500 000a 2020 2020 2020 2020 496e 7461  ....        Inta
+00001800: 6c6c 7320 6120 6d6f 6475 6c65 2066 726f  lls a module fro
+00001810: 6d20 6120 6769 7420 7265 706f 7369 746f  m a git reposito
+00001820: 7279 2e0a 0a20 2020 2020 2020 2055 7361  ry...        Usa
+00001830: 6765 3a20 6060 6d61 7465 2069 6e73 7461  ge: ``mate insta
+00001840: 6c6c 207b 7572 6c7d 202d 7b79 7c6e 7c6f  ll {url} -{y|n|o
+00001850: 7d20 7b70 6d7d 6060 0a0a 2020 2020 2020  } {pm}``..      
+00001860: 2020 496e 7374 616c 6c20 6d6f 6475 6c65    Install module
+00001870: 2073 7570 706f 7274 2074 6865 2066 6f6c   support the fol
+00001880: 6c6f 7769 6e67 2066 6f72 6d61 7473 3a0a  lowing formats:.
+00001890: 2020 2020 2020 2020 2d20 6060 6d61 7465          - ``mate
+000018a0: 2069 6e73 7461 6c6c 207b 636f 6d70 6c65   install {comple
+000018b0: 7465 5f75 726c 7d60 600a 2020 2020 2020  te_url}``.      
+000018c0: 2020 2d20 6060 6d61 7465 2069 6e73 7461    - ``mate insta
+000018d0: 6c6c 207b 7573 6572 7d2f 7b72 6570 6f7d  ll {user}/{repo}
+000018e0: 2f7b 726f 6f74 5f6d 6f64 756c 657d 2f7b  /{root_module}/{
+000018f0: 6d6f 6475 6c65 7d60 600a 2020 2020 2020  module}``.      
+00001900: 2020 2d20 6060 6d61 7465 2069 6e73 7461    - ``mate insta
+00001910: 6c6c 207b 7573 6572 7d2f 7b72 6570 6f7c  ll {user}/{repo|
+00001920: 726f 6f74 5f6d 6f64 756c 657d 2f7b 6d6f  root_module}/{mo
+00001930: 6475 6c65 7d60 600a 0a20 2020 2020 2020  dule}``..       
+00001940: 2041 7267 733a 0a20 2020 2020 2020 202d   Args:.        -
+00001950: 2020 2020 7572 6c3a 2055 726c 206f 6620      url: Url of 
+00001960: 7468 6520 6769 7420 7265 706f 7369 746f  the git reposito
+00001970: 7279 2e0a 2020 2020 2020 2020 2d20 2020  ry..        -   
+00001980: 202d 793a 2053 6b69 7073 2063 6f6e 6669   -y: Skips confi
+00001990: 726d 6174 696f 6e20 616e 6420 696e 7374  rmation and inst
+000019a0: 616c 6c73 2070 7974 686f 6e20 6465 7065  alls python depe
+000019b0: 6e64 656e 6369 6573 0a20 2020 2020 2020  ndencies.       
+000019c0: 202d 2020 2020 2d6e 3a20 536b 6970 7320   -    -n: Skips 
+000019d0: 696e 7374 616c 6c69 6e67 2070 7974 686f  installing pytho
+000019e0: 6e20 6465 7065 6e64 656e 6369 6573 0a20  n dependencies. 
+000019f0: 2020 2020 2020 202d 2020 2020 2d6f 3a20         -    -o: 
+00001a00: 4f76 6572 7772 6974 6573 2065 7869 7374  Overwrites exist
+00001a10: 696e 6720 636f 6465 206d 6f64 756c 6573  ing code modules
+00001a20: 0a20 2020 2020 2020 202d 2020 2020 706d  .        -    pm
+00001a30: 3a20 5061 636b 6167 6520 6d61 6e61 6765  : Package manage
+00001a40: 7220 746f 2075 7365 2e20 4465 6661 756c  r to use. Defaul
+00001a50: 7473 2074 6f20 6173 6b69 6e67 2074 6865  ts to asking the
+00001a60: 2075 7365 722e 0a0a 2020 2020 2020 2020   user...        
+00001a70: 4578 616d 706c 6520 496e 7374 616c 6c69  Example Installi
+00001a80: 6e67 2061 206d 6f64 756c 6520 6672 6f6d  ng a module from
+00001a90: 2073 7472 7563 7475 7265 6420 6769 7420   structured git 
+00001aa0: 7265 706f 7369 746f 7279 2028 7265 636f  repository (reco
+00001ab0: 6d6d 656e 6465 6429 3a0a 0a0a 2020 2020  mmended):...    
+00001ac0: 2020 2020 2020 2020 6d61 7465 2069 6e73          mate ins
+00001ad0: 7461 6c6c 206f 616c 6565 2f64 6565 702d  tall oalee/deep-
+00001ae0: 7669 7369 6f6e 2f64 6565 706e 6574 2f6d  vision/deepnet/m
+00001af0: 6f64 656c 732f 746f 7263 685f 7669 7420  odels/torch_vit 
+00001b00: 2d79 6f20 7069 700a 0a20 2020 2020 2020  -yo pip..       
+00001b10: 2020 2020 2054 6869 7320 7769 6c6c 2069       This will i
+00001b20: 6e73 7461 6c6c 2074 6865 206d 6f64 756c  nstall the modul
+00001b30: 6520 6074 6f72 6368 5f76 6974 6020 6672  e `torch_vit` fr
+00001b40: 6f6d 2074 6865 2072 6570 6f73 6974 6f72  om the repositor
+00001b50: 7920 606f 616c 6565 2f64 6565 702d 7669  y `oalee/deep-vi
+00001b60: 7369 6f6e 6020 696e 2074 6f20 796f 7572  sion` in to your
+00001b70: 2060 6d6f 6465 6c73 6020 666f 6c64 6572   `models` folder
+00001b80: 2e0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00001b90: 6520 6079 6f60 2066 6c61 6773 2077 696c  e `yo` flags wil
+00001ba0: 6c20 736b 6970 2063 6f6e 6669 726d 6174  l skip confirmat
+00001bb0: 696f 6e20 616e 6420 696e 7374 616c 6c20  ion and install 
+00001bc0: 7079 7468 6f6e 2064 6570 656e 6465 6e63  python dependenc
+00001bd0: 6965 7320 7573 696e 6720 7069 702e 0a0a  ies using pip...
+00001be0: 2020 2020 2020 2020 4578 616d 706c 6520          Example 
+00001bf0: 496e 7374 616c 6c69 6e67 2061 206d 6f64  Installing a mod
+00001c00: 756c 6520 6672 6f6d 2075 6e73 7472 7563  ule from unstruc
+00001c10: 7475 7265 6420 6769 7420 7265 706f 7369  tured git reposi
+00001c20: 746f 7279 3a0a 0a0a 2020 2020 2020 2020  tory:...        
+00001c30: 2020 2020 6d61 7465 2069 6e73 7461 6c6c      mate install
+00001c40: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00001c50: 636f 6d2f 7277 6967 6874 6d61 6e2f 7079  com/rwightman/py
+00001c60: 746f 7263 682d 696d 6167 652d 6d6f 6465  torch-image-mode
+00001c70: 6c73 2f74 7265 652f 6d61 696e 2f74 696d  ls/tree/main/tim
+00001c80: 6d0a 0a0a 2020 2020 2020 2020 2020 2020  m...            
+00001c90: 5468 6973 2077 696c 6c20 696e 7374 616c  This will instal
+00001ca0: 6c20 7468 6520 6d6f 6475 6c65 2060 7469  l the module `ti
+00001cb0: 6d6d 6020 6672 6f6d 2074 6865 2072 6570  mm` from the rep
+00001cc0: 6f73 6974 6f72 7920 6173 2061 2073 6973  ository as a sis
+00001cd0: 7465 7220 6d6f 6475 6c65 2074 6f20 796f  ter module to yo
+00001ce0: 7572 2072 6f6f 7420 6d6f 6475 6c65 2e0a  ur root module..
+00001cf0: 2020 2020 2020 2020 2020 2020 5461 6b65              Take
+00001d00: 2069 6e74 6f20 6163 636f 756e 7420 7468   into account th
+00001d10: 6174 2074 6869 7320 7769 6c6c 2069 6e73  at this will ins
+00001d20: 7461 6c6c 206f 6e6c 7920 7468 6520 636f  tall only the co
+00001d30: 6465 2061 6e64 206e 6f74 2074 6865 2070  de and not the p
+00001d40: 7974 686f 6e20 6465 7065 6e64 656e 6369  ython dependenci
+00001d50: 6573 2e0a 2020 2020 2020 2020 4e29 0272  es..        N).r
+00001d60: 1100 0000 5a0b 696e 7374 616c 6c5f 7572  ....Z.install_ur
+00001d70: 6c29 0472 1200 0000 7249 0000 0072 1800  l).r....rI...r..
+00001d80: 0000 7219 0000 0072 1400 0000 7214 0000  ..r....r....r...
+00001d90: 0072 1500 0000 da07 696e 7374 616c 6cf2  .r......install.
+00001da0: 0000 0073 0200 0000 1e23 7a0c 4d61 7465  ...s.....#z.Mate
+00001db0: 2e69 6e73 7461 6c6c 6301 0000 0000 0000  .installc.......
+00001dc0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00001dd0: 0073 1400 0000 7400 a001 a100 5c02 7c00  .s....t.....\.|.
+00001de0: 5f02 7c00 5f03 6401 5300 2902 7a71 0a20  _.|._.d.S.).zq. 
+00001df0: 2020 2020 2020 204d 6574 686f 6420 696e         Method in
+00001e00: 2063 6861 7267 6520 6f66 2066 696e 6469   charge of findi
+00001e10: 6e67 2074 6865 2072 6f6f 7420 666f 6c64  ng the root fold
+00001e20: 6572 206f 6620 7468 6520 7072 6f6a 6563  er of the projec
+00001e30: 7420 616e 6420 7265 6164 696e 6720 7468  t and reading th
+00001e40: 6520 636f 6e74 656e 7420 6f66 206d 6174  e content of mat
+00001e50: 652e 6a73 6f6e 0a20 2020 2020 2020 204e  e.json.        N
+00001e60: 2904 7202 0000 005a 0966 696e 645f 726f  ).r....Z.find_ro
+00001e70: 6f74 7209 0000 0072 0f00 0000 721d 0000  otr....r....r...
+00001e80: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+00001e90: 5a0a 5f5f 6669 6e64 726f 6f74 1701 0000  Z.__findroot....
+00001ea0: 7302 0000 0014 047a 0f4d 6174 652e 5f5f  s......z.Mate.__
+00001eb0: 6669 6e64 726f 6f74 2901 4629 024e 5429  findroot).F).NT)
+00001ec0: 13da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00001ed0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00001ee0: 616d 655f 5fda 075f 5f64 6f63 5f5f 7216  ame__..__doc__r.
+00001ef0: 0000 00da 0c73 7461 7469 636d 6574 686f  .....staticmetho
+00001f00: 64da 0373 7472 7213 0000 0072 1a00 0000  d..strr....r....
+00001f10: da04 626f 6f6c 7224 0000 0072 1c00 0000  ..boolr$...r....
+00001f20: 722a 0000 0072 3a00 0000 723c 0000 0072  r*...r:...r<...r
+00001f30: 4700 0000 7248 0000 0072 4a00 0000 7210  G...rH...rJ...r.
+00001f40: 0000 0072 1400 0000 7214 0000 0072 1400  ...r....r....r..
+00001f50: 0000 7215 0000 0072 0700 0000 1000 0000  ..r....r........
+00001f60: 732a 0000 0008 0004 010a 0402 0910 0108  s*..............
+00001f70: 1d02 1602 0104 fd02 0202 fe02 030a fd0e  ................
+00001f80: 1a08 1416 070e 3012 0312 240e 160c 2572  ......0...$...%r
+00001f90: 0700 0000 290e 720b 0000 0072 4400 0000  ....).r....rD...
+00001fa0: 5a20 7965 7262 616d 6174 652e 6170 692e  Z yerbamate.api.
+00001fb0: 6461 7461 2e73 6f75 7263 6573 2e6c 6f63  data.sources.loc
+00001fc0: 616c 7202 0000 0072 2600 0000 5a16 7965  alr....r&...Z.ye
+00001fd0: 7262 616d 6174 652e 6170 692e 6d61 7465  rbamate.api.mate
+00001fe0: 5f61 7069 7203 0000 0072 3200 0000 da04  _apir....r2.....
+00001ff0: 6970 6462 7205 0000 0072 3400 0000 da06  ipdbr....r4.....
+00002000: 7479 7069 6e67 7206 0000 0072 0700 0000  typingr....r....
+00002010: 7214 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
+00002020: 1500 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00002030: 0000 7316 0000 0008 0008 010c 0108 010c  ..s.............
+00002040: 0108 0208 020c 0108 010c 0112 04         .............
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Feb 13 21:11:01 2023 UTC, .py size: 10647 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,590 +1,587 @@
-00000000: 6f0d 0d0a 0000 0000 65a7 ea63 9729 0000  o.......e..c.)..
+00000000: 6f0d 0d0a 0000 0000 e7c6 3164 7329 0000  o.........1ds)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
-00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
-00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
-00000050: 6404 6c06 6d07 5a07 0100 6405 6406 6c08  d.l.m.Z...d.d.l.
-00000060: 5a08 6405 6407 6c09 6d0a 5a0a 6d0b 5a0b  Z.d.d.l.m.Z.m.Z.
-00000070: 6d0c 5a0c 0100 6405 6406 6c0d 5a0d 6405  m.Z...d.d.l.Z.d.
-00000080: 6406 6c0e 5a0e 6405 6406 6c0f 5a0f 6408  d.l.Z.d.d.l.Z.d.
-00000090: 6510 6602 6409 640a 8404 5a11 640b 640c  e.f.d.d...Z.d.d.
-000000a0: 8400 5a12 641b 640d 650a 650b 1900 6602  ..Z.d.d.e.e...f.
-000000b0: 640e 640f 8405 5a13 6410 6510 6602 6411  d.d...Z.d.e.f.d.
-000000c0: 6412 8404 5a14 4700 6413 6414 8400 6414  d...Z.G.d.d...d.
-000000d0: 8302 5a15 6415 6516 6510 1900 6416 6517  ..Z.d.e.e...d.e.
-000000e0: 650b 1900 6410 6517 6516 6518 6602 1900  e...d.e.e.e.f...
-000000f0: 6606 6417 6418 8404 5a19 6419 641a 8400  f.d.d...Z.d.d...
-00000100: 5a1a 6406 5300 291c 614a 0100 000a 2323  Z.d.S.).aJ....##
-00000110: 2043 6c69 2050 6172 7365 720a 0a4d 6174   Cli Parser..Mat
-00000120: 6527 7320 636c 6920 7061 7273 6572 2069  e's cli parser i
-00000130: 7320 6120 7369 6d70 6c65 2070 6172 7365  s a simple parse
-00000140: 7220 7468 6174 2070 6172 7365 7320 7468  r that parses th
-00000150: 6520 636f 6d6d 616e 6420 6c69 6e65 2061  e command line a
-00000160: 7267 756d 656e 7473 2061 6e64 2063 616c  rguments and cal
-00000170: 6c73 2074 6865 2061 7070 726f 7072 6961  ls the appropria
-00000180: 7465 206d 6574 686f 6420 6f6e 2074 6865  te method on the
-00000190: 204d 6174 6520 636c 6173 732e 0a0a 4e6f   Mate class...No
-000001a0: 7469 6365 2074 6861 7420 666f 7220 626f  tice that for bo
-000001b0: 6f6c 6561 6e20 6172 6775 6d65 6e74 732c  olean arguments,
-000001c0: 2079 6f75 2063 616e 2075 7365 2065 6974   you can use eit
-000001d0: 6865 7220 6661 6c73 6520 6f72 2046 616c  her false or Fal
-000001e0: 7365 2c20 7472 7565 206f 7220 5472 7565  se, true or True
-000001f0: 2e20 416e 6420 666f 7220 4e6f 6e65 2079  . And for None y
-00000200: 6f75 2063 616e 2075 7365 2065 6974 6865  ou can use eithe
-00000210: 7220 6e75 6c6c 206f 7220 4e6f 6e65 2e0a  r null or None..
-00000220: 0a2a 2a45 7861 6d70 6c65 2a2a 0a0a 6060  .**Example**..``
-00000230: 600a 6d61 7465 2069 6e69 7420 6d79 5f70  `.mate init my_p
-00000240: 726f 6a65 6374 2076 656e 763d 6661 6c73  roject venv=fals
-00000250: 650a 6060 600a 0ae9 0100 0000 2901 da0a  e.```.......)...
-00000260: 4d61 7465 436f 6e66 6967 2902 da0e 7072  MateConfig)...pr
-00000270: 696e 745f 6d61 726b 646f 776e da0d 7265  int_markdown..re
-00000280: 6d6f 7665 5f69 6e64 656e 7429 01da 044d  move_indent)...M
-00000290: 6174 65e9 0000 0000 4e29 03da 084f 7074  ate.....N)...Opt
-000002a0: 696f 6e61 6cda 0843 616c 6c61 626c 65da  ional..Callable.
-000002b0: 0553 697a 6564 da0b 6d65 7468 6f64 5f6e  .Sized..method_n
-000002c0: 616d 6563 0200 0000 0000 0000 0000 0000  amec............
-000002d0: 0200 0000 0700 0000 4300 0000 7324 0000  ........C...s$..
-000002e0: 0074 0064 0164 0284 0074 01a0 0274 037c  .t.d.d...t...t.|
-000002f0: 007c 0183 02a1 016a 04a0 05a1 0044 0083  .|.....j.....D..
-00000300: 0183 0153 0029 034e 6301 0000 0000 0000  ...S.).Nc.......
-00000310: 0000 0000 0003 0000 0003 0000 0073 0000  .............s..
-00000320: 0073 2000 0000 8100 7c00 5d0b 5c02 7d01  .s .....|.].\.}.
-00000330: 7d02 7c01 6400 6b03 7202 7c02 5600 0100  }.|.d.k.r.|.V...
-00000340: 7102 6401 5300 2902 da04 7365 6c66 4ea9  q.d.S.)...selfN.
-00000350: 0029 03da 022e 30da 046e 616d 65da 0376  .)....0..name..v
-00000360: 616c 720c 0000 0072 0c00 0000 fa38 2f68  alr....r.....8/h
-00000370: 6f6d 652f 616c 2f47 6974 6875 622f 7965  ome/al/Github/ye
-00000380: 7262 616d 6174 652f 7061 636b 6167 6573  rbamate/packages
-00000390: 2f79 6572 6261 6d61 7465 2f6d 6174 655f  /yerbamate/mate_
-000003a0: 636c 692e 7079 da09 3c67 656e 6578 7072  cli.py..<genexpr
-000003b0: 3e1a 0000 0073 0e00 0000 0280 0400 0602  >....s..........
-000003c0: 0803 02fc 0604 04fb 7a24 5f5f 7061 7273  ........z$__pars
-000003d0: 655f 7369 676e 6174 7572 652e 3c6c 6f63  e_signature.<loc
-000003e0: 616c 733e 2e3c 6765 6e65 7870 723e 2906  als>.<genexpr>).
-000003f0: da05 7475 706c 65da 0769 6e73 7065 6374  ..tuple..inspect
-00000400: da09 7369 676e 6174 7572 65da 0767 6574  ..signature..get
-00000410: 6174 7472 da0a 7061 7261 6d65 7465 7273  attr..parameters
-00000420: da05 6974 656d 7329 02da 0a63 6c61 7373  ..items)...class
-00000430: 5f6e 616d 6572 0a00 0000 720c 0000 0072  _namer....r....r
-00000440: 0c00 0000 7210 0000 00da 115f 5f70 6172  ....r......__par
-00000450: 7365 5f73 6967 6e61 7475 7265 1900 0000  se_signature....
-00000460: 730c 0000 0008 0104 0208 0102 ff06 0208  s...............
-00000470: fc72 1900 0000 6301 0000 0000 0000 0000  .r....c.........
-00000480: 0000 0001 0000 0003 0000 0003 0000 0073  ...............s
-00000490: 1800 0000 8700 6601 6401 6402 8408 8800  ......f.d.d.....
-000004a0: 6a00 a001 a100 4400 8301 5300 2903 4e63  j.....D...S.).Nc
-000004b0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000004c0: 0600 0000 1300 0000 7322 0000 0069 007c  ........s"...i.|
-000004d0: 005d 0d7d 017c 01a0 0064 00a1 0173 027c  .].}.|...d...s.|
-000004e0: 0174 0188 007c 0183 0293 0271 0253 00a9  .t...|.....q.S..
-000004f0: 01da 015f 2902 da0a 7374 6172 7473 7769  ..._)...startswi
-00000500: 7468 7219 0000 0029 0272 0d00 0000 da01  thr....).r......
-00000510: 6ba9 0172 1800 0000 720c 0000 0072 1000  k..r....r....r..
-00000520: 0000 da0a 3c64 6963 7463 6f6d 703e 2400  ....<dictcomp>$.
-00000530: 0000 730c 0000 0006 0002 0208 0102 fd0a  ..s.............
-00000540: 0106 ff7a 305f 5f67 6574 5f6d 6574 686f  ...z0__get_metho
-00000550: 6473 5f77 6974 685f 6172 6775 6d65 6e74  ds_with_argument
-00000560: 732e 3c6c 6f63 616c 733e 2e3c 6469 6374  s.<locals>.<dict
-00000570: 636f 6d70 3e29 02da 085f 5f64 6963 745f  comp>)...__dict_
-00000580: 5fda 046b 6579 7372 1e00 0000 720c 0000  _..keysr....r...
-00000590: 0072 1e00 0000 7210 0000 00da 1c5f 5f67  .r....r......__g
-000005a0: 6574 5f6d 6574 686f 6473 5f77 6974 685f  et_methods_with_
-000005b0: 6172 6775 6d65 6e74 7323 0000 0073 0600  arguments#...s..
-000005c0: 0000 0a01 0802 06fe 7222 0000 00da 066d  ........r".....m
-000005d0: 656d 6265 7263 0200 0000 0000 0000 0000  emberc..........
-000005e0: 0000 0900 0000 0800 0000 0300 0000 73e8  ..............s.
-000005f0: 0000 007c 0164 0075 0072 0974 0074 017c  ...|.d.u.r.t.t.|
-00000600: 0083 027d 017c 0164 0075 0173 0f4a 0082  ...}.|.d.u.s.J..
-00000610: 0174 02a0 037c 01a1 016a 04a0 05a1 007d  .t...|...j.....}
-00000620: 0264 01a0 0664 0264 0384 007c 0244 0083  .d...d.d...|.D..
-00000630: 01a1 017d 0364 0464 0584 0064 0664 0384  ...}.d.d...d.d..
-00000640: 0074 077c 016a 0883 01a0 0964 07a1 0144  .t.|.j.....d...D
-00000650: 0083 0144 0083 0189 0087 0066 0164 0864  ...D.......f.d.d
-00000660: 0384 087c 0244 0083 017d 0464 07a0 067c  ...|.D...}.d...|
-00000670: 04a1 017d 0564 07a0 0664 0964 0384 0074  ...}.d...d.d...t
-00000680: 077c 016a 0883 01a0 0964 07a1 0144 0083  .|.j.....d...D..
-00000690: 01a1 017d 0674 0a64 0a7c 009b 0064 017c  ...}.t.d.|...d.|
-000006a0: 039b 0064 0b9d 0583 01a0 0ba1 007d 0774  ...d.........}.t
-000006b0: 0a64 077c 079b 0064 0c7c 05a0 0ba1 009b  .d.|...d.|......
-000006c0: 0064 0d74 0a7c 0683 019b 0064 0e9d 0783  .d.t.|.....d....
-000006d0: 017d 0874 0a7c 0883 0153 0029 0f4e fa01  .}.t.|...S.).N..
-000006e0: 2063 0100 0000 0000 0000 0000 0000 0200   c..............
-000006f0: 0000 0700 0000 5300 0000 7342 0000 0067  ......S...sB...g
-00000700: 007c 005d 1d7d 017c 016a 0064 006b 0372  .|.].}.|.j.d.k.r
-00000710: 0264 017c 016a 009b 007c 016a 0174 026a  .d.|.j...|.j.t.j
-00000720: 036b 0372 1a64 0274 047c 016a 0183 0117  .k.r.d.t.|.j....
-00000730: 006e 0164 039b 0064 049d 0491 0271 0253  .n.d...d.....q.S
-00000740: 0029 0572 0b00 0000 fa01 3cfa 013d da00  .).r......<..=..
-00000750: fa01 3e29 0572 0e00 0000 da07 6465 6661  ..>).r......defa
-00000760: 756c 7472 1300 0000 da06 5f65 6d70 7479  ultr......_empty
-00000770: da03 7374 72a9 0272 0d00 0000 da05 7061  ..str..r......pa
-00000780: 7261 6d72 0c00 0000 720c 0000 0072 1000  ramr....r....r..
-00000790: 0000 da0a 3c6c 6973 7463 6f6d 703e 3100  ....<listcomp>1.
-000007a0: 0000 730a 0000 0006 0002 020a 012a fe06  ..s..........*..
-000007b0: 027a 206d 6574 686f 645f 746f 5f6d 642e  .z method_to_md.
-000007c0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000007d0: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
-000007e0: 0200 0000 0800 0000 5300 0000 7348 0000  ........S...sH..
-000007f0: 0069 007c 005d 207d 0174 007c 0183 0164  .i.|.] }.t.|...d
-00000800: 006b 0472 027c 0164 0019 00a0 0164 01a1  .k.r.|.d.....d..
-00000810: 0172 027c 0164 0019 00a0 0264 02a1 0164  .r.|.d.....d...d
-00000820: 0019 0064 03a0 037c 0164 0464 0585 0219  ...d...|.d.d....
-00000830: 00a1 0193 0271 0253 0029 0672 0100 0000  .....q.S.).r....
-00000840: 722d 0000 0072 2400 0000 fa01 3ae9 0200  r-...r$.....:...
-00000850: 0000 4e29 04da 036c 656e 721c 0000 00da  ..N)...lenr.....
-00000860: 0573 706c 6974 da04 6a6f 696e a902 720d  .split..join..r.
-00000870: 0000 00da 046c 696e 6572 0c00 0000 720c  .....liner....r.
-00000880: 0000 0072 1000 0000 721f 0000 0037 0000  ...r....r....7..
-00000890: 0073 0a00 0000 0600 0202 1a01 20fe 0602  .s.......... ...
-000008a0: 7a20 6d65 7468 6f64 5f74 6f5f 6d64 2e3c  z method_to_md.<
-000008b0: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
-000008c0: 703e 6301 0000 0000 0000 0000 0000 0002  p>c.............
-000008d0: 0000 0005 0000 0053 0000 0073 1a00 0000  .......S...s....
-000008e0: 6700 7c00 5d09 7d01 7c01 a000 a100 a001  g.|.].}.|.......
-000008f0: 6400 a101 9102 7102 5300 2901 722f 0000  d.....q.S.).r/..
-00000900: 0029 02da 0573 7472 6970 7232 0000 0029  .)...stripr2...)
-00000910: 0272 0d00 0000 da01 6c72 0c00 0000 720c  .r......lr....r.
-00000920: 0000 0072 1000 0000 722e 0000 0039 0000  ...r....r....9..
-00000930: 00f3 0200 0000 1a00 da01 0a63 0100 0000  ...........c....
-00000940: 0000 0000 0000 0000 0200 0000 0b00 0000  ................
-00000950: 1300 0000 7358 0000 0067 007c 005d 287d  ....sX...g.|.](}
-00000960: 017c 016a 0064 006b 0372 0264 017c 016a  .|.j.d.k.r.d.|.j
-00000970: 009b 0064 027c 016a 016a 029b 0064 0388  ...d.|.j.j...d..
-00000980: 00a0 037c 016a 0064 04a1 029b 009d 067c  ...|.j.d.......|
-00000990: 016a 0474 056a 066b 0372 2764 057c 016a  .j.t.j.k.r'd.|.j
-000009a0: 049b 009d 026e 0164 0417 0091 0271 0253  .....n.d.....q.S
-000009b0: 0029 0672 0b00 0000 fa02 2d20 7a04 203a  .).r......- z. :
-000009c0: 2060 fa04 6020 3a20 7227 0000 0072 2600   `..` : r'...r&.
-000009d0: 0000 2907 720e 0000 00da 0a61 6e6e 6f74  ..).r......annot
-000009e0: 6174 696f 6eda 085f 5f6e 616d 655f 5fda  ation..__name__.
-000009f0: 0367 6574 7229 0000 0072 1300 0000 722a  .getr)...r....r*
-00000a00: 0000 0072 2c00 0000 a901 5a12 7061 7261  ...r,.....Z.para
-00000a10: 6d5f 6465 7363 7269 7074 696f 6e73 720c  m_descriptionsr.
-00000a20: 0000 0072 1000 0000 722e 0000 003d 0000  ...r....r....=..
-00000a30: 0073 0e00 0000 0600 0203 0a01 24fd 1a01  .s..........$...
-00000a40: 02ff 0603 6301 0000 0000 0000 0000 0000  ....c...........
-00000a50: 0002 0000 0005 0000 0053 0000 0073 1e00  .........S...s..
-00000a60: 0000 6700 7c00 5d0b 7d01 7c01 a000 a100  ..g.|.].}.|.....
-00000a70: a001 6400 a101 7302 7c01 9102 7102 5300  ..d...s.|...q.S.
-00000a80: 2901 7a06 3a70 6172 616d 2902 7236 0000  ).z.:param).r6..
-00000a90: 0072 1c00 0000 7234 0000 0072 0c00 0000  .r....r4...r....
-00000aa0: 720c 0000 0072 1000 0000 722e 0000 0045  r....r....r....E
-00000ab0: 0000 0073 0c00 0000 0600 0202 0c01 02fd  ...s............
-00000ac0: 0201 06ff 7518 0000 000a 2020 2020 6060  ....u.....    ``
-00000ad0: 600a 2020 2020 2020 e29d af20 6d61 7465  `.      ... mate
-00000ae0: 207a 0d0a 2020 2020 6060 600a 2020 2020   z..    ```.    
-00000af0: 7a0e 0a0a 2a2a 5061 7261 6d73 2a2a 0a0a  z...**Params**..
-00000b00: fa02 0a0a 7a06 0a0a 2d2d 2d0a 290c 7215  ....z...---.).r.
-00000b10: 0000 005a 074d 6174 6543 4c49 7213 0000  ...Z.MateCLIr...
-00000b20: 0072 1400 0000 7216 0000 00da 0676 616c  .r....r......val
-00000b30: 7565 7372 3300 0000 722b 0000 00da 075f  uesr3...r+....._
-00000b40: 5f64 6f63 5f5f 7232 0000 0072 0400 0000  _doc__r2...r....
-00000b50: 7236 0000 0029 0972 0a00 0000 7223 0000  r6...).r....r#..
-00000b60: 00da 0670 6172 616d 735a 0d69 6e6c 696e  ...paramsZ.inlin
-00000b70: 655f 7061 7261 6d73 5a0f 7261 775f 6c69  e_paramsZ.raw_li
-00000b80: 7374 5f70 6172 616d 735a 0b6c 6973 745f  st_paramsZ.list_
-00000b90: 7061 7261 6d73 5a12 6d65 7468 6f64 5f64  paramsZ.method_d
-00000ba0: 6573 6372 6970 7469 6f6e da04 636f 6465  escription..code
-00000bb0: da03 646f 6372 0c00 0000 723f 0000 0072  ..docr....r?...r
-00000bc0: 1000 0000 da0c 6d65 7468 6f64 5f74 6f5f  ......method_to_
-00000bd0: 6d64 2b00 0000 7350 0000 0008 010a 010c  md+...sP........
-00000be0: 0110 0104 0106 0102 0204 fe04 ff06 0718  ................
-00000bf0: 0206 fe0a 0602 0306 fd0a 0604 0106 010e  ................
-00000c00: 0204 fe04 ff02 0802 0102 0204 fe02 0206  ................
-00000c10: fe02 ff04 0602 fa02 0702 0102 0104 ff06  ................
-00000c20: 0504 fb06 0706 f904 ff08 0e72 4600 0000  ...........rF...
-00000c30: da06 7265 7475 726e 6300 0000 0000 0000  ..returnc.......
-00000c40: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
-00000c50: 0073 6800 0000 7400 7401 7402 6a03 8301  .sh...t.t.t.j...
-00000c60: 8301 6401 1700 7d00 7401 7404 6a05 7406  ..d...}.t.t.j.t.
-00000c70: 1900 6a03 8301 7d01 7c00 7c01 6401 1700  ..j...}.|.|.d...
-00000c80: 3700 7d00 6402 6403 8400 7407 6a08 7402  7.}.d.d...t.j.t.
-00000c90: 7407 6a09 6404 8d02 4400 8301 7d02 7c02  t.j.d...D...}.|.
-00000ca0: 4400 5d0b 5c02 7d03 7d04 7c00 740a 7c03  D.].\.}.}.|.t.|.
-00000cb0: 7c04 8302 3700 7d00 7126 7c00 5300 2905  |...7.}.q&|.S.).
-00000cc0: 4efa 070a 202d 2d2d 200a 6301 0000 0000  N... --- .c.....
-00000cd0: 0000 0000 0000 0003 0000 0005 0000 0053  ...............S
-00000ce0: 0000 0073 2200 0000 6700 7c00 5d0d 5c02  ...s"...g.|.].\.
-00000cf0: 7d01 7d02 7c01 a000 6400 a101 7302 7c01  }.}.|...d...s.|.
-00000d00: 7c02 6602 9102 7102 5300 721a 0000 0029  |.f...q.S.r....)
-00000d10: 0172 1c00 0000 2903 720d 0000 0072 1d00  .r....).r....r..
-00000d20: 0000 da01 7672 0c00 0000 720c 0000 0072  ....vr....r....r
-00000d30: 1000 0000 722e 0000 0069 0000 0073 0c00  ....r....i...s..
-00000d40: 0000 0600 0602 0801 02fd 0601 06ff 7a24  ..............z$
-00000d50: 6765 6e65 7261 7465 5f68 656c 705f 6d64  generate_help_md
-00000d60: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00000d70: 6f6d 703e 2901 da09 7072 6564 6963 6174  omp>)...predicat
-00000d80: 6529 0b72 0400 0000 722b 0000 0072 0500  e).r....r+...r..
-00000d90: 0000 7242 0000 00da 0373 7973 da07 6d6f  ..rB.....sys..mo
-00000da0: 6475 6c65 7372 3d00 0000 7213 0000 00da  dulesr=...r.....
-00000db0: 0a67 6574 6d65 6d62 6572 73da 0a69 7366  .getmembers..isf
-00000dc0: 756e 6374 696f 6e72 4600 0000 2905 7245  unctionrF...).rE
-00000dd0: 0000 005a 1163 7572 7265 6e74 5f64 6f63  ...Z.current_doc
-00000de0: 7374 7269 6e67 da07 6d65 6d62 6572 7372  string..membersr
-00000df0: 0e00 0000 720f 0000 0072 0c00 0000 720c  ....r....r....r.
-00000e00: 0000 0072 1000 0000 da10 6765 6e65 7261  ...r......genera
-00000e10: 7465 5f68 656c 705f 6d64 6400 0000 7312  te_help_mdd...s.
-00000e20: 0000 0012 0210 010c 0106 010e 0206 fe0c  ................
-00000e30: 0510 0104 0172 5000 0000 6300 0000 0000  .....rP...c.....
-00000e40: 0000 0000 0000 0000 0000 0005 0000 0040  ...............@
-00000e50: 0000 0073 6200 0000 6500 5a01 6400 5a02  ...sb...e.Z.d.Z.
-00000e60: 6401 6402 8400 5a03 6403 6404 8400 5a04  d.d...Z.d.d...Z.
-00000e70: 6405 6406 8400 5a05 6412 6408 6506 6409  d.d...Z.d.d.e.d.
-00000e80: 640a 6604 640b 640c 8405 5a07 6413 6408  d.f.d.d...Z.d.d.
-00000e90: 6506 6409 6506 6604 640e 640f 8405 5a08  e.d.e.f.d.d...Z.
-00000ea0: 6409 6509 6506 6506 6602 1900 6602 6410  d.e.e.e.f...f.d.
-00000eb0: 6411 8404 5a0a 640a 5300 2914 da08 4d61  d...Z.d.S.)...Ma
-00000ec0: 7465 4865 6c70 6301 0000 0000 0000 0000  teHelpc.........
-00000ed0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-00000ee0: 2200 0000 6401 7c00 5f00 6402 7c00 5f01  "...d.|._.d.|._.
-00000ef0: 7c00 a002 7403 a101 5c02 7c00 5f04 7c00  |...t...\.|._.|.
-00000f00: 5f05 6400 5300 2903 4e29 07da 0469 6e69  _.d.S.).N)...ini
-00000f10: 74da 0769 6e73 7461 6c6c da05 7472 6169  t..install..trai
-00000f20: 6eda 0461 7574 6f5a 0665 7870 6f72 74da  n..autoZ.export.
-00000f30: 0563 6c6f 6e65 da04 7465 7374 2907 7a18  .clone..test).z.
-00000f40: 496e 6974 6961 6c69 7a65 2061 206e 6577  Initialize a new
-00000f50: 2070 726f 6a65 6374 7a14 496e 7374 616c   projectz.Instal
-00000f60: 6c20 6465 7065 6e64 656e 6369 6573 7a0d  l dependenciesz.
-00000f70: 5472 6169 6e20 6120 6d6f 6465 6c7a 3456  Train a modelz4V
-00000f80: 6172 696f 7573 2063 6f6d 6d61 6e64 7320  arious commands 
-00000f90: 746f 2068 656c 7020 7769 7468 2074 6865  to help with the
-00000fa0: 2064 6576 656c 6f70 6d65 6e74 2070 726f   development pro
-00000fb0: 6365 737a 1345 7870 6f72 7420 6465 7065  cesz.Export depe
-00000fc0: 6e64 656e 6369 6573 7a17 436c 6f6e 6573  ndenciesz.Clones
-00000fd0: 2069 6e74 6572 6e61 6c20 6d6f 6475 6c65   internal module
-00000fe0: 737a 0c54 6573 7420 6120 6d6f 6465 6c29  sz.Test a model)
-00000ff0: 06da 0c68 656c 705f 6f70 7469 6f6e 73da  ...help_options.
-00001000: 0d68 656c 705f 636f 6d6d 656e 7473 da0d  .help_comments..
-00001010: 6765 745f 6675 6c6c 5f64 6f63 7372 0500  get_full_docsr..
-00001020: 0000 5a0a 5f66 756c 6c5f 646f 6373 da08  ..Z._full_docs..
-00001030: 5f6d 6574 686f 6473 a901 720b 0000 0072  _methods..r....r
-00001040: 0c00 0000 720c 0000 0072 1000 0000 da08  ....r....r......
-00001050: 5f5f 696e 6974 5f5f 7400 0000 7306 0000  __init__t...s...
-00001060: 0006 0106 0916 0a7a 114d 6174 6548 656c  .......z.MateHel
-00001070: 702e 5f5f 696e 6974 5f5f 6301 0000 0000  p.__init__c.....
-00001080: 0000 0000 0000 0003 0000 0006 0000 0043  ...............C
-00001090: 0000 0073 3a00 0000 6401 7d01 6402 6403  ...s:...d.}.d.d.
-000010a0: 8400 7400 7c00 6a01 7c00 6a02 8302 4400  ..t.|.j.|.j...D.
-000010b0: 8301 7d02 7403 6404 6405 7c01 6406 1700  ..}.t.d.d.|.d...
-000010c0: a004 7c02 a101 1700 9b00 6407 9d03 8301  ..|.......d.....
-000010d0: 5300 2908 4e72 3900 0000 6301 0000 0000  S.).Nr9...c.....
-000010e0: 0000 0000 0000 0003 0000 0006 0000 0053  ...............S
-000010f0: 0000 0073 2000 0000 6700 7c00 5d0c 5c02  ...s ...g.|.].\.
-00001100: 7d01 7d02 6400 7c01 9b00 6401 7c02 9b00  }.}.d.|...d.|...
-00001110: 9d04 9102 7102 5300 2902 fa01 6072 3b00  ....q.S.)...`r;.
-00001120: 0000 720c 0000 0029 0372 0d00 0000 da06  ..r....).r......
-00001130: 6f70 7469 6f6e da07 636f 6d6d 656e 7472  option..commentr
-00001140: 0c00 0000 720c 0000 0072 1000 0000 722e  ....r....r....r.
-00001150: 0000 0092 0000 0073 0800 0000 0600 0602  .......s........
-00001160: 0eff 06ff 7a26 4d61 7465 4865 6c70 2e67  ....z&MateHelp.g
-00001170: 6574 5f69 6e64 6578 2e3c 6c6f 6361 6c73  et_index.<locals
-00001180: 3e2e 3c6c 6973 7463 6f6d 703e 7ac2 0a20  >.<listcomp>z.. 
-00001190: 2020 2020 2020 2023 2048 656c 7020 496e         # Help In
-000011a0: 6465 780a 0a20 2020 2020 2020 204d 6174  dex..        Mat
-000011b0: 652c 2079 6f75 7220 6672 6965 6e64 6c79  e, your friendly
-000011c0: 204d 4c20 7072 6f6a 6563 7420 6d61 6e61   ML project mana
-000011d0: 6765 722e 0a20 2020 2020 2020 200a 2020  ger..        .  
-000011e0: 2020 2020 2020 5479 7065 2060 6d61 7465        Type `mate
-000011f0: 2068 656c 7020 3c6f 7074 696f 6e3e 6020   help <option>` 
-00001200: 746f 2067 6574 206d 6f72 6520 696e 666f  to get more info
-00001210: 726d 6174 696f 6e20 6162 6f75 7420 6120  rmation about a 
-00001220: 746f 7069 632e 0a0a 2020 2020 2020 2020  topic...        
-00001230: 4176 6169 6c61 626c 6520 6f70 7469 6f6e  Available option
-00001240: 7320 6172 653a 0a0a 2020 2020 2020 2020  s are:..        
-00001250: 723a 0000 007a 0320 2d20 7a09 0a20 2020  r:...z. - z..   
-00001260: 2020 2020 2029 05da 037a 6970 7258 0000       )...ziprX..
-00001270: 0072 5900 0000 7204 0000 0072 3300 0000  .rY...r....r3...
-00001280: 2903 720b 0000 00da 026e 6c5a 0568 656c  ).r......nlZ.hel
-00001290: 7073 720c 0000 0072 0c00 0000 7210 0000  psr....r....r...
-000012a0: 00da 0967 6574 5f69 6e64 6578 8e00 0000  ...get_index....
-000012b0: 7312 0000 0004 0106 030c 0206 fe02 0402  s...............
-000012c0: 0110 0906 f704 ff7a 124d 6174 6548 656c  .......z.MateHel
-000012d0: 702e 6765 745f 696e 6465 7863 0200 0000  p.get_indexc....
-000012e0: 0000 0000 0000 0000 0500 0000 0700 0000  ................
-000012f0: 0300 0000 7356 0000 0074 007c 016a 0183  ....sV...t.|.j..
-00001300: 0164 0117 007d 0264 0264 0384 0089 0087  .d...}.d.d......
-00001310: 0066 0164 0464 0584 0874 02a0 037c 0174  .f.d.d...t...|.t
-00001320: 026a 04a1 0244 0083 017d 0364 067d 047c  .j...D...}.d.}.|
-00001330: 029b 0064 0774 007c 04a0 057c 03a0 06a1  ...d.t.|...|....
-00001340: 00a1 0183 019b 009d 037c 0366 0253 0029  .........|.f.S.)
-00001350: 084e 7a08 0a0a 202d 2d2d 200a 6302 0000  .Nz... --- .c...
-00001360: 0000 0000 0000 0000 0008 0000 0005 0000  ................
-00001370: 0053 0000 0073 6e00 0000 7400 7c01 6a01  .S...sn...t.|.j.
-00001380: 8301 7d02 7402 a003 7c01 a101 7d03 7404  ..}.t...|...}.t.
-00001390: 7c03 6a05 a006 a100 8301 7d04 7c04 6401  |.j.......}.|.d.
-000013a0: 1900 6a07 6402 6b03 7d05 6403 6404 8400  ..j.d.k.}.d.d...
-000013b0: 7c04 4400 8301 7d04 6405 a008 6406 6404  |.D...}.d...d.d.
-000013c0: 8400 7404 7c04 8301 4400 8301 a101 7d06  ..t.|...D.....}.
-000013d0: 6407 7c00 9b00 6408 9d03 7d07 7c07 7c02  d.|...d...}.|.|.
-000013e0: 1700 6409 1700 5300 290a 4e72 0600 0000  ..d...S.).Nr....
-000013f0: 720b 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00001400: 0000 0200 0000 0400 0000 5300 0000 731a  ..........S...s.
-00001410: 0000 0067 007c 005d 097d 017c 016a 0064  ...g.|.].}.|.j.d
-00001420: 006b 0372 027c 0191 0271 0253 0072 5c00  .k.r.|...q.S.r\.
-00001430: 0000 2901 720e 0000 0029 0272 0d00 0000  ..).r....).r....
-00001440: da03 6172 6772 0c00 0000 720c 0000 0072  ..argr....r....r
-00001450: 1000 0000 722e 0000 00ac 0000 0072 3800  ....r........r8.
-00001460: 0000 7a42 4d61 7465 4865 6c70 2e67 6574  ..zBMateHelp.get
-00001470: 5f66 756c 6c5f 646f 6373 2e3c 6c6f 6361  _full_docs.<loca
-00001480: 6c73 3e2e 6765 745f 6d65 7468 6f64 5f64  ls>.get_method_d
-00001490: 6f63 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  oc.<locals>.<lis
-000014a0: 7463 6f6d 703e 7a02 2c20 6301 0000 0000  tcomp>z., c.....
-000014b0: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-000014c0: 0000 0073 1400 0000 6700 7c00 5d06 7d01  ...s....g.|.].}.
-000014d0: 7400 7c01 8301 9102 7102 5300 720c 0000  t.|.....q.S.r...
-000014e0: 0029 0172 2b00 0000 2902 720d 0000 00da  .).r+...).r.....
-000014f0: 0161 720c 0000 0072 0c00 0000 7210 0000  .ar....r....r...
-00001500: 0072 2e00 0000 ad00 0000 7302 0000 0014  .r........s.....
-00001510: 007a 0b23 2323 2060 6d61 7465 6020 7239  .z.### `mate` r9
-00001520: 0000 0072 4800 0000 2909 7204 0000 0072  ...rH...).r....r
-00001530: 4200 0000 7213 0000 0072 1400 0000 da04  B...r....r......
-00001540: 6c69 7374 7216 0000 0072 4100 0000 720e  listr....rA...r.
-00001550: 0000 0072 3300 0000 2908 720a 0000 00da  ...r3...).r.....
-00001560: 066d 6574 686f 6472 4500 0000 7214 0000  .methodrE...r...
-00001570: 00da 0461 7267 735a 0969 735f 7374 6174  ...argsZ.is_stat
-00001580: 6963 da0b 616e 6e6f 7461 7469 6f6e 73da  ic..annotations.
-00001590: 0668 6561 6465 7272 0c00 0000 720c 0000  .headerr....r...
-000015a0: 0072 1000 0000 da0e 6765 745f 6d65 7468  .r......get_meth
-000015b0: 6f64 5f64 6f63 a700 0000 7310 0000 000a  od_doc....s.....
-000015c0: 010a 010e 010e 010e 0118 010c 010c 017a  ...............z
-000015d0: 2e4d 6174 6548 656c 702e 6765 745f 6675  .MateHelp.get_fu
-000015e0: 6c6c 5f64 6f63 732e 3c6c 6f63 616c 733e  ll_docs.<locals>
-000015f0: 2e67 6574 5f6d 6574 686f 645f 646f 6363  .get_method_docc
-00001600: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00001610: 0700 0000 1300 0000 7332 0000 0069 007c  ........s2...i.|
-00001620: 005d 155c 027d 017d 027c 01a0 0064 00a1  .].\.}.}.|...d..
-00001630: 0173 177c 026a 0164 0175 0172 027c 0188  .s.|.j.d.u.r.|..
-00001640: 007c 017c 0264 028d 0293 0271 0253 0029  .|.|.d.....q.S.)
-00001650: 0372 1b00 0000 4e29 0272 0a00 0000 7267  .r....N).r....rg
-00001660: 0000 0029 0272 1c00 0000 7242 0000 0029  ...).r....rB...)
-00001670: 0372 0d00 0000 720a 0000 0072 6700 0000  .r....r....rg...
-00001680: a901 726b 0000 0072 0c00 0000 7210 0000  ..rk...r....r...
-00001690: 0072 1f00 0000 b900 0000 730e 0000 0006  .r........s.....
-000016a0: 0006 0208 0302 fb0a 050c fc06 047a 2a4d  .............z*M
-000016b0: 6174 6548 656c 702e 6765 745f 6675 6c6c  ateHelp.get_full
-000016c0: 5f64 6f63 732e 3c6c 6f63 616c 733e 2e3c  _docs.<locals>.<
-000016d0: 6469 6374 636f 6d70 3e72 3900 0000 7240  dictcomp>r9...r@
-000016e0: 0000 0029 0772 0400 0000 7242 0000 0072  ...).r....rB...r
-000016f0: 1300 0000 724d 0000 0072 4e00 0000 7233  ....rM...rN...r3
-00001700: 0000 0072 4100 0000 2905 720b 0000 00da  ...rA...).r.....
-00001710: 0b63 6c61 7373 5f76 616c 7565 726a 0000  .class_valuerj..
-00001720: 005a 0b6d 6574 686f 645f 6469 6374 7262  .Z.method_dictrb
-00001730: 0000 0072 0c00 0000 726c 0000 0072 1000  ...r....rl...r..
-00001740: 0000 725a 0000 00a4 0000 0073 1600 0000  ..rZ.......s....
-00001750: 0e01 0802 0a12 0402 0601 02ff 06fe 0408  ................
-00001760: 1a02 0201 04fe 7a16 4d61 7465 4865 6c70  ......z.MateHelp
-00001770: 2e67 6574 5f66 756c 6c5f 646f 6373 7227  .get_full_docsr'
-00001780: 0000 00da 0477 6861 7472 4700 0000 4e63  .....whatrG...Nc
-00001790: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000017a0: 0300 0000 4300 0000 732c 0000 007c 017c  ....C...s,...|.|
-000017b0: 006a 0076 0072 0e74 017c 006a 027c 0119  .j.v.r.t.|.j.|..
-000017c0: 0083 0101 0064 0053 0074 017c 00a0 03a1  .....d.S.t.|....
-000017d0: 0083 0101 0064 0053 00a9 014e 2904 7258  .....d.S...N).rX
-000017e0: 0000 0072 0300 0000 725b 0000 0072 6300  ...r....r[...rc.
-000017f0: 0000 a902 720b 0000 0072 6e00 0000 720c  ....r....rn...r.
-00001800: 0000 0072 0c00 0000 7210 0000 00da 0a70  ...r....r......p
-00001810: 7269 6e74 5f68 656c 70c7 0000 0073 0600  rint_help....s..
-00001820: 0000 0a02 1202 1002 7a13 4d61 7465 4865  ........z.MateHe
-00001830: 6c70 2e70 7269 6e74 5f68 656c 70da 0363  lp.print_help..c
-00001840: 6c69 6302 0000 0000 0000 0000 0000 0002  lic.............
-00001850: 0000 0004 0000 0043 0000 0073 2a00 0000  .......C...s*...
-00001860: 7c01 6401 6b02 7207 7400 8300 5300 7c01  |.d.k.r.t...S.|.
-00001870: 6402 6b02 7212 7401 7c00 a002 7403 a101  d.k.r.t.|...t...
-00001880: 8301 5300 7400 8300 5300 2903 4e72 7200  ..S.t...S.).Nrr.
-00001890: 0000 da04 6d61 7465 2904 7250 0000 0072  ....mate).rP...r
-000018a0: 2b00 0000 725a 0000 0072 0500 0000 7270  +...rZ...r....rp
-000018b0: 0000 0072 0c00 0000 720c 0000 0072 1000  ...r....r....r..
-000018c0: 0000 da0b 6765 745f 6865 6c70 5f6d 64de  ....get_help_md.
-000018d0: 0000 0073 0a00 0000 0801 0601 0801 0e01  ...s............
-000018e0: 0608 7a14 4d61 7465 4865 6c70 2e67 6574  ..z.MateHelp.get
-000018f0: 5f68 656c 705f 6d64 6301 0000 0000 0000  _help_mdc.......
-00001900: 0000 0000 0001 0000 0003 0000 0003 0000  ................
-00001910: 0073 1400 0000 8700 6601 6401 6402 8408  .s......f.d.d...
-00001920: 8800 6a00 4400 8301 5300 2903 4e63 0100  ..j.D...S.).Nc..
-00001930: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-00001940: 0000 1300 0000 7318 0000 0069 007c 005d  ......s....i.|.]
-00001950: 087d 017c 0188 00a0 007c 01a1 0193 0271  .}.|.....|.....q
-00001960: 0253 0072 0c00 0000 2901 7274 0000 0029  .S.r....).rt...)
-00001970: 0272 0d00 0000 da03 6b65 7972 5c00 0000  .r......keyr\...
-00001980: 720c 0000 0072 1000 0000 721f 0000 00ed  r....r....r.....
-00001990: 0000 0073 0200 0000 1800 7a2c 4d61 7465  ...s......z,Mate
-000019a0: 4865 6c70 2e67 6574 5f61 6c6c 5f68 656c  Help.get_all_hel
-000019b0: 705f 6d64 2e3c 6c6f 6361 6c73 3e2e 3c64  p_md.<locals>.<d
-000019c0: 6963 7463 6f6d 703e 2901 7258 0000 0072  ictcomp>).rX...r
-000019d0: 5c00 0000 720c 0000 0072 5c00 0000 7210  \...r....r\...r.
-000019e0: 0000 00da 0f67 6574 5f61 6c6c 5f68 656c  .....get_all_hel
-000019f0: 705f 6d64 ec00 0000 7302 0000 0014 017a  p_md....s......z
-00001a00: 184d 6174 6548 656c 702e 6765 745f 616c  .MateHelp.get_al
-00001a10: 6c5f 6865 6c70 5f6d 6429 0172 2700 0000  l_help_md).r'...
-00001a20: 2901 7272 0000 0029 0b72 3d00 0000 da0a  ).rr...).r=.....
-00001a30: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00001a40: 616c 6e61 6d65 5f5f 725d 0000 0072 6300  alname__r]...rc.
-00001a50: 0000 725a 0000 0072 2b00 0000 7271 0000  ..rZ...r+...rq..
-00001a60: 0072 7400 0000 da04 6469 6374 7276 0000  .rt.....dictrv..
-00001a70: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-00001a80: 7210 0000 0072 5100 0000 7300 0000 730e  r....rQ...s...s.
-00001a90: 0000 0008 0008 0108 1a08 1614 2314 171a  ............#...
-00001aa0: 0e72 5100 0000 7268 0000 0072 6900 0000  .rQ...rh...ri...
-00001ab0: 6302 0000 0000 0000 0000 0000 000d 0000  c...............
-00001ac0: 0008 0000 0043 0000 0073 1801 0000 6900  .....C...s....i.
-00001ad0: 7d02 6700 7d03 6401 7d04 6402 7400 6602  }.g.}.d.}.d.t.f.
-00001ae0: 6403 6404 8404 7d05 6402 7400 6602 6405  d.d...}.d.t.f.d.
-00001af0: 6406 8404 7d06 7401 7c01 8301 7401 7c00  d...}.t.|...t.|.
-00001b00: 8301 6b00 7229 7c01 7c05 6601 7401 7c00  ..k.r)|.|.f.t.|.
-00001b10: 8301 7401 7c01 8301 1800 1400 1700 7d01  ..t.|.........}.
-00001b20: 6407 6408 6c02 6d03 7d07 0100 7404 7405  d.d.l.m.}...t.t.
-00001b30: 7c00 7c01 8302 8301 4400 5d51 5c02 7d08  |.|.....D.]Q\.}.
-00001b40: 5c02 7d09 7d0a 7c0a 7406 6b02 7243 7c06  \.}.}.|.t.k.rC|.
-00001b50: 7d0a 6e10 7c0a 7407 6a08 6b02 724b 7c05  }.n.|.t.j.k.rK|.
-00001b60: 7d0a 6e08 7409 7c0a 6409 8302 7253 7c0a  }.n.t.|.d...rS|.
-00001b70: 6a0a 7d0a 640a 7c09 7600 7267 7c09 a00b  j.}.d.|.v.rg|...
-00001b80: 640a a101 5c02 7d0b 7d0c 7c0a 7c0c 8301  d...\.}.}.|.|...
-00001b90: 7c02 7c0b 3c00 640b 7d04 7136 740c 7c0a  |.|.<.d.}.q6t.|.
-00001ba0: 740d 8302 7270 7c0a 6407 1900 7d0a 7c03  t...rp|.d...}.|.
-00001bb0: a00e 7c0a 7c09 8301 a101 0100 7c04 7287  ..|.|.......|.r.
-00001bc0: 740f 640c 7c09 9b00 640d 7c00 7c08 640e  t.d.|...d.|.|.d.
-00001bd0: 1800 1900 9b00 9d04 8301 8201 7136 7c03  ............q6|.
-00001be0: 7c02 6602 5300 290f 4e46 7264 0000 0063  |.f.S.).NFrd...c
-00001bf0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00001c00: 0900 0000 5300 0000 7368 0000 0074 0074  ....S...sh...t.t
-00001c10: 0174 0267 037d 017c 00a0 03a1 0064 0176  .t.g.}.|.....d.v
-00001c20: 0072 0d64 0053 007c 00a0 03a1 0064 026b  .r.d.S.|.....d.k
-00001c30: 0272 1564 0353 007c 00a0 03a1 0064 046b  .r.d.S.|.....d.k
-00001c40: 0272 1d64 0553 007c 0144 005d 127d 027a  .r.d.S.|.D.].}.z
-00001c50: 077c 027c 0083 0157 0002 0001 0053 0004  .|.|...W.....S..
-00001c60: 0074 0479 3101 0001 0001 0059 0071 1f77  .t.y1......Y.q.w
-00001c70: 0064 0053 0029 064e 2902 da04 6e6f 6e65  .d.S.).N)...none
-00001c80: da04 6e75 6c6c da04 7472 7565 54da 0566  ..null..trueT..f
-00001c90: 616c 7365 4629 05da 0369 6e74 da05 666c  alseF)...int..fl
-00001ca0: 6f61 7472 2b00 0000 da05 6c6f 7765 72da  oatr+.....lower.
-00001cb0: 0a56 616c 7565 4572 726f 7229 0372 6400  .ValueError).rd.
-00001cc0: 0000 da05 7479 7065 73da 0174 720c 0000  ....types..tr...
-00001cd0: 0072 0c00 0000 7210 0000 00da 0f67 6f6f  .r....r......goo
-00001ce0: 645f 6775 6573 735f 7479 7065 fb00 0000  d_guess_type....
-00001cf0: 731c 0000 000a 010c 0104 010c 0104 010c  s...............
-00001d00: 0104 0108 0102 010e 010c 0104 0102 ff04  ................
-00001d10: fd7a 2563 6f6c 6c65 6374 5f61 7267 732e  .z%collect_args.
-00001d20: 3c6c 6f63 616c 733e 2e67 6f6f 645f 6775  <locals>.good_gu
-00001d30: 6573 735f 7479 7065 6301 0000 0000 0000  ess_typec.......
-00001d40: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
-00001d50: 0073 2800 0000 7c00 a000 a100 6401 6b02  .s(...|.....d.k.
-00001d60: 7208 6402 5300 7c00 a000 a100 6403 6b02  r.d.S.|.....d.k.
-00001d70: 7210 6404 5300 7401 6405 8301 8201 2906  r.d.S.t.d.....).
-00001d80: 4e72 7c00 0000 5472 7d00 0000 467a 0d4e  Nr|...Tr}...Fz.N
-00001d90: 6f74 2061 2062 6f6f 6c65 616e 2902 7280  ot a boolean).r.
-00001da0: 0000 0072 8100 0000 2901 7264 0000 0072  ...r....).rd...r
-00001db0: 0c00 0000 720c 0000 0072 1000 0000 da0c  ....r....r......
-00001dc0: 626f 6f6c 6561 6e5f 7479 7065 0901 0000  boolean_type....
-00001dd0: 730a 0000 000c 0104 010c 0104 0108 027a  s..............z
-00001de0: 2263 6f6c 6c65 6374 5f61 7267 732e 3c6c  "collect_args.<l
-00001df0: 6f63 616c 733e 2e62 6f6f 6c65 616e 5f74  ocals>.boolean_t
-00001e00: 7970 6572 0600 0000 2901 da05 556e 696f  yper....)...Unio
-00001e10: 6eda 085f 5f61 7267 735f 5f72 2600 0000  n..__args__r&...
-00001e20: 547a 1470 6f73 6974 696f 6e61 6c20 6172  Tz.positional ar
-00001e30: 6775 6d65 6e74 207a 1820 6166 7465 7220  gument z. after 
-00001e40: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
-00001e50: 2072 0100 0000 2910 722b 0000 0072 3100   r....).r+...r1.
-00001e60: 0000 da06 7479 7069 6e67 7286 0000 00da  ....typingr.....
-00001e70: 0965 6e75 6d65 7261 7465 7261 0000 00da  .enumeratera....
-00001e80: 0462 6f6f 6c72 1300 0000 722a 0000 00da  .boolr....r*....
-00001e90: 0768 6173 6174 7472 7287 0000 0072 3200  .hasattrr....r2.
-00001ea0: 0000 da0a 6973 696e 7374 616e 6365 7212  ....isinstancer.
-00001eb0: 0000 00da 0661 7070 656e 6472 8100 0000  .....appendr....
-00001ec0: 290d 7268 0000 0072 6900 0000 da06 6b77  ).rh...ri.....kw
-00001ed0: 6172 6773 5a0f 706f 7369 7469 6f6e 616c  argsZ.positional
-00001ee0: 5f61 7267 735a 1770 6f73 6974 696f 6e61  _argsZ.positiona
-00001ef0: 6c5f 6172 6773 5f73 7461 7274 6564 7284  l_args_startedr.
-00001f00: 0000 0072 8500 0000 7286 0000 00da 0169  ...r....r......i
-00001f10: 7264 0000 0072 3c00 0000 7275 0000 00da  rd...r<...ru....
-00001f20: 0576 616c 7565 720c 0000 0072 0c00 0000  .valuer....r....
-00001f30: 7210 0000 00da 0c63 6f6c 6c65 6374 5f61  r......collect_a
-00001f40: 7267 73f0 0000 0073 3800 0000 0407 0401  rgs....s8.......
-00001f50: 0401 0e02 0e0e 1008 1a01 0c01 1a02 0801  ................
-00001f60: 0601 0a01 0601 0a01 0601 0801 0e01 0c01  ................
-00001f70: 0601 0a02 0801 0e01 0401 0201 1601 04ff  ................
-00001f80: 02ff 0805 7291 0000 0063 0000 0000 0000  ....r....c......
-00001f90: 0000 0000 0000 0d00 0000 0a00 0000 4300  ..............C.
-00001fa0: 0000 739c 0100 0074 0074 0183 017d 0074  ..s....t.t...}.t
-00001fb0: 026a 0364 0164 0085 0219 007d 017c 0164  .j.d.d.....}.|.d
-00001fc0: 0164 0085 0219 007d 0264 027d 0374 0464  .d.....}.d.}.t.d
-00001fd0: 0364 0484 007c 0044 0083 0183 017c 0317  .d...|.D.....|..
-00001fe0: 007d 0474 0583 007d 0574 067c 0183 0164  .}.t...}.t.|...d
-00001ff0: 056b 0273 2d7c 0164 0519 007c 0376 0072  .k.s-|.d...|.v.r
-00002000: 4274 067c 0183 0164 016b 0472 3c7c 05a0  Bt.|...d.k.r<|..
-00002010: 077c 0164 0119 00a1 0101 0064 0053 007c  .|.d.......d.S.|
-00002020: 05a0 07a1 0001 0064 0053 007c 0164 0519  .......d.S.|.d..
-00002030: 007d 0674 067c 0183 0164 016b 0472 5c7c  .}.t.|...d.k.r\|
-00002040: 0164 0119 0064 0676 0072 5c74 087c 0683  .d...d.v.r\t.|..
-00002050: 017d 0774 097c 0783 0101 0064 0053 007c  .}.t.|.....d.S.|
-00002060: 067c 0076 0172 8b7a 0f74 0183 007d 087c  .|.v.r.z.t...}.|
-00002070: 086a 0a7c 0164 0164 0085 0219 008e 0001  .j.|.d.d........
-00002080: 0057 0064 0053 0004 0074 0b79 8a01 007d  .W.d.S...t.y...}
-00002090: 0901 007a 0f74 0c7c 0983 0101 007c 05a0  ...z.t.|.....|..
-000020a0: 07a1 0001 0057 0059 0064 007d 097e 0964  .....W.Y.d.}.~.d
-000020b0: 0053 0064 007d 097e 0977 0177 0074 0464  .S.d.}.~.w.w.t.d
-000020c0: 0764 0484 007c 007c 0619 0044 0083 0183  .d...|.|...D....
-000020d0: 017d 0a74 0d7c 027c 0a83 025c 027d 0b7d  .}.t.|.|...\.}.}
-000020e0: 0c7c 0664 086b 0272 ab74 016a 0e7c 0b69  .|.d.k.r.t.j.|.i
-000020f0: 007c 0ca4 018e 0101 0064 0053 0074 0183  .|.......d.S.t..
-00002100: 007d 0874 0f7c 087c 0683 0272 bf74 107c  .}.t.|.|...r.t.|
-00002110: 087c 0683 027c 0b69 007c 0ca4 018e 0101  .|...|.i.|......
-00002120: 0064 0053 0074 067c 0b83 0164 096b 0272  .d.S.t.|...d.k.r
-00002130: cc7c 086a 0a7c 0b8e 0001 0064 0053 0064  .|.j.|.....d.S.d
-00002140: 0053 0029 0a4e 7201 0000 0029 03da 0468  .S.).Nr....)...h
-00002150: 656c 70fa 062d 2d68 656c 70fa 022d 6863  elp..--help..-hc
-00002160: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00002170: 0500 0000 7300 0000 731c 0000 0081 007c  ....s...s......|
-00002180: 005d 097d 017c 01a0 0064 0064 01a1 0256  .].}.|...d.d...V
-00002190: 0001 0071 0264 0253 0029 0372 1b00 0000  ...q.d.S.).r....
-000021a0: fa01 2d4e 2901 da07 7265 706c 6163 6529  ..-N)...replace)
-000021b0: 0272 0d00 0000 7267 0000 0072 0c00 0000  .r....rg...r....
-000021c0: 720c 0000 0072 1000 0000 7211 0000 0031  r....r....r....1
-000021d0: 0100 0073 0400 0000 0280 1a00 7a17 6d61  ...s........z.ma
-000021e0: 696e 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  in.<locals>.<gen
-000021f0: 6578 7072 3e72 0600 0000 2902 7293 0000  expr>r....).r...
-00002200: 0072 9400 0000 6301 0000 0000 0000 0000  .r....c.........
-00002210: 0000 0002 0000 0003 0000 0073 0000 0073  ...........s...s
-00002220: 3200 0000 8100 7c00 5d14 7d01 7c01 6a00  2.....|.].}.|.j.
-00002230: 7401 6a02 6a03 6b03 7216 7c01 6a00 7401  t.j.j.k.r.|.j.t.
-00002240: 6a02 6a04 6b03 7202 7c01 6a05 5600 0100  j.j.k.r.|.j.V...
-00002250: 7102 6400 5300 726f 0000 0029 06da 046b  q.d.S.ro...)...k
-00002260: 696e 6472 1300 0000 da09 5061 7261 6d65  indr......Parame
-00002270: 7465 72da 0b56 4152 5f4b 4559 574f 5244  ter..VAR_KEYWORD
-00002280: da0e 5641 525f 504f 5349 5449 4f4e 414c  ..VAR_POSITIONAL
-00002290: 723c 0000 0072 2c00 0000 720c 0000 0072  r<...r,...r....r
-000022a0: 0c00 0000 7210 0000 0072 1100 0000 4a01  ....r....r....J.
-000022b0: 0000 7310 0000 0002 8004 0002 020e 010e  ..s.............
-000022c0: 0104 fd06 0304 fc72 5200 0000 7230 0000  .......rR...r0..
-000022d0: 0029 1172 2200 0000 7205 0000 0072 4b00  .).r"...r....rK.
-000022e0: 0000 da04 6172 6776 7212 0000 0072 5100  ....argvr....rQ.
-000022f0: 0000 7231 0000 0072 7100 0000 7246 0000  ..r1...rq...rF..
-00002300: 0072 0300 0000 7254 0000 00da 0945 7863  .r....rT.....Exc
-00002310: 6570 7469 6f6e da05 7072 696e 7472 9100  eption..printr..
-00002320: 0000 7252 0000 0072 8b00 0000 7215 0000  ..rR...r....r...
-00002330: 0029 0dda 076d 6574 686f 6473 7268 0000  .)...methodsrh..
-00002340: 005a 0f72 6177 5f6d 6574 686f 645f 6172  .Z.raw_method_ar
-00002350: 6773 5a09 6865 6c70 5f61 7267 73da 0761  gsZ.help_args..a
-00002360: 6374 696f 6e73 7292 0000 00da 0661 6374  ctionsr......act
-00002370: 696f 6eda 026d 6472 7300 0000 da01 6572  ion..mdrs.....er
-00002380: 6900 0000 5a08 706f 735f 6172 6773 728e  i...Z.pos_argsr.
-00002390: 0000 0072 0c00 0000 720c 0000 0072 1000  ...r....r....r..
-000023a0: 0000 da04 6d61 696e 2c01 0000 7346 0000  ....main,...sF..
-000023b0: 0008 010e 010c 0104 0116 0106 0118 020c  ................
-000023c0: 0112 010c 0208 0418 0108 010c 0108 0202  ................
-000023d0: 0106 0118 010e 0108 0116 0108 8002 fe08  ................
-000023e0: 0506 0208 fe0e 0708 0114 0106 020a 0118  ................
-000023f0: 010c 020e 0104 ff72 a300 0000 726f 0000  .......r....ro..
-00002400: 0029 1b72 4200 0000 5a0b 6d61 7465 5f63  .).rB...Z.mate_c
-00002410: 6f6e 6669 6772 0200 0000 da05 7574 696c  onfigr......util
-00002420: 7372 0300 0000 7204 0000 0072 7300 0000  sr....r....rs...
-00002430: 7205 0000 0072 1300 0000 7288 0000 0072  r....r....r....r
-00002440: 0700 0000 7208 0000 0072 0900 0000 da04  ....r....r......
-00002450: 6970 6462 da02 6f73 724b 0000 0072 2b00  ipdb..osrK...r+.
-00002460: 0000 7219 0000 0072 2200 0000 7246 0000  ..r....r"...rF..
-00002470: 0072 5000 0000 7251 0000 0072 6600 0000  .rP...rQ...rf...
-00002480: 7212 0000 0072 7900 0000 7291 0000 0072  r....ry...r....r
-00002490: a300 0000 720c 0000 0072 0c00 0000 720c  ....r....r....r.
-000024a0: 0000 0072 1000 0000 da08 3c6d 6f64 756c  ...r......<modul
-000024b0: 653e 0100 0000 7320 0000 0004 000c 0e10  e>....s ........
-000024c0: 010c 0108 0114 0108 0108 0108 010e 0308  ................
-000024d0: 0a14 080e 390e 0f26 7d0c 3c              ....9..&}.<
+00000020: 0008 0000 0040 0000 0073 cc00 0000 6400  .....@...s....d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
+00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6404  ..d.d.l.m.Z...d.
+00000050: 6405 6c06 5a06 6404 6406 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
+00000060: 6d09 5a09 6d0a 5a0a 0100 6404 6405 6c0b  m.Z.m.Z...d.d.l.
+00000070: 5a0b 6404 6405 6c0c 5a0c 6404 6405 6c0d  Z.d.d.l.Z.d.d.l.
+00000080: 5a0d 6407 650e 6602 6408 6409 8404 5a0f  Z.d.e.f.d.d...Z.
+00000090: 640a 640b 8400 5a10 641a 640c 6508 6509  d.d...Z.d.d.e.e.
+000000a0: 1900 6602 640d 640e 8405 5a11 640f 650e  ..f.d.d...Z.d.e.
+000000b0: 6602 6410 6411 8404 5a12 4700 6412 6413  f.d.d...Z.G.d.d.
+000000c0: 8400 6413 8302 5a13 6414 6514 650e 1900  ..d...Z.d.e.e...
+000000d0: 6415 6515 6509 1900 640f 6515 6514 6516  d.e.e...d.e.e.e.
+000000e0: 6602 1900 6606 6416 6417 8404 5a17 6418  f...f.d.d...Z.d.
+000000f0: 6419 8400 5a18 6405 5300 291b 614a 0100  d...Z.d.S.).aJ..
+00000100: 000a 2323 2043 6c69 2050 6172 7365 720a  ..## Cli Parser.
+00000110: 0a4d 6174 6527 7320 636c 6920 7061 7273  .Mate's cli pars
+00000120: 6572 2069 7320 6120 7369 6d70 6c65 2070  er is a simple p
+00000130: 6172 7365 7220 7468 6174 2070 6172 7365  arser that parse
+00000140: 7320 7468 6520 636f 6d6d 616e 6420 6c69  s the command li
+00000150: 6e65 2061 7267 756d 656e 7473 2061 6e64  ne arguments and
+00000160: 2063 616c 6c73 2074 6865 2061 7070 726f   calls the appro
+00000170: 7072 6961 7465 206d 6574 686f 6420 6f6e  priate method on
+00000180: 2074 6865 204d 6174 6520 636c 6173 732e   the Mate class.
+00000190: 0a0a 4e6f 7469 6365 2074 6861 7420 666f  ..Notice that fo
+000001a0: 7220 626f 6f6c 6561 6e20 6172 6775 6d65  r boolean argume
+000001b0: 6e74 732c 2079 6f75 2063 616e 2075 7365  nts, you can use
+000001c0: 2065 6974 6865 7220 6661 6c73 6520 6f72   either false or
+000001d0: 2046 616c 7365 2c20 7472 7565 206f 7220   False, true or 
+000001e0: 5472 7565 2e20 416e 6420 666f 7220 4e6f  True. And for No
+000001f0: 6e65 2079 6f75 2063 616e 2075 7365 2065  ne you can use e
+00000200: 6974 6865 7220 6e75 6c6c 206f 7220 4e6f  ither null or No
+00000210: 6e65 2e0a 0a2a 2a45 7861 6d70 6c65 2a2a  ne...**Example**
+00000220: 0a0a 6060 600a 6d61 7465 2069 6e69 7420  ..```.mate init 
+00000230: 6d79 5f70 726f 6a65 6374 2076 656e 763d  my_project venv=
+00000240: 6661 6c73 650a 6060 600a 0ae9 0100 0000  false.```.......
+00000250: 2902 da0e 7072 696e 745f 6d61 726b 646f  )...print_markdo
+00000260: 776e da0d 7265 6d6f 7665 5f69 6e64 656e  wn..remove_inden
+00000270: 7429 01da 044d 6174 65e9 0000 0000 4e29  t)...Mate.....N)
+00000280: 03da 084f 7074 696f 6e61 6cda 0843 616c  ...Optional..Cal
+00000290: 6c61 626c 65da 0553 697a 6564 da0b 6d65  lable..Sized..me
+000002a0: 7468 6f64 5f6e 616d 6563 0200 0000 0000  thod_namec......
+000002b0: 0000 0000 0000 0200 0000 0700 0000 4300  ..............C.
+000002c0: 0000 7324 0000 0074 0064 0164 0284 0074  ..s$...t.d.d...t
+000002d0: 01a0 0274 037c 007c 0183 02a1 016a 04a0  ...t.|.|.....j..
+000002e0: 05a1 0044 0083 0183 0153 0029 034e 6301  ...D.....S.).Nc.
+000002f0: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+00000300: 0000 0073 0000 0073 2000 0000 8100 7c00  ...s...s .....|.
+00000310: 5d0b 5c02 7d01 7d02 7c01 6400 6b03 7202  ].\.}.}.|.d.k.r.
+00000320: 7c02 5600 0100 7102 6401 5300 2902 da04  |.V...q.d.S.)...
+00000330: 7365 6c66 4ea9 0029 03da 022e 30da 046e  selfN..)....0..n
+00000340: 616d 65da 0376 616c 720b 0000 0072 0b00  ame..valr....r..
+00000350: 0000 fa38 2f68 6f6d 652f 616c 2f47 6974  ...8/home/al/Git
+00000360: 4875 622f 7965 7262 616d 6174 652f 7061  Hub/yerbamate/pa
+00000370: 636b 6167 6573 2f79 6572 6261 6d61 7465  ckages/yerbamate
+00000380: 2f6d 6174 655f 636c 692e 7079 da09 3c67  /mate_cli.py..<g
+00000390: 656e 6578 7072 3e19 0000 0073 0e00 0000  enexpr>....s....
+000003a0: 0280 0400 0602 0803 02fc 0604 04fb 7a24  ..............z$
+000003b0: 5f5f 7061 7273 655f 7369 676e 6174 7572  __parse_signatur
+000003c0: 652e 3c6c 6f63 616c 733e 2e3c 6765 6e65  e.<locals>.<gene
+000003d0: 7870 723e 2906 da05 7475 706c 65da 0769  xpr>)...tuple..i
+000003e0: 6e73 7065 6374 da09 7369 676e 6174 7572  nspect..signatur
+000003f0: 65da 0767 6574 6174 7472 da0a 7061 7261  e..getattr..para
+00000400: 6d65 7465 7273 da05 6974 656d 7329 02da  meters..items)..
+00000410: 0a63 6c61 7373 5f6e 616d 6572 0900 0000  .class_namer....
+00000420: 720b 0000 0072 0b00 0000 720f 0000 00da  r....r....r.....
+00000430: 115f 5f70 6172 7365 5f73 6967 6e61 7475  .__parse_signatu
+00000440: 7265 1800 0000 730c 0000 0008 0104 0208  re....s.........
+00000450: 0102 ff06 0208 fc72 1800 0000 6301 0000  .......r....c...
+00000460: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000470: 0003 0000 0073 1800 0000 8700 6601 6401  .....s......f.d.
+00000480: 6402 8408 8800 6a00 a001 a100 4400 8301  d.....j.....D...
+00000490: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
+000004a0: 0000 0200 0000 0600 0000 1300 0000 7322  ..............s"
+000004b0: 0000 0069 007c 005d 0d7d 017c 01a0 0064  ...i.|.].}.|...d
+000004c0: 00a1 0173 027c 0174 0188 007c 0183 0293  ...s.|.t...|....
+000004d0: 0271 0253 00a9 01da 015f 2902 da0a 7374  .q.S....._)...st
+000004e0: 6172 7473 7769 7468 7218 0000 0029 0272  artswithr....).r
+000004f0: 0c00 0000 da01 6ba9 0172 1700 0000 720b  ......k..r....r.
+00000500: 0000 0072 0f00 0000 da0a 3c64 6963 7463  ...r......<dictc
+00000510: 6f6d 703e 2300 0000 730c 0000 0006 0002  omp>#...s.......
+00000520: 0208 0102 fd0a 0106 ff7a 305f 5f67 6574  .........z0__get
+00000530: 5f6d 6574 686f 6473 5f77 6974 685f 6172  _methods_with_ar
+00000540: 6775 6d65 6e74 732e 3c6c 6f63 616c 733e  guments.<locals>
+00000550: 2e3c 6469 6374 636f 6d70 3e29 02da 085f  .<dictcomp>)..._
+00000560: 5f64 6963 745f 5fda 046b 6579 7372 1d00  _dict__..keysr..
+00000570: 0000 720b 0000 0072 1d00 0000 720f 0000  ..r....r....r...
+00000580: 00da 1c5f 5f67 6574 5f6d 6574 686f 6473  ...__get_methods
+00000590: 5f77 6974 685f 6172 6775 6d65 6e74 7322  _with_arguments"
+000005a0: 0000 0073 0600 0000 0a01 0802 06fe 7221  ...s..........r!
+000005b0: 0000 00da 066d 656d 6265 7263 0200 0000  .....memberc....
+000005c0: 0000 0000 0000 0000 0900 0000 0800 0000  ................
+000005d0: 0300 0000 73e8 0000 007c 0164 0075 0072  ....s....|.d.u.r
+000005e0: 0974 0074 017c 0083 027d 017c 0164 0075  .t.t.|...}.|.d.u
+000005f0: 0173 0f4a 0082 0174 02a0 037c 01a1 016a  .s.J...t...|...j
+00000600: 04a0 05a1 007d 0264 01a0 0664 0264 0384  .....}.d...d.d..
+00000610: 007c 0244 0083 01a1 017d 0364 0464 0584  .|.D.....}.d.d..
+00000620: 0064 0664 0384 0074 077c 016a 0883 01a0  .d.d...t.|.j....
+00000630: 0964 07a1 0144 0083 0144 0083 0189 0087  .d...D...D......
+00000640: 0066 0164 0864 0384 087c 0244 0083 017d  .f.d.d...|.D...}
+00000650: 0464 07a0 067c 04a1 017d 0564 07a0 0664  .d...|...}.d...d
+00000660: 0964 0384 0074 077c 016a 0883 01a0 0964  .d...t.|.j.....d
+00000670: 07a1 0144 0083 01a1 017d 0674 0a64 0a7c  ...D.....}.t.d.|
+00000680: 009b 0064 017c 039b 0064 0b9d 0583 01a0  ...d.|...d......
+00000690: 0ba1 007d 0774 0a64 077c 079b 0064 0c7c  ...}.t.d.|...d.|
+000006a0: 05a0 0ba1 009b 0064 0d74 0a7c 0683 019b  .......d.t.|....
+000006b0: 0064 0e9d 0783 017d 0874 0a7c 0883 0153  .d.....}.t.|...S
+000006c0: 0029 0f4e fa01 2063 0100 0000 0000 0000  .).N.. c........
+000006d0: 0000 0000 0200 0000 0700 0000 5300 0000  ............S...
+000006e0: 7342 0000 0067 007c 005d 1d7d 017c 016a  sB...g.|.].}.|.j
+000006f0: 0064 006b 0372 0264 017c 016a 009b 007c  .d.k.r.d.|.j...|
+00000700: 016a 0174 026a 036b 0372 1a64 0274 047c  .j.t.j.k.r.d.t.|
+00000710: 016a 0183 0117 006e 0164 039b 0064 049d  .j.....n.d...d..
+00000720: 0491 0271 0253 0029 0572 0a00 0000 fa01  ...q.S.).r......
+00000730: 3cfa 013d da00 fa01 3e29 0572 0d00 0000  <..=....>).r....
+00000740: da07 6465 6661 756c 7472 1200 0000 da06  ..defaultr......
+00000750: 5f65 6d70 7479 da03 7374 72a9 0272 0c00  _empty..str..r..
+00000760: 0000 da05 7061 7261 6d72 0b00 0000 720b  ....paramr....r.
+00000770: 0000 0072 0f00 0000 da0a 3c6c 6973 7463  ...r......<listc
+00000780: 6f6d 703e 3000 0000 730a 0000 0006 0002  omp>0...s.......
+00000790: 020a 012a fe06 027a 206d 6574 686f 645f  ...*...z method_
+000007a0: 746f 5f6d 642e 3c6c 6f63 616c 733e 2e3c  to_md.<locals>.<
+000007b0: 6c69 7374 636f 6d70 3e63 0100 0000 0000  listcomp>c......
+000007c0: 0000 0000 0000 0200 0000 0800 0000 5300  ..............S.
+000007d0: 0000 7348 0000 0069 007c 005d 207d 0174  ..sH...i.|.] }.t
+000007e0: 007c 0183 0164 006b 0472 027c 0164 0019  .|...d.k.r.|.d..
+000007f0: 00a0 0164 01a1 0172 027c 0164 0019 00a0  ...d...r.|.d....
+00000800: 0264 02a1 0164 0019 0064 03a0 037c 0164  .d...d...d...|.d
+00000810: 0464 0585 0219 00a1 0193 0271 0253 0029  .d.........q.S.)
+00000820: 0672 0100 0000 722c 0000 0072 2300 0000  .r....r,...r#...
+00000830: fa01 3ae9 0200 0000 4e29 04da 036c 656e  ..:.....N)...len
+00000840: 721b 0000 00da 0573 706c 6974 da04 6a6f  r......split..jo
+00000850: 696e a902 720c 0000 00da 046c 696e 6572  in..r......liner
+00000860: 0b00 0000 720b 0000 0072 0f00 0000 721e  ....r....r....r.
+00000870: 0000 0036 0000 0073 0a00 0000 0600 0202  ...6...s........
+00000880: 1a01 20fe 0602 7a20 6d65 7468 6f64 5f74  .. ...z method_t
+00000890: 6f5f 6d64 2e3c 6c6f 6361 6c73 3e2e 3c64  o_md.<locals>.<d
+000008a0: 6963 7463 6f6d 703e 6301 0000 0000 0000  ictcomp>c.......
+000008b0: 0000 0000 0002 0000 0005 0000 0053 0000  .............S..
+000008c0: 0073 1a00 0000 6700 7c00 5d09 7d01 7c01  .s....g.|.].}.|.
+000008d0: a000 a100 a001 6400 a101 9102 7102 5300  ......d.....q.S.
+000008e0: 2901 722e 0000 0029 02da 0573 7472 6970  ).r....)...strip
+000008f0: 7231 0000 0029 0272 0c00 0000 da01 6c72  r1...).r......lr
+00000900: 0b00 0000 720b 0000 0072 0f00 0000 722d  ....r....r....r-
+00000910: 0000 0038 0000 00f3 0200 0000 1a00 da01  ...8............
+00000920: 0a63 0100 0000 0000 0000 0000 0000 0200  .c..............
+00000930: 0000 0b00 0000 1300 0000 7358 0000 0067  ..........sX...g
+00000940: 007c 005d 287d 017c 016a 0064 006b 0372  .|.](}.|.j.d.k.r
+00000950: 0264 017c 016a 009b 0064 027c 016a 016a  .d.|.j...d.|.j.j
+00000960: 029b 0064 0388 00a0 037c 016a 0064 04a1  ...d.....|.j.d..
+00000970: 029b 009d 067c 016a 0474 056a 066b 0372  .....|.j.t.j.k.r
+00000980: 2764 057c 016a 049b 009d 026e 0164 0417  'd.|.j.....n.d..
+00000990: 0091 0271 0253 0029 0672 0a00 0000 fa02  ...q.S.).r......
+000009a0: 2d20 7a04 203a 2060 fa04 6020 3a20 7226  - z. : `..` : r&
+000009b0: 0000 0072 2500 0000 2907 720d 0000 00da  ...r%...).r.....
+000009c0: 0a61 6e6e 6f74 6174 696f 6eda 085f 5f6e  .annotation..__n
+000009d0: 616d 655f 5fda 0367 6574 7228 0000 0072  ame__..getr(...r
+000009e0: 1200 0000 7229 0000 0072 2b00 0000 a901  ....r)...r+.....
+000009f0: 5a12 7061 7261 6d5f 6465 7363 7269 7074  Z.param_descript
+00000a00: 696f 6e73 720b 0000 0072 0f00 0000 722d  ionsr....r....r-
+00000a10: 0000 003c 0000 0073 0e00 0000 0600 0203  ...<...s........
+00000a20: 0a01 24fd 1a01 02ff 0603 6301 0000 0000  ..$.......c.....
+00000a30: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
+00000a40: 0000 0073 1e00 0000 6700 7c00 5d0b 7d01  ...s....g.|.].}.
+00000a50: 7c01 a000 a100 a001 6400 a101 7302 7c01  |.......d...s.|.
+00000a60: 9102 7102 5300 2901 7a06 3a70 6172 616d  ..q.S.).z.:param
+00000a70: 2902 7235 0000 0072 1b00 0000 7233 0000  ).r5...r....r3..
+00000a80: 0072 0b00 0000 720b 0000 0072 0f00 0000  .r....r....r....
+00000a90: 722d 0000 0044 0000 0073 0c00 0000 0600  r-...D...s......
+00000aa0: 0202 0c01 02fd 0201 06ff 7518 0000 000a  ..........u.....
+00000ab0: 2020 2020 6060 600a 2020 2020 2020 e29d      ```.      ..
+00000ac0: af20 6d61 7465 207a 0d0a 2020 2020 6060  . mate z..    ``
+00000ad0: 600a 2020 2020 7a0e 0a0a 2a2a 5061 7261  `.    z...**Para
+00000ae0: 6d73 2a2a 0a0a fa02 0a0a 7a06 0a0a 2d2d  ms**......z...--
+00000af0: 2d0a 290c 7214 0000 005a 074d 6174 6543  -.).r....Z.MateC
+00000b00: 4c49 7212 0000 0072 1300 0000 7215 0000  LIr....r....r...
+00000b10: 00da 0676 616c 7565 7372 3200 0000 722a  ...valuesr2...r*
+00000b20: 0000 00da 075f 5f64 6f63 5f5f 7231 0000  .....__doc__r1..
+00000b30: 0072 0300 0000 7235 0000 0029 0972 0900  .r....r5...).r..
+00000b40: 0000 7222 0000 00da 0670 6172 616d 735a  ..r".....paramsZ
+00000b50: 0d69 6e6c 696e 655f 7061 7261 6d73 5a0f  .inline_paramsZ.
+00000b60: 7261 775f 6c69 7374 5f70 6172 616d 735a  raw_list_paramsZ
+00000b70: 0b6c 6973 745f 7061 7261 6d73 5a12 6d65  .list_paramsZ.me
+00000b80: 7468 6f64 5f64 6573 6372 6970 7469 6f6e  thod_description
+00000b90: da04 636f 6465 da03 646f 6372 0b00 0000  ..code..docr....
+00000ba0: 723e 0000 0072 0f00 0000 da0c 6d65 7468  r>...r......meth
+00000bb0: 6f64 5f74 6f5f 6d64 2a00 0000 7350 0000  od_to_md*...sP..
+00000bc0: 0008 010a 010c 0110 0104 0106 0102 0204  ................
+00000bd0: fe04 ff06 0718 0206 fe0a 0602 0306 fd0a  ................
+00000be0: 0604 0106 010e 0204 fe04 ff02 0802 0102  ................
+00000bf0: 0204 fe02 0206 fe02 ff04 0602 fa02 0702  ................
+00000c00: 0102 0104 ff06 0504 fb06 0706 f904 ff08  ................
+00000c10: 0e72 4500 0000 da06 7265 7475 726e 6300  .rE.....returnc.
+00000c20: 0000 0000 0000 0000 0000 0005 0000 0005  ................
+00000c30: 0000 0043 0000 0073 6800 0000 7400 7401  ...C...sh...t.t.
+00000c40: 7402 6a03 8301 8301 6401 1700 7d00 7401  t.j.....d...}.t.
+00000c50: 7404 6a05 7406 1900 6a03 8301 7d01 7c00  t.j.t...j...}.|.
+00000c60: 7c01 6401 1700 3700 7d00 6402 6403 8400  |.d...7.}.d.d...
+00000c70: 7407 6a08 7402 7407 6a09 6404 8d02 4400  t.j.t.t.j.d...D.
+00000c80: 8301 7d02 7c02 4400 5d0b 5c02 7d03 7d04  ..}.|.D.].\.}.}.
+00000c90: 7c00 740a 7c03 7c04 8302 3700 7d00 7126  |.t.|.|...7.}.q&
+00000ca0: 7c00 5300 2905 4efa 070a 202d 2d2d 200a  |.S.).N... --- .
+00000cb0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00000cc0: 0005 0000 0053 0000 0073 2200 0000 6700  .....S...s"...g.
+00000cd0: 7c00 5d0d 5c02 7d01 7d02 7c01 a000 6400  |.].\.}.}.|...d.
+00000ce0: a101 7302 7c01 7c02 6602 9102 7102 5300  ..s.|.|.f...q.S.
+00000cf0: 7219 0000 0029 0172 1b00 0000 2903 720c  r....).r....).r.
+00000d00: 0000 0072 1c00 0000 da01 7672 0b00 0000  ...r......vr....
+00000d10: 720b 0000 0072 0f00 0000 722d 0000 0068  r....r....r-...h
+00000d20: 0000 0073 0c00 0000 0600 0602 0801 02fd  ...s............
+00000d30: 0601 06ff 7a24 6765 6e65 7261 7465 5f68  ....z$generate_h
+00000d40: 656c 705f 6d64 2e3c 6c6f 6361 6c73 3e2e  elp_md.<locals>.
+00000d50: 3c6c 6973 7463 6f6d 703e 2901 da09 7072  <listcomp>)...pr
+00000d60: 6564 6963 6174 6529 0b72 0300 0000 722a  edicate).r....r*
+00000d70: 0000 0072 0400 0000 7241 0000 00da 0373  ...r....rA.....s
+00000d80: 7973 da07 6d6f 6475 6c65 7372 3c00 0000  ys..modulesr<...
+00000d90: 7212 0000 00da 0a67 6574 6d65 6d62 6572  r......getmember
+00000da0: 73da 0a69 7366 756e 6374 696f 6e72 4500  s..isfunctionrE.
+00000db0: 0000 2905 7244 0000 005a 1163 7572 7265  ..).rD...Z.curre
+00000dc0: 6e74 5f64 6f63 7374 7269 6e67 da07 6d65  nt_docstring..me
+00000dd0: 6d62 6572 7372 0d00 0000 720e 0000 0072  mbersr....r....r
+00000de0: 0b00 0000 720b 0000 0072 0f00 0000 da10  ....r....r......
+00000df0: 6765 6e65 7261 7465 5f68 656c 705f 6d64  generate_help_md
+00000e00: 6300 0000 7312 0000 0012 0210 010c 0106  c...s...........
+00000e10: 010e 0206 fe0c 0510 0104 0172 4f00 0000  ...........rO...
+00000e20: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000e30: 0005 0000 0040 0000 0073 6200 0000 6500  .....@...sb...e.
+00000e40: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
+00000e50: 6404 8400 5a04 6405 6406 8400 5a05 6412  d...Z.d.d...Z.d.
+00000e60: 6408 6506 6409 640a 6604 640b 640c 8405  d.e.d.d.f.d.d...
+00000e70: 5a07 6413 6408 6506 6409 6506 6604 640e  Z.d.d.e.d.e.f.d.
+00000e80: 640f 8405 5a08 6409 6509 6506 6506 6602  d...Z.d.e.e.e.f.
+00000e90: 1900 6602 6410 6411 8404 5a0a 640a 5300  ..f.d.d...Z.d.S.
+00000ea0: 2914 da08 4d61 7465 4865 6c70 6301 0000  )...MateHelpc...
+00000eb0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000ec0: 0043 0000 0073 2200 0000 6401 7c00 5f00  .C...s"...d.|._.
+00000ed0: 6402 7c00 5f01 7c00 a002 7403 a101 5c02  d.|._.|...t...\.
+00000ee0: 7c00 5f04 7c00 5f05 6400 5300 2903 4e29  |._.|._.d.S.).N)
+00000ef0: 07da 0469 6e69 74da 0769 6e73 7461 6c6c  ...init..install
+00000f00: da05 7472 6169 6eda 0461 7574 6f5a 0665  ..train..autoZ.e
+00000f10: 7870 6f72 74da 0563 6c6f 6e65 da04 7465  xport..clone..te
+00000f20: 7374 2907 7a18 496e 6974 6961 6c69 7a65  st).z.Initialize
+00000f30: 2061 206e 6577 2070 726f 6a65 6374 7a14   a new projectz.
+00000f40: 496e 7374 616c 6c20 6465 7065 6e64 656e  Install dependen
+00000f50: 6369 6573 7a0d 5472 6169 6e20 6120 6d6f  ciesz.Train a mo
+00000f60: 6465 6c7a 3456 6172 696f 7573 2063 6f6d  delz4Various com
+00000f70: 6d61 6e64 7320 746f 2068 656c 7020 7769  mands to help wi
+00000f80: 7468 2074 6865 2064 6576 656c 6f70 6d65  th the developme
+00000f90: 6e74 2070 726f 6365 737a 1345 7870 6f72  nt procesz.Expor
+00000fa0: 7420 6465 7065 6e64 656e 6369 6573 7a17  t dependenciesz.
+00000fb0: 436c 6f6e 6573 2069 6e74 6572 6e61 6c20  Clones internal 
+00000fc0: 6d6f 6475 6c65 737a 0c54 6573 7420 6120  modulesz.Test a 
+00000fd0: 6d6f 6465 6c29 06da 0c68 656c 705f 6f70  model)...help_op
+00000fe0: 7469 6f6e 73da 0d68 656c 705f 636f 6d6d  tions..help_comm
+00000ff0: 656e 7473 da0d 6765 745f 6675 6c6c 5f64  ents..get_full_d
+00001000: 6f63 7372 0400 0000 5a0a 5f66 756c 6c5f  ocsr....Z._full_
+00001010: 646f 6373 da08 5f6d 6574 686f 6473 a901  docs.._methods..
+00001020: 720a 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
+00001030: 0f00 0000 da08 5f5f 696e 6974 5f5f 7300  ......__init__s.
+00001040: 0000 7306 0000 0006 0106 0916 0a7a 114d  ..s..........z.M
+00001050: 6174 6548 656c 702e 5f5f 696e 6974 5f5f  ateHelp.__init__
+00001060: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00001070: 0006 0000 0043 0000 0073 3a00 0000 6401  .....C...s:...d.
+00001080: 7d01 6402 6403 8400 7400 7c00 6a01 7c00  }.d.d...t.|.j.|.
+00001090: 6a02 8302 4400 8301 7d02 7403 6404 6405  j...D...}.t.d.d.
+000010a0: 7c01 6406 1700 a004 7c02 a101 1700 9b00  |.d.....|.......
+000010b0: 6407 9d03 8301 5300 2908 4e72 3800 0000  d.....S.).Nr8...
+000010c0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+000010d0: 0006 0000 0053 0000 0073 2000 0000 6700  .....S...s ...g.
+000010e0: 7c00 5d0c 5c02 7d01 7d02 6400 7c01 9b00  |.].\.}.}.d.|...
+000010f0: 6401 7c02 9b00 9d04 9102 7102 5300 2902  d.|.......q.S.).
+00001100: fa01 6072 3a00 0000 720b 0000 0029 0372  ..`r:...r....).r
+00001110: 0c00 0000 da06 6f70 7469 6f6e da07 636f  ......option..co
+00001120: 6d6d 656e 7472 0b00 0000 720b 0000 0072  mmentr....r....r
+00001130: 0f00 0000 722d 0000 0091 0000 0073 0800  ....r-.......s..
+00001140: 0000 0600 0602 0eff 06ff 7a26 4d61 7465  ..........z&Mate
+00001150: 4865 6c70 2e67 6574 5f69 6e64 6578 2e3c  Help.get_index.<
+00001160: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00001170: 703e 7ac2 0a20 2020 2020 2020 2023 2048  p>z..        # H
+00001180: 656c 7020 496e 6465 780a 0a20 2020 2020  elp Index..     
+00001190: 2020 204d 6174 652c 2079 6f75 7220 6672     Mate, your fr
+000011a0: 6965 6e64 6c79 204d 4c20 7072 6f6a 6563  iendly ML projec
+000011b0: 7420 6d61 6e61 6765 722e 0a20 2020 2020  t manager..     
+000011c0: 2020 200a 2020 2020 2020 2020 5479 7065     .        Type
+000011d0: 2060 6d61 7465 2068 656c 7020 3c6f 7074   `mate help <opt
+000011e0: 696f 6e3e 6020 746f 2067 6574 206d 6f72  ion>` to get mor
+000011f0: 6520 696e 666f 726d 6174 696f 6e20 6162  e information ab
+00001200: 6f75 7420 6120 746f 7069 632e 0a0a 2020  out a topic...  
+00001210: 2020 2020 2020 4176 6169 6c61 626c 6520        Available 
+00001220: 6f70 7469 6f6e 7320 6172 653a 0a0a 2020  options are:..  
+00001230: 2020 2020 2020 7239 0000 007a 0320 2d20        r9...z. - 
+00001240: 7a09 0a20 2020 2020 2020 2029 05da 037a  z..        )...z
+00001250: 6970 7257 0000 0072 5800 0000 7203 0000  iprW...rX...r...
+00001260: 0072 3200 0000 2903 720a 0000 00da 026e  .r2...).r......n
+00001270: 6c5a 0568 656c 7073 720b 0000 0072 0b00  lZ.helpsr....r..
+00001280: 0000 720f 0000 00da 0967 6574 5f69 6e64  ..r......get_ind
+00001290: 6578 8d00 0000 7312 0000 0004 0106 030c  ex....s.........
+000012a0: 0206 fe02 0402 0110 0906 f704 ff7a 124d  .............z.M
+000012b0: 6174 6548 656c 702e 6765 745f 696e 6465  ateHelp.get_inde
+000012c0: 7863 0200 0000 0000 0000 0000 0000 0500  xc..............
+000012d0: 0000 0700 0000 0300 0000 7356 0000 0074  ..........sV...t
+000012e0: 007c 016a 0183 0164 0117 007d 0264 0264  .|.j...d...}.d.d
+000012f0: 0384 0089 0087 0066 0164 0464 0584 0874  .......f.d.d...t
+00001300: 02a0 037c 0174 026a 04a1 0244 0083 017d  ...|.t.j...D...}
+00001310: 0364 067d 047c 029b 0064 0774 007c 04a0  .d.}.|...d.t.|..
+00001320: 057c 03a0 06a1 00a1 0183 019b 009d 037c  .|.............|
+00001330: 0366 0253 0029 084e 7a08 0a0a 202d 2d2d  .f.S.).Nz... ---
+00001340: 200a 6302 0000 0000 0000 0000 0000 0008   .c.............
+00001350: 0000 0005 0000 0053 0000 0073 6e00 0000  .......S...sn...
+00001360: 7400 7c01 6a01 8301 7d02 7402 a003 7c01  t.|.j...}.t...|.
+00001370: a101 7d03 7404 7c03 6a05 a006 a100 8301  ..}.t.|.j.......
+00001380: 7d04 7c04 6401 1900 6a07 6402 6b03 7d05  }.|.d...j.d.k.}.
+00001390: 6403 6404 8400 7c04 4400 8301 7d04 6405  d.d...|.D...}.d.
+000013a0: a008 6406 6404 8400 7404 7c04 8301 4400  ..d.d...t.|...D.
+000013b0: 8301 a101 7d06 6407 7c00 9b00 6408 9d03  ....}.d.|...d...
+000013c0: 7d07 7c07 7c02 1700 6409 1700 5300 290a  }.|.|...d...S.).
+000013d0: 4e72 0500 0000 720a 0000 0063 0100 0000  Nr....r....c....
+000013e0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000013f0: 5300 0000 731a 0000 0067 007c 005d 097d  S...s....g.|.].}
+00001400: 017c 016a 0064 006b 0372 027c 0191 0271  .|.j.d.k.r.|...q
+00001410: 0253 0072 5b00 0000 2901 720d 0000 0029  .S.r[...).r....)
+00001420: 0272 0c00 0000 da03 6172 6772 0b00 0000  .r......argr....
+00001430: 720b 0000 0072 0f00 0000 722d 0000 00ab  r....r....r-....
+00001440: 0000 0072 3700 0000 7a42 4d61 7465 4865  ...r7...zBMateHe
+00001450: 6c70 2e67 6574 5f66 756c 6c5f 646f 6373  lp.get_full_docs
+00001460: 2e3c 6c6f 6361 6c73 3e2e 6765 745f 6d65  .<locals>.get_me
+00001470: 7468 6f64 5f64 6f63 2e3c 6c6f 6361 6c73  thod_doc.<locals
+00001480: 3e2e 3c6c 6973 7463 6f6d 703e 7a02 2c20  >.<listcomp>z., 
+00001490: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000014a0: 0004 0000 0053 0000 0073 1400 0000 6700  .....S...s....g.
+000014b0: 7c00 5d06 7d01 7400 7c01 8301 9102 7102  |.].}.t.|.....q.
+000014c0: 5300 720b 0000 0029 0172 2a00 0000 2902  S.r....).r*...).
+000014d0: 720c 0000 00da 0161 720b 0000 0072 0b00  r......ar....r..
+000014e0: 0000 720f 0000 0072 2d00 0000 ac00 0000  ..r....r-.......
+000014f0: 7302 0000 0014 007a 0b23 2323 2060 6d61  s......z.### `ma
+00001500: 7465 6020 7238 0000 0072 4700 0000 2909  te` r8...rG...).
+00001510: 7203 0000 0072 4100 0000 7212 0000 0072  r....rA...r....r
+00001520: 1300 0000 da04 6c69 7374 7215 0000 0072  ......listr....r
+00001530: 4000 0000 720d 0000 0072 3200 0000 2908  @...r....r2...).
+00001540: 7209 0000 00da 066d 6574 686f 6472 4400  r......methodrD.
+00001550: 0000 7213 0000 00da 0461 7267 735a 0969  ..r......argsZ.i
+00001560: 735f 7374 6174 6963 da0b 616e 6e6f 7461  s_static..annota
+00001570: 7469 6f6e 73da 0668 6561 6465 7272 0b00  tions..headerr..
+00001580: 0000 720b 0000 0072 0f00 0000 da0e 6765  ..r....r......ge
+00001590: 745f 6d65 7468 6f64 5f64 6f63 a600 0000  t_method_doc....
+000015a0: 7310 0000 000a 010a 010e 010e 010e 0118  s...............
+000015b0: 010c 010c 017a 2e4d 6174 6548 656c 702e  .....z.MateHelp.
+000015c0: 6765 745f 6675 6c6c 5f64 6f63 732e 3c6c  get_full_docs.<l
+000015d0: 6f63 616c 733e 2e67 6574 5f6d 6574 686f  ocals>.get_metho
+000015e0: 645f 646f 6363 0100 0000 0000 0000 0000  d_docc..........
+000015f0: 0000 0300 0000 0700 0000 1300 0000 7332  ..............s2
+00001600: 0000 0069 007c 005d 155c 027d 017d 027c  ...i.|.].\.}.}.|
+00001610: 01a0 0064 00a1 0173 177c 026a 0164 0175  ...d...s.|.j.d.u
+00001620: 0172 027c 0188 007c 017c 0264 028d 0293  .r.|...|.|.d....
+00001630: 0271 0253 0029 0372 1a00 0000 4e29 0272  .q.S.).r....N).r
+00001640: 0900 0000 7266 0000 0029 0272 1b00 0000  ....rf...).r....
+00001650: 7241 0000 0029 0372 0c00 0000 7209 0000  rA...).r....r...
+00001660: 0072 6600 0000 a901 726a 0000 0072 0b00  .rf.....rj...r..
+00001670: 0000 720f 0000 0072 1e00 0000 b800 0000  ..r....r........
+00001680: 730e 0000 0006 0006 0208 0302 fb0a 050c  s...............
+00001690: fc06 047a 2a4d 6174 6548 656c 702e 6765  ...z*MateHelp.ge
+000016a0: 745f 6675 6c6c 5f64 6f63 732e 3c6c 6f63  t_full_docs.<loc
+000016b0: 616c 733e 2e3c 6469 6374 636f 6d70 3e72  als>.<dictcomp>r
+000016c0: 3800 0000 723f 0000 0029 0772 0300 0000  8...r?...).r....
+000016d0: 7241 0000 0072 1200 0000 724c 0000 0072  rA...r....rL...r
+000016e0: 4d00 0000 7232 0000 0072 4000 0000 2905  M...r2...r@...).
+000016f0: 720a 0000 00da 0b63 6c61 7373 5f76 616c  r......class_val
+00001700: 7565 7269 0000 005a 0b6d 6574 686f 645f  ueri...Z.method_
+00001710: 6469 6374 7261 0000 0072 0b00 0000 726b  dictra...r....rk
+00001720: 0000 0072 0f00 0000 7259 0000 00a3 0000  ...r....rY......
+00001730: 0073 1600 0000 0e01 0802 0a12 0402 0601  .s..............
+00001740: 02ff 06fe 0408 1a02 0201 04fe 7a16 4d61  ............z.Ma
+00001750: 7465 4865 6c70 2e67 6574 5f66 756c 6c5f  teHelp.get_full_
+00001760: 646f 6373 7226 0000 00da 0477 6861 7472  docsr&.....whatr
+00001770: 4600 0000 4e63 0200 0000 0000 0000 0000  F...Nc..........
+00001780: 0000 0200 0000 0300 0000 4300 0000 732c  ..........C...s,
+00001790: 0000 007c 017c 006a 0076 0072 0e74 017c  ...|.|.j.v.r.t.|
+000017a0: 006a 027c 0119 0083 0101 0064 0053 0074  .j.|.......d.S.t
+000017b0: 017c 00a0 03a1 0083 0101 0064 0053 00a9  .|.........d.S..
+000017c0: 014e 2904 7257 0000 0072 0200 0000 725a  .N).rW...r....rZ
+000017d0: 0000 0072 6200 0000 a902 720a 0000 0072  ...rb.....r....r
+000017e0: 6d00 0000 720b 0000 0072 0b00 0000 720f  m...r....r....r.
+000017f0: 0000 00da 0a70 7269 6e74 5f68 656c 70c6  .....print_help.
+00001800: 0000 0073 0600 0000 0a02 1202 1002 7a13  ...s..........z.
+00001810: 4d61 7465 4865 6c70 2e70 7269 6e74 5f68  MateHelp.print_h
+00001820: 656c 70da 0363 6c69 6302 0000 0000 0000  elp..clic.......
+00001830: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00001840: 0073 2a00 0000 7c01 6401 6b02 7207 7400  .s*...|.d.k.r.t.
+00001850: 8300 5300 7c01 6402 6b02 7212 7401 7c00  ..S.|.d.k.r.t.|.
+00001860: a002 7403 a101 8301 5300 7400 8300 5300  ..t.....S.t...S.
+00001870: 2903 4e72 7100 0000 da04 6d61 7465 2904  ).Nrq.....mate).
+00001880: 724f 0000 0072 2a00 0000 7259 0000 0072  rO...r*...rY...r
+00001890: 0400 0000 726f 0000 0072 0b00 0000 720b  ....ro...r....r.
+000018a0: 0000 0072 0f00 0000 da0b 6765 745f 6865  ...r......get_he
+000018b0: 6c70 5f6d 64dd 0000 0073 0a00 0000 0801  lp_md....s......
+000018c0: 0601 0801 0e01 0608 7a14 4d61 7465 4865  ........z.MateHe
+000018d0: 6c70 2e67 6574 5f68 656c 705f 6d64 6301  lp.get_help_mdc.
+000018e0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+000018f0: 0000 0003 0000 0073 1400 0000 8700 6601  .......s......f.
+00001900: 6401 6402 8408 8800 6a00 4400 8301 5300  d.d.....j.D...S.
+00001910: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
+00001920: 0200 0000 0600 0000 1300 0000 7318 0000  ............s...
+00001930: 0069 007c 005d 087d 017c 0188 00a0 007c  .i.|.].}.|.....|
+00001940: 01a1 0193 0271 0253 0072 0b00 0000 2901  .....q.S.r....).
+00001950: 7273 0000 0029 0272 0c00 0000 da03 6b65  rs...).r......ke
+00001960: 7972 5b00 0000 720b 0000 0072 0f00 0000  yr[...r....r....
+00001970: 721e 0000 00ec 0000 0073 0200 0000 1800  r........s......
+00001980: 7a2c 4d61 7465 4865 6c70 2e67 6574 5f61  z,MateHelp.get_a
+00001990: 6c6c 5f68 656c 705f 6d64 2e3c 6c6f 6361  ll_help_md.<loca
+000019a0: 6c73 3e2e 3c64 6963 7463 6f6d 703e 2901  ls>.<dictcomp>).
+000019b0: 7257 0000 0072 5b00 0000 720b 0000 0072  rW...r[...r....r
+000019c0: 5b00 0000 720f 0000 00da 0f67 6574 5f61  [...r......get_a
+000019d0: 6c6c 5f68 656c 705f 6d64 eb00 0000 7302  ll_help_md....s.
+000019e0: 0000 0014 017a 184d 6174 6548 656c 702e  .....z.MateHelp.
+000019f0: 6765 745f 616c 6c5f 6865 6c70 5f6d 6429  get_all_help_md)
+00001a00: 0172 2600 0000 2901 7271 0000 0029 0b72  .r&...).rq...).r
+00001a10: 3c00 0000 da0a 5f5f 6d6f 6475 6c65 5f5f  <.....__module__
+00001a20: da0c 5f5f 7175 616c 6e61 6d65 5f5f 725c  ..__qualname__r\
+00001a30: 0000 0072 6200 0000 7259 0000 0072 2a00  ...rb...rY...r*.
+00001a40: 0000 7270 0000 0072 7300 0000 da04 6469  ..rp...rs.....di
+00001a50: 6374 7275 0000 0072 0b00 0000 720b 0000  ctru...r....r...
+00001a60: 0072 0b00 0000 720f 0000 0072 5000 0000  .r....r....rP...
+00001a70: 7200 0000 730e 0000 0008 0008 0108 1a08  r...s...........
+00001a80: 1614 2314 171a 0e72 5000 0000 7267 0000  ..#....rP...rg..
+00001a90: 0072 6800 0000 6302 0000 0000 0000 0000  .rh...c.........
+00001aa0: 0000 000d 0000 0008 0000 0043 0000 0073  ...........C...s
+00001ab0: 1801 0000 6900 7d02 6700 7d03 6401 7d04  ....i.}.g.}.d.}.
+00001ac0: 6402 7400 6602 6403 6404 8404 7d05 6402  d.t.f.d.d...}.d.
+00001ad0: 7400 6602 6405 6406 8404 7d06 7401 7c01  t.f.d.d...}.t.|.
+00001ae0: 8301 7401 7c00 8301 6b00 7229 7c01 7c05  ..t.|...k.r)|.|.
+00001af0: 6601 7401 7c00 8301 7401 7c01 8301 1800  f.t.|...t.|.....
+00001b00: 1400 1700 7d01 6407 6408 6c02 6d03 7d07  ....}.d.d.l.m.}.
+00001b10: 0100 7404 7405 7c00 7c01 8302 8301 4400  ..t.t.|.|.....D.
+00001b20: 5d51 5c02 7d08 5c02 7d09 7d0a 7c0a 7406  ]Q\.}.\.}.}.|.t.
+00001b30: 6b02 7243 7c06 7d0a 6e10 7c0a 7407 6a08  k.rC|.}.n.|.t.j.
+00001b40: 6b02 724b 7c05 7d0a 6e08 7409 7c0a 6409  k.rK|.}.n.t.|.d.
+00001b50: 8302 7253 7c0a 6a0a 7d0a 640a 7c09 7600  ..rS|.j.}.d.|.v.
+00001b60: 7267 7c09 a00b 640a a101 5c02 7d0b 7d0c  rg|...d...\.}.}.
+00001b70: 7c0a 7c0c 8301 7c02 7c0b 3c00 640b 7d04  |.|...|.|.<.d.}.
+00001b80: 7136 740c 7c0a 740d 8302 7270 7c0a 6407  q6t.|.t...rp|.d.
+00001b90: 1900 7d0a 7c03 a00e 7c0a 7c09 8301 a101  ..}.|...|.|.....
+00001ba0: 0100 7c04 7287 740f 640c 7c09 9b00 640d  ..|.r.t.d.|...d.
+00001bb0: 7c00 7c08 640e 1800 1900 9b00 9d04 8301  |.|.d...........
+00001bc0: 8201 7136 7c03 7c02 6602 5300 290f 4e46  ..q6|.|.f.S.).NF
+00001bd0: 7263 0000 0063 0100 0000 0000 0000 0000  rc...c..........
+00001be0: 0000 0300 0000 0900 0000 5300 0000 7368  ..........S...sh
+00001bf0: 0000 0074 0074 0174 0267 037d 017c 00a0  ...t.t.t.g.}.|..
+00001c00: 03a1 0064 0176 0072 0d64 0053 007c 00a0  ...d.v.r.d.S.|..
+00001c10: 03a1 0064 026b 0272 1564 0353 007c 00a0  ...d.k.r.d.S.|..
+00001c20: 03a1 0064 046b 0272 1d64 0553 007c 0144  ...d.k.r.d.S.|.D
+00001c30: 005d 127d 027a 077c 027c 0083 0157 0002  .].}.z.|.|...W..
+00001c40: 0001 0053 0004 0074 0479 3101 0001 0001  ...S...t.y1.....
+00001c50: 0059 0071 1f77 0064 0053 0029 064e 2902  .Y.q.w.d.S.).N).
+00001c60: da04 6e6f 6e65 da04 6e75 6c6c da04 7472  ..none..null..tr
+00001c70: 7565 54da 0566 616c 7365 4629 05da 0369  ueT..falseF)...i
+00001c80: 6e74 da05 666c 6f61 7472 2a00 0000 da05  nt..floatr*.....
+00001c90: 6c6f 7765 72da 0a56 616c 7565 4572 726f  lower..ValueErro
+00001ca0: 7229 0372 6300 0000 da05 7479 7065 73da  r).rc.....types.
+00001cb0: 0174 720b 0000 0072 0b00 0000 720f 0000  .tr....r....r...
+00001cc0: 00da 0f67 6f6f 645f 6775 6573 735f 7479  ...good_guess_ty
+00001cd0: 7065 fa00 0000 731c 0000 000a 010c 0104  pe....s.........
+00001ce0: 010c 0104 010c 0104 0108 0102 010e 010c  ................
+00001cf0: 0104 0102 ff04 fd7a 2563 6f6c 6c65 6374  .......z%collect
+00001d00: 5f61 7267 732e 3c6c 6f63 616c 733e 2e67  _args.<locals>.g
+00001d10: 6f6f 645f 6775 6573 735f 7479 7065 6301  ood_guess_typec.
+00001d20: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00001d30: 0000 0053 0000 0073 2800 0000 7c00 a000  ...S...s(...|...
+00001d40: a100 6401 6b02 7208 6402 5300 7c00 a000  ..d.k.r.d.S.|...
+00001d50: a100 6403 6b02 7210 6404 5300 7401 6405  ..d.k.r.d.S.t.d.
+00001d60: 8301 8201 2906 4e72 7b00 0000 5472 7c00  ....).Nr{...Tr|.
+00001d70: 0000 467a 0d4e 6f74 2061 2062 6f6f 6c65  ..Fz.Not a boole
+00001d80: 616e 2902 727f 0000 0072 8000 0000 2901  an).r....r....).
+00001d90: 7263 0000 0072 0b00 0000 720b 0000 0072  rc...r....r....r
+00001da0: 0f00 0000 da0c 626f 6f6c 6561 6e5f 7479  ......boolean_ty
+00001db0: 7065 0801 0000 730a 0000 000c 0104 010c  pe....s.........
+00001dc0: 0104 0108 027a 2263 6f6c 6c65 6374 5f61  .....z"collect_a
+00001dd0: 7267 732e 3c6c 6f63 616c 733e 2e62 6f6f  rgs.<locals>.boo
+00001de0: 6c65 616e 5f74 7970 6572 0500 0000 2901  lean_typer....).
+00001df0: da05 556e 696f 6eda 085f 5f61 7267 735f  ..Union..__args_
+00001e00: 5f72 2500 0000 547a 1470 6f73 6974 696f  _r%...Tz.positio
+00001e10: 6e61 6c20 6172 6775 6d65 6e74 207a 1820  nal argument z. 
+00001e20: 6166 7465 7220 6b65 7977 6f72 6420 6172  after keyword ar
+00001e30: 6775 6d65 6e74 2072 0100 0000 2910 722a  gument r....).r*
+00001e40: 0000 0072 3000 0000 da06 7479 7069 6e67  ...r0.....typing
+00001e50: 7285 0000 00da 0965 6e75 6d65 7261 7465  r......enumerate
+00001e60: 7260 0000 00da 0462 6f6f 6c72 1200 0000  r`.....boolr....
+00001e70: 7229 0000 00da 0768 6173 6174 7472 7286  r).....hasattrr.
+00001e80: 0000 0072 3100 0000 da0a 6973 696e 7374  ...r1.....isinst
+00001e90: 616e 6365 7211 0000 00da 0661 7070 656e  ancer......appen
+00001ea0: 6472 8000 0000 290d 7267 0000 0072 6800  dr....).rg...rh.
+00001eb0: 0000 da06 6b77 6172 6773 5a0f 706f 7369  ....kwargsZ.posi
+00001ec0: 7469 6f6e 616c 5f61 7267 735a 1770 6f73  tional_argsZ.pos
+00001ed0: 6974 696f 6e61 6c5f 6172 6773 5f73 7461  itional_args_sta
+00001ee0: 7274 6564 7283 0000 0072 8400 0000 7285  rtedr....r....r.
+00001ef0: 0000 00da 0169 7263 0000 0072 3b00 0000  .....irc...r;...
+00001f00: 7274 0000 00da 0576 616c 7565 720b 0000  rt.....valuer...
+00001f10: 0072 0b00 0000 720f 0000 00da 0c63 6f6c  .r....r......col
+00001f20: 6c65 6374 5f61 7267 73ef 0000 0073 3800  lect_args....s8.
+00001f30: 0000 0407 0401 0401 0e02 0e0e 1008 1a01  ................
+00001f40: 0c01 1a02 0801 0601 0a01 0601 0a01 0601  ................
+00001f50: 0801 0e01 0c01 0601 0a02 0801 0e01 0401  ................
+00001f60: 0201 1601 04ff 02ff 0805 7290 0000 0063  ..........r....c
+00001f70: 0000 0000 0000 0000 0000 0000 0d00 0000  ................
+00001f80: 0a00 0000 4300 0000 739c 0100 0074 0074  ....C...s....t.t
+00001f90: 0183 017d 0074 026a 0364 0164 0085 0219  ...}.t.j.d.d....
+00001fa0: 007d 017c 0164 0164 0085 0219 007d 0264  .}.|.d.d.....}.d
+00001fb0: 027d 0374 0464 0364 0484 007c 0044 0083  .}.t.d.d...|.D..
+00001fc0: 0183 017c 0317 007d 0474 0583 007d 0574  ...|...}.t...}.t
+00001fd0: 067c 0183 0164 056b 0273 2d7c 0164 0519  .|...d.k.s-|.d..
+00001fe0: 007c 0376 0072 4274 067c 0183 0164 016b  .|.v.rBt.|...d.k
+00001ff0: 0472 3c7c 05a0 077c 0164 0119 00a1 0101  .r<|...|.d......
+00002000: 0064 0053 007c 05a0 07a1 0001 0064 0053  .d.S.|.......d.S
+00002010: 007c 0164 0519 007d 0674 067c 0183 0164  .|.d...}.t.|...d
+00002020: 016b 0472 5c7c 0164 0119 0064 0676 0072  .k.r\|.d...d.v.r
+00002030: 5c74 087c 0683 017d 0774 097c 0783 0101  \t.|...}.t.|....
+00002040: 0064 0053 007c 067c 0076 0172 8b7a 0f74  .d.S.|.|.v.r.z.t
+00002050: 0183 007d 087c 086a 0a7c 0164 0164 0085  ...}.|.j.|.d.d..
+00002060: 0219 008e 0001 0057 0064 0053 0004 0074  .......W.d.S...t
+00002070: 0b79 8a01 007d 0901 007a 0f74 0c7c 0983  .y...}...z.t.|..
+00002080: 0101 007c 05a0 07a1 0001 0057 0059 0064  ...|.......W.Y.d
+00002090: 007d 097e 0964 0053 0064 007d 097e 0977  .}.~.d.S.d.}.~.w
+000020a0: 0177 0074 0464 0764 0484 007c 007c 0619  .w.t.d.d...|.|..
+000020b0: 0044 0083 0183 017d 0a74 0d7c 027c 0a83  .D.....}.t.|.|..
+000020c0: 025c 027d 0b7d 0c7c 0664 086b 0272 ab74  .\.}.}.|.d.k.r.t
+000020d0: 016a 0e7c 0b69 007c 0ca4 018e 0101 0064  .j.|.i.|.......d
+000020e0: 0053 0074 0183 007d 0874 0f7c 087c 0683  .S.t...}.t.|.|..
+000020f0: 0272 bf74 107c 087c 0683 027c 0b69 007c  .r.t.|.|...|.i.|
+00002100: 0ca4 018e 0101 0064 0053 0074 067c 0b83  .......d.S.t.|..
+00002110: 0164 096b 0272 cc7c 086a 0a7c 0b8e 0001  .d.k.r.|.j.|....
+00002120: 0064 0053 0064 0053 0029 0a4e 7201 0000  .d.S.d.S.).Nr...
+00002130: 0029 03da 0468 656c 70fa 062d 2d68 656c  .)...help..--hel
+00002140: 70fa 022d 6863 0100 0000 0000 0000 0000  p..-hc..........
+00002150: 0000 0200 0000 0500 0000 7300 0000 731c  ..........s...s.
+00002160: 0000 0081 007c 005d 097d 017c 01a0 0064  .....|.].}.|...d
+00002170: 0064 01a1 0256 0001 0071 0264 0253 0029  .d...V...q.d.S.)
+00002180: 0372 1a00 0000 fa01 2d4e 2901 da07 7265  .r......-N)...re
+00002190: 706c 6163 6529 0272 0c00 0000 7266 0000  place).r....rf..
+000021a0: 0072 0b00 0000 720b 0000 0072 0f00 0000  .r....r....r....
+000021b0: 7210 0000 0030 0100 0073 0400 0000 0280  r....0...s......
+000021c0: 1a00 7a17 6d61 696e 2e3c 6c6f 6361 6c73  ..z.main.<locals
+000021d0: 3e2e 3c67 656e 6578 7072 3e72 0500 0000  >.<genexpr>r....
+000021e0: 2902 7292 0000 0072 9300 0000 6301 0000  ).r....r....c...
+000021f0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00002200: 0073 0000 0073 3200 0000 8100 7c00 5d14  .s...s2.....|.].
+00002210: 7d01 7c01 6a00 7401 6a02 6a03 6b03 7216  }.|.j.t.j.j.k.r.
+00002220: 7c01 6a00 7401 6a02 6a04 6b03 7202 7c01  |.j.t.j.j.k.r.|.
+00002230: 6a05 5600 0100 7102 6400 5300 726e 0000  j.V...q.d.S.rn..
+00002240: 0029 06da 046b 696e 6472 1200 0000 da09  .)...kindr......
+00002250: 5061 7261 6d65 7465 72da 0b56 4152 5f4b  Parameter..VAR_K
+00002260: 4559 574f 5244 da0e 5641 525f 504f 5349  EYWORD..VAR_POSI
+00002270: 5449 4f4e 414c 723b 0000 0072 2b00 0000  TIONALr;...r+...
+00002280: 720b 0000 0072 0b00 0000 720f 0000 0072  r....r....r....r
+00002290: 1000 0000 4901 0000 7310 0000 0002 8004  ....I...s.......
+000022a0: 0002 020e 010e 0104 fd06 0304 fc72 5100  .............rQ.
+000022b0: 0000 722f 0000 0029 1172 2100 0000 7204  ..r/...).r!...r.
+000022c0: 0000 0072 4a00 0000 da04 6172 6776 7211  ...rJ.....argvr.
+000022d0: 0000 0072 5000 0000 7230 0000 0072 7000  ...rP...r0...rp.
+000022e0: 0000 7245 0000 0072 0200 0000 7253 0000  ..rE...r....rS..
+000022f0: 00da 0945 7863 6570 7469 6f6e da05 7072  ...Exception..pr
+00002300: 696e 7472 9000 0000 7251 0000 0072 8a00  intr....rQ...r..
+00002310: 0000 7214 0000 0029 0dda 076d 6574 686f  ..r....)...metho
+00002320: 6473 7267 0000 005a 0f72 6177 5f6d 6574  dsrg...Z.raw_met
+00002330: 686f 645f 6172 6773 5a09 6865 6c70 5f61  hod_argsZ.help_a
+00002340: 7267 73da 0761 6374 696f 6e73 7291 0000  rgs..actionsr...
+00002350: 00da 0661 6374 696f 6eda 026d 6472 7200  ...action..mdrr.
+00002360: 0000 da01 6572 6800 0000 5a08 706f 735f  ....erh...Z.pos_
+00002370: 6172 6773 728d 0000 0072 0b00 0000 720b  argsr....r....r.
+00002380: 0000 0072 0f00 0000 da04 6d61 696e 2b01  ...r......main+.
+00002390: 0000 7346 0000 0008 010e 010c 0104 0116  ..sF............
+000023a0: 0106 0118 020c 0112 010c 0208 0418 0108  ................
+000023b0: 010c 0108 0202 0106 0118 010e 0108 0116  ................
+000023c0: 0108 8002 fe08 0506 0208 fe0e 0708 0114  ................
+000023d0: 0106 020a 0118 010c 020e 0104 ff72 a200  .............r..
+000023e0: 0000 726e 0000 0029 1972 4100 0000 da05  ..rn...).rA.....
+000023f0: 7574 696c 7372 0200 0000 7203 0000 0072  utilsr....r....r
+00002400: 7200 0000 7204 0000 0072 1200 0000 7287  r...r....r....r.
+00002410: 0000 0072 0600 0000 7207 0000 0072 0800  ...r....r....r..
+00002420: 0000 da04 6970 6462 da02 6f73 724a 0000  ....ipdb..osrJ..
+00002430: 0072 2a00 0000 7218 0000 0072 2100 0000  .r*...r....r!...
+00002440: 7245 0000 0072 4f00 0000 7250 0000 0072  rE...rO...rP...r
+00002450: 6500 0000 7211 0000 0072 7800 0000 7290  e...r....rx...r.
+00002460: 0000 0072 a200 0000 720b 0000 0072 0b00  ...r....r....r..
+00002470: 0000 720b 0000 0072 0f00 0000 da08 3c6d  ..r....r......<m
+00002480: 6f64 756c 653e 0100 0000 731e 0000 0004  odule>....s.....
+00002490: 0010 0e0c 0108 0114 0108 0108 0108 010e  ................
+000024a0: 0308 0a14 080e 390e 0f26 7d0c 3c         ......9..&}.<
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/__pycache__/package.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Sep 27 14:37:11 2022 UTC, .py size: 3445 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-00000000: 6f0d 0d0a 0000 0000 970a 3363 750d 0000  o.........3cu...
+00000000: 6f0d 0d0a 0000 0000 e7c6 3164 770d 0000  o.........1dw...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 6d06 5a06 6d07 5a07  d.l.m.Z.m.Z.m.Z.
 00000060: 6d08 5a08 0100 6403 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6401 6c0b 5a0b 6400 6401 6c0c  ..d.d.l.Z.d.d.l.
 00000080: 5a0c 4700 6405 6406 8400 6406 8302 5a0d  Z.G.d.d...d...Z.
 00000090: 4700 6407 6408 8400 6408 650d 8303 5a0e  G.d.d...d.e...Z.
 000000a0: 6401 5300 2909 e900 0000 004e 2904 da05  d.S.)......N)...
 000000b0: 556e 696f 6eda 0843 616c 6c61 626c 65da  Union..Callable.
 000000c0: 084f 7074 696f 6e61 6cda 0454 7970 65e9  .Optional..Type.
-000000d0: 0100 0000 2901 da05 4275 6e63 6863 0000  ....)...Bunchc..
+000000d0: 0300 0000 2901 da05 4275 6e63 6863 0000  ....)...Bunchc..
 000000e0: 0000 0000 0000 0000 0000 0000 0000 1b00  ................
 000000f0: 0000 4000 0000 73e8 0000 0065 005a 0164  ..@...s....e.Z.d
 00000100: 005a 0209 0109 0109 0109 0109 0109 0109  .Z..............
 00000110: 0109 0109 0109 0109 0109 0109 0164 2764  .............d'd
 00000120: 0265 0364 0365 0464 0465 0464 0565 0464  .e.d.e.d.e.d.e.d
 00000130: 0665 0464 0765 0464 0865 0464 0965 0364  .e.d.e.d.e.d.e.d
 00000140: 0a65 0464 0b65 0464 0c65 0464 0d65 0464  .e.d.e.d.e.d.e.d
@@ -46,162 +46,163 @@
 000002d0: 720a 0000 0072 0b00 0000 720f 0000 0072  r....r....r....r
 000002e0: 0900 0000 7210 0000 0072 0d00 0000 7211  ....r....r....r.
 000002f0: 0000 0072 1200 0000 7213 0000 0029 0eda  ...r....r....)..
 00000300: 0473 656c 6672 0900 0000 720a 0000 0072  .selfr....r....r
 00000310: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
 00000320: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
 00000330: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
-00000340: 0072 1500 0000 a900 7218 0000 00fa 372f  .r......r.....7/
-00000350: 686f 6d65 2f61 6c2f 4769 7468 7562 2f79  home/al/Github/y
+00000340: 0072 1500 0000 a900 7218 0000 00fa 402f  .r......r.....@/
+00000350: 686f 6d65 2f61 6c2f 4769 7448 7562 2f79  home/al/GitHub/y
 00000360: 6572 6261 6d61 7465 2f70 6163 6b61 6765  erbamate/package
-00000370: 732f 7965 7262 616d 6174 652f 7061 636b  s/yerbamate/pack
-00000380: 6167 652e 7079 da08 5f5f 696e 6974 5f5f  age.py..__init__
-00000390: 1700 0000 7318 0000 0006 1006 0106 0106  ....s...........
-000003a0: 0106 0106 0106 0206 0106 0206 0106 010a  ................
-000003b0: 017a 1050 6163 6b61 6765 2e5f 5f69 6e69  .z.Package.__ini
-000003c0: 745f 5fda 0b64 6573 7469 6e61 7469 6f6e  t__..destination
-000003d0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000003e0: 0001 0000 0043 0000 00f3 0400 0000 6400  .....C........d.
-000003f0: 5300 7216 0000 0072 1800 0000 2902 720c  S.r....r....).r.
-00000400: 0000 0072 1b00 0000 7218 0000 0072 1800  ...r....r....r..
-00000410: 0000 7219 0000 00da 0769 6e73 7461 6c6c  ..r......install
-00000420: 3700 0000 7302 0000 0004 027a 0f50 6163  7...s......z.Pac
-00000430: 6b61 6765 2e69 6e73 7461 6c6c da10 7061  kage.install..pa
-00000440: 636b 6167 655f 6c6f 6361 7469 6f6e da0c  ckage_location..
-00000450: 7061 636b 6167 655f 6e61 6d65 da06 7265  package_name..re
-00000460: 7475 726e 6303 0000 0000 0000 0000 0000  turnc...........
-00000470: 0005 0000 0005 0000 0043 0000 0073 2e00  .........C...s..
-00000480: 0000 7400 7c01 7c01 a001 6401 a101 6402  ..t.|.|...d...d.
-00000490: 1900 6701 6403 8d02 7d03 7402 7c03 7c02  ..g.d...}.t.|.|.
-000004a0: 8302 7d04 7403 a004 a100 0100 7c04 5300  ..}.t.......|.S.
-000004b0: 2904 4eda 012e 7206 0000 0029 01da 0866  ).N...r....)...f
-000004c0: 726f 6d6c 6973 7429 05da 0a5f 5f69 6d70  romlist)...__imp
-000004d0: 6f72 745f 5fda 0573 706c 6974 da07 6765  ort__..split..ge
-000004e0: 7461 7474 72da 0469 7064 62da 0973 6574  tattr..ipdb..set
-000004f0: 5f74 7261 6365 2905 7217 0000 0072 1e00  _trace).r....r..
-00000500: 0000 721f 0000 0072 0d00 0000 5a0d 7061  ..r....r....Z.pa
-00000510: 636b 6167 655f 636c 6173 7372 1800 0000  ckage_classr....
-00000520: 7218 0000 0072 1900 0000 da12 5f67 6574  r....r......_get
-00000530: 5f70 6163 6b61 6765 5f63 6c61 7373 3b00  _package_class;.
-00000540: 0000 730e 0000 0002 0302 010e 0106 fe0a  ..s.............
-00000550: 0408 0104 017a 1a50 6163 6b61 6765 2e5f  .....z.Package._
-00000560: 6765 745f 7061 636b 6167 655f 636c 6173  get_package_clas
-00000570: 73da 0a65 6e74 7279 706f 696e 7463 0200  s..entrypointc..
-00000580: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000590: 0000 4300 0000 730c 0000 0074 00a0 017c  ..C...s....t...|
-000005a0: 01a1 016a 0253 0072 1600 0000 2903 da07  ...j.S.r....)...
-000005b0: 696e 7370 6563 74da 0e67 6574 6675 6c6c  inspect..getfull
-000005c0: 6172 6773 7065 63da 0461 7267 7329 0272  argspec..args).r
-000005d0: 1700 0000 7229 0000 0072 1800 0000 7218  ....r)...r....r.
-000005e0: 0000 0072 1900 0000 da13 5f67 656e 6572  ...r......_gener
-000005f0: 6174 655f 7369 676e 6174 7572 6546 0000  ate_signatureF..
-00000600: 0073 0200 0000 0c01 7a1b 5061 636b 6167  .s......z.Packag
-00000610: 652e 5f67 656e 6572 6174 655f 7369 676e  e._generate_sign
-00000620: 6174 7572 6572 2c00 0000 6302 0000 0000  aturer,...c.....
-00000630: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-00000640: 0000 0073 1a00 0000 7c00 a000 7c00 6a01  ...s....|...|.j.
-00000650: 7c00 6a02 a102 6401 6900 7c01 a401 8e01  |.j...d.i.|.....
-00000660: 5300 2902 4e72 1800 0000 a903 7228 0000  S.).Nr......r(..
-00000670: 0072 0a00 0000 720c 0000 0029 0272 1700  .r....r....).r..
-00000680: 0000 722c 0000 0072 1800 0000 7218 0000  ..r,...r....r...
-00000690: 0072 1900 0000 da10 5f70 6172 7365 5f73  .r......_parse_s
-000006a0: 6967 6e61 7475 7265 4900 0000 7302 0000  ignatureI...s...
-000006b0: 001a 017a 1850 6163 6b61 6765 2e5f 7061  ...z.Package._pa
-000006c0: 7273 655f 7369 676e 6174 7572 6563 0100  rse_signaturec..
-000006d0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-000006e0: 0000 4300 0000 7310 0000 007c 00a0 007c  ..C...s....|...|
-000006f0: 006a 017c 006a 02a1 0253 0072 1600 0000  .j.|.j...S.r....
-00000700: 722e 0000 00a9 0172 1700 0000 7218 0000  r......r....r...
-00000710: 0072 1800 0000 7219 0000 00da 075f 6f62  .r....r......_ob
-00000720: 6a65 6374 4c00 0000 7302 0000 0010 027a  jectL...s......z
-00000730: 0f50 6163 6b61 6765 2e5f 6f62 6a65 6374  .Package._object
-00000740: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000750: 0001 0000 0043 0000 0072 1c00 0000 7216  .....C...r....r.
-00000760: 0000 0072 1800 0000 7230 0000 0072 1800  ...r....r0...r..
-00000770: 0000 7218 0000 0072 1900 0000 da06 7570  ..r....r......up
-00000780: 6461 7465 5000 0000 f302 0000 0004 017a  dateP..........z
-00000790: 0e50 6163 6b61 6765 2e75 7064 6174 6563  .Package.updatec
-000007a0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000007b0: 0100 0000 4300 0000 721c 0000 0072 1600  ....C...r....r..
-000007c0: 0000 7218 0000 0072 3000 0000 7218 0000  ..r....r0...r...
-000007d0: 0072 1800 0000 7219 0000 00da 0975 6e69  .r....r......uni
-000007e0: 6e73 7461 6c6c 5300 0000 7233 0000 007a  nstallS...r3...z
-000007f0: 1150 6163 6b61 6765 2e75 6e69 6e73 7461  .Package.uninsta
-00000800: 6c6c 6301 0000 0000 0000 0000 0000 0001  llc.............
-00000810: 0000 0004 0000 0043 0000 0073 1400 0000  .......C...s....
-00000820: 6401 7c00 6a00 9b00 6402 7c00 6a01 9b00  d.|.j...d.|.j...
-00000830: 9d04 5300 2903 4e7a 0950 6163 6b61 6765  ..S.).Nz.Package
-00000840: 3a20 fa01 2029 0272 0e00 0000 720c 0000  : .. ).r....r...
-00000850: 0072 3000 0000 7218 0000 0072 1800 0000  .r0...r....r....
-00000860: 7219 0000 00da 075f 5f73 7472 5f5f 5600  r......__str__V.
-00000870: 0000 7302 0000 0014 017a 0f50 6163 6b61  ..s......z.Packa
-00000880: 6765 2e5f 5f73 7472 5f5f 290d 4e4e 4e4e  ge.__str__).NNNN
-00000890: 4e4e 4e4e 4e4e 4e4e 4e29 0272 2000 0000  NNNNNNNNN).r ...
-000008a0: 4e29 14da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-000008b0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-000008c0: 6c6e 616d 655f 5f72 0700 0000 da03 7374  lname__r......st
-000008d0: 7272 1a00 0000 da0c 7374 6174 6963 6d65  rr......staticme
-000008e0: 7468 6f64 721d 0000 00da 0464 6963 7472  thodr......dictr
-000008f0: 2800 0000 7202 0000 0072 0500 0000 7203  (...r....r....r.
-00000900: 0000 0072 2d00 0000 da06 6f62 6a65 6374  ...r-.....object
-00000910: 722f 0000 0072 3100 0000 7232 0000 0072  r/...r1...r2...r
-00000920: 3400 0000 7236 0000 0072 1800 0000 7218  4...r6...r....r.
-00000930: 0000 0072 1800 0000 7219 0000 0072 0800  ...r....r....r..
-00000940: 0000 1200 0000 7364 0000 0008 0002 0702  ......sd........
-00000950: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000960: 0102 0102 0102 0104 f202 0202 fe02 0302  ................
-00000970: fd02 0402 fc02 0502 fb02 0602 fa02 0702  ................
-00000980: f902 0802 f802 0902 f702 0a02 f602 0b02  ................
-00000990: f502 0c02 f402 0d02 f302 0e0a f202 2014  .............. .
-000009a0: 0116 031a 0b12 030e 030a 040a 030c 0372  ...............r
-000009b0: 0800 0000 6300 0000 0000 0000 0000 0000  ....c...........
-000009c0: 0000 0000 0015 0000 0000 0000 0073 5c00  .............s\.
-000009d0: 0000 6500 5a01 6400 5a02 0901 0901 0902  ..e.Z.d.Z.......
-000009e0: 0903 0901 0904 0901 0901 0901 0901 6411  ..............d.
-000009f0: 6405 6503 6406 6504 6407 6504 6408 6504  d.e.d.e.d.e.d.e.
-00000a00: 6409 6504 640a 6504 640b 6504 640c 6503  d.e.d.e.d.e.d.e.
-00000a10: 640d 6504 640e 6504 6614 8700 6601 640f  d.e.d.e.f...f.d.
-00000a20: 6410 840d 5a05 8700 0400 5a06 5300 2912  d...Z.....Z.S.).
-00000a30: da10 504c 5472 6169 6e65 7250 6163 6b61  ..PLTrainerPacka
-00000a40: 6765 4eda 0574 6f72 6368 da05 6c6f 6361  geN..torch..loca
-00000a50: 6cda 0870 6c5f 7472 6169 6e72 0900 0000  l..pl_trainr....
-00000a60: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00000a70: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
-00000a80: 0000 0072 1100 0000 7212 0000 0063 0b00  ...r....r....c..
-00000a90: 0000 0000 0000 0000 0000 0b00 0000 0c00  ................
-00000aa0: 0000 0300 0000 7324 0000 0074 0083 006a  ......s$...t...j
-00000ab0: 017c 027c 037c 047c 057c 067c 077c 017c  .|.|.|.|.|.|.|.|
-00000ac0: 087c 097c 0a64 018d 0a01 0064 0053 0029  .|.|.d.....d.S.)
-00000ad0: 024e 290a 720a 0000 0072 0b00 0000 720c  .N).r....r....r.
-00000ae0: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
-00000af0: 0000 7209 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00000b00: 0072 1200 0000 2902 da05 7375 7065 7272  .r....)...superr
-00000b10: 1a00 0000 290b 7217 0000 0072 0900 0000  ....).r....r....
-00000b20: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00000b30: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
-00000b40: 0000 0072 1100 0000 7212 0000 00a9 01da  ...r....r.......
-00000b50: 095f 5f63 6c61 7373 5f5f 7218 0000 0072  .__class__r....r
-00000b60: 1900 0000 721a 0000 005f 0000 0073 1800  ....r...._...s..
-00000b70: 0000 060d 0201 0201 0201 0201 0201 0201  ................
-00000b80: 0201 0201 0201 0201 0af6 7a19 504c 5472  ..........z.PLTr
-00000b90: 6169 6e65 7250 6163 6b61 6765 2e5f 5f69  ainerPackage.__i
-00000ba0: 6e69 745f 5f29 0a4e 4e72 3f00 0000 7240  nit__).NNr?...r@
-00000bb0: 0000 004e 7241 0000 004e 4e4e 4e29 0772  ...NrA...NNNN).r
-00000bc0: 3700 0000 7238 0000 0072 3900 0000 7207  7...r8...r9...r.
-00000bd0: 0000 0072 3a00 0000 721a 0000 00da 0d5f  ...r:...r......_
-00000be0: 5f63 6c61 7373 6365 6c6c 5f5f 7218 0000  _classcell__r...
-00000bf0: 0072 1800 0000 7243 0000 0072 1900 0000  .r....rC...r....
-00000c00: 723e 0000 005a 0000 0073 4000 0000 0800  r>...Z...s@.....
-00000c10: 0207 0201 0201 0201 0201 0201 0201 0201  ................
-00000c20: 0201 0201 04f5 0202 02fe 0203 02fd 0204  ................
-00000c30: 02fc 0205 02fb 0206 02fa 0207 02f9 0208  ................
-00000c40: 02f8 0209 02f7 020a 02f6 020b 16f5 723e  ..............r>
-00000c50: 0000 0029 0fda 026f 73da 0373 7973 da06  ...)...os..sys..
-00000c60: 7368 7574 696c da06 7572 6c6c 6962 da06  shutil..urllib..
-00000c70: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
-00000c80: 7204 0000 0072 0500 0000 da0b 7574 696c  r....r......util
-00000c90: 732e 6275 6e63 6872 0700 0000 722a 0000  s.bunchr....r*..
-00000ca0: 0072 2600 0000 7208 0000 0072 3e00 0000  .r&...r....r>...
-00000cb0: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00000cc0: 1900 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000cd0: 0000 7314 0000 0008 0608 0108 0108 0118  ..s.............
-00000ce0: 010c 0108 0208 010e 0314 48              ..........H
+00000370: 732f 7965 7262 616d 6174 652f 6170 692f  s/yerbamate/api/
+00000380: 6461 7461 2f70 6163 6b61 6765 2e70 79da  data/package.py.
+00000390: 085f 5f69 6e69 745f 5f17 0000 0073 1800  .__init__....s..
+000003a0: 0000 0610 0601 0601 0601 0601 0601 0602  ................
+000003b0: 0601 0602 0601 0601 0a01 7a10 5061 636b  ..........z.Pack
+000003c0: 6167 652e 5f5f 696e 6974 5f5f da0b 6465  age.__init__..de
+000003d0: 7374 696e 6174 696f 6e63 0200 0000 0000  stinationc......
+000003e0: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
+000003f0: 0000 f304 0000 0064 0053 0072 1600 0000  .......d.S.r....
+00000400: 7218 0000 0029 0272 0c00 0000 721b 0000  r....).r....r...
+00000410: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000420: da07 696e 7374 616c 6c37 0000 0073 0200  ..install7...s..
+00000430: 0000 0402 7a0f 5061 636b 6167 652e 696e  ....z.Package.in
+00000440: 7374 616c 6cda 1070 6163 6b61 6765 5f6c  stall..package_l
+00000450: 6f63 6174 696f 6eda 0c70 6163 6b61 6765  ocation..package
+00000460: 5f6e 616d 65da 0672 6574 7572 6e63 0300  _name..returnc..
+00000470: 0000 0000 0000 0000 0000 0500 0000 0500  ................
+00000480: 0000 4300 0000 732e 0000 0074 007c 017c  ..C...s....t.|.|
+00000490: 01a0 0164 01a1 0164 0219 0067 0164 038d  ...d...d...g.d..
+000004a0: 027d 0374 027c 037c 0283 027d 0474 03a0  .}.t.|.|...}.t..
+000004b0: 04a1 0001 007c 0453 0029 044e da01 2ee9  .....|.S.).N....
+000004c0: 0100 0000 2901 da08 6672 6f6d 6c69 7374  ....)...fromlist
+000004d0: 2905 da0a 5f5f 696d 706f 7274 5f5f da05  )...__import__..
+000004e0: 7370 6c69 74da 0767 6574 6174 7472 da04  split..getattr..
+000004f0: 6970 6462 da09 7365 745f 7472 6163 6529  ipdb..set_trace)
+00000500: 0572 1700 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00000510: 720d 0000 005a 0d70 6163 6b61 6765 5f63  r....Z.package_c
+00000520: 6c61 7373 7218 0000 0072 1800 0000 7219  lassr....r....r.
+00000530: 0000 00da 125f 6765 745f 7061 636b 6167  ....._get_packag
+00000540: 655f 636c 6173 733b 0000 0073 0e00 0000  e_class;...s....
+00000550: 0203 0201 0e01 06fe 0a04 0801 0401 7a1a  ..............z.
+00000560: 5061 636b 6167 652e 5f67 6574 5f70 6163  Package._get_pac
+00000570: 6b61 6765 5f63 6c61 7373 da0a 656e 7472  kage_class..entr
+00000580: 7970 6f69 6e74 6302 0000 0000 0000 0000  ypointc.........
+00000590: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+000005a0: 0c00 0000 7400 a001 7c01 a101 6a02 5300  ....t...|...j.S.
+000005b0: 7216 0000 0029 03da 0769 6e73 7065 6374  r....)...inspect
+000005c0: da0e 6765 7466 756c 6c61 7267 7370 6563  ..getfullargspec
+000005d0: da04 6172 6773 2902 7217 0000 0072 2a00  ..args).r....r*.
+000005e0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+000005f0: 00da 135f 6765 6e65 7261 7465 5f73 6967  ..._generate_sig
+00000600: 6e61 7475 7265 4600 0000 7302 0000 000c  natureF...s.....
+00000610: 017a 1b50 6163 6b61 6765 2e5f 6765 6e65  .z.Package._gene
+00000620: 7261 7465 5f73 6967 6e61 7475 7265 722d  rate_signaturer-
+00000630: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00000640: 0200 0000 0400 0000 4300 0000 731a 0000  ........C...s...
+00000650: 007c 00a0 007c 006a 017c 006a 02a1 0264  .|...|.j.|.j...d
+00000660: 0169 007c 01a4 018e 0153 0029 024e 7218  .i.|.....S.).Nr.
+00000670: 0000 00a9 0372 2900 0000 720a 0000 0072  .....r)...r....r
+00000680: 0c00 0000 2902 7217 0000 0072 2d00 0000  ....).r....r-...
+00000690: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
+000006a0: 105f 7061 7273 655f 7369 676e 6174 7572  ._parse_signatur
+000006b0: 6549 0000 0073 0200 0000 1a01 7a18 5061  eI...s......z.Pa
+000006c0: 636b 6167 652e 5f70 6172 7365 5f73 6967  ckage._parse_sig
+000006d0: 6e61 7475 7265 6301 0000 0000 0000 0000  naturec.........
+000006e0: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
+000006f0: 1000 0000 7c00 a000 7c00 6a01 7c00 6a02  ....|...|.j.|.j.
+00000700: a102 5300 7216 0000 0072 2f00 0000 a901  ..S.r....r/.....
+00000710: 7217 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
+00000720: 1900 0000 da07 5f6f 626a 6563 744c 0000  ......_objectL..
+00000730: 0073 0200 0000 1002 7a0f 5061 636b 6167  .s......z.Packag
+00000740: 652e 5f6f 626a 6563 7463 0100 0000 0000  e._objectc......
+00000750: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00000760: 0000 721c 0000 0072 1600 0000 7218 0000  ..r....r....r...
+00000770: 0072 3100 0000 7218 0000 0072 1800 0000  .r1...r....r....
+00000780: 7219 0000 00da 0675 7064 6174 6550 0000  r......updateP..
+00000790: 00f3 0200 0000 0401 7a0e 5061 636b 6167  ........z.Packag
+000007a0: 652e 7570 6461 7465 6301 0000 0000 0000  e.updatec.......
+000007b0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+000007c0: 0072 1c00 0000 7216 0000 0072 1800 0000  .r....r....r....
+000007d0: 7231 0000 0072 1800 0000 7218 0000 0072  r1...r....r....r
+000007e0: 1900 0000 da09 756e 696e 7374 616c 6c53  ......uninstallS
+000007f0: 0000 0072 3400 0000 7a11 5061 636b 6167  ...r4...z.Packag
+00000800: 652e 756e 696e 7374 616c 6c63 0100 0000  e.uninstallc....
+00000810: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00000820: 4300 0000 7314 0000 0064 017c 006a 009b  C...s....d.|.j..
+00000830: 0064 027c 006a 019b 009d 0453 0029 034e  .d.|.j.....S.).N
+00000840: 7a09 5061 636b 6167 653a 20fa 0120 2902  z.Package: .. ).
+00000850: 720e 0000 0072 0c00 0000 7231 0000 0072  r....r....r1...r
+00000860: 1800 0000 7218 0000 0072 1900 0000 da07  ....r....r......
+00000870: 5f5f 7374 725f 5f56 0000 0073 0200 0000  __str__V...s....
+00000880: 1401 7a0f 5061 636b 6167 652e 5f5f 7374  ..z.Package.__st
+00000890: 725f 5f29 0d4e 4e4e 4e4e 4e4e 4e4e 4e4e  r__).NNNNNNNNNNN
+000008a0: 4e4e 2902 7220 0000 004e 2914 da08 5f5f  NN).r ...N)...__
+000008b0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+000008c0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+000008d0: 7207 0000 00da 0373 7472 721a 0000 00da  r......strr.....
+000008e0: 0c73 7461 7469 636d 6574 686f 6472 1d00  .staticmethodr..
+000008f0: 0000 da04 6469 6374 7229 0000 0072 0200  ....dictr)...r..
+00000900: 0000 7205 0000 0072 0300 0000 722e 0000  ..r....r....r...
+00000910: 00da 066f 626a 6563 7472 3000 0000 7232  ...objectr0...r2
+00000920: 0000 0072 3300 0000 7235 0000 0072 3700  ...r3...r5...r7.
+00000930: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
+00000940: 0072 1900 0000 7208 0000 0012 0000 0073  .r....r........s
+00000950: 6400 0000 0800 0207 0201 0201 0201 0201  d...............
+00000960: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00000970: 04f2 0202 02fe 0203 02fd 0204 02fc 0205  ................
+00000980: 02fb 0206 02fa 0207 02f9 0208 02f8 0209  ................
+00000990: 02f7 020a 02f6 020b 02f5 020c 02f4 020d  ................
+000009a0: 02f3 020e 0af2 0220 1401 1603 1a0b 1203  ....... ........
+000009b0: 0e03 0a04 0a03 0c03 7208 0000 0063 0000  ........r....c..
+000009c0: 0000 0000 0000 0000 0000 0000 0000 1500  ................
+000009d0: 0000 0000 0000 735c 0000 0065 005a 0164  ......s\...e.Z.d
+000009e0: 005a 0209 0109 0109 0209 0309 0109 0409  .Z..............
+000009f0: 0109 0109 0109 0164 1164 0565 0364 0665  .......d.d.e.d.e
+00000a00: 0464 0765 0464 0865 0464 0965 0464 0a65  .d.e.d.e.d.e.d.e
+00000a10: 0464 0b65 0464 0c65 0364 0d65 0464 0e65  .d.e.d.e.d.e.d.e
+00000a20: 0466 1487 0066 0164 0f64 1084 0d5a 0587  .f...f.d.d...Z..
+00000a30: 0004 005a 0653 0029 12da 1050 4c54 7261  ...Z.S.)...PLTra
+00000a40: 696e 6572 5061 636b 6167 654e da05 746f  inerPackageN..to
+00000a50: 7263 68da 056c 6f63 616c da08 706c 5f74  rch..local..pl_t
+00000a60: 7261 696e 7209 0000 0072 0a00 0000 720b  rainr....r....r.
+00000a70: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000a80: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00000a90: 0072 1200 0000 630b 0000 0000 0000 0000  .r....c.........
+00000aa0: 0000 000b 0000 000c 0000 0003 0000 0073  ...............s
+00000ab0: 2400 0000 7400 8300 6a01 7c02 7c03 7c04  $...t...j.|.|.|.
+00000ac0: 7c05 7c06 7c07 7c01 7c08 7c09 7c0a 6401  |.|.|.|.|.|.|.d.
+00000ad0: 8d0a 0100 6400 5300 2902 4e29 0a72 0a00  ....d.S.).N).r..
+00000ae0: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000af0: 0072 0e00 0000 720f 0000 0072 0900 0000  .r....r....r....
+00000b00: 7210 0000 0072 1100 0000 7212 0000 0029  r....r....r....)
+00000b10: 02da 0573 7570 6572 721a 0000 0029 0b72  ...superr....).r
+00000b20: 1700 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
+00000b30: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000b40: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00000b50: 0072 1200 0000 a901 da09 5f5f 636c 6173  .r........__clas
+00000b60: 735f 5f72 1800 0000 7219 0000 0072 1a00  s__r....r....r..
+00000b70: 0000 5f00 0000 7318 0000 0006 0d02 0102  .._...s.........
+00000b80: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000b90: 010a f67a 1950 4c54 7261 696e 6572 5061  ...z.PLTrainerPa
+00000ba0: 636b 6167 652e 5f5f 696e 6974 5f5f 290a  ckage.__init__).
+00000bb0: 4e4e 7240 0000 0072 4100 0000 4e72 4200  NNr@...rA...NrB.
+00000bc0: 0000 4e4e 4e4e 2907 7238 0000 0072 3900  ..NNNN).r8...r9.
+00000bd0: 0000 723a 0000 0072 0700 0000 723b 0000  ..r:...r....r;..
+00000be0: 0072 1a00 0000 da0d 5f5f 636c 6173 7363  .r......__classc
+00000bf0: 656c 6c5f 5f72 1800 0000 7218 0000 0072  ell__r....r....r
+00000c00: 4400 0000 7219 0000 0072 3f00 0000 5a00  D...r....r?...Z.
+00000c10: 0000 7340 0000 0008 0002 0702 0102 0102  ..s@............
+00000c20: 0102 0102 0102 0102 0102 0102 0104 f502  ................
+00000c30: 0202 fe02 0302 fd02 0402 fc02 0502 fb02  ................
+00000c40: 0602 fa02 0702 f902 0802 f802 0902 f702  ................
+00000c50: 0a02 f602 0b16 f572 3f00 0000 290f da02  .......r?...)...
+00000c60: 6f73 da03 7379 73da 0673 6875 7469 6cda  os..sys..shutil.
+00000c70: 0675 726c 6c69 62da 0674 7970 696e 6772  .urllib..typingr
+00000c80: 0200 0000 7203 0000 0072 0400 0000 7205  ....r....r....r.
+00000c90: 0000 005a 0b75 7469 6c73 2e62 756e 6368  ...Z.utils.bunch
+00000ca0: 7207 0000 0072 2b00 0000 7227 0000 0072  r....r+...r'...r
+00000cb0: 0800 0000 723f 0000 0072 1800 0000 7218  ....r?...r....r.
+00000cc0: 0000 0072 1800 0000 7219 0000 00da 083c  ...r....r......<
+00000cd0: 6d6f 6475 6c65 3e01 0000 0073 1400 0000  module>....s....
+00000ce0: 0806 0801 0801 0801 1801 0c01 0802 0801  ................
+00000cf0: 0e03 1448                                ...H
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Feb 10 22:28:52 2023 UTC, .py size: 923 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,90 @@
-00000000: 6f0d 0d0a 0000 0000 24c5 e663 9b03 0000  o.......$..c....
+00000000: 6f0d 0d0a 0000 0000 e7c6 3164 6503 0000  o.........1de...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
+00000020: 0003 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
-00000050: 6d05 5a05 0100 6404 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6401 6c08 5a08 0900 4700 6406  ..d.d.l.Z...G.d.
-00000070: 6407 8400 6407 8302 5a09 6401 5300 2908  d...d...Z.d.S.).
-00000080: e900 0000 004e 2901 da05 736c 6565 7029  .....N)...sleep)
-00000090: 01da 0a4d 6174 6543 6f6e 6669 67e9 0100  ...MateConfig...
-000000a0: 0000 2901 da10 4d6f 6475 6c65 5265 706f  ..)...ModuleRepo
-000000b0: 7369 746f 7279 6300 0000 0000 0000 0000  sitoryc.........
-000000c0: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
-000000d0: 5e00 0000 6500 5a01 6400 5a02 6401 6503  ^...e.Z.d.Z.d.e.
-000000e0: 6602 6402 6403 8404 5a04 6505 6404 6506  f.d.d...Z.e.d.e.
-000000f0: 6602 6405 6406 8404 8301 5a07 6407 6506  f.d.d.....Z.d.e.
-00000100: 6602 6408 6409 8404 5a08 640a 6506 6602  f.d.d...Z.d.e.f.
-00000110: 640b 640c 8404 5a09 640d 640e 8400 5a0a  d.d...Z.d.d...Z.
-00000120: 640f 6506 6602 6410 6411 8404 5a0b 6412  d.e.f.d.d...Z.d.
-00000130: 5300 2913 da07 4d61 7465 4150 49da 0663  S.)...MateAPI..c
-00000140: 6f6e 6669 6763 0200 0000 0000 0000 0000  onfigc..........
-00000150: 0000 0200 0000 0200 0000 4300 0000 7314  ..........C...s.
-00000160: 0000 007c 017c 005f 0074 017c 0183 017c  ...|.|._.t.|...|
-00000170: 005f 0264 0053 00a9 014e 2903 7207 0000  ._.d.S...N).r...
-00000180: 0072 0500 0000 da0a 7265 706f 7369 746f  .r......reposito
-00000190: 7279 2902 da04 7365 6c66 7207 0000 00a9  ry)...selfr.....
-000001a0: 0072 0b00 0000 fa3c 2f68 6f6d 652f 616c  .r.....</home/al
-000001b0: 2f47 6974 6875 622f 7965 7262 616d 6174  /Github/yerbamat
-000001c0: 652f 7061 636b 6167 6573 2f79 6572 6261  e/packages/yerba
-000001d0: 6d61 7465 2f61 7069 2f6d 6174 655f 6170  mate/api/mate_ap
-000001e0: 692e 7079 da08 5f5f 696e 6974 5f5f 1500  i.py..__init__..
-000001f0: 0000 7304 0000 0006 010e 017a 104d 6174  ..s........z.Mat
-00000200: 6541 5049 2e5f 5f69 6e69 745f 5fda 0c70  eAPI.__init__..p
-00000210: 726f 6a65 6374 5f6e 616d 6563 0100 0000  roject_namec....
-00000220: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00000230: 4300 0000 730e 0000 0074 00a0 017c 00a1  C...s....t...|..
-00000240: 0101 0064 0053 0072 0800 0000 2902 7205  ...d.S.r....).r.
-00000250: 0000 00da 0c69 6e69 745f 7072 6f6a 6563  .....init_projec
-00000260: 7429 0172 0e00 0000 720b 0000 0072 0b00  t).r....r....r..
-00000270: 0000 720c 0000 0072 0f00 0000 1a00 0000  ..r....r........
-00000280: 7302 0000 000e 027a 144d 6174 6541 5049  s......z.MateAPI
-00000290: 2e69 6e69 745f 7072 6f6a 6563 74da 0375  .init_project..u
-000002a0: 726c 6302 0000 0000 0000 0000 0000 0004  rlc.............
-000002b0: 0000 0004 0000 004f 0000 0073 1e00 0000  .......O...s....
-000002c0: 7c00 6a00 6a01 7c01 6701 7c02 a201 5200  |.j.j.|.g.|...R.
-000002d0: 6900 7c03 a401 8e01 0100 6400 5300 7208  i.|.......d.S.r.
-000002e0: 0000 0029 0272 0900 0000 da0b 696e 7374  ...).r......inst
-000002f0: 616c 6c5f 7572 6c29 0472 0a00 0000 7210  all_url).r....r.
-00000300: 0000 00da 0461 7267 73da 066b 7761 7267  .....args..kwarg
-00000310: 7372 0b00 0000 720b 0000 0072 0c00 0000  sr....r....r....
-00000320: 7211 0000 0021 0000 0073 0200 0000 1e01  r....!...s......
-00000330: 7a13 4d61 7465 4150 492e 696e 7374 616c  z.MateAPI.instal
-00000340: 6c5f 7572 6cda 066d 6f64 756c 6563 0200  l_url..modulec..
-00000350: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000360: 0000 4300 0000 730c 0000 007c 006a 00a0  ..C...s....|.j..
-00000370: 017c 01a1 0153 0072 0800 0000 2902 7209  .|...S.r....).r.
-00000380: 0000 00da 046c 6973 7429 0272 0a00 0000  .....list).r....
-00000390: 7214 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-000003a0: 0c00 0000 7215 0000 0024 0000 0073 0200  ....r....$...s..
-000003b0: 0000 0c01 7a0c 4d61 7465 4150 492e 6c69  ....z.MateAPI.li
-000003c0: 7374 6301 0000 0000 0000 0000 0000 0001  stc.............
-000003d0: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-000003e0: 7c00 6a00 a001 a100 5300 7208 0000 0029  |.j.....S.r....)
-000003f0: 0272 0900 0000 5a10 6765 745f 6d61 7465  .r....Z.get_mate
-00000400: 5f73 756d 6d61 7279 2901 720a 0000 0072  _summary).r....r
-00000410: 0b00 0000 720b 0000 0072 0c00 0000 da07  ....r....r......
-00000420: 7375 6d6d 6172 7928 0000 0073 0200 0000  summary(...s....
-00000430: 0a01 7a0f 4d61 7465 4150 492e 7375 6d6d  ..z.MateAPI.summ
-00000440: 6172 79da 0763 6f6d 6d61 6e64 6302 0000  ary..commandc...
-00000450: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00000460: 0043 0000 0073 1000 0000 7c00 6a00 a001  .C...s....|.j...
-00000470: 7c01 a101 0100 6400 5300 7208 0000 0029  |.....d.S.r....)
-00000480: 0272 0900 0000 da04 6175 746f 2902 720a  .r......auto).r.
-00000490: 0000 0072 1700 0000 720b 0000 0072 0b00  ...r....r....r..
-000004a0: 0000 720c 0000 0072 1800 0000 2b00 0000  ..r....r....+...
-000004b0: 7302 0000 0010 017a 0c4d 6174 6541 5049  s......z.MateAPI
-000004c0: 2e61 7574 6f4e 290c da08 5f5f 6e61 6d65  .autoN)...__name
-000004d0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-000004e0: 5f5f 7175 616c 6e61 6d65 5f5f 7203 0000  __qualname__r...
-000004f0: 0072 0d00 0000 da0c 7374 6174 6963 6d65  .r......staticme
-00000500: 7468 6f64 da03 7374 7272 0f00 0000 7211  thod..strr....r.
-00000510: 0000 0072 1500 0000 7216 0000 0072 1800  ...r....r....r..
-00000520: 0000 720b 0000 0072 0b00 0000 720b 0000  ..r....r....r...
-00000530: 0072 0c00 0000 7206 0000 0014 0000 0073  .r....r........s
-00000540: 1000 0000 0800 0e01 0205 1001 0e06 0e03  ................
-00000550: 0804 1203 7206 0000 0029 0ada 026f 73da  ....r....)...os.
-00000560: 0373 7973 da04 7469 6d65 7202 0000 005a  .sys..timer....Z
-00000570: 1579 6572 6261 6d61 7465 2e6d 6174 655f  .yerbamate.mate_
-00000580: 636f 6e66 6967 7203 0000 005a 1664 6174  configr....Z.dat
-00000590: 612e 6d6f 6475 6c65 5f72 6570 6f73 6974  a.module_reposit
-000005a0: 6f72 7972 0500 0000 da04 6970 6462 7206  oryr......ipdbr.
-000005b0: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
-000005c0: 0000 720c 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000005d0: 3e01 0000 0073 1000 0000 0800 0802 0c02  >....s..........
-000005e0: 0c01 0c03 0802 0203 1206                 ..........
+00000040: 6402 6c02 6d03 5a03 0100 6403 6404 6c04  d.l.m.Z...d.d.l.
+00000050: 6d05 5a05 0100 6400 6401 6c06 5a06 0900  m.Z...d.d.l.Z...
+00000060: 4700 6405 6406 8400 6406 8302 5a07 6401  G.d.d...d...Z.d.
+00000070: 5300 2907 e900 0000 004e 2901 da05 736c  S.)......N)...sl
+00000080: 6565 70e9 0100 0000 2901 da10 4d6f 6475  eep.....)...Modu
+00000090: 6c65 5265 706f 7369 746f 7279 6300 0000  leRepositoryc...
+000000a0: 0000 0000 0000 0000 0000 0000 0004 0000  ................
+000000b0: 0040 0000 0073 5800 0000 6500 5a01 6400  .@...sX...e.Z.d.
+000000c0: 5a02 6401 6402 8400 5a03 6504 6403 6505  Z.d.d...Z.e.d.e.
+000000d0: 6602 6404 6405 8404 8301 5a06 6406 6505  f.d.d.....Z.d.e.
+000000e0: 6602 6407 6408 8404 5a07 6409 6505 6602  f.d.d...Z.d.e.f.
+000000f0: 640a 640b 8404 5a08 640c 640d 8400 5a09  d.d...Z.d.d...Z.
+00000100: 640e 6505 6602 640f 6410 8404 5a0a 6411  d.e.f.d.d...Z.d.
+00000110: 5300 2912 da07 4d61 7465 4150 4963 0200  S.)...MateAPIc..
+00000120: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00000130: 0000 4300 0000 730e 0000 0074 007c 0183  ..C...s....t.|..
+00000140: 017c 005f 0164 0053 00a9 014e 2902 7204  .|._.d.S...N).r.
+00000150: 0000 00da 0a72 6570 6f73 6974 6f72 7929  .....repository)
+00000160: 02da 0473 656c 66da 0663 6f6e 6669 67a9  ...self..config.
+00000170: 0072 0a00 0000 fa3c 2f68 6f6d 652f 616c  .r.....</home/al
+00000180: 2f47 6974 4875 622f 7965 7262 616d 6174  /GitHub/yerbamat
+00000190: 652f 7061 636b 6167 6573 2f79 6572 6261  e/packages/yerba
+000001a0: 6d61 7465 2f61 7069 2f6d 6174 655f 6170  mate/api/mate_ap
+000001b0: 692e 7079 da08 5f5f 696e 6974 5f5f 1500  i.py..__init__..
+000001c0: 0000 f302 0000 000e 027a 104d 6174 6541  .........z.MateA
+000001d0: 5049 2e5f 5f69 6e69 745f 5fda 0c70 726f  PI.__init__..pro
+000001e0: 6a65 6374 5f6e 616d 6563 0100 0000 0000  ject_namec......
+000001f0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00000200: 0000 730e 0000 0074 00a0 017c 00a1 0101  ..s....t...|....
+00000210: 0064 0053 0072 0600 0000 2902 7204 0000  .d.S.r....).r...
+00000220: 00da 0c69 6e69 745f 7072 6f6a 6563 7429  ...init_project)
+00000230: 0172 0e00 0000 720a 0000 0072 0a00 0000  .r....r....r....
+00000240: 720b 0000 0072 0f00 0000 1a00 0000 720d  r....r........r.
+00000250: 0000 007a 144d 6174 6541 5049 2e69 6e69  ...z.MateAPI.ini
+00000260: 745f 7072 6f6a 6563 74da 0375 726c 6302  t_project..urlc.
+00000270: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+00000280: 0000 004f 0000 0073 1e00 0000 7c00 6a00  ...O...s....|.j.
+00000290: 6a01 7c01 6701 7c02 a201 5200 6900 7c03  j.|.g.|...R.i.|.
+000002a0: a401 8e01 0100 6400 5300 7206 0000 0029  ......d.S.r....)
+000002b0: 0272 0700 0000 da0b 696e 7374 616c 6c5f  .r......install_
+000002c0: 7572 6c29 0472 0800 0000 7210 0000 00da  url).r....r.....
+000002d0: 0461 7267 73da 066b 7761 7267 7372 0a00  .args..kwargsr..
+000002e0: 0000 720a 0000 0072 0b00 0000 7211 0000  ..r....r....r...
+000002f0: 0021 0000 0073 0200 0000 1e01 7a13 4d61  .!...s......z.Ma
+00000300: 7465 4150 492e 696e 7374 616c 6c5f 7572  teAPI.install_ur
+00000310: 6cda 066d 6f64 756c 6563 0200 0000 0000  l..modulec......
+00000320: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00000330: 0000 730c 0000 007c 006a 00a0 017c 01a1  ..s....|.j...|..
+00000340: 0153 0072 0600 0000 2902 7207 0000 00da  .S.r....).r.....
+00000350: 046c 6973 7429 0272 0800 0000 7214 0000  .list).r....r...
+00000360: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000370: 7215 0000 0024 0000 0073 0200 0000 0c01  r....$...s......
+00000380: 7a0c 4d61 7465 4150 492e 6c69 7374 6301  z.MateAPI.listc.
+00000390: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+000003a0: 0000 0043 0000 0073 0a00 0000 7c00 6a00  ...C...s....|.j.
+000003b0: a001 a100 5300 7206 0000 0029 0272 0700  ....S.r....).r..
+000003c0: 0000 5a10 6765 745f 6d61 7465 5f73 756d  ..Z.get_mate_sum
+000003d0: 6d61 7279 2901 7208 0000 0072 0a00 0000  mary).r....r....
+000003e0: 720a 0000 0072 0b00 0000 da07 7375 6d6d  r....r......summ
+000003f0: 6172 7928 0000 0073 0200 0000 0a01 7a0f  ary(...s......z.
+00000400: 4d61 7465 4150 492e 7375 6d6d 6172 79da  MateAPI.summary.
+00000410: 0763 6f6d 6d61 6e64 6302 0000 0000 0000  .commandc.......
+00000420: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00000430: 0073 1000 0000 7c00 6a00 a001 7c01 a101  .s....|.j...|...
+00000440: 0100 6400 5300 7206 0000 0029 0272 0700  ..d.S.r....).r..
+00000450: 0000 da04 6175 746f 2902 7208 0000 0072  ....auto).r....r
+00000460: 1700 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+00000470: 0000 0072 1800 0000 2b00 0000 7302 0000  ...r....+...s...
+00000480: 0010 017a 0c4d 6174 6541 5049 2e61 7574  ...z.MateAPI.aut
+00000490: 6f4e 290b da08 5f5f 6e61 6d65 5f5f da0a  oN)...__name__..
+000004a0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000004b0: 616c 6e61 6d65 5f5f 720c 0000 00da 0c73  alname__r......s
+000004c0: 7461 7469 636d 6574 686f 64da 0373 7472  taticmethod..str
+000004d0: 720f 0000 0072 1100 0000 7215 0000 0072  r....r....r....r
+000004e0: 1600 0000 7218 0000 0072 0a00 0000 720a  ....r....r....r.
+000004f0: 0000 0072 0a00 0000 720b 0000 0072 0500  ...r....r....r..
+00000500: 0000 1400 0000 7310 0000 0008 0008 0102  ......s.........
+00000510: 0510 010e 060e 0308 0412 0372 0500 0000  ...........r....
+00000520: 2908 da02 6f73 da03 7379 73da 0474 696d  )...os..sys..tim
+00000530: 6572 0200 0000 5a16 6461 7461 2e6d 6f64  er....Z.data.mod
+00000540: 756c 655f 7265 706f 7369 746f 7279 7204  ule_repositoryr.
+00000550: 0000 00da 0469 7064 6272 0500 0000 720a  .....ipdbr....r.
+00000560: 0000 0072 0a00 0000 720a 0000 0072 0b00  ...r....r....r..
+00000570: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000580: 730e 0000 0008 0008 020c 020c 0408 0202  s...............
+00000590: 0312 06                                  ...
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Feb 12 17:39:59 2023 UTC, .py size: 9516 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,358 +1,354 @@
-00000000: 6f0d 0d0a 0000 0000 6f24 e963 2c25 0000  o.......o$.c,%..
+00000000: 6f0d 0d0a 0000 0000 e7c6 3164 f424 0000  o.........1d.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
+00000020: 0003 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 6d06 5a06 0100 6400  d.l.m.Z.m.Z...d.
-00000060: 6401 6c07 5a07 6400 6403 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
-00000070: 0100 6404 6405 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
-00000080: 6401 6c0c 5a0c 4700 6406 6407 8400 6407  d.l.Z.G.d.d...d.
-00000090: 8302 5a0d 6401 5300 2908 e900 0000 004e  ..Z.d.S.)......N
-000000a0: 2902 da08 636f 7079 7472 6565 da06 726d  )...copytree..rm
-000000b0: 7472 6565 2901 da0a 4d61 7465 436f 6e66  tree)...MateConf
-000000c0: 6967 e901 0000 0029 01da 0864 6f77 6e6c  ig.....)...downl
-000000d0: 6f61 6463 0000 0000 0000 0000 0000 0000  oadc............
-000000e0: 0000 0000 0300 0000 4000 0000 7376 0000  ........@...sv..
-000000f0: 0065 005a 0164 005a 0255 0064 015a 0365  .e.Z.d.Z.U.d.Z.e
-00000100: 0465 0564 023c 0064 0365 0666 0264 0464  .e.d.<.d.e.f.d.d
-00000110: 0584 045a 0764 0664 0784 005a 0864 0864  ...Z.d.d...Z.d.d
-00000120: 0984 005a 0964 0a64 0b84 005a 0a64 0c64  ...Z.d.d...Z.d.d
-00000130: 0d84 005a 0b64 0e64 0f84 005a 0c64 1064  ...Z.d.d...Z.d.d
-00000140: 1184 005a 0d64 1265 0466 0264 1364 1484  ...Z.d.e.f.d.d..
-00000150: 045a 0e64 1564 1684 005a 0f64 1764 1884  .Z.d.d...Z.d.d..
-00000160: 005a 1064 1953 0029 1ada 0d4d 6f64 756c  .Z.d.S.)...Modul
-00000170: 654d 616e 6167 6572 da00 da09 726f 6f74  eManager....root
-00000180: 5f70 6174 68da 0463 6f6e 6663 0200 0000  _path..confc....
-00000190: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-000001a0: 4300 0000 7312 0000 007c 017c 005f 007c  C...s....|.|._.|
-000001b0: 00a0 01a1 0001 0064 0053 00a9 014e 2902  .......d.S...N).
-000001c0: 720a 0000 00da 1269 6e69 745f 7061 636b  r......init_pack
-000001d0: 6167 655f 6361 6368 6529 02da 0473 656c  age_cache)...sel
-000001e0: 6672 0a00 0000 a900 720e 0000 00fa 472f  fr......r.....G/
-000001f0: 686f 6d65 2f61 6c2f 4769 7468 7562 2f79  home/al/Github/y
-00000200: 6572 6261 6d61 7465 2f70 6163 6b61 6765  erbamate/package
-00000210: 732f 7965 7262 616d 6174 652f 6170 692f  s/yerbamate/api/
-00000220: 6461 7461 2f6d 6f64 756c 655f 6d61 6e61  data/module_mana
-00000230: 6765 722e 7079 da08 5f5f 696e 6974 5f5f  ger.py..__init__
-00000240: 1000 0000 7304 0000 0006 010c 027a 164d  ....s........z.M
-00000250: 6f64 756c 654d 616e 6167 6572 2e5f 5f69  oduleManager.__i
-00000260: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-00000270: 0000 0200 0000 0400 0000 4300 0000 7332  ..........C...s2
-00000280: 0000 0064 017d 0174 006a 01a0 027c 01a1  ...d.}.t.j...|..
-00000290: 0173 0d74 00a0 037c 01a1 0101 0074 006a  .s.t...|.....t.j
-000002a0: 01a0 0474 00a0 05a1 007c 01a1 027c 005f  ...t.....|...|._
-000002b0: 0664 0053 0029 024e 7a05 2e6d 6174 6529  .d.S.).Nz..mate)
-000002c0: 07da 026f 73da 0470 6174 68da 0665 7869  ...os..path..exi
-000002d0: 7374 73da 056d 6b64 6972 da04 6a6f 696e  sts..mkdir..join
-000002e0: da06 6765 7463 7764 7209 0000 0029 0272  ..getcwdr....).r
-000002f0: 0d00 0000 5a0b 666f 6c64 6572 5f6e 616d  ....Z.folder_nam
-00000300: 6572 0e00 0000 720e 0000 0072 0f00 0000  er....r....r....
-00000310: 720c 0000 0015 0000 0073 0800 0000 0402  r........s......
-00000320: 0c01 0a01 1802 7a20 4d6f 6475 6c65 4d61  ......z ModuleMa
-00000330: 6e61 6765 722e 696e 6974 5f70 6163 6b61  nager.init_packa
-00000340: 6765 5f63 6163 6865 6301 0000 0000 0000  ge_cachec.......
-00000350: 0000 0000 0002 0000 0003 0000 0047 0000  .............G..
-00000360: 0073 1600 0000 7400 6a01 6a02 7c00 6a03  .s....t.j.j.|.j.
-00000370: 6701 7c01 a201 5200 8e00 5300 720b 0000  g.|...R...S.r...
-00000380: 0029 0472 1100 0000 7212 0000 0072 1500  .).r....r....r..
-00000390: 0000 7209 0000 0029 0272 0d00 0000 da04  ..r....).r......
-000003a0: 6172 6773 720e 0000 0072 0e00 0000 720f  argsr....r....r.
-000003b0: 0000 00da 0867 6574 5f70 6174 681d 0000  .....get_path...
-000003c0: 0073 0200 0000 1601 7a16 4d6f 6475 6c65  .s......z.Module
-000003d0: 4d61 6e61 6765 722e 6765 745f 7061 7468  Manager.get_path
-000003e0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-000003f0: 0003 0000 004f 0000 00f3 3000 0000 7400  .....O....0...t.
-00000400: 7c01 8301 6401 6b00 7208 6402 5300 7c01  |...d.k.r.d.S.|.
-00000410: 6403 1900 6404 6b02 7314 6405 7c01 6403  d...d.k.s.d.|.d.
-00000420: 1900 7600 7216 6406 5300 6400 5300 2907  ..v.r.d.S.d.S.).
-00000430: 4e72 0500 0000 4672 0100 0000 7a02 2d79  Nr....Fr....z.-y
-00000440: da01 7954 a901 da03 6c65 6ea9 0372 0d00  ..yT....len..r..
-00000450: 0000 7217 0000 00da 066b 7761 7267 7372  ..r......kwargsr
-00000460: 0e00 0000 720e 0000 0072 0f00 0000 da17  ....r....r......
-00000470: 6368 6563 6b5f 6175 746f 5f69 6e73 7461  check_auto_insta
-00000480: 6c6c 5f72 6571 7320 0000 00f3 0a00 0000  ll_reqs ........
-00000490: 0c01 0401 1801 0401 04ff 7a25 4d6f 6475  ..........z%Modu
-000004a0: 6c65 4d61 6e61 6765 722e 6368 6563 6b5f  leManager.check_
-000004b0: 6175 746f 5f69 6e73 7461 6c6c 5f72 6571  auto_install_req
-000004c0: 7363 0100 0000 0000 0000 0000 0000 0300  sc..............
-000004d0: 0000 0300 0000 4f00 0000 7219 0000 0029  ......O...r....)
-000004e0: 074e 7205 0000 0046 7201 0000 007a 022d  .Nr....Fr....z.-
-000004f0: 6eda 016e 5472 1b00 0000 721d 0000 0072  n..nTr....r....r
-00000500: 0e00 0000 720e 0000 0072 0f00 0000 da1a  ....r....r......
-00000510: 6368 6563 6b5f 6175 746f 5f6e 6f5f 696e  check_auto_no_in
-00000520: 7374 616c 6c5f 7265 7173 2600 0000 7220  stall_reqs&...r 
-00000530: 0000 007a 284d 6f64 756c 654d 616e 6167  ...z(ModuleManag
-00000540: 6572 2e63 6865 636b 5f61 7574 6f5f 6e6f  er.check_auto_no
-00000550: 5f69 6e73 7461 6c6c 5f72 6571 7363 0100  _install_reqsc..
-00000560: 0000 0000 0000 0000 0000 0500 0000 0400  ................
-00000570: 0000 4f00 0000 7372 0000 007c 006a 007c  ..O...sr...|.j.|
-00000580: 0169 007c 02a4 018e 0172 3774 017c 0183  .i.|.....r7t.|..
-00000590: 0164 016b 0472 197c 0164 0119 007d 037c  .d.k.r.|.d...}.|
-000005a0: 0364 0276 0072 187c 0353 006e 0a74 0264  .d.v.r.|.S.n.t.d
-000005b0: 0383 017d 047c 0464 0276 0072 237c 0453  ...}.|.d.v.r#|.S
-000005c0: 007c 0464 0276 0172 357c 0464 0383 017d  .|.d.v.r5|.d...}
-000005d0: 047c 0464 0276 0072 317c 0453 007c 0464  .|.d.v.r1|.S.|.d
-000005e0: 0276 0173 2764 0053 0064 0053 0029 044e  .v.s'd.S.d.S.).N
-000005f0: 7205 0000 0029 02da 0370 6970 da05 636f  r....)...pip..co
-00000600: 6e64 617a 2849 6e73 7461 6c6c 2077 6974  ndaz(Install wit
-00000610: 6820 7069 7020 6f72 2063 6f6e 6461 3f20  h pip or conda? 
-00000620: 5b70 6970 2f63 6f6e 6461 5d3a 2029 0372  [pip/conda]: ).r
-00000630: 1f00 0000 721c 0000 00da 0569 6e70 7574  ....r......input
-00000640: 2905 720d 0000 0072 1700 0000 721e 0000  ).r....r....r...
-00000650: 00da 0270 6dda 0363 6d64 720e 0000 0072  ...pm..cmdr....r
-00000660: 0e00 0000 720f 0000 00da 1461 7574 6f5f  ....r......auto_
-00000670: 696e 7374 616c 6c5f 6d61 6e61 6765 722c  install_manager,
-00000680: 0000 0073 2000 0000 1001 0c01 0801 0801  ...s ...........
-00000690: 0401 02ff 0803 0801 0401 0802 0801 0801  ................
-000006a0: 0401 08fd 0405 0401 7a22 4d6f 6475 6c65  ........z"Module
-000006b0: 4d61 6e61 6765 722e 6175 746f 5f69 6e73  Manager.auto_ins
-000006c0: 7461 6c6c 5f6d 616e 6167 6572 6301 0000  tall_managerc...
-000006d0: 0000 0000 0000 0000 0005 0000 0006 0000  ................
-000006e0: 004f 0000 0073 4e00 0000 7400 7c01 8301  .O...sN...t.|...
-000006f0: 6401 6b00 7208 6402 5300 7a18 7c01 6403  d.k.r.d.S.z.|.d.
-00000700: 1900 6403 1900 7d03 7c03 4400 5d0c 7d04  ..d...}.|.D.].}.
-00000710: 7401 a002 6404 7c04 a102 721d 0100 5700  t...d.|...r...W.
-00000720: 6405 5300 7111 5700 6400 5300 0100 0100  d.S.q.W.d.S.....
-00000730: 0100 5900 6402 5300 2906 4e72 0500 0000  ..Y.d.S.).Nr....
-00000740: 4672 0100 0000 7a05 2d5c 772a 6f54 2903  Fr....z.-\w*oT).
-00000750: 721c 0000 00da 0272 65da 056d 6174 6368  r......re..match
-00000760: 2905 720d 0000 005a 056d 6172 6773 721e  ).r....Z.margsr.
-00000770: 0000 0072 1700 0000 da03 6172 6772 0e00  ...r......argr..
-00000780: 0000 720e 0000 0072 0f00 0000 da14 6368  ..r....r......ch
-00000790: 6563 6b5f 6175 746f 5f6f 7665 7277 7269  eck_auto_overwri
-000007a0: 7465 3f00 0000 7316 0000 000c 0104 0102  te?...s.........
-000007b0: 030c 0108 020c 0108 0102 ff06 ff06 0306  ................
-000007c0: 017a 224d 6f64 756c 654d 616e 6167 6572  .z"ModuleManager
-000007d0: 2e63 6865 636b 5f61 7574 6f5f 6f76 6572  .check_auto_over
-000007e0: 7772 6974 65da 0375 726c 6302 0000 0000  write..urlc.....
-000007f0: 0000 0000 0000 000d 0000 000a 0000 004f  ...............O
-00000800: 0000 0073 4a02 0000 6401 6402 6702 7d04  ...sJ...d.d.g.}.
-00000810: 7c01 a000 6403 a101 6404 6b04 722b 6405  |...d...d.k.r+d.
-00000820: 7c01 7601 722b 7c01 a001 6403 a101 7d01  |.v.r+|...d...}.
-00000830: 6406 7c01 6407 1900 9b00 6403 7c01 6408  d.|.d.....d.|.d.
-00000840: 1900 9b00 6409 6403 a002 7c01 640a 6400  ....d.d...|.d.d.
-00000850: 8502 1900 a101 9b00 9d06 7d01 6e26 7c01  ..........}.n&|.
-00000860: a000 6403 a101 6404 6b02 7251 6405 7c01  ..d...d.k.rQd.|.
-00000870: 7601 7251 7c01 a001 6403 a101 7d01 6406  v.rQ|...d...}.d.
-00000880: 7c01 6407 1900 9b00 6403 7c01 6408 1900  |.d.....d.|.d...
-00000890: 9b00 6409 6403 a002 7c01 6408 6400 8502  ..d.d...|.d.d...
-000008a0: 1900 a101 9b00 9d06 7d01 7403 a004 7c01  ........}.t...|.
-000008b0: a101 735a 4a00 640b 8301 8201 7c00 a005  ..sZJ.d.....|...
-000008c0: 7c01 7c02 7c03 a103 7d05 7c05 9001 721c  |.|.|...}.|...r.
-000008d0: 7406 6a07 a002 7c05 640c a102 7d06 7406  t.j...|.d...}.t.
-000008e0: 6a07 a008 7c06 a101 72db 7c00 6a09 7c02  j...|...r.|.j.|.
-000008f0: 6900 7c03 a401 8e01 72a8 7c00 6a0a 7c02  i.|.....r.|.j.|.
-00000900: 6900 7c03 a401 8e01 7d07 7c07 640d 6b02  i.|.....}.|.d.k.
-00000910: 7292 7406 a00b 640e 7c06 9b00 9d02 a101  r.t...d.|.......
-00000920: 0100 740c 640f 8301 0100 6e4d 7c07 6410  ..t.d.....nM|.d.
-00000930: 6b02 72a3 7406 a00b 6411 7c06 9b00 9d02  k.r.t...d.|.....
-00000940: a101 0100 740c 640f 8301 0100 6e3c 740c  ....t.d.....n<t.
-00000950: 6412 8301 0100 6e37 7c00 6a0d 7c02 6900  d.....n7|.j.|.i.
-00000960: 7c03 a401 8e01 73da 740e 6413 8301 7d08  |.....s.t.d...}.
-00000970: 7c08 6414 6b02 72c5 7406 a00b 640e 7c06  |.d.k.r.t...d.|.
-00000980: 9b00 9d02 a101 0100 740c 640f 8301 0100  ........t.d.....
-00000990: 6e1a 7c08 6410 6b02 72d6 7406 a00b 6411  n.|.d.k.r.t...d.
-000009a0: 7c06 9b00 9d02 a101 0100 740c 640f 8301  |.........t.d...
-000009b0: 0100 6e09 740c 6412 8301 0100 6e04 740c  ..n.t.d.....n.t.
-000009c0: 6415 8301 0100 7406 6a07 a002 7c05 6416  d.....t.j...|.d.
-000009d0: a102 7d09 7406 6a07 a008 7c09 a101 9001  ..}.t.j...|.....
-000009e0: 721c 740f 7c09 6417 8302 8f0d 7d0a 7410  r.t.|.d.....}.t.
-000009f0: a011 7c0a a101 7d0b 5700 6400 0400 0400  ..|...}.W.d.....
-00000a00: 8303 0100 6e09 3100 9001 7303 7701 0100  ....n.1...s.w...
-00000a10: 0100 0100 5900 0100 7c0b 6418 1900 4400  ....Y...|.d...D.
-00000a20: 5d0f 7d0c 7c00 6a12 7c0c 6701 7c02 a201  ].}.|.j.|.g.|...
-00000a30: 5200 6900 7c03 a401 8e01 0100 9001 710c  R.i.|.........q.
-00000a40: 740c 6419 7c05 9b00 9d02 8301 0100 6400  t.d.|.........d.
-00000a50: 5300 291a 4eda 046d 6169 6eda 066d 6173  S.).N..main..mas
-00000a60: 7465 72fa 012f e903 0000 00da 0568 7474  ter../.......htt
-00000a70: 7073 7a13 6874 7470 733a 2f2f 6769 7468  psz.https://gith
-00000a80: 7562 2e63 6f6d 2f72 0100 0000 7205 0000  ub.com/r....r...
-00000a90: 007a 0b2f 7472 6565 2f6d 6169 6e2f e902  .z./tree/main/..
-00000aa0: 0000 007a 0b49 6e76 616c 6964 2075 726c  ...z.Invalid url
-00000ab0: 7a10 7265 7175 6972 656d 656e 7473 2e74  z.requirements.t
-00000ac0: 7874 7223 0000 007a 0f70 6970 2069 6e73  xtr#...z.pip ins
-00000ad0: 7461 6c6c 202d 7220 7208 0000 0072 2400  tall -r r....r$.
-00000ae0: 0000 7a15 636f 6e64 6120 696e 7374 616c  ..z.conda instal
-00000af0: 6c20 2d2d 6669 6c65 207a 2253 6b69 7070  l --file z"Skipp
-00000b00: 696e 6720 7265 7175 6972 656d 656e 7473  ing requirements
-00000b10: 2069 6e73 7461 6c6c 6174 696f 6e7a 4752   installationzGR
-00000b20: 6571 7569 7265 6d65 6e74 7320 666f 756e  equirements foun
-00000b30: 642e 2044 6f20 796f 7520 7761 6e74 2074  d. Do you want t
-00000b40: 6f20 696e 7374 616c 6c20 7468 656d 2077  o install them w
-00000b50: 6974 6820 7069 703f 205b 792f 636f 6e64  ith pip? [y/cond
-00000b60: 612f 6e5d 3a20 721a 0000 007a 3f4e 6f20  a/n]: r....z?No 
-00000b70: 7265 7175 6972 656d 656e 7473 2066 6f75  requirements fou
-00000b80: 6e64 2e20 4d61 6e75 616c 6c79 2063 6865  nd. Manually che
-00000b90: 636b 2061 6e64 2069 6e73 7461 6c6c 2064  ck and install d
-00000ba0: 6570 656e 6465 6e63 6965 732e 7a11 6465  ependencies.z.de
-00000bb0: 7065 6e64 656e 6369 6573 2e6a 736f 6eda  pendencies.json.
-00000bc0: 0172 da0c 6465 7065 6e64 656e 6369 6573  .r..dependencies
-00000bd0: 7a14 4d6f 6475 6c65 2069 6e73 7461 6c6c  z.Module install
-00000be0: 6564 2061 7420 2913 da05 636f 756e 74da  ed at )...count.
-00000bf0: 0573 706c 6974 7215 0000 00da 0a76 616c  .splitr......val
-00000c00: 6964 6174 6f72 7372 2d00 0000 da1f 5f4d  idatorsr-....._M
-00000c10: 6f64 756c 654d 616e 6167 6572 5f5f 696e  oduleManager__in
-00000c20: 7374 616c 6c5f 7061 636b 6167 6572 1100  stall_packager..
-00000c30: 0000 7212 0000 0072 1300 0000 721f 0000  ..r....r....r...
-00000c40: 0072 2800 0000 da06 7379 7374 656d da05  .r(.....system..
-00000c50: 7072 696e 7472 2200 0000 7225 0000 00da  printr"...r%....
-00000c60: 046f 7065 6eda 046a 736f 6eda 046c 6f61  .open..json..loa
-00000c70: 64da 0f69 6e73 7461 6c6c 5f70 6163 6b61  d..install_packa
-00000c80: 6765 290d 720d 0000 0072 2d00 0000 7217  ge).r....r-...r.
-00000c90: 0000 0072 1e00 0000 5a0d 6465 6661 756c  ...r....Z.defaul
-00000ca0: 745f 7472 6565 735a 1370 6163 6b61 6765  t_treesZ.package
-00000cb0: 5f69 6e73 7461 6c6c 5f64 7374 5a11 7265  _install_dstZ.re
-00000cc0: 7175 6972 656d 656e 7473 5f70 6174 6872  quirements_pathr
-00000cd0: 2600 0000 7227 0000 005a 1164 6570 656e  &...r'...Z.depen
-00000ce0: 6465 6e63 6965 735f 7061 7468 da01 6672  dencies_path..fr
-00000cf0: 3500 0000 5a0a 6465 7065 6e64 656e 6379  5...Z.dependency
-00000d00: 720e 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
-00000d10: 3f00 0000 5b00 0000 7354 0000 0008 0216  ?...[...sT......
-00000d20: 030a 022e 0316 040a 042c 0112 060e 0106  .........,......
-00000d30: 030e 010c 0110 0210 0108 0110 010a 0108  ................
-00000d40: 0110 010a 010a 0210 0202 0102 0104 ff08  ................
-00000d50: 0310 010a 0108 0210 010a 0108 0202 8008  ................
-00000d60: 020e 020e 010c 010c 011e ff0c 021c 0212  ................
-00000d70: 047a 1d4d 6f64 756c 654d 616e 6167 6572  .z.ModuleManager
-00000d80: 2e69 6e73 7461 6c6c 5f70 6163 6b61 6765  .install_package
-00000d90: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000da0: 0004 0000 0043 0000 0073 0c00 0000 7400  .....C...s....t.
-00000db0: a001 6401 7c01 a102 5300 2902 4e7a 335e  ..d.|...S.).Nz3^
-00000dc0: 5b61 2d7a 412d 5a5f 5d5b 612d 7a41 2d5a  [a-zA-Z_][a-zA-Z
-00000dd0: 302d 395f 5d2a 285c 2e5b 612d 7a41 2d5a  0-9_]*(\.[a-zA-Z
-00000de0: 5f5d 5b61 2d7a 412d 5a30 2d39 5f5d 2a29  _][a-zA-Z0-9_]*)
-00000df0: 2a24 2902 7229 0000 0072 2a00 0000 2902  *$).r)...r*...).
-00000e00: 720d 0000 00da 046e 616d 6572 0e00 0000  r......namer....
-00000e10: 720e 0000 0072 0f00 0000 5a11 5f5f 6973  r....r....Z.__is
-00000e20: 5f76 616c 6964 5f6d 6f64 756c 65a3 0000  _valid_module...
-00000e30: 0073 0200 0000 0c02 7a1f 4d6f 6475 6c65  .s......z.Module
-00000e40: 4d61 6e61 6765 722e 5f5f 6973 5f76 616c  Manager.__is_val
-00000e50: 6964 5f6d 6f64 756c 6563 0200 0000 0000  id_modulec......
-00000e60: 0000 0000 0000 0e00 0000 0800 0000 4f00  ..............O.
-00000e70: 0000 73c6 0200 0064 01a0 007c 01a0 0164  ..s....d...|...d
-00000e80: 01a1 0164 0064 0285 0219 00a1 017d 0474  ...d.d.......}.t
-00000e90: 02a0 037c 04a0 0464 03a1 01a1 01a0 05a1  ...|...d........
-00000ea0: 007d 057c 00a0 067c 05a1 017d 067c 067d  .}.|...|...}.|.}
-00000eb0: 0774 076a 08a0 097c 06a1 0173 2a74 076a  .t.j...|...s*t.j
-00000ec0: 0a7c 0664 0464 058d 0201 007c 01a0 0164  .|.d.d.....|...d
-00000ed0: 01a1 0164 0619 007d 087c 01a0 0164 01a1  ...d...}.|...d..
-00000ee0: 0164 0719 007d 0974 0b64 087c 089b 0064  .d...}.t.d.|...d
-00000ef0: 017c 099b 0064 097c 049b 009d 0683 0101  .|...d.|........
-00000f00: 007c 0864 0a76 0072 5774 076a 08a0 0074  .|.d.v.rWt.j...t
-00000f10: 07a0 0ca1 007c 006a 0d6a 0e7c 087c 09a1  .....|.j.j.|.|..
-00000f20: 047d 0a6e 687c 0964 0b6b 0272 6574 076a  .}.nh|.d.k.ret.j
-00000f30: 08a0 0074 07a0 0ca1 007c 08a1 027d 0a6e  ...t.....|...}.n
-00000f40: 5a7c 0864 0c76 0072 7374 076a 08a0 0074  Z|.d.v.rst.j...t
-00000f50: 07a0 0ca1 007c 09a1 027d 0a6e 4c74 0b64  .....|...}.nLt.d
-00000f60: 0d83 0101 0074 0f64 0e7c 006a 0d6a 0e9b  .....t.d.|.j.j..
-00000f70: 0064 0f7c 089b 0064 0f7c 099b 0064 109d  .d.|...d.|...d..
-00000f80: 0783 017d 0b7c 0b64 116b 0272 9974 076a  ...}.|.d.k.r.t.j
-00000f90: 08a0 0074 07a0 0ca1 007c 006a 0d6a 0e7c  ...t.....|.j.j.|
-00000fa0: 087c 09a1 047d 0a6e 2674 0f64 1283 017d  .|...}.n&t.d...}
-00000fb0: 0a7c 00a0 107c 0aa1 0173 ab74 0f64 1283  .|...|...s.t.d..
-00000fc0: 017d 0a7c 00a0 107c 0aa1 0172 a27c 0aa0  .}.|...|...r.|..
-00000fd0: 0164 0fa1 017d 0a74 076a 086a 0074 07a0  .d...}.t.j.j.t..
-00000fe0: 0ca1 007c 006a 0d6a 0e67 027c 0aa2 0152  ...|.j.j.g.|...R
-00000ff0: 008e 007d 0a74 076a 08a0 097c 0aa1 0190  ...}.t.j...|....
-00001000: 0172 197c 00a0 117c 027c 03a1 0273 d174  .r.|...|.|...s.t
-00001010: 0f64 1383 017d 0c6e 0264 147d 0c7c 0c64  .d...}.n.d.}.|.d
-00001020: 146b 0272 e174 127c 0a83 0101 0074 0b64  .k.r.t.|.....t.d
-00001030: 157c 0a83 0201 006e 387c 0c64 166b 0272  .|.....n8|.d.k.r
-00001040: e764 0053 007c 0c64 176b 0290 0172 1374  .d.S.|.d.k...r.t
-00001050: 0f64 1283 017d 0a7c 00a0 107c 0aa1 0173  .d...}.|...|...s
-00001060: fe74 0f64 1283 017d 0a7c 00a0 107c 0aa1  .t.d...}.|...|..
-00001070: 0172 f57c 0aa0 0164 0fa1 017d 0a74 076a  .r.|...d...}.t.j
-00001080: 086a 0074 07a0 0ca1 007c 006a 0d6a 0e67  .j.t.....|.j.j.g
-00001090: 027c 0aa2 0152 008e 007d 0a6e 0674 076a  .|...R...}.n.t.j
-000010a0: 08a0 097c 0aa1 0173 c674 0b64 187c 019b  ...|...s.t.d.|..
-000010b0: 009d 0283 0101 007a 0874 137c 017c 0764  .......z.t.|.|.d
-000010c0: 198d 0201 0057 006e 1701 0001 0001 007c  .....W.n.......|
-000010d0: 01a0 1464 1a64 1ba1 027d 0174 0b64 187c  ...d.d...}.t.d.|
-000010e0: 019b 009d 0283 0101 0074 137c 017c 0764  .........t.|.|.d
-000010f0: 198d 0201 0059 007c 01a0 0164 1ca1 0164  .....Y.|...d...d
-00001100: 1d19 00a0 0164 01a1 0164 1e64 0085 0219  .....d...d.d....
-00001110: 007d 0d74 076a 086a 007c 0767 017c 0da2  .}.t.j.j.|.g.|..
-00001120: 0152 008e 007d 0d74 157c 0d7c 0a83 0201  .R...}.t.|.|....
-00001130: 0074 127c 0783 0101 007c 0a53 0029 1f4e  .t.|.....|.S.).N
-00001140: 7230 0000 00e9 0700 0000 7a05 7574 662d  r0........z.utf-
-00001150: 3854 2901 da08 6578 6973 745f 6f6b e9fe  8T)...exist_ok..
-00001160: ffff ffe9 ffff ffff 7a0b 496e 7374 616c  ........z.Instal
-00001170: 6c69 6e67 207a 0620 6672 6f6d 2029 04da  ling z. from )..
-00001180: 066d 6f64 656c 73da 0464 6174 61da 0b65  .models..data..e
-00001190: 7870 6572 696d 656e 7473 da08 7472 6169  xperiments..trai
-000011a0: 6e65 7273 7208 0000 0029 0272 2f00 0000  nersr....).r/...
-000011b0: 722e 0000 007a 4243 6f75 6c64 206e 6f74  r....zBCould not
-000011c0: 2061 7574 6f6d 6174 6963 616c 6c79 2064   automatically d
-000011d0: 6574 6572 6d69 6e65 2074 6865 206d 6f64  etermine the mod
-000011e0: 756c 6520 7479 7065 2e20 506c 6561 7365  ule type. Please
-000011f0: 2073 7065 6369 6679 2e7a 0349 7320 da01   specify.z.Is ..
-00001200: 2e7a 1020 436f 7272 6563 7420 5b79 2c6e  .z. Correct [y,n
-00001210: 5d3f 2072 1a00 0000 7a3a 506c 6561 7365  ]? r....z:Please
-00001220: 2073 7065 6369 6679 2074 6865 2063 6f72   specify the cor
-00001230: 7265 6374 206d 6f64 756c 653a 2028 652e  rect module: (e.
-00001240: 672e 206d 6f64 656c 732e 6d79 5f6d 6f64  g. models.my_mod
-00001250: 656c 2920 7a42 5061 636b 6167 6520 616c  el) zBPackage al
-00001260: 7265 6164 7920 6578 6973 7473 2c20 6f70  ready exists, op
-00001270: 7469 6f6e 733a 205b 6f5d 7665 7277 7269  tions: [o]verwri
-00001280: 7465 2c20 5b63 5d61 6e63 656c 2c20 5b72  te, [c]ancel, [r
-00001290: 5d65 6e61 6d65 3a20 da01 6f7a 1c44 656c  ]ename: ..oz.Del
-000012a0: 6574 6564 2065 7869 7374 696e 6720 7061  eted existing pa
-000012b0: 636b 6167 6520 6174 20da 0163 7234 0000  ckage at ..cr4..
-000012c0: 007a 0c44 6f77 6e6c 6f61 6469 6e67 2029  .z.Downloading )
-000012d0: 01da 0a6f 7574 7075 745f 6469 727a 062f  ...output_dirz./
-000012e0: 6d61 696e 2f7a 082f 6d61 7374 6572 2fda  main/z./master/.
-000012f0: 0474 7265 6572 0500 0000 7233 0000 0029  .treer....r3...)
-00001300: 1672 1500 0000 7237 0000 00da 0768 6173  .r....r7.....has
-00001310: 686c 6962 da04 7368 6131 da06 656e 636f  hlib..sha1..enco
-00001320: 6465 da09 6865 7864 6967 6573 7472 1800  de..hexdigestr..
-00001330: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00001340: 00da 086d 616b 6564 6972 7372 3b00 0000  ...makedirsr;...
-00001350: 7216 0000 0072 0a00 0000 da07 7072 6f6a  r....r......proj
-00001360: 6563 7472 2500 0000 da1f 5f4d 6f64 756c  ectr%....._Modul
-00001370: 654d 616e 6167 6572 5f5f 6973 5f76 616c  eManager__is_val
-00001380: 6964 5f6d 6f64 756c 6572 2c00 0000 7203  id_moduler,...r.
-00001390: 0000 0072 0600 0000 da07 7265 706c 6163  ...r......replac
-000013a0: 6572 0200 0000 290e 720d 0000 0072 2d00  er....).r....r-.
-000013b0: 0000 7217 0000 0072 1e00 0000 5a0c 6261  ..r....r....Z.ba
-000013c0: 7365 5f67 6974 5f75 726c 5a08 7572 6c5f  se_git_urlZ.url_
-000013d0: 6861 7368 da0b 6f75 7470 7574 5f70 6174  hash..output_pat
-000013e0: 6872 4d00 0000 5a0b 726f 6f74 5f6d 6f64  hrM...Z.root_mod
-000013f0: 756c 65da 0b6d 6f64 756c 655f 6e61 6d65  ule..module_name
-00001400: da09 6465 7374 5f70 6174 68da 0763 6f6d  ..dest_path..com
-00001410: 6d61 6e64 7227 0000 005a 0a73 7263 5f6d  mandr'...Z.src_m
-00001420: 6f64 756c 6572 0e00 0000 720e 0000 0072  oduler....r....r
-00001430: 0f00 0000 5a11 5f5f 696e 7374 616c 6c5f  ....Z.__install_
-00001440: 7061 636b 6167 65a8 0000 0073 9400 0000  package....s....
-00001450: 1803 1402 0a02 0401 0c02 0e01 0e02 0e01  ................
-00001460: 1a02 0802 0601 1001 06ff 0806 1401 0801  ................
-00001470: 1401 0202 0201 04ff 0203 1a01 04ff 0803  ................
-00001480: 0601 1001 06ff 0204 0201 04ff 0a03 0201  ................
-00001490: 0201 04ff 0aff 0a04 1e01 0e02 0c01 0201  ................
-000014a0: 0201 06ff 0404 0802 0801 0a01 0201 0802  ................
-000014b0: 0401 0a02 0201 0201 04ff 0a03 0201 0201  ................
-000014c0: 04ff 0aff 0a04 1e01 0201 0ce6 0e1c 0202  ................
-000014d0: 1001 0601 0c02 0e01 0e01 1c02 1401 0a05  ................
-000014e0: 0801 0401 7a1f 4d6f 6475 6c65 4d61 6e61  ....z.ModuleMana
-000014f0: 6765 722e 5f5f 696e 7374 616c 6c5f 7061  ger.__install_pa
-00001500: 636b 6167 654e 2911 da08 5f5f 6e61 6d65  ckageN)...__name
-00001510: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00001520: 5f5f 7175 616c 6e61 6d65 5f5f 7209 0000  __qualname__r...
-00001530: 00da 0373 7472 da0f 5f5f 616e 6e6f 7461  ...str..__annota
-00001540: 7469 6f6e 735f 5f72 0400 0000 7210 0000  tions__r....r...
-00001550: 0072 0c00 0000 7218 0000 0072 1f00 0000  .r....r....r....
-00001560: 7222 0000 0072 2800 0000 722c 0000 0072  r"...r(...r,...r
-00001570: 3f00 0000 7255 0000 0072 3900 0000 720e  ?...rU...r9...r.
-00001580: 0000 0072 0e00 0000 720e 0000 0072 0f00  ...r....r....r..
-00001590: 0000 7207 0000 000d 0000 0073 1800 0000  ..r........s....
-000015a0: 0a00 0c01 0e02 0805 0808 0803 0806 0806  ................
-000015b0: 0813 0e1c 0848 0c05 7207 0000 0029 0e72  .....H..r....).r
-000015c0: 4f00 0000 723d 0000 0072 1100 0000 7229  O...r=...r....r)
-000015d0: 0000 00da 0673 6875 7469 6c72 0200 0000  .....shutilr....
-000015e0: 7203 0000 0072 3800 0000 da15 7965 7262  r....r8.....yerb
-000015f0: 616d 6174 652e 6d61 7465 5f63 6f6e 6669  amate.mate_confi
-00001600: 6772 0400 0000 5a0c 7574 696c 732e 6769  gr....Z.utils.gi
-00001610: 7464 6972 7206 0000 00da 0469 7064 6272  tdirr......ipdbr
-00001620: 0700 0000 720e 0000 0072 0e00 0000 720e  ....r....r....r.
-00001630: 0000 0072 0f00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00001640: 653e 0100 0000 7314 0000 0008 0008 0108  e>....s.........
-00001650: 0108 0110 0108 010c 010c 0208 0112 03    ...............
+00000060: 6401 6c07 5a07 6403 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
+00000070: 0100 6400 6401 6c0a 5a0a 4700 6405 6406  ..d.d.l.Z.G.d.d.
+00000080: 8400 6406 8302 5a0b 6401 5300 2907 e900  ..d...Z.d.S.)...
+00000090: 0000 004e 2902 da08 636f 7079 7472 6565  ...N)...copytree
+000000a0: da06 726d 7472 6565 e901 0000 0029 01da  ..rmtree.....)..
+000000b0: 0864 6f77 6e6c 6f61 6463 0000 0000 0000  .downloadc......
+000000c0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+000000d0: 0000 7370 0000 0065 005a 0164 005a 0255  ..sp...e.Z.d.Z.U
+000000e0: 0064 015a 0365 0465 0564 023c 0064 0364  .d.Z.e.e.d.<.d.d
+000000f0: 0484 005a 0664 0564 0684 005a 0764 0764  ...Z.d.d...Z.d.d
+00000100: 0884 005a 0864 0964 0a84 005a 0964 0b64  ...Z.d.d...Z.d.d
+00000110: 0c84 005a 0a64 0d64 0e84 005a 0b64 0f64  ...Z.d.d...Z.d.d
+00000120: 1084 005a 0c64 1165 0466 0264 1264 1384  ...Z.d.e.f.d.d..
+00000130: 045a 0d64 1464 1584 005a 0e64 1664 1784  .Z.d.d...Z.d.d..
+00000140: 005a 0f64 1853 0029 19da 0d4d 6f64 756c  .Z.d.S.)...Modul
+00000150: 654d 616e 6167 6572 da00 da09 726f 6f74  eManager....root
+00000160: 5f70 6174 6863 0200 0000 0000 0000 0000  _pathc..........
+00000170: 0000 0200 0000 0200 0000 4300 0000 7312  ..........C...s.
+00000180: 0000 007c 017c 005f 007c 00a0 01a1 0001  ...|.|._.|......
+00000190: 0064 0053 00a9 014e 2902 da04 636f 6e66  .d.S...N)...conf
+000001a0: da12 696e 6974 5f70 6163 6b61 6765 5f63  ..init_package_c
+000001b0: 6163 6865 2902 da04 7365 6c66 720a 0000  ache)...selfr...
+000001c0: 00a9 0072 0d00 0000 fa47 2f68 6f6d 652f  ...r.....G/home/
+000001d0: 616c 2f47 6974 4875 622f 7965 7262 616d  al/GitHub/yerbam
+000001e0: 6174 652f 7061 636b 6167 6573 2f79 6572  ate/packages/yer
+000001f0: 6261 6d61 7465 2f61 7069 2f64 6174 612f  bamate/api/data/
+00000200: 6d6f 6475 6c65 5f6d 616e 6167 6572 2e70  module_manager.p
+00000210: 79da 085f 5f69 6e69 745f 5f10 0000 0073  y..__init__....s
+00000220: 0400 0000 0601 0c02 7a16 4d6f 6475 6c65  ........z.Module
+00000230: 4d61 6e61 6765 722e 5f5f 696e 6974 5f5f  Manager.__init__
+00000240: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000250: 0004 0000 0043 0000 0073 3200 0000 6401  .....C...s2...d.
+00000260: 7d01 7400 6a01 a002 7c01 a101 730d 7400  }.t.j...|...s.t.
+00000270: a003 7c01 a101 0100 7400 6a01 a004 7400  ..|.....t.j...t.
+00000280: a005 a100 7c01 a102 7c00 5f06 6400 5300  ....|...|._.d.S.
+00000290: 2902 4e7a 052e 6d61 7465 2907 da02 6f73  ).Nz..mate)...os
+000002a0: da04 7061 7468 da06 6578 6973 7473 da05  ..path..exists..
+000002b0: 6d6b 6469 72da 046a 6f69 6eda 0667 6574  mkdir..join..get
+000002c0: 6377 6472 0800 0000 2902 720c 0000 005a  cwdr....).r....Z
+000002d0: 0b66 6f6c 6465 725f 6e61 6d65 720d 0000  .folder_namer...
+000002e0: 0072 0d00 0000 720e 0000 0072 0b00 0000  .r....r....r....
+000002f0: 1500 0000 7308 0000 0004 020c 010a 0118  ....s...........
+00000300: 027a 204d 6f64 756c 654d 616e 6167 6572  .z ModuleManager
+00000310: 2e69 6e69 745f 7061 636b 6167 655f 6361  .init_package_ca
+00000320: 6368 6563 0100 0000 0000 0000 0000 0000  chec............
+00000330: 0200 0000 0300 0000 4700 0000 7316 0000  ........G...s...
+00000340: 0074 006a 016a 027c 006a 0367 017c 01a2  .t.j.j.|.j.g.|..
+00000350: 0152 008e 0053 0072 0900 0000 2904 7210  .R...S.r....).r.
+00000360: 0000 0072 1100 0000 7214 0000 0072 0800  ...r....r....r..
+00000370: 0000 2902 720c 0000 00da 0461 7267 7372  ..).r......argsr
+00000380: 0d00 0000 720d 0000 0072 0e00 0000 da08  ....r....r......
+00000390: 6765 745f 7061 7468 1d00 0000 7302 0000  get_path....s...
+000003a0: 0016 017a 164d 6f64 756c 654d 616e 6167  ...z.ModuleManag
+000003b0: 6572 2e67 6574 5f70 6174 6863 0100 0000  er.get_pathc....
+000003c0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+000003d0: 4f00 0000 f330 0000 0074 007c 0183 0164  O....0...t.|...d
+000003e0: 016b 0072 0864 0253 007c 0164 0319 0064  .k.r.d.S.|.d...d
+000003f0: 046b 0273 1464 057c 0164 0319 0076 0072  .k.s.d.|.d...v.r
+00000400: 1664 0653 0064 0053 0029 074e 7204 0000  .d.S.d.S.).Nr...
+00000410: 0046 7201 0000 007a 022d 79da 0179 54a9  .Fr....z.-y..yT.
+00000420: 01da 036c 656e a903 720c 0000 0072 1600  ...len..r....r..
+00000430: 0000 da06 6b77 6172 6773 720d 0000 0072  ....kwargsr....r
+00000440: 0d00 0000 720e 0000 00da 1763 6865 636b  ....r......check
+00000450: 5f61 7574 6f5f 696e 7374 616c 6c5f 7265  _auto_install_re
+00000460: 7173 2000 0000 f30a 0000 000c 0104 0118  qs .............
+00000470: 0104 0104 ff7a 254d 6f64 756c 654d 616e  .....z%ModuleMan
+00000480: 6167 6572 2e63 6865 636b 5f61 7574 6f5f  ager.check_auto_
+00000490: 696e 7374 616c 6c5f 7265 7173 6301 0000  install_reqsc...
+000004a0: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+000004b0: 004f 0000 0072 1800 0000 2907 4e72 0400  .O...r....).Nr..
+000004c0: 0000 4672 0100 0000 7a02 2d6e da01 6e54  ..Fr....z.-n..nT
+000004d0: 721a 0000 0072 1c00 0000 720d 0000 0072  r....r....r....r
+000004e0: 0d00 0000 720e 0000 00da 1a63 6865 636b  ....r......check
+000004f0: 5f61 7574 6f5f 6e6f 5f69 6e73 7461 6c6c  _auto_no_install
+00000500: 5f72 6571 7326 0000 0072 1f00 0000 7a28  _reqs&...r....z(
+00000510: 4d6f 6475 6c65 4d61 6e61 6765 722e 6368  ModuleManager.ch
+00000520: 6563 6b5f 6175 746f 5f6e 6f5f 696e 7374  eck_auto_no_inst
+00000530: 616c 6c5f 7265 7173 6301 0000 0000 0000  all_reqsc.......
+00000540: 0000 0000 0005 0000 0004 0000 004f 0000  .............O..
+00000550: 0073 7200 0000 7c00 6a00 7c01 6900 7c02  .sr...|.j.|.i.|.
+00000560: a401 8e01 7237 7401 7c01 8301 6401 6b04  ....r7t.|...d.k.
+00000570: 7219 7c01 6401 1900 7d03 7c03 6402 7600  r.|.d...}.|.d.v.
+00000580: 7218 7c03 5300 6e0a 7402 6403 8301 7d04  r.|.S.n.t.d...}.
+00000590: 7c04 6402 7600 7223 7c04 5300 7c04 6402  |.d.v.r#|.S.|.d.
+000005a0: 7601 7235 7c04 6403 8301 7d04 7c04 6402  v.r5|.d...}.|.d.
+000005b0: 7600 7231 7c04 5300 7c04 6402 7601 7327  v.r1|.S.|.d.v.s'
+000005c0: 6400 5300 6400 5300 2904 4e72 0400 0000  d.S.d.S.).Nr....
+000005d0: 2902 da03 7069 70da 0563 6f6e 6461 7a28  )...pip..condaz(
+000005e0: 496e 7374 616c 6c20 7769 7468 2070 6970  Install with pip
+000005f0: 206f 7220 636f 6e64 613f 205b 7069 702f   or conda? [pip/
+00000600: 636f 6e64 615d 3a20 2903 721e 0000 0072  conda]: ).r....r
+00000610: 1b00 0000 da05 696e 7075 7429 0572 0c00  ......input).r..
+00000620: 0000 7216 0000 0072 1d00 0000 da02 706d  ..r....r......pm
+00000630: da03 636d 6472 0d00 0000 720d 0000 0072  ..cmdr....r....r
+00000640: 0e00 0000 da14 6175 746f 5f69 6e73 7461  ......auto_insta
+00000650: 6c6c 5f6d 616e 6167 6572 2c00 0000 7320  ll_manager,...s 
+00000660: 0000 0010 010c 0108 0108 0104 0102 ff08  ................
+00000670: 0308 0104 0108 0208 0108 0104 0108 fd04  ................
+00000680: 0504 017a 224d 6f64 756c 654d 616e 6167  ...z"ModuleManag
+00000690: 6572 2e61 7574 6f5f 696e 7374 616c 6c5f  er.auto_install_
+000006a0: 6d61 6e61 6765 7263 0100 0000 0000 0000  managerc........
+000006b0: 0000 0000 0500 0000 0600 0000 4f00 0000  ............O...
+000006c0: 734e 0000 0074 007c 0183 0164 016b 0072  sN...t.|...d.k.r
+000006d0: 0864 0253 007a 187c 0164 0319 0064 0319  .d.S.z.|.d...d..
+000006e0: 007d 037c 0344 005d 0c7d 0474 01a0 0264  .}.|.D.].}.t...d
+000006f0: 047c 04a1 0272 1d01 0057 0064 0553 0071  .|...r...W.d.S.q
+00000700: 1157 0064 0053 0001 0001 0001 0059 0064  .W.d.S.......Y.d
+00000710: 0253 0029 064e 7204 0000 0046 7201 0000  .S.).Nr....Fr...
+00000720: 007a 052d 5c77 2a6f 5429 0372 1b00 0000  .z.-\w*oT).r....
+00000730: da02 7265 da05 6d61 7463 6829 0572 0c00  ..re..match).r..
+00000740: 0000 5a05 6d61 7267 7372 1d00 0000 7216  ..Z.margsr....r.
+00000750: 0000 00da 0361 7267 720d 0000 0072 0d00  .....argr....r..
+00000760: 0000 720e 0000 00da 1463 6865 636b 5f61  ..r......check_a
+00000770: 7574 6f5f 6f76 6572 7772 6974 653f 0000  uto_overwrite?..
+00000780: 0073 1600 0000 0c01 0401 0203 0c01 0802  .s..............
+00000790: 0c01 0801 02ff 06ff 0603 0601 7a22 4d6f  ............z"Mo
+000007a0: 6475 6c65 4d61 6e61 6765 722e 6368 6563  duleManager.chec
+000007b0: 6b5f 6175 746f 5f6f 7665 7277 7269 7465  k_auto_overwrite
+000007c0: da03 7572 6c63 0200 0000 0000 0000 0000  ..urlc..........
+000007d0: 0000 0d00 0000 0a00 0000 4f00 0000 734a  ..........O...sJ
+000007e0: 0200 0064 0164 0267 027d 047c 01a0 0064  ...d.d.g.}.|...d
+000007f0: 03a1 0164 046b 0472 2b64 057c 0176 0172  ...d.k.r+d.|.v.r
+00000800: 2b7c 01a0 0164 03a1 017d 0164 067c 0164  +|...d...}.d.|.d
+00000810: 0719 009b 0064 037c 0164 0819 009b 0064  .....d.|.d.....d
+00000820: 0964 03a0 027c 0164 0a64 0085 0219 00a1  .d...|.d.d......
+00000830: 019b 009d 067d 016e 267c 01a0 0064 03a1  .....}.n&|...d..
+00000840: 0164 046b 0272 5164 057c 0176 0172 517c  .d.k.rQd.|.v.rQ|
+00000850: 01a0 0164 03a1 017d 0164 067c 0164 0719  ...d...}.d.|.d..
+00000860: 009b 0064 037c 0164 0819 009b 0064 0964  ...d.|.d.....d.d
+00000870: 03a0 027c 0164 0864 0085 0219 00a1 019b  ...|.d.d........
+00000880: 009d 067d 0174 03a0 047c 01a1 0173 5a4a  ...}.t...|...sZJ
+00000890: 0064 0b83 0182 017c 00a0 057c 017c 027c  .d.....|...|.|.|
+000008a0: 03a1 037d 057c 0590 0172 1c74 066a 07a0  ...}.|...r.t.j..
+000008b0: 027c 0564 0ca1 027d 0674 066a 07a0 087c  .|.d...}.t.j...|
+000008c0: 06a1 0172 db7c 006a 097c 0269 007c 03a4  ...r.|.j.|.i.|..
+000008d0: 018e 0172 a87c 006a 0a7c 0269 007c 03a4  ...r.|.j.|.i.|..
+000008e0: 018e 017d 077c 0764 0d6b 0272 9274 06a0  ...}.|.d.k.r.t..
+000008f0: 0b64 0e7c 069b 009d 02a1 0101 0074 0c64  .d.|.........t.d
+00000900: 0f83 0101 006e 4d7c 0764 106b 0272 a374  .....nM|.d.k.r.t
+00000910: 06a0 0b64 117c 069b 009d 02a1 0101 0074  ...d.|.........t
+00000920: 0c64 0f83 0101 006e 3c74 0c64 1283 0101  .d.....n<t.d....
+00000930: 006e 377c 006a 0d7c 0269 007c 03a4 018e  .n7|.j.|.i.|....
+00000940: 0173 da74 0e64 1383 017d 087c 0864 146b  .s.t.d...}.|.d.k
+00000950: 0272 c574 06a0 0b64 0e7c 069b 009d 02a1  .r.t...d.|......
+00000960: 0101 0074 0c64 0f83 0101 006e 1a7c 0864  ...t.d.....n.|.d
+00000970: 106b 0272 d674 06a0 0b64 117c 069b 009d  .k.r.t...d.|....
+00000980: 02a1 0101 0074 0c64 0f83 0101 006e 0974  .....t.d.....n.t
+00000990: 0c64 1283 0101 006e 0474 0c64 1583 0101  .d.....n.t.d....
+000009a0: 0074 066a 07a0 027c 0564 16a1 027d 0974  .t.j...|.d...}.t
+000009b0: 066a 07a0 087c 09a1 0190 0172 1c74 0f7c  .j...|.....r.t.|
+000009c0: 0964 1783 028f 0d7d 0a74 10a0 117c 0aa1  .d.....}.t...|..
+000009d0: 017d 0b57 0064 0004 0004 0083 0301 006e  .}.W.d.........n
+000009e0: 0931 0090 0173 0377 0101 0001 0001 0059  .1...s.w.......Y
+000009f0: 0001 007c 0b64 1819 0044 005d 0f7d 0c7c  ...|.d...D.].}.|
+00000a00: 006a 127c 0c67 017c 02a2 0152 0069 007c  .j.|.g.|...R.i.|
+00000a10: 03a4 018e 0101 0090 0171 0c74 0c64 197c  .........q.t.d.|
+00000a20: 059b 009d 0283 0101 0064 0053 0029 1a4e  .........d.S.).N
+00000a30: da04 6d61 696e da06 6d61 7374 6572 fa01  ..main..master..
+00000a40: 2fe9 0300 0000 da05 6874 7470 737a 1368  /.......httpsz.h
+00000a50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000a60: 6d2f 7201 0000 0072 0400 0000 7a0b 2f74  m/r....r....z./t
+00000a70: 7265 652f 6d61 696e 2fe9 0200 0000 7a0b  ree/main/.....z.
+00000a80: 496e 7661 6c69 6420 7572 6c7a 1072 6571  Invalid urlz.req
+00000a90: 7569 7265 6d65 6e74 732e 7478 7472 2200  uirements.txtr".
+00000aa0: 0000 7a0f 7069 7020 696e 7374 616c 6c20  ..z.pip install 
+00000ab0: 2d72 2072 0700 0000 7223 0000 007a 1563  -r r....r#...z.c
+00000ac0: 6f6e 6461 2069 6e73 7461 6c6c 202d 2d66  onda install --f
+00000ad0: 696c 6520 7a22 536b 6970 7069 6e67 2072  ile z"Skipping r
+00000ae0: 6571 7569 7265 6d65 6e74 7320 696e 7374  equirements inst
+00000af0: 616c 6c61 7469 6f6e 7a47 5265 7175 6972  allationzGRequir
+00000b00: 656d 656e 7473 2066 6f75 6e64 2e20 446f  ements found. Do
+00000b10: 2079 6f75 2077 616e 7420 746f 2069 6e73   you want to ins
+00000b20: 7461 6c6c 2074 6865 6d20 7769 7468 2070  tall them with p
+00000b30: 6970 3f20 5b79 2f63 6f6e 6461 2f6e 5d3a  ip? [y/conda/n]:
+00000b40: 2072 1900 0000 7a3f 4e6f 2072 6571 7569   r....z?No requi
+00000b50: 7265 6d65 6e74 7320 666f 756e 642e 204d  rements found. M
+00000b60: 616e 7561 6c6c 7920 6368 6563 6b20 616e  anually check an
+00000b70: 6420 696e 7374 616c 6c20 6465 7065 6e64  d install depend
+00000b80: 656e 6369 6573 2e7a 1164 6570 656e 6465  encies.z.depende
+00000b90: 6e63 6965 732e 6a73 6f6e da01 72da 0c64  ncies.json..r..d
+00000ba0: 6570 656e 6465 6e63 6965 737a 144d 6f64  ependenciesz.Mod
+00000bb0: 756c 6520 696e 7374 616c 6c65 6420 6174  ule installed at
+00000bc0: 2029 13da 0563 6f75 6e74 da05 7370 6c69   )...count..spli
+00000bd0: 7472 1400 0000 da0a 7661 6c69 6461 746f  tr......validato
+00000be0: 7273 722c 0000 00da 1f5f 4d6f 6475 6c65  rsr,....._Module
+00000bf0: 4d61 6e61 6765 725f 5f69 6e73 7461 6c6c  Manager__install
+00000c00: 5f70 6163 6b61 6765 7210 0000 0072 1100  _packager....r..
+00000c10: 0000 7212 0000 0072 1e00 0000 7227 0000  ..r....r....r'..
+00000c20: 00da 0673 7973 7465 6dda 0570 7269 6e74  ...system..print
+00000c30: 7221 0000 0072 2400 0000 da04 6f70 656e  r!...r$.....open
+00000c40: da04 6a73 6f6e da04 6c6f 6164 da0f 696e  ..json..load..in
+00000c50: 7374 616c 6c5f 7061 636b 6167 6529 0d72  stall_package).r
+00000c60: 0c00 0000 722c 0000 0072 1600 0000 721d  ....r,...r....r.
+00000c70: 0000 005a 0d64 6566 6175 6c74 5f74 7265  ...Z.default_tre
+00000c80: 6573 5a13 7061 636b 6167 655f 696e 7374  esZ.package_inst
+00000c90: 616c 6c5f 6473 745a 1172 6571 7569 7265  all_dstZ.require
+00000ca0: 6d65 6e74 735f 7061 7468 7225 0000 0072  ments_pathr%...r
+00000cb0: 2600 0000 5a11 6465 7065 6e64 656e 6369  &...Z.dependenci
+00000cc0: 6573 5f70 6174 68da 0166 7234 0000 005a  es_path..fr4...Z
+00000cd0: 0a64 6570 656e 6465 6e63 7972 0d00 0000  .dependencyr....
+00000ce0: 720d 0000 0072 0e00 0000 723e 0000 005b  r....r....r>...[
+00000cf0: 0000 0073 5400 0000 0802 1603 0a02 2e03  ...sT...........
+00000d00: 1604 0a04 2c01 1206 0e01 0603 0e01 0c01  ....,...........
+00000d10: 1002 1001 0801 1001 0a01 0801 1001 0a01  ................
+00000d20: 0a02 1002 0201 0201 04ff 0803 1001 0a01  ................
+00000d30: 0802 1001 0a01 0802 0280 0802 0e02 0e01  ................
+00000d40: 0c01 0c01 1eff 0c02 1c02 1204 7a1d 4d6f  ............z.Mo
+00000d50: 6475 6c65 4d61 6e61 6765 722e 696e 7374  duleManager.inst
+00000d60: 616c 6c5f 7061 636b 6167 6563 0200 0000  all_packagec....
+00000d70: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000d80: 4300 0000 730c 0000 0074 00a0 0164 017c  C...s....t...d.|
+00000d90: 01a1 0253 0029 024e 7a33 5e5b 612d 7a41  ...S.).Nz3^[a-zA
+00000da0: 2d5a 5f5d 5b61 2d7a 412d 5a30 2d39 5f5d  -Z_][a-zA-Z0-9_]
+00000db0: 2a28 5c2e 5b61 2d7a 412d 5a5f 5d5b 612d  *(\.[a-zA-Z_][a-
+00000dc0: 7a41 2d5a 302d 395f 5d2a 292a 2429 0272  zA-Z0-9_]*)*$).r
+00000dd0: 2800 0000 7229 0000 0029 0272 0c00 0000  (...r)...).r....
+00000de0: da04 6e61 6d65 720d 0000 0072 0d00 0000  ..namer....r....
+00000df0: 720e 0000 005a 115f 5f69 735f 7661 6c69  r....Z.__is_vali
+00000e00: 645f 6d6f 6475 6c65 a300 0000 7302 0000  d_module....s...
+00000e10: 000c 027a 1f4d 6f64 756c 654d 616e 6167  ...z.ModuleManag
+00000e20: 6572 2e5f 5f69 735f 7661 6c69 645f 6d6f  er.__is_valid_mo
+00000e30: 6475 6c65 6302 0000 0000 0000 0000 0000  dulec...........
+00000e40: 000e 0000 0008 0000 004f 0000 0073 c602  .........O...s..
+00000e50: 0000 6401 a000 7c01 a001 6401 a101 6400  ..d...|...d...d.
+00000e60: 6402 8502 1900 a101 7d04 7402 a003 7c04  d.......}.t...|.
+00000e70: a004 6403 a101 a101 a005 a100 7d05 7c00  ..d.........}.|.
+00000e80: a006 7c05 a101 7d06 7c06 7d07 7407 6a08  ..|...}.|.}.t.j.
+00000e90: a009 7c06 a101 732a 7407 6a0a 7c06 6404  ..|...s*t.j.|.d.
+00000ea0: 6405 8d02 0100 7c01 a001 6401 a101 6406  d.....|...d...d.
+00000eb0: 1900 7d08 7c01 a001 6401 a101 6407 1900  ..}.|...d...d...
+00000ec0: 7d09 740b 6408 7c08 9b00 6401 7c09 9b00  }.t.d.|...d.|...
+00000ed0: 6409 7c04 9b00 9d06 8301 0100 7c08 640a  d.|.........|.d.
+00000ee0: 7600 7257 7407 6a08 a000 7407 a00c a100  v.rWt.j...t.....
+00000ef0: 7c00 6a0d 6a0e 7c08 7c09 a104 7d0a 6e68  |.j.j.|.|...}.nh
+00000f00: 7c09 640b 6b02 7265 7407 6a08 a000 7407  |.d.k.ret.j...t.
+00000f10: a00c a100 7c08 a102 7d0a 6e5a 7c08 640c  ....|...}.nZ|.d.
+00000f20: 7600 7273 7407 6a08 a000 7407 a00c a100  v.rst.j...t.....
+00000f30: 7c09 a102 7d0a 6e4c 740b 640d 8301 0100  |...}.nLt.d.....
+00000f40: 740f 640e 7c00 6a0d 6a0e 9b00 640f 7c08  t.d.|.j.j...d.|.
+00000f50: 9b00 640f 7c09 9b00 6410 9d07 8301 7d0b  ..d.|...d.....}.
+00000f60: 7c0b 6411 6b02 7299 7407 6a08 a000 7407  |.d.k.r.t.j...t.
+00000f70: a00c a100 7c00 6a0d 6a0e 7c08 7c09 a104  ....|.j.j.|.|...
+00000f80: 7d0a 6e26 740f 6412 8301 7d0a 7c00 a010  }.n&t.d...}.|...
+00000f90: 7c0a a101 73ab 740f 6412 8301 7d0a 7c00  |...s.t.d...}.|.
+00000fa0: a010 7c0a a101 72a2 7c0a a001 640f a101  ..|...r.|...d...
+00000fb0: 7d0a 7407 6a08 6a00 7407 a00c a100 7c00  }.t.j.j.t.....|.
+00000fc0: 6a0d 6a0e 6702 7c0a a201 5200 8e00 7d0a  j.j.g.|...R...}.
+00000fd0: 7407 6a08 a009 7c0a a101 9001 7219 7c00  t.j...|.....r.|.
+00000fe0: a011 7c02 7c03 a102 73d1 740f 6413 8301  ..|.|...s.t.d...
+00000ff0: 7d0c 6e02 6414 7d0c 7c0c 6414 6b02 72e1  }.n.d.}.|.d.k.r.
+00001000: 7412 7c0a 8301 0100 740b 6415 7c0a 8302  t.|.....t.d.|...
+00001010: 0100 6e38 7c0c 6416 6b02 72e7 6400 5300  ..n8|.d.k.r.d.S.
+00001020: 7c0c 6417 6b02 9001 7213 740f 6412 8301  |.d.k...r.t.d...
+00001030: 7d0a 7c00 a010 7c0a a101 73fe 740f 6412  }.|...|...s.t.d.
+00001040: 8301 7d0a 7c00 a010 7c0a a101 72f5 7c0a  ..}.|...|...r.|.
+00001050: a001 640f a101 7d0a 7407 6a08 6a00 7407  ..d...}.t.j.j.t.
+00001060: a00c a100 7c00 6a0d 6a0e 6702 7c0a a201  ....|.j.j.g.|...
+00001070: 5200 8e00 7d0a 6e06 7407 6a08 a009 7c0a  R...}.n.t.j...|.
+00001080: a101 73c6 740b 6418 7c01 9b00 9d02 8301  ..s.t.d.|.......
+00001090: 0100 7a08 7413 7c01 7c07 6419 8d02 0100  ..z.t.|.|.d.....
+000010a0: 5700 6e17 0100 0100 0100 7c01 a014 641a  W.n.......|...d.
+000010b0: 641b a102 7d01 740b 6418 7c01 9b00 9d02  d...}.t.d.|.....
+000010c0: 8301 0100 7413 7c01 7c07 6419 8d02 0100  ....t.|.|.d.....
+000010d0: 5900 7c01 a001 641c a101 641d 1900 a001  Y.|...d...d.....
+000010e0: 6401 a101 641e 6400 8502 1900 7d0d 7407  d...d.d.....}.t.
+000010f0: 6a08 6a00 7c07 6701 7c0d a201 5200 8e00  j.j.|.g.|...R...
+00001100: 7d0d 7415 7c0d 7c0a 8302 0100 7412 7c07  }.t.|.|.....t.|.
+00001110: 8301 0100 7c0a 5300 291f 4e72 2f00 0000  ....|.S.).Nr/...
+00001120: e907 0000 007a 0575 7466 2d38 5429 01da  .....z.utf-8T)..
+00001130: 0865 7869 7374 5f6f 6be9 feff ffff e9ff  .exist_ok.......
+00001140: ffff ff7a 0b49 6e73 7461 6c6c 696e 6720  ...z.Installing 
+00001150: 7a06 2066 726f 6d20 2904 da06 6d6f 6465  z. from )...mode
+00001160: 6c73 da04 6461 7461 da0b 6578 7065 7269  ls..data..experi
+00001170: 6d65 6e74 73da 0874 7261 696e 6572 7372  ments..trainersr
+00001180: 0700 0000 2902 722e 0000 0072 2d00 0000  ....).r....r-...
+00001190: 7a42 436f 756c 6420 6e6f 7420 6175 746f  zBCould not auto
+000011a0: 6d61 7469 6361 6c6c 7920 6465 7465 726d  matically determ
+000011b0: 696e 6520 7468 6520 6d6f 6475 6c65 2074  ine the module t
+000011c0: 7970 652e 2050 6c65 6173 6520 7370 6563  ype. Please spec
+000011d0: 6966 792e 7a03 4973 20da 012e 7a10 2043  ify.z.Is ...z. C
+000011e0: 6f72 7265 6374 205b 792c 6e5d 3f20 7219  orrect [y,n]? r.
+000011f0: 0000 007a 3a50 6c65 6173 6520 7370 6563  ...z:Please spec
+00001200: 6966 7920 7468 6520 636f 7272 6563 7420  ify the correct 
+00001210: 6d6f 6475 6c65 3a20 2865 2e67 2e20 6d6f  module: (e.g. mo
+00001220: 6465 6c73 2e6d 795f 6d6f 6465 6c29 207a  dels.my_model) z
+00001230: 4250 6163 6b61 6765 2061 6c72 6561 6479  BPackage already
+00001240: 2065 7869 7374 732c 206f 7074 696f 6e73   exists, options
+00001250: 3a20 5b6f 5d76 6572 7772 6974 652c 205b  : [o]verwrite, [
+00001260: 635d 616e 6365 6c2c 205b 725d 656e 616d  c]ancel, [r]enam
+00001270: 653a 20da 016f 7a1c 4465 6c65 7465 6420  e: ..oz.Deleted 
+00001280: 6578 6973 7469 6e67 2070 6163 6b61 6765  existing package
+00001290: 2061 7420 da01 6372 3300 0000 7a0c 446f   at ..cr3...z.Do
+000012a0: 776e 6c6f 6164 696e 6720 2901 da0a 6f75  wnloading )...ou
+000012b0: 7470 7574 5f64 6972 7a06 2f6d 6169 6e2f  tput_dirz./main/
+000012c0: 7a08 2f6d 6173 7465 722f da04 7472 6565  z./master/..tree
+000012d0: 7204 0000 0072 3200 0000 2916 7214 0000  r....r2...).r...
+000012e0: 0072 3600 0000 da07 6861 7368 6c69 62da  .r6.....hashlib.
+000012f0: 0473 6861 31da 0665 6e63 6f64 65da 0968  .sha1..encode..h
+00001300: 6578 6469 6765 7374 7217 0000 0072 1000  exdigestr....r..
+00001310: 0000 7211 0000 0072 1200 0000 da08 6d61  ..r....r......ma
+00001320: 6b65 6469 7273 723a 0000 0072 1500 0000  kedirsr:...r....
+00001330: 720a 0000 00da 0770 726f 6a65 6374 7224  r......projectr$
+00001340: 0000 00da 1f5f 4d6f 6475 6c65 4d61 6e61  ....._ModuleMana
+00001350: 6765 725f 5f69 735f 7661 6c69 645f 6d6f  ger__is_valid_mo
+00001360: 6475 6c65 722b 0000 0072 0300 0000 7205  duler+...r....r.
+00001370: 0000 00da 0772 6570 6c61 6365 7202 0000  .....replacer...
+00001380: 0029 0e72 0c00 0000 722c 0000 0072 1600  .).r....r,...r..
+00001390: 0000 721d 0000 005a 0c62 6173 655f 6769  ..r....Z.base_gi
+000013a0: 745f 7572 6c5a 0875 726c 5f68 6173 68da  t_urlZ.url_hash.
+000013b0: 0b6f 7574 7075 745f 7061 7468 724c 0000  .output_pathrL..
+000013c0: 005a 0b72 6f6f 745f 6d6f 6475 6c65 da0b  .Z.root_module..
+000013d0: 6d6f 6475 6c65 5f6e 616d 65da 0964 6573  module_name..des
+000013e0: 745f 7061 7468 da07 636f 6d6d 616e 6472  t_path..commandr
+000013f0: 2600 0000 5a0a 7372 635f 6d6f 6475 6c65  &...Z.src_module
+00001400: 720d 0000 0072 0d00 0000 720e 0000 005a  r....r....r....Z
+00001410: 115f 5f69 6e73 7461 6c6c 5f70 6163 6b61  .__install_packa
+00001420: 6765 a800 0000 7394 0000 0018 0314 020a  ge....s.........
+00001430: 0204 010c 020e 010e 020e 011a 0208 0206  ................
+00001440: 0110 0106 ff08 0614 0108 0114 0102 0202  ................
+00001450: 0104 ff02 031a 0104 ff08 0306 0110 0106  ................
+00001460: ff02 0402 0104 ff0a 0302 0102 0104 ff0a  ................
+00001470: ff0a 041e 010e 020c 0102 0102 0106 ff04  ................
+00001480: 0408 0208 010a 0102 0108 0204 010a 0202  ................
+00001490: 0102 0104 ff0a 0302 0102 0104 ff0a ff0a  ................
+000014a0: 041e 0102 010c e60e 1c02 0210 0106 010c  ................
+000014b0: 020e 010e 011c 0214 010a 0508 0104 017a  ...............z
+000014c0: 1f4d 6f64 756c 654d 616e 6167 6572 2e5f  .ModuleManager._
+000014d0: 5f69 6e73 7461 6c6c 5f70 6163 6b61 6765  _install_package
+000014e0: 4e29 10da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+000014f0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00001500: 6c6e 616d 655f 5f72 0800 0000 da03 7374  lname__r......st
+00001510: 72da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  r..__annotations
+00001520: 5f5f 720f 0000 0072 0b00 0000 7217 0000  __r....r....r...
+00001530: 0072 1e00 0000 7221 0000 0072 2700 0000  .r....r!...r'...
+00001540: 722b 0000 0072 3e00 0000 7254 0000 0072  r+...r>...rT...r
+00001550: 3800 0000 720d 0000 0072 0d00 0000 720d  8...r....r....r.
+00001560: 0000 0072 0e00 0000 7206 0000 000d 0000  ...r....r.......
+00001570: 0073 1800 0000 0a00 0c01 0802 0805 0808  .s..............
+00001580: 0803 0806 0806 0813 0e1c 0848 0c05 7206  ...........H..r.
+00001590: 0000 0029 0c72 4e00 0000 723c 0000 0072  ...).rN...r<...r
+000015a0: 1000 0000 7228 0000 00da 0673 6875 7469  ....r(.....shuti
+000015b0: 6c72 0200 0000 7203 0000 0072 3700 0000  lr....r....r7...
+000015c0: 5a0c 7574 696c 732e 6769 7464 6972 7205  Z.utils.gitdirr.
+000015d0: 0000 00da 0469 7064 6272 0600 0000 720d  .....ipdbr....r.
+000015e0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+000015f0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001600: 7312 0000 0008 0008 0108 0108 0110 0108  s...............
+00001610: 010c 0308 0112 03                        .......
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Feb 13 20:36:20 2023 UTC, .py size: 12872 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,681 +1,708 @@
-00000000: 6f0d 0d0a 0000 0000 449f ea63 4832 0000  o.......D..cH2..
+00000000: 6f0d 0d0a 0000 0000 e7c6 3164 5e39 0000  o.........1d^9..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6402 6403 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6402 6404 6c07 6d08 5a08 0100 6402  ..d.d.l.m.Z...d.
-00000070: 6405 6c09 6d0a 5a0a 0100 6406 6407 6c0b  d.l.m.Z...d.d.l.
-00000080: 6d0c 5a0c 0100 6402 6408 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
-00000090: 0100 6402 6409 6c0f 6d10 5a10 0100 6400  ..d.d.l.m.Z...d.
-000000a0: 640a 6c11 6d11 5a11 0100 6402 640b 6c12  d.l.m.Z...d.d.l.
-000000b0: 6d13 5a13 0100 6400 640c 6c14 6d15 5a15  m.Z...d.d.l.m.Z.
-000000c0: 0100 6400 6401 6c16 5a16 4700 640d 640e  ..d.d.l.Z.G.d.d.
-000000d0: 8400 640e 8302 5a17 6401 5300 290f e900  ..d...Z.d.S.)...
-000000e0: 0000 004e e901 0000 0029 01da 0d4d 6f64  ...N.....)...Mod
-000000f0: 756c 654d 616e 6167 6572 2901 da14 6765  uleManager)...ge
-00000100: 745f 7265 6c61 7469 7665 5f69 6d70 6f72  t_relative_impor
-00000110: 7473 2901 da12 7061 7273 655f 7572 6c5f  ts)...parse_url_
-00000120: 6672 6f6d 5f67 6974 e903 0000 0029 01da  from_git.....)..
-00000130: 0a4d 6174 6543 6f6e 6669 6729 01da 1052  .MateConfig)...R
-00000140: 656d 6f74 6544 6174 6153 6f75 7263 6529  emoteDataSource)
-00000150: 01da 0f4c 6f63 616c 4461 7461 536f 7572  ...LocalDataSour
-00000160: 6365 2901 da07 7069 7072 6571 7329 01da  ce)...pipreqs)..
-00000170: 0750 6163 6b61 6765 2901 da08 4f70 7469  .Package)...Opti
-00000180: 6f6e 616c 6300 0000 0000 0000 0000 0000  onalc...........
-00000190: 0000 0000 0005 0000 0040 0000 0073 cc00  .........@...s..
-000001a0: 0000 6500 5a01 6400 5a02 642b 6402 6503  ..e.Z.d.Z.d+d.e.
-000001b0: 6403 6504 6604 6404 6405 8405 5a05 6506  d.e.f.d.d...Z.e.
-000001c0: 6406 6507 6602 6407 6408 8404 8301 5a08  d.e.f.d.d.....Z.
-000001d0: 6409 6507 6602 640a 640b 8404 5a09 640c  d.e.f.d.d...Z.d.
-000001e0: 6507 6602 640d 640e 8404 5a0a 642c 6410  e.f.d.d...Z.d,d.
-000001f0: 6507 6602 6411 6412 8405 5a0b 6413 650c  e.f.d.d...Z.d.e.
-00000200: 6507 1900 6602 6414 6415 8404 5a0d 6416  e...f.d.d...Z.d.
-00000210: 6507 6602 6417 6418 8404 5a0e 6419 641a  e.f.d.d...Z.d.d.
-00000220: 8400 5a0f 641b 641c 8400 5a10 641d 641e  ..Z.d.d...Z.d.d.
-00000230: 8400 5a11 641f 6420 8400 5a12 6421 6422  ..Z.d.d ..Z.d!d"
-00000240: 8400 5a13 642c 6423 6507 6602 6424 6425  ..Z.d,d#e.f.d$d%
-00000250: 8405 5a0c 6426 6427 8400 5a14 6428 6515  ..Z.d&d'..Z.d(e.
-00000260: 6602 6429 642a 8404 5a16 640f 5300 292d  f.d)d*..Z.d.S.)-
-00000270: da10 4d6f 6475 6c65 5265 706f 7369 746f  ..ModuleReposito
-00000280: 7279 46da 0663 6f6e 6669 67da 1472 756e  ryF..config..run
-00000290: 5f6c 6f63 616c 5f61 7069 5f73 6572 7665  _local_api_serve
-000002a0: 7263 0300 0000 0000 0000 0000 0000 0300  rc..............
-000002b0: 0000 0200 0000 4300 0000 7326 0000 007c  ......C...s&...|
-000002c0: 017c 005f 0074 017c 0183 017c 005f 0274  .|._.t.|...|._.t
-000002d0: 0383 007c 005f 0474 057c 0183 017c 005f  ...|._.t.|...|._
-000002e0: 0664 0053 00a9 014e 2907 720e 0000 0072  .d.S...N).r....r
-000002f0: 0300 0000 da0f 7061 636b 6167 655f 6d61  ......package_ma
-00000300: 6e61 6765 7272 0800 0000 5a06 7265 6d6f  nagerr....Z.remo
-00000310: 7465 7209 0000 00da 056c 6f63 616c 2903  ter......local).
-00000320: da04 7365 6c66 720e 0000 0072 0f00 0000  ..selfr....r....
-00000330: a900 7214 0000 00fa 4a2f 686f 6d65 2f61  ..r.....J/home/a
-00000340: 6c2f 4769 7468 7562 2f79 6572 6261 6d61  l/Github/yerbama
-00000350: 7465 2f70 6163 6b61 6765 732f 7965 7262  te/packages/yerb
-00000360: 616d 6174 652f 6170 692f 6461 7461 2f6d  amate/api/data/m
-00000370: 6f64 756c 655f 7265 706f 7369 746f 7279  odule_repository
-00000380: 2e70 79da 085f 5f69 6e69 745f 5f16 0000  .py..__init__...
-00000390: 0073 0800 0000 0601 0a01 0801 0e01 7a19  .s............z.
-000003a0: 4d6f 6475 6c65 5265 706f 7369 746f 7279  ModuleRepository
-000003b0: 2e5f 5f69 6e69 745f 5fda 0c70 726f 6a65  .__init__..proje
-000003c0: 6374 5f6e 616d 6563 0100 0000 0000 0000  ct_namec........
-000003d0: 0000 0000 0800 0000 0a00 0000 4300 0000  ............C...
-000003e0: 736e 0100 0074 006a 01a0 027c 00a1 0173  sn...t.j...|...s
-000003f0: 1174 00a0 037c 00a1 0101 0074 00a0 047c  .t...|.....t...|
-00000400: 00a1 0101 006e 0974 0564 0183 0101 0074  .....n.t.d.....t
-00000410: 06a0 0764 02a1 0101 0074 006a 01a0 0864  ...d.....t.j...d
-00000420: 03a1 017d 0174 006a 01a0 027c 01a1 0173  ...}.t.j...|...s
-00000430: 4864 047c 0069 017d 0274 097c 0164 0583  Hd.|.i.}.t.|.d..
-00000440: 028f 107d 0374 0a6a 0b7c 027c 0364 0664  ...}.t.j.|.|.d.d
-00000450: 078d 0301 0057 0064 0004 0004 0083 0301  .....W.d........
-00000460: 006e 0831 0073 4277 0101 0001 0001 0059  .n.1.sBw.......Y
-00000470: 0001 006e 0974 0564 0183 0101 0074 06a0  ...n.t.d.....t..
-00000480: 0764 02a1 0101 0074 006a 01a0 027c 00a1  .d.....t.j...|..
-00000490: 0173 6a74 00a0 037c 00a1 0101 0074 006a  .sjt...|.....t.j
-000004a0: 01a0 087c 0064 08a1 027d 0474 097c 0464  ...|.d...}.t.|.d
-000004b0: 0983 02a0 0ca1 0001 007a 3567 0064 0aa2  .........z5g.d..
-000004c0: 017d 057c 0544 005d 237d 0674 006a 0d74  .}.|.D.]#}.t.j.t
-000004d0: 006a 01a0 087c 007c 06a1 0264 0b64 0c8d  .j...|.|...d.d..
-000004e0: 0201 0074 006a 01a0 087c 007c 0664 08a1  ...t.j...|.|.d..
-000004f0: 037d 0474 006a 01a0 027c 04a1 0173 9474  .}.t.j...|...s.t
-00000500: 097c 0464 0983 02a0 0ca1 0001 0071 7174  .|.d.........qqt
-00000510: 0564 0da0 0e7c 007c 00a1 0283 0101 0057  .d...|.|.......W
-00000520: 0064 0053 0004 0074 0f79 b601 007d 0701  .d.S...t.y...}..
-00000530: 007a 0b74 057c 0783 0101 0057 0059 0064  .z.t.|.....W.Y.d
-00000540: 007d 077e 0764 0053 0064 007d 077e 0777  .}.~.d.S.d.}.~.w
-00000550: 0177 0029 0e4e 7a16 5072 6f6a 6563 7420  .w.).Nz.Project 
-00000560: 616c 7265 6164 7920 6578 6973 7473 7202  already existsr.
-00000570: 0000 007a 096d 6174 652e 6a73 6f6e da07  ...z.mate.json..
-00000580: 7072 6f6a 6563 74da 0177 e904 0000 00a9  project..w......
-00000590: 01da 0669 6e64 656e 74fa 0b5f 5f69 6e69  ...indent..__ini
-000005a0: 745f 5f2e 7079 da01 6129 04da 0b65 7870  t__.py..a)...exp
-000005b0: 6572 696d 656e 7473 da06 6d6f 6465 6c73  eriments..models
-000005c0: da04 6461 7461 da08 7472 6169 6e65 7273  ..data..trainers
-000005d0: 5429 01da 0865 7869 7374 5f6f 6b7a 3b50  T)...exist_okz;P
-000005e0: 726f 6a65 6374 207b 7d20 6372 6561 7465  roject {} create
-000005f0: 642c 2072 756e 2060 6364 207b 7d60 2074  d, run `cd {}` t
-00000600: 6f20 656e 7465 7220 7468 6520 7072 6f6a  o enter the proj
-00000610: 6563 7420 666f 6c64 6572 2910 da02 6f73  ect folder)...os
-00000620: da04 7061 7468 da06 6578 6973 7473 da05  ..path..exists..
-00000630: 6d6b 6469 72da 0563 6864 6972 da05 7072  mkdir..chdir..pr
-00000640: 696e 74da 0373 7973 da04 6578 6974 da04  int..sys..exit..
-00000650: 6a6f 696e da04 6f70 656e da04 6a73 6f6e  join..open..json
-00000660: da04 6475 6d70 da05 636c 6f73 65da 086d  ..dump..close..m
-00000670: 616b 6564 6972 73da 0666 6f72 6d61 74da  akedirs..format.
-00000680: 0945 7863 6570 7469 6f6e 2908 7217 0000  .Exception).r...
-00000690: 005a 096d 6174 655f 6a73 6f6e 5a03 6469  .Z.mate_jsonZ.di
-000006a0: 63da 0166 5a0a 696e 6974 5f5f 6669 6c65  c..fZ.init__file
-000006b0: 5a07 666f 6c64 6572 73da 0666 6f6c 6465  Z.folders..folde
-000006c0: 72da 0165 7214 0000 0072 1400 0000 7215  r..er....r....r.
-000006d0: 0000 00da 0c69 6e69 745f 7072 6f6a 6563  .....init_projec
-000006e0: 741d 0000 0073 4800 0000 0c03 0a01 0c01  t....sH.........
-000006f0: 0802 0a01 0c02 0c01 0402 04ff 0c05 1201  ................
-00000700: 1cff 0280 0803 0a01 0c02 0a01 0e01 0e01  ................
-00000710: 0201 0801 0801 1801 1001 0c01 0e01 0280  ................
-00000720: 0201 0401 0401 02ff 0aff 0e06 1601 0880  ................
-00000730: 02ff 7a1d 4d6f 6475 6c65 5265 706f 7369  ..z.ModuleReposi
-00000740: 746f 7279 2e69 6e69 745f 7072 6f6a 6563  tory.init_projec
-00000750: 74da 0375 726c 6302 0000 0000 0000 0000  t..urlc.........
-00000760: 0000 0004 0000 0004 0000 004f 0000 0073  ...........O...s
-00000770: 1e00 0000 7c00 6a00 6a01 7c01 6701 7c02  ....|.j.j.|.g.|.
-00000780: a201 5200 6900 7c03 a401 8e01 0100 6400  ..R.i.|.......d.
-00000790: 5300 7210 0000 0029 0272 1100 0000 da0f  S.r....).r......
-000007a0: 696e 7374 616c 6c5f 7061 636b 6167 6529  install_package)
-000007b0: 0472 1300 0000 7238 0000 00da 0461 7267  .r....r8.....arg
-000007c0: 73da 066b 7761 7267 7372 1400 0000 7214  s..kwargsr....r.
-000007d0: 0000 0072 1500 0000 da0b 696e 7374 616c  ...r......instal
-000007e0: 6c5f 7572 6c48 0000 0073 0200 0000 1e02  l_urlH...s......
-000007f0: 7a1c 4d6f 6475 6c65 5265 706f 7369 746f  z.ModuleReposito
-00000800: 7279 2e69 6e73 7461 6c6c 5f75 726c da07  ry.install_url..
-00000810: 636f 6d6d 616e 6463 0200 0000 0000 0000  commandc........
-00000820: 0000 0000 0300 0000 0300 0000 4700 0000  ............G...
-00000830: 7332 0000 007c 0164 016b 0272 0a7c 00a0  s2...|.d.k.r.|..
-00000840: 00a1 0001 0064 0053 007c 0164 0276 0072  .....d.S.|.d.v.r
-00000850: 177c 00a0 017c 006a 026a 03a1 0101 0064  .|...|.j.j.....d
-00000860: 0053 0064 0053 0029 034e da06 6578 706f  .S.d.S.).N..expo
-00000870: 7274 2903 da04 696e 6974 da03 6669 78da  rt)...init..fix.
-00000880: 0169 2904 da19 5f4d 6f64 756c 6552 6570  .i)..._ModuleRep
-00000890: 6f73 6974 6f72 795f 5f65 7870 6f72 74da  ository__export.
-000008a0: 125f 5f67 656e 6572 6174 655f 5f69 6e69  .__generate__ini
-000008b0: 745f 5f72 0e00 0000 7218 0000 0029 0372  t__r....r....).r
-000008c0: 1300 0000 723d 0000 0072 3a00 0000 7214  ....r=...r:...r.
-000008d0: 0000 0072 1400 0000 7215 0000 00da 0461  ...r....r......a
-000008e0: 7574 6f4c 0000 0073 0a00 0000 0801 0c01  utoL...s........
-000008f0: 0801 1201 04ff 7a15 4d6f 6475 6c65 5265  ......z.ModuleRe
-00000900: 706f 7369 746f 7279 2e61 7574 6f4e da04  pository.autoN..
-00000910: 726f 6f74 6302 0000 0000 0000 0000 0000  rootc...........
-00000920: 0006 0000 0009 0000 0043 0000 0073 0201  .........C...s..
-00000930: 0000 7400 6a01 a002 7c01 6401 a102 7d02  ..t.j...|.d...}.
-00000940: 7400 6a01 a003 7c02 a101 732e 7404 7c02  t.j...|...s.t.|.
-00000950: 6402 8302 8f0d 7d03 7c03 a005 6403 a101  d.....}.|...d...
-00000960: 0100 5700 6400 0400 0400 8303 0100 6e08  ..W.d.........n.
-00000970: 3100 7322 7701 0100 0100 0100 5900 0100  1.s"w.......Y...
-00000980: 7406 6404 7c02 9b00 9d02 8301 0100 7400  t.d.|.........t.
-00000990: a007 7c01 a101 4400 5d4b 7d04 7400 6a01  ..|...D.]K}.t.j.
-000009a0: a002 7c01 7c04 a102 7d05 7400 6a01 a008  ..|.|...}.t.j...
-000009b0: 7c05 a101 724a 7c04 6405 6b02 734a 6406  |...rJ|.d.k.sJd.
-000009c0: 7c04 7600 724b 7133 7400 6a01 a002 7c05  |.v.rKq3t.j...|.
-000009d0: 6401 a102 7d02 7400 6a01 a003 7c02 a101  d...}.t.j...|...
-000009e0: 7379 7404 7c02 6402 8302 8f0d 7d03 7c03  syt.|.d.....}.|.
-000009f0: a005 6403 a101 0100 5700 6400 0400 0400  ..d.....W.d.....
-00000a00: 8303 0100 6e08 3100 736d 7701 0100 0100  ....n.1.smw.....
-00000a10: 0100 5900 0100 7406 6404 7c02 9b00 9d02  ..Y...t.d.|.....
-00000a20: 8301 0100 7c00 a009 7c05 a101 0100 7133  ....|...|.....q3
-00000a30: 6400 5300 2907 4e72 1d00 0000 7219 0000  d.S.).Nr....r...
-00000a40: 00da 007a 0843 7265 6174 6564 20da 0b5f  ...z.Created .._
-00000a50: 5f70 7963 6163 6865 5f5f da01 2e29 0a72  _pycache__...).r
-00000a60: 2400 0000 7225 0000 0072 2c00 0000 7226  $...r%...r,...r&
-00000a70: 0000 0072 2d00 0000 da05 7772 6974 6572  ...r-.....writer
-00000a80: 2900 0000 da07 6c69 7374 6469 72da 0569  ).....listdir..i
-00000a90: 7364 6972 7243 0000 0029 0672 1300 0000  sdirrC...).r....
-00000aa0: 7245 0000 005a 0869 6e69 745f 5f70 7972  rE...Z.init__pyr
-00000ab0: 3400 0000 7235 0000 0072 2500 0000 7214  4...r5...r%...r.
-00000ac0: 0000 0072 1400 0000 7215 0000 0072 4300  ...r....r....rC.
-00000ad0: 0000 5200 0000 7324 0000 000e 010c 010c  ..R...s$........
-00000ae0: 010c 011c ff0e 020e 020e 011c 0102 010e  ................
-00000af0: 010c 010c 010c 011c ff0e 020c 0104 f77a  ...............z
-00000b00: 234d 6f64 756c 6552 6570 6f73 6974 6f72  #ModuleRepositor
-00000b10: 792e 5f5f 6765 6e65 7261 7465 5f5f 696e  y.__generate__in
-00000b20: 6974 5f5f da04 7265 7173 6302 0000 0000  it__..reqsc.....
-00000b30: 0000 0000 0000 0005 0000 0005 0000 0043  ...............C
-00000b40: 0000 0073 4a00 0000 6401 6402 6403 9c02  ...sJ...d.d.d...
-00000b50: 7d02 7400 8300 7d03 7c01 4400 5d18 7d04  }.t...}.|.D.].}.
-00000b60: 6404 7c04 7600 7217 7c03 a001 7c02 6404  d.|.v.r.|...|.d.
-00000b70: 1900 a101 0100 6405 7c04 7600 7222 7c03  ......d.|.v.r"|.
-00000b80: a001 7c02 6405 1900 a101 0100 710a 7c03  ..|.d.......q.|.
-00000b90: 5300 2906 4e7a 3268 7474 7073 3a2f 2f64  S.).Nz2https://d
-00000ba0: 6f77 6e6c 6f61 642e 7079 746f 7263 682e  ownload.pytorch.
-00000bb0: 6f72 672f 7768 6c2f 746f 7263 685f 7374  org/whl/torch_st
-00000bc0: 6162 6c65 2e68 746d 6c7a 3d68 7474 7073  able.htmlz=https
-00000bd0: 3a2f 2f73 746f 7261 6765 2e67 6f6f 676c  ://storage.googl
-00000be0: 6561 7069 732e 636f 6d2f 6a61 782d 7265  eapis.com/jax-re
-00000bf0: 6c65 6173 6573 2f6a 6178 5f72 656c 6561  leases/jax_relea
-00000c00: 7365 732e 6874 6d6c 2902 da05 746f 7263  ses.html)...torc
-00000c10: 68da 036a 6178 724d 0000 0072 4e00 0000  h..jaxrM...rN...
-00000c20: 2902 da03 7365 74da 0361 6464 2905 7213  )...set..add).r.
-00000c30: 0000 0072 4c00 0000 da04 7572 6c73 da07  ...rL.....urls..
-00000c40: 696e 6465 7865 73da 0372 6571 7214 0000  indexes..reqr...
-00000c50: 0072 1400 0000 7215 0000 005a 125f 5f70  .r....r....Z.__p
-00000c60: 6172 7365 5f69 6e64 6578 5f75 726c 7364  arse_index_urlsd
-00000c70: 0000 0073 1600 0000 0202 0201 06fe 0604  ...s............
-00000c80: 0801 0801 0e01 0801 0e01 0280 0402 7a23  ..............z#
-00000c90: 4d6f 6475 6c65 5265 706f 7369 746f 7279  ModuleRepository
-00000ca0: 2e5f 5f70 6172 7365 5f69 6e64 6578 5f75  .__parse_index_u
-00000cb0: 726c 7372 2500 0000 6302 0000 0000 0000  rlsr%...c.......
-00000cc0: 0000 0000 0008 0000 0008 0000 0003 0000  ................
-00000cd0: 0073 4601 0000 7400 7401 6a02 a003 7c01  .sF...t.t.j...|.
-00000ce0: a101 6401 8302 8f0c 7d02 7c02 a004 a100  ..d.....}.|.....
-00000cf0: 7d03 5700 6400 0400 0400 8303 0100 6e08  }.W.d.........n.
-00000d00: 3100 7318 7701 0100 0100 0100 5900 0100  1.s.w.......Y...
-00000d10: 7405 7c03 8301 7d04 6402 6403 8400 7c03  t.|...}.d.d...|.
-00000d20: 4400 8301 7d03 7406 a007 6404 a101 8900  D...}.t...d.....
-00000d30: 8700 6601 6405 6403 8408 7c03 4400 8301  ..f.d.d...|.D...
-00000d40: 7d03 7c00 a008 7c03 a101 7d05 7405 7c05  }.|...|...}.t.|.
-00000d50: 8301 6406 6b04 7275 7400 7401 6a02 a003  ..d.k.rut.t.j...
-00000d60: 7c01 a101 6407 8302 8f21 7d02 7c05 4400  |...d....!}.|.D.
-00000d70: 5d0b 7d06 7c02 a009 6408 7c06 9b00 6409  ].}.|...d.|...d.
-00000d80: 9d03 a101 0100 714d 7c03 4400 5d07 7d07  ......qM|.D.].}.
-00000d90: 7c02 a009 7c07 a101 0100 715b 5700 6400  |...|.....q[W.d.
-00000da0: 0400 0400 8303 0100 6400 5300 3100 736e  ........d.S.1.sn
-00000db0: 7701 0100 0100 0100 5900 0100 6400 5300  w.......Y...d.S.
-00000dc0: 7c04 7405 7c03 8301 6b03 72a1 7400 7401  |.t.|...k.r.t.t.
-00000dd0: 6a02 a003 7c01 a101 6407 8302 8f13 7d02  j...|...d.....}.
-00000de0: 7c03 4400 5d07 7d07 7c02 a009 7c07 a101  |.D.].}.|...|...
-00000df0: 0100 7187 5700 6400 0400 0400 8303 0100  ..q.W.d.........
-00000e00: 6400 5300 3100 739a 7701 0100 0100 0100  d.S.1.s.w.......
-00000e10: 5900 0100 6400 5300 6400 5300 290a 4eda  Y...d.S.d.S.).N.
-00000e20: 0172 6301 0000 0000 0000 0000 0000 0002  .rc.............
-00000e30: 0000 0004 0000 0053 0000 0073 2800 0000  .......S...s(...
-00000e40: 6700 7c00 5d10 7d01 6400 7c01 7601 7212  g.|.].}.d.|.v.r.
-00000e50: 6401 7c01 7601 7212 6402 7c01 7601 7202  d.|.v.r.d.|.v.r.
-00000e60: 7c01 9102 7102 5300 2903 7a0a 2e65 6767  |...q.S.).z..egg
-00000e70: 3e3d 696e 666f 7a0a 2e65 6767 3d3d 696e  >=infoz..egg==in
-00000e80: 666f 7a0a 2e65 6767 7e3d 696e 666f 7214  foz..egg~=infor.
-00000e90: 0000 00a9 02da 022e 30da 046c 696e 6572  ........0..liner
-00000ea0: 1400 0000 7214 0000 0072 1500 0000 da0a  ....r....r......
-00000eb0: 3c6c 6973 7463 6f6d 703e 7600 0000 730e  <listcomp>v...s.
-00000ec0: 0000 0006 0002 0208 0108 0108 0102 fc06  ................
-00000ed0: 047a 444d 6f64 756c 6552 6570 6f73 6974  .zDModuleReposit
-00000ee0: 6f72 792e 5f5f 6164 645f 696e 6465 785f  ory.__add_index_
-00000ef0: 7572 6c5f 746f 5f72 6571 7569 7265 6d65  url_to_requireme
-00000f00: 6e74 732e 3c6c 6f63 616c 733e 2e3c 6c69  nts.<locals>.<li
-00000f10: 7374 636f 6d70 3e7a 075c 2b63 755c 642b  stcomp>z.\+cu\d+
-00000f20: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000f30: 0006 0000 0013 0000 0073 1800 0000 6700  .........s....g.
-00000f40: 7c00 5d08 7d01 8800 a000 6400 7c01 a102  |.].}.....d.|...
-00000f50: 9102 7102 5300 2901 7246 0000 0029 01da  ..q.S.).rF...)..
-00000f60: 0373 7562 7255 0000 00a9 01da 0572 6567  .subrU.......reg
-00000f70: 6578 7214 0000 0072 1500 0000 7258 0000  exr....r....rX..
-00000f80: 0081 0000 00f3 0200 0000 1800 7201 0000  ............r...
-00000f90: 0072 1900 0000 7a12 2d2d 6578 7472 612d  .r....z.--extra-
-00000fa0: 696e 6465 782d 7572 6c20 da01 0a29 0a72  index-url ...).r
-00000fb0: 2d00 0000 7224 0000 0072 2500 0000 722c  -...r$...r%...r,
-00000fc0: 0000 00da 0972 6561 646c 696e 6573 da03  .....readlines..
-00000fd0: 6c65 6eda 0272 65da 0763 6f6d 7069 6c65  len..re..compile
-00000fe0: da23 5f4d 6f64 756c 6552 6570 6f73 6974  .#_ModuleReposit
-00000ff0: 6f72 795f 5f70 6172 7365 5f69 6e64 6578  ory__parse_index
-00001000: 5f75 726c 7372 4900 0000 2908 7213 0000  _urlsrI...).r...
-00001010: 0072 2500 0000 7234 0000 00da 056c 696e  .r%...r4.....lin
-00001020: 6573 5a09 6c69 6e65 636f 756e 7472 5100  esZ.linecountrQ.
-00001030: 0000 7238 0000 0072 5700 0000 7214 0000  ..r8...rW...r...
-00001040: 0072 5a00 0000 7215 0000 005a 1f5f 5f61  .rZ...r....Z.__a
-00001050: 6464 5f69 6e64 6578 5f75 726c 5f74 6f5f  dd_index_url_to_
-00001060: 7265 7175 6972 656d 656e 7473 7200 0000  requirementsr...
-00001070: 7332 0000 0014 010a 011c ff08 0206 0102  s2..............
-00001080: 0206 fe0a 0a12 010a 020c 0114 0108 0114  ................
-00001090: 0108 010c 0102 ff22 fd0c 0514 0108 010c  ......."........
-000010a0: 0102 ff22 ff04 ff7a 304d 6f64 756c 6552  ..."...z0ModuleR
-000010b0: 6570 6f73 6974 6f72 792e 5f5f 6164 645f  epository.__add_
-000010c0: 696e 6465 785f 7572 6c5f 746f 5f72 6571  index_url_to_req
-000010d0: 7569 7265 6d65 6e74 7363 0200 0000 0000  uirementsc......
-000010e0: 0000 0000 0000 0500 0000 0600 0000 4300  ..............C.
-000010f0: 0000 738a 0000 0074 00a0 017c 01a1 0144  ..s....t...|...D
-00001100: 005d 3d7d 027c 02a0 0264 01a1 0173 117c  .]=}.|...d...s.|
-00001110: 02a0 0264 02a1 0172 1271 0574 006a 03a0  ...d...r.q.t.j..
-00001120: 047c 017c 02a1 027d 0374 006a 03a0 057c  .|.|...}.t.j...|
-00001130: 03a1 0172 4274 006a 03a0 047c 017c 0264  ...rBt.j...|.|.d
-00001140: 03a1 037d 0474 006a 03a0 067c 04a1 0173  ...}.t.j...|...s
-00001150: 2e71 057c 0264 0476 0072 387c 006a 076a  .q.|.d.v.r8|.j.j
-00001160: 087c 0176 0073 3d7c 00a0 097c 03a1 0101  .|.v.s=|...|....
-00001170: 007c 00a0 0a7c 03a1 0101 0071 0564 0053  .|...|.....q.d.S
-00001180: 0029 054e 7248 0000 00da 025f 5f72 1d00  .).NrH.....__r..
-00001190: 0000 2904 7222 0000 0072 1f00 0000 7220  ..).r"...r....r 
-000011a0: 0000 0072 2100 0000 290b 7224 0000 0072  ...r!...).r$...r
-000011b0: 4a00 0000 da0a 7374 6172 7473 7769 7468  J.....startswith
-000011c0: 7225 0000 0072 2c00 0000 724b 0000 0072  r%...r,...rK...r
-000011d0: 2600 0000 720e 0000 0072 1800 0000 da2c  &...r....r.....,
-000011e0: 5f4d 6f64 756c 6552 6570 6f73 6974 6f72  _ModuleRepositor
-000011f0: 795f 5f67 656e 6572 6174 655f 7069 705f  y__generate_pip_
-00001200: 7265 7175 6972 656d 656e 7473 da29 5f4d  requirements.)_M
-00001210: 6f64 756c 6552 6570 6f73 6974 6f72 795f  oduleRepository_
-00001220: 5f67 656e 6572 6174 655f 6465 7073 5f69  _generate_deps_i
-00001230: 6e5f 6465 7074 68a9 0572 1300 0000 5a09  n_depth..r....Z.
-00001240: 726f 6f74 5f70 6174 68da 0364 6972 7225  root_path..dirr%
-00001250: 0000 005a 0a69 6e69 745f 5f70 6174 6872  ...Z.init__pathr
-00001260: 1400 0000 7214 0000 0072 1500 0000 5a18  ....r....r....Z.
-00001270: 5f5f 6765 6e65 7261 7465 5f64 6570 735f  __generate_deps_
-00001280: 696e 5f64 6570 7468 8f00 0000 731c 0000  in_depth....s...
-00001290: 000e 0414 0102 010e 010c 0110 020c 0102  ................
-000012a0: 0108 030c 010a 020a 0202 8004 f07a 294d  .............z)M
-000012b0: 6f64 756c 6552 6570 6f73 6974 6f72 792e  oduleRepository.
-000012c0: 5f5f 6765 6e65 7261 7465 5f64 6570 735f  __generate_deps_
-000012d0: 696e 5f64 6570 7468 6301 0000 0000 0000  in_depthc.......
-000012e0: 0000 0000 000b 0000 000b 0000 0003 0000  ................
-000012f0: 0073 a602 0000 7c00 a000 a100 0100 7c00  .s....|.......|.
-00001300: a001 a100 7d01 6700 7d02 7c01 a002 a100  ....}.g.}.|.....
-00001310: 4400 5d2b 5c02 8900 7d03 7403 7c03 8301  D.]+\...}.t.|...
-00001320: 7401 7500 7225 7c02 a004 8700 6601 6401  t.u.r%|.....f.d.
-00001330: 6402 8408 7c03 4400 8301 a101 0100 710e  d...|.D.......q.
-00001340: 7403 7c03 8301 7405 7500 7239 7c02 a004  t.|...t.u.r9|...
-00001350: 8700 6601 6403 6402 8408 7c03 a006 a100  ..f.d.d...|.....
-00001360: 4400 8301 a101 0100 710e 6404 6402 8400  D.......q.d.d...
-00001370: 7c02 4400 8301 7d02 7407 8300 7d04 7c04  |.D...}.t...}.|.
-00001380: a008 6405 a101 6406 1900 7d05 7c04 a008  ..d...d...}.|...
-00001390: 6405 a101 6407 1900 7d06 7c02 4400 5d47  d...d...}.|.D.]G
-000013a0: 7d07 7c04 9b00 7c00 6a09 6a0a 9b00 6405  }.|...|.j.j...d.
-000013b0: 7c07 6408 1900 9b00 6405 7c07 6409 1900  |.d.....d.|.d...
-000013c0: 9b00 9d06 7c07 640a 3c00 7c05 9b00 6405  ....|.d.<.|...d.
-000013d0: 7c06 9b00 6405 7c00 6a09 6a0a 9b00 6405  |...d.|.j.j...d.
-000013e0: 7c07 6408 1900 9b00 6405 7c07 6409 1900  |.d.....d.|.d...
-000013f0: 9b00 9d09 7c07 640b 3c00 7c06 7c00 6a09  ....|.d.<.|.|.j.
-00001400: 6a0a 6b02 729b 7c05 9b00 6405 7c06 9b00  j.k.r.|...d.|...
-00001410: 6405 7c07 6408 1900 9b00 6405 7c07 6409  d.|.d.....d.|.d.
-00001420: 1900 9b00 9d07 7c07 640b 3c00 7154 7c02  ......|.d.<.qT|.
-00001430: 4400 5d89 7d07 740b 6a0c a00d 7c00 6a09  D.].}.t.j...|.j.
-00001440: 6a0a 7c07 6408 1900 7c07 6409 1900 640c  j.|.d...|.d...d.
-00001450: a104 7d08 740b 6a0c a00d 7c00 6a09 6a0a  ..}.t.j...|.j.j.
-00001460: 7c07 6408 1900 7c07 6409 1900 640d a104  |.d...|.d...d...
-00001470: 7d09 740b 6a0c a00e 7c08 a101 72df 740f  }.t.j...|...r.t.
-00001480: 7c08 640e 8302 8f0e 7d0a 7c0a a010 a100  |.d.....}.|.....
-00001490: 7c07 640f 3c00 5700 6400 0400 0400 8303  |.d.<.W.d.......
-000014a0: 0100 6e08 3100 73da 7701 0100 0100 0100  ..n.1.s.w.......
-000014b0: 5900 0100 740b 6a0c a00e 7c09 a101 9001  Y...t.j...|.....
-000014c0: 7217 740f 7c09 640e 8302 8f23 7d0a 640f  r.t.|.d....#}.d.
-000014d0: 7c07 7600 72fe 7c07 640f 0500 1900 7411  |.v.r.|.d.....t.
-000014e0: a012 7c0a a101 640f 1900 3700 0300 3c00  ..|...d...7...<.
-000014f0: 6e09 7411 a012 7c0a a101 640f 1900 7c07  n.t...|...d...|.
-00001500: 640f 3c00 5700 6400 0400 0400 8303 0100  d.<.W.d.........
-00001510: 6e09 3100 9001 7312 7701 0100 0100 0100  n.1...s.w.......
-00001520: 5900 0100 640f 7c07 7600 9001 7227 6410  Y...d.|.v...r'd.
-00001530: 6402 8400 7c07 640f 1900 4400 8301 7c07  d...|.d...D...|.
-00001540: 640f 3c00 719e 7413 6a13 7c02 6411 6412  d.<.q.t.j.|.d.d.
-00001550: 6413 6414 6415 8d05 7d02 740f 6416 6417  d.d.d...}.t.d.d.
-00001560: 8302 8f0d 7d0a 7c0a a014 7c02 a101 0100  ....}.|...|.....
-00001570: 5700 6400 0400 0400 8303 0100 6e09 3100  W.d.........n.1.
-00001580: 9001 7348 7701 0100 0100 0100 5900 0100  ..sHw.......Y...
-00001590: 7415 6418 8301 0100 6400 5300 2919 4e63  t.d.....d.S.).Nc
-000015a0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000015b0: 0500 0000 1300 0000 f316 0000 0067 007c  .............g.|
-000015c0: 005d 077d 0188 007c 0164 009c 0291 0271  .].}...|.d.....q
-000015d0: 0253 00a9 0129 02da 0474 7970 65da 046e  .S...)...type..n
-000015e0: 616d 6572 1400 0000 a902 7256 0000 0072  amer......rV...r
-000015f0: 6d00 0000 a901 da03 6b65 7972 1400 0000  m.......keyr....
-00001600: 7215 0000 0072 5800 0000 ae00 0000 f302  r....rX.........
-00001610: 0000 0016 007a 2d4d 6f64 756c 6552 6570  .....z-ModuleRep
-00001620: 6f73 6974 6f72 792e 5f5f 6578 706f 7274  ository.__export
-00001630: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00001640: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
-00001650: 0002 0000 0005 0000 0013 0000 0072 6a00  .............rj.
-00001660: 0000 726b 0000 0072 1400 0000 726e 0000  ..rk...r....rn..
-00001670: 0072 6f00 0000 7214 0000 0072 1500 0000  .ro...r....r....
-00001680: 7258 0000 00b0 0000 0072 7100 0000 6301  rX.......rq...c.
-00001690: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-000016a0: 0000 0053 0000 00f3 1a00 0000 6700 7c00  ...S........g.|.
-000016b0: 5d09 7d01 7c01 4400 5d04 7d02 7c02 9103  ].}.|.D.].}.|...
-000016c0: 7106 7102 5300 7214 0000 0072 1400 0000  q.q.S.r....r....
-000016d0: a903 7256 0000 005a 0773 7562 6c69 7374  ..rV...Z.sublist
-000016e0: da04 6974 656d 7214 0000 0072 1400 0000  ..itemr....r....
-000016f0: 7215 0000 0072 5800 0000 b400 0000 f302  r....rX.........
-00001700: 0000 001a 00fa 012f 7206 0000 0072 1a00  ......./r....r..
-00001710: 0000 726c 0000 0072 6d00 0000 7238 0000  ..rl...rm...r8..
-00001720: 005a 0973 686f 7274 5f75 726c fa10 7265  .Z.short_url..re
-00001730: 7175 6972 656d 656e 7473 2e74 7874 fa11  quirements.txt..
-00001740: 6465 7065 6e64 656e 6369 6573 2e6a 736f  dependencies.jso
-00001750: 6e72 5400 0000 da0c 6465 7065 6e64 656e  nrT.....dependen
-00001760: 6369 6573 6301 0000 0000 0000 0000 0000  ciesc...........
-00001770: 0002 0000 0006 0000 0053 0000 00f3 1800  .........S......
-00001780: 0000 6700 7c00 5d08 7d01 7c01 a000 6400  ..g.|.].}.|...d.
-00001790: 6401 a102 9102 7102 5300 2902 725d 0000  d.....q.S.).r]..
-000017a0: 0072 4600 0000 a901 da07 7265 706c 6163  .rF.......replac
-000017b0: 6529 0272 5600 0000 da03 6465 7072 1400  e).rV.....depr..
-000017c0: 0000 7214 0000 0072 1500 0000 7258 0000  ..r....r....rX..
-000017d0: 00e1 0000 0073 0600 0000 0600 0c01 06ff  .....s..........
-000017e0: da04 6b65 7973 5a06 6769 7468 7562 da06  ..keysZ.github..
-000017f0: 616c 7761 7973 5429 04da 0768 6561 6465  alwaysT)...heade
-00001800: 7273 5a08 7461 626c 6566 6d74 5a09 7368  rsZ.tablefmtZ.sh
-00001810: 6f77 696e 6465 785a 1064 6973 6162 6c65  owindexZ.disable
-00001820: 5f6e 756d 7061 7273 657a 0965 7870 6f72  _numparsez.expor
-00001830: 742e 6d64 7219 0000 007a 1545 7870 6f72  t.mdr....z.Expor
-00001840: 7465 6420 746f 2065 7870 6f72 742e 6d64  ted to export.md
-00001850: 2916 da28 5f4d 6f64 756c 6552 6570 6f73  )..(_ModuleRepos
-00001860: 6974 6f72 795f 5f67 656e 6572 6174 655f  itory__generate_
-00001870: 7375 625f 7069 705f 7265 7173 da04 6c69  sub_pip_reqs..li
-00001880: 7374 da05 6974 656d 7372 6c00 0000 da06  st..itemsrl.....
-00001890: 6170 7065 6e64 da04 6469 6374 727e 0000  append..dictr~..
-000018a0: 0072 0500 0000 da05 7370 6c69 7472 0e00  .r......splitr..
-000018b0: 0000 7218 0000 0072 2400 0000 7225 0000  ..r....r$...r%..
-000018c0: 0072 2c00 0000 7226 0000 0072 2d00 0000  .r,...r&...r-...
-000018d0: 725e 0000 0072 2e00 0000 da04 6c6f 6164  r^...r......load
-000018e0: da08 7461 6275 6c61 7465 7249 0000 0072  ..tabulaterI...r
-000018f0: 2900 0000 290b 7213 0000 00da 076d 6f64  )...).r......mod
-00001900: 756c 6573 da05 7461 626c 65da 0576 616c  ules..table..val
-00001910: 7565 5a08 6261 7365 5f75 726c 5a09 7573  ueZ.base_urlZ.us
-00001920: 6572 5f6e 616d 655a 0972 6570 6f5f 6e61  er_nameZ.repo_na
-00001930: 6d65 7274 0000 0072 2500 0000 5a08 6465  mert...r%...Z.de
-00001940: 705f 7061 7468 7234 0000 0072 1400 0000  p_pathr4...r....
-00001950: 726f 0000 0072 1500 0000 5a08 5f5f 6578  ro...r....Z.__ex
-00001960: 706f 7274 a500 0000 737c 0000 0008 0108  port....s|......
-00001970: 0204 0210 020c 011a 010c 011c 0102 800e  ................
-00001980: 0406 040e 010e 0108 0122 0402 fe02 0102  ........."......
-00001990: ff2a 0502 fe02 0102 ff0c 0520 0502 fe02  .*......... ....
-000019a0: 0102 ff02 8008 0506 0114 0104 ff06 0314  ................
-000019b0: 0104 ff0c 040c 010e 011c ff0e 020c 0108  ................
-000019c0: 011c 0112 0202 801e fc0a 0706 0106 010a  ................
-000019d0: ff02 8004 0402 0102 0102 0102 0102 0106  ................
-000019e0: fb0c 090c 011e ff0c 037a 194d 6f64 756c  .........z.Modul
-000019f0: 6552 6570 6f73 6974 6f72 792e 5f5f 6578  eRepository.__ex
-00001a00: 706f 7274 6301 0000 0000 0000 0000 0000  portc...........
-00001a10: 0005 0000 0006 0000 0043 0000 0073 8a00  .........C...s..
-00001a20: 0000 7c00 6a00 6a01 7d01 7c00 a002 7c01  ..|.j.j.}.|...|.
-00001a30: a101 0100 7403 a004 6401 a101 4400 5d34  ....t...d...D.]4
-00001a40: 7d02 7c02 a005 6401 a101 7320 7c02 a005  }.|...d...s |...
-00001a50: 6402 a101 7320 7c02 7c00 6a00 6a01 6b02  d...s |.|.j.j.k.
-00001a60: 7221 710e 7403 6a06 a007 6401 7c02 a102  r!q.t.j...d.|...
-00001a70: 7d03 7403 6a06 a008 7c03 a101 7242 7403  }.t.j...|...rBt.
-00001a80: 6a06 a007 6401 7c02 6403 a103 7d04 7403  j...d.|.d...}.t.
-00001a90: 6a06 a009 7c04 a101 733d 710e 7c00 a00a  j...|...s=q.|...
-00001aa0: 7c03 a101 0100 710e 6400 5300 2904 4e72  |.....q.d.S.).Nr
-00001ab0: 4800 0000 7264 0000 0072 1d00 0000 290b  H...rd...r....).
-00001ac0: 720e 0000 0072 1800 0000 7267 0000 0072  r....r....rg...r
-00001ad0: 2400 0000 724a 0000 0072 6500 0000 7225  $...rJ...re...r%
-00001ae0: 0000 0072 2c00 0000 724b 0000 0072 2600  ...r,...rK...r&.
-00001af0: 0000 7266 0000 0072 6800 0000 7214 0000  ..rf...rh...r...
-00001b00: 0072 1400 0000 7215 0000 005a 175f 5f67  .r....r....Z.__g
-00001b10: 656e 6572 6174 655f 7375 625f 7069 705f  enerate_sub_pip_
-00001b20: 7265 7173 f300 0000 7322 0000 0008 020a  reqs....s"......
-00001b30: 010e 0208 0202 ff08 0202 fe0c 0302 020e  ................
-00001b40: 010c 0110 020c 0102 010a 0102 8004 f37a  ...............z
-00001b50: 284d 6f64 756c 6552 6570 6f73 6974 6f72  (ModuleRepositor
-00001b60: 792e 5f5f 6765 6e65 7261 7465 5f73 7562  y.__generate_sub
-00001b70: 5f70 6970 5f72 6571 7363 0200 0000 0000  _pip_reqsc......
-00001b80: 0000 0000 0000 0e00 0000 0a00 0000 0300  ................
-00001b90: 0000 736e 0200 0064 0164 0284 0074 00a0  ..sn...d.d...t..
-00001ba0: 0188 01a1 0144 0083 017d 0264 0364 0284  .....D...}.d.d..
-00001bb0: 007c 0244 0083 0164 0464 0284 0074 00a0  .|.D...d.d...t..
-00001bc0: 0188 01a1 0144 0083 0117 0089 0087 0166  .....D.........f
-00001bd0: 0164 0564 0284 087c 0244 0083 017d 0374  .d.d...|.D...}.t
-00001be0: 0264 0664 0284 007c 0344 0083 0183 017d  .d.d...|.D.....}
-00001bf0: 0387 0066 0164 0764 0284 087c 0344 0083  ...f.d.d...|.D..
-00001c00: 017d 0374 0383 007d 047c 0464 0075 0072  .}.t...}.|.d.u.r
-00001c10: 4374 0464 0883 0101 0064 0053 0074 0283  Ct.d.....d.S.t..
-00001c20: 007d 057c 0344 005d 5d7d 067c 06a0 0564  .}.|.D.]]}.|...d
-00001c30: 09a1 0172 5071 487c 006a 066a 0767 017c  ...rPqH|.j.j.g.|
-00001c40: 06a0 0864 0aa1 01a2 017d 077c 0764 0b19  ...d.....}.|.d..
-00001c50: 0064 0917 007c 0764 0b3c 0067 007c 06a0  .d...|.d.<.g.|..
-00001c60: 0864 0aa1 01a2 017d 0874 006a 09a0 0a74  .d.....}.t.j...t
-00001c70: 006a 096a 0b7c 078e 00a1 0172 7d64 0ca0  .j.j.|.....r}d..
-00001c80: 0b7c 0764 0064 0b85 0219 00a1 017d 096e  .|.d.d.......}.n
-00001c90: 1d74 006a 09a0 0a74 006a 096a 0b7c 088e  .t.j...t.j.j.|..
-00001ca0: 00a1 0172 8e7c 0864 0d19 0064 0c17 007d  ...r.|.d...d...}
-00001cb0: 096e 0c7c 006a 066a 0764 0c17 007c 06a0  .n.|.j.j.d...|..
-00001cc0: 0c64 0a64 0ca1 0217 007d 097c 0472 a07c  .d.d.....}.|.r.|
-00001cd0: 047c 0917 007d 097c 05a0 0d7c 09a1 0101  .|...}.|...|....
-00001ce0: 0071 4874 0e7c 0583 0164 0d6b 0272 ae64  .qHt.|...d.k.r.d
-00001cf0: 0053 007a 3774 006a 09a0 0b88 0164 0ea1  .S.z7t.j.....d..
-00001d00: 027d 0a74 006a 09a0 0a7c 0aa1 0172 e274  .}.t.j...|...r.t
-00001d10: 0f7c 0a64 0f83 028f 187d 0b74 10a0 117c  .|.d.....}.t...|
-00001d20: 0ba1 017d 0a64 107c 0a76 0072 d07c 0a64  ...}.d.|.v.r.|.d
-00001d30: 1019 007d 0c6e 0269 007d 0c57 0064 0004  ...}.n.i.}.W.d..
-00001d40: 0004 0083 0301 006e 0831 0073 dc77 0101  .......n.1.s.w..
-00001d50: 0001 0001 0059 0001 006e 0269 007d 0c57  .....Y...n.i.}.W
-00001d60: 006e 1d04 0074 1290 0179 0201 007d 0d01  .n...t...y...}..
-00001d70: 007a 1074 0464 1188 019b 0064 129d 0383  .z.t.d.....d....
-00001d80: 0101 0069 007d 0c57 0059 0064 007d 0d7e  ...i.}.W.Y.d.}.~
-00001d90: 0d6e 0564 007d 0d7e 0d77 0177 0074 0f74  .n.d.}.~.w.w.t.t
-00001da0: 006a 09a0 0b88 0164 0ea1 0264 1383 028f  .j.....d...d....
-00001db0: 1f7d 0b74 137c 0583 017c 0c64 149c 027d  .}.t.|...|.d...}
-00001dc0: 0574 106a 147c 057c 0b64 1564 168d 0301  .t.j.|.|.d.d....
-00001dd0: 0074 0464 1788 019b 009d 0283 0101 0057  .t.d...........W
-00001de0: 0064 0004 0004 0083 0301 0064 0053 0031  .d.........d.S.1
-00001df0: 0090 0173 3077 0101 0001 0001 0059 0001  ...s0w.......Y..
-00001e00: 0064 0053 0029 184e 6301 0000 0000 0000  .d.S.).Nc.......
-00001e10: 0000 0000 0002 0000 0005 0000 0053 0000  .............S..
-00001e20: 0073 2200 0000 6700 7c00 5d0d 7d01 7c01  .s"...g.|.].}.|.
-00001e30: a000 6400 a101 7202 6401 7c01 7601 7202  ..d...r.d.|.v.r.
-00001e40: 7c01 9102 7102 5300 2902 fa03 2e70 7972  |...q.S.)....pyr
-00001e50: 6400 0000 2901 da08 656e 6473 7769 7468  d...)...endswith
-00001e60: a902 7256 0000 0072 3400 0000 7214 0000  ..rV...r4...r...
-00001e70: 0072 1400 0000 7215 0000 0072 5800 0000  .r....r....rX...
-00001e80: 0a01 0000 7302 0000 0022 007a 414d 6f64  ....s....".zAMod
-00001e90: 756c 6552 6570 6f73 6974 6f72 792e 5f5f  uleRepository.__
-00001ea0: 6765 6e65 7261 7465 5f6d 6174 655f 6465  generate_mate_de
-00001eb0: 7065 6e64 656e 6369 6573 2e3c 6c6f 6361  pendencies.<loca
-00001ec0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 6301  ls>.<listcomp>c.
-00001ed0: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-00001ee0: 0000 0053 0000 0072 7a00 0000 2902 728c  ...S...rz...).r.
-00001ef0: 0000 0072 4600 0000 727b 0000 00a9 0272  ...rF...r{.....r
-00001f00: 5600 0000 da04 6669 6c65 7214 0000 0072  V.....filer....r
-00001f10: 1400 0000 7215 0000 0072 5800 0000 0b01  ....r....rX.....
-00001f20: 0000 725c 0000 0063 0100 0000 0000 0000  ..r\...c........
-00001f30: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00001f40: 7318 0000 0067 007c 005d 087d 0164 007c  s....g.|.].}.d.|
-00001f50: 0176 0172 027c 0191 0271 0253 0029 0172  .v.r.|...q.S.).r
-00001f60: 6400 0000 7214 0000 0072 8e00 0000 7214  d...r....r....r.
-00001f70: 0000 0072 1400 0000 7215 0000 0072 5800  ...r....r....rX.
-00001f80: 0000 0b01 0000 7304 0000 0006 0012 0163  ......s........c
-00001f90: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001fa0: 0700 0000 1300 0000 731e 0000 0067 007c  ........s....g.|
-00001fb0: 005d 0b7d 0174 0074 016a 02a0 0388 007c  .].}.t.t.j.....|
-00001fc0: 01a1 0283 0191 0271 0253 0072 1400 0000  .......q.S.r....
-00001fd0: 2904 7204 0000 0072 2400 0000 7225 0000  ).r....r$...r%..
-00001fe0: 0072 2c00 0000 728e 0000 0029 0172 2500  .r,...r....).r%.
-00001ff0: 0000 7214 0000 0072 1500 0000 7258 0000  ..r....r....rX..
-00002000: 000f 0100 0073 0200 0000 1e00 6301 0000  .....s......c...
-00002010: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00002020: 0053 0000 0072 7200 0000 7214 0000 0072  .S...rr...r....r
-00002030: 1400 0000 7273 0000 0072 1400 0000 7214  ....rs...r....r.
-00002040: 0000 0072 1500 0000 7258 0000 0012 0100  ...r....rX......
-00002050: 0072 7500 0000 6301 0000 0000 0000 0000  .ru...c.........
-00002060: 0000 0001 0000 0006 0000 0013 0000 0073  ...............s
-00002070: 2600 0000 6700 7c00 5d0f 8900 7400 8700  &...g.|.]...t...
-00002080: 6601 6400 6401 8408 8801 4400 8301 8301  f.d.d.....D.....
-00002090: 7302 8800 9102 7102 5300 2902 6301 0000  s.....q.S.).c...
-000020a0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-000020b0: 0013 0000 0073 1400 0000 6700 7c00 5d06  .....s....g.|.].
-000020c0: 7d01 7c01 8800 7600 9102 7102 5300 7214  }.|...v...q.S.r.
-000020d0: 0000 0072 1400 0000 728f 0000 00a9 01da  ...r....r.......
-000020e0: 066d 6f64 756c 6572 1400 0000 7215 0000  .moduler....r...
-000020f0: 0072 5800 0000 1801 0000 7302 0000 0014  .rX.......s.....
-00002100: 007a 4c4d 6f64 756c 6552 6570 6f73 6974  .zLModuleReposit
-00002110: 6f72 792e 5f5f 6765 6e65 7261 7465 5f6d  ory.__generate_m
-00002120: 6174 655f 6465 7065 6e64 656e 6369 6573  ate_dependencies
-00002130: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00002140: 6f6d 703e 2e3c 6c69 7374 636f 6d70 3e29  omp>.<listcomp>)
-00002150: 01da 0361 6e79 2901 7256 0000 0029 01da  ...any).rV...)..
-00002160: 0e6f 7269 6769 6e61 6c5f 6669 6c65 7372  .original_filesr
-00002170: 9100 0000 7215 0000 0072 5800 0000 1501  ....r....rX.....
-00002180: 0000 730c 0000 0006 0002 0214 0102 fd02  ..s.............
-00002190: 0106 ff7a 2c4e 6f20 6769 7420 7572 6c20  ...z,No git url 
-000021a0: 666f 756e 642c 2073 6b69 7070 696e 6720  found, skipping 
-000021b0: 6465 7065 6e64 656e 6369 6573 2e6a 736f  dependencies.jso
-000021c0: 6e72 8c00 0000 7248 0000 00e9 ffff ffff  nr....rH........
-000021d0: 7276 0000 0072 0100 0000 7278 0000 0072  rv...r....rx...r
-000021e0: 5400 0000 da03 656e 767a 0e45 7272 6f72  T.....envz.Error
-000021f0: 2072 6561 6469 6e67 207a 202f 6465 7065   reading z /depe
-00002200: 6e64 656e 6369 6573 2e6a 736f 6e2c 2073  ndencies.json, s
-00002210: 6b69 7070 696e 6720 656e 7672 1900 0000  kipping envr....
-00002220: 2902 7279 0000 0072 9600 0000 721a 0000  ).ry...r....r...
-00002230: 0072 1b00 0000 7a20 4765 6e65 7261 7465  .r....z Generate
-00002240: 6420 6465 7065 6e64 656e 6369 6573 2e6a  d dependencies.j
-00002250: 736f 6e20 666f 7220 2915 7224 0000 0072  son for ).r$...r
-00002260: 4a00 0000 724f 0000 0072 0500 0000 7229  J...rO...r....r)
-00002270: 0000 0072 8d00 0000 720e 0000 0072 1800  ...r....r....r..
-00002280: 0000 7286 0000 0072 2500 0000 7226 0000  ..r....r%...r&..
-00002290: 0072 2c00 0000 727c 0000 0072 5000 0000  .r,...r|...rP...
-000022a0: 725f 0000 0072 2d00 0000 722e 0000 0072  r_...r-...r....r
-000022b0: 8700 0000 7233 0000 0072 8200 0000 722f  ....r3...r....r/
-000022c0: 0000 0029 0e72 1300 0000 7225 0000 00da  ...).r....r%....
-000022d0: 0566 696c 6573 5a10 7265 6c61 7469 7665  .filesZ.relative
-000022e0: 5f69 6d70 6f72 7473 5a07 7572 6c5f 6769  _importsZ.url_gi
-000022f0: 74da 0464 6570 7372 9200 0000 5a05 7470  t..depsr....Z.tp
-00002300: 6174 685a 1273 6973 7465 725f 6d6f 6475  athZ.sister_modu
-00002310: 6c65 5f70 6174 6872 3800 0000 5a09 6465  le_pathr8...Z.de
-00002320: 7073 5f6a 736f 6e72 3400 0000 7296 0000  ps_jsonr4...r...
-00002330: 0072 3600 0000 7214 0000 0029 0272 9400  .r6...r....).r..
-00002340: 0000 7225 0000 0072 1500 0000 5a1c 5f5f  ..r%...r....Z.__
-00002350: 6765 6e65 7261 7465 5f6d 6174 655f 6465  generate_mate_de
-00002360: 7065 6e64 656e 6369 6573 0701 0000 736e  pendencies....sn
-00002370: 0000 0014 0312 0108 0108 ff12 0402 020c  ................
-00002380: 0104 ff0a 0402 0206 fe06 0608 0208 0104  ................
-00002390: 0106 0208 010a 0202 0114 0310 010e 0214  ................
-000023a0: 0214 0214 010e 0118 0204 0208 010c 010c  ................
-000023b0: 0204 0102 020e 020c 010c 010a 0208 010a  ................
-000023c0: 0104 0202 801c fa02 8004 0904 8010 0110  ................
-000023d0: 0110 0108 8002 fe16 040e 0110 0110 0124  ...............$
-000023e0: fd7a 2d4d 6f64 756c 6552 6570 6f73 6974  .z-ModuleReposit
-000023f0: 6f72 792e 5f5f 6765 6e65 7261 7465 5f6d  ory.__generate_m
-00002400: 6174 655f 6465 7065 6e64 656e 6369 6573  ate_dependencies
-00002410: 6302 0000 0000 0000 0000 0000 0009 0000  c...............
-00002420: 0006 0000 0043 0000 0073 b800 0000 7400  .....C...s....t.
-00002430: a001 7c01 a101 7d02 7400 a002 7c02 a101  ..|...}.t...|...
-00002440: 7d03 7c00 a003 7c01 a101 0100 6700 7d04  }.|...|.....g.}.
-00002450: 7c01 7c00 6a04 6a05 6b02 7224 7400 a006  |.|.j.j.k.r$t...
-00002460: 6401 7c03 6402 a103 0100 7c00 a007 6401  d.|.d.....|...d.
-00002470: a101 0100 6e1d 7400 a006 7408 6a09 a00a  ....n.t...t.j...
-00002480: 7c01 6401 a102 7c03 6402 a103 0100 7c00  |.d...|.d.....|.
-00002490: a007 7408 6a09 a00a 7c01 6401 a102 a101  ..t.j...|.d.....
-000024a0: 0100 740b 6403 7c01 9b00 9d02 8301 0100  ..t.d.|.........
-000024b0: 7c03 4400 5d14 7d05 7c05 6404 1900 7d06  |.D.].}.|.d...}.
-000024c0: 7c05 6405 1900 7d07 7c06 7c07 6406 9c02  |.d...}.|.|.d...
-000024d0: 7d08 7c04 a00c 7c08 a101 0100 7143 6407  }.|...|.....qCd.
-000024e0: 7c04 6901 5300 2908 4e72 7700 0000 7a02  |.i.S.).Nrw...z.
-000024f0: 7e3d 7a1f 4765 6e65 7261 7465 6420 7265  ~=z.Generated re
-00002500: 7175 6972 656d 656e 7473 2e74 7874 2066  quirements.txt f
-00002510: 6f72 2072 6d00 0000 da07 7665 7273 696f  or rm.....versio
-00002520: 6e29 0272 6d00 0000 7299 0000 00da 0370  n).rm...r......p
-00002530: 6970 290d 720a 0000 005a 0f67 6574 5f61  ip).r....Z.get_a
-00002540: 6c6c 5f69 6d70 6f72 7473 5a10 6765 745f  ll_importsZ.get_
-00002550: 696d 706f 7274 5f6c 6f63 616c da2d 5f4d  import_local.-_M
-00002560: 6f64 756c 6552 6570 6f73 6974 6f72 795f  oduleRepository_
-00002570: 5f67 656e 6572 6174 655f 6d61 7465 5f64  _generate_mate_d
-00002580: 6570 656e 6465 6e63 6965 7372 0e00 0000  ependenciesr....
-00002590: 7218 0000 005a 1a67 656e 6572 6174 655f  r....Z.generate_
-000025a0: 7265 7175 6972 656d 656e 7473 5f66 696c  requirements_fil
-000025b0: 65da 305f 4d6f 6475 6c65 5265 706f 7369  e.0_ModuleReposi
-000025c0: 746f 7279 5f5f 6164 645f 696e 6465 785f  tory__add_index_
-000025d0: 7572 6c5f 746f 5f72 6571 7569 7265 6d65  url_to_requireme
-000025e0: 6e74 7372 2400 0000 7225 0000 0072 2c00  ntsr$...r%...r,.
-000025f0: 0000 7229 0000 0072 8400 0000 2909 7213  ..r)...r....).r.
-00002600: 0000 0072 2500 0000 da07 696d 706f 7274  ...r%.....import
-00002610: 735a 1169 6d70 6f72 745f 696e 666f 5f6c  sZ.import_info_l
-00002620: 6f63 616c 5a0b 696d 706f 7274 5f69 6e66  ocalZ.import_inf
-00002630: 6f5a 0269 6d72 6d00 0000 7299 0000 00da  oZ.imrm...r.....
-00002640: 0372 6573 7214 0000 0072 1400 0000 7215  .resr....r....r.
-00002650: 0000 005a 1b5f 5f67 656e 6572 6174 655f  ...Z.__generate_
-00002660: 7069 705f 7265 7175 6972 656d 656e 7473  pip_requirements
-00002670: 5301 0000 732c 0000 000a 030a 030a 0204  S...s,..........
-00002680: 020c 0204 0106 0104 ff0c 0304 0310 0104  ................
-00002690: ff14 030e 0108 0208 0208 0102 0302 0106  ................
-000026a0: fe0c 0508 027a 2c4d 6f64 756c 6552 6570  .....z,ModuleRep
-000026b0: 6f73 6974 6f72 792e 5f5f 6765 6e65 7261  ository.__genera
-000026c0: 7465 5f70 6970 5f72 6571 7569 7265 6d65  te_pip_requireme
-000026d0: 6e74 7372 9200 0000 6302 0000 0000 0000  ntsr....c.......
-000026e0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-000026f0: 0073 1e00 0000 7c01 6400 6b02 7209 7c00  .s....|.d.k.r.|.
-00002700: 6a00 a001 a100 5300 7c00 6a00 a002 7c01  j.....S.|.j...|.
-00002710: a101 5300 7210 0000 0029 0372 1200 0000  ..S.r....).r....
-00002720: da07 7375 6d6d 6172 7972 8200 0000 2902  ..summaryr....).
-00002730: 7213 0000 0072 9200 0000 7214 0000 0072  r....r....r....r
-00002740: 1400 0000 7215 0000 0072 8200 0000 7a01  ....r....r....z.
-00002750: 0000 7306 0000 0008 010a 010c 017a 154d  ..s..........z.M
-00002760: 6f64 756c 6552 6570 6f73 6974 6f72 792e  oduleRepository.
-00002770: 6c69 7374 6301 0000 0000 0000 0000 0000  listc...........
-00002780: 0001 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
-00002790: 0000 7c00 6a00 a001 a100 5300 7210 0000  ..|.j.....S.r...
-000027a0: 0029 0272 1200 0000 729f 0000 0029 0172  .).r....r....).r
-000027b0: 1300 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
-000027c0: 0000 00da 1067 6574 5f6d 6174 655f 7375  .....get_mate_su
-000027d0: 6d6d 6172 797f 0100 0073 0200 0000 0a01  mmary....s......
-000027e0: 7a21 4d6f 6475 6c65 5265 706f 7369 746f  z!ModuleReposito
-000027f0: 7279 2e67 6574 5f6d 6174 655f 7375 6d6d  ry.get_mate_summ
-00002800: 6172 79da 0770 6163 6b61 6765 6302 0000  ary..packagec...
-00002810: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00002820: 0043 0000 0073 1000 0000 7c00 6a00 a001  .C...s....|.j...
-00002830: 7c01 a101 0100 6400 5300 7210 0000 0029  |.....d.S.r....)
-00002840: 0272 1200 0000 7239 0000 0029 0272 1300  .r....r9...).r..
-00002850: 0000 72a1 0000 0072 1400 0000 7214 0000  ..r....r....r...
-00002860: 0072 1500 0000 7239 0000 0082 0100 0073  .r....r9.......s
-00002870: 0200 0000 1001 7a20 4d6f 6475 6c65 5265  ......z ModuleRe
-00002880: 706f 7369 746f 7279 2e69 6e73 7461 6c6c  pository.install
-00002890: 5f70 6163 6b61 6765 2901 4672 1000 0000  _package).Fr....
-000028a0: 2917 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000028b0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000028c0: 6e61 6d65 5f5f 7207 0000 00da 0462 6f6f  name__r......boo
-000028d0: 6c72 1600 0000 da0c 7374 6174 6963 6d65  lr......staticme
-000028e0: 7468 6f64 da03 7374 7272 3700 0000 723c  thod..strr7...r<
-000028f0: 0000 0072 4400 0000 7243 0000 0072 8200  ...rD...rC...r..
-00002900: 0000 7262 0000 0072 9c00 0000 7267 0000  ..rb...r....rg..
-00002910: 0072 4200 0000 7281 0000 0072 9b00 0000  .rB...r....r....
-00002920: 7266 0000 0072 a000 0000 720b 0000 0072  rf...r....r....r
-00002930: 3900 0000 7214 0000 0072 1400 0000 7214  9...r....r....r.
-00002940: 0000 0072 1500 0000 720d 0000 0015 0000  ...r....r.......
-00002950: 0073 2200 0000 0800 1401 0207 1001 0e2a  .s"............*
-00002960: 0e04 1006 1212 0e0e 081d 0816 084e 0814  .............N..
-00002970: 084c 1027 0805 1203 720d 0000 0029 1872  .L.'....r....).r
-00002980: 2e00 0000 7224 0000 0072 6000 0000 722a  ....r$...r`...r*
-00002990: 0000 0072 8800 0000 5a0e 6d6f 6475 6c65  ...r....Z.module
-000029a0: 5f6d 616e 6167 6572 7203 0000 005a 0e75  _managerr....Z.u
-000029b0: 7469 6c73 2e65 7870 5f75 7469 6c72 0400  tils.exp_utilr..
-000029c0: 0000 5a0e 7574 696c 732e 6769 745f 7574  ..Z.utils.git_ut
-000029d0: 696c 7205 0000 00da 0b6d 6174 655f 636f  ilr......mate_co
-000029e0: 6e66 6967 7207 0000 005a 0e73 6f75 7263  nfigr....Z.sourc
-000029f0: 6573 2e72 656d 6f74 6572 0800 0000 5a13  es.remoter....Z.
-00002a00: 736f 7572 6365 732e 6c6f 6361 6c2e 6c6f  sources.local.lo
-00002a10: 6361 6c72 0900 0000 720a 0000 0072 a100  calr....r....r..
-00002a20: 0000 720b 0000 00da 0674 7970 696e 6772  ..r......typingr
-00002a30: 0c00 0000 da04 6970 6462 720d 0000 0072  ......ipdbr....r
-00002a40: 1400 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
-00002a50: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00002a60: 0073 2000 0000 0800 0801 0801 0801 0802  .s .............
-00002a70: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c02  ................
-00002a80: 0c01 0801 1203                           ......
+00000070: 6405 6c09 6d0a 5a0a 0100 6402 6406 6c0b  d.l.m.Z...d.d.l.
+00000080: 6d0c 5a0c 0100 6402 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
+00000090: 0100 6400 6408 6c0f 6d0f 5a0f 0100 6402  ..d.d.l.m.Z...d.
+000000a0: 6409 6c10 6d11 5a11 0100 6400 640a 6c12  d.l.m.Z...d.d.l.
+000000b0: 6d13 5a13 0100 6400 6401 6c14 5a14 4700  m.Z...d.d.l.Z.G.
+000000c0: 640b 640c 8400 640c 8302 5a15 6401 5300  d.d...d...Z.d.S.
+000000d0: 290d e900 0000 004e e901 0000 0029 01da  )......N.....)..
+000000e0: 0d4d 6f64 756c 654d 616e 6167 6572 2901  .ModuleManager).
+000000f0: da14 6765 745f 7265 6c61 7469 7665 5f69  ..get_relative_i
+00000100: 6d70 6f72 7473 2901 da12 7061 7273 655f  mports)...parse_
+00000110: 7572 6c5f 6672 6f6d 5f67 6974 2901 da10  url_from_git)...
+00000120: 5265 6d6f 7465 4461 7461 536f 7572 6365  RemoteDataSource
+00000130: 2901 da0f 4c6f 6361 6c44 6174 6153 6f75  )...LocalDataSou
+00000140: 7263 6529 01da 0770 6970 7265 7173 2901  rce)...pipreqs).
+00000150: da07 5061 636b 6167 6529 01da 084f 7074  ..Package)...Opt
+00000160: 696f 6e61 6c63 0000 0000 0000 0000 0000  ionalc..........
+00000170: 0000 0000 0000 0400 0000 4000 0000 73c8  ..........@...s.
+00000180: 0000 0065 005a 0164 005a 0264 2a64 0265  ...e.Z.d.Z.d*d.e
+00000190: 0366 0264 0364 0484 055a 0465 0564 0565  .f.d.d...Z.e.d.e
+000001a0: 0666 0264 0664 0784 0483 015a 0764 0865  .f.d.d.....Z.d.e
+000001b0: 0666 0264 0964 0a84 045a 0864 0b65 0666  .f.d.d...Z.d.e.f
+000001c0: 0264 0c64 0d84 045a 0964 2b64 0f65 0666  .d.d...Z.d+d.e.f
+000001d0: 0264 1064 1184 055a 0a64 1265 0b65 0619  .d.d...Z.d.e.e..
+000001e0: 0066 0264 1364 1484 045a 0c64 1565 0666  .f.d.d...Z.d.e.f
+000001f0: 0264 1664 1784 045a 0d64 1864 1984 005a  .d.d...Z.d.d...Z
+00000200: 0e64 1a64 1b84 005a 0f64 1c64 1d84 005a  .d.d...Z.d.d...Z
+00000210: 1064 1e64 1f84 005a 1164 2064 2184 005a  .d.d...Z.d d!..Z
+00000220: 1264 2b64 2265 0666 0264 2364 2484 055a  .d+d"e.f.d#d$..Z
+00000230: 0b64 2564 2684 005a 1364 2765 1466 0264  .d%d&..Z.d'e.f.d
+00000240: 2864 2984 045a 1564 0e53 0029 2cda 104d  (d)..Z.d.S.),..M
+00000250: 6f64 756c 6552 6570 6f73 6974 6f72 7946  oduleRepositoryF
+00000260: da14 7275 6e5f 6c6f 6361 6c5f 6170 695f  ..run_local_api_
+00000270: 7365 7276 6572 6303 0000 0000 0000 0000  serverc.........
+00000280: 0000 0003 0000 0002 0000 0043 0000 0073  ...........C...s
+00000290: 2600 0000 7c01 7c00 5f00 7401 7c01 8301  &...|.|._.t.|...
+000002a0: 7c00 5f02 7403 8300 7c00 5f04 7405 7c01  |._.t...|._.t.|.
+000002b0: 8301 7c00 5f06 6400 5300 a901 4e29 07da  ..|._.d.S...N)..
+000002c0: 0663 6f6e 6669 6772 0300 0000 da0f 7061  .configr......pa
+000002d0: 636b 6167 655f 6d61 6e61 6765 7272 0600  ckage_managerr..
+000002e0: 0000 5a06 7265 6d6f 7465 7207 0000 00da  ..Z.remoter.....
+000002f0: 056c 6f63 616c 2903 da04 7365 6c66 720e  .local)...selfr.
+00000300: 0000 0072 0c00 0000 a900 7212 0000 00fa  ...r......r.....
+00000310: 4a2f 686f 6d65 2f61 6c2f 4769 7448 7562  J/home/al/GitHub
+00000320: 2f79 6572 6261 6d61 7465 2f70 6163 6b61  /yerbamate/packa
+00000330: 6765 732f 7965 7262 616d 6174 652f 6170  ges/yerbamate/ap
+00000340: 692f 6461 7461 2f6d 6f64 756c 655f 7265  i/data/module_re
+00000350: 706f 7369 746f 7279 2e70 79da 085f 5f69  pository.py..__i
+00000360: 6e69 745f 5f15 0000 0073 0800 0000 0601  nit__....s......
+00000370: 0a01 0801 0e01 7a19 4d6f 6475 6c65 5265  ......z.ModuleRe
+00000380: 706f 7369 746f 7279 2e5f 5f69 6e69 745f  pository.__init_
+00000390: 5fda 0c70 726f 6a65 6374 5f6e 616d 6563  _..project_namec
+000003a0: 0100 0000 0000 0000 0000 0000 0800 0000  ................
+000003b0: 0a00 0000 4300 0000 736e 0100 0074 006a  ....C...sn...t.j
+000003c0: 01a0 027c 00a1 0173 1174 00a0 037c 00a1  ...|...s.t...|..
+000003d0: 0101 0074 00a0 047c 00a1 0101 006e 0974  ...t...|.....n.t
+000003e0: 0564 0183 0101 0074 06a0 0764 02a1 0101  .d.....t...d....
+000003f0: 0074 006a 01a0 0864 03a1 017d 0174 006a  .t.j...d...}.t.j
+00000400: 01a0 027c 01a1 0173 4864 047c 0069 017d  ...|...sHd.|.i.}
+00000410: 0274 097c 0164 0583 028f 107d 0374 0a6a  .t.|.d.....}.t.j
+00000420: 0b7c 027c 0364 0664 078d 0301 0057 0064  .|.|.d.d.....W.d
+00000430: 0004 0004 0083 0301 006e 0831 0073 4277  .........n.1.sBw
+00000440: 0101 0001 0001 0059 0001 006e 0974 0564  .......Y...n.t.d
+00000450: 0183 0101 0074 06a0 0764 02a1 0101 0074  .....t...d.....t
+00000460: 006a 01a0 027c 00a1 0173 6a74 00a0 037c  .j...|...sjt...|
+00000470: 00a1 0101 0074 006a 01a0 087c 0064 08a1  .....t.j...|.d..
+00000480: 027d 0474 097c 0464 0983 02a0 0ca1 0001  .}.t.|.d........
+00000490: 007a 3567 0064 0aa2 017d 057c 0544 005d  .z5g.d...}.|.D.]
+000004a0: 237d 0674 006a 0d74 006a 01a0 087c 007c  #}.t.j.t.j...|.|
+000004b0: 06a1 0264 0b64 0c8d 0201 0074 006a 01a0  ...d.d.....t.j..
+000004c0: 087c 007c 0664 08a1 037d 0474 006a 01a0  .|.|.d...}.t.j..
+000004d0: 027c 04a1 0173 9474 097c 0464 0983 02a0  .|...s.t.|.d....
+000004e0: 0ca1 0001 0071 7174 0564 0da0 0e7c 007c  .....qqt.d...|.|
+000004f0: 00a1 0283 0101 0057 0064 0053 0004 0074  .......W.d.S...t
+00000500: 0f79 b601 007d 0701 007a 0b74 057c 0783  .y...}...z.t.|..
+00000510: 0101 0057 0059 0064 007d 077e 0764 0053  ...W.Y.d.}.~.d.S
+00000520: 0064 007d 077e 0777 0177 0029 0e4e 7a16  .d.}.~.w.w.).Nz.
+00000530: 5072 6f6a 6563 7420 616c 7265 6164 7920  Project already 
+00000540: 6578 6973 7473 7202 0000 007a 096d 6174  existsr....z.mat
+00000550: 652e 6a73 6f6e da07 7072 6f6a 6563 74da  e.json..project.
+00000560: 0177 e904 0000 00a9 01da 0669 6e64 656e  .w.........inden
+00000570: 74fa 0b5f 5f69 6e69 745f 5f2e 7079 da01  t..__init__.py..
+00000580: 6129 04da 0b65 7870 6572 696d 656e 7473  a)...experiments
+00000590: da06 6d6f 6465 6c73 da04 6461 7461 da08  ..models..data..
+000005a0: 7472 6169 6e65 7273 5429 01da 0865 7869  trainersT)...exi
+000005b0: 7374 5f6f 6b7a 3b50 726f 6a65 6374 207b  st_okz;Project {
+000005c0: 7d20 6372 6561 7465 642c 2072 756e 2060  } created, run `
+000005d0: 6364 207b 7d60 2074 6f20 656e 7465 7220  cd {}` to enter 
+000005e0: 7468 6520 7072 6f6a 6563 7420 666f 6c64  the project fold
+000005f0: 6572 2910 da02 6f73 da04 7061 7468 da06  er)...os..path..
+00000600: 6578 6973 7473 da05 6d6b 6469 72da 0563  exists..mkdir..c
+00000610: 6864 6972 da05 7072 696e 74da 0373 7973  hdir..print..sys
+00000620: da04 6578 6974 da04 6a6f 696e da04 6f70  ..exit..join..op
+00000630: 656e da04 6a73 6f6e da04 6475 6d70 da05  en..json..dump..
+00000640: 636c 6f73 65da 086d 616b 6564 6972 73da  close..makedirs.
+00000650: 0666 6f72 6d61 74da 0945 7863 6570 7469  .format..Excepti
+00000660: 6f6e 2908 7215 0000 005a 096d 6174 655f  on).r....Z.mate_
+00000670: 6a73 6f6e 5a03 6469 63da 0166 5a0a 696e  jsonZ.dic..fZ.in
+00000680: 6974 5f5f 6669 6c65 5a07 666f 6c64 6572  it__fileZ.folder
+00000690: 73da 0666 6f6c 6465 72da 0165 7212 0000  s..folder..er...
+000006a0: 0072 1200 0000 7213 0000 00da 0c69 6e69  .r....r......ini
+000006b0: 745f 7072 6f6a 6563 741c 0000 0073 4800  t_project....sH.
+000006c0: 0000 0c03 0a01 0c01 0802 0a01 0c02 0c01  ................
+000006d0: 0402 04ff 0c05 1201 1cff 0280 0803 0a01  ................
+000006e0: 0c02 0a01 0e01 0e01 0201 0801 0801 1801  ................
+000006f0: 1001 0c01 0e01 0280 0201 0401 0401 02ff  ................
+00000700: 0aff 0e06 1601 0880 02ff 7a1d 4d6f 6475  ..........z.Modu
+00000710: 6c65 5265 706f 7369 746f 7279 2e69 6e69  leRepository.ini
+00000720: 745f 7072 6f6a 6563 74da 0375 726c 6302  t_project..urlc.
+00000730: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+00000740: 0000 004f 0000 0073 1e00 0000 7c00 6a00  ...O...s....|.j.
+00000750: 6a01 7c01 6701 7c02 a201 5200 6900 7c03  j.|.g.|...R.i.|.
+00000760: a401 8e01 0100 6400 5300 720d 0000 0029  ......d.S.r....)
+00000770: 0272 0f00 0000 da0f 696e 7374 616c 6c5f  .r......install_
+00000780: 7061 636b 6167 6529 0472 1100 0000 7236  package).r....r6
+00000790: 0000 00da 0461 7267 73da 066b 7761 7267  .....args..kwarg
+000007a0: 7372 1200 0000 7212 0000 0072 1300 0000  sr....r....r....
+000007b0: da0b 696e 7374 616c 6c5f 7572 6c47 0000  ..install_urlG..
+000007c0: 0073 0200 0000 1e02 7a1c 4d6f 6475 6c65  .s......z.Module
+000007d0: 5265 706f 7369 746f 7279 2e69 6e73 7461  Repository.insta
+000007e0: 6c6c 5f75 726c da07 636f 6d6d 616e 6463  ll_url..commandc
+000007f0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00000800: 0300 0000 4700 0000 7332 0000 007c 0164  ....G...s2...|.d
+00000810: 016b 0272 0a7c 00a0 00a1 0001 0064 0053  .k.r.|.......d.S
+00000820: 007c 0164 0276 0072 177c 00a0 017c 006a  .|.d.v.r.|...|.j
+00000830: 026a 03a1 0101 0064 0053 0064 0053 0029  .j.....d.S.d.S.)
+00000840: 034e da06 6578 706f 7274 2903 da04 696e  .N..export)...in
+00000850: 6974 da03 6669 78da 0169 2904 da19 5f4d  it..fix..i)..._M
+00000860: 6f64 756c 6552 6570 6f73 6974 6f72 795f  oduleRepository_
+00000870: 5f65 7870 6f72 74da 125f 5f67 656e 6572  _export..__gener
+00000880: 6174 655f 5f69 6e69 745f 5f72 0e00 0000  ate__init__r....
+00000890: 7216 0000 0029 0372 1100 0000 723b 0000  r....).r....r;..
+000008a0: 0072 3800 0000 7212 0000 0072 1200 0000  .r8...r....r....
+000008b0: 7213 0000 00da 0461 7574 6f4b 0000 0073  r......autoK...s
+000008c0: 0a00 0000 0801 0c01 0801 1201 04ff 7a15  ..............z.
+000008d0: 4d6f 6475 6c65 5265 706f 7369 746f 7279  ModuleRepository
+000008e0: 2e61 7574 6f4e da04 726f 6f74 6302 0000  .autoN..rootc...
+000008f0: 0000 0000 0000 0000 0006 0000 0009 0000  ................
+00000900: 0043 0000 0073 0201 0000 7400 6a01 a002  .C...s....t.j...
+00000910: 7c01 6401 a102 7d02 7400 6a01 a003 7c02  |.d...}.t.j...|.
+00000920: a101 732e 7404 7c02 6402 8302 8f0d 7d03  ..s.t.|.d.....}.
+00000930: 7c03 a005 6403 a101 0100 5700 6400 0400  |...d.....W.d...
+00000940: 0400 8303 0100 6e08 3100 7322 7701 0100  ......n.1.s"w...
+00000950: 0100 0100 5900 0100 7406 6404 7c02 9b00  ....Y...t.d.|...
+00000960: 9d02 8301 0100 7400 a007 7c01 a101 4400  ......t...|...D.
+00000970: 5d4b 7d04 7400 6a01 a002 7c01 7c04 a102  ]K}.t.j...|.|...
+00000980: 7d05 7400 6a01 a008 7c05 a101 724a 7c04  }.t.j...|...rJ|.
+00000990: 6405 6b02 734a 6406 7c04 7600 724b 7133  d.k.sJd.|.v.rKq3
+000009a0: 7400 6a01 a002 7c05 6401 a102 7d02 7400  t.j...|.d...}.t.
+000009b0: 6a01 a003 7c02 a101 7379 7404 7c02 6402  j...|...syt.|.d.
+000009c0: 8302 8f0d 7d03 7c03 a005 6403 a101 0100  ....}.|...d.....
+000009d0: 5700 6400 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
+000009e0: 736d 7701 0100 0100 0100 5900 0100 7406  smw.......Y...t.
+000009f0: 6404 7c02 9b00 9d02 8301 0100 7c00 a009  d.|.........|...
+00000a00: 7c05 a101 0100 7133 6400 5300 2907 4e72  |.....q3d.S.).Nr
+00000a10: 1b00 0000 7217 0000 00da 007a 0843 7265  ....r......z.Cre
+00000a20: 6174 6564 20da 0b5f 5f70 7963 6163 6865  ated ..__pycache
+00000a30: 5f5f da01 2e29 0a72 2200 0000 7223 0000  __...).r"...r#..
+00000a40: 0072 2a00 0000 7224 0000 0072 2b00 0000  .r*...r$...r+...
+00000a50: da05 7772 6974 6572 2700 0000 da07 6c69  ..writer'.....li
+00000a60: 7374 6469 72da 0569 7364 6972 7241 0000  stdir..isdirrA..
+00000a70: 0029 0672 1100 0000 7243 0000 005a 0869  .).r....rC...Z.i
+00000a80: 6e69 745f 5f70 7972 3200 0000 7233 0000  nit__pyr2...r3..
+00000a90: 0072 2300 0000 7212 0000 0072 1200 0000  .r#...r....r....
+00000aa0: 7213 0000 0072 4100 0000 5100 0000 7324  r....rA...Q...s$
+00000ab0: 0000 000e 010c 010c 010c 011c ff0e 020e  ................
+00000ac0: 020e 011c 0102 010e 010c 010c 010c 011c  ................
+00000ad0: ff0e 020c 0104 f77a 234d 6f64 756c 6552  .......z#ModuleR
+00000ae0: 6570 6f73 6974 6f72 792e 5f5f 6765 6e65  epository.__gene
+00000af0: 7261 7465 5f5f 696e 6974 5f5f da04 7265  rate__init__..re
+00000b00: 7173 6302 0000 0000 0000 0000 0000 0005  qsc.............
+00000b10: 0000 0005 0000 0043 0000 0073 4a00 0000  .......C...sJ...
+00000b20: 6401 6402 6403 9c02 7d02 7400 8300 7d03  d.d.d...}.t...}.
+00000b30: 7c01 4400 5d18 7d04 6404 7c04 7600 7217  |.D.].}.d.|.v.r.
+00000b40: 7c03 a001 7c02 6404 1900 a101 0100 6405  |...|.d.......d.
+00000b50: 7c04 7600 7222 7c03 a001 7c02 6405 1900  |.v.r"|...|.d...
+00000b60: a101 0100 710a 7c03 5300 2906 4e7a 3268  ....q.|.S.).Nz2h
+00000b70: 7474 7073 3a2f 2f64 6f77 6e6c 6f61 642e  ttps://download.
+00000b80: 7079 746f 7263 682e 6f72 672f 7768 6c2f  pytorch.org/whl/
+00000b90: 746f 7263 685f 7374 6162 6c65 2e68 746d  torch_stable.htm
+00000ba0: 6c7a 3d68 7474 7073 3a2f 2f73 746f 7261  lz=https://stora
+00000bb0: 6765 2e67 6f6f 676c 6561 7069 732e 636f  ge.googleapis.co
+00000bc0: 6d2f 6a61 782d 7265 6c65 6173 6573 2f6a  m/jax-releases/j
+00000bd0: 6178 5f72 656c 6561 7365 732e 6874 6d6c  ax_releases.html
+00000be0: 2902 da05 746f 7263 68da 036a 6178 724b  )...torch..jaxrK
+00000bf0: 0000 0072 4c00 0000 2902 da03 7365 74da  ...rL...)...set.
+00000c00: 0361 6464 2905 7211 0000 0072 4a00 0000  .add).r....rJ...
+00000c10: da04 7572 6c73 da07 696e 6465 7865 73da  ..urls..indexes.
+00000c20: 0372 6571 7212 0000 0072 1200 0000 7213  .reqr....r....r.
+00000c30: 0000 005a 125f 5f70 6172 7365 5f69 6e64  ...Z.__parse_ind
+00000c40: 6578 5f75 726c 7363 0000 0073 1600 0000  ex_urlsc...s....
+00000c50: 0202 0201 06fe 0604 0801 0801 0e01 0801  ................
+00000c60: 0e01 0280 0402 7a23 4d6f 6475 6c65 5265  ......z#ModuleRe
+00000c70: 706f 7369 746f 7279 2e5f 5f70 6172 7365  pository.__parse
+00000c80: 5f69 6e64 6578 5f75 726c 7372 2300 0000  _index_urlsr#...
+00000c90: 6302 0000 0000 0000 0000 0000 0008 0000  c...............
+00000ca0: 0008 0000 0003 0000 0073 4601 0000 7400  .........sF...t.
+00000cb0: 7401 6a02 a003 7c01 a101 6401 8302 8f0c  t.j...|...d.....
+00000cc0: 7d02 7c02 a004 a100 7d03 5700 6400 0400  }.|.....}.W.d...
+00000cd0: 0400 8303 0100 6e08 3100 7318 7701 0100  ......n.1.s.w...
+00000ce0: 0100 0100 5900 0100 7405 7c03 8301 7d04  ....Y...t.|...}.
+00000cf0: 6402 6403 8400 7c03 4400 8301 7d03 7406  d.d...|.D...}.t.
+00000d00: a007 6404 a101 8900 8700 6601 6405 6403  ..d.......f.d.d.
+00000d10: 8408 7c03 4400 8301 7d03 7c00 a008 7c03  ..|.D...}.|...|.
+00000d20: a101 7d05 7405 7c05 8301 6406 6b04 7275  ..}.t.|...d.k.ru
+00000d30: 7400 7401 6a02 a003 7c01 a101 6407 8302  t.t.j...|...d...
+00000d40: 8f21 7d02 7c05 4400 5d0b 7d06 7c02 a009  .!}.|.D.].}.|...
+00000d50: 6408 7c06 9b00 6409 9d03 a101 0100 714d  d.|...d.......qM
+00000d60: 7c03 4400 5d07 7d07 7c02 a009 7c07 a101  |.D.].}.|...|...
+00000d70: 0100 715b 5700 6400 0400 0400 8303 0100  ..q[W.d.........
+00000d80: 6400 5300 3100 736e 7701 0100 0100 0100  d.S.1.snw.......
+00000d90: 5900 0100 6400 5300 7c04 7405 7c03 8301  Y...d.S.|.t.|...
+00000da0: 6b03 72a1 7400 7401 6a02 a003 7c01 a101  k.r.t.t.j...|...
+00000db0: 6407 8302 8f13 7d02 7c03 4400 5d07 7d07  d.....}.|.D.].}.
+00000dc0: 7c02 a009 7c07 a101 0100 7187 5700 6400  |...|.....q.W.d.
+00000dd0: 0400 0400 8303 0100 6400 5300 3100 739a  ........d.S.1.s.
+00000de0: 7701 0100 0100 0100 5900 0100 6400 5300  w.......Y...d.S.
+00000df0: 6400 5300 290a 4eda 0172 6301 0000 0000  d.S.).N..rc.....
+00000e00: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+00000e10: 0000 0073 2800 0000 6700 7c00 5d10 7d01  ...s(...g.|.].}.
+00000e20: 6400 7c01 7601 7212 6401 7c01 7601 7212  d.|.v.r.d.|.v.r.
+00000e30: 6402 7c01 7601 7202 7c01 9102 7102 5300  d.|.v.r.|...q.S.
+00000e40: 2903 7a0a 2e65 6767 3e3d 696e 666f 7a0a  ).z..egg>=infoz.
+00000e50: 2e65 6767 3d3d 696e 666f 7a0a 2e65 6767  .egg==infoz..egg
+00000e60: 7e3d 696e 666f 7212 0000 00a9 02da 022e  ~=infor.........
+00000e70: 30da 046c 696e 6572 1200 0000 7212 0000  0..liner....r...
+00000e80: 0072 1300 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
+00000e90: 703e 7500 0000 730e 0000 0006 0002 0208  p>u...s.........
+00000ea0: 0108 0108 0102 fc06 047a 444d 6f64 756c  .........zDModul
+00000eb0: 6552 6570 6f73 6974 6f72 792e 5f5f 6164  eRepository.__ad
+00000ec0: 645f 696e 6465 785f 7572 6c5f 746f 5f72  d_index_url_to_r
+00000ed0: 6571 7569 7265 6d65 6e74 732e 3c6c 6f63  equirements.<loc
+00000ee0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e7a  als>.<listcomp>z
+00000ef0: 075c 2b63 755c 642b 6301 0000 0000 0000  .\+cu\d+c.......
+00000f00: 0000 0000 0002 0000 0006 0000 0013 0000  ................
+00000f10: 0073 1800 0000 6700 7c00 5d08 7d01 8800  .s....g.|.].}...
+00000f20: a000 6400 7c01 a102 9102 7102 5300 2901  ..d.|.....q.S.).
+00000f30: 7244 0000 0029 01da 0373 7562 7253 0000  rD...)...subrS..
+00000f40: 00a9 01da 0572 6567 6578 7212 0000 0072  .....regexr....r
+00000f50: 1300 0000 7256 0000 0080 0000 00f3 0200  ....rV..........
+00000f60: 0000 1800 7201 0000 0072 1700 0000 7a12  ....r....r....z.
+00000f70: 2d2d 6578 7472 612d 696e 6465 782d 7572  --extra-index-ur
+00000f80: 6c20 da01 0a29 0a72 2b00 0000 7222 0000  l ...).r+...r"..
+00000f90: 0072 2300 0000 722a 0000 00da 0972 6561  .r#...r*.....rea
+00000fa0: 646c 696e 6573 da03 6c65 6eda 0272 65da  dlines..len..re.
+00000fb0: 0763 6f6d 7069 6c65 da23 5f4d 6f64 756c  .compile.#_Modul
+00000fc0: 6552 6570 6f73 6974 6f72 795f 5f70 6172  eRepository__par
+00000fd0: 7365 5f69 6e64 6578 5f75 726c 7372 4700  se_index_urlsrG.
+00000fe0: 0000 2908 7211 0000 0072 2300 0000 7232  ..).r....r#...r2
+00000ff0: 0000 00da 056c 696e 6573 5a09 6c69 6e65  .....linesZ.line
+00001000: 636f 756e 7472 4f00 0000 7236 0000 0072  countrO...r6...r
+00001010: 5500 0000 7212 0000 0072 5800 0000 7213  U...r....rX...r.
+00001020: 0000 005a 1f5f 5f61 6464 5f69 6e64 6578  ...Z.__add_index
+00001030: 5f75 726c 5f74 6f5f 7265 7175 6972 656d  _url_to_requirem
+00001040: 656e 7473 7100 0000 7332 0000 0014 010a  entsq...s2......
+00001050: 011c ff08 0206 0102 0206 fe0a 0a12 010a  ................
+00001060: 020c 0114 0108 0114 0108 010c 0102 ff22  ..............."
+00001070: fd0c 0514 0108 010c 0102 ff22 ff04 ff7a  ..........."...z
+00001080: 304d 6f64 756c 6552 6570 6f73 6974 6f72  0ModuleRepositor
+00001090: 792e 5f5f 6164 645f 696e 6465 785f 7572  y.__add_index_ur
+000010a0: 6c5f 746f 5f72 6571 7569 7265 6d65 6e74  l_to_requirement
+000010b0: 7363 0200 0000 0000 0000 0000 0000 0500  sc..............
+000010c0: 0000 0600 0000 4300 0000 738a 0000 0074  ......C...s....t
+000010d0: 00a0 017c 01a1 0144 005d 3d7d 027c 02a0  ...|...D.]=}.|..
+000010e0: 0264 01a1 0173 117c 02a0 0264 02a1 0172  .d...s.|...d...r
+000010f0: 1271 0574 006a 03a0 047c 017c 02a1 027d  .q.t.j...|.|...}
+00001100: 0374 006a 03a0 057c 03a1 0172 4274 006a  .t.j...|...rBt.j
+00001110: 03a0 047c 017c 0264 03a1 037d 0474 006a  ...|.|.d...}.t.j
+00001120: 03a0 067c 04a1 0173 2e71 057c 0264 0476  ...|...s.q.|.d.v
+00001130: 0072 387c 006a 076a 087c 0176 0073 3d7c  .r8|.j.j.|.v.s=|
+00001140: 00a0 097c 03a1 0101 007c 00a0 0a7c 03a1  ...|.....|...|..
+00001150: 0101 0071 0564 0053 0029 054e 7246 0000  ...q.d.S.).NrF..
+00001160: 00da 025f 5f72 1b00 0000 2904 7220 0000  ...__r....).r ..
+00001170: 0072 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00001180: 290b 7222 0000 0072 4800 0000 da0a 7374  ).r"...rH.....st
+00001190: 6172 7473 7769 7468 7223 0000 0072 2a00  artswithr#...r*.
+000011a0: 0000 7249 0000 0072 2400 0000 720e 0000  ..rI...r$...r...
+000011b0: 0072 1600 0000 da2c 5f4d 6f64 756c 6552  .r.....,_ModuleR
+000011c0: 6570 6f73 6974 6f72 795f 5f67 656e 6572  epository__gener
+000011d0: 6174 655f 7069 705f 7265 7175 6972 656d  ate_pip_requirem
+000011e0: 656e 7473 da29 5f4d 6f64 756c 6552 6570  ents.)_ModuleRep
+000011f0: 6f73 6974 6f72 795f 5f67 656e 6572 6174  ository__generat
+00001200: 655f 6465 7073 5f69 6e5f 6465 7074 68a9  e_deps_in_depth.
+00001210: 0572 1100 0000 5a09 726f 6f74 5f70 6174  .r....Z.root_pat
+00001220: 68da 0364 6972 7223 0000 005a 0a69 6e69  h..dirr#...Z.ini
+00001230: 745f 5f70 6174 6872 1200 0000 7212 0000  t__pathr....r...
+00001240: 0072 1300 0000 5a18 5f5f 6765 6e65 7261  .r....Z.__genera
+00001250: 7465 5f64 6570 735f 696e 5f64 6570 7468  te_deps_in_depth
+00001260: 8e00 0000 731c 0000 000e 0414 0102 010e  ....s...........
+00001270: 010c 0110 020c 0102 0108 030c 010a 020a  ................
+00001280: 0202 8004 f07a 294d 6f64 756c 6552 6570  .....z)ModuleRep
+00001290: 6f73 6974 6f72 792e 5f5f 6765 6e65 7261  ository.__genera
+000012a0: 7465 5f64 6570 735f 696e 5f64 6570 7468  te_deps_in_depth
+000012b0: 6301 0000 0000 0000 0000 0000 0011 0000  c...............
+000012c0: 000b 0000 000f 0000 0073 bc03 0000 7c00  .........s....|.
+000012d0: a000 a100 0100 7c00 a001 a100 7d03 6700  ......|.....}.g.
+000012e0: 7d04 7c03 a002 a100 4400 5d2b 5c02 8900  }.|.....D.]+\...
+000012f0: 7d05 7403 7c05 8301 7401 7500 7225 7c04  }.t.|...t.u.r%|.
+00001300: a004 8700 6601 6401 6402 8408 7c05 4400  ....f.d.d...|.D.
+00001310: 8301 a101 0100 710e 7403 7c05 8301 7405  ......q.t.|...t.
+00001320: 7500 7239 7c04 a004 8700 6601 6403 6402  u.r9|.....f.d.d.
+00001330: 8408 7c05 a006 a100 4400 8301 a101 0100  ..|.....D.......
+00001340: 710e 6404 6402 8400 7c04 4400 8301 7d04  q.d.d...|.D...}.
+00001350: 7407 8300 7d06 7c06 a008 6405 a101 6406  t...}.|...d...d.
+00001360: 1900 7d07 7c06 a008 6405 a101 6407 1900  ..}.|...d...d...
+00001370: 7d08 7c04 4400 5d47 7d09 7c06 9b00 7c00  }.|.D.]G}.|...|.
+00001380: 6a09 6a0a 9b00 6405 7c09 6408 1900 9b00  j.j...d.|.d.....
+00001390: 6405 7c09 6409 1900 9b00 9d06 7c09 640a  d.|.d.......|.d.
+000013a0: 3c00 7c07 9b00 6405 7c08 9b00 6405 7c00  <.|...d.|...d.|.
+000013b0: 6a09 6a0a 9b00 6405 7c09 6408 1900 9b00  j.j...d.|.d.....
+000013c0: 6405 7c09 6409 1900 9b00 9d09 7c09 640b  d.|.d.......|.d.
+000013d0: 3c00 7c08 7c00 6a09 6a0a 6b02 729b 7c07  <.|.|.j.j.k.r.|.
+000013e0: 9b00 6405 7c08 9b00 6405 7c09 6408 1900  ..d.|...d.|.d...
+000013f0: 9b00 6405 7c09 6409 1900 9b00 9d07 7c09  ..d.|.d.......|.
+00001400: 640b 3c00 7154 7c04 4400 5d89 7d09 740b  d.<.qT|.D.].}.t.
+00001410: 6a0c a00d 7c00 6a09 6a0a 7c09 6408 1900  j...|.j.j.|.d...
+00001420: 7c09 6409 1900 640c a104 7d0a 740b 6a0c  |.d...d...}.t.j.
+00001430: a00d 7c00 6a09 6a0a 7c09 6408 1900 7c09  ..|.j.j.|.d...|.
+00001440: 6409 1900 640d a104 7d0b 740b 6a0c a00e  d...d...}.t.j...
+00001450: 7c0a a101 72df 740f 7c0a 640e 8302 8f0e  |...r.t.|.d.....
+00001460: 7d0c 7c0c a010 a100 7c09 640f 3c00 5700  }.|.....|.d.<.W.
+00001470: 6400 0400 0400 8303 0100 6e08 3100 73da  d.........n.1.s.
+00001480: 7701 0100 0100 0100 5900 0100 740b 6a0c  w.......Y...t.j.
+00001490: a00e 7c0b a101 9001 7217 740f 7c0b 640e  ..|.....r.t.|.d.
+000014a0: 8302 8f23 7d0c 640f 7c09 7600 72fe 7c09  ...#}.d.|.v.r.|.
+000014b0: 640f 0500 1900 7411 a012 7c0c a101 640f  d.....t...|...d.
+000014c0: 1900 3700 0300 3c00 6e09 7411 a012 7c0c  ..7...<.n.t...|.
+000014d0: a101 640f 1900 7c09 640f 3c00 5700 6400  ..d...|.d.<.W.d.
+000014e0: 0400 0400 8303 0100 6e09 3100 9001 7312  ........n.1...s.
+000014f0: 7701 0100 0100 0100 5900 0100 640f 7c09  w.......Y...d.|.
+00001500: 7600 9001 7227 6410 6402 8400 7c09 640f  v...r'd.d...|.d.
+00001510: 1900 4400 8301 7c09 640f 3c00 719e 7c04  ..D...|.d.<.q.|.
+00001520: 7d0d 6700 7d0d 740f 6411 6412 8302 8f10  }.g.}.t.d.d.....
+00001530: 7d0c 7411 6a13 7c04 7c0c 6407 6413 8d03  }.t.j.|.|.d.d...
+00001540: 0100 5700 6400 0400 0400 8303 0100 6e09  ..W.d.........n.
+00001550: 3100 9001 7345 7701 0100 0100 0100 5900  1...sEw.......Y.
+00001560: 0100 7c04 4400 5d42 7d09 640f 7c09 7600  ..|.D.]B}.d.|.v.
+00001570: 9001 727b 6700 7d0e 7c09 640f 1900 4400  ..r{g.}.|.d...D.
+00001580: 5d0f 7d0f 6414 7c0f 7600 9001 7262 9001  ].}.d.|.v...rb..
+00001590: 7159 7c0e a004 7c0f a101 0100 9001 7159  qY|...|.......qY
+000015a0: 7c0d a004 7c09 6409 1900 7c09 6408 1900  |...|.d...|.d...
+000015b0: 7c09 640b 1900 7c0e 6415 9c04 a101 0100  |.d...|.d.......
+000015c0: 9001 714c 7c0d a004 7c09 6409 1900 7c09  ..qL|...|.d...|.
+000015d0: 6408 1900 7c09 640b 1900 7c09 640f 1900  d...|.d...|.d...
+000015e0: 6415 9c04 a101 0100 9001 714c 7414 6a14  d.........qLt.j.
+000015f0: 7c0d 6416 6417 6418 6419 8d04 7d10 7414  |.d.d.d.d...}.t.
+00001600: 6a14 7c04 6416 641a 641b 641c 641d 8d05  j.|.d.d.d.d.d...
+00001610: 7d04 740f 641e 6412 8302 8f0d 7d0c 7c0c  }.t.d.d.....}.|.
+00001620: a015 7c04 a101 0100 5700 6400 0400 0400  ..|.....W.d.....
+00001630: 8303 0100 6e09 3100 9001 73b8 7701 0100  ....n.1...s.w...
+00001640: 0100 0100 5900 0100 740f 641f 6412 8302  ....Y...t.d.d...
+00001650: 8f0d 7d0c 7c0c a015 7c10 a101 0100 5700  ..}.|...|.....W.
+00001660: 6400 0400 0400 8303 0100 6e09 3100 9001  d.........n.1...
+00001670: 73d3 7701 0100 0100 0100 5900 0100 7416  s.w.......Y...t.
+00001680: 6420 8301 0100 6400 5300 2921 4e63 0100  d ....d.S.)!Nc..
+00001690: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+000016a0: 0000 1300 0000 f316 0000 0067 007c 005d  ...........g.|.]
+000016b0: 077d 0188 007c 0164 009c 0291 0271 0253  .}...|.d.....q.S
+000016c0: 00a9 0129 02da 0474 7970 65da 046e 616d  ...)...type..nam
+000016d0: 6572 1200 0000 a902 7254 0000 0072 6b00  er......rT...rk.
+000016e0: 0000 a901 da03 6b65 7972 1200 0000 7213  ......keyr....r.
+000016f0: 0000 0072 5600 0000 ae00 0000 f302 0000  ...rV...........
+00001700: 0016 007a 2d4d 6f64 756c 6552 6570 6f73  ...z-ModuleRepos
+00001710: 6974 6f72 792e 5f5f 6578 706f 7274 2e3c  itory.__export.<
+00001720: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00001730: 703e 6301 0000 0000 0000 0000 0000 0002  p>c.............
+00001740: 0000 0005 0000 0013 0000 0072 6800 0000  ...........rh...
+00001750: 7269 0000 0072 1200 0000 726c 0000 0072  ri...r....rl...r
+00001760: 6d00 0000 7212 0000 0072 1300 0000 7256  m...r....r....rV
+00001770: 0000 00b0 0000 0072 6f00 0000 6301 0000  .......ro...c...
+00001780: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00001790: 0053 0000 00f3 1a00 0000 6700 7c00 5d09  .S........g.|.].
+000017a0: 7d01 7c01 4400 5d04 7d02 7c02 9103 7106  }.|.D.].}.|...q.
+000017b0: 7102 5300 7212 0000 0072 1200 0000 a903  q.S.r....r......
+000017c0: 7254 0000 005a 0773 7562 6c69 7374 da04  rT...Z.sublist..
+000017d0: 6974 656d 7212 0000 0072 1200 0000 7213  itemr....r....r.
+000017e0: 0000 0072 5600 0000 b400 0000 f302 0000  ...rV...........
+000017f0: 001a 00fa 012f e903 0000 0072 1800 0000  ...../.....r....
+00001800: 726a 0000 0072 6b00 0000 7236 0000 00da  rj...rk...r6....
+00001810: 0973 686f 7274 5f75 726c fa10 7265 7175  .short_url..requ
+00001820: 6972 656d 656e 7473 2e74 7874 fa11 6465  irements.txt..de
+00001830: 7065 6e64 656e 6369 6573 2e6a 736f 6e72  pendencies.jsonr
+00001840: 5200 0000 da0c 6465 7065 6e64 656e 6369  R.....dependenci
+00001850: 6573 6301 0000 0000 0000 0000 0000 0002  esc.............
+00001860: 0000 0006 0000 0053 0000 00f3 1800 0000  .......S........
+00001870: 6700 7c00 5d08 7d01 7c01 a000 6400 6401  g.|.].}.|...d.d.
+00001880: a102 9102 7102 5300 2902 725b 0000 0072  ....q.S.).r[...r
+00001890: 4400 0000 a901 da07 7265 706c 6163 6529  D.......replace)
+000018a0: 0272 5400 0000 da03 6465 7072 1200 0000  .rT.....depr....
+000018b0: 7212 0000 0072 1300 0000 7256 0000 00e1  r....r....rV....
+000018c0: 0000 0073 0600 0000 0600 0c01 06ff 7a0c  ...s..........z.
+000018d0: 6578 706f 7274 732e 6a73 6f6e 7217 0000  exports.jsonr...
+000018e0: 0072 1900 0000 7a07 2d2d 6578 7472 6129  .r....z.--extra)
+000018f0: 0472 6b00 0000 726a 0000 0072 7600 0000  .rk...rj...rv...
+00001900: 7279 0000 00da 046b 6579 73da 056c 6174  ry.....keys..lat
+00001910: 6578 da05 6e65 7665 7229 03da 0768 6561  ex..never)...hea
+00001920: 6465 7273 da08 7461 626c 6566 6d74 da09  ders..tablefmt..
+00001930: 7368 6f77 696e 6465 785a 0667 6974 6875  showindexZ.githu
+00001940: 62da 0661 6c77 6179 7354 2904 7281 0000  b..alwaysT).r...
+00001950: 0072 8200 0000 7283 0000 005a 1064 6973  .r....r....Z.dis
+00001960: 6162 6c65 5f6e 756d 7061 7273 657a 0965  able_numparsez.e
+00001970: 7870 6f72 742e 6d64 7a0b 6578 706f 7274  xport.mdz.export
+00001980: 732e 7465 787a 1545 7870 6f72 7465 6420  s.texz.Exported 
+00001990: 746f 2065 7870 6f72 742e 6d64 2917 da28  to export.md)..(
+000019a0: 5f4d 6f64 756c 6552 6570 6f73 6974 6f72  _ModuleRepositor
+000019b0: 795f 5f67 656e 6572 6174 655f 7375 625f  y__generate_sub_
+000019c0: 7069 705f 7265 7173 da04 6c69 7374 da05  pip_reqs..list..
+000019d0: 6974 656d 7372 6a00 0000 da06 6170 7065  itemsrj.....appe
+000019e0: 6e64 da04 6469 6374 727e 0000 0072 0500  nd..dictr~...r..
+000019f0: 0000 da05 7370 6c69 7472 0e00 0000 7216  ....splitr....r.
+00001a00: 0000 0072 2200 0000 7223 0000 0072 2a00  ...r"...r#...r*.
+00001a10: 0000 7224 0000 0072 2b00 0000 725c 0000  ..r$...r+...r\..
+00001a20: 0072 2c00 0000 da04 6c6f 6164 722d 0000  .r,.....loadr-..
+00001a30: 00da 0874 6162 756c 6174 6572 4700 0000  ...tabulaterG...
+00001a40: 7227 0000 0029 1172 1100 0000 7238 0000  r'...).r....r8..
+00001a50: 0072 3900 0000 da07 6d6f 6475 6c65 73da  .r9.....modules.
+00001a60: 0574 6162 6c65 da05 7661 6c75 655a 0862  .table..valueZ.b
+00001a70: 6173 655f 7572 6c5a 0975 7365 725f 6e61  ase_urlZ.user_na
+00001a80: 6d65 5a09 7265 706f 5f6e 616d 6572 7200  meZ.repo_namerr.
+00001a90: 0000 7223 0000 005a 0864 6570 5f70 6174  ..r#...Z.dep_pat
+00001aa0: 6872 3200 0000 5a06 6c74 6162 6c65 5a07  hr2...Z.ltableZ.
+00001ab0: 6e65 775f 6465 7072 7d00 0000 5a0b 6c61  new_depr}...Z.la
+00001ac0: 7465 785f 7461 626c 6572 1200 0000 726d  tex_tabler....rm
+00001ad0: 0000 0072 1300 0000 5a08 5f5f 6578 706f  ...r....Z.__expo
+00001ae0: 7274 a400 0000 73c2 0000 0008 0208 0204  rt....s.........
+00001af0: 0210 020c 011a 010c 011c 0102 800e 0406  ................
+00001b00: 040e 010e 0108 0122 0402 fe02 0102 ff2a  .......".......*
+00001b10: 0502 fe02 0102 ff0c 0520 0502 fe02 0102  ......... ......
+00001b20: ff02 8008 0506 0114 0104 ff06 0314 0104  ................
+00001b30: ff0c 040c 010e 011c ff0e 020c 0108 011c  ................
+00001b40: 0112 0202 801e fc0a 0706 0106 010a ff02  ................
+00001b50: 8004 0904 0b0c 0312 011e ff08 030a 0204  ................
+00001b60: 020c 010a 0104 010e 0104 0106 0206 0106  ................
+00001b70: 0102 0104 fc08 ff04 0906 0206 0106 0106  ................
+00001b80: 0104 fc08 ff04 0b02 0102 0102 0102 0106  ................
+00001b90: fc04 0802 0102 0102 0102 0102 0106 fb0c  ................
+00001ba0: 0a0c 011e ff0c 030c 011e ff0c 047a 194d  .............z.M
+00001bb0: 6f64 756c 6552 6570 6f73 6974 6f72 792e  oduleRepository.
+00001bc0: 5f5f 6578 706f 7274 6301 0000 0000 0000  __exportc.......
+00001bd0: 0000 0000 0005 0000 0006 0000 0043 0000  .............C..
+00001be0: 0073 8a00 0000 7c00 6a00 6a01 7d01 7c00  .s....|.j.j.}.|.
+00001bf0: a002 7c01 a101 0100 7403 a004 6401 a101  ..|.....t...d...
+00001c00: 4400 5d34 7d02 7c02 a005 6401 a101 7320  D.]4}.|...d...s 
+00001c10: 7c02 a005 6402 a101 7320 7c02 7c00 6a00  |...d...s |.|.j.
+00001c20: 6a01 6b02 7221 710e 7403 6a06 a007 6401  j.k.r!q.t.j...d.
+00001c30: 7c02 a102 7d03 7403 6a06 a008 7c03 a101  |...}.t.j...|...
+00001c40: 7242 7403 6a06 a007 6401 7c02 6403 a103  rBt.j...d.|.d...
+00001c50: 7d04 7403 6a06 a009 7c04 a101 733d 710e  }.t.j...|...s=q.
+00001c60: 7c00 a00a 7c03 a101 0100 710e 6400 5300  |...|.....q.d.S.
+00001c70: 2904 4e72 4600 0000 7262 0000 0072 1b00  ).NrF...rb...r..
+00001c80: 0000 290b 720e 0000 0072 1600 0000 7265  ..).r....r....re
+00001c90: 0000 0072 2200 0000 7248 0000 0072 6300  ...r"...rH...rc.
+00001ca0: 0000 7223 0000 0072 2a00 0000 7249 0000  ..r#...r*...rI..
+00001cb0: 0072 2400 0000 7264 0000 0072 6600 0000  .r$...rd...rf...
+00001cc0: 7212 0000 0072 1200 0000 7213 0000 005a  r....r....r....Z
+00001cd0: 175f 5f67 656e 6572 6174 655f 7375 625f  .__generate_sub_
+00001ce0: 7069 705f 7265 7173 3301 0000 7322 0000  pip_reqs3...s"..
+00001cf0: 0008 020a 010e 0208 0202 ff08 0202 fe0c  ................
+00001d00: 0302 020e 010c 0110 020c 0102 010a 0102  ................
+00001d10: 8004 f37a 284d 6f64 756c 6552 6570 6f73  ...z(ModuleRepos
+00001d20: 6974 6f72 792e 5f5f 6765 6e65 7261 7465  itory.__generate
+00001d30: 5f73 7562 5f70 6970 5f72 6571 7363 0200  _sub_pip_reqsc..
+00001d40: 0000 0000 0000 0000 0000 0e00 0000 0a00  ................
+00001d50: 0000 0300 0000 736e 0200 0064 0164 0284  ......sn...d.d..
+00001d60: 0074 00a0 0188 01a1 0144 0083 017d 0264  .t.......D...}.d
+00001d70: 0364 0284 007c 0244 0083 0164 0464 0284  .d...|.D...d.d..
+00001d80: 0074 00a0 0188 01a1 0144 0083 0117 0089  .t.......D......
+00001d90: 0087 0166 0164 0564 0284 087c 0244 0083  ...f.d.d...|.D..
+00001da0: 017d 0374 0264 0664 0284 007c 0344 0083  .}.t.d.d...|.D..
+00001db0: 0183 017d 0387 0066 0164 0764 0284 087c  ...}...f.d.d...|
+00001dc0: 0344 0083 017d 0374 0383 007d 047c 0464  .D...}.t...}.|.d
+00001dd0: 0075 0072 4374 0464 0883 0101 0064 0053  .u.rCt.d.....d.S
+00001de0: 0074 0283 007d 057c 0344 005d 5d7d 067c  .t...}.|.D.]]}.|
+00001df0: 06a0 0564 09a1 0172 5071 487c 006a 066a  ...d...rPqH|.j.j
+00001e00: 0767 017c 06a0 0864 0aa1 01a2 017d 077c  .g.|...d.....}.|
+00001e10: 0764 0b19 0064 0917 007c 0764 0b3c 0067  .d...d...|.d.<.g
+00001e20: 007c 06a0 0864 0aa1 01a2 017d 0874 006a  .|...d.....}.t.j
+00001e30: 09a0 0a74 006a 096a 0b7c 078e 00a1 0172  ...t.j.j.|.....r
+00001e40: 7d64 0ca0 0b7c 0764 0064 0b85 0219 00a1  }d...|.d.d......
+00001e50: 017d 096e 1d74 006a 09a0 0a74 006a 096a  .}.n.t.j...t.j.j
+00001e60: 0b7c 088e 00a1 0172 8e7c 0864 0d19 0064  .|.....r.|.d...d
+00001e70: 0c17 007d 096e 0c7c 006a 066a 0764 0c17  ...}.n.|.j.j.d..
+00001e80: 007c 06a0 0c64 0a64 0ca1 0217 007d 097c  .|...d.d.....}.|
+00001e90: 0472 a07c 047c 0917 007d 097c 05a0 0d7c  .r.|.|...}.|...|
+00001ea0: 09a1 0101 0071 4874 0e7c 0583 0164 0d6b  .....qHt.|...d.k
+00001eb0: 0272 ae64 0053 007a 3774 006a 09a0 0b88  .r.d.S.z7t.j....
+00001ec0: 0164 0ea1 027d 0a74 006a 09a0 0a7c 0aa1  .d...}.t.j...|..
+00001ed0: 0172 e274 0f7c 0a64 0f83 028f 187d 0b74  .r.t.|.d.....}.t
+00001ee0: 10a0 117c 0ba1 017d 0a64 107c 0a76 0072  ...|...}.d.|.v.r
+00001ef0: d07c 0a64 1019 007d 0c6e 0269 007d 0c57  .|.d...}.n.i.}.W
+00001f00: 0064 0004 0004 0083 0301 006e 0831 0073  .d.........n.1.s
+00001f10: dc77 0101 0001 0001 0059 0001 006e 0269  .w.......Y...n.i
+00001f20: 007d 0c57 006e 1d04 0074 1290 0179 0201  .}.W.n...t...y..
+00001f30: 007d 0d01 007a 1074 0464 1188 019b 0064  .}...z.t.d.....d
+00001f40: 129d 0383 0101 0069 007d 0c57 0059 0064  .......i.}.W.Y.d
+00001f50: 007d 0d7e 0d6e 0564 007d 0d7e 0d77 0177  .}.~.n.d.}.~.w.w
+00001f60: 0074 0f74 006a 09a0 0b88 0164 0ea1 0264  .t.t.j.....d...d
+00001f70: 1383 028f 1f7d 0b74 137c 0583 017c 0c64  .....}.t.|...|.d
+00001f80: 149c 027d 0574 106a 147c 057c 0b64 1564  ...}.t.j.|.|.d.d
+00001f90: 168d 0301 0074 0464 1788 019b 009d 0283  .....t.d........
+00001fa0: 0101 0057 0064 0004 0004 0083 0301 0064  ...W.d.........d
+00001fb0: 0053 0031 0090 0173 3077 0101 0001 0001  .S.1...s0w......
+00001fc0: 0059 0001 0064 0053 0029 184e 6301 0000  .Y...d.S.).Nc...
+00001fd0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00001fe0: 0053 0000 0073 2200 0000 6700 7c00 5d0d  .S...s"...g.|.].
+00001ff0: 7d01 7c01 a000 6400 a101 7202 6401 7c01  }.|...d...r.d.|.
+00002000: 7601 7202 7c01 9102 7102 5300 2902 fa03  v.r.|...q.S.)...
+00002010: 2e70 7972 6200 0000 2901 da08 656e 6473  .pyrb...)...ends
+00002020: 7769 7468 a902 7254 0000 0072 3200 0000  with..rT...r2...
+00002030: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00002040: 5600 0000 4a01 0000 7302 0000 0022 007a  V...J...s....".z
+00002050: 414d 6f64 756c 6552 6570 6f73 6974 6f72  AModuleRepositor
+00002060: 792e 5f5f 6765 6e65 7261 7465 5f6d 6174  y.__generate_mat
+00002070: 655f 6465 7065 6e64 656e 6369 6573 2e3c  e_dependencies.<
+00002080: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00002090: 703e 6301 0000 0000 0000 0000 0000 0002  p>c.............
+000020a0: 0000 0006 0000 0053 0000 0072 7a00 0000  .......S...rz...
+000020b0: 2902 7290 0000 0072 4400 0000 727b 0000  ).r....rD...r{..
+000020c0: 00a9 0272 5400 0000 da04 6669 6c65 7212  ...rT.....filer.
+000020d0: 0000 0072 1200 0000 7213 0000 0072 5600  ...r....r....rV.
+000020e0: 0000 4b01 0000 725a 0000 0063 0100 0000  ..K...rZ...c....
+000020f0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00002100: 5300 0000 7318 0000 0067 007c 005d 087d  S...s....g.|.].}
+00002110: 0164 007c 0176 0172 027c 0191 0271 0253  .d.|.v.r.|...q.S
+00002120: 0029 0172 6200 0000 7212 0000 0072 9200  .).rb...r....r..
+00002130: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00002140: 0072 5600 0000 4b01 0000 7304 0000 0006  .rV...K...s.....
+00002150: 0012 0163 0100 0000 0000 0000 0000 0000  ...c............
+00002160: 0200 0000 0700 0000 1300 0000 731e 0000  ............s...
+00002170: 0067 007c 005d 0b7d 0174 0074 016a 02a0  .g.|.].}.t.t.j..
+00002180: 0388 007c 01a1 0283 0191 0271 0253 0072  ...|.......q.S.r
+00002190: 1200 0000 2904 7204 0000 0072 2200 0000  ....).r....r"...
+000021a0: 7223 0000 0072 2a00 0000 7292 0000 0029  r#...r*...r....)
+000021b0: 0172 2300 0000 7212 0000 0072 1300 0000  .r#...r....r....
+000021c0: 7256 0000 004f 0100 0073 0200 0000 1e00  rV...O...s......
+000021d0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+000021e0: 0004 0000 0053 0000 0072 7000 0000 7212  .....S...rp...r.
+000021f0: 0000 0072 1200 0000 7271 0000 0072 1200  ...r....rq...r..
+00002200: 0000 7212 0000 0072 1300 0000 7256 0000  ..r....r....rV..
+00002210: 0052 0100 0072 7300 0000 6301 0000 0000  .R...rs...c.....
+00002220: 0000 0000 0000 0001 0000 0006 0000 0013  ................
+00002230: 0000 0073 2600 0000 6700 7c00 5d0f 8900  ...s&...g.|.]...
+00002240: 7400 8700 6601 6400 6401 8408 8801 4400  t...f.d.d.....D.
+00002250: 8301 8301 7302 8800 9102 7102 5300 2902  ....s.....q.S.).
+00002260: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00002270: 0004 0000 0013 0000 0073 1400 0000 6700  .........s....g.
+00002280: 7c00 5d06 7d01 7c01 8800 7600 9102 7102  |.].}.|...v...q.
+00002290: 5300 7212 0000 0072 1200 0000 7293 0000  S.r....r....r...
+000022a0: 00a9 01da 066d 6f64 756c 6572 1200 0000  .....moduler....
+000022b0: 7213 0000 0072 5600 0000 5801 0000 7302  r....rV...X...s.
+000022c0: 0000 0014 007a 4c4d 6f64 756c 6552 6570  .....zLModuleRep
+000022d0: 6f73 6974 6f72 792e 5f5f 6765 6e65 7261  ository.__genera
+000022e0: 7465 5f6d 6174 655f 6465 7065 6e64 656e  te_mate_dependen
+000022f0: 6369 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c  cies.<locals>.<l
+00002300: 6973 7463 6f6d 703e 2e3c 6c69 7374 636f  istcomp>.<listco
+00002310: 6d70 3e29 01da 0361 6e79 2901 7254 0000  mp>)...any).rT..
+00002320: 0029 01da 0e6f 7269 6769 6e61 6c5f 6669  .)...original_fi
+00002330: 6c65 7372 9500 0000 7213 0000 0072 5600  lesr....r....rV.
+00002340: 0000 5501 0000 730c 0000 0006 0002 0214  ..U...s.........
+00002350: 0102 fd02 0106 ff7a 2c4e 6f20 6769 7420  .......z,No git 
+00002360: 7572 6c20 666f 756e 642c 2073 6b69 7070  url found, skipp
+00002370: 696e 6720 6465 7065 6e64 656e 6369 6573  ing dependencies
+00002380: 2e6a 736f 6e72 9000 0000 7246 0000 00e9  .jsonr....rF....
+00002390: ffff ffff 7274 0000 0072 0100 0000 7278  ....rt...r....rx
+000023a0: 0000 0072 5200 0000 da03 656e 767a 0e45  ...rR.....envz.E
+000023b0: 7272 6f72 2072 6561 6469 6e67 207a 202f  rror reading z /
+000023c0: 6465 7065 6e64 656e 6369 6573 2e6a 736f  dependencies.jso
+000023d0: 6e2c 2073 6b69 7070 696e 6720 656e 7672  n, skipping envr
+000023e0: 1700 0000 2902 7279 0000 0072 9a00 0000  ....).ry...r....
+000023f0: 7218 0000 0072 1900 0000 7a20 4765 6e65  r....r....z Gene
+00002400: 7261 7465 6420 6465 7065 6e64 656e 6369  rated dependenci
+00002410: 6573 2e6a 736f 6e20 666f 7220 2915 7222  es.json for ).r"
+00002420: 0000 0072 4800 0000 724d 0000 0072 0500  ...rH...rM...r..
+00002430: 0000 7227 0000 0072 9100 0000 720e 0000  ..r'...r....r...
+00002440: 0072 1600 0000 728a 0000 0072 2300 0000  .r....r....r#...
+00002450: 7224 0000 0072 2a00 0000 727c 0000 0072  r$...r*...r|...r
+00002460: 4e00 0000 725d 0000 0072 2b00 0000 722c  N...r]...r+...r,
+00002470: 0000 0072 8b00 0000 7231 0000 0072 8600  ...r....r1...r..
+00002480: 0000 722d 0000 0029 0e72 1100 0000 7223  ..r-...).r....r#
+00002490: 0000 00da 0566 696c 6573 5a10 7265 6c61  .....filesZ.rela
+000024a0: 7469 7665 5f69 6d70 6f72 7473 5a07 7572  tive_importsZ.ur
+000024b0: 6c5f 6769 74da 0464 6570 7372 9600 0000  l_git..depsr....
+000024c0: 5a05 7470 6174 685a 1273 6973 7465 725f  Z.tpathZ.sister_
+000024d0: 6d6f 6475 6c65 5f70 6174 6872 3600 0000  module_pathr6...
+000024e0: 5a09 6465 7073 5f6a 736f 6e72 3200 0000  Z.deps_jsonr2...
+000024f0: 729a 0000 0072 3400 0000 7212 0000 0029  r....r4...r....)
+00002500: 0272 9800 0000 7223 0000 0072 1300 0000  .r....r#...r....
+00002510: 5a1c 5f5f 6765 6e65 7261 7465 5f6d 6174  Z.__generate_mat
+00002520: 655f 6465 7065 6e64 656e 6369 6573 4701  e_dependenciesG.
+00002530: 0000 736e 0000 0014 0312 0108 0108 ff12  ..sn............
+00002540: 0402 020c 0104 ff0a 0402 0206 fe06 0608  ................
+00002550: 0208 0104 0106 0208 010a 0202 0114 0310  ................
+00002560: 010e 0214 0214 0214 010e 0118 0204 0208  ................
+00002570: 010c 010c 0204 0102 020e 020c 010c 010a  ................
+00002580: 0208 010a 0104 0202 801c fa02 8004 0904  ................
+00002590: 8010 0110 0110 0108 8002 fe16 040e 0110  ................
+000025a0: 0110 0124 fd7a 2d4d 6f64 756c 6552 6570  ...$.z-ModuleRep
+000025b0: 6f73 6974 6f72 792e 5f5f 6765 6e65 7261  ository.__genera
+000025c0: 7465 5f6d 6174 655f 6465 7065 6e64 656e  te_mate_dependen
+000025d0: 6369 6573 6302 0000 0000 0000 0000 0000  ciesc...........
+000025e0: 0009 0000 0006 0000 0043 0000 0073 b800  .........C...s..
+000025f0: 0000 7400 a001 7c01 a101 7d02 7400 a002  ..t...|...}.t...
+00002600: 7c02 a101 7d03 7c00 a003 7c01 a101 0100  |...}.|...|.....
+00002610: 6700 7d04 7c01 7c00 6a04 6a05 6b02 7224  g.}.|.|.j.j.k.r$
+00002620: 7400 a006 6401 7c03 6402 a103 0100 7c00  t...d.|.d.....|.
+00002630: a007 6401 a101 0100 6e1d 7400 a006 7408  ..d.....n.t...t.
+00002640: 6a09 a00a 7c01 6401 a102 7c03 6402 a103  j...|.d...|.d...
+00002650: 0100 7c00 a007 7408 6a09 a00a 7c01 6401  ..|...t.j...|.d.
+00002660: a102 a101 0100 740b 6403 7c01 9b00 9d02  ......t.d.|.....
+00002670: 8301 0100 7c03 4400 5d14 7d05 7c05 6404  ....|.D.].}.|.d.
+00002680: 1900 7d06 7c05 6405 1900 7d07 7c06 7c07  ..}.|.d...}.|.|.
+00002690: 6406 9c02 7d08 7c04 a00c 7c08 a101 0100  d...}.|...|.....
+000026a0: 7143 6407 7c04 6901 5300 2908 4e72 7700  qCd.|.i.S.).Nrw.
+000026b0: 0000 7a02 7e3d 7a1f 4765 6e65 7261 7465  ..z.~=z.Generate
+000026c0: 6420 7265 7175 6972 656d 656e 7473 2e74  d requirements.t
+000026d0: 7874 2066 6f72 2072 6b00 0000 da07 7665  xt for rk.....ve
+000026e0: 7273 696f 6e29 0272 6b00 0000 729d 0000  rsion).rk...r...
+000026f0: 00da 0370 6970 290d 7208 0000 005a 0f67  ...pip).r....Z.g
+00002700: 6574 5f61 6c6c 5f69 6d70 6f72 7473 5a10  et_all_importsZ.
+00002710: 6765 745f 696d 706f 7274 5f6c 6f63 616c  get_import_local
+00002720: da2d 5f4d 6f64 756c 6552 6570 6f73 6974  .-_ModuleReposit
+00002730: 6f72 795f 5f67 656e 6572 6174 655f 6d61  ory__generate_ma
+00002740: 7465 5f64 6570 656e 6465 6e63 6965 7372  te_dependenciesr
+00002750: 0e00 0000 7216 0000 005a 1a67 656e 6572  ....r....Z.gener
+00002760: 6174 655f 7265 7175 6972 656d 656e 7473  ate_requirements
+00002770: 5f66 696c 65da 305f 4d6f 6475 6c65 5265  _file.0_ModuleRe
+00002780: 706f 7369 746f 7279 5f5f 6164 645f 696e  pository__add_in
+00002790: 6465 785f 7572 6c5f 746f 5f72 6571 7569  dex_url_to_requi
+000027a0: 7265 6d65 6e74 7372 2200 0000 7223 0000  rementsr"...r#..
+000027b0: 0072 2a00 0000 7227 0000 0072 8800 0000  .r*...r'...r....
+000027c0: 2909 7211 0000 0072 2300 0000 da07 696d  ).r....r#.....im
+000027d0: 706f 7274 735a 1169 6d70 6f72 745f 696e  portsZ.import_in
+000027e0: 666f 5f6c 6f63 616c 5a0b 696d 706f 7274  fo_localZ.import
+000027f0: 5f69 6e66 6f5a 0269 6d72 6b00 0000 729d  _infoZ.imrk...r.
+00002800: 0000 00da 0372 6573 7212 0000 0072 1200  .....resr....r..
+00002810: 0000 7213 0000 005a 1b5f 5f67 656e 6572  ..r....Z.__gener
+00002820: 6174 655f 7069 705f 7265 7175 6972 656d  ate_pip_requirem
+00002830: 656e 7473 9301 0000 732c 0000 000a 030a  ents....s,......
+00002840: 030a 0204 020c 0204 0106 0104 ff0c 0304  ................
+00002850: 0310 0104 ff14 030e 0108 0208 0208 0102  ................
+00002860: 0302 0106 fe0c 0508 027a 2c4d 6f64 756c  .........z,Modul
+00002870: 6552 6570 6f73 6974 6f72 792e 5f5f 6765  eRepository.__ge
+00002880: 6e65 7261 7465 5f70 6970 5f72 6571 7569  nerate_pip_requi
+00002890: 7265 6d65 6e74 7372 9600 0000 6302 0000  rementsr....c...
+000028a0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+000028b0: 0043 0000 0073 1e00 0000 7c01 6400 6b02  .C...s....|.d.k.
+000028c0: 7209 7c00 6a00 a001 a100 5300 7c00 6a00  r.|.j.....S.|.j.
+000028d0: a002 7c01 a101 5300 720d 0000 0029 0372  ..|...S.r....).r
+000028e0: 1000 0000 da07 7375 6d6d 6172 7972 8600  ......summaryr..
+000028f0: 0000 2902 7211 0000 0072 9600 0000 7212  ..).r....r....r.
+00002900: 0000 0072 1200 0000 7213 0000 0072 8600  ...r....r....r..
+00002910: 0000 ba01 0000 7306 0000 0008 010a 010c  ......s.........
+00002920: 017a 154d 6f64 756c 6552 6570 6f73 6974  .z.ModuleReposit
+00002930: 6f72 792e 6c69 7374 6301 0000 0000 0000  ory.listc.......
+00002940: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00002950: 0073 0a00 0000 7c00 6a00 a001 a100 5300  .s....|.j.....S.
+00002960: 720d 0000 0029 0272 1000 0000 72a3 0000  r....).r....r...
+00002970: 0029 0172 1100 0000 7212 0000 0072 1200  .).r....r....r..
+00002980: 0000 7213 0000 00da 1067 6574 5f6d 6174  ..r......get_mat
+00002990: 655f 7375 6d6d 6172 79bf 0100 0073 0200  e_summary....s..
+000029a0: 0000 0a01 7a21 4d6f 6475 6c65 5265 706f  ....z!ModuleRepo
+000029b0: 7369 746f 7279 2e67 6574 5f6d 6174 655f  sitory.get_mate_
+000029c0: 7375 6d6d 6172 79da 0770 6163 6b61 6765  summary..package
+000029d0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000029e0: 0003 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
+000029f0: 6a00 a001 7c01 a101 0100 6400 5300 720d  j...|.....d.S.r.
+00002a00: 0000 0029 0272 1000 0000 7237 0000 0029  ...).r....r7...)
+00002a10: 0272 1100 0000 72a5 0000 0072 1200 0000  .r....r....r....
+00002a20: 7212 0000 0072 1300 0000 7237 0000 00c2  r....r....r7....
+00002a30: 0100 0073 0200 0000 1001 7a20 4d6f 6475  ...s......z Modu
+00002a40: 6c65 5265 706f 7369 746f 7279 2e69 6e73  leRepository.ins
+00002a50: 7461 6c6c 5f70 6163 6b61 6765 2901 4672  tall_package).Fr
+00002a60: 0d00 0000 2916 da08 5f5f 6e61 6d65 5f5f  ....)...__name__
+00002a70: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00002a80: 7175 616c 6e61 6d65 5f5f da04 626f 6f6c  qualname__..bool
+00002a90: 7214 0000 00da 0c73 7461 7469 636d 6574  r......staticmet
+00002aa0: 686f 64da 0373 7472 7235 0000 0072 3a00  hod..strr5...r:.
+00002ab0: 0000 7242 0000 0072 4100 0000 7286 0000  ..rB...rA...r...
+00002ac0: 0072 6000 0000 72a0 0000 0072 6500 0000  .r`...r....re...
+00002ad0: 7240 0000 0072 8500 0000 729f 0000 0072  r@...r....r....r
+00002ae0: 6400 0000 72a4 0000 0072 0900 0000 7237  d...r....r....r7
+00002af0: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
+00002b00: 0000 7213 0000 0072 0b00 0000 1400 0000  ..r....r........
+00002b10: 7324 0000 0008 0010 0102 0710 010e 2a0e  s$............*.
+00002b20: 0410 0612 120e 0e08 1d08 1600 7f08 1008  ................
+00002b30: 1408 4c10 2708 0512 0372 0b00 0000 2916  ..L.'....r....).
+00002b40: 722c 0000 0072 2200 0000 725e 0000 0072  r,...r"...r^...r
+00002b50: 2800 0000 728c 0000 005a 0e6d 6f64 756c  (...r....Z.modul
+00002b60: 655f 6d61 6e61 6765 7272 0300 0000 5a0e  e_managerr....Z.
+00002b70: 7574 696c 732e 6578 705f 7574 696c 7204  utils.exp_utilr.
+00002b80: 0000 005a 0e75 7469 6c73 2e67 6974 5f75  ...Z.utils.git_u
+00002b90: 7469 6c72 0500 0000 5a0e 736f 7572 6365  tilr....Z.source
+00002ba0: 732e 7265 6d6f 7465 7206 0000 005a 1373  s.remoter....Z.s
+00002bb0: 6f75 7263 6573 2e6c 6f63 616c 2e6c 6f63  ources.local.loc
+00002bc0: 616c 7207 0000 0072 0800 0000 72a5 0000  alr....r....r...
+00002bd0: 0072 0900 0000 da06 7479 7069 6e67 720a  .r......typingr.
+00002be0: 0000 00da 0469 7064 6272 0b00 0000 7212  .....ipdbr....r.
+00002bf0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+00002c00: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00002c10: 731e 0000 0008 0008 0108 0108 0108 020c  s...............
+00002c20: 020c 010c 010c 010c 010c 010c 020c 0108  ................
+00002c30: 0112 03                                  ...
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/module_manager.py` & `yerbamate-0.9.22/packages/yerbamate/api/data/module_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import hashlib
 import json
 import os
 import re
 from shutil import copytree, rmtree
 import validators
-from yerbamate.mate_config import MateConfig
+
 
 from .utils.gitdir import download
 import ipdb
 
 
 class ModuleManager:
     root_path: str = ""
 
-    def __init__(self, conf: MateConfig):
+    def __init__(self, conf):
         self.conf = conf
 
         self.init_package_cache()
 
     def init_package_cache(self):
 
         folder_name = ".mate"
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/module_repository.py` & `yerbamate-0.9.22/packages/yerbamate/api/data/module_repository.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 import sys
 
 import tabulate
 
 from .module_manager import ModuleManager
 from .utils.exp_util import get_relative_imports
 from .utils.git_util import parse_url_from_git
-from ...mate_config import MateConfig
 from .sources.remote import RemoteDataSource
 from .sources.local.local import LocalDataSource
 from pipreqs import pipreqs
 
 from .package import Package
 from typing import Optional
 import ipdb
 
 
 class ModuleRepository:
-    def __init__(self, config: MateConfig, run_local_api_server: bool = False):
+    def __init__(self, config, run_local_api_server: bool = False):
         self.config = config
         self.package_manager = ModuleManager(config)
         self.remote = RemoteDataSource()
         self.local = LocalDataSource(config)
         # self.__generate_pip_requirements(self.config.project)
 
     @staticmethod
@@ -158,15 +157,16 @@
                     dir in ["trainers", "experiments", "models", "data"]
                     and self.config.project in root_path
                 ):
                     self.__generate_pip_requirements(path)
 
                 self.__generate_deps_in_depth(path)
 
-    def __export(self):
+    def __export(self, *args, **kwargs):
+
         self.__generate_sub_pip_reqs()
 
         modules = self.list()
 
         table = []
 
         for key, value in modules.items():
@@ -222,26 +222,90 @@
                     # item["module_dependencies"] = json.load(f)
 
             if "dependencies" in item:
                 item["dependencies"] = [
                     dep.replace("\n", "") for dep in item["dependencies"]
                 ]
 
+        # create latex table
+
+        # ipdb.set_trace()
+        # l_table = [t for t in table if t["type"] == "models"]
+        # remove url from table
+        ltable = table
+        # for item in ltable:
+        #     del item["url"]
+        #     for dep in item["dependencies"]:
+        #         if "--extra" in dep:
+        #             item["dependencies"].remove(dep)
+        #         # if "https" in dep:
+
+
+        # create latex table
+        # recreate table to remove url
+        ltable = []
+
+
+        with open("exports.json", "w") as f:
+            json.dump(table, f, indent=4)
+
+        for item in table:
+            # remove --extra from dep
+            if "dependencies" in item:
+                # if --extra in dep
+                new_dep = []
+                for dep in item["dependencies"]:
+                    if "--extra" in dep:
+                        continue
+                    new_dep.append(dep)
+                ltable.append(
+                    {
+                        "name": item["name"],
+                        "type": item["type"],
+                        "short_url": item["short_url"],
+                        "dependencies": new_dep,
+                    }
+                )
+            else:
+                ltable.append(
+                    {
+                        "name": item["name"],
+                        "type": item["type"],
+                        "short_url": item["short_url"],
+                        "dependencies": item["dependencies"],
+                    }
+                )
+
+        # ipdb.set_trace()
+
+        latex_table = tabulate.tabulate(
+            ltable,
+            headers="keys",
+            tablefmt="latex",
+            showindex="never"
+            # disable_numparse=False,
+        )
+
         table = tabulate.tabulate(
             table,
             headers="keys",
             tablefmt="github",
             showindex="always",
             disable_numparse=True,
         )
 
         # save table to export.md
+
         with open("export.md", "w") as f:
             f.write(table)
 
+        with open("exports.tex", "w") as f:
+            f.write(latex_table)
+
+
         print("Exported to export.md")
 
     def __generate_sub_pip_reqs(self):
 
         root_path = self.config.project
         self.__generate_deps_in_depth(root_path)
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/package.py` & `yerbamate-0.9.22/packages/yerbamate/api/data/package.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/sources/__pycache__/remote.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Oct  4 10:54:52 2022 UTC, .py size: 1077 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-00000000: 6f0d 0d0a 0000 0000 fc10 3c63 3504 0000  o.........<c5...
+00000000: 6f0d 0d0a 0000 0000 e7c6 3164 3604 0000  o.........1d6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
-00000050: e901 0000 0029 01da 0a44 6174 6153 6f75  .....)...DataSou
+00000050: e902 0000 0029 01da 0a44 6174 6153 6f75  .....)...DataSou
 00000060: 7263 6563 0000 0000 0000 0000 0000 0000  rcec............
 00000070: 0000 0000 0400 0000 0000 0000 7394 0000  ............s...
 00000080: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
 00000090: 0284 085a 0364 1964 0465 0466 0264 0564  ...Z.d.d.e.f.d.d
 000000a0: 0684 055a 0564 1964 0465 0466 0264 0764  ...Z.d.d.e.f.d.d
 000000b0: 0884 055a 0664 1964 0465 0466 0264 0964  ...Z.d.d.e.f.d.d
 000000c0: 0a84 055a 0764 1964 0465 0466 0264 0b64  ...Z.d.d.e.f.d.d
@@ -23,111 +23,112 @@
 00000160: 005f 0467 007c 005f 0567 007c 005f 0664  ._.g.|._.g.|._.d
 00000170: 0053 00a9 014e 2907 da05 7375 7065 72da  .S...N)...super.
 00000180: 085f 5f69 6e69 745f 5fda 066d 6f64 656c  .__init__..model
 00000190: 73da 0874 7261 696e 6572 73da 0864 6174  s..trainers..dat
 000001a0: 6173 6574 73da 0b65 7870 6572 696d 656e  asets..experimen
 000001b0: 7473 da08 7061 636b 6167 6573 2901 da04  ts..packages)...
 000001c0: 7365 6c66 a901 da09 5f5f 636c 6173 735f  self....__class_
-000001d0: 5fa9 00fa 472f 686f 6d65 2f61 6c2f 4769  _...G/home/al/Gi
-000001e0: 7468 7562 2f79 6572 6261 6d61 7465 2f70  thub/yerbamate/p
+000001d0: 5fa9 00fa 4e2f 686f 6d65 2f61 6c2f 4769  _...N/home/al/Gi
+000001e0: 7448 7562 2f79 6572 6261 6d61 7465 2f70  tHub/yerbamate/p
 000001f0: 6163 6b61 6765 732f 7965 7262 616d 6174  ackages/yerbamat
-00000200: 652f 7061 636b 6167 6573 2f73 6f75 7263  e/packages/sourc
-00000210: 6573 2f72 656d 6f74 652e 7079 7206 0000  es/remote.pyr...
-00000220: 0006 0000 0073 0c00 0000 0a01 0601 0601  .....s..........
-00000230: 0601 0601 0a01 7a19 5265 6d6f 7465 4461  ......z.RemoteDa
-00000240: 7461 536f 7572 6365 2e5f 5f69 6e69 745f  taSource.__init_
-00000250: 5f4e da05 7175 6572 7963 0200 0000 0000  _N..queryc......
-00000260: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
-00000270: 0000 f306 0000 007c 006a 0053 0072 0400  .......|.j.S.r..
-00000280: 0000 2901 7207 0000 00a9 0272 0c00 0000  ..).r......r....
-00000290: 7211 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-000002a0: 1000 0000 da0a 6765 745f 6d6f 6465 6c73  ......get_models
-000002b0: 0e00 0000 f302 0000 0006 017a 1b52 656d  ...........z.Rem
-000002c0: 6f74 6544 6174 6153 6f75 7263 652e 6765  oteDataSource.ge
-000002d0: 745f 6d6f 6465 6c73 6302 0000 0000 0000  t_modelsc.......
-000002e0: 0000 0000 0002 0000 0001 0000 0043 0000  .............C..
-000002f0: 0072 1200 0000 7204 0000 0029 0172 0800  .r....r....).r..
-00000300: 0000 7213 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-00000310: 0072 1000 0000 da0c 6765 745f 7472 6169  .r......get_trai
-00000320: 6e65 7273 1100 0000 7215 0000 007a 1d52  ners....r....z.R
-00000330: 656d 6f74 6544 6174 6153 6f75 7263 652e  emoteDataSource.
-00000340: 6765 745f 7472 6169 6e65 7273 6302 0000  get_trainersc...
-00000350: 0000 0000 0000 0000 0002 0000 0001 0000  ................
-00000360: 0043 0000 0072 1200 0000 7204 0000 0029  .C...r....r....)
-00000370: 0172 0900 0000 7213 0000 0072 0f00 0000  .r....r....r....
-00000380: 720f 0000 0072 1000 0000 da10 6765 745f  r....r......get_
-00000390: 6461 7461 5f6c 6f61 6465 7273 1400 0000  data_loaders....
-000003a0: 7215 0000 007a 2152 656d 6f74 6544 6174  r....z!RemoteDat
-000003b0: 6153 6f75 7263 652e 6765 745f 6461 7461  aSource.get_data
-000003c0: 5f6c 6f61 6465 7273 6302 0000 0000 0000  _loadersc.......
-000003d0: 0000 0000 0002 0000 0001 0000 0043 0000  .............C..
-000003e0: 0072 1200 0000 7204 0000 0029 0172 0a00  .r....r....).r..
-000003f0: 0000 7213 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-00000400: 0072 1000 0000 da0f 6765 745f 6578 7065  .r......get_expe
-00000410: 7269 6d65 6e74 7317 0000 0072 1500 0000  riments....r....
-00000420: 7a20 5265 6d6f 7465 4461 7461 536f 7572  z RemoteDataSour
-00000430: 6365 2e67 6574 5f65 7870 6572 696d 656e  ce.get_experimen
-00000440: 7473 6302 0000 0000 0000 0000 0000 0002  tsc.............
-00000450: 0000 0001 0000 0043 0000 0072 1200 0000  .......C...r....
-00000460: 7204 0000 0029 0172 0b00 0000 7213 0000  r....).r....r...
-00000470: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
-00000480: da0c 6765 745f 7061 636b 6167 6573 1a00  ..get_packages..
-00000490: 0000 7215 0000 007a 1d52 656d 6f74 6544  ..r....z.RemoteD
-000004a0: 6174 6153 6f75 7263 652e 6765 745f 7061  ataSource.get_pa
-000004b0: 636b 6167 6573 6302 0000 0000 0000 0000  ckagesc.........
-000004c0: 0000 0002 0000 0003 0000 0043 0000 00f3  ...........C....
-000004d0: 1000 0000 7c00 6a00 a001 7c01 a101 0100  ....|.j...|.....
-000004e0: 6400 5300 7204 0000 0029 0272 0700 0000  d.S.r....).r....
-000004f0: da06 6170 7065 6e64 2902 720c 0000 00da  ..append).r.....
-00000500: 056d 6f64 656c 720f 0000 0072 0f00 0000  .modelr....r....
-00000510: 7210 0000 00da 0961 6464 5f6d 6f64 656c  r......add_model
-00000520: 1d00 0000 f302 0000 0010 017a 1a52 656d  ...........z.Rem
-00000530: 6f74 6544 6174 6153 6f75 7263 652e 6164  oteDataSource.ad
-00000540: 645f 6d6f 6465 6c63 0200 0000 0000 0000  d_modelc........
-00000550: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-00000560: 721a 0000 0072 0400 0000 2902 7208 0000  r....r....).r...
-00000570: 0072 1b00 0000 2902 720c 0000 00da 0774  .r....).r......t
-00000580: 7261 696e 6572 720f 0000 0072 0f00 0000  rainerr....r....
-00000590: 7210 0000 00da 0b61 6464 5f74 7261 696e  r......add_train
-000005a0: 6572 2000 0000 721e 0000 007a 1c52 656d  er ...r....z.Rem
-000005b0: 6f74 6544 6174 6153 6f75 7263 652e 6164  oteDataSource.ad
-000005c0: 645f 7472 6169 6e65 7263 0200 0000 0000  d_trainerc......
-000005d0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-000005e0: 0000 721a 0000 0072 0400 0000 2902 7209  ..r....r....).r.
-000005f0: 0000 0072 1b00 0000 2902 720c 0000 00da  ...r....).r.....
-00000600: 0764 6174 6173 6574 720f 0000 0072 0f00  .datasetr....r..
-00000610: 0000 7210 0000 00da 0b61 6464 5f64 6174  ..r......add_dat
-00000620: 6173 6574 2300 0000 721e 0000 007a 1c52  aset#...r....z.R
-00000630: 656d 6f74 6544 6174 6153 6f75 7263 652e  emoteDataSource.
-00000640: 6164 645f 6461 7461 7365 7463 0200 0000  add_datasetc....
-00000650: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000660: 4300 0000 721a 0000 0072 0400 0000 2902  C...r....r....).
-00000670: 720a 0000 0072 1b00 0000 2902 720c 0000  r....r....).r...
-00000680: 00da 0a65 7870 6572 696d 656e 7472 0f00  ...experimentr..
-00000690: 0000 720f 0000 0072 1000 0000 da0e 6164  ..r....r......ad
-000006a0: 645f 6578 7065 7269 6d65 6e74 2600 0000  d_experiment&...
-000006b0: 721e 0000 007a 1f52 656d 6f74 6544 6174  r....z.RemoteDat
-000006c0: 6153 6f75 7263 652e 6164 645f 6578 7065  aSource.add_expe
-000006d0: 7269 6d65 6e74 6302 0000 0000 0000 0000  rimentc.........
-000006e0: 0000 0002 0000 0003 0000 0043 0000 0072  ...........C...r
-000006f0: 1a00 0000 7204 0000 0029 0272 0b00 0000  ....r....).r....
-00000700: 721b 0000 0029 0272 0c00 0000 da07 7061  r....).r......pa
-00000710: 636b 6167 6572 0f00 0000 720f 0000 0072  ckager....r....r
-00000720: 1000 0000 da0b 6164 645f 7061 636b 6167  ......add_packag
-00000730: 6529 0000 0072 1e00 0000 7a1c 5265 6d6f  e)...r....z.Remo
-00000740: 7465 4461 7461 536f 7572 6365 2e61 6464  teDataSource.add
-00000750: 5f70 6163 6b61 6765 7204 0000 0029 10da  _packager....)..
-00000760: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000770: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000780: 655f 5f72 0600 0000 da03 7374 7272 1400  e__r......strr..
-00000790: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
-000007a0: 0072 1900 0000 721d 0000 0072 2000 0000  .r....r....r ...
-000007b0: 7222 0000 0072 2400 0000 7226 0000 00da  r"...r$...r&....
-000007c0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 720f  .__classcell__r.
-000007d0: 0000 0072 0f00 0000 720d 0000 0072 1000  ...r....r....r..
-000007e0: 0000 7203 0000 0005 0000 0073 1800 0000  ..r........s....
-000007f0: 0800 0c01 1008 1003 1003 1003 1003 0803  ................
-00000800: 0803 0803 0803 1003 7203 0000 004e 2903  ........r....N).
-00000810: da06 736f 7572 6365 7202 0000 0072 0300  ..sourcer....r..
-00000820: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-00000830: 0072 1000 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000840: 0100 0000 7304 0000 000c 0014 04         ....s........
+00000200: 652f 6170 692f 6461 7461 2f73 6f75 7263  e/api/data/sourc
+00000210: 6573 2f72 656d 6f74 652f 7265 6d6f 7465  es/remote/remote
+00000220: 2e70 7972 0600 0000 0600 0000 730c 0000  .pyr........s...
+00000230: 000a 0106 0106 0106 0106 010a 017a 1952  .............z.R
+00000240: 656d 6f74 6544 6174 6153 6f75 7263 652e  emoteDataSource.
+00000250: 5f5f 696e 6974 5f5f 4eda 0571 7565 7279  __init__N..query
+00000260: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000270: 0001 0000 0043 0000 00f3 0600 0000 7c00  .....C........|.
+00000280: 6a00 5300 7204 0000 0029 0172 0700 0000  j.S.r....).r....
+00000290: a902 720c 0000 0072 1100 0000 720f 0000  ..r....r....r...
+000002a0: 0072 0f00 0000 7210 0000 00da 0a67 6574  .r....r......get
+000002b0: 5f6d 6f64 656c 730e 0000 00f3 0200 0000  _models.........
+000002c0: 0601 7a1b 5265 6d6f 7465 4461 7461 536f  ..z.RemoteDataSo
+000002d0: 7572 6365 2e67 6574 5f6d 6f64 656c 7363  urce.get_modelsc
+000002e0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000002f0: 0100 0000 4300 0000 7212 0000 0072 0400  ....C...r....r..
+00000300: 0000 2901 7208 0000 0072 1300 0000 720f  ..).r....r....r.
+00000310: 0000 0072 0f00 0000 7210 0000 00da 0c67  ...r....r......g
+00000320: 6574 5f74 7261 696e 6572 7311 0000 0072  et_trainers....r
+00000330: 1500 0000 7a1d 5265 6d6f 7465 4461 7461  ....z.RemoteData
+00000340: 536f 7572 6365 2e67 6574 5f74 7261 696e  Source.get_train
+00000350: 6572 7363 0200 0000 0000 0000 0000 0000  ersc............
+00000360: 0200 0000 0100 0000 4300 0000 7212 0000  ........C...r...
+00000370: 0072 0400 0000 2901 7209 0000 0072 1300  .r....).r....r..
+00000380: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00000390: 00da 1067 6574 5f64 6174 615f 6c6f 6164  ...get_data_load
+000003a0: 6572 7314 0000 0072 1500 0000 7a21 5265  ers....r....z!Re
+000003b0: 6d6f 7465 4461 7461 536f 7572 6365 2e67  moteDataSource.g
+000003c0: 6574 5f64 6174 615f 6c6f 6164 6572 7363  et_data_loadersc
+000003d0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000003e0: 0100 0000 4300 0000 7212 0000 0072 0400  ....C...r....r..
+000003f0: 0000 2901 720a 0000 0072 1300 0000 720f  ..).r....r....r.
+00000400: 0000 0072 0f00 0000 7210 0000 00da 0f67  ...r....r......g
+00000410: 6574 5f65 7870 6572 696d 656e 7473 1700  et_experiments..
+00000420: 0000 7215 0000 007a 2052 656d 6f74 6544  ..r....z RemoteD
+00000430: 6174 6153 6f75 7263 652e 6765 745f 6578  ataSource.get_ex
+00000440: 7065 7269 6d65 6e74 7363 0200 0000 0000  perimentsc......
+00000450: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
+00000460: 0000 7212 0000 0072 0400 0000 2901 720b  ..r....r....).r.
+00000470: 0000 0072 1300 0000 720f 0000 0072 0f00  ...r....r....r..
+00000480: 0000 7210 0000 00da 0c67 6574 5f70 6163  ..r......get_pac
+00000490: 6b61 6765 731a 0000 0072 1500 0000 7a1d  kages....r....z.
+000004a0: 5265 6d6f 7465 4461 7461 536f 7572 6365  RemoteDataSource
+000004b0: 2e67 6574 5f70 6163 6b61 6765 7363 0200  .get_packagesc..
+000004c0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000004d0: 0000 4300 0000 f310 0000 007c 006a 00a0  ..C........|.j..
+000004e0: 017c 01a1 0101 0064 0053 0072 0400 0000  .|.....d.S.r....
+000004f0: 2902 7207 0000 00da 0661 7070 656e 6429  ).r......append)
+00000500: 0272 0c00 0000 da05 6d6f 6465 6c72 0f00  .r......modelr..
+00000510: 0000 720f 0000 0072 1000 0000 da09 6164  ..r....r......ad
+00000520: 645f 6d6f 6465 6c1d 0000 00f3 0200 0000  d_model.........
+00000530: 1001 7a1a 5265 6d6f 7465 4461 7461 536f  ..z.RemoteDataSo
+00000540: 7572 6365 2e61 6464 5f6d 6f64 656c 6302  urce.add_modelc.
+00000550: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00000560: 0000 0043 0000 0072 1a00 0000 7204 0000  ...C...r....r...
+00000570: 0029 0272 0800 0000 721b 0000 0029 0272  .).r....r....).r
+00000580: 0c00 0000 da07 7472 6169 6e65 7272 0f00  ......trainerr..
+00000590: 0000 720f 0000 0072 1000 0000 da0b 6164  ..r....r......ad
+000005a0: 645f 7472 6169 6e65 7220 0000 0072 1e00  d_trainer ...r..
+000005b0: 0000 7a1c 5265 6d6f 7465 4461 7461 536f  ..z.RemoteDataSo
+000005c0: 7572 6365 2e61 6464 5f74 7261 696e 6572  urce.add_trainer
+000005d0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000005e0: 0003 0000 0043 0000 0072 1a00 0000 7204  .....C...r....r.
+000005f0: 0000 0029 0272 0900 0000 721b 0000 0029  ...).r....r....)
+00000600: 0272 0c00 0000 da07 6461 7461 7365 7472  .r......datasetr
+00000610: 0f00 0000 720f 0000 0072 1000 0000 da0b  ....r....r......
+00000620: 6164 645f 6461 7461 7365 7423 0000 0072  add_dataset#...r
+00000630: 1e00 0000 7a1c 5265 6d6f 7465 4461 7461  ....z.RemoteData
+00000640: 536f 7572 6365 2e61 6464 5f64 6174 6173  Source.add_datas
+00000650: 6574 6302 0000 0000 0000 0000 0000 0002  etc.............
+00000660: 0000 0003 0000 0043 0000 0072 1a00 0000  .......C...r....
+00000670: 7204 0000 0029 0272 0a00 0000 721b 0000  r....).r....r...
+00000680: 0029 0272 0c00 0000 da0a 6578 7065 7269  .).r......experi
+00000690: 6d65 6e74 720f 0000 0072 0f00 0000 7210  mentr....r....r.
+000006a0: 0000 00da 0e61 6464 5f65 7870 6572 696d  .....add_experim
+000006b0: 656e 7426 0000 0072 1e00 0000 7a1f 5265  ent&...r....z.Re
+000006c0: 6d6f 7465 4461 7461 536f 7572 6365 2e61  moteDataSource.a
+000006d0: 6464 5f65 7870 6572 696d 656e 7463 0200  dd_experimentc..
+000006e0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000006f0: 0000 4300 0000 721a 0000 0072 0400 0000  ..C...r....r....
+00000700: 2902 720b 0000 0072 1b00 0000 2902 720c  ).r....r....).r.
+00000710: 0000 00da 0770 6163 6b61 6765 720f 0000  .....packager...
+00000720: 0072 0f00 0000 7210 0000 00da 0b61 6464  .r....r......add
+00000730: 5f70 6163 6b61 6765 2900 0000 721e 0000  _package)...r...
+00000740: 007a 1c52 656d 6f74 6544 6174 6153 6f75  .z.RemoteDataSou
+00000750: 7263 652e 6164 645f 7061 636b 6167 6572  rce.add_packager
+00000760: 0400 0000 2910 da08 5f5f 6e61 6d65 5f5f  ....)...__name__
+00000770: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000780: 7175 616c 6e61 6d65 5f5f 7206 0000 00da  qualname__r.....
+00000790: 0373 7472 7214 0000 0072 1600 0000 7217  .strr....r....r.
+000007a0: 0000 0072 1800 0000 7219 0000 0072 1d00  ...r....r....r..
+000007b0: 0000 7220 0000 0072 2200 0000 7224 0000  ..r ...r"...r$..
+000007c0: 0072 2600 0000 da0d 5f5f 636c 6173 7363  .r&.....__classc
+000007d0: 656c 6c5f 5f72 0f00 0000 720f 0000 0072  ell__r....r....r
+000007e0: 0d00 0000 7210 0000 0072 0300 0000 0500  ....r....r......
+000007f0: 0000 7318 0000 0008 000c 0110 0810 0310  ..s.............
+00000800: 0310 0310 0308 0308 0308 0308 0310 0372  ...............r
+00000810: 0300 0000 4e29 03da 0673 6f75 7263 6572  ....N)...sourcer
+00000820: 0200 0000 7203 0000 0072 0f00 0000 720f  ....r....r....r.
+00000830: 0000 0072 0f00 0000 7210 0000 00da 083c  ...r....r......<
+00000840: 6d6f 6475 6c65 3e01 0000 0073 0400 0000  module>....s....
+00000850: 0c00 1404                                ....
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Feb  6 14:44:16 2023 UTC, .py size: 365 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4012 e163 6d01 0000  o.......@..cm...
+00000000: 6f0d 0d0a 0000 0000 e7c6 3164 6d01 0000  o.........1dm...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1200 0000 4700  .....@...s....G.
 00000030: 6400 6401 8400 6401 8302 5a00 6402 5300  d.d...d...Z.d.S.
 00000040: 2903 6300 0000 0000 0000 0000 0000 0000  ).c.............
 00000050: 0000 0004 0000 0040 0000 0073 6400 0000  .......@...sd...
 00000060: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
 00000070: 640f 6404 6504 6602 6405 6406 8405 5a05  d.d.e.f.d.d...Z.
@@ -11,15 +11,15 @@
 000000a0: 640f 6404 6504 6602 640b 640c 8405 5a08  d.d.e.f.d.d...Z.
 000000b0: 640f 6404 6504 6602 640d 640e 8405 5a09  d.d.e.f.d.d...Z.
 000000c0: 6403 5300 2910 da0a 4461 7461 536f 7572  d.S.)...DataSour
 000000d0: 6365 6301 0000 0000 0000 0000 0000 0001  cec.............
 000000e0: 0000 0001 0000 0043 0000 00f3 0400 0000  .......C........
 000000f0: 6400 5300 a901 4ea9 0029 01da 0473 656c  d.S...N..)...sel
 00000100: 6672 0400 0000 7204 0000 00fa 472f 686f  fr....r.....G/ho
-00000110: 6d65 2f61 6c2f 4769 7468 7562 2f79 6572  me/al/Github/yer
+00000110: 6d65 2f61 6c2f 4769 7448 7562 2f79 6572  me/al/GitHub/yer
 00000120: 6261 6d61 7465 2f70 6163 6b61 6765 732f  bamate/packages/
 00000130: 7965 7262 616d 6174 652f 6170 692f 6461  yerbamate/api/da
 00000140: 7461 2f73 6f75 7263 6573 2f73 6f75 7263  ta/sources/sourc
 00000150: 652e 7079 da08 5f5f 696e 6974 5f5f 0200  e.py..__init__..
 00000160: 0000 f302 0000 0004 017a 1344 6174 6153  .........z.DataS
 00000170: 6f75 7263 652e 5f5f 696e 6974 5f5f 4eda  ource.__init__N.
 00000180: 0571 7565 7279 6302 0000 0000 0000 0000  .queryc.........
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Feb 10 22:21:54 2023 UTC, .py size: 5486 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,330 +1,346 @@
-00000000: 6f0d 0d0a 0000 0000 82c3 e663 6e15 0000  o..........cn...
+00000000: 6f0d 0d0a 0000 0000 e7c6 3164 c515 0000  o.........1d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 0a01 0000 6400  .....@...s....d.
+00000020: 0006 0000 0040 0000 0073 0601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6400 6401 6c06  d.l.m.Z...d.d.l.
 00000060: 5a06 6403 6404 6c07 6d08 5a08 0100 6403  Z.d.d.l.m.Z...d.
-00000070: 6405 6c09 6d0a 5a0a 0100 6403 6406 6c0b  d.l.m.Z...d.d.l.
-00000080: 6d0c 5a0c 0100 650c 650d 8301 5a0e 6407  m.Z...e.e...Z.d.
-00000090: 6408 8400 5a0f 6409 6510 640a 6510 6604  d...Z.d.e.d.e.f.
-000000a0: 640b 640c 8404 5a11 6409 6510 640d 6510  d.d...Z.d.e.d.e.
-000000b0: 640e 6510 6606 640f 6410 8404 5a12 6423  d.e.f.d.d...Z.d#
-000000c0: 6412 6510 6602 6413 6414 8405 5a13 6409  d.e.f.d.d...Z.d.
-000000d0: 6510 640d 6510 6604 6415 6416 8404 5a14  e.d.e.f.d.d...Z.
-000000e0: 6417 6418 8400 5a15 6409 6510 640d 6510  d.d...Z.d.e.d.e.
-000000f0: 6604 6419 641a 8404 5a16 6409 6510 640a  f.d.d...Z.d.e.d.
-00000100: 6510 6604 641b 641c 8404 5a17 6409 6510  e.f.d.d...Z.d.e.
-00000110: 641d 6510 641e 6510 6606 641f 6420 8404  d.e.d.e.f.d.d ..
-00000120: 5a18 6409 6510 640d 6510 6604 6421 6422  Z.d.e.d.e.f.d!d"
-00000130: 8404 5a19 6401 5300 2924 e900 0000 004e  ..Z.d.S.)$.....N
-00000140: 2901 da08 4f70 7469 6f6e 616c e905 0000  )...Optional....
-00000150: 0029 01da 0a4d 6174 6543 6f6e 6669 6729  .)...MateConfig)
-00000160: 01da 0542 756e 6368 2901 da04 6f6e 6365  ...Bunch)...once
-00000170: 6300 0000 0000 0000 0000 0000 0006 0000  c...............
-00000180: 0006 0000 0043 0000 0073 b400 0000 7400  .....C...s....t.
-00000190: a001 a100 7d00 6401 7d01 6402 7d02 6403  ....}.d.}.d.}.d.
-000001a0: 7d03 6404 7d04 7c01 734d 7c02 6405 6b00  }.d.}.|.sM|.d.k.
-000001b0: 724d 7400 6a02 a003 7400 6a02 a004 7c00  rMt.j...t.j...|.
-000001c0: 6406 a102 a101 722e 7400 6a02 a004 7c00  d.....r.t.j...|.
-000001d0: 6406 a102 7d05 7405 7c05 8301 7d04 7c04  d...}.t.|...}.|.
-000001e0: 6a06 7d03 6407 7d01 6e19 7400 a007 6408  j.}.d.}.n.t...d.
-000001f0: a101 0100 7400 a001 a100 7d00 7c02 6409  ....t.....}.|.d.
-00000200: 3700 7d02 7c00 640a 6b02 7343 7c02 6405  7.}.|.d.k.sC|.d.
-00000210: 6b02 7247 7408 640b 8301 8201 7c01 734d  k.rGt.d.....|.sM
-00000220: 7c02 6405 6b00 7312 7409 6a02 a00a 6402  |.d.k.s.t.j...d.
-00000230: 7400 a001 a100 a102 0100 7c03 7c04 6602  t.........|.|.f.
-00000240: 5300 290c 7a69 0a20 2020 204d 6574 686f  S.).zi.    Metho
-00000250: 6420 696e 2063 6861 7267 6520 6f66 2066  d in charge of f
-00000260: 696e 6469 6e67 2074 6865 2072 6f6f 7420  inding the root 
-00000270: 666f 6c64 6572 206f 6620 7468 6520 7072  folder of the pr
-00000280: 6f6a 6563 7420 616e 6420 7265 6164 696e  oject and readin
-00000290: 6720 7468 6520 636f 6e74 656e 7420 6f66  g the content of
-000002a0: 206d 6174 652e 6a73 6f6e 0a20 2020 2046   mate.json.    F
-000002b0: 7201 0000 00da 004e e902 0000 007a 096d  r......N.....z.m
-000002c0: 6174 652e 6a73 6f6e 547a 022e 2ee9 0100  ate.jsonTz......
-000002d0: 0000 fa01 2f7a 5543 6f75 6c64 206e 6f74  ..../zUCould not
-000002e0: 2066 696e 6420 6d61 7465 2e6a 736f 6e2e   find mate.json.
-000002f0: 2050 6c65 6173 6520 6d61 6b65 2073 7572   Please make sur
-00000300: 6520 796f 7520 6172 6520 696e 2074 6865  e you are in the
-00000310: 2072 6f6f 7420 666f 6c64 6572 206f 6620   root folder of 
-00000320: 7468 6520 7072 6f6a 6563 742e 290b da02  the project.)...
-00000330: 6f73 da06 6765 7463 7764 da04 7061 7468  os..getcwd..path
-00000340: da06 6578 6973 7473 da04 6a6f 696e da10  ..exists..join..
-00000350: 6c6f 6164 5f6d 6174 655f 636f 6e66 6967  load_mate_config
-00000360: da07 7072 6f6a 6563 74da 0563 6864 6972  ..project..chdir
-00000370: da09 4578 6365 7074 696f 6eda 0373 7973  ..Exception..sys
-00000380: da06 696e 7365 7274 2906 5a0c 6375 7272  ..insert).Z.curr
-00000390: 656e 745f 7061 7468 da05 666f 756e 64da  ent_path..found.
-000003a0: 0169 da0b 726f 6f74 5f66 6f6c 6465 72da  .i..root_folder.
-000003b0: 0663 6f6e 6669 675a 0963 6f6e 665f 7061  .configZ.conf_pa
-000003c0: 7468 a900 721a 0000 00fa 492f 686f 6d65  th..r.....I/home
-000003d0: 2f61 6c2f 4769 7468 7562 2f79 6572 6261  /al/Github/yerba
-000003e0: 6d61 7465 2f70 6163 6b61 6765 732f 7965  mate/packages/ye
-000003f0: 7262 616d 6174 652f 6170 692f 6461 7461  rbamate/api/data
-00000400: 2f73 6f75 7263 6573 2f6c 6f63 616c 2f69  /sources/local/i
-00000410: 6f2e 7079 da09 6669 6e64 5f72 6f6f 7411  o.py..find_root.
-00000420: 0000 0073 2a00 0000 0805 0401 0401 0401  ...s*...........
-00000430: 0401 0c01 1601 0e01 0801 0601 0602 0a02  ................
-00000440: 0801 0801 1001 0201 0201 04ff 0cf4 1211  ................
-00000450: 0801 721c 0000 0072 1800 0000 da06 666f  ..r....r......fo
-00000460: 6c64 6572 6302 0000 0000 0000 0000 0000  lderc...........
-00000470: 0002 0000 0008 0000 0043 0000 0073 3e00  .........C...s>.
-00000480: 0000 7400 6a01 a002 7400 6a01 a003 7c00  ..t.j...t.j...|.
-00000490: 7c01 a102 a101 721c 7404 6401 6402 8400  |.....r.t.d.d...
-000004a0: 7400 a005 7400 6a01 a003 7c00 7c01 a102  t...t.j...|.|...
-000004b0: a101 4400 8301 8301 5300 7404 8300 5300  ..D.....S.t...S.
-000004c0: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-000004d0: 0200 0000 0300 0000 7300 0000 731c 0000  ........s...s...
-000004e0: 0081 007c 005d 097d 0164 007c 0176 0172  ...|.].}.d.|.v.r
-000004f0: 027c 0156 0001 0071 0264 0153 0029 02da  .|.V...q.d.S.)..
-00000500: 025f 5f4e 721a 0000 00a9 02da 022e 30da  .__Nr.........0.
-00000510: 0178 721a 0000 0072 1a00 0000 721b 0000  .xr....r....r...
-00000520: 00da 093c 6765 6e65 7870 723e 3300 0000  ...<genexpr>3...
-00000530: f304 0000 0002 801a 007a 206c 6973 745f  .........z list_
-00000540: 7061 636b 6167 6573 2e3c 6c6f 6361 6c73  packages.<locals
-00000550: 3e2e 3c67 656e 6578 7072 3e29 0672 0b00  >.<genexpr>).r..
-00000560: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
-00000570: 00da 0574 7570 6c65 da07 6c69 7374 6469  ...tuple..listdi
-00000580: 72a9 0272 1800 0000 721d 0000 0072 1a00  r..r....r....r..
-00000590: 0000 721a 0000 0072 1b00 0000 da0d 6c69  ..r....r......li
-000005a0: 7374 5f70 6163 6b61 6765 7331 0000 0073  st_packages1...s
-000005b0: 0a00 0000 1403 22ff 02ff 0403 02fd 7227  ......".......r'
-000005c0: 0000 00da 0a6d 6f64 656c 5f6e 616d 65da  .....model_name.
-000005d0: 0a65 7870 6572 696d 656e 7463 0300 0000  .experimentc....
-000005e0: 0000 0000 0000 0000 0500 0000 0400 0000  ................
-000005f0: 4300 0000 735a 0000 0074 007c 007c 0164  C...sZ...t.|.|.d
-00000600: 0183 037d 037c 0344 005d 227d 047c 0464  ...}.|.D.]"}.|.d
-00000610: 0219 007c 026b 0272 1a7c 0464 0319 007c  ...|.k.r.|.d...|
-00000620: 016b 0272 1a7c 0402 0001 0053 007c 0464  .k.r.|.....S.|.d
-00000630: 0219 007c 016b 0272 2a7c 0464 0319 0064  ...|.k.r*|.d...d
-00000640: 046b 0272 2a7c 0402 0001 0053 0071 0864  .k.r*|.....S.q.d
-00000650: 0053 0029 054e 4672 0900 0000 7208 0000  .S.).NFr....r...
-00000660: 00da 0b65 7870 6572 696d 656e 7473 a901  ...experiments..
-00000670: da10 6c69 7374 5f65 7870 6572 696d 656e  ..list_experimen
-00000680: 7473 2905 7218 0000 0072 2800 0000 7229  ts).r....r(...r)
-00000690: 0000 0072 2a00 0000 da03 6578 7072 1a00  ...r*.....expr..
-000006a0: 0000 721a 0000 0072 1b00 0000 da1a 6765  ..r....r......ge
-000006b0: 745f 6578 7065 7269 6d65 6e74 5f64 6573  t_experiment_des
-000006c0: 6372 6970 7469 6f6e 3900 0000 7310 0000  cription9...s...
-000006d0: 000c 0208 0118 0108 0118 0108 0102 8004  ................
-000006e0: 0172 2e00 0000 54da 0c72 6f6f 745f 666f  .r....T..root_fo
-000006f0: 6f6c 6465 7263 0300 0000 0000 0000 0000  olderc..........
-00000700: 0000 0300 0000 0600 0000 4300 0000 7314  ..........C...s.
-00000710: 0000 0074 00a0 0174 006a 02a0 037c 0064  ...t...t.j...|.d
-00000720: 01a1 02a1 0153 0029 0261 bc03 0000 0a20  .....S.).a..... 
-00000730: 2020 206d 6f64 656c 7320 3d20 6c69 7374     models = list
-00000740: 5f70 6163 6b61 6765 7328 726f 6f74 5f66  _packages(root_f
-00000750: 6f6f 6c64 6572 2c20 226d 6f64 656c 7322  oolder, "models"
-00000760: 290a 0a20 2020 2064 6972 7320 3d20 5b0a  )..    dirs = [.
-00000770: 2020 2020 2020 2020 286f 732e 7061 7468          (os.path
-00000780: 2e6a 6f69 6e28 726f 6f74 5f66 6f6f 6c64  .join(root_foold
-00000790: 6572 2c20 2265 7870 6572 696d 656e 7473  er, "experiments
-000007a0: 2229 2c20 2265 7870 6572 696d 656e 7473  "), "experiments
-000007b0: 2229 2c0a 2020 2020 5d0a 0a20 2020 2069  "),.    ]..    i
-000007c0: 6620 6d6f 6465 6c5f 6e61 6d65 2021 3d20  f model_name != 
-000007d0: 4e6f 6e65 2061 6e64 206d 6f64 656c 5f6e  None and model_n
-000007e0: 616d 6520 696e 206d 6f64 656c 733a 0a20  ame in models:. 
-000007f0: 2020 2020 2020 206d 6f64 656c 7320 3d20         models = 
-00000800: 5b6d 6f64 656c 5f6e 616d 655d 0a20 2020  [model_name].   
-00000810: 2020 2020 2064 6972 7320 3d20 5b5d 0a0a       dirs = []..
-00000820: 2020 2020 666f 7220 6d6f 6465 6c20 696e      for model in
-00000830: 206d 6f64 656c 733a 0a20 2020 2020 2020   models:.       
-00000840: 2064 6972 732e 6170 7065 6e64 2828 6f73   dirs.append((os
-00000850: 2e70 6174 682e 6a6f 696e 2872 6f6f 745f  .path.join(root_
-00000860: 666f 6f6c 6465 722c 2022 6d6f 6465 6c73  foolder, "models
-00000870: 222c 206d 6f64 656c 2c20 2265 7870 6572  ", model, "exper
-00000880: 696d 656e 7473 2229 2c20 6d6f 6465 6c29  iments"), model)
-00000890: 290a 0a20 2020 2065 7870 6572 696d 656e  )..    experimen
-000008a0: 7473 203d 205b 5d0a 0a20 2020 2066 6f72  ts = []..    for
-000008b0: 2064 6972 2c20 6d6f 6465 6c20 696e 2064   dir, model in d
-000008c0: 6972 733a 0a20 2020 2020 2020 2069 6620  irs:.        if 
-000008d0: 6f73 2e70 6174 682e 6578 6973 7473 2864  os.path.exists(d
-000008e0: 6972 293a 0a20 2020 2020 2020 2020 2020  ir):.           
-000008f0: 2066 696c 6573 203d 206f 732e 6c69 7374   files = os.list
-00000900: 6469 7228 6469 7229 0a20 2020 2020 2020  dir(dir).       
-00000910: 2020 2020 2066 6f72 2066 696c 6520 696e       for file in
-00000920: 2066 696c 6573 3a0a 2020 2020 2020 2020   files:.        
-00000930: 2020 2020 2020 2020 6966 206e 6f74 2022          if not "
-00000940: 5f5f 2220 696e 2066 696c 6520 616e 6420  __" in file and 
-00000950: 222e 6a73 6f6e 2220 696e 2066 696c 653a  ".json" in file:
-00000960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000970: 2020 2020 2065 7870 6572 696d 656e 7473       experiments
-00000980: 2e61 7070 656e 6428 5b64 6972 2c20 6669  .append([dir, fi
-00000990: 6c65 2e72 6570 6c61 6365 2822 2e6a 736f  le.replace(".jso
-000009a0: 6e22 2c20 2222 292c 206d 6f64 656c 5d29  n", ""), model])
-000009b0: 0a0a 2020 2020 6966 206c 6f67 3a0a 2020  ..    if log:.  
-000009c0: 2020 2020 2020 666f 7220 280a 2020 2020        for (.    
-000009d0: 2020 2020 2020 2020 6469 722c 0a20 2020          dir,.   
-000009e0: 2020 2020 2020 2020 2070 6172 616d 5f66           param_f
-000009f0: 696c 652c 0a20 2020 2020 2020 2020 2020  ile,.           
-00000a00: 206d 6f64 656c 2c0a 2020 2020 2020 2020   model,.        
-00000a10: 2920 696e 2065 7870 6572 696d 656e 7473  ) in experiments
-00000a20: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00000a30: 696e 7428 6622 7b6d 6f64 656c 7d3a 207b  int(f"{model}: {
-00000a40: 6469 727d 207b 7061 7261 6d5f 6669 6c65  dir} {param_file
-00000a50: 7d22 290a 0a20 2020 2070 6174 6873 203d  }")..    paths =
-00000a60: 205b 785b 305d 2066 6f72 2078 2069 6e20   [x[0] for x in 
-00000a70: 6578 7065 7269 6d65 6e74 735d 0a20 2020  experiments].   
-00000a80: 206e 616d 6573 203d 205b 785b 315d 2066   names = [x[1] f
-00000a90: 6f72 2078 2069 6e20 6578 7065 7269 6d65  or x in experime
-00000aa0: 6e74 735d 0a20 2020 206d 6f64 656c 7320  nts].    models 
-00000ab0: 3d20 5b78 5b32 5d20 666f 7220 7820 696e  = [x[2] for x in
-00000ac0: 2065 7870 6572 696d 656e 7473 5d0a 0a20   experiments].. 
-00000ad0: 2020 2072 6574 7572 6e20 6578 7065 7269     return experi
-00000ae0: 6d65 6e74 730a 2020 2020 722a 0000 0029  ments.    r*...)
-00000af0: 0472 0b00 0000 7225 0000 0072 0d00 0000  .r....r%...r....
-00000b00: 720f 0000 0029 0372 2f00 0000 7228 0000  r....).r/...r(..
-00000b10: 00da 036c 6f67 721a 0000 0072 1a00 0000  ...logr....r....
-00000b20: 721b 0000 0072 2c00 0000 4400 0000 7302  r....r,...D...s.
-00000b30: 0000 0014 2672 2c00 0000 6302 0000 0000  ....&r,...c.....
-00000b40: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-00000b50: 0000 0073 1a00 0000 7400 7c00 6400 6401  ...s....t.|.d.d.
-00000b60: 8303 7d02 6402 6403 8400 7c02 4400 8301  ..}.d.d...|.D...
-00000b70: 5300 2904 4e46 6301 0000 0000 0000 0000  S.).NFc.........
-00000b80: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
-00000b90: 1400 0000 6700 7c00 5d06 7d01 7c01 6400  ....g.|.].}.|.d.
-00000ba0: 1900 9102 7102 5300 a901 7209 0000 0072  ....q.S...r....r
-00000bb0: 1a00 0000 721f 0000 0072 1a00 0000 721a  ....r....r....r.
-00000bc0: 0000 0072 1b00 0000 da0a 3c6c 6973 7463  ...r......<listc
-00000bd0: 6f6d 703e 6f00 0000 7302 0000 0014 007a  omp>o...s......z
-00000be0: 296c 6973 745f 6578 7065 7269 6d65 6e74  )list_experiment
-00000bf0: 5f6e 616d 6573 2e3c 6c6f 6361 6c73 3e2e  _names.<locals>.
-00000c00: 3c6c 6973 7463 6f6d 703e 722b 0000 0029  <listcomp>r+...)
-00000c10: 0372 1800 0000 7228 0000 0072 2a00 0000  .r....r(...r*...
-00000c20: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
-00000c30: 156c 6973 745f 6578 7065 7269 6d65 6e74  .list_experiment
-00000c40: 5f6e 616d 6573 6d00 0000 7304 0000 000c  _namesm...s.....
-00000c50: 010e 0172 3300 0000 6301 0000 0000 0000  ...r3...c.......
-00000c60: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
-00000c70: 0073 3c00 0000 7400 7c00 8301 8f10 7d01  .s<...t.|.....}.
-00000c80: 7401 7402 a003 7c01 a101 8301 7d02 5700  t.t...|.....}.W.
-00000c90: 6400 0400 0400 8303 0100 7c02 5300 3100  d.........|.S.1.
-00000ca0: 7317 7701 0100 0100 0100 5900 0100 7c02  s.w.......Y...|.
-00000cb0: 5300 2901 4e29 04da 046f 7065 6e72 0400  S.).N)...openr..
-00000cc0: 0000 da04 6a73 6f6e da04 6c6f 6164 2903  ....json..load).
-00000cd0: 720d 0000 00da 0166 7219 0000 0072 1a00  r......fr....r..
-00000ce0: 0000 721a 0000 0072 1b00 0000 7210 0000  ..r....r....r...
-00000cf0: 007f 0000 0073 0c00 0000 0a01 1001 0aff  .....s..........
-00000d00: 0406 10fa 0406 7210 0000 0063 0200 0000  ......r....c....
-00000d10: 0000 0000 0000 0000 0300 0000 0700 0000  ................
-00000d20: 4300 0000 7360 0000 0064 017d 027c 0264  C...s`...d.}.|.d
-00000d30: 0276 0172 1274 0064 037c 019b 0064 049d  .v.r.t.d.|...d..
-00000d40: 0383 017d 027c 0264 0276 0173 067c 0264  ...}.|.d.v.s.|.d
-00000d50: 056b 0272 2a74 01a0 0274 036a 04a0 057c  .k.r*t...t.j...|
-00000d60: 0064 067c 01a1 03a1 0101 0074 0664 077c  .d.|.......t.d.|
-00000d70: 019b 009d 0283 0101 0064 0053 0074 0664  .........d.S.t.d
-00000d80: 0883 0101 0064 0053 0029 094e da02 676f  .....d.S.).N..go
-00000d90: 2902 da01 79da 016e 7a27 4172 6520 796f  )...y..nz'Are yo
-00000da0: 7520 7375 7265 2079 6f75 2077 616e 7420  u sure you want 
-00000db0: 746f 2072 656d 6f76 6520 6d6f 6465 6c20  to remove model 
-00000dc0: 227a 0922 3f20 2879 2f6e 290a 7239 0000  "z."? (y/n).r9..
-00000dd0: 00da 066d 6f64 656c 737a 0e52 656d 6f76  ...modelsz.Remov
-00000de0: 6564 206d 6f64 656c 207a 0c4f 6b2c 2065  ed model z.Ok, e
-00000df0: 7869 7469 6e67 2e29 07da 0569 6e70 7574  xiting.)...input
-00000e00: da06 7368 7574 696c da06 726d 7472 6565  ..shutil..rmtree
-00000e10: 720b 0000 0072 0d00 0000 720f 0000 00da  r....r....r.....
-00000e20: 0570 7269 6e74 2903 7218 0000 0072 2800  .print).r....r(.
-00000e30: 0000 da06 6163 7469 6f6e 721a 0000 0072  ....actionr....r
-00000e40: 1a00 0000 721b 0000 00da 0672 656d 6f76  ....r......remov
-00000e50: 6589 0000 0073 1000 0000 0401 0801 1001  e....s..........
-00000e60: 08ff 0802 1601 1201 0c02 7241 0000 0063  ..........rA...c
-00000e70: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000e80: 0800 0000 4300 0000 7326 0000 0074 0064  ....C...s&...t.d
-00000e90: 01a0 0174 0264 0264 0384 0074 037c 007c  ...t.d.d...t.|.|
-00000ea0: 0183 0244 0083 0183 01a1 0183 0101 0064  ...D...........d
-00000eb0: 0053 0029 044e da01 0a63 0100 0000 0000  .S.).N...c......
-00000ec0: 0000 0000 0000 0200 0000 0400 0000 7300  ..............s.
-00000ed0: 0000 731c 0000 0081 007c 005d 097d 0164  ..s......|.].}.d
-00000ee0: 0074 007c 0183 0117 0056 0001 0071 0264  .t.|.....V...q.d
-00000ef0: 0153 0029 02fa 0109 4e29 01da 0373 7472  .S.)....N)...str
-00000f00: 2902 7220 0000 00da 016d 721a 0000 0072  ).r .....mr....r
-00000f10: 1a00 0000 721b 0000 0072 2200 0000 9500  ....r....r".....
-00000f20: 0000 7223 0000 007a 176c 6973 742e 3c6c  ..r#...z.list.<l
-00000f30: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
-00000f40: 2904 723f 0000 0072 0f00 0000 7224 0000  ).r?...r....r$..
-00000f50: 0072 2700 0000 7226 0000 0072 1a00 0000  .r'...r&...r....
-00000f60: 721a 0000 0072 1b00 0000 da04 6c69 7374  r....r......list
-00000f70: 9400 0000 7302 0000 0026 0172 4600 0000  ....s....&.rF...
-00000f80: da0c 736f 7572 6365 5f6d 6f64 656c da0c  ..source_model..
-00000f90: 7461 7267 6574 5f6d 6f64 656c 6303 0000  target_modelc...
-00000fa0: 0000 0000 0000 0000 0003 0000 0008 0000  ................
-00000fb0: 0043 0000 0073 2800 0000 7400 a001 7402  .C...s(...t...t.
-00000fc0: 6a03 a004 7c00 6401 7c01 a103 7402 6a03  j...|.d.|...t.j.
-00000fd0: a004 7c00 6401 7c02 a103 a102 0100 6400  ..|.d.|.......d.
-00000fe0: 5300 2902 4e72 3b00 0000 2905 723d 0000  S.).Nr;...).r=..
-00000ff0: 00da 0863 6f70 7974 7265 6572 0b00 0000  ...copytreer....
-00001000: 720d 0000 0072 0f00 0000 2903 7218 0000  r....r....).r...
-00001010: 0072 4700 0000 7248 0000 0072 1a00 0000  .rG...rH...r....
-00001020: 721a 0000 0072 1b00 0000 da05 636c 6f6e  r....r......clon
-00001030: 6598 0000 0073 0800 0000 0401 0e01 0e01  e....s..........
-00001040: 08fe 724a 0000 0063 0200 0000 0000 0000  ..rJ...c........
-00001050: 0000 0000 0600 0000 0800 0000 0300 0000  ................
-00001060: 73c4 0000 0074 006a 01a0 0274 006a 01a0  s....t.j...t.j..
-00001070: 037c 0064 01a1 02a1 0173 1574 00a0 0474  .|.d.....s.t...t
-00001080: 006a 01a0 037c 0064 01a1 02a1 0101 0064  .j...|.d.......d
-00001090: 0264 0384 0074 00a0 0574 006a 01a0 037c  .d...t...t.j...|
-000010a0: 0064 01a1 02a1 0144 0083 017d 0287 0066  .d.....D...}...f
-000010b0: 0164 0464 0384 087c 0244 0083 017d 0374  .d.d...|.D...}.t
-000010c0: 067c 0383 0164 056b 0472 3c74 0764 0664  .|...d.k.r<t.d.d
-000010d0: 0384 007c 0344 0083 0183 016e 0164 057d  ...|.D.....n.d.}
-000010e0: 0488 009b 0064 077c 0464 0817 009b 009d  .....d.|.d......
-000010f0: 037d 0574 08a0 0974 006a 01a0 037c 0064  .}.t...t.j...|.d
-00001100: 0988 00a1 0374 006a 01a0 037c 0064 017c  .....t.j...|.d.|
-00001110: 05a1 03a1 0201 0074 0a64 0a7c 059b 009d  .......t.d.|....
-00001120: 0283 0101 0064 0053 0029 0b4e 5a09 736e  .....d.S.).NZ.sn
-00001130: 6170 7368 6f74 7363 0100 0000 0000 0000  apshotsc........
-00001140: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
-00001150: 7316 0000 0067 007c 005d 077d 017c 01a0  s....g.|.].}.|..
-00001160: 0064 00a1 0191 0271 0253 0029 0172 1e00  .d.....q.S.).r..
-00001170: 0000 2901 da05 7370 6c69 74a9 0272 2000  ..)...split..r .
-00001180: 0000 da04 6e61 6d65 721a 0000 0072 1a00  ....namer....r..
-00001190: 0000 721b 0000 0072 3200 0000 a400 0000  ..r....r2.......
-000011a0: 7306 0000 0006 000a 0106 ff7a 1c73 6e61  s..........z.sna
-000011b0: 7073 686f 742e 3c6c 6f63 616c 733e 2e3c  pshot.<locals>.<
-000011c0: 6c69 7374 636f 6d70 3e63 0100 0000 0000  listcomp>c......
-000011d0: 0000 0000 0000 0200 0000 0400 0000 1300  ................
-000011e0: 0000 731c 0000 0067 007c 005d 0a7d 017c  ..s....g.|.].}.|
-000011f0: 0164 0019 0088 006b 0272 027c 0191 0271  .d.....k.r.|...q
-00001200: 0253 0029 0172 0100 0000 721a 0000 0072  .S.).r....r....r
-00001210: 4c00 0000 a901 7228 0000 0072 1a00 0000  L.....r(...r....
-00001220: 721b 0000 0072 3200 0000 a700 0000 7302  r....r2.......s.
-00001230: 0000 001c 0072 0100 0000 6301 0000 0000  .....r....c.....
-00001240: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
-00001250: 0000 0073 1800 0000 6700 7c00 5d08 7d01  ...s....g.|.].}.
-00001260: 7400 7c01 6400 1900 8301 9102 7102 5300  t.|.d.......q.S.
-00001270: 7231 0000 0029 01da 0369 6e74 724c 0000  r1...)...intrL..
-00001280: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00001290: 7232 0000 00a9 0000 0073 0200 0000 1800  r2.......s......
-000012a0: 721e 0000 0072 0900 0000 723b 0000 007a  r....r....r;...z
-000012b0: 1143 7265 6174 6564 2073 6e61 7073 686f  .Created snapsho
-000012c0: 7420 290b 720b 0000 0072 0d00 0000 720e  t ).r....r....r.
-000012d0: 0000 0072 0f00 0000 da08 6d61 6b65 6469  ...r......makedi
-000012e0: 7273 7225 0000 00da 036c 656e da03 6d61  rsr%.....len..ma
-000012f0: 7872 3d00 0000 7249 0000 0072 3f00 0000  xr=...rI...r?...
-00001300: 2906 7218 0000 0072 2800 0000 5a0e 736e  ).r....r(...Z.sn
-00001310: 6170 7368 6f74 5f6e 616d 6573 5a12 6d61  apshot_namesZ.ma
-00001320: 7463 6869 6e67 5f73 6e61 7073 686f 7473  tching_snapshots
-00001330: 5a14 6d61 785f 7665 7273 696f 6e5f 6d61  Z.max_version_ma
-00001340: 7463 6869 6e67 5a0d 736e 6170 7368 6f74  tchingZ.snapshot
-00001350: 5f6e 616d 6572 1a00 0000 724e 0000 0072  _namer....rN...r
-00001360: 1b00 0000 da08 736e 6170 7368 6f74 9f00  ......snapshot..
-00001370: 0000 7320 0000 0016 0214 0106 0212 0106  ..s ............
-00001380: ff12 030c 0312 ff02 0202 fd12 0504 020e  ................
-00001390: 010e 0104 fe12 0472 5300 0000 2902 4e54  .......rS...).NT
-000013a0: 291a 7235 0000 0072 0b00 0000 723d 0000  ).r5...r....r=..
-000013b0: 0072 1400 0000 da06 7479 7069 6e67 7202  .r......typingr.
-000013c0: 0000 00da 0469 7064 62da 0b6d 6174 655f  .....ipdb..mate_
-000013d0: 636f 6e66 6967 7204 0000 005a 0b75 7469  configr....Z.uti
-000013e0: 6c73 2e62 756e 6368 7205 0000 005a 0b75  ls.bunchr....Z.u
-000013f0: 7469 6c73 2e75 7469 6c73 7206 0000 0072  tils.utilsr....r
-00001400: 3f00 0000 5a0a 7072 696e 745f 6f6e 6365  ?...Z.print_once
-00001410: 721c 0000 0072 4400 0000 7227 0000 0072  r....rD...r'...r
-00001420: 2e00 0000 722c 0000 0072 3300 0000 7210  ....r,...r3...r.
-00001430: 0000 0072 4100 0000 7246 0000 0072 4a00  ...rA...rF...rJ.
-00001440: 0000 7253 0000 0072 1a00 0000 721a 0000  ..rS...r....r...
-00001450: 0072 1a00 0000 721b 0000 00da 083c 6d6f  .r....r......<mo
-00001460: 6475 6c65 3e01 0000 0073 2800 0000 0800  dule>....s(.....
-00001470: 0801 0801 0801 0c01 0801 0c02 0c01 0c01  ................
-00001480: 0804 0803 1220 1608 100b 1229 0812 120a  ..... .....)....
-00001490: 120b 1604 1607                           ......
+00000070: 6405 6c09 6d0a 5a0a 0100 650a 650b 8301  d.l.m.Z...e.e...
+00000080: 5a0c 6406 6407 8400 5a0d 6408 6409 8400  Z.d.d...Z.d.d...
+00000090: 5a0e 640a 650f 640b 650f 6604 640c 640d  Z.d.e.d.e.f.d.d.
+000000a0: 8404 5a10 640a 650f 640e 650f 640f 650f  ..Z.d.e.d.e.d.e.
+000000b0: 6606 6410 6411 8404 5a11 6424 6413 650f  f.d.d...Z.d$d.e.
+000000c0: 6602 6414 6415 8405 5a12 640a 650f 640e  f.d.d...Z.d.e.d.
+000000d0: 650f 6604 6416 6417 8404 5a13 6418 6419  e.f.d.d...Z.d.d.
+000000e0: 8400 5a14 640a 650f 640e 650f 6604 641a  ..Z.d.e.d.e.f.d.
+000000f0: 641b 8404 5a15 640a 650f 640b 650f 6604  d...Z.d.e.d.e.f.
+00000100: 641c 641d 8404 5a16 640a 650f 641e 650f  d.d...Z.d.e.d.e.
+00000110: 641f 650f 6606 6420 6421 8404 5a17 640a  d.e.f.d d!..Z.d.
+00000120: 650f 640e 650f 6604 6422 6423 8404 5a18  e.d.e.f.d"d#..Z.
+00000130: 6401 5300 2925 e900 0000 004e 2901 da08  d.S.)%.....N)...
+00000140: 4f70 7469 6f6e 616c e905 0000 00a9 01da  Optional........
+00000150: 0542 756e 6368 2901 da04 6f6e 6365 6300  .Bunch)...oncec.
+00000160: 0000 0000 0000 0000 0000 0006 0000 0006  ................
+00000170: 0000 0043 0000 0073 ba00 0000 7400 a001  ...C...s....t...
+00000180: a100 7d00 6401 7d01 6402 7d02 6403 7d03  ..}.d.}.d.}.d.}.
+00000190: 6404 7d04 7c01 734e 7c02 6405 6b00 724e  d.}.|.sN|.d.k.rN
+000001a0: 7400 6a02 a003 7400 6a02 a004 7c00 6406  t.j...t.j...|.d.
+000001b0: a102 a101 722f 7400 6a02 a004 7c00 6406  ....r/t.j...|.d.
+000001c0: a102 7d05 7405 7c05 8301 7d04 7c04 6407  ..}.t.|...}.|.d.
+000001d0: 1900 7d03 6408 7d01 6e19 7400 a006 6409  ..}.d.}.n.t...d.
+000001e0: a101 0100 7400 a001 a100 7d00 7c02 640a  ....t.....}.|.d.
+000001f0: 3700 7d02 7c00 640b 6b02 7344 7c02 6405  7.}.|.d.k.sD|.d.
+00000200: 6b02 7248 7407 640c 8301 8201 7c01 734e  k.rHt.d.....|.sN
+00000210: 7c02 6405 6b00 7312 7408 6a02 a009 6402  |.d.k.s.t.j...d.
+00000220: 7400 a001 a100 a102 0100 7c03 740a 7c04  t.........|.t.|.
+00000230: 8301 6602 5300 290d 7a69 0a20 2020 204d  ..f.S.).zi.    M
+00000240: 6574 686f 6420 696e 2063 6861 7267 6520  ethod in charge 
+00000250: 6f66 2066 696e 6469 6e67 2074 6865 2072  of finding the r
+00000260: 6f6f 7420 666f 6c64 6572 206f 6620 7468  oot folder of th
+00000270: 6520 7072 6f6a 6563 7420 616e 6420 7265  e project and re
+00000280: 6164 696e 6720 7468 6520 636f 6e74 656e  ading the conten
+00000290: 7420 6f66 206d 6174 652e 6a73 6f6e 0a20  t of mate.json. 
+000002a0: 2020 2046 7201 0000 00da 004e e902 0000     Fr......N....
+000002b0: 007a 096d 6174 652e 6a73 6f6e da07 7072  .z.mate.json..pr
+000002c0: 6f6a 6563 7454 7a02 2e2e e901 0000 00fa  ojectTz.........
+000002d0: 012f 7a55 436f 756c 6420 6e6f 7420 6669  ./zUCould not fi
+000002e0: 6e64 206d 6174 652e 6a73 6f6e 2e20 506c  nd mate.json. Pl
+000002f0: 6561 7365 206d 616b 6520 7375 7265 2079  ease make sure y
+00000300: 6f75 2061 7265 2069 6e20 7468 6520 726f  ou are in the ro
+00000310: 6f74 2066 6f6c 6465 7220 6f66 2074 6865  ot folder of the
+00000320: 2070 726f 6a65 6374 2e29 0bda 026f 73da   project.)...os.
+00000330: 0667 6574 6377 64da 0470 6174 68da 0665  .getcwd..path..e
+00000340: 7869 7374 73da 046a 6f69 6eda 106c 6f61  xists..join..loa
+00000350: 645f 6d61 7465 5f63 6f6e 6669 67da 0563  d_mate_config..c
+00000360: 6864 6972 da09 4578 6365 7074 696f 6eda  hdir..Exception.
+00000370: 0373 7973 da06 696e 7365 7274 7205 0000  .sys..insertr...
+00000380: 0029 065a 0c63 7572 7265 6e74 5f70 6174  .).Z.current_pat
+00000390: 68da 0566 6f75 6e64 da01 69da 0b72 6f6f  h..found..i..roo
+000003a0: 745f 666f 6c64 6572 da06 636f 6e66 6967  t_folder..config
+000003b0: 5a09 636f 6e66 5f70 6174 68a9 0072 1a00  Z.conf_path..r..
+000003c0: 0000 fa49 2f68 6f6d 652f 616c 2f47 6974  ...I/home/al/Git
+000003d0: 4875 622f 7965 7262 616d 6174 652f 7061  Hub/yerbamate/pa
+000003e0: 636b 6167 6573 2f79 6572 6261 6d61 7465  ckages/yerbamate
+000003f0: 2f61 7069 2f64 6174 612f 736f 7572 6365  /api/data/source
+00000400: 732f 6c6f 6361 6c2f 696f 2e70 79da 0966  s/local/io.py..f
+00000410: 696e 645f 726f 6f74 1000 0000 732a 0000  ind_root....s*..
+00000420: 0008 0504 0104 0104 0104 010c 0116 010e  ................
+00000430: 0108 0108 0106 020a 0208 0108 0110 0102  ................
+00000440: 0102 0104 ff0c f412 110c 0172 1c00 0000  ...........r....
+00000450: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000460: 0003 0000 0003 0000 0073 1000 0000 8700  .........s......
+00000470: 6601 6401 6402 8408 7d01 7c01 5300 2903  f.d.d...}.|.S.).
+00000480: 4e63 0000 0000 0000 0000 0000 0000 0200  Nc..............
+00000490: 0000 0500 0000 1f00 0000 7312 0000 0074  ..........s....t
+000004a0: 0088 007c 0069 007c 01a4 018e 0183 0153  ...|.i.|.......S
+000004b0: 00a9 014e 7204 0000 0029 02da 0461 7267  ...Nr....)...arg
+000004c0: 73da 066b 7761 7267 73a9 01da 0466 756e  s..kwargs....fun
+000004d0: 6372 1a00 0000 721b 0000 00da 0777 7261  cr....r......wra
+000004e0: 7070 6572 3000 0000 7302 0000 0012 017a  pper0...s......z
+000004f0: 2964 6563 6f72 6174 6f72 5f64 6963 745f  )decorator_dict_
+00000500: 746f 5f6f 626a 6563 742e 3c6c 6f63 616c  to_object.<local
+00000510: 733e 2e77 7261 7070 6572 721a 0000 0029  s>.wrapperr....)
+00000520: 0272 2100 0000 7222 0000 0072 1a00 0000  .r!...r"...r....
+00000530: 7220 0000 0072 1b00 0000 da18 6465 636f  r ...r......deco
+00000540: 7261 746f 725f 6469 6374 5f74 6f5f 6f62  rator_dict_to_ob
+00000550: 6a65 6374 2f00 0000 7304 0000 000c 0104  ject/...s.......
+00000560: 0372 2300 0000 7218 0000 00da 0666 6f6c  .r#...r......fol
+00000570: 6465 7263 0200 0000 0000 0000 0000 0000  derc............
+00000580: 0200 0000 0800 0000 4300 0000 733e 0000  ........C...s>..
+00000590: 0074 006a 01a0 0274 006a 01a0 037c 007c  .t.j...t.j...|.|
+000005a0: 01a1 02a1 0172 1c74 0464 0164 0284 0074  .....r.t.d.d...t
+000005b0: 00a0 0574 006a 01a0 037c 007c 01a1 02a1  ...t.j...|.|....
+000005c0: 0144 0083 0183 0153 0074 0483 0053 0029  .D.....S.t...S.)
+000005d0: 034e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
+000005e0: 0000 0003 0000 0073 0000 0073 1c00 0000  .......s...s....
+000005f0: 8100 7c00 5d09 7d01 6400 7c01 7601 7202  ..|.].}.d.|.v.r.
+00000600: 7c01 5600 0100 7102 6401 5300 2902 da02  |.V...q.d.S.)...
+00000610: 5f5f 4e72 1a00 0000 a902 da02 2e30 da01  __Nr.........0..
+00000620: 7872 1a00 0000 721a 0000 0072 1b00 0000  xr....r....r....
+00000630: da09 3c67 656e 6578 7072 3e38 0000 00f3  ..<genexpr>8....
+00000640: 0400 0000 0280 1a00 7a20 6c69 7374 5f70  ........z list_p
+00000650: 6163 6b61 6765 732e 3c6c 6f63 616c 733e  ackages.<locals>
+00000660: 2e3c 6765 6e65 7870 723e 2906 720c 0000  .<genexpr>).r...
+00000670: 0072 0e00 0000 720f 0000 0072 1000 0000  .r....r....r....
+00000680: da05 7475 706c 65da 076c 6973 7464 6972  ..tuple..listdir
+00000690: a902 7218 0000 0072 2400 0000 721a 0000  ..r....r$...r...
+000006a0: 0072 1a00 0000 721b 0000 00da 0d6c 6973  .r....r......lis
+000006b0: 745f 7061 636b 6167 6573 3600 0000 730a  t_packages6...s.
+000006c0: 0000 0014 0322 ff02 ff04 0302 fd72 2e00  .....".......r..
+000006d0: 0000 da0a 6d6f 6465 6c5f 6e61 6d65 da0a  ....model_name..
+000006e0: 6578 7065 7269 6d65 6e74 6303 0000 0000  experimentc.....
+000006f0: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
+00000700: 0000 0073 5a00 0000 7400 7c00 7c01 6401  ...sZ...t.|.|.d.
+00000710: 8303 7d03 7c03 4400 5d22 7d04 7c04 6402  ..}.|.D.]"}.|.d.
+00000720: 1900 7c02 6b02 721a 7c04 6403 1900 7c01  ..|.k.r.|.d...|.
+00000730: 6b02 721a 7c04 0200 0100 5300 7c04 6402  k.r.|.....S.|.d.
+00000740: 1900 7c01 6b02 722a 7c04 6403 1900 6404  ..|.k.r*|.d...d.
+00000750: 6b02 722a 7c04 0200 0100 5300 7108 6400  k.r*|.....S.q.d.
+00000760: 5300 2905 4e46 720a 0000 0072 0800 0000  S.).NFr....r....
+00000770: da0b 6578 7065 7269 6d65 6e74 73a9 01da  ..experiments...
+00000780: 106c 6973 745f 6578 7065 7269 6d65 6e74  .list_experiment
+00000790: 7329 0572 1800 0000 722f 0000 0072 3000  s).r....r/...r0.
+000007a0: 0000 7231 0000 00da 0365 7870 721a 0000  ..r1.....expr...
+000007b0: 0072 1a00 0000 721b 0000 00da 1a67 6574  .r....r......get
+000007c0: 5f65 7870 6572 696d 656e 745f 6465 7363  _experiment_desc
+000007d0: 7269 7074 696f 6e3e 0000 0073 1000 0000  ription>...s....
+000007e0: 0c02 0801 1801 0801 1801 0801 0280 0401  ................
+000007f0: 7235 0000 0054 da0c 726f 6f74 5f66 6f6f  r5...T..root_foo
+00000800: 6c64 6572 6303 0000 0000 0000 0000 0000  lderc...........
+00000810: 0003 0000 0006 0000 0043 0000 0073 1400  .........C...s..
+00000820: 0000 7400 a001 7400 6a02 a003 7c00 6401  ..t...t.j...|.d.
+00000830: a102 a101 5300 2902 61bc 0300 000a 2020  ....S.).a.....  
+00000840: 2020 6d6f 6465 6c73 203d 206c 6973 745f    models = list_
+00000850: 7061 636b 6167 6573 2872 6f6f 745f 666f  packages(root_fo
+00000860: 6f6c 6465 722c 2022 6d6f 6465 6c73 2229  older, "models")
+00000870: 0a0a 2020 2020 6469 7273 203d 205b 0a20  ..    dirs = [. 
+00000880: 2020 2020 2020 2028 6f73 2e70 6174 682e         (os.path.
+00000890: 6a6f 696e 2872 6f6f 745f 666f 6f6c 6465  join(root_foolde
+000008a0: 722c 2022 6578 7065 7269 6d65 6e74 7322  r, "experiments"
+000008b0: 292c 2022 6578 7065 7269 6d65 6e74 7322  ), "experiments"
+000008c0: 292c 0a20 2020 205d 0a0a 2020 2020 6966  ),.    ]..    if
+000008d0: 206d 6f64 656c 5f6e 616d 6520 213d 204e   model_name != N
+000008e0: 6f6e 6520 616e 6420 6d6f 6465 6c5f 6e61  one and model_na
+000008f0: 6d65 2069 6e20 6d6f 6465 6c73 3a0a 2020  me in models:.  
+00000900: 2020 2020 2020 6d6f 6465 6c73 203d 205b        models = [
+00000910: 6d6f 6465 6c5f 6e61 6d65 5d0a 2020 2020  model_name].    
+00000920: 2020 2020 6469 7273 203d 205b 5d0a 0a20      dirs = [].. 
+00000930: 2020 2066 6f72 206d 6f64 656c 2069 6e20     for model in 
+00000940: 6d6f 6465 6c73 3a0a 2020 2020 2020 2020  models:.        
+00000950: 6469 7273 2e61 7070 656e 6428 286f 732e  dirs.append((os.
+00000960: 7061 7468 2e6a 6f69 6e28 726f 6f74 5f66  path.join(root_f
+00000970: 6f6f 6c64 6572 2c20 226d 6f64 656c 7322  oolder, "models"
+00000980: 2c20 6d6f 6465 6c2c 2022 6578 7065 7269  , model, "experi
+00000990: 6d65 6e74 7322 292c 206d 6f64 656c 2929  ments"), model))
+000009a0: 0a0a 2020 2020 6578 7065 7269 6d65 6e74  ..    experiment
+000009b0: 7320 3d20 5b5d 0a0a 2020 2020 666f 7220  s = []..    for 
+000009c0: 6469 722c 206d 6f64 656c 2069 6e20 6469  dir, model in di
+000009d0: 7273 3a0a 2020 2020 2020 2020 6966 206f  rs:.        if o
+000009e0: 732e 7061 7468 2e65 7869 7374 7328 6469  s.path.exists(di
+000009f0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00000a00: 6669 6c65 7320 3d20 6f73 2e6c 6973 7464  files = os.listd
+00000a10: 6972 2864 6972 290a 2020 2020 2020 2020  ir(dir).        
+00000a20: 2020 2020 666f 7220 6669 6c65 2069 6e20      for file in 
+00000a30: 6669 6c65 733a 0a20 2020 2020 2020 2020  files:.         
+00000a40: 2020 2020 2020 2069 6620 6e6f 7420 225f         if not "_
+00000a50: 5f22 2069 6e20 6669 6c65 2061 6e64 2022  _" in file and "
+00000a60: 2e6a 736f 6e22 2069 6e20 6669 6c65 3a0a  .json" in file:.
+00000a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a80: 2020 2020 6578 7065 7269 6d65 6e74 732e      experiments.
+00000a90: 6170 7065 6e64 285b 6469 722c 2066 696c  append([dir, fil
+00000aa0: 652e 7265 706c 6163 6528 222e 6a73 6f6e  e.replace(".json
+00000ab0: 222c 2022 2229 2c20 6d6f 6465 6c5d 290a  ", ""), model]).
+00000ac0: 0a20 2020 2069 6620 6c6f 673a 0a20 2020  .    if log:.   
+00000ad0: 2020 2020 2066 6f72 2028 0a20 2020 2020       for (.     
+00000ae0: 2020 2020 2020 2064 6972 2c0a 2020 2020         dir,.    
+00000af0: 2020 2020 2020 2020 7061 7261 6d5f 6669          param_fi
+00000b00: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
+00000b10: 6d6f 6465 6c2c 0a20 2020 2020 2020 2029  model,.        )
+00000b20: 2069 6e20 6578 7065 7269 6d65 6e74 733a   in experiments:
+00000b30: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00000b40: 6e74 2866 227b 6d6f 6465 6c7d 3a20 7b64  nt(f"{model}: {d
+00000b50: 6972 7d20 7b70 6172 616d 5f66 696c 657d  ir} {param_file}
+00000b60: 2229 0a0a 2020 2020 7061 7468 7320 3d20  ")..    paths = 
+00000b70: 5b78 5b30 5d20 666f 7220 7820 696e 2065  [x[0] for x in e
+00000b80: 7870 6572 696d 656e 7473 5d0a 2020 2020  xperiments].    
+00000b90: 6e61 6d65 7320 3d20 5b78 5b31 5d20 666f  names = [x[1] fo
+00000ba0: 7220 7820 696e 2065 7870 6572 696d 656e  r x in experimen
+00000bb0: 7473 5d0a 2020 2020 6d6f 6465 6c73 203d  ts].    models =
+00000bc0: 205b 785b 325d 2066 6f72 2078 2069 6e20   [x[2] for x in 
+00000bd0: 6578 7065 7269 6d65 6e74 735d 0a0a 2020  experiments]..  
+00000be0: 2020 7265 7475 726e 2065 7870 6572 696d    return experim
+00000bf0: 656e 7473 0a20 2020 2072 3100 0000 2904  ents.    r1...).
+00000c00: 720c 0000 0072 2c00 0000 720e 0000 0072  r....r,...r....r
+00000c10: 1000 0000 2903 7236 0000 0072 2f00 0000  ....).r6...r/...
+00000c20: da03 6c6f 6772 1a00 0000 721a 0000 0072  ..logr....r....r
+00000c30: 1b00 0000 7233 0000 0049 0000 0073 0200  ....r3...I...s..
+00000c40: 0000 1426 7233 0000 0063 0200 0000 0000  ...&r3...c......
+00000c50: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
+00000c60: 0000 731a 0000 0074 007c 0064 0064 0183  ..s....t.|.d.d..
+00000c70: 037d 0264 0264 0384 007c 0244 0083 0153  .}.d.d...|.D...S
+00000c80: 0029 044e 4663 0100 0000 0000 0000 0000  .).NFc..........
+00000c90: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
+00000ca0: 0000 0067 007c 005d 067d 017c 0164 0019  ...g.|.].}.|.d..
+00000cb0: 0091 0271 0253 00a9 0172 0a00 0000 721a  ...q.S...r....r.
+00000cc0: 0000 0072 2600 0000 721a 0000 0072 1a00  ...r&...r....r..
+00000cd0: 0000 721b 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
+00000ce0: 6d70 3e74 0000 0073 0200 0000 1400 7a29  mp>t...s......z)
+00000cf0: 6c69 7374 5f65 7870 6572 696d 656e 745f  list_experiment_
+00000d00: 6e61 6d65 732e 3c6c 6f63 616c 733e 2e3c  names.<locals>.<
+00000d10: 6c69 7374 636f 6d70 3e72 3200 0000 2903  listcomp>r2...).
+00000d20: 7218 0000 0072 2f00 0000 7231 0000 0072  r....r/...r1...r
+00000d30: 1a00 0000 721a 0000 0072 1b00 0000 da15  ....r....r......
+00000d40: 6c69 7374 5f65 7870 6572 696d 656e 745f  list_experiment_
+00000d50: 6e61 6d65 7372 0000 0073 0400 0000 0c01  namesr...s......
+00000d60: 0e01 723a 0000 0063 0100 0000 0000 0000  ..r:...c........
+00000d70: 0000 0000 0300 0000 0800 0000 4300 0000  ............C...
+00000d80: 7338 0000 0074 007c 0083 018f 0e7d 0174  s8...t.|.....}.t
+00000d90: 01a0 027c 01a1 017d 0257 0064 0004 0004  ...|...}.W.d....
+00000da0: 0083 0301 007c 0253 0031 0073 1577 0101  .....|.S.1.s.w..
+00000db0: 0001 0001 0059 0001 007c 0253 0072 1d00  .....Y...|.S.r..
+00000dc0: 0000 2903 da04 6f70 656e da04 6a73 6f6e  ..)...open..json
+00000dd0: da04 6c6f 6164 2903 720e 0000 00da 0166  ..load).r......f
+00000de0: 7219 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00000df0: 1b00 0000 7211 0000 0084 0000 0073 0c00  ....r........s..
+00000e00: 0000 0a01 0c01 0aff 0409 10f7 0409 7211  ..............r.
+00000e10: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00000e20: 0300 0000 0700 0000 4300 0000 7360 0000  ........C...s`..
+00000e30: 0064 017d 027c 0264 0276 0172 1274 0064  .d.}.|.d.v.r.t.d
+00000e40: 037c 019b 0064 049d 0383 017d 027c 0264  .|...d.....}.|.d
+00000e50: 0276 0173 067c 0264 056b 0272 2a74 01a0  .v.s.|.d.k.r*t..
+00000e60: 0274 036a 04a0 057c 0064 067c 01a1 03a1  .t.j...|.d.|....
+00000e70: 0101 0074 0664 077c 019b 009d 0283 0101  ...t.d.|........
+00000e80: 0064 0053 0074 0664 0883 0101 0064 0053  .d.S.t.d.....d.S
+00000e90: 0029 094e da02 676f 2902 da01 79da 016e  .).N..go)...y..n
+00000ea0: 7a27 4172 6520 796f 7520 7375 7265 2079  z'Are you sure y
+00000eb0: 6f75 2077 616e 7420 746f 2072 656d 6f76  ou want to remov
+00000ec0: 6520 6d6f 6465 6c20 227a 0922 3f20 2879  e model "z."? (y
+00000ed0: 2f6e 290a 7240 0000 00da 066d 6f64 656c  /n).r@.....model
+00000ee0: 737a 0e52 656d 6f76 6564 206d 6f64 656c  sz.Removed model
+00000ef0: 207a 0c4f 6b2c 2065 7869 7469 6e67 2e29   z.Ok, exiting.)
+00000f00: 07da 0569 6e70 7574 da06 7368 7574 696c  ...input..shutil
+00000f10: da06 726d 7472 6565 720c 0000 0072 0e00  ..rmtreer....r..
+00000f20: 0000 7210 0000 00da 0570 7269 6e74 2903  ..r......print).
+00000f30: 7218 0000 0072 2f00 0000 da06 6163 7469  r....r/.....acti
+00000f40: 6f6e 721a 0000 0072 1a00 0000 721b 0000  onr....r....r...
+00000f50: 00da 0672 656d 6f76 6591 0000 0073 1000  ...remove....s..
+00000f60: 0000 0401 0801 1001 08ff 0802 1601 1201  ................
+00000f70: 0c02 7248 0000 0063 0200 0000 0000 0000  ..rH...c........
+00000f80: 0000 0000 0200 0000 0800 0000 4300 0000  ............C...
+00000f90: 7326 0000 0074 0064 01a0 0174 0264 0264  s&...t.d...t.d.d
+00000fa0: 0384 0074 037c 007c 0183 0244 0083 0183  ...t.|.|...D....
+00000fb0: 01a1 0183 0101 0064 0053 0029 044e da01  .......d.S.).N..
+00000fc0: 0a63 0100 0000 0000 0000 0000 0000 0200  .c..............
+00000fd0: 0000 0400 0000 7300 0000 731c 0000 0081  ......s...s.....
+00000fe0: 007c 005d 097d 0164 0074 007c 0183 0117  .|.].}.d.t.|....
+00000ff0: 0056 0001 0071 0264 0153 0029 02fa 0109  .V...q.d.S.)....
+00001000: 4e29 01da 0373 7472 2902 7227 0000 00da  N)...str).r'....
+00001010: 016d 721a 0000 0072 1a00 0000 721b 0000  .mr....r....r...
+00001020: 0072 2900 0000 9d00 0000 722a 0000 007a  .r).......r*...z
+00001030: 176c 6973 742e 3c6c 6f63 616c 733e 2e3c  .list.<locals>.<
+00001040: 6765 6e65 7870 723e 2904 7246 0000 0072  genexpr>).rF...r
+00001050: 1000 0000 722b 0000 0072 2e00 0000 722d  ....r+...r....r-
+00001060: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
+00001070: 0000 da04 6c69 7374 9c00 0000 7302 0000  ....list....s...
+00001080: 0026 0172 4d00 0000 da0c 736f 7572 6365  .&.rM.....source
+00001090: 5f6d 6f64 656c da0c 7461 7267 6574 5f6d  _model..target_m
+000010a0: 6f64 656c 6303 0000 0000 0000 0000 0000  odelc...........
+000010b0: 0003 0000 0008 0000 0043 0000 0073 2800  .........C...s(.
+000010c0: 0000 7400 a001 7402 6a03 a004 7c00 6401  ..t...t.j...|.d.
+000010d0: 7c01 a103 7402 6a03 a004 7c00 6401 7c02  |...t.j...|.d.|.
+000010e0: a103 a102 0100 6400 5300 2902 4e72 4200  ......d.S.).NrB.
+000010f0: 0000 2905 7244 0000 00da 0863 6f70 7974  ..).rD.....copyt
+00001100: 7265 6572 0c00 0000 720e 0000 0072 1000  reer....r....r..
+00001110: 0000 2903 7218 0000 0072 4e00 0000 724f  ..).r....rN...rO
+00001120: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
+00001130: 0000 da05 636c 6f6e 65a0 0000 0073 0800  ....clone....s..
+00001140: 0000 0401 0e01 0e01 08fe 7251 0000 0063  ..........rQ...c
+00001150: 0200 0000 0000 0000 0000 0000 0600 0000  ................
+00001160: 0800 0000 0300 0000 73c4 0000 0074 006a  ........s....t.j
+00001170: 01a0 0274 006a 01a0 037c 0064 01a1 02a1  ...t.j...|.d....
+00001180: 0173 1574 00a0 0474 006a 01a0 037c 0064  .s.t...t.j...|.d
+00001190: 01a1 02a1 0101 0064 0264 0384 0074 00a0  .......d.d...t..
+000011a0: 0574 006a 01a0 037c 0064 01a1 02a1 0144  .t.j...|.d.....D
+000011b0: 0083 017d 0287 0066 0164 0464 0384 087c  ...}...f.d.d...|
+000011c0: 0244 0083 017d 0374 067c 0383 0164 056b  .D...}.t.|...d.k
+000011d0: 0472 3c74 0764 0664 0384 007c 0344 0083  .r<t.d.d...|.D..
+000011e0: 0183 016e 0164 057d 0488 009b 0064 077c  ...n.d.}.....d.|
+000011f0: 0464 0817 009b 009d 037d 0574 08a0 0974  .d.......}.t...t
+00001200: 006a 01a0 037c 0064 0988 00a1 0374 006a  .j...|.d.....t.j
+00001210: 01a0 037c 0064 017c 05a1 03a1 0201 0074  ...|.d.|.......t
+00001220: 0a64 0a7c 059b 009d 0283 0101 0064 0053  .d.|.........d.S
+00001230: 0029 0b4e 5a09 736e 6170 7368 6f74 7363  .).NZ.snapshotsc
+00001240: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001250: 0500 0000 5300 0000 7316 0000 0067 007c  ....S...s....g.|
+00001260: 005d 077d 017c 01a0 0064 00a1 0191 0271  .].}.|...d.....q
+00001270: 0253 0029 0172 2500 0000 2901 da05 7370  .S.).r%...)...sp
+00001280: 6c69 74a9 0272 2700 0000 da04 6e61 6d65  lit..r'.....name
+00001290: 721a 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+000012a0: 3900 0000 ac00 0000 7306 0000 0006 000a  9.......s.......
+000012b0: 0106 ff7a 1c73 6e61 7073 686f 742e 3c6c  ...z.snapshot.<l
+000012c0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+000012d0: 3e63 0100 0000 0000 0000 0000 0000 0200  >c..............
+000012e0: 0000 0400 0000 1300 0000 731c 0000 0067  ..........s....g
+000012f0: 007c 005d 0a7d 017c 0164 0019 0088 006b  .|.].}.|.d.....k
+00001300: 0272 027c 0191 0271 0253 0029 0172 0100  .r.|...q.S.).r..
+00001310: 0000 721a 0000 0072 5300 0000 a901 722f  ..r....rS.....r/
+00001320: 0000 0072 1a00 0000 721b 0000 0072 3900  ...r....r....r9.
+00001330: 0000 af00 0000 7302 0000 001c 0072 0100  ......s......r..
+00001340: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00001350: 0000 0005 0000 0053 0000 0073 1800 0000  .......S...s....
+00001360: 6700 7c00 5d08 7d01 7400 7c01 6400 1900  g.|.].}.t.|.d...
+00001370: 8301 9102 7102 5300 7238 0000 0029 01da  ....q.S.r8...)..
+00001380: 0369 6e74 7253 0000 0072 1a00 0000 721a  .intrS...r....r.
+00001390: 0000 0072 1b00 0000 7239 0000 00b1 0000  ...r....r9......
+000013a0: 0073 0200 0000 1800 7225 0000 0072 0a00  .s......r%...r..
+000013b0: 0000 7242 0000 007a 1143 7265 6174 6564  ..rB...z.Created
+000013c0: 2073 6e61 7073 686f 7420 290b 720c 0000   snapshot ).r...
+000013d0: 0072 0e00 0000 720f 0000 0072 1000 0000  .r....r....r....
+000013e0: da08 6d61 6b65 6469 7273 722c 0000 00da  ..makedirsr,....
+000013f0: 036c 656e da03 6d61 7872 4400 0000 7250  .len..maxrD...rP
+00001400: 0000 0072 4600 0000 2906 7218 0000 0072  ...rF...).r....r
+00001410: 2f00 0000 5a0e 736e 6170 7368 6f74 5f6e  /...Z.snapshot_n
+00001420: 616d 6573 5a12 6d61 7463 6869 6e67 5f73  amesZ.matching_s
+00001430: 6e61 7073 686f 7473 5a14 6d61 785f 7665  napshotsZ.max_ve
+00001440: 7273 696f 6e5f 6d61 7463 6869 6e67 5a0d  rsion_matchingZ.
+00001450: 736e 6170 7368 6f74 5f6e 616d 6572 1a00  snapshot_namer..
+00001460: 0000 7255 0000 0072 1b00 0000 da08 736e  ..rU...r......sn
+00001470: 6170 7368 6f74 a700 0000 7320 0000 0016  apshot....s ....
+00001480: 0214 0106 0212 0106 ff12 030c 0312 ff02  ................
+00001490: 0202 fd12 0504 020e 010e 0104 fe12 0472  ...............r
+000014a0: 5a00 0000 2902 4e54 2919 723c 0000 0072  Z...).NT).r<...r
+000014b0: 0c00 0000 7244 0000 0072 1400 0000 da06  ....rD...r......
+000014c0: 7479 7069 6e67 7202 0000 00da 0469 7064  typingr......ipd
+000014d0: 625a 0b75 7469 6c73 2e62 756e 6368 7205  bZ.utils.bunchr.
+000014e0: 0000 005a 0b75 7469 6c73 2e75 7469 6c73  ...Z.utils.utils
+000014f0: 7206 0000 0072 4600 0000 5a0a 7072 696e  r....rF...Z.prin
+00001500: 745f 6f6e 6365 721c 0000 0072 2300 0000  t_oncer....r#...
+00001510: 724b 0000 0072 2e00 0000 7235 0000 0072  rK...r....r5...r
+00001520: 3300 0000 723a 0000 0072 1100 0000 7248  3...r:...r....rH
+00001530: 0000 0072 4d00 0000 7251 0000 0072 5a00  ...rM...rQ...rZ.
+00001540: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+00001550: 0072 1b00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00001560: 0100 0000 7328 0000 0008 0008 0108 0108  ....s(..........
+00001570: 010c 0108 010c 020c 0108 0408 0308 1f12  ................
+00001580: 0716 0810 0b12 2908 1212 0d12 0b16 0416  ......).........
+00001590: 07                                       .
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Feb 13 20:59:45 2023 UTC, .py size: 5184 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,364 +1,359 @@
-00000000: 6f0d 0d0a 0000 0000 c1a4 ea63 4014 0000  o..........c@...
+00000000: 6f0d 0d0a 0000 0000 e7c6 3164 0a14 0000  o.........1d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
-00000050: 6d05 5a05 0100 6404 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6406 6c08 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6401 6c09 5a09 6400 6407 6c0a 6d0b 5a0b  d.l.Z.d.d.l.m.Z.
-00000080: 0100 6400 6401 6c0c 5a0c 6404 6408 6c0d  ..d.d.l.Z.d.d.l.
-00000090: 6d0e 5a0e 0100 6400 6409 6c0a 6d0f 5a0f  m.Z...d.d.l.m.Z.
-000000a0: 0100 4700 640a 640b 8400 640b 6507 8303  ..G.d.d...d.e...
-000000b0: 5a10 6401 5300 290c e900 0000 004e 2901  Z.d.S.)......N).
-000000c0: da0a 4d61 7465 436f 6e66 6967 2901 da05  ..MateConfig)...
-000000d0: 4275 6e63 68e9 0200 0000 2901 da0a 4461  Bunch.....)...Da
-000000e0: 7461 536f 7572 6365 2901 da04 676c 6f62  taSource)...glob
-000000f0: 2901 da08 4f70 7469 6f6e 616c 2901 da02  )...Optional)...
-00000100: 696f 2901 da03 416e 7963 0000 0000 0000  io)...Anyc......
-00000110: 0000 0000 0000 0000 0000 0900 0000 0000  ................
-00000120: 0000 73d6 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00000130: 0165 0366 0287 0066 0164 0264 0384 0c5a  .e.f...f.d.d...Z
-00000140: 0464 0464 0584 005a 0564 0664 0784 005a  .d.d...Z.d.d...Z
-00000150: 0664 0865 0766 0264 0964 0a84 045a 0864  .d.e.f.d.d...Z.d
-00000160: 0b65 0965 0719 0066 0264 0c64 0d84 045a  .e.e...f.d.d...Z
-00000170: 0a64 0e65 0b65 0719 0064 0b65 0965 0719  .d.e.e...d.e.e..
-00000180: 0066 0464 0f64 1084 045a 0c64 1165 0766  .f.d.d...Z.d.e.f
-00000190: 0264 1264 1384 045a 0964 1464 1584 005a  .d.d...Z.d.d...Z
-000001a0: 0d09 1664 2964 1765 0e64 1865 0764 1965  ...d)d.e.d.e.d.e
-000001b0: 0764 1a65 0f66 0864 1b64 1c84 055a 1064  .d.e.f.d.d...Z.d
-000001c0: 1965 0766 0264 1d64 1e84 045a 1164 1f64  .e.f.d.d...Z.d.d
-000001d0: 2084 005a 1264 2164 2284 005a 1364 2364   ..Z.d!d"..Z.d#d
-000001e0: 2484 005a 1464 2564 2684 005a 1564 2764  $..Z.d%d&..Z.d'd
-000001f0: 2884 005a 1687 0004 005a 1753 0029 2ada  (..Z.....Z.S.)*.
-00000200: 0f4c 6f63 616c 4461 7461 536f 7572 6365  .LocalDataSource
-00000210: da06 636f 6e66 6967 6302 0000 0000 0000  ..configc.......
-00000220: 0000 0000 0003 0000 0003 0000 0003 0000  ................
-00000230: 0073 3000 0000 7400 8300 a001 a100 0100  .s0...t.........
-00000240: 7c01 6a02 7d02 7c02 7c00 5f03 7c01 7c00  |.j.}.|.|._.|.|.
-00000250: 5f04 6400 7c00 5f05 7c00 a006 7c02 a101  _.d.|._.|...|...
-00000260: 0100 6400 5300 a901 4e29 07da 0573 7570  ..d.S...N)...sup
-00000270: 6572 da08 5f5f 696e 6974 5f5f da07 7072  er..__init__..pr
-00000280: 6f6a 6563 74da 0b72 6f6f 745f 666f 6c64  oject..root_fold
-00000290: 6572 720b 0000 00da 036d 6170 da1b 5f4c  err......map.._L
-000002a0: 6f63 616c 4461 7461 536f 7572 6365 5f5f  ocalDataSource__
-000002b0: 6c6f 6164 5f64 6174 6129 03da 0473 656c  load_data)...sel
-000002c0: 6672 0b00 0000 da08 726f 6f74 5f64 6972  fr......root_dir
-000002d0: a901 da09 5f5f 636c 6173 735f 5fa9 00fa  ....__class__...
-000002e0: 4c2f 686f 6d65 2f61 6c2f 4769 7468 7562  L/home/al/Github
-000002f0: 2f79 6572 6261 6d61 7465 2f70 6163 6b61  /yerbamate/packa
-00000300: 6765 732f 7965 7262 616d 6174 652f 6170  ges/yerbamate/ap
-00000310: 692f 6461 7461 2f73 6f75 7263 6573 2f6c  i/data/sources/l
-00000320: 6f63 616c 2f6c 6f63 616c 2e70 7972 0e00  ocal/local.pyr..
-00000330: 0000 0f00 0000 730c 0000 000a 0506 0206  ......s.........
-00000340: 0106 0106 010e 047a 184c 6f63 616c 4461  .......z.LocalDa
-00000350: 7461 536f 7572 6365 2e5f 5f69 6e69 745f  taSource.__init_
-00000360: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-00000370: 0000 0200 0000 4300 0000 7308 0000 007c  ......C...s....|
-00000380: 00a0 00a1 0053 0072 0c00 0000 2901 da1a  .....S.r....)...
-00000390: 5f4c 6f63 616c 4461 7461 536f 7572 6365  _LocalDataSource
-000003a0: 5f5f 6669 6e64 726f 6f74 a901 7213 0000  __findroot..r...
-000003b0: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
-000003c0: da19 6c6f 6164 5f6d 6174 655f 636f 6e66  ..load_mate_conf
-000003d0: 6967 5f61 6e64 5f72 6f6f 741f 0000 0073  ig_and_root....s
-000003e0: 0200 0000 0801 7a29 4c6f 6361 6c44 6174  ......z)LocalDat
-000003f0: 6153 6f75 7263 652e 6c6f 6164 5f6d 6174  aSource.load_mat
-00000400: 655f 636f 6e66 6967 5f61 6e64 5f72 6f6f  e_config_and_roo
-00000410: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
-00000420: 0000 0300 0000 4300 0000 7312 0000 007c  ......C...s....|
-00000430: 00a0 007c 006a 01a1 0101 007c 006a 0253  ...|.j.....|.j.S
-00000440: 0072 0c00 0000 2903 7212 0000 0072 1000  .r....).r....r..
-00000450: 0000 7211 0000 0072 1a00 0000 7217 0000  ..r....r....r...
-00000460: 0072 1700 0000 7218 0000 00da 0773 756d  .r....r......sum
-00000470: 6d61 7279 2200 0000 7304 0000 000c 0106  mary"...s.......
-00000480: 017a 174c 6f63 616c 4461 7461 536f 7572  .z.LocalDataSour
-00000490: 6365 2e73 756d 6d61 7279 7214 0000 0063  ce.summaryr....c
-000004a0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000004b0: 0800 0000 0300 0000 73ba 0000 007c 006a  ........s....|.j
-000004c0: 0064 006b 0372 0764 0053 0069 007c 005f  .d.k.r.d.S.i.|._
-000004d0: 0074 01a0 0288 01a1 0144 005d 4b89 0088  .t.......D.]K...
-000004e0: 0064 016b 0272 2a87 0166 0164 0264 0384  .d.k.r*..f.d.d..
-000004f0: 0874 01a0 0274 016a 03a0 0488 0164 01a1  .t...t.j.....d..
-00000500: 02a1 0144 0083 017c 006a 0064 013c 0071  ...D...|.j.d.<.q
-00000510: 0f74 016a 03a0 0574 016a 03a0 0488 0188  .t.j...t.j......
-00000520: 00a1 02a1 0172 5a88 0064 046b 0372 5a64  .....rZ..d.k.rZd
-00000530: 0574 01a0 0274 016a 03a0 0488 0188 00a1  .t...t.j........
-00000540: 02a1 0176 0072 5a87 0087 0166 0264 0664  ...v.rZ....f.d.d
-00000550: 0784 0874 01a0 0274 016a 03a0 0488 0188  ...t...t.j......
-00000560: 00a1 02a1 0144 0083 017c 006a 0088 003c  .....D...|.j...<
-00000570: 0071 0f64 0053 0029 084e da0b 6578 7065  .q.d.S.).N..expe
-00000580: 7269 6d65 6e74 7363 0100 0000 0000 0000  rimentsc........
-00000590: 0000 0000 0200 0000 0b00 0000 1300 0000  ................
-000005a0: 735e 0000 0069 007c 005d 2b7d 0174 006a  s^...i.|.]+}.t.j
-000005b0: 01a0 0274 006a 01a0 0388 0064 007c 01a1  ...t.j.....d.|..
-000005c0: 03a1 0172 147c 0164 016b 0373 1c64 027c  ...r.|.d.k.s.d.|
-000005d0: 0176 0072 027c 0164 036b 0372 027c 0164  .v.r.|.d.k.r.|.d
-000005e0: 0464 0584 0074 00a0 0474 006a 01a0 0388  .d...t...t.j....
-000005f0: 0064 007c 01a1 03a1 0144 0083 0193 0271  .d.|.....D.....q
-00000600: 0253 0029 0672 1d00 0000 da0b 5f5f 7079  .S.).r......__py
-00000610: 6361 6368 655f 5ffa 032e 7079 fa0b 5f5f  cache__...py..__
-00000620: 696e 6974 5f5f 2e70 7963 0100 0000 0000  init__.pyc......
-00000630: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00000640: 0000 7320 0000 0067 007c 005d 0c7d 0164  ..s ...g.|.].}.d
-00000650: 007c 0176 0072 027c 0164 016b 0372 027c  .|.v.r.|.d.k.r.|
-00000660: 0191 0271 0253 0029 0272 1f00 0000 7220  ...q.S.).r....r 
-00000670: 0000 0072 1700 0000 2902 da02 2e30 5a08  ...r....)....0Z.
-00000680: 6578 705f 6669 6c65 7217 0000 0072 1700  exp_filer....r..
-00000690: 0000 7218 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
-000006a0: 6d70 3e30 0000 0073 0a00 0000 0600 0202  mp>0...s........
-000006b0: 1003 02fc 0604 7a3a 4c6f 6361 6c44 6174  ......z:LocalDat
-000006c0: 6153 6f75 7263 652e 5f5f 6c6f 6164 5f64  aSource.__load_d
-000006d0: 6174 612e 3c6c 6f63 616c 733e 2e3c 6469  ata.<locals>.<di
-000006e0: 6374 636f 6d70 3e2e 3c6c 6973 7463 6f6d  ctcomp>.<listcom
-000006f0: 703e 2905 da02 6f73 da04 7061 7468 da05  p>)...os..path..
-00000700: 6973 6469 72da 046a 6f69 6eda 076c 6973  isdir..join..lis
-00000710: 7464 6972 2902 7221 0000 00da 0364 6972  tdir).r!.....dir
-00000720: 2901 7214 0000 0072 1700 0000 7218 0000  ).r....r....r...
-00000730: 00da 0a3c 6469 6374 636f 6d70 3e2f 0000  ...<dictcomp>/..
-00000740: 0073 1800 0000 0600 0208 1601 02f7 080a  .s..............
-00000750: 1001 08f6 0402 0e01 02ff 04fe 060a 7a2f  ..............z/
-00000760: 4c6f 6361 6c44 6174 6153 6f75 7263 652e  LocalDataSource.
-00000770: 5f5f 6c6f 6164 5f64 6174 612e 3c6c 6f63  __load_data.<loc
-00000780: 616c 733e 2e3c 6469 6374 636f 6d70 3e72  als>.<dictcomp>r
-00000790: 1e00 0000 7220 0000 0063 0100 0000 0000  ....r ...c......
-000007a0: 0000 0000 0000 0200 0000 0a00 0000 1300  ................
-000007b0: 0000 734a 0000 0067 007c 005d 217d 0174  ..sJ...g.|.]!}.t
-000007c0: 006a 01a0 0274 006a 01a0 0388 0188 007c  .j...t.j.......|
-000007d0: 01a1 03a1 0172 2374 006a 01a0 0474 006a  .....r#t.j...t.j
-000007e0: 01a0 0388 0188 007c 0164 00a1 04a1 0172  .......|.d.....r
-000007f0: 237c 0164 016b 0372 027c 0191 0271 0253  #|.d.k.r.|...q.S
-00000800: 0029 0272 2000 0000 721e 0000 0029 0572  .).r ...r....).r
-00000810: 2300 0000 7224 0000 0072 2500 0000 7226  #...r$...r%...r&
-00000820: 0000 00da 0665 7869 7374 7329 0272 2100  .....exists).r!.
-00000830: 0000 5a07 7375 625f 6469 72a9 0272 2800  ..Z.sub_dir..r(.
-00000840: 0000 7214 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00000850: 0072 2200 0000 4100 0000 7316 0000 0006  .r"...A...s.....
-00000860: 0002 0216 0102 fd06 0410 0102 ff02 fc08  ................
-00000870: 0702 fa06 067a 2f4c 6f63 616c 4461 7461  .....z/LocalData
-00000880: 536f 7572 6365 2e5f 5f6c 6f61 645f 6461  Source.__load_da
-00000890: 7461 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ta.<locals>.<lis
-000008a0: 7463 6f6d 703e 2906 7211 0000 0072 2300  tcomp>).r....r#.
-000008b0: 0000 7227 0000 0072 2400 0000 7226 0000  ..r'...r$...r&..
-000008c0: 0072 2500 0000 2902 7213 0000 0072 1400  .r%...).r....r..
-000008d0: 0000 7217 0000 0072 2b00 0000 7218 0000  ..r....r+...r...
-000008e0: 005a 0b5f 5f6c 6f61 645f 6461 7461 2600  .Z.__load_data&.
-000008f0: 0000 731e 0000 000a 0204 0106 020e 0108  ..s.............
-00000900: 020a 0112 080e f81e 0f18 020c 0112 020c  ................
-00000910: fe02 8004 eb7a 1b4c 6f63 616c 4461 7461  .....z.LocalData
-00000920: 536f 7572 6365 2e5f 5f6c 6f61 645f 6461  Source.__load_da
-00000930: 7461 da05 6e61 6d65 7363 0200 0000 0000  ta..namesc......
-00000940: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
-00000950: 0000 730e 0000 0064 0164 0284 007c 0144  ..s....d.d...|.D
-00000960: 0083 0153 0029 034e 6301 0000 0000 0000  ...S.).Nc.......
-00000970: 0000 0000 0002 0000 0005 0000 0053 0000  .............S..
-00000980: 0073 1a00 0000 6700 7c00 5d09 7d01 7c01  .s....g.|.].}.|.
-00000990: a000 6400 a101 7302 7c01 9102 7102 5300  ..d...s.|...q.S.
-000009a0: 2901 da02 5f5f 2901 da0a 7374 6172 7473  )...__)...starts
-000009b0: 7769 7468 2902 7221 0000 00da 0266 6e72  with).r!.....fnr
-000009c0: 1700 0000 7217 0000 0072 1800 0000 7222  ....r....r....r"
-000009d0: 0000 004e 0000 0073 0200 0000 1a00 7a3c  ...N...s......z<
-000009e0: 4c6f 6361 6c44 6174 6153 6f75 7263 652e  LocalDataSource.
-000009f0: 5f5f 6669 6c74 6572 5f72 6567 756c 6172  __filter_regular
-00000a00: 5f66 6f6c 6465 7273 2e3c 6c6f 6361 6c73  _folders.<locals
-00000a10: 3e2e 3c6c 6973 7463 6f6d 703e 7217 0000  >.<listcomp>r...
-00000a20: 0029 0272 1300 0000 722c 0000 0072 1700  .).r....r,...r..
-00000a30: 0000 7217 0000 0072 1800 0000 5a18 5f5f  ..r....r....Z.__
-00000a40: 6669 6c74 6572 5f72 6567 756c 6172 5f66  filter_regular_f
-00000a50: 6f6c 6465 7273 4d00 0000 7302 0000 000e  oldersM...s.....
-00000a60: 017a 284c 6f63 616c 4461 7461 536f 7572  .z(LocalDataSour
-00000a70: 6365 2e5f 5f66 696c 7465 725f 7265 6775  ce.__filter_regu
-00000a80: 6c61 725f 666f 6c64 6572 73da 0571 7565  lar_folders..que
-00000a90: 7279 6303 0000 0000 0000 0000 0000 0003  ryc.............
-00000aa0: 0000 0003 0000 0003 0000 0073 1e00 0000  ...........s....
-00000ab0: 8800 6400 7500 7206 7c02 5300 8700 6601  ..d.u.r.|.S...f.
-00000ac0: 6401 6402 8408 7c02 4400 8301 5300 2903  d.d...|.D...S.).
-00000ad0: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
-00000ae0: 0000 0400 0000 1300 0000 7318 0000 0067  ..........s....g
-00000af0: 007c 005d 087d 0188 007c 016b 0272 027c  .|.].}...|.k.r.|
-00000b00: 0191 0271 0253 0072 1700 0000 7217 0000  ...q.S.r....r...
-00000b10: 0029 0272 2100 0000 da04 6e61 6d65 a901  .).r!.....name..
-00000b20: 7230 0000 0072 1700 0000 7218 0000 0072  r0...r....r....r
-00000b30: 2200 0000 5100 0000 7302 0000 0018 007a  "...Q...s......z
-00000b40: 324c 6f63 616c 4461 7461 536f 7572 6365  2LocalDataSource
-00000b50: 2e5f 5f66 696c 7465 725f 6e61 6d65 732e  .__filter_names.
-00000b60: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00000b70: 6d70 3e72 1700 0000 2903 7213 0000 0072  mp>r....).r....r
-00000b80: 3000 0000 722c 0000 0072 1700 0000 7232  0...r,...r....r2
-00000b90: 0000 0072 1800 0000 5a0e 5f5f 6669 6c74  ...r....Z.__filt
-00000ba0: 6572 5f6e 616d 6573 5000 0000 7302 0000  er_namesP...s...
-00000bb0: 001e 017a 1e4c 6f63 616c 4461 7461 536f  ...z.LocalDataSo
-00000bc0: 7572 6365 2e5f 5f66 696c 7465 725f 6e61  urce.__filter_na
-00000bd0: 6d65 73da 066d 6f64 756c 6563 0200 0000  mes..modulec....
-00000be0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000bf0: 4300 0000 7336 0000 007c 0164 0075 0072  C...s6...|.d.u.r
-00000c00: 077c 006a 0053 007c 017c 006a 00a0 01a1  .|.j.S.|.|.j....
-00000c10: 0076 0073 164a 0064 017c 019b 0064 029d  .v.s.J.d.|...d..
-00000c20: 0383 0182 017c 006a 007c 0119 0053 0029  .....|.j.|...S.)
-00000c30: 034e 7a07 4d6f 6475 6c65 207a 0a20 6e6f  .Nz.Module z. no
-00000c40: 7420 666f 756e 6429 0272 1100 0000 da04  t found).r......
-00000c50: 6b65 7973 2902 7213 0000 0072 3300 0000  keys).r....r3...
-00000c60: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
-00000c70: 046c 6973 7453 0000 0073 0800 0000 0802  .listS...s......
-00000c80: 0601 1e02 0a01 7a14 4c6f 6361 6c44 6174  ......z.LocalDat
-00000c90: 6153 6f75 7263 652e 6c69 7374 6301 0000  aSource.listc...
-00000ca0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00000cb0: 0043 0000 0073 3200 0000 7400 a001 a100  .C...s2...t.....
-00000cc0: 5c02 7c00 5f02 7c00 5f03 7c00 6a03 6a04  \.|._.|._.|.j.j.
-00000cd0: 7c00 5f05 7c00 6a05 7c00 5f06 7c00 6a03  |._.|.j.|._.|.j.
-00000ce0: 7c00 6a02 7c00 6a05 6603 5300 2901 7a71  |.j.|.j.f.S.).zq
-00000cf0: 0a20 2020 2020 2020 204d 6574 686f 6420  .        Method 
-00000d00: 696e 2063 6861 7267 6520 6f66 2066 696e  in charge of fin
-00000d10: 6469 6e67 2074 6865 2072 6f6f 7420 666f  ding the root fo
-00000d20: 6c64 6572 206f 6620 7468 6520 7072 6f6a  lder of the proj
-00000d30: 6563 7420 616e 6420 7265 6164 696e 6720  ect and reading 
-00000d40: 7468 6520 636f 6e74 656e 7420 6f66 206d  the content of m
-00000d50: 6174 652e 6a73 6f6e 0a20 2020 2020 2020  ate.json.       
-00000d60: 2029 0772 0800 0000 da09 6669 6e64 5f72   ).r......find_r
-00000d70: 6f6f 7472 1000 0000 720b 0000 00da 0e72  ootr....r......r
-00000d80: 6573 756c 7473 5f66 6f6c 6465 72da 1072  esults_folder..r
-00000d90: 6f6f 745f 7361 7665 5f66 6f6c 6465 72da  oot_save_folder.
-00000da0: 0973 6176 655f 7061 7468 721a 0000 0072  .save_pathr....r
-00000db0: 1700 0000 7217 0000 0072 1800 0000 da0a  ....r....r......
-00000dc0: 5f5f 6669 6e64 726f 6f74 5b00 0000 7308  __findroot[...s.
-00000dd0: 0000 0010 040a 0108 0110 017a 1a4c 6f63  ...........z.Loc
-00000de0: 616c 4461 7461 536f 7572 6365 2e5f 5f66  alDataSource.__f
-00000df0: 696e 6472 6f6f 7446 da04 726f 6f74 da0a  indrootF..root..
-00000e00: 6d6f 6465 6c5f 6e61 6d65 da0a 6578 7065  model_name..expe
-00000e10: 7269 6d65 6e74 da11 6765 6e65 7261 7465  riment..generate
-00000e20: 5f64 6566 6175 6c74 7363 0500 0000 0000  _defaultsc......
-00000e30: 0000 0000 0000 0800 0000 0500 0000 4300  ..............C.
-00000e40: 0000 734e 0000 007c 006a 00a0 01a1 005c  ..sN...|.j.....\
-00000e50: 027d 057d 0674 027c 0683 0164 016b 0472  .}.}.t.|...d.k.r
-00000e60: 2574 0364 027c 029b 0064 037c 039b 009d  %t.d.|...d.|....
-00000e70: 0483 0101 007c 0644 005d 067d 0774 037c  .....|.D.].}.t.|
-00000e80: 0783 0101 0071 1974 04a0 0564 04a1 0101  .....q.t...d....
-00000e90: 007c 0553 0029 057a 5b0a 2020 2020 2020  .|.S.).z[.      
-00000ea0: 2020 5661 6c69 6461 7465 7320 7468 6174    Validates that
-00000eb0: 2061 6c6c 2074 6865 2072 6571 7569 7265   all the require
-00000ec0: 6420 7061 7261 6d65 7465 7273 2061 7265  d parameters are
-00000ed0: 2070 7265 7365 6e74 2069 6e20 7468 6520   present in the 
-00000ee0: 7061 7261 6d73 2066 696c 650a 2020 2020  params file.    
-00000ef0: 2020 2020 7201 0000 00fa 0a45 7272 6f72      r......Error
-00000f00: 7320 696e 20fa 012f e901 0000 0029 06da  s in ../.....)..
-00000f10: 0774 7261 696e 6572 da12 6765 6e65 7261  .trainer..genera
-00000f20: 7465 5f66 756c 6c5f 6469 6374 da03 6c65  te_full_dict..le
-00000f30: 6eda 0570 7269 6e74 da03 7379 73da 0465  n..print..sys..e
-00000f40: 7869 7429 0872 1300 0000 723b 0000 0072  xit).r....r;...r
-00000f50: 3c00 0000 723d 0000 0072 3e00 0000 5a0d  <...r=...r>...Z.
-00000f60: 7061 7273 6564 5f70 6172 616d 73da 0665  parsed_params..e
-00000f70: 7272 6f72 73da 0565 7272 6f72 7217 0000  rrors..errorr...
-00000f80: 0072 1700 0000 7218 0000 005a 195f 5f76  .r....r....Z.__v
-00000f90: 616c 6964 6174 655f 6d69 7373 696e 675f  alidate_missing_
-00000fa0: 7061 7261 6d73 6400 0000 730e 0000 000e  paramsd...s.....
-00000fb0: 0b0c 0214 0108 010a 010a 0504 027a 294c  .............z)L
-00000fc0: 6f63 616c 4461 7461 536f 7572 6365 2e5f  ocalDataSource._
-00000fd0: 5f76 616c 6964 6174 655f 6d69 7373 696e  _validate_missin
-00000fe0: 675f 7061 7261 6d73 6303 0000 0000 0000  g_paramsc.......
-00000ff0: 0000 0000 0006 0000 0005 0000 0043 0000  .............C..
-00001000: 0073 6a00 0000 7c00 6a00 6400 7501 7309  .sj...|.j.d.u.s.
-00001010: 4a00 6401 8301 8201 7c01 a001 a100 5c02  J.d.....|.....\.
-00001020: 7d03 7d04 7402 7c04 8301 6402 6b04 722a  }.}.t.|...d.k.r*
-00001030: 7403 6403 7c02 9b00 9d02 8301 0100 7c04  t.d.|.........|.
-00001040: 4400 5d06 7d05 7403 7c05 8301 0100 711e  D.].}.t.|.....q.
-00001050: 7404 a005 6404 a101 0100 7406 a007 7c00  t...d.....t...|.
-00001060: 6a08 7c03 7c00 6a09 a103 0100 7c03 5300  j.|.|.j.....|.S.
-00001070: 2905 4e7a 5254 7261 696e 6572 206d 7573  ).NzRTrainer mus
-00001080: 7420 6265 2069 6e69 7469 616c 697a 6564  t be initialized
-00001090: 2062 6566 6f72 6520 7061 7273 696e 6720   before parsing 
-000010a0: 7061 7261 6d73 2028 426f 6d62 696c 6c61  params (Bombilla
-000010b0: 2069 7320 6d61 6e61 6765 6420 6279 2054   is managed by T
-000010c0: 7261 696e 6572 2972 0100 0000 723f 0000  rainer)r....r?..
-000010d0: 0072 4100 0000 290a 7242 0000 0072 4300  .rA...).rB...rC.
-000010e0: 0000 7244 0000 0072 4500 0000 7246 0000  ..rD...rE...rF..
-000010f0: 0072 4700 0000 7208 0000 005a 1673 6176  .rG...r....Z.sav
-00001100: 655f 7472 6169 6e5f 6578 7065 7269 6d65  e_train_experime
-00001110: 6e74 7372 3900 0000 720b 0000 0029 0672  ntsr9...r....).r
-00001120: 1300 0000 7242 0000 0072 3d00 0000 da04  ....rB...r=.....
-00001130: 6675 6c6c da03 6572 7272 4900 0000 7217  full..errrI...r.
-00001140: 0000 0072 1700 0000 7218 0000 005a 1b5f  ...r....r....Z._
-00001150: 5f70 6172 7365 5f61 6e64 5f76 616c 6964  _parse_and_valid
-00001160: 6174 655f 7061 7261 6d73 7d00 0000 7316  ate_params}...s.
-00001170: 0000 000c 0202 0104 ff0c 030c 020e 0108  ................
-00001180: 010a 010a 0312 0204 027a 2b4c 6f63 616c  .........z+Local
-00001190: 4461 7461 536f 7572 6365 2e5f 5f70 6172  DataSource.__par
-000011a0: 7365 5f61 6e64 5f76 616c 6964 6174 655f  se_and_validate_
-000011b0: 7061 7261 6d73 6302 0000 0000 0000 0000  paramsc.........
-000011c0: 0000 0002 0000 0003 0000 0043 0000 00f3  ...........C....
-000011d0: 1000 0000 7c00 6a00 a001 7c01 a101 0100  ....|.j...|.....
-000011e0: 6400 5300 720c 0000 0029 02da 066d 6f64  d.S.r....)...mod
-000011f0: 656c 73da 0661 7070 656e 6429 0272 1300  els..append).r..
-00001200: 0000 da05 6d6f 6465 6c72 1700 0000 7217  ....modelr....r.
-00001210: 0000 0072 1800 0000 da09 6164 645f 6d6f  ...r......add_mo
-00001220: 6465 6c90 0000 00f3 0200 0000 1001 7a19  del...........z.
-00001230: 4c6f 6361 6c44 6174 6153 6f75 7263 652e  LocalDataSource.
-00001240: 6164 645f 6d6f 6465 6c63 0200 0000 0000  add_modelc......
-00001250: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-00001260: 0000 724c 0000 0072 0c00 0000 2902 5a08  ..rL...r....).Z.
-00001270: 7472 6169 6e65 7273 724e 0000 0029 0272  trainersrN...).r
-00001280: 1300 0000 7242 0000 0072 1700 0000 7217  ....rB...r....r.
-00001290: 0000 0072 1800 0000 da0b 6164 645f 7472  ...r......add_tr
-000012a0: 6169 6e65 7293 0000 0072 5100 0000 7a1b  ainer....rQ...z.
-000012b0: 4c6f 6361 6c44 6174 6153 6f75 7263 652e  LocalDataSource.
-000012c0: 6164 645f 7472 6169 6e65 7263 0200 0000  add_trainerc....
-000012d0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-000012e0: 4300 0000 724c 0000 0072 0c00 0000 2902  C...rL...r....).
-000012f0: 5a0c 6461 7461 5f6c 6f61 6465 7273 724e  Z.data_loadersrN
-00001300: 0000 0029 0272 1300 0000 5a07 6461 7461  ...).r....Z.data
-00001310: 7365 7472 1700 0000 7217 0000 0072 1800  setr....r....r..
-00001320: 0000 da0f 6164 645f 6461 7461 5f6c 6f61  ....add_data_loa
-00001330: 6465 7296 0000 0072 5100 0000 7a1f 4c6f  der....rQ...z.Lo
-00001340: 6361 6c44 6174 6153 6f75 7263 652e 6164  calDataSource.ad
-00001350: 645f 6461 7461 5f6c 6f61 6465 7263 0200  d_data_loaderc..
-00001360: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00001370: 0000 4300 0000 724c 0000 0072 0c00 0000  ..C...rL...r....
-00001380: 2902 721d 0000 0072 4e00 0000 2902 7213  ).r....rN...).r.
-00001390: 0000 0072 3d00 0000 7217 0000 0072 1700  ...r=...r....r..
-000013a0: 0000 7218 0000 00da 0e61 6464 5f65 7870  ..r......add_exp
-000013b0: 6572 696d 656e 7499 0000 0072 5100 0000  eriment....rQ...
-000013c0: 7a1e 4c6f 6361 6c44 6174 6153 6f75 7263  z.LocalDataSourc
-000013d0: 652e 6164 645f 6578 7065 7269 6d65 6e74  e.add_experiment
-000013e0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000013f0: 0003 0000 0043 0000 0072 4c00 0000 720c  .....C...rL...r.
-00001400: 0000 0029 02da 0870 6163 6b61 6765 7372  ...)...packagesr
-00001410: 4e00 0000 2902 7213 0000 00da 0770 6163  N...).r......pac
-00001420: 6b61 6765 7217 0000 0072 1700 0000 7218  kager....r....r.
-00001430: 0000 00da 0b61 6464 5f70 6163 6b61 6765  .....add_package
-00001440: 9c00 0000 7251 0000 007a 1b4c 6f63 616c  ....rQ...z.Local
-00001450: 4461 7461 536f 7572 6365 2e61 6464 5f70  DataSource.add_p
-00001460: 6163 6b61 6765 2901 4629 18da 085f 5f6e  ackage).F)...__n
-00001470: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00001480: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00001490: 0200 0000 720e 0000 0072 1b00 0000 721c  ....r....r....r.
-000014a0: 0000 00da 0373 7472 7212 0000 0072 3500  .....strr....r5.
-000014b0: 0000 5a28 5f4c 6f63 616c 4461 7461 536f  ..Z(_LocalDataSo
-000014c0: 7572 6365 5f5f 6669 6c74 6572 5f72 6567  urce__filter_reg
-000014d0: 756c 6172 5f66 6f6c 6465 7273 7207 0000  ular_foldersr...
-000014e0: 005a 1e5f 4c6f 6361 6c44 6174 6153 6f75  .Z._LocalDataSou
-000014f0: 7263 655f 5f66 696c 7465 725f 6e61 6d65  rce__filter_name
-00001500: 7372 1900 0000 7203 0000 00da 0462 6f6f  sr....r......boo
-00001510: 6c5a 295f 4c6f 6361 6c44 6174 6153 6f75  lZ)_LocalDataSou
-00001520: 7263 655f 5f76 616c 6964 6174 655f 6d69  rce__validate_mi
-00001530: 7373 696e 675f 7061 7261 6d73 5a2b 5f4c  ssing_paramsZ+_L
-00001540: 6f63 616c 4461 7461 536f 7572 6365 5f5f  ocalDataSource__
-00001550: 7061 7273 655f 616e 645f 7661 6c69 6461  parse_and_valida
-00001560: 7465 5f70 6172 616d 7372 5000 0000 7252  te_paramsrP...rR
-00001570: 0000 0072 5300 0000 7254 0000 0072 5700  ...rS...rT...rW.
-00001580: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
-00001590: 5f72 1700 0000 7217 0000 0072 1500 0000  _r....r....r....
-000015a0: 7218 0000 0072 0a00 0000 0e00 0000 7336  r....r........s6
-000015b0: 0000 0008 0002 0102 020e fe08 1008 030e  ................
-000015c0: 0412 271a 030e 0308 0802 0e04 fb02 0202  ..'.............
-000015d0: fe02 0302 fd02 0402 fc02 050a fb0e 1908  ................
-000015e0: 1308 0308 0308 0310 0372 0a00 0000 2911  .........r....).
-000015f0: da04 6a73 6f6e 7246 0000 005a 1579 6572  ..jsonrF...Z.yer
-00001600: 6261 6d61 7465 2e6d 6174 655f 636f 6e66  bamate.mate_conf
-00001610: 6967 7202 0000 005a 1579 6572 6261 6d61  igr....Z.yerbama
-00001620: 7465 2e75 7469 6c73 2e62 756e 6368 7203  te.utils.bunchr.
-00001630: 0000 00da 0673 6f75 7263 6572 0500 0000  .....sourcer....
-00001640: 7206 0000 0072 2300 0000 da06 7479 7069  r....r#.....typi
-00001650: 6e67 7207 0000 00da 0469 7064 62da 056c  ngr......ipdb..l
-00001660: 6f63 616c 7208 0000 0072 0900 0000 720a  ocalr....r....r.
-00001670: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
-00001680: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00001690: 3e01 0000 0073 1800 0000 0800 0801 0c01  >....s..........
-000016a0: 0c01 0c01 0c01 0801 0c01 0801 0c01 0c01  ................
-000016b0: 1403                                     ..
+00000040: 6402 6c02 6d03 5a03 0100 6403 6404 6c04  d.l.m.Z...d.d.l.
+00000050: 6d05 5a05 0100 6400 6405 6c06 6d06 5a06  m.Z...d.d.l.m.Z.
+00000060: 0100 6400 6401 6c07 5a07 6400 6406 6c08  ..d.d.l.Z.d.d.l.
+00000070: 6d09 5a09 0100 6400 6401 6c0a 5a0a 6403  m.Z...d.d.l.Z.d.
+00000080: 6407 6c0b 6d0c 5a0c 0100 6400 6408 6c08  d.l.m.Z...d.d.l.
+00000090: 6d0d 5a0d 0100 4700 6409 640a 8400 640a  m.Z...G.d.d...d.
+000000a0: 6505 8303 5a0e 6401 5300 290b e900 0000  e...Z.d.S.).....
+000000b0: 004e 2901 da05 4275 6e63 68e9 0200 0000  .N)...Bunch.....
+000000c0: 2901 da0a 4461 7461 536f 7572 6365 2901  )...DataSource).
+000000d0: da04 676c 6f62 2901 da08 4f70 7469 6f6e  ..glob)...Option
+000000e0: 616c 2901 da02 696f 2901 da03 416e 7963  al)...io)...Anyc
+000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000100: 0900 0000 0000 0000 73d0 0000 0065 005a  ........s....e.Z
+00000110: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
+00000120: 0364 0364 0484 005a 0464 0564 0684 005a  .d.d...Z.d.d...Z
+00000130: 0564 0765 0666 0264 0864 0984 045a 0764  .d.e.f.d.d...Z.d
+00000140: 0a65 0865 0619 0066 0264 0b64 0c84 045a  .e.e...f.d.d...Z
+00000150: 0964 0d65 0a65 0619 0064 0a65 0865 0619  .d.e.e...d.e.e..
+00000160: 0066 0464 0e64 0f84 045a 0b64 1065 0666  .f.d.d...Z.d.e.f
+00000170: 0264 1164 1284 045a 0864 1364 1484 005a  .d.d...Z.d.d...Z
+00000180: 0c09 1564 2864 1665 0d64 1765 0664 1865  ...d(d.e.d.e.d.e
+00000190: 0664 1965 0e66 0864 1a64 1b84 055a 0f64  .d.e.f.d.d...Z.d
+000001a0: 1865 0666 0264 1c64 1d84 045a 1064 1e64  .e.f.d.d...Z.d.d
+000001b0: 1f84 005a 1164 2064 2184 005a 1264 2264  ...Z.d d!..Z.d"d
+000001c0: 2384 005a 1364 2464 2584 005a 1464 2664  #..Z.d$d%..Z.d&d
+000001d0: 2784 005a 1587 0004 005a 1653 0029 29da  '..Z.....Z.S.)).
+000001e0: 0f4c 6f63 616c 4461 7461 536f 7572 6365  .LocalDataSource
+000001f0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00000200: 0003 0000 0003 0000 0073 3200 0000 7400  .........s2...t.
+00000210: 8300 a001 a100 0100 7c01 6401 1900 7d02  ........|.d...}.
+00000220: 7c02 7c00 5f02 7c01 7c00 5f03 6400 7c00  |.|._.|.|._.d.|.
+00000230: 5f04 7c00 a005 7c02 a101 0100 6400 5300  _.|...|.....d.S.
+00000240: 2902 4eda 0770 726f 6a65 6374 2906 da05  ).N..project)...
+00000250: 7375 7065 72da 085f 5f69 6e69 745f 5fda  super..__init__.
+00000260: 0b72 6f6f 745f 666f 6c64 6572 da06 636f  .root_folder..co
+00000270: 6e66 6967 da03 6d61 70da 1b5f 4c6f 6361  nfig..map.._Loca
+00000280: 6c44 6174 6153 6f75 7263 655f 5f6c 6f61  lDataSource__loa
+00000290: 645f 6461 7461 2903 da04 7365 6c66 720e  d_data)...selfr.
+000002a0: 0000 00da 0872 6f6f 745f 6469 72a9 01da  .....root_dir...
+000002b0: 095f 5f63 6c61 7373 5f5f a900 fa4c 2f68  .__class__...L/h
+000002c0: 6f6d 652f 616c 2f47 6974 4875 622f 7965  ome/al/GitHub/ye
+000002d0: 7262 616d 6174 652f 7061 636b 6167 6573  rbamate/packages
+000002e0: 2f79 6572 6261 6d61 7465 2f61 7069 2f64  /yerbamate/api/d
+000002f0: 6174 612f 736f 7572 6365 732f 6c6f 6361  ata/sources/loca
+00000300: 6c2f 6c6f 6361 6c2e 7079 720c 0000 000e  l/local.pyr.....
+00000310: 0000 0073 0c00 0000 0a05 0802 0601 0601  ...s............
+00000320: 0601 0e04 7a18 4c6f 6361 6c44 6174 6153  ....z.LocalDataS
+00000330: 6f75 7263 652e 5f5f 696e 6974 5f5f 6301  ource.__init__c.
+00000340: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00000350: 0000 0043 0000 0073 0800 0000 7c00 a000  ...C...s....|...
+00000360: a100 5300 a901 4e29 01da 1a5f 4c6f 6361  ..S...N)..._Loca
+00000370: 6c44 6174 6153 6f75 7263 655f 5f66 696e  lDataSource__fin
+00000380: 6472 6f6f 74a9 0172 1100 0000 7215 0000  droot..r....r...
+00000390: 0072 1500 0000 7216 0000 00da 196c 6f61  .r....r......loa
+000003a0: 645f 6d61 7465 5f63 6f6e 6669 675f 616e  d_mate_config_an
+000003b0: 645f 726f 6f74 1e00 0000 7302 0000 0008  d_root....s.....
+000003c0: 017a 294c 6f63 616c 4461 7461 536f 7572  .z)LocalDataSour
+000003d0: 6365 2e6c 6f61 645f 6d61 7465 5f63 6f6e  ce.load_mate_con
+000003e0: 6669 675f 616e 645f 726f 6f74 6301 0000  fig_and_rootc...
+000003f0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000400: 0043 0000 0073 1200 0000 7c00 a000 7c00  .C...s....|...|.
+00000410: 6a01 a101 0100 7c00 6a02 5300 7217 0000  j.....|.j.S.r...
+00000420: 0029 0372 1000 0000 720d 0000 0072 0f00  .).r....r....r..
+00000430: 0000 7219 0000 0072 1500 0000 7215 0000  ..r....r....r...
+00000440: 0072 1600 0000 da07 7375 6d6d 6172 7921  .r......summary!
+00000450: 0000 0073 0400 0000 0c01 0601 7a17 4c6f  ...s........z.Lo
+00000460: 6361 6c44 6174 6153 6f75 7263 652e 7375  calDataSource.su
+00000470: 6d6d 6172 7972 1200 0000 6302 0000 0000  mmaryr....c.....
+00000480: 0000 0000 0000 0002 0000 0008 0000 0003  ................
+00000490: 0000 0073 ba00 0000 7c00 6a00 6400 6b03  ...s....|.j.d.k.
+000004a0: 7207 6400 5300 6900 7c00 5f00 7401 a002  r.d.S.i.|._.t...
+000004b0: 8801 a101 4400 5d4b 8900 8800 6401 6b02  ....D.]K....d.k.
+000004c0: 722a 8701 6601 6402 6403 8408 7401 a002  r*..f.d.d...t...
+000004d0: 7401 6a03 a004 8801 6401 a102 a101 4400  t.j.....d.....D.
+000004e0: 8301 7c00 6a00 6401 3c00 710f 7401 6a03  ..|.j.d.<.q.t.j.
+000004f0: a005 7401 6a03 a004 8801 8800 a102 a101  ..t.j...........
+00000500: 725a 8800 6404 6b03 725a 6405 7401 a002  rZ..d.k.rZd.t...
+00000510: 7401 6a03 a004 8801 8800 a102 a101 7600  t.j...........v.
+00000520: 725a 8700 8701 6602 6406 6407 8408 7401  rZ....f.d.d...t.
+00000530: a002 7401 6a03 a004 8801 8800 a102 a101  ..t.j...........
+00000540: 4400 8301 7c00 6a00 8800 3c00 710f 6400  D...|.j...<.q.d.
+00000550: 5300 2908 4eda 0b65 7870 6572 696d 656e  S.).N..experimen
+00000560: 7473 6301 0000 0000 0000 0000 0000 0002  tsc.............
+00000570: 0000 000b 0000 0013 0000 0073 5e00 0000  ...........s^...
+00000580: 6900 7c00 5d2b 7d01 7400 6a01 a002 7400  i.|.]+}.t.j...t.
+00000590: 6a01 a003 8800 6400 7c01 a103 a101 7214  j.....d.|.....r.
+000005a0: 7c01 6401 6b03 731c 6402 7c01 7600 7202  |.d.k.s.d.|.v.r.
+000005b0: 7c01 6403 6b03 7202 7c01 6404 6405 8400  |.d.k.r.|.d.d...
+000005c0: 7400 a004 7400 6a01 a003 8800 6400 7c01  t...t.j.....d.|.
+000005d0: a103 a101 4400 8301 9302 7102 5300 2906  ....D.....q.S.).
+000005e0: 721c 0000 00da 0b5f 5f70 7963 6163 6865  r......__pycache
+000005f0: 5f5f fa03 2e70 79fa 0b5f 5f69 6e69 745f  __...py..__init_
+00000600: 5f2e 7079 6301 0000 0000 0000 0000 0000  _.pyc...........
+00000610: 0002 0000 0004 0000 0053 0000 0073 2000  .........S...s .
+00000620: 0000 6700 7c00 5d0c 7d01 6400 7c01 7600  ..g.|.].}.d.|.v.
+00000630: 7202 7c01 6401 6b03 7202 7c01 9102 7102  r.|.d.k.r.|...q.
+00000640: 5300 2902 721e 0000 0072 1f00 0000 7215  S.).r....r....r.
+00000650: 0000 0029 02da 022e 305a 0865 7870 5f66  ...)....0Z.exp_f
+00000660: 696c 6572 1500 0000 7215 0000 0072 1600  iler....r....r..
+00000670: 0000 da0a 3c6c 6973 7463 6f6d 703e 2f00  ....<listcomp>/.
+00000680: 0000 730a 0000 0006 0002 0210 0302 fc06  ..s.............
+00000690: 047a 3a4c 6f63 616c 4461 7461 536f 7572  .z:LocalDataSour
+000006a0: 6365 2e5f 5f6c 6f61 645f 6461 7461 2e3c  ce.__load_data.<
+000006b0: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
+000006c0: 703e 2e3c 6c69 7374 636f 6d70 3e29 05da  p>.<listcomp>)..
+000006d0: 026f 73da 0470 6174 68da 0569 7364 6972  .os..path..isdir
+000006e0: da04 6a6f 696e da07 6c69 7374 6469 7229  ..join..listdir)
+000006f0: 0272 2000 0000 da03 6469 7229 0172 1200  .r .....dir).r..
+00000700: 0000 7215 0000 0072 1600 0000 da0a 3c64  ..r....r......<d
+00000710: 6963 7463 6f6d 703e 2e00 0000 7318 0000  ictcomp>....s...
+00000720: 0006 0002 0816 0102 f708 0a10 0108 f604  ................
+00000730: 020e 0102 ff04 fe06 0a7a 2f4c 6f63 616c  .........z/Local
+00000740: 4461 7461 536f 7572 6365 2e5f 5f6c 6f61  DataSource.__loa
+00000750: 645f 6461 7461 2e3c 6c6f 6361 6c73 3e2e  d_data.<locals>.
+00000760: 3c64 6963 7463 6f6d 703e 721d 0000 0072  <dictcomp>r....r
+00000770: 1f00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00000780: 0002 0000 000a 0000 0013 0000 0073 4a00  .............sJ.
+00000790: 0000 6700 7c00 5d21 7d01 7400 6a01 a002  ..g.|.]!}.t.j...
+000007a0: 7400 6a01 a003 8801 8800 7c01 a103 a101  t.j.......|.....
+000007b0: 7223 7400 6a01 a004 7400 6a01 a003 8801  r#t.j...t.j.....
+000007c0: 8800 7c01 6400 a104 a101 7223 7c01 6401  ..|.d.....r#|.d.
+000007d0: 6b03 7202 7c01 9102 7102 5300 2902 721f  k.r.|...q.S.).r.
+000007e0: 0000 0072 1d00 0000 2905 7222 0000 0072  ...r....).r"...r
+000007f0: 2300 0000 7224 0000 0072 2500 0000 da06  #...r$...r%.....
+00000800: 6578 6973 7473 2902 7220 0000 005a 0773  exists).r ...Z.s
+00000810: 7562 5f64 6972 a902 7227 0000 0072 1200  ub_dir..r'...r..
+00000820: 0000 7215 0000 0072 1600 0000 7221 0000  ..r....r....r!..
+00000830: 0040 0000 0073 1600 0000 0600 0202 1601  .@...s..........
+00000840: 02fd 0604 1001 02ff 02fc 0807 02fa 0606  ................
+00000850: 7a2f 4c6f 6361 6c44 6174 6153 6f75 7263  z/LocalDataSourc
+00000860: 652e 5f5f 6c6f 6164 5f64 6174 612e 3c6c  e.__load_data.<l
+00000870: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000880: 3e29 0672 0f00 0000 7222 0000 0072 2600  >).r....r"...r&.
+00000890: 0000 7223 0000 0072 2500 0000 7224 0000  ..r#...r%...r$..
+000008a0: 0029 0272 1100 0000 7212 0000 0072 1500  .).r....r....r..
+000008b0: 0000 722a 0000 0072 1600 0000 5a0b 5f5f  ..r*...r....Z.__
+000008c0: 6c6f 6164 5f64 6174 6125 0000 0073 1e00  load_data%...s..
+000008d0: 0000 0a02 0401 0602 0e01 0802 0a01 1208  ................
+000008e0: 0ef8 1e0f 1802 0c01 1202 0cfe 0280 04eb  ................
+000008f0: 7a1b 4c6f 6361 6c44 6174 6153 6f75 7263  z.LocalDataSourc
+00000900: 652e 5f5f 6c6f 6164 5f64 6174 61da 056e  e.__load_data..n
+00000910: 616d 6573 6302 0000 0000 0000 0000 0000  amesc...........
+00000920: 0002 0000 0002 0000 0043 0000 0073 0e00  .........C...s..
+00000930: 0000 6401 6402 8400 7c01 4400 8301 5300  ..d.d...|.D...S.
+00000940: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
+00000950: 0200 0000 0500 0000 5300 0000 731a 0000  ........S...s...
+00000960: 0067 007c 005d 097d 017c 01a0 0064 00a1  .g.|.].}.|...d..
+00000970: 0173 027c 0191 0271 0253 0029 01da 025f  .s.|...q.S.)..._
+00000980: 5f29 01da 0a73 7461 7274 7377 6974 6829  _)...startswith)
+00000990: 0272 2000 0000 da02 666e 7215 0000 0072  .r .....fnr....r
+000009a0: 1500 0000 7216 0000 0072 2100 0000 4d00  ....r....r!...M.
+000009b0: 0000 7302 0000 001a 007a 3c4c 6f63 616c  ..s......z<Local
+000009c0: 4461 7461 536f 7572 6365 2e5f 5f66 696c  DataSource.__fil
+000009d0: 7465 725f 7265 6775 6c61 725f 666f 6c64  ter_regular_fold
+000009e0: 6572 732e 3c6c 6f63 616c 733e 2e3c 6c69  ers.<locals>.<li
+000009f0: 7374 636f 6d70 3e72 1500 0000 2902 7211  stcomp>r....).r.
+00000a00: 0000 0072 2b00 0000 7215 0000 0072 1500  ...r+...r....r..
+00000a10: 0000 7216 0000 005a 185f 5f66 696c 7465  ..r....Z.__filte
+00000a20: 725f 7265 6775 6c61 725f 666f 6c64 6572  r_regular_folder
+00000a30: 734c 0000 0073 0200 0000 0e01 7a28 4c6f  sL...s......z(Lo
+00000a40: 6361 6c44 6174 6153 6f75 7263 652e 5f5f  calDataSource.__
+00000a50: 6669 6c74 6572 5f72 6567 756c 6172 5f66  filter_regular_f
+00000a60: 6f6c 6465 7273 da05 7175 6572 7963 0300  olders..queryc..
+00000a70: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+00000a80: 0000 0300 0000 731e 0000 0088 0064 0075  ......s......d.u
+00000a90: 0072 067c 0253 0087 0066 0164 0164 0284  .r.|.S...f.d.d..
+00000aa0: 087c 0244 0083 0153 0029 034e 6301 0000  .|.D...S.).Nc...
+00000ab0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000ac0: 0013 0000 0073 1800 0000 6700 7c00 5d08  .....s....g.|.].
+00000ad0: 7d01 8800 7c01 6b02 7202 7c01 9102 7102  }...|.k.r.|...q.
+00000ae0: 5300 7215 0000 0072 1500 0000 2902 7220  S.r....r....).r 
+00000af0: 0000 00da 046e 616d 65a9 0172 2f00 0000  .....name..r/...
+00000b00: 7215 0000 0072 1600 0000 7221 0000 0050  r....r....r!...P
+00000b10: 0000 0073 0200 0000 1800 7a32 4c6f 6361  ...s......z2Loca
+00000b20: 6c44 6174 6153 6f75 7263 652e 5f5f 6669  lDataSource.__fi
+00000b30: 6c74 6572 5f6e 616d 6573 2e3c 6c6f 6361  lter_names.<loca
+00000b40: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7215  ls>.<listcomp>r.
+00000b50: 0000 0029 0372 1100 0000 722f 0000 0072  ...).r....r/...r
+00000b60: 2b00 0000 7215 0000 0072 3100 0000 7216  +...r....r1...r.
+00000b70: 0000 005a 0e5f 5f66 696c 7465 725f 6e61  ...Z.__filter_na
+00000b80: 6d65 734f 0000 0073 0200 0000 1e01 7a1e  mesO...s......z.
+00000b90: 4c6f 6361 6c44 6174 6153 6f75 7263 652e  LocalDataSource.
+00000ba0: 5f5f 6669 6c74 6572 5f6e 616d 6573 da06  __filter_names..
+00000bb0: 6d6f 6475 6c65 6302 0000 0000 0000 0000  modulec.........
+00000bc0: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+00000bd0: 3600 0000 7c01 6400 7500 7207 7c00 6a00  6...|.d.u.r.|.j.
+00000be0: 5300 7c01 7c00 6a00 a001 a100 7600 7316  S.|.|.j.....v.s.
+00000bf0: 4a00 6401 7c01 9b00 6402 9d03 8301 8201  J.d.|...d.......
+00000c00: 7c00 6a00 7c01 1900 5300 2903 4e7a 074d  |.j.|...S.).Nz.M
+00000c10: 6f64 756c 6520 7a0a 206e 6f74 2066 6f75  odule z. not fou
+00000c20: 6e64 2902 720f 0000 00da 046b 6579 7329  nd).r......keys)
+00000c30: 0272 1100 0000 7232 0000 0072 1500 0000  .r....r2...r....
+00000c40: 7215 0000 0072 1600 0000 da04 6c69 7374  r....r......list
+00000c50: 5200 0000 7308 0000 0008 0206 011e 020a  R...s...........
+00000c60: 017a 144c 6f63 616c 4461 7461 536f 7572  .z.LocalDataSour
+00000c70: 6365 2e6c 6973 7463 0100 0000 0000 0000  ce.listc........
+00000c80: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+00000c90: 7332 0000 0074 00a0 01a1 005c 027c 005f  s2...t.....\.|._
+00000ca0: 027c 005f 037c 006a 036a 047c 005f 057c  .|._.|.j.j.|._.|
+00000cb0: 006a 057c 005f 067c 006a 037c 006a 027c  .j.|._.|.j.|.j.|
+00000cc0: 006a 0566 0353 0029 017a 710a 2020 2020  .j.f.S.).zq.    
+00000cd0: 2020 2020 4d65 7468 6f64 2069 6e20 6368      Method in ch
+00000ce0: 6172 6765 206f 6620 6669 6e64 696e 6720  arge of finding 
+00000cf0: 7468 6520 726f 6f74 2066 6f6c 6465 7220  the root folder 
+00000d00: 6f66 2074 6865 2070 726f 6a65 6374 2061  of the project a
+00000d10: 6e64 2072 6561 6469 6e67 2074 6865 2063  nd reading the c
+00000d20: 6f6e 7465 6e74 206f 6620 6d61 7465 2e6a  ontent of mate.j
+00000d30: 736f 6e0a 2020 2020 2020 2020 2907 7207  son.        ).r.
+00000d40: 0000 00da 0966 696e 645f 726f 6f74 720d  .....find_rootr.
+00000d50: 0000 0072 0e00 0000 5a0e 7265 7375 6c74  ...r....Z.result
+00000d60: 735f 666f 6c64 6572 5a10 726f 6f74 5f73  s_folderZ.root_s
+00000d70: 6176 655f 666f 6c64 6572 da09 7361 7665  ave_folder..save
+00000d80: 5f70 6174 6872 1900 0000 7215 0000 0072  _pathr....r....r
+00000d90: 1500 0000 7216 0000 00da 0a5f 5f66 696e  ....r......__fin
+00000da0: 6472 6f6f 745a 0000 0073 0800 0000 1004  drootZ...s......
+00000db0: 0a01 0801 1001 7a1a 4c6f 6361 6c44 6174  ......z.LocalDat
+00000dc0: 6153 6f75 7263 652e 5f5f 6669 6e64 726f  aSource.__findro
+00000dd0: 6f74 46da 0472 6f6f 74da 0a6d 6f64 656c  otF..root..model
+00000de0: 5f6e 616d 65da 0a65 7870 6572 696d 656e  _name..experimen
+00000df0: 74da 1167 656e 6572 6174 655f 6465 6661  t..generate_defa
+00000e00: 756c 7473 6305 0000 0000 0000 0000 0000  ultsc...........
+00000e10: 0008 0000 0005 0000 0043 0000 0073 4e00  .........C...sN.
+00000e20: 0000 7c00 6a00 a001 a100 5c02 7d05 7d06  ..|.j.....\.}.}.
+00000e30: 7402 7c06 8301 6401 6b04 7225 7403 6402  t.|...d.k.r%t.d.
+00000e40: 7c02 9b00 6403 7c03 9b00 9d04 8301 0100  |...d.|.........
+00000e50: 7c06 4400 5d06 7d07 7403 7c07 8301 0100  |.D.].}.t.|.....
+00000e60: 7119 7404 a005 6404 a101 0100 7c05 5300  q.t...d.....|.S.
+00000e70: 2905 7a5b 0a20 2020 2020 2020 2056 616c  ).z[.        Val
+00000e80: 6964 6174 6573 2074 6861 7420 616c 6c20  idates that all 
+00000e90: 7468 6520 7265 7175 6972 6564 2070 6172  the required par
+00000ea0: 616d 6574 6572 7320 6172 6520 7072 6573  ameters are pres
+00000eb0: 656e 7420 696e 2074 6865 2070 6172 616d  ent in the param
+00000ec0: 7320 6669 6c65 0a20 2020 2020 2020 2072  s file.        r
+00000ed0: 0100 0000 fa0a 4572 726f 7273 2069 6e20  ......Errors in 
+00000ee0: fa01 2fe9 0100 0000 2906 da07 7472 6169  ../.....)...trai
+00000ef0: 6e65 72da 1267 656e 6572 6174 655f 6675  ner..generate_fu
+00000f00: 6c6c 5f64 6963 74da 036c 656e da05 7072  ll_dict..len..pr
+00000f10: 696e 74da 0373 7973 da04 6578 6974 2908  int..sys..exit).
+00000f20: 7211 0000 0072 3800 0000 7239 0000 0072  r....r8...r9...r
+00000f30: 3a00 0000 723b 0000 005a 0d70 6172 7365  :...r;...Z.parse
+00000f40: 645f 7061 7261 6d73 da06 6572 726f 7273  d_params..errors
+00000f50: da05 6572 726f 7272 1500 0000 7215 0000  ..errorr....r...
+00000f60: 0072 1600 0000 5a19 5f5f 7661 6c69 6461  .r....Z.__valida
+00000f70: 7465 5f6d 6973 7369 6e67 5f70 6172 616d  te_missing_param
+00000f80: 7363 0000 0073 0e00 0000 0e0b 0c02 1401  sc...s..........
+00000f90: 0801 0a01 0a05 0402 7a29 4c6f 6361 6c44  ........z)LocalD
+00000fa0: 6174 6153 6f75 7263 652e 5f5f 7661 6c69  ataSource.__vali
+00000fb0: 6461 7465 5f6d 6973 7369 6e67 5f70 6172  date_missing_par
+00000fc0: 616d 7363 0300 0000 0000 0000 0000 0000  amsc............
+00000fd0: 0600 0000 0500 0000 4300 0000 736a 0000  ........C...sj..
+00000fe0: 007c 006a 0064 0075 0173 094a 0064 0183  .|.j.d.u.s.J.d..
+00000ff0: 0182 017c 01a0 01a1 005c 027d 037d 0474  ...|.....\.}.}.t
+00001000: 027c 0483 0164 026b 0472 2a74 0364 037c  .|...d.k.r*t.d.|
+00001010: 029b 009d 0283 0101 007c 0444 005d 067d  .........|.D.].}
+00001020: 0574 037c 0583 0101 0071 1e74 04a0 0564  .t.|.....q.t...d
+00001030: 04a1 0101 0074 06a0 077c 006a 087c 037c  .....t...|.j.|.|
+00001040: 006a 09a1 0301 007c 0353 0029 054e 7a52  .j.....|.S.).NzR
+00001050: 5472 6169 6e65 7220 6d75 7374 2062 6520  Trainer must be 
+00001060: 696e 6974 6961 6c69 7a65 6420 6265 666f  initialized befo
+00001070: 7265 2070 6172 7369 6e67 2070 6172 616d  re parsing param
+00001080: 7320 2842 6f6d 6269 6c6c 6120 6973 206d  s (Bombilla is m
+00001090: 616e 6167 6564 2062 7920 5472 6169 6e65  anaged by Traine
+000010a0: 7229 7201 0000 0072 3c00 0000 723e 0000  r)r....r<...r>..
+000010b0: 0029 0a72 3f00 0000 7240 0000 0072 4100  .).r?...r@...rA.
+000010c0: 0000 7242 0000 0072 4300 0000 7244 0000  ..rB...rC...rD..
+000010d0: 0072 0700 0000 5a16 7361 7665 5f74 7261  .r....Z.save_tra
+000010e0: 696e 5f65 7870 6572 696d 656e 7473 7236  in_experimentsr6
+000010f0: 0000 0072 0e00 0000 2906 7211 0000 0072  ...r....).r....r
+00001100: 3f00 0000 723a 0000 00da 0466 756c 6cda  ?...r:.....full.
+00001110: 0365 7272 7246 0000 0072 1500 0000 7215  .errrF...r....r.
+00001120: 0000 0072 1600 0000 5a1b 5f5f 7061 7273  ...r....Z.__pars
+00001130: 655f 616e 645f 7661 6c69 6461 7465 5f70  e_and_validate_p
+00001140: 6172 616d 737c 0000 0073 1600 0000 0c02  arams|...s......
+00001150: 0201 04ff 0c03 0c02 0e01 0801 0a01 0a03  ................
+00001160: 1202 0402 7a2b 4c6f 6361 6c44 6174 6153  ....z+LocalDataS
+00001170: 6f75 7263 652e 5f5f 7061 7273 655f 616e  ource.__parse_an
+00001180: 645f 7661 6c69 6461 7465 5f70 6172 616d  d_validate_param
+00001190: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
+000011a0: 0000 0300 0000 4300 0000 f310 0000 007c  ......C........|
+000011b0: 006a 00a0 017c 01a1 0101 0064 0053 0072  .j...|.....d.S.r
+000011c0: 1700 0000 2902 da06 6d6f 6465 6c73 da06  ....)...models..
+000011d0: 6170 7065 6e64 2902 7211 0000 00da 056d  append).r......m
+000011e0: 6f64 656c 7215 0000 0072 1500 0000 7216  odelr....r....r.
+000011f0: 0000 00da 0961 6464 5f6d 6f64 656c 8f00  .....add_model..
+00001200: 0000 f302 0000 0010 017a 194c 6f63 616c  .........z.Local
+00001210: 4461 7461 536f 7572 6365 2e61 6464 5f6d  DataSource.add_m
+00001220: 6f64 656c 6302 0000 0000 0000 0000 0000  odelc...........
+00001230: 0002 0000 0003 0000 0043 0000 0072 4900  .........C...rI.
+00001240: 0000 7217 0000 0029 025a 0874 7261 696e  ..r....).Z.train
+00001250: 6572 7372 4b00 0000 2902 7211 0000 0072  ersrK...).r....r
+00001260: 3f00 0000 7215 0000 0072 1500 0000 7216  ?...r....r....r.
+00001270: 0000 00da 0b61 6464 5f74 7261 696e 6572  .....add_trainer
+00001280: 9200 0000 724e 0000 007a 1b4c 6f63 616c  ....rN...z.Local
+00001290: 4461 7461 536f 7572 6365 2e61 6464 5f74  DataSource.add_t
+000012a0: 7261 696e 6572 6302 0000 0000 0000 0000  rainerc.........
+000012b0: 0000 0002 0000 0003 0000 0043 0000 0072  ...........C...r
+000012c0: 4900 0000 7217 0000 0029 025a 0c64 6174  I...r....).Z.dat
+000012d0: 615f 6c6f 6164 6572 7372 4b00 0000 2902  a_loadersrK...).
+000012e0: 7211 0000 005a 0764 6174 6173 6574 7215  r....Z.datasetr.
+000012f0: 0000 0072 1500 0000 7216 0000 00da 0f61  ...r....r......a
+00001300: 6464 5f64 6174 615f 6c6f 6164 6572 9500  dd_data_loader..
+00001310: 0000 724e 0000 007a 1f4c 6f63 616c 4461  ..rN...z.LocalDa
+00001320: 7461 536f 7572 6365 2e61 6464 5f64 6174  taSource.add_dat
+00001330: 615f 6c6f 6164 6572 6302 0000 0000 0000  a_loaderc.......
+00001340: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00001350: 0072 4900 0000 7217 0000 0029 0272 1c00  .rI...r....).r..
+00001360: 0000 724b 0000 0029 0272 1100 0000 723a  ..rK...).r....r:
+00001370: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+00001380: 0000 da0e 6164 645f 6578 7065 7269 6d65  ....add_experime
+00001390: 6e74 9800 0000 724e 0000 007a 1e4c 6f63  nt....rN...z.Loc
+000013a0: 616c 4461 7461 536f 7572 6365 2e61 6464  alDataSource.add
+000013b0: 5f65 7870 6572 696d 656e 7463 0200 0000  _experimentc....
+000013c0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+000013d0: 4300 0000 7249 0000 0072 1700 0000 2902  C...rI...r....).
+000013e0: da08 7061 636b 6167 6573 724b 0000 0029  ..packagesrK...)
+000013f0: 0272 1100 0000 da07 7061 636b 6167 6572  .r......packager
+00001400: 1500 0000 7215 0000 0072 1600 0000 da0b  ....r....r......
+00001410: 6164 645f 7061 636b 6167 659b 0000 0072  add_package....r
+00001420: 4e00 0000 7a1b 4c6f 6361 6c44 6174 6153  N...z.LocalDataS
+00001430: 6f75 7263 652e 6164 645f 7061 636b 6167  ource.add_packag
+00001440: 6529 0146 2917 da08 5f5f 6e61 6d65 5f5f  e).F)...__name__
+00001450: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00001460: 7175 616c 6e61 6d65 5f5f 720c 0000 0072  qualname__r....r
+00001470: 1a00 0000 721b 0000 00da 0373 7472 7210  ....r......strr.
+00001480: 0000 0072 3400 0000 5a28 5f4c 6f63 616c  ...r4...Z(_Local
+00001490: 4461 7461 536f 7572 6365 5f5f 6669 6c74  DataSource__filt
+000014a0: 6572 5f72 6567 756c 6172 5f66 6f6c 6465  er_regular_folde
+000014b0: 7273 7206 0000 005a 1e5f 4c6f 6361 6c44  rsr....Z._LocalD
+000014c0: 6174 6153 6f75 7263 655f 5f66 696c 7465  ataSource__filte
+000014d0: 725f 6e61 6d65 7372 1800 0000 7202 0000  r_namesr....r...
+000014e0: 00da 0462 6f6f 6c5a 295f 4c6f 6361 6c44  ...boolZ)_LocalD
+000014f0: 6174 6153 6f75 7263 655f 5f76 616c 6964  ataSource__valid
+00001500: 6174 655f 6d69 7373 696e 675f 7061 7261  ate_missing_para
+00001510: 6d73 5a2b 5f4c 6f63 616c 4461 7461 536f  msZ+_LocalDataSo
+00001520: 7572 6365 5f5f 7061 7273 655f 616e 645f  urce__parse_and_
+00001530: 7661 6c69 6461 7465 5f70 6172 616d 7372  validate_paramsr
+00001540: 4d00 0000 724f 0000 0072 5000 0000 7251  M...rO...rP...rQ
+00001550: 0000 0072 5400 0000 da0d 5f5f 636c 6173  ...rT.....__clas
+00001560: 7363 656c 6c5f 5f72 1500 0000 7215 0000  scell__r....r...
+00001570: 0072 1300 0000 7216 0000 0072 0900 0000  .r....r....r....
+00001580: 0d00 0000 7332 0000 0008 000c 0108 1008  ....s2..........
+00001590: 030e 0412 271a 030e 0308 0802 0e04 fb02  ....'...........
+000015a0: 0202 fe02 0302 fd02 0402 fc02 050a fb0e  ................
+000015b0: 1908 1308 0308 0308 0310 0372 0900 0000  ...........r....
+000015c0: 290f da04 6a73 6f6e 7243 0000 005a 1579  )...jsonrC...Z.y
+000015d0: 6572 6261 6d61 7465 2e75 7469 6c73 2e62  erbamate.utils.b
+000015e0: 756e 6368 7202 0000 00da 0673 6f75 7263  unchr......sourc
+000015f0: 6572 0400 0000 7205 0000 0072 2200 0000  er....r....r"...
+00001600: da06 7479 7069 6e67 7206 0000 00da 0469  ..typingr......i
+00001610: 7064 62da 056c 6f63 616c 7207 0000 0072  pdb..localr....r
+00001620: 0800 0000 7209 0000 0072 1500 0000 7215  ....r....r....r.
+00001630: 0000 0072 1500 0000 7216 0000 00da 083c  ...r....r......<
+00001640: 6d6f 6475 6c65 3e01 0000 0073 1600 0000  module>....s....
+00001650: 0800 0801 0c01 0c01 0c01 0801 0c01 0801  ................
+00001660: 0c01 0c01 1403                           ......
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/sources/local/io.py` & `yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import os
 import shutil
 import sys
 from typing import Optional
 import ipdb
 
-from .....mate_config import MateConfig
 from .....utils.bunch import Bunch
 from .....utils.utils import once
 
 
 
 print_once = once(print)
 
@@ -19,36 +18,42 @@
     Method in charge of finding the root folder of the project and reading the content of mate.json
     """
     # path of execution
     current_path = os.getcwd()
     found = False
     i = 0
     root_folder = ""
-    config: Optional[MateConfig] = None
+    config = None
     while not found and i < 2:
         if os.path.exists(os.path.join(current_path, "mate.json")):
             conf_path = os.path.join(current_path, "mate.json")
             config = load_mate_config(conf_path)
-            root_folder = config.project
+            root_folder = config["project"]
             # self.__import_submodules(self.root_folder)
             found = True
         else:
             os.chdir("..")
             current_path = os.getcwd()
             i += 1
             if current_path == "/" or i == 2:
                 raise Exception(
                     "Could not find mate.json. Please make sure you are in the root folder of the project."
                 )
 
     # self.root_save_folder = self.root_folder
     sys.path.insert(0, os.getcwd())
-    return root_folder, config
+    return root_folder, Bunch(config)
 
 
+def decorator_dict_to_object(func):
+    def wrapper(*args, **kwargs):
+        return Bunch(func(*args, **kwargs))
+
+    return wrapper
+
 
 def list_packages(root_folder: str, folder: str):
     return (
         tuple(x for x in os.listdir(os.path.join(root_folder, folder)) if not "__" in x)
         if os.path.exists(os.path.join(root_folder, folder))
         else tuple()
     )
@@ -122,19 +127,22 @@
 #     exp_path = __get_experiment_path(root_folder, model_name, experiment_name)
 
 #     assert os.path.exists(exp_path), f"Experiment {exp_path} does not exist"
 
 
 def load_mate_config(path):
     with open(path) as f:
-        config = MateConfig(json.load(f))
+        config = json.load(f)
         # assert (
         #    "results_folder" in config
         # ), 'Please add "results_folder":<path> in mate.json'
         # assert "project" in config, 'Please add "project":<project name> in mate.json'
+
+    # for
+    
     return config
 
 
 def remove(root_folder: str, model_name: str):
     action = "go"
     while action not in ("y", "n"):
         action = input(f'Are you sure you want to remove model "{model_name}"? (y/n)\n')
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/sources/local/local.py` & `yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/local.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import json
 import sys
-from yerbamate.mate_config import MateConfig
 from yerbamate.utils.bunch import Bunch
 from ..source import DataSource
 from glob import glob
 import os
 from typing import Optional
 import ipdb
 from ..local import io
 from typing import Any
 
 
 class LocalDataSource(DataSource):
     def __init__(
         self,
-        config: MateConfig,
+        config,
         # root_dir: str = ".",  # a different root (".mate") is used while installing a packaage installing a package, we can use the root dir of the package
     ):
         super().__init__()
 
-        root_dir = config.project
+        root_dir = config["project"]
         self.root_folder = root_dir
         self.config = config
         self.map = None
 
         # ProjectParser.check_project_structure(root_dir)
 
         self.__load_data(root_dir)
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/sources/remote/remote.py` & `yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/remote.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Feb  6 19:48:30 2023 UTC, .py size: 326 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8e59 e163 4601 0000  o........Y.cF...
+00000000: 6f0d 0d0a 0000 0000 e7c6 3164 4601 0000  o.........1dF...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6402 6403 8400 5a01 6401  d.l.Z.d.d...Z.d.
 00000040: 5300 2904 e900 0000 004e 6301 0000 0000  S.)......Nc.....
 00000050: 0000 0000 0000 0005 0000 0008 0000 0043  ...............C
 00000060: 0000 0073 7200 0000 7400 7c00 6401 8302  ...sr...t.|.d...
 00000070: 8f0f 7d01 7401 a002 7c01 a003 a100 a101  ..}.t...|.......
@@ -17,15 +17,15 @@
 00000100: 0477 616c 6bda 0a69 7369 6e73 7461 6e63  .walk..isinstanc
 00000110: 65da 0a49 6d70 6f72 7446 726f 6dda 056c  e..ImportFrom..l
 00000120: 6576 656c da06 6170 7065 6e64 da06 6d6f  evel..append..mo
 00000130: 6475 6c65 2905 da04 6669 6c65 da01 66da  dule)...file..f.
 00000140: 0474 7265 65da 1072 656c 6174 6976 655f  .tree..relative_
 00000150: 696d 706f 7274 73da 046e 6f64 65a9 0072  imports..node..r
 00000160: 1200 0000 fa47 2f68 6f6d 652f 616c 2f47  .....G/home/al/G
-00000170: 6974 6875 622f 7965 7262 616d 6174 652f  ithub/yerbamate/
+00000170: 6974 4875 622f 7965 7262 616d 6174 652f  itHub/yerbamate/
 00000180: 7061 636b 6167 6573 2f79 6572 6261 6d61  packages/yerbama
 00000190: 7465 2f61 7069 2f64 6174 612f 7574 696c  te/api/data/util
 000001a0: 732f 6578 705f 7574 696c 2e70 79da 1467  s/exp_util.py..g
 000001b0: 6574 5f72 656c 6174 6976 655f 696d 706f  et_relative_impo
 000001c0: 7274 7303 0000 0073 1400 0000 0c01 1001  rts....s........
 000001d0: 1cff 0402 0e01 0c01 0a01 0c01 0280 0401  ................
 000001e0: 7214 0000 0029 0272 0400 0000 7214 0000  r....).r....r...
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Feb  6 23:30:31 2023 UTC, .py size: 1197 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 978d e163 ad04 0000  o..........c....
+00000000: 6f0d 0d0a 0000 0000 e7c6 3164 ad04 0000  o.........1d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6403 6404 8400  Z.d.d.l.Z.d.d...
 00000050: 5a04 6405 6406 8400 5a05 6402 5300 2907  Z.d.d...Z.d.S.).
 00000060: e900 0000 0029 01da 0452 6570 6f4e 6300  .....)...RepoNc.
 00000070: 0000 0000 0000 0000 0000 0006 0000 0009  ................
@@ -20,27 +20,27 @@
 00000130: 7c05 5300 6400 5300 2906 4ee9 0300 0000  |.S.d.S.).N.....
 00000140: fa01 2fe9 ffff ffff 7a02 2e2e 7201 0000  ../.....z...r...
 00000150: 0029 0bda 026f 73da 0667 6574 6377 64da  .)...os..getcwd.
 00000160: 0572 616e 6765 7202 0000 00da 0661 7070  .ranger......app
 00000170: 656e 64da 0573 706c 6974 da04 7061 7468  end..split..path
 00000180: da04 6a6f 696e da07 6162 7370 6174 68da  ..join..abspath.
 00000190: 0c5f 5f70 6172 7365 5f72 6570 6fda 036c  .__parse_repo..l
-000001a0: 656e 2906 5a09 6d61 785f 6465 7074 685a  en).Z.max_depthZ
+000001a0: 656e 2906 da09 6d61 785f 6465 7074 685a  en)...max_depthZ
 000001b0: 0b72 6f6f 745f 7365 6172 6368 da05 6e6f  .root_search..no
 000001c0: 6465 73da 0472 6570 6fda 0169 da0a 7061  des..repo..i..pa
-000001d0: 7273 6564 5f75 726c a900 7214 0000 00fa  rsed_url..r.....
-000001e0: 472f 686f 6d65 2f61 6c2f 4769 7468 7562  G/home/al/Github
+000001d0: 7273 6564 5f75 726c a900 7215 0000 00fa  rsed_url..r.....
+000001e0: 472f 686f 6d65 2f61 6c2f 4769 7448 7562  G/home/al/GitHub
 000001f0: 2f79 6572 6261 6d61 7465 2f70 6163 6b61  /yerbamate/packa
 00000200: 6765 732f 7965 7262 616d 6174 652f 6170  ges/yerbamate/ap
 00000210: 692f 6461 7461 2f75 7469 6c73 2f67 6974  i/data/utils/git
 00000220: 5f75 7469 6c2e 7079 da12 7061 7273 655f  _util.py..parse_
 00000230: 7572 6c5f 6672 6f6d 5f67 6974 0600 0000  url_from_git....
 00000240: 7328 0000 0004 0208 0204 0104 010c 0102  s(..............
 00000250: 0108 0106 0106 0114 010e 0210 0104 0208  ................
-00000260: 010e 021a 0104 0104 ff04 0104 0272 1600  .............r..
+00000260: 010e 021a 0104 0104 ff04 0104 0272 1700  .............r..
 00000270: 0000 6301 0000 0000 0000 0000 0000 0003  ..c.............
 00000280: 0000 0004 0000 0043 0000 0073 6400 0000  .......C...sd...
 00000290: 7c00 6a00 6401 1900 6a01 7d01 7c01 a002  |.j.d...j.}.|...
 000002a0: 6402 a101 7219 7c01 a003 6402 6403 a102  d...r.|...d.d...
 000002b0: a003 6404 6405 a102 a003 6406 6407 a102  ..d.d.....d.d...
 000002c0: 7d01 7c01 a004 6408 a101 7224 7c01 6400  }.|...d...r$|.d.
 000002d0: 6409 8502 1900 7d01 7c00 6a05 6a06 7d02  d.....}.|.j.j.}.
@@ -49,17 +49,17 @@
 00000300: 7440 7a07 6874 7470 733a 2ffa 013a 7204  t@z.https:/..:r.
 00000310: 0000 007a 022f 2f7a 033a 2f2f 7a04 2e67  ...z.//z.://z..g
 00000320: 6974 e9fc ffff ff7a 062f 7472 6565 2f29  it.....z./tree/)
 00000330: 075a 0772 656d 6f74 6573 da03 7572 6cda  .Z.remotes..url.
 00000340: 0a73 7461 7274 7377 6974 68da 0772 6570  .startswith..rep
 00000350: 6c61 6365 da08 656e 6473 7769 7468 5a0d  lace..endswithZ.
 00000360: 6163 7469 7665 5f62 7261 6e63 68da 046e  active_branch..n
-00000370: 616d 6529 0372 1100 0000 7219 0000 00da  ame).r....r.....
-00000380: 0662 7261 6e63 6872 1400 0000 7214 0000  .branchr....r...
-00000390: 0072 1500 0000 720e 0000 0021 0000 0073  .r....r....!...s
+00000370: 616d 6529 0372 1200 0000 721a 0000 00da  ame).r....r.....
+00000380: 0662 7261 6e63 6872 1500 0000 7215 0000  .branchr....r...
+00000390: 0072 1600 0000 720e 0000 0021 0000 0073  .r....r....!...s
 000003a0: 1000 0000 0c01 0a03 1c03 0a03 0c01 0802  ................
 000003b0: 1001 0402 720e 0000 0029 06da 0367 6974  ....r....)...git
 000003c0: 7202 0000 0072 0600 0000 da04 6970 6462  r....r......ipdb
-000003d0: 7216 0000 0072 0e00 0000 7214 0000 0072  r....r....r....r
-000003e0: 1400 0000 7214 0000 0072 1500 0000 da08  ....r....r......
+000003d0: 7217 0000 0072 0e00 0000 7215 0000 0072  r....r....r....r
+000003e0: 1500 0000 7215 0000 0072 1600 0000 da08  ....r....r......
 000003f0: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
 00000400: 000c 0008 0108 0108 030c 1b              ...........
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Feb 12 12:12:33 2023 UTC, .py size: 7395 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b1d7 e863 e31c 0000  o..........c....
+00000000: 6f0d 0d0a 0000 0000 e7c6 3164 e31c 0000  o.........1d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a05 6400 6401 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c07 5a07 6400 6402 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 6d0a 5a0a 6d0b 5a0b 0100 6400 6401 6c0c  m.Z.m.Z...d.d.l.
@@ -43,15 +43,15 @@
 000002a0: 2901 da03 656e 644e 2905 da05 7072 696e  )...endN)...prin
 000002b0: 74da 0a45 5241 5345 5f4c 494e 45da 1243  t..ERASE_LINE..C
 000002c0: 4f4c 4f52 5f4e 414d 455f 544f 5f43 4f44  OLOR_NAME_TO_COD
 000002d0: 4572 0300 0000 da09 5245 5345 545f 414c  Er......RESET_AL
 000002e0: 4c29 04da 0474 6578 74da 0563 6f6c 6f72  L)...text..color
 000002f0: da08 696e 5f70 6c61 6365 da06 6b77 6172  ..in_place..kwar
 00000300: 6773 a900 7213 0000 00fa 452f 686f 6d65  gs..r.....E/home
-00000310: 2f61 6c2f 4769 7468 7562 2f79 6572 6261  /al/Github/yerba
+00000310: 2f61 6c2f 4769 7448 7562 2f79 6572 6261  /al/GitHub/yerba
 00000320: 6d61 7465 2f70 6163 6b61 6765 732f 7965  mate/packages/ye
 00000330: 7262 616d 6174 652f 6170 692f 6461 7461  rbamate/api/data
 00000340: 2f75 7469 6c73 2f67 6974 6469 722e 7079  /utils/gitdir.py
 00000350: da0a 7072 696e 745f 7465 7874 1800 0000  ..print_text....
 00000360: 7306 0000 0004 0b10 0122 0172 1500 0000  s........".r....
 00000370: 6301 0000 0000 0000 0000 0000 0006 0000  c...............
 00000380: 0005 0000 0043 0000 0073 8800 0000 7400  .....C...s....t.
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/utils/git_util.py` & `yerbamate-0.9.22/packages/yerbamate/api/data/utils/git_util.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/data/utils/gitdir.py` & `yerbamate-0.9.22/packages/yerbamate/api/data/utils/gitdir.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.21/packages/yerbamate/api/mate_api.py` & `yerbamate-0.9.22/packages/yerbamate/api/mate_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import os
 
 import sys
 
 from time import sleep
-from yerbamate.mate_config import MateConfig
+
 
 
 from .data.module_repository import ModuleRepository
 
 import ipdb
 
 
 """
 MATE API
 
 """
 
 
 class MateAPI:
-    def __init__(self, config: MateConfig):
-        self.config: MateConfig = config
+    def __init__(self, config):
+        # self.config: MateConfig = config
         self.repository = ModuleRepository(config)
 
 
     @staticmethod
     def init_project(project_name: str):
         ModuleRepository.init_project(project_name)
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/environment.py` & `yerbamate-0.9.22/packages/yerbamate/environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,47 +4,48 @@
 import shutil
 import sys
 import ipdb
 
 
 ENV_KEY = "env"
 
+
 class Environment(dict):
 
     def __init__(self):
-        
 
         # default restart, test to False
         self.restart = False
         self.test = False
         self.train = False
         self.sample = False
         self.hparams = {}
 
         # set command to True
-        setattr(self, sys.argv[1], True)
-        
+        try:
+            setattr(self, sys.argv[1], True)
+        except:
+            pass
 
         self._root = self.__find_root()
 
-
         # parse python -m module train arg=1 arg2=2
         for arg in sys.argv:
             if "=" not in arg:
                 continue
             key, value = arg.split("=")
             value = self.convert_str_to_data(value)
             setattr(self, key, value)
             self.hparams[key] = value
 
-        
         self._path = sys.argv[0]
         if "bin/mate" in self._path:
             self.name = os.path.join(*sys.argv[2:4])
-            self._path = os.path.join(self._root, "experiments", sys.argv[2],  sys.argv[3] + ".py")
+            self._path = os.path.join(
+                self._root, "experiments", sys.argv[2],  sys.argv[3] + ".py")
             # detect path to experiment
         else:
             self.name = self._path.split("/")[-2:]
             self.name = os.path.join(*self.name)[: -3]
 
         self.__set_env()
 
@@ -63,52 +64,51 @@
                 elif input in ["False", "false"]:
                     return False
 
         return input
 
     def __find_root(self):
         # TODO, find root of the project
-        
+
         path = os.getcwd()
 
         if os.path.exists(os.path.join(path, "mate.json")):
             conf = json.load(open(os.path.join(path, "mate.json"), "r"))
 
             return os.path.join(path, conf["project"])
-       
+
         return None
 
     def __generate_experiment(self):
         # copies the experiment to the results folder
-        results =["results", "results_path", "results_dir", "save", "save_path", "save_dir"]
+        results = ["results", "results_path",
+                   "results_dir", "save", "save_path", "save_dir"]
         result = None
         for key in results:
             if key in self.env:
                 result = self.env[key]
                 break
         if result is None:
             return
         if not os.path.exists(result):
             os.makedirs(result)
-        
+
         save_file = os.path.join(result, "experiment.py")
         # copy from self._path to save_file
         shutil.copyfile(self._path, save_file)
-       
+
         # ipdb.set_trace()
 
         if self.hparams != {}:
             params_file = os.path.join(result, "experiment.json")
             # dump self to params
             # overwrite if exists
             with open(params_file, "w") as f:
                 json.dump(dict(self.hparams), f, indent=4)
 
-
-
     def __set_env(self):
         mate_conf_path = os.path.join("mate.json")
         conf = json.load(open(mate_conf_path, "r"))
 
         env_path = os.path.join("env.json")
         if not os.path.exists(env_path):
             print("Environment file not found, creating one with defaults: env.json")
@@ -119,15 +119,14 @@
                 required_keys = ["results"]
 
             defualt_env = {key: "" for key in required_keys}
 
             with open(env_path, "w") as f:
                 json.dump(defualt_env, f, indent=4)
 
-            
         with open(env_path, "r") as f:
             try:
                 env = json.load(f)
             except json.decoder.JSONDecodeError:
                 env = {
                     "results": "",
                 }
@@ -139,53 +138,54 @@
                 if env[key] == "":
                     if key in os.environ:
                         env[key] = os.environ[key]
                         # print(f"Environment variable {key} set to {os.environ[key]} from shell.")
                     else:
                         env_not_found.append(key)
                         env[key] = value
-        
+
         if len(env_not_found) > 0:
-            print(f"Environment variables not found. Set them in env.json or in your shell.")
+            print(
+                f"Environment variables not found. Set them in env.json or in your shell.")
             for key in env_not_found:
                 desc = conf[ENV_KEY][key] if key in conf[ENV_KEY] else "Required environment variable"
                 print(f"{key} : {desc}")
 
             print("Exiting...")
             sys.exit(1)
-            
+
         # automatically append experiment name to results path
-        search_results = ["results", "results_path", "results_dir", "save", "save_path", "save_dir"]
+        search_results = ["auto_save"]
         for key in search_results:
             if key in env:
                 env[key] = os.path.join(env[key], *self.name.split("/"))
-                env["results"] = env[key]
+                # env["results"] = env[key]
                 break
             if os.environ.get(key, None) is not None and os.environ.get(key, None) != "":
                 env[key] = os.environ.get(key)
-                env["results"] = env[key]
+                # env["results"] = env[key]
                 break
-            
+
         if len(env) == 0:
-            print(f"results/save_dir/save environment variable is empty. Set it in env.json or in your shell.")
+            print(
+                f"results/save_dir/save environment variable is empty. Set it in env.json or in your shell.")
             print("Exiting...")
             sys.exit(1)
-        
+
         setattr(self, "env", env)
 
     def __getitem__(self, key):
         if not key in self:
             # ipdb.set_trace()
             if key in self.env:
                 return self.env[key]
             res = os.environ.get(key, None)
 
             if res is None or res == "":
-                print(f"Environment variable {key} not found. Set it in env.json or in your shell.")
-                print("Exiting...") 
+                print(
+                    f"Environment variable {key} not found. Set it in env.json or in your shell.")
+                print("Exiting...")
                 sys.exit(1)
             else:
                 return res
-            
-        return super().__getitem__(key)
 
- 
+        return super().__getitem__(key)
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/mate.py` & `yerbamate-0.9.22/packages/yerbamate/mate.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,26 @@
 import sys
 
 import ipdb
 from .utils import utils
 import shutil
 from typing import Optional
 
-from .mate_config import MateConfig
 
 
 class Mate:
     """
     Mate, your friendly ML project manager.
     """
 
     def __init__(self, init=False):
         self.root_folder = ""
         self.save_path = ""
         self.current_folder = os.path.dirname(__file__)
-        self.config: Optional[MateConfig] = None
+        self.config = None
         self.__findroot()
         self.api = MateAPI(self.config)
         self.run_params = None
 
     @staticmethod
     def init(project_name: str, *args, **kwargs):
         """
@@ -278,8 +277,8 @@
         self.api.install_url(url, *args, **kwargs)
 
     def __findroot(self):
         """
         Method in charge of finding the root folder of the project and reading the content of mate.json
         """
         self.root_folder, self.config = io.find_root()
-        self.root_save_folder = self.config.results_folder
+        # self.root_save_folder = self.config.results
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/mate_cli.py` & `yerbamate-0.9.22/packages/yerbamate/mate_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 **Example**
 
 ```
 mate init my_project venv=false
 ```
 
 """
-from .mate_config import MateConfig
 from .utils import print_markdown, remove_indent
 from .mate import Mate
 import inspect
 from typing import Optional, Callable, Sized
 import ipdb
 import os
 import sys
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/utils/__init__.py` & `yerbamate-0.9.22/packages/yerbamate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.21/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb  7 19:44:00 2023 UTC, .py size: 1433 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 00aa e263 9905 0000  o..........c....
+00000000: 6f0d 0d0a 0000 0000 e7c6 3164 9905 0000  o.........1d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 9000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c07 5a07 6400 6405 6c08 5a08 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6405 6c09 5a09 6406 650a 6602 6407 6408  d.l.Z.d.e.f.d.d.
@@ -27,15 +27,15 @@
 000001a0: 640b a101 4400 8301 a101 5300 290d 4e63  d...D.....S.).Nc
 000001b0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
 000001c0: 0400 0000 5300 0000 731c 0000 0067 007c  ....S...s....g.|
 000001d0: 005d 0a7d 017c 01a0 00a1 0064 006b 0372  .].}.|.....d.k.r
 000001e0: 027c 0191 0271 0253 0029 01da 0029 01da  .|...q.S.)...)..
 000001f0: 0573 7472 6970 2902 da02 2e30 da01 6ca9  .strip)....0..l.
 00000200: 0072 0b00 0000 fa3e 2f68 6f6d 652f 616c  .r.....>/home/al
-00000210: 2f47 6974 6875 622f 7965 7262 616d 6174  /Github/yerbamat
+00000210: 2f47 6974 4875 622f 7965 7262 616d 6174  /GitHub/yerbamat
 00000220: 652f 7061 636b 6167 6573 2f79 6572 6261  e/packages/yerba
 00000230: 6d61 7465 2f75 7469 6c73 2f5f 5f69 6e69  mate/utils/__ini
 00000240: 745f 5f2e 7079 da0a 3c6c 6973 7463 6f6d  t__.py..<listcom
 00000250: 703e 0e00 0000 7302 0000 001c 007a 2172  p>....s......z!r
 00000260: 656d 6f76 655f 696e 6465 6e74 2e3c 6c6f  emove_indent.<lo
 00000270: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
 00000280: 7201 0000 00e9 0100 0000 6301 0000 0000  r.........c.....
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc` & `yerbamate-0.9.22/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Sep 29 23:08:07 2022 UTC, .py size: 4419 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5725 3663 4311 0000  o.......W%6cC...
+00000000: 6f0d 0d0a 0000 0000 e7c6 3164 4311 0000  o.........1dC...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 e000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6401 6c04  ..d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6403 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6401 6c07 5a07 6404 6405 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6406 6407 8400 5a0a 650a 650b 8301  ..d.d...Z.e.e...
@@ -24,15 +24,15 @@
 00000170: 044e 6300 0000 0000 0000 0000 0000 0002  .Nc.............
 00000180: 0000 0004 0000 001f 0000 0073 1e00 0000  ...........s....
 00000190: 8801 6a00 730d 6401 8801 5f00 8800 7c00  ..j.s.d..._...|.
 000001a0: 6900 7c01 a401 8e01 5300 6400 5300 2902  i.|.....S.d.S.).
 000001b0: 4e54 a901 5a07 6861 735f 7275 6e29 02da  NT..Z.has_run)..
 000001c0: 0461 7267 73da 066b 7761 7267 73a9 02da  .args..kwargs...
 000001d0: 0466 756e 63da 0777 7261 7070 6572 a900  .func..wrapper..
-000001e0: fa3b 2f68 6f6d 652f 616c 2f47 6974 6875  .;/home/al/Githu
+000001e0: fa3b 2f68 6f6d 652f 616c 2f47 6974 4875  .;/home/al/GitHu
 000001f0: 622f 7965 7262 616d 6174 652f 7061 636b  b/yerbamate/pack
 00000200: 6167 6573 2f79 6572 6261 6d61 7465 2f75  ages/yerbamate/u
 00000210: 7469 6c73 2f75 7469 6c73 2e70 7972 0b00  tils/utils.pyr..
 00000220: 0000 0c00 0000 7308 0000 0006 0106 010e  ......s.........
 00000230: 0104 fe7a 156f 6e63 652e 3c6c 6f63 616c  ...z.once.<local
 00000240: 733e 2e77 7261 7070 6572 4672 0600 0000  s>.wrapperFr....
 00000250: 2901 720a 0000 0072 0c00 0000 7209 0000  ).r....r....r...
@@ -104,133 +104,133 @@
 00000670: 6561 7365 2073 656e 6420 7468 6520 6c6f  ease send the lo
 00000680: 6773 2061 6e64 206f 7065 6e20 616e 2069  gs and open an i
 00000690: 7373 7565 206f 6e20 6769 7468 7562 7a09  ssue on githubz.
 000006a0: 6d61 7465 2e6a 736f 6eda 0177 e904 0000  mate.json..w....
 000006b0: 0029 01da 0669 6e64 656e 747a 154d 6967  .)...indentz.Mig
 000006c0: 7261 7469 6f6e 2073 7563 6573 7366 756c  ration sucessful
 000006d0: 6c21 2910 da09 7965 7262 616d 6174 6572  l!)...yerbamater
-000006e0: 2700 0000 da00 7228 0000 00da 0c6d 6174  '.....r(.....mat
+000006e0: 2700 0000 da00 7228 0000 005a 0c6d 6174  '.....r(...Z.mat
 000006f0: 655f 7665 7273 696f 6e5a 094d 6967 7261  e_versionZ.Migra
 00000700: 7469 6f6e 5a07 6d69 6772 6174 65da 0945  tionZ.migrate..E
 00000710: 7863 6570 7469 6f6e da04 6f70 656e da02  xception..open..
 00000720: 6f73 da04 7061 7468 da04 6a6f 696e da04  os..path..join..
 00000730: 6a73 6f6e da04 6475 6d70 da05 7072 696e  json..dump..prin
 00000740: 7472 0500 0000 2906 7225 0000 0072 2600  tr....).r%...r&.
 00000750: 0000 7227 0000 0072 2800 0000 da07 7375  ..r'...r(.....su
 00000760: 6363 6573 73da 0166 720c 0000 0072 0c00  ccess..fr....r..
 00000770: 0000 720d 0000 00da 146d 6967 7261 7465  ..r......migrate
 00000780: 5f6d 6174 655f 7665 7273 696f 6e44 0000  _mate_versionD..
 00000790: 0073 2000 0000 0c02 0c01 0a02 0401 1003  .s .............
 000007a0: 0802 0401 0201 0201 04ff 0604 1602 1201  ................
-000007b0: 1cff 0803 0801 7239 0000 0072 3200 0000  ......r9...r2...
+000007b0: 1cff 0803 0801 7238 0000 0072 3100 0000  ......r8...r1...
 000007c0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
 000007d0: 0005 0000 0043 0000 0073 3600 0000 7c00  .....C...s6...|.
 000007e0: a000 6401 6402 a102 7d00 7401 7c00 9b00  ..d.d...}.t.|...
 000007f0: 6403 9d02 7c00 a002 6402 a101 6404 1900  d...|...d...d...
 00000800: 6701 6405 8d02 6a03 7d01 7404 7c01 6a05  g.d...j.}.t.|.j.
 00000810: 8301 5300 2906 4efa 012f da01 2e7a 062e  ..S.).N../...z..
 00000820: 6d6f 6465 6c72 0400 0000 2901 da08 6672  modelr....)...fr
 00000830: 6f6d 6c69 7374 2906 da07 7265 706c 6163  omlist)...replac
 00000840: 65da 0a5f 5f69 6d70 6f72 745f 5fda 0573  e..__import__..s
 00000850: 706c 6974 5a05 4d6f 6465 6c72 2400 0000  plitZ.Modelr$...
-00000860: da08 5f5f 696e 6974 5f5f 2902 7232 0000  ..__init__).r2..
+00000860: da08 5f5f 696e 6974 5f5f 2902 7231 0000  ..__init__).r1..
 00000870: 005a 0b6d 6f64 656c 5f63 6c61 7373 720c  .Z.model_classr.
 00000880: 0000 0072 0c00 0000 720d 0000 00da 1467  ...r....r......g
 00000890: 6574 5f6d 6f64 656c 5f70 6172 616d 6574  et_model_paramet
 000008a0: 6572 7373 0000 0073 1000 0000 0c01 0201  erss...s........
-000008b0: 0801 0e01 04fe 0203 02fd 0a04 7241 0000  ............rA..
+000008b0: 0801 0e01 04fe 0203 02fd 0a04 7240 0000  ............r@..
 000008c0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
 000008d0: 0000 0600 0000 4300 0000 7340 0000 0064  ......C...s@...d
 000008e0: 0164 0284 0064 0364 0284 0074 00a0 017c  .d...d.d...t...|
 000008f0: 00a1 0144 0083 0144 0083 017d 0174 006a  ...D...D...}.t.j
 00000900: 02a0 0374 006a 02a0 047c 0064 04a1 02a1  ...t.j...|.d....
 00000910: 0170 1f74 057c 0183 0164 056b 0253 0029  .p.t.|...d.k.S.)
 00000920: 064e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
 00000930: 0000 0005 0000 0053 0000 0073 1c00 0000  .......S...s....
 00000940: 6700 7c00 5d0a 7d01 7400 6a01 a002 7c01  g.|.].}.t.j...|.
 00000950: a101 7202 7c01 9102 7102 5300 720c 0000  ..r.|...q.S.r...
-00000960: 0029 0372 3100 0000 7232 0000 00da 0569  .).r1...r2.....i
+00000960: 0029 0372 3000 0000 7231 0000 00da 0569  .).r0...r1.....i
 00000970: 7364 6972 2902 da02 2e30 da01 7572 0c00  sdir)....0..ur..
 00000980: 0000 720c 0000 0072 0d00 0000 da0a 3c6c  ..r....r......<l
 00000990: 6973 7463 6f6d 703e 7d00 0000 7302 0000  istcomp>}...s...
 000009a0: 001c 007a 1b69 735f 6c65 6166 2e3c 6c6f  ...z.is_leaf.<lo
 000009b0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
 000009c0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
 000009d0: 0003 0000 0053 0000 0073 1000 0000 6700  .....S...s....g.
 000009e0: 7c00 5d04 7d01 7c01 9102 7102 5300 720c  |.].}.|...q.S.r.
-000009f0: 0000 0072 0c00 0000 a902 7243 0000 00da  ...r......rC....
+000009f0: 0000 0072 0c00 0000 a902 7242 0000 00da  ...r......rB....
 00000a00: 0170 720c 0000 0072 0c00 0000 720d 0000  .pr....r....r...
-00000a10: 0072 4500 0000 7d00 0000 7302 0000 0010  .rE...}...s.....
+00000a10: 0072 4400 0000 7d00 0000 7302 0000 0010  .rD...}...s.....
 00000a20: 00da 0772 6573 756c 7473 7201 0000 0029  ...resultsr....)
-00000a30: 0672 3100 0000 da07 6c69 7374 6469 7272  .r1.....listdirr
-00000a40: 3200 0000 da06 6578 6973 7473 7233 0000  2.....existsr3..
-00000a50: 00da 036c 656e 2902 7232 0000 00da 0863  ...len).r2.....c
+00000a30: 0672 3000 0000 da07 6c69 7374 6469 7272  .r0.....listdirr
+00000a40: 3100 0000 da06 6578 6973 7473 7232 0000  1.....existsr2..
+00000a50: 00da 036c 656e 2902 7231 0000 00da 0863  ...len).r1.....c
 00000a60: 6869 6c64 7265 6e72 0c00 0000 720c 0000  hildrenr....r...
 00000a70: 0072 0d00 0000 da07 6973 5f6c 6561 667c  .r......is_leaf|
-00000a80: 0000 0073 0400 0000 1e01 2201 724d 0000  ...s......".rM..
+00000a80: 0000 0073 0400 0000 1e01 2201 724c 0000  ...s......".rL..
 00000a90: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
 00000aa0: 0000 0400 0000 0300 0000 7340 0000 0087  ..........s@....
 00000ab0: 0066 0164 0164 0284 0874 00a0 0188 00a1  .f.d.d...t......
 00000ac0: 0144 0083 017d 0174 0274 0364 0364 0284  .D...}.t.t.d.d..
 00000ad0: 007c 0144 0083 0183 0183 017d 0274 0488  .|.D.......}.t..
 00000ae0: 0083 0173 1d7c 0253 0088 0067 0153 0029  ...s.|.S...g.S.)
 00000af0: 044e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
 00000b00: 0000 0006 0000 0013 0000 0073 1a00 0000  ...........s....
 00000b10: 6700 7c00 5d09 7d01 7400 6a01 a002 8800  g.|.].}.t.j.....
 00000b20: 7c01 a102 9102 7102 5300 720c 0000 0029  |.....q.S.r....)
-00000b30: 0372 3100 0000 7232 0000 0072 3300 0000  .r1...r2...r3...
-00000b40: 7246 0000 00a9 0172 3200 0000 720c 0000  rF.....r2...r...
-00000b50: 0072 0d00 0000 7245 0000 0082 0000 0073  .r....rE.......s
+00000b30: 0372 3000 0000 7231 0000 0072 3200 0000  .r0...r1...r2...
+00000b40: 7245 0000 00a9 0172 3100 0000 720c 0000  rE.....r1...r...
+00000b50: 0072 0d00 0000 7244 0000 0082 0000 0073  .r....rD.......s
 00000b60: 0200 0000 1a00 7a22 6765 745f 6c65 6176  ......z"get_leav
 00000b70: 6573 5f72 6563 2e3c 6c6f 6361 6c73 3e2e  es_rec.<locals>.
 00000b80: 3c6c 6973 7463 6f6d 703e 6301 0000 0000  <listcomp>c.....
 00000b90: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
 00000ba0: 0000 0073 2c00 0000 6700 7c00 5d12 7d01  ...s,...g.|.].}.
 00000bb0: 7400 6a01 a002 7c01 a101 7202 6400 7c01  t.j...|...r.d.|.
 00000bc0: 7601 7202 7403 7c01 8301 6401 1900 9102  v.r.t.|...d.....
 00000bd0: 7102 5300 2902 da02 5f5f 7201 0000 0029  q.S.)...__r....)
-00000be0: 0472 3100 0000 7232 0000 0072 4200 0000  .r1...r2...rB...
+00000be0: 0472 3000 0000 7231 0000 0072 4100 0000  .r0...r1...rA...
 00000bf0: da0e 6765 745f 6c65 6176 6573 5f72 6563  ..get_leaves_rec
-00000c00: 2902 7243 0000 00da 0173 720c 0000 0072  ).rC.....sr....r
-00000c10: 0c00 0000 720d 0000 0072 4500 0000 8400  ....r....rE.....
-00000c20: 0000 7302 0000 002c 0029 0572 3100 0000  ..s....,.).r1...
-00000c30: 7249 0000 00da 046c 6973 7472 0300 0000  rI.....listr....
-00000c40: 724d 0000 0029 0372 3200 0000 da03 7375  rM...).r2.....su
-00000c50: 62da 0464 6972 7372 0c00 0000 724e 0000  b..dirsr....rN..
-00000c60: 0072 0d00 0000 7250 0000 0081 0000 0073  .r....rP.......s
-00000c70: 0a00 0000 1801 0201 1001 04ff 1203 7250  ..............rP
+00000c00: 2902 7242 0000 00da 0173 720c 0000 0072  ).rB.....sr....r
+00000c10: 0c00 0000 720d 0000 0072 4400 0000 8400  ....r....rD.....
+00000c20: 0000 7302 0000 002c 0029 0572 3000 0000  ..s....,.).r0...
+00000c30: 7248 0000 00da 046c 6973 7472 0300 0000  rH.....listr....
+00000c40: 724c 0000 0029 0372 3100 0000 da03 7375  rL...).r1.....su
+00000c50: 62da 0464 6972 7372 0c00 0000 724d 0000  b..dirsr....rM..
+00000c60: 0072 0d00 0000 724f 0000 0081 0000 0073  .r....rO.......s
+00000c70: 0a00 0000 1801 0201 1001 04ff 1203 724f  ..............rO
 00000c80: 0000 0072 1d00 0000 da07 6461 7461 7365  ...r......datase
 00000c90: 7463 0200 0000 0000 0000 0000 0000 0500  tc..............
 00000ca0: 0000 0800 0000 4300 0000 7362 0000 0074  ......C...sb...t
 00000cb0: 006a 01a0 027c 0064 017c 019b 0064 029d  .j...|.d.|...d..
 00000cc0: 02a1 037d 0274 006a 01a0 037c 02a1 0172  ...}.t.j...|...r
 00000cd0: 2d74 047c 0283 018f 0e7d 0374 05a0 067c  -t.|.....}.t...|
 00000ce0: 03a1 017d 0457 0064 0004 0004 0083 0301  ...}.W.d........
 00000cf0: 007c 0453 0031 0073 2677 0101 0001 0001  .|.S.1.s&w......
 00000d00: 0059 0001 007c 0453 0074 077c 0083 0153  .Y...|.S.t.|...S
 00000d10: 0029 034e 7219 0000 007a 052e 6a73 6f6e  .).Nr....z..json
-00000d20: 2908 7231 0000 0072 3200 0000 7233 0000  ).r1...r2...r3..
-00000d30: 0072 4a00 0000 7230 0000 0072 3400 0000  .rJ...r0...r4...
-00000d40: da04 6c6f 6164 7241 0000 0029 0572 3200  ..loadrA...).r2.
-00000d50: 0000 7255 0000 0072 2500 0000 7238 0000  ..rU...r%...r8..
+00000d20: 2908 7230 0000 0072 3100 0000 7232 0000  ).r0...r1...r2..
+00000d30: 0072 4900 0000 722f 0000 0072 3300 0000  .rI...r/...r3...
+00000d40: da04 6c6f 6164 7240 0000 0029 0572 3100  ..loadr@...).r1.
+00000d50: 0000 7254 0000 0072 2500 0000 7237 0000  ..rT...r%...r7..
 00000d60: 00da 0672 6573 756c 7472 0c00 0000 720c  ...resultr....r.
 00000d70: 0000 0072 0d00 0000 da0e 6765 745f 7061  ...r......get_pa
 00000d80: 7261 6d65 7465 7273 8900 0000 7312 0000  rameters....s...
 00000d90: 0016 020c 010a 010c 010a ff04 0210 fe04  ................
-00000da0: 0208 0272 5800 0000 da08 5f5f 6d61 696e  ...rX.....__main
+00000da0: 0208 0272 5700 0000 da08 5f5f 6d61 696e  ...rW.....__main
 00000db0: 5f5f 5a04 6369 616f 2902 4646 2901 721d  __Z.ciao).FF).r.
 00000dc0: 0000 0029 1772 1700 0000 da06 7479 7069  ...).r......typi
-00000dd0: 6e67 7202 0000 00da 0469 7064 6272 3100  ngr......ipdbr1.
+00000dd0: 6e67 7202 0000 00da 0469 7064 6272 3000  ngr......ipdbr0.
 00000de0: 0000 da09 6974 6572 746f 6f6c 7372 0300  ....itertoolsr..
-00000df0: 0000 7234 0000 00da 0562 756e 6368 7205  ..r4.....bunchr.
-00000e00: 0000 0072 0e00 0000 7236 0000 00da 0a70  ...r....r6.....p
+00000df0: 0000 7233 0000 00da 0562 756e 6368 7205  ..r3.....bunchr.
+00000e00: 0000 0072 0e00 0000 7235 0000 00da 0a70  ...r....r5.....p
 00000e10: 7269 6e74 5f6f 6e63 65da 0464 6963 74da  rint_once..dict.
 00000e20: 0462 6f6f 6c72 2400 0000 da03 7374 7272  .boolr$.....strr
-00000e30: 3900 0000 7241 0000 0072 4d00 0000 7250  9...rA...rM...rP
-00000e40: 0000 0072 5800 0000 da08 5f5f 6e61 6d65  ...rX.....__name
+00000e30: 3800 0000 7240 0000 0072 4c00 0000 724f  8...r@...rL...rO
+00000e40: 0000 0072 5700 0000 da08 5f5f 6e61 6d65  ...rW.....__name
 00000e50: 5f5f 720c 0000 0072 0c00 0000 720c 0000  __r....r....r...
 00000e60: 0072 0d00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
 00000e70: 0100 0000 7338 0000 0008 000c 0108 0108  ....s8..........
 00000e80: 010c 0108 010c 0208 0308 0a02 0602 0104  ................
 00000e90: fc02 0102 ff02 0202 fe02 0302 fd02 040a  ................
 00000ea0: fc12 2c0e 2f0e 090e 0514 0808 1010 0104  ..,./...........
 00000eb0: ff                                       .
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/utils/bunch.py` & `yerbamate-0.9.22/packages/yerbamate/utils/bunch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,68 @@
 from types import SimpleNamespace
 
 import json
 import ipdb
 
 
 class Bunch(dict):
-    def __init__(self, kwargs):
-        super().__init__(kwargs)
-        for key, val in kwargs.items():
-            self.__dict__[key] = val if not isinstance(val, dict) else Bunch(val)
+    def __init__(self, dict):
+        super().__init__(dict)
 
-    def to_dict(self):
-        proto = self.__dict__.copy()
-        for key, val in proto.items():
-            proto[key] = val if not isinstance(val, Bunch) else val.to_dict()
-        return proto
+        self.__original_dict = dict
 
-    def contains(self, key):
-        return key in self.keys()
-
-    def has(self, key):
-        return self.contains(key)
-
-    def is_empty(self):
-        return len(self.keys()) == 0
-
-    def clone(self):
-        return Bunch(self.to_dict())
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=4, default=str)
-
-    def __setattr__(self, key, value):
-        self.__setitem__(key, value)
-
-    def __dir__(self):
-        return self.keys()
-
-    def __getattr__(self, key):
-        return self.__getitem__(key)
-
-    def __setitem__(self, key, value):
-        super().__setitem__(key, value)
-        self.__dict__[key] = value
-
-    def __getitem__(self, key):
-        return super().__getitem__(key)
+        for key, val in dict.items():
+            self.__dict__[key] = val
+            self.__setattr__(key, val)
+        
+        
+        # for key, val in kwargs.items():
+        #     self.__dict__[key] = val if not isinstance(val, dict) else Bunch(val)
+
+    # def to_dict(self):
+    #     proto = self.__dict__.copy()
+    #     for key, val in proto.items():
+    #         proto[key] = val if not isinstance(val, Bunch) else val.to_dict()
+    #     return proto
+
+    # def contains(self, key):
+    #     return key in self.keys()
+
+    # def has(self, key):
+    #     return self.contains(key)
+
+    # def is_empty(self):
+    #     return len(self.keys()) == 0
+
+    # def clone(self):
+    #     return Bunch(self.to_dict())
+
+    # def __str__(self):
+    #     return json.dumps(self.to_dict(), indent=4, default=str)
+
+    # def __setattr__(self, key, value):
+    #     self.__setitem__(key, value)
+
+    # def __dir__(self):
+    #     return self.keys()
+
+    # def __getattr__(self, key):
+    #     return self.__getitem__(key)
+
+    # def __setitem__(self, key, value):
+    #     super().__setitem__(key, value)
+    #     self.__dict__[key] = value
+
+    # def __getitem__(self, key):
+    #     if key in self.__dict__:
+    #         return self.__dict__[key]
+    #     else:
+    #         if hasattr(self, key):
+    #             return getattr(self, key)
+    #     return super().__getitem__(key)
 
     def __setstate__(self, state):
         # Bunch pickles generated with scikit-learn 0.16.* have an non
         # empty __dict__. This causes a surprising behaviour when
         # loading these pickles scikit-learn 0.17: reading bunch.key
         # uses __dict__ but assigning to bunch.key use __setattr__ and
         # only changes bunch['key']. More details can be found at:
```

### Comparing `yerbamate-0.9.21/packages/yerbamate/utils/git_url_parser.py` & `yerbamate-0.9.22/packages/yerbamate/utils/git_url_parser.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.21/packages/yerbamate/utils/utils.py` & `yerbamate-0.9.22/packages/yerbamate/utils/utils.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.21/packages/yerbamate/yerbamate.egg-info/PKG-INFO` & `yerbamate-0.9.22/packages/yerbamate/yerbamate.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.21/packages/yerbamate.egg-info/PKG-INFO` & `yerbamate-0.9.22/packages/yerbamate.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yerbamate
-Version: 0.9.21
+Version: 0.9.22
 Summary:  A python module and experiment manager for deep learning
 Home-page: https://github.com/oalee/yerbamate
 Author: Giulio Zani, Ali Rahimi
 Author-email: yerba.mate.dl@proton.me
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -12,44 +12,51 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1 style="color:green"><span style="color:green">Maté 🧉</span> your friendly AI project and experiment manager</h1>
+<h1 style="color:green"><span style="color:green">Maté 🧉</span> your modular AI project and experiment manager</h1>
 
-Maté is a python project, package and experiment manager. Whether you are a
+<!-- Maté is a python project, package and experiment manager. Whether you are a
 seasoned deep learning researcher or just starting out, Maté provides you with
 the tools to easily add source code and dependencies of models, trainers, and
 data loaders to your projects. With Maté, you can also evaluate, train, and keep
-track of your experiments with ease 🚀
+track of your experiments with ease 🚀 -->
+### Welcome to [Maté](https://github.com/oalee/yerbamate)! 🎉👋🏼
 
-## Features 🎉
+Maté is an open science modular Python framework designed to streamline and simplify the development and management of machine learning projects. It was developed to address the reproducibility crisis in artificial intelligence research by promoting open science and accessible AI. 🌍💻
+
+The framework is built around the best software engineering practices of modularity and separation of concerns, encouraging quality coding, collaboration, and the sharing of models, trainers, data loaders, and knowledge. The modular design and separation of concerns simplify the development and maintenance of machine learning models, leading to an improved developer experience. 🚀💻👨‍💻💬🧠
+
+With Maté, you can easily install the source code of open-source projects and adhere to modularity and separation of concerns, making your models and modules sharable out of the box. This means you can collaborate more effectively with others and easily share your work. 📦💻🤝
 
-- Seamless integration with any installed python library such as PyTorch/Lightning,
-  TensorFlow/Keras, JAX/Flax, Huggingface/transformers.
-- Easy to use interface to add source code of models, trainers, and data loaders
-  to your projects.
-- Support for full customizability and reproducibility of results through the
-  inclusion of dependencies in your project.
-- Modular project structure that enforces a clean and organized codebase.
-- Fully compatible with python. 
-- Convenient environment management through the Maté Environment API.
-- Support for pip and conda for dependency management.
-- Works with Colab.
+Thank you for choosing Maté, and we can't wait to see the amazing machine learning projects you'll create with it! 🎉👨‍💻🌟
+
+## Features 🎉
+- Seamless integration with any python library such as PyTorch/Lightning, TensorFlow/Keras, JAX/Flax, Huggingface/transformers. 🤝🤗🐉
+- Easy to use interface to add source code of models, trainers, and data loaders to your projects. 🎨💻📝
+- Support for full customizability and reproducibility of results through the inclusion of dependencies in your project. 🌟🔍🧪
+- Modular project structure that enforces a clean and organized codebase. 🧱👨‍💻👌
+- Fully compatible with python. No need to use mate commands to run your experiments. 🐍💻🚀
+- Convenient environment management through the Maté Environment API. 🌍👨‍💻🔧
+- Support for pip and conda for dependency management. 📦🔍💻
+- Works with [Colab](https://github.com/oalee/yerbamate/blob/main/deep_learning.ipynb) out of the box.  🎉👌🤖
 
 ## Table of Contents
 
-- [Installation](#installation-🔌)
-- [Quick Start](#quick-start-⚡)
-- [Project Structure](#project-structure-📁)
-- [Example Projects](#example-projects-📚)
-- [Documentation](https://oalee.github.io/yerbamate/)
-- [Contribution](#Contribution-🤝)
+- [Installation](#installation-)
+- [Quick Start](#quick-start-)
+- [Project Structure](#project-structure-)
+- [Example Projects](#example-projects-)
+- [Documentation](#documentation-)
+- [Contribution](#Contribution-)
+- [Guides](#guides-)
+- [Open Science](#open-science-)
 
 ## Installation 🔌
 
 ```bash
 pip install yerbamate
 ```
 
@@ -75,15 +82,15 @@
 |   |-- __init__.py
 ```
 
 ### **Install an experiment**
 
 To install an experiment, you can use `mate install` to install a module and its
 dependencies from a github repository. See
-[docs](https://oalee.github.io/yerbamate/#/?id=install) for more details.
+[docs](https://oalee.github.io/yerbamate/#/?id=mate-install) for more details.
 
 ```bash
 # Short version of GitHub URL https://github.com/oalee/big_transfer/tree/master/big_transfer/experiments/bit
 mate install oalee/big_transfer/experiments/bit -yo pip
 
 # Short version of GitHub URL https://github.com/oalee/deep-vision/tree/main/deepnet/experiments/resnet
 mate install oalee/deep-vision/deepnet/experiments/resnet -yo pip
@@ -100,17 +107,25 @@
 mate install oalee/big_transfer/models/bit -yo pip
 mate install oalee/deep-vision/deepnet/models/vit_pytorch -yo pip
 mate install oalee/deep-vision/deepnet/trainers/classification -yo pip
 ```
 
 ### **Setting up environment**
 
-Take a look at
-[Environment API](https://oalee.github.io/yerbamate#maté-environment-api) and
-set up your environment before running your experiments.
+Set up your environment before running your experiments. This can be done by using shell, or `env.json` file in the root of your project. Maté API requires `results` to be set in the environment. For more information, see [docs](https://oalee.github.io/yerbamate/#/?id=mat%c3%a9-environment-api).
+```bash
+DATA_PATH=/path/to/data
+results=/path/to/results
+```
+```json
+{
+    "DATA_PATH": "/path/to/data",
+    "results": "/path/to/results"
+}
+```
 
 ### **Train a model**
 
 To train a model, you can use the `mate train` command. This command will train
 the model with the specified experiment. For example, to train the an experiment
 called `learn` in the `bit` module, you can use the following command:
 
@@ -121,37 +136,51 @@
 ```
 
 ## Project Structure 📁
 
 Deep learning projects can be organized into the following structure with
 modularity and seperation of concerns in mind. This offers a clean and organized
 codebase that is easy to maintain and is sharable out-of-the-box.
+The modular structure of the framework involves organizing the project directory in a hierarchical tree structure, with an arbitrary name given to the root project directory by the user. The project is then broken down into distinct concerns such as models, data, trainers, experiments, analyzers, and simulators, each with its own subdirectory. Within each concern, modules can be defined with their own subdirectories, such as specific models, trainers, data loaders, data augmentations, or loss functions.
 
 ```bash
-/
-|-- models/
-|   |-- __init__.py
-|-- experiments/
-|   |-- __init__.py
-|-- trainers/
-|   |-- __init__.py
-|-- data/
-|   |-- __init__.py
+└── project_name
+    ├── data
+    │   ├── my_independent_data_loader
+    │   └── __init__.py
+    ├── experiments
+    │   ├── my_awesome_experiment
+    │   └── __init__.py
+    ├── __init__.py
+    ├── models
+    │   ├── awesomenet
+    │   └── __init__.py
+    └── trainers
+        ├── big_brain_trainer
+        └── __init__.py
 ```
 
 ### Modularity
 
 Modularity is a software design principle that focuses on creating
 self-contained, reusable and interchangeable components. In the context of a
 deep learning project, modularity means creating three independent standalone
 modules for models, trainers and data. This allows for a more organized,
 maintainable and sharable project structure. The forth module, experiments, is
 not independent, but rather combines the three modules together to create a
 complete experiment.
 
+### Independent Modules
+
+Yerbamate prioritizes the organization of the project into independent modules when applicable. Independent modules only depend on Python dependencies (such as NumPy, PyTorch, TensorFlow, or Hugging Face), and the code inside the module uses relative imports to import within the module. This makes it an independent module that can be re-used when Python dependencies are installed.
+
+### Non-Independent Modules
+In some cases, a combination of independent modules may be necessary for a particular concern. An example of this is the experiment concern, which imports and combines models, data, and trainers to define and create a specific experiment. In such cases, the module is not independent and is designed to combine the previously defined independent modules. In the case of non-independent modules, Yerbamate creates a dependency list of independent modules that can be used to install the code and Python dependencies. This ensures that the necessary modules are installed, and that the code can be run without issue.
+
+
 ### Sample Modular Project Structure
 
 This structure highlights modularity and seperation of concerns. The `models`,
 `data` and `trainers` modules are independent and can be used in any project.
 The `experiments` module is not independent, but rather combines the three
 modules together to create a complete experiment.
 
@@ -196,33 +225,38 @@
         │   ├── requirements.txt
         │   └── trainer.py
         └── __init__.py
 ```
 
 ## Example Projects 📚
 
-Please check out the [transfer learning](https://github.com/oalee/big-transfer),
+Please check out the [transfer learning](https://github.com/oalee/big_transfer),
 [vision models](https://github.com/oalee/deep-vision), and
 [lightweight gan](https://github.com/oalee/lightweight-gan).
 
 ## Documentation 📚
 
 Please check out the [documentation](https://oalee.github.io/yerbamate).
 
 ## Guides 📖
 
 For more information on modularity, please check out this [guide](https://medium.com/@alee.rmi/the-ultimate-deep-learning-project-structure-a-software-engineers-guide-into-the-land-of-ai-c383f234fd2f).
 
 For running experiments on Google Colab, please check out this
-[example](https://colab.research.google.com/gist/oalee/5f5c2b3bb2da4ec3168f3edd4a52056a/deep-learning.ipynb)
+[example](https://github.com/oalee/yerbamate/blob/main/deep_learning.ipynb)
 
 ## Contribution 🤝
 
 We welcome contributions from the community! Please check out our
 [contributing](https://github.com/oalee/yerbamate/blob/main/CONTRIBUTING.md)
 guide for more information on how to get started.
 
 ## Contact 🤝
 
 For questions please contact:
 
-yerba.mate.dl(at)proton.me
+oalee(at)proton.me
+
+
+## Open Science 📖
+
+As an open science work, Yerbamate strives to promote the principles of transparency and collaboration. To this end, the history of the LaTeX files for work are available on [GitHub](https://github.com/oalee/os-yerbamate). These open science repositories are open to collaboration and encourage participation from the community to enhance the validity, reproducibility, accessibility, and quality of this work.
```

### Comparing `yerbamate-0.9.21/packages/yerbamate.egg-info/SOURCES.txt` & `yerbamate-0.9.22/packages/yerbamate.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,50 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 ./src/mate
-./src/mateboard
 packages/requirements.txt
 packages/yerbamate/__init__.py
 packages/yerbamate/constants.py
 packages/yerbamate/environment.py
 packages/yerbamate/mate.py
 packages/yerbamate/mate_cli.py
-packages/yerbamate/mate_config.py
 packages/yerbamate.egg-info/PKG-INFO
 packages/yerbamate.egg-info/SOURCES.txt
 packages/yerbamate.egg-info/dependency_links.txt
 packages/yerbamate.egg-info/requires.txt
 packages/yerbamate.egg-info/top_level.txt
 packages/yerbamate/__pycache__/__init__.cpython-310.pyc
-packages/yerbamate/__pycache__/backbone_type.cpython-310.pyc
 packages/yerbamate/__pycache__/environment.cpython-310.pyc
 packages/yerbamate/__pycache__/mate.cpython-310.pyc
 packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc
-packages/yerbamate/__pycache__/mate_config.cpython-310.pyc
-packages/yerbamate/__pycache__/package.cpython-310.pyc
 packages/yerbamate/api/__init__.py
 packages/yerbamate/api/mate_api.py
 packages/yerbamate/api/__pycache__/__init__.cpython-310.pyc
 packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc
-packages/yerbamate/api/__pycache__/package.cpython-310.pyc
-packages/yerbamate/api/__pycache__/package_manager.cpython-310.pyc
-packages/yerbamate/api/__pycache__/package_repository.cpython-310.pyc
-packages/yerbamate/api/__pycache__/socket.cpython-310.pyc
 packages/yerbamate/api/data/__init__.py
 packages/yerbamate/api/data/module_manager.py
 packages/yerbamate/api/data/module_repository.py
 packages/yerbamate/api/data/package.py
 packages/yerbamate/api/data/__pycache__/__init__.cpython-310.pyc
 packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc
 packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc
 packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc
-packages/yerbamate/api/data/__pycache__/package_manager.cpython-310.pyc
-packages/yerbamate/api/data/__pycache__/package_repository.cpython-310.pyc
 packages/yerbamate/api/data/sources/__init__.py
 packages/yerbamate/api/data/sources/source.py
 packages/yerbamate/api/data/sources/__pycache__/__init__.cpython-310.pyc
-packages/yerbamate/api/data/sources/__pycache__/local.cpython-310.pyc
-packages/yerbamate/api/data/sources/__pycache__/remote.cpython-310.pyc
 packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc
 packages/yerbamate/api/data/sources/local/__init__.py
 packages/yerbamate/api/data/sources/local/io.py
 packages/yerbamate/api/data/sources/local/local.py
 packages/yerbamate/api/data/sources/local/__pycache__/__init__.cpython-310.pyc
 packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc
 packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc
-packages/yerbamate/api/data/sources/local/__pycache__/server.cpython-310.pyc
 packages/yerbamate/api/data/sources/remote/__init__.py
 packages/yerbamate/api/data/sources/remote/remote.py
 packages/yerbamate/api/data/sources/remote/__pycache__/__init__.cpython-310.pyc
 packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc
 packages/yerbamate/api/data/utils/__init__.py
 packages/yerbamate/api/data/utils/exp_util.py
 packages/yerbamate/api/data/utils/git_util.py
@@ -69,14 +55,12 @@
 packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc
 packages/yerbamate/utils/__init__.py
 packages/yerbamate/utils/bunch.py
 packages/yerbamate/utils/git_url_parser.py
 packages/yerbamate/utils/utils.py
 packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc
 packages/yerbamate/utils/__pycache__/bunch.cpython-310.pyc
-packages/yerbamate/utils/__pycache__/git_url_parser.cpython-310.pyc
-packages/yerbamate/utils/__pycache__/migrator.cpython-310.pyc
 packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc
 packages/yerbamate/yerbamate.egg-info/PKG-INFO
 packages/yerbamate/yerbamate.egg-info/SOURCES.txt
 packages/yerbamate/yerbamate.egg-info/dependency_links.txt
 packages/yerbamate/yerbamate.egg-info/top_level.txt
```

### Comparing `yerbamate-0.9.21/setup.py` & `yerbamate-0.9.22/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 setup(
     name="yerbamate",
     description=" A python module and experiment manager for deep learning",
     author="Giulio Zani, Ali Rahimi",
     author_email="yerba.mate.dl@proton.me",
     url="https://github.com/oalee/yerbamate",
     python_requires=">=3.9",
-    version="0.9.21",
+    version="0.9.22",
     packages=find_packages("packages", exclude=["tests"]),
     include_package_data=True,
     package_dir={"": "packages/"},
     license="Apache License 2.0",
     license_files=("LICENSE",),
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -25,14 +25,15 @@
         "GitPython",
         "validators",
         "ipdb",
         "pipreqs",
         "dirhash",
         "rich",
         "docstring-parser",
+        "tabulate"
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

