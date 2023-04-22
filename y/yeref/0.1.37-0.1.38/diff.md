# Comparing `tmp/yeref-0.1.37.tar.gz` & `tmp/yeref-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.37.tar", last modified: Sat Apr 22 08:00:52 2023, max compression
+gzip compressed data, was "yeref-0.1.38.tar", last modified: Sat Apr 22 08:07:06 2023, max compression
```

## Comparing `yeref-0.1.37.tar` & `yeref-0.1.38.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:00:52.459186 yeref-0.1.37/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-22 08:00:52.459423 yeref-0.1.37/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-22 08:00:52.460275 yeref-0.1.37/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-22 08:00:40.000000 yeref-0.1.37/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:00:52.443329 yeref-0.1.37/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.37/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)    47055 2023-04-22 07:58:34.000000 yeref-0.1.37/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   205172 2023-04-21 19:06:27.000000 yeref-0.1.37/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:00:52.458485 yeref-0.1.37/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-22 08:00:52.000000 yeref-0.1.37/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-22 08:00:52.000000 yeref-0.1.37/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-22 08:00:52.000000 yeref-0.1.37/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-22 08:00:52.000000 yeref-0.1.37/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:07:06.553514 yeref-0.1.38/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-22 08:07:06.553751 yeref-0.1.38/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-22 08:07:06.554719 yeref-0.1.38/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-22 08:06:54.000000 yeref-0.1.38/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:07:06.548661 yeref-0.1.38/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.38/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)    47055 2023-04-22 07:58:34.000000 yeref-0.1.38/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   205153 2023-04-22 08:05:52.000000 yeref-0.1.38/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:07:06.552800 yeref-0.1.38/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-22 08:07:06.000000 yeref-0.1.38/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-22 08:07:06.000000 yeref-0.1.38/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-22 08:07:06.000000 yeref-0.1.38/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-22 08:07:06.000000 yeref-0.1.38/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.37/setup.py` & `yeref-0.1.38/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.37',
+      version='0.1.38',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.37/yeref/l_.py` & `yeref-0.1.38/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.1.37/yeref/yeref.py` & `yeref-0.1.38/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from pyrogram.errors import FloodWait, UserAlreadyParticipant, UsernameInvalid, BadRequest, SlowmodeWait, \
     UserDeactivatedBan, SessionRevoked, SessionExpired, AuthKeyUnregistered, AuthKeyInvalid, AuthKeyDuplicated, \
     InviteHashExpired, InviteHashInvalid, ChatAdminRequired, UserDeactivated, UsernameNotOccupied, ChannelBanned
 from pyrogram.raw import functions
 from stegano import lsb, exifHeader
 from telegraph import Telegraph
 
-from yeref import l_post_media_toobig
+import yeref
 
 one_minute = 60
 one_hour = 3600
 seconds_in_day = 86400
 my_tid = 5491025132
 my_tids = [
     '5900268983',
@@ -1941,15 +1941,15 @@
         await asyncio.sleep(e.retry_after + 1)
     # except FileIsTooBig as e:
     #     logger.info(log_ % str(e))
     #     await asyncio.sleep(round(random.uniform(0, 1), 2))
     #     await bot.send_message(chat_id, l_offer_media_toobig[lz])
     except Exception as e:
         if 'too big' in str(e):
-            await bot.send_message(chat_id, l_post_media_toobig[lz])
+            await bot.send_message(chat_id, yeref.l_post_media_toobig[lz])
         else:
             logger.info(log_ % str(e))
             await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def fsm_button_admin(bot, FsmOffer, message, state, BASE_D):
     try:
```

