# Comparing `tmp/py-Ayra-8.2.5.tar.gz` & `tmp/py-Ayra-8.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayra-8.2.5.tar", last modified: Sat Apr 22 17:08:42 2023, max compression
+gzip compressed data, was "py-Ayra-8.2.6.tar", last modified: Sat Apr 22 17:44:41 2023, max compression
```

## Comparing `py-Ayra-8.2.5.tar` & `py-Ayra-8.2.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 17:08:42.022357 py-Ayra-8.2.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 17:08:42.018357 py-Ayra-8.2.5/Ayra/
--rw-r--r--   0 root         (0) root         (0)     3077 2023-04-22 17:06:15.000000 py-Ayra-8.2.5/Ayra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2824 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 17:08:42.018357 py-Ayra-8.2.5/Ayra/_misc/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/_misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4800 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/_misc/_assistant.py
--rw-r--r--   0 root         (0) root         (0)    12369 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/_misc/_decorators.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/_misc/_supporter.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/_misc/_wrappers.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-04-20 13:04:25.000000 py-Ayra-8.2.5/Ayra/configs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 17:08:42.018357 py-Ayra-8.2.5/Ayra/dB/
--rw-r--r--   0 root         (0) root         (0)     1951 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/__init__.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/_core.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/afk_db.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/antiflood_db.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/asst_fns.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/asstcmd_db.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/autoban_db.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/blacklist_chat_db.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/botchat_db.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/broadcast_db.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/ch_db.py
--rw-r--r--   0 root         (0) root         (0)      618 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/dnd_db.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/echo_db.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/filestore_db.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/filter_db.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/forcesub_db.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/gban_mute_db.py
--rw-r--r--   0 root         (0) root         (0)      639 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/gcast_blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/greetings_db.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/logusers_db.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/mute_db.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/night_db.py
--rw-r--r--   0 root         (0) root         (0)     1192 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/notes_db.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/nsfw_db.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/pmpermit_db.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/snips_db.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/vc_sudos.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/dB/warn_db.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 17:08:42.022357 py-Ayra-8.2.5/Ayra/fns/
--rw-r--r--   0 root         (0) root         (0)    12365 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/fns/FastTelethon.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/fns/admins.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/fns/executor.py
--rw-r--r--   0 root         (0) root         (0)     9150 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/fns/gDrive.py
--rw-r--r--   0 root         (0) root         (0)    43096 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/fns/google_image.py
--rw-r--r--   0 root         (0) root         (0)    19948 2023-04-22 17:06:15.000000 py-Ayra-8.2.5/Ayra/fns/helper.py
--rw-r--r--   0 root         (0) root         (0)     7427 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/fns/info.py
--rw-r--r--   0 root         (0) root         (0)    17343 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/fns/misc.py
--rw-r--r--   0 root         (0) root         (0)    25519 2023-04-22 17:06:15.000000 py-Ayra-8.2.5/Ayra/fns/tools.py
--rw-r--r--   0 root         (0) root         (0)     8262 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/fns/ytdl.py
--rw-r--r--   0 root         (0) root         (0)     9174 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/kynan.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 17:08:42.022357 py-Ayra-8.2.5/Ayra/startup/
--rw-r--r--   0 root         (0) root         (0)     8452 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/startup/BaseClient.py
--rw-r--r--   0 root         (0) root         (0)     2596 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/startup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9774 2023-04-20 13:10:06.000000 py-Ayra-8.2.5/Ayra/startup/_database.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/startup/_extra.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/startup/connections.py
--rw-r--r--   0 root         (0) root         (0)    18429 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/startup/funcs.py
--rw-r--r--   0 root         (0) root         (0)     2284 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/startup/loader.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/Ayra/startup/utils.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-22 17:06:15.000000 py-Ayra-8.2.5/Ayra/version.py
--rw-r--r--   0 root         (0) root         (0)    35182 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3387 2023-04-22 17:08:42.022357 py-Ayra-8.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2570 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 17:08:42.022357 py-Ayra-8.2.5/py_Ayra.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3387 2023-04-22 17:08:41.000000 py-Ayra-8.2.5/py_Ayra.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1466 2023-04-22 17:08:41.000000 py-Ayra-8.2.5/py_Ayra.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 17:08:41.000000 py-Ayra-8.2.5/py_Ayra.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 17:08:41.000000 py-Ayra-8.2.5/py_Ayra.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-22 17:08:41.000000 py-Ayra-8.2.5/py_Ayra.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 17:08:42.022357 py-Ayra-8.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1496 2023-04-19 16:51:17.000000 py-Ayra-8.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 17:44:40.995589 py-Ayra-8.2.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 17:44:40.991589 py-Ayra-8.2.6/Ayra/
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-04-22 17:06:15.000000 py-Ayra-8.2.6/Ayra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 17:44:40.991589 py-Ayra-8.2.6/Ayra/_misc/
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/_misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4800 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/_misc/_assistant.py
+-rw-r--r--   0 root         (0) root         (0)    12369 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/_misc/_decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/_misc/_supporter.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/_misc/_wrappers.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-04-20 13:04:25.000000 py-Ayra-8.2.6/Ayra/configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 17:44:40.995589 py-Ayra-8.2.6/Ayra/dB/
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/_core.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/afk_db.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/antiflood_db.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/asst_fns.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/asstcmd_db.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/autoban_db.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/blacklist_chat_db.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/botchat_db.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/broadcast_db.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/ch_db.py
+-rw-r--r--   0 root         (0) root         (0)      618 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/dnd_db.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/echo_db.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/filestore_db.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/filter_db.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/forcesub_db.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/gban_mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      639 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/gcast_blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/greetings_db.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/logusers_db.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/night_db.py
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/notes_db.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/nsfw_db.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/pmpermit_db.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/snips_db.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/vc_sudos.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/dB/warn_db.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 17:44:40.995589 py-Ayra-8.2.6/Ayra/fns/
+-rw-r--r--   0 root         (0) root         (0)    12365 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/fns/FastTelethon.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/fns/admins.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/fns/executor.py
+-rw-r--r--   0 root         (0) root         (0)     9150 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/fns/gDrive.py
+-rw-r--r--   0 root         (0) root         (0)    43096 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/fns/google_image.py
+-rw-r--r--   0 root         (0) root         (0)    19948 2023-04-22 17:06:15.000000 py-Ayra-8.2.6/Ayra/fns/helper.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/fns/info.py
+-rw-r--r--   0 root         (0) root         (0)    17343 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/fns/misc.py
+-rw-r--r--   0 root         (0) root         (0)    25348 2023-04-22 17:43:43.000000 py-Ayra-8.2.6/Ayra/fns/tools.py
+-rw-r--r--   0 root         (0) root         (0)     8262 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/fns/ytdl.py
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/kynan.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 17:44:40.995589 py-Ayra-8.2.6/Ayra/startup/
+-rw-r--r--   0 root         (0) root         (0)     8452 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/startup/BaseClient.py
+-rw-r--r--   0 root         (0) root         (0)     2596 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/startup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2023-04-20 13:10:06.000000 py-Ayra-8.2.6/Ayra/startup/_database.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/startup/_extra.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/startup/connections.py
+-rw-r--r--   0 root         (0) root         (0)    18429 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/startup/funcs.py
+-rw-r--r--   0 root         (0) root         (0)     2284 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/startup/loader.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/Ayra/startup/utils.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-22 17:43:43.000000 py-Ayra-8.2.6/Ayra/version.py
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-04-22 17:44:40.995589 py-Ayra-8.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 17:44:40.995589 py-Ayra-8.2.6/py_Ayra.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-04-22 17:44:40.000000 py-Ayra-8.2.6/py_Ayra.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-04-22 17:44:40.000000 py-Ayra-8.2.6/py_Ayra.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 17:44:40.000000 py-Ayra-8.2.6/py_Ayra.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 17:44:40.000000 py-Ayra-8.2.6/py_Ayra.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-22 17:44:40.000000 py-Ayra-8.2.6/py_Ayra.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 17:44:40.999589 py-Ayra-8.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-04-19 16:51:17.000000 py-Ayra-8.2.6/setup.py
```

### Comparing `py-Ayra-8.2.5/Ayra/__init__.py` & `py-Ayra-8.2.6/Ayra/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/__main__.py` & `py-Ayra-8.2.6/Ayra/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/_misc/__init__.py` & `py-Ayra-8.2.6/Ayra/_misc/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/_misc/_assistant.py` & `py-Ayra-8.2.6/Ayra/_misc/_assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/_misc/_decorators.py` & `py-Ayra-8.2.6/Ayra/_misc/_decorators.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/_misc/_supporter.py` & `py-Ayra-8.2.6/Ayra/_misc/_supporter.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/_misc/_wrappers.py` & `py-Ayra-8.2.6/Ayra/_misc/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/configs.py` & `py-Ayra-8.2.6/Ayra/configs.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/__init__.py` & `py-Ayra-8.2.6/Ayra/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/afk_db.py` & `py-Ayra-8.2.6/Ayra/dB/afk_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/antiflood_db.py` & `py-Ayra-8.2.6/Ayra/dB/antiflood_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/asst_fns.py` & `py-Ayra-8.2.6/Ayra/dB/asst_fns.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/asstcmd_db.py` & `py-Ayra-8.2.6/Ayra/dB/asstcmd_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/autoban_db.py` & `py-Ayra-8.2.6/Ayra/dB/autoban_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/blacklist_db.py` & `py-Ayra-8.2.6/Ayra/dB/blacklist_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/botchat_db.py` & `py-Ayra-8.2.6/Ayra/dB/botchat_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/broadcast_db.py` & `py-Ayra-8.2.6/Ayra/dB/broadcast_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/ch_db.py` & `py-Ayra-8.2.6/Ayra/dB/ch_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/dnd_db.py` & `py-Ayra-8.2.6/Ayra/dB/dnd_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/echo_db.py` & `py-Ayra-8.2.6/Ayra/dB/echo_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/filestore_db.py` & `py-Ayra-8.2.6/Ayra/dB/filestore_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/filter_db.py` & `py-Ayra-8.2.6/Ayra/dB/filter_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/forcesub_db.py` & `py-Ayra-8.2.6/Ayra/dB/forcesub_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/gban_mute_db.py` & `py-Ayra-8.2.6/Ayra/dB/gban_mute_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/gcast_blacklist_db.py` & `py-Ayra-8.2.6/Ayra/dB/gcast_blacklist_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/greetings_db.py` & `py-Ayra-8.2.6/Ayra/dB/greetings_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/logusers_db.py` & `py-Ayra-8.2.6/Ayra/dB/logusers_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/mute_db.py` & `py-Ayra-8.2.6/Ayra/dB/mute_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/night_db.py` & `py-Ayra-8.2.6/Ayra/dB/night_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/notes_db.py` & `py-Ayra-8.2.6/Ayra/dB/notes_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/nsfw_db.py` & `py-Ayra-8.2.6/Ayra/dB/nsfw_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/pmpermit_db.py` & `py-Ayra-8.2.6/Ayra/dB/pmpermit_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/snips_db.py` & `py-Ayra-8.2.6/Ayra/dB/snips_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/vc_sudos.py` & `py-Ayra-8.2.6/Ayra/dB/vc_sudos.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/dB/warn_db.py` & `py-Ayra-8.2.6/Ayra/dB/warn_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/fns/FastTelethon.py` & `py-Ayra-8.2.6/Ayra/fns/FastTelethon.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/fns/__init__.py` & `py-Ayra-8.2.6/Ayra/fns/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/fns/admins.py` & `py-Ayra-8.2.6/Ayra/fns/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/fns/executor.py` & `py-Ayra-8.2.6/Ayra/fns/executor.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/fns/gDrive.py` & `py-Ayra-8.2.6/Ayra/fns/gDrive.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/fns/google_image.py` & `py-Ayra-8.2.6/Ayra/fns/google_image.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/fns/helper.py` & `py-Ayra-8.2.6/Ayra/fns/helper.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/fns/info.py` & `py-Ayra-8.2.6/Ayra/fns/info.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/fns/misc.py` & `py-Ayra-8.2.6/Ayra/fns/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/fns/tools.py` & `py-Ayra-8.2.6/Ayra/fns/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,37 +513,32 @@
         html_content=html,
     )
     return page["url"]
 
 
 async def Carbon(
     code,
-    base_url="https://carbonara.vercel.app/api/cook",
+    base_url="https://rayso-api-desvhu-33.koyeb.app/generate",
     file_name="ayra",
     download=False,
     rayso=False,
     **kwargs,
 ):
-    if rayso:
-        base_url = "https://rayso-api-desvhu-33.koyeb.app/generate"
-        kwargs["text"] = code
-        kwargs["theme"] = kwargs.get("theme", "breeze")
-        kwargs["darkMode"] = kwargs.get("darkMode", True)
-        kwargs["title"] = kwargs.get("title", "Ayra")
-    else:
-        kwargs["code"] = code
+    # if rayso:
+    kwargs["text"] = code
+    kwargs["theme"] = kwargs.get("theme", "meadow")
+    kwargs["darkMode"] = kwargs.get("darkMode", True)
+    kwargs["title"] = kwargs.get("title", "Ayra")
+    # else:
+    #    kwargs["code"] = code
     con = await async_searcher(base_url, post=True, json=kwargs, re_content=True)
     if not download:
         file = BytesIO(con)
         file.name = file_name + ".jpg"
     else:
-        try:
-            return json_parser(con.decode())
-        except Exception:
-            pass
         file = file_name + ".jpg"
         with open(file, "wb") as f:
             f.write(con)
     return file
 
 
 async def get_file_link(msg):
```

### Comparing `py-Ayra-8.2.5/Ayra/fns/ytdl.py` & `py-Ayra-8.2.6/Ayra/fns/ytdl.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/kynan.py` & `py-Ayra-8.2.6/Ayra/kynan.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/loader.py` & `py-Ayra-8.2.6/Ayra/loader.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/startup/BaseClient.py` & `py-Ayra-8.2.6/Ayra/startup/BaseClient.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/startup/__init__.py` & `py-Ayra-8.2.6/Ayra/startup/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/startup/_database.py` & `py-Ayra-8.2.6/Ayra/startup/_database.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/startup/_extra.py` & `py-Ayra-8.2.6/Ayra/startup/_extra.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/startup/connections.py` & `py-Ayra-8.2.6/Ayra/startup/connections.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/startup/funcs.py` & `py-Ayra-8.2.6/Ayra/startup/funcs.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/startup/loader.py` & `py-Ayra-8.2.6/Ayra/startup/loader.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/Ayra/startup/utils.py` & `py-Ayra-8.2.6/Ayra/startup/utils.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/LICENSE` & `py-Ayra-8.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/PKG-INFO` & `py-Ayra-8.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayra
-Version: 8.2.5
+Version: 8.2.6
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `py-Ayra-8.2.5/README.md` & `py-Ayra-8.2.6/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/py_Ayra.egg-info/PKG-INFO` & `py-Ayra-8.2.6/py_Ayra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayra
-Version: 8.2.5
+Version: 8.2.6
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `py-Ayra-8.2.5/py_Ayra.egg-info/SOURCES.txt` & `py-Ayra-8.2.6/py_Ayra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.2.5/setup.py` & `py-Ayra-8.2.6/setup.py`

 * *Files identical despite different names*

