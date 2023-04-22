# Comparing `tmp/yeref-0.1.35.tar.gz` & `tmp/yeref-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.35.tar", last modified: Fri Apr 21 18:25:49 2023, max compression
+gzip compressed data, was "yeref-0.1.37.tar", last modified: Sat Apr 22 08:00:52 2023, max compression
```

## Comparing `yeref-0.1.35.tar` & `yeref-0.1.37.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 18:25:49.983016 yeref-0.1.35/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 18:25:49.983313 yeref-0.1.35/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-21 18:25:49.984854 yeref-0.1.35/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1125 2023-04-21 18:25:30.000000 yeref-0.1.35/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 18:25:49.979365 yeref-0.1.35/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.35/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)    40958 2023-04-21 18:21:56.000000 yeref-0.1.35/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   241923 2023-04-21 16:49:48.000000 yeref-0.1.35/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 18:25:49.982370 yeref-0.1.35/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 18:25:49.000000 yeref-0.1.35/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-21 18:25:49.000000 yeref-0.1.35/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-21 18:25:49.000000 yeref-0.1.35/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-21 18:25:49.000000 yeref-0.1.35/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:00:52.459186 yeref-0.1.37/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-22 08:00:52.459423 yeref-0.1.37/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-22 08:00:52.460275 yeref-0.1.37/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-22 08:00:40.000000 yeref-0.1.37/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:00:52.443329 yeref-0.1.37/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.37/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)    47055 2023-04-22 07:58:34.000000 yeref-0.1.37/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   205172 2023-04-21 19:06:27.000000 yeref-0.1.37/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:00:52.458485 yeref-0.1.37/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-22 08:00:52.000000 yeref-0.1.37/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-22 08:00:52.000000 yeref-0.1.37/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-22 08:00:52.000000 yeref-0.1.37/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-22 08:00:52.000000 yeref-0.1.37/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.35/setup.py` & `yeref-0.1.37/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.35',
+      version='0.1.37',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -15,15 +15,15 @@
       #       "oauth2client>=4.1.3",
       #       "google-api-python-client>=2.61.0",
       #       "telegraph>=2.1.0",
       #       "setuptools>=65.3.0",
       # ]
 )
 
-
+# region misc
 # from distutils.core import setup
 # from setuptools import setup, find_packages
 # setup(
 #       name='yeref',
 #       version='0.0.1',
 #       description='desc-f',
 #       author='john smith',
@@ -31,14 +31,18 @@
 #       packages=find_packages(),
 #       scripts=['yeref.py']
 # )
 #
 # python setup.py sdist
 # python setup.py install
 # python setup.py develop
+#
+# python setup.py bdist_wheel
+# endregion
 
 # python -m build
+
 # twine upload dist/*
-# python3 -m pip install --upgrade yeref
 
-# python setup.py bdist_wheel
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.34-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.37-py3-none-any.whl
+
+# python3 -m pip install --upgrade yeref
```

### Comparing `yeref-0.1.35/yeref/l_.py` & `yeref-0.1.37/yeref/l_.py`

 * *Files 10% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     'en': f"<b>🦋 Аuto-funnel & chat-bots in SocialMedia</b> for:\n\n▪️target: @ferey_send_bot\n▪️search: @ferey_find_bot\n▪️post: @ferey_post_bot\n▪️auto-answer: @ferey_user_bot\n▪️channel: @ferey_chat_bot\n▪️channel: @ferey_channel_bot\n▪️advert: @ferey_advert_bot\n\n❗️All bots are public & for common use",
     'es': f"<b>🦋 Embudo automático & bots de chat en redes sociales</b> para:\n\n▪️objetivo: @ferey_send_bot\n▪️búsqueda: @ferey_find_bot\n▪️publicación: @ferey_post_bot\n▪️respuesta automática: @ferey_user_bot\n▪️grupo: @ferey_chat_bot\n▪️canal: @ferey_channel_bot\n▪️anuncio: @ferey_advert_bot\n\n❗️Todos los bots son públicos y de uso común",
     'fr': f"<b>🦋 Аuto-entonnoir & chat-bots dans les médias sociaux</b> pour :\n\n▪️cible : @ferey_send_bot\n▪️recherche : @ferey_find_bot\n▪️post : @ferey_post_bot\n▪️réponse automatique : @ferey_user_bot\n▪️channele : @ferey_chat_bot\n▪️canal : @ferey_channel_bot\n▪️annonce : @ferey_advert_bot\n\n❗️Tous les bots sont publics et à usage commun",
     'zh': f"<b>🦋 社交媒體中的自動漏斗和聊天機器人</b> 為了:\n\n▪️目標: @ferey_send_bot\n▪️搜索: @ferey_find_bot\n▪️優惠: @ferey_post_bot\n▪️自動應答: @ferey_user_bot\n▪️組: @ferey_chat_bot\n▪️頻道: @ferey_channel_bot\n▪️廣告: @ferey_advert_bot\n\n❗️️所有機器人都是公開的 & 普通用途",
     'ar': f"<b>🦋 التحويل التلقائي وروبوتات الدردشة في وسائل التواصل الاجتماعي</b> إلى عن على:\n\n▪️ الهدف: @ferey_send_bot\n▪️ البحث: @ferey_find_bot\n▪️ آخر: @ferey_post_bot\n▪️رد ألي: @ferey_user_bot\n▪️المجموعة: @ferey_chat_bot\n▪️القناة: @ferey_channel_bot\n▪️ادفع: @ferey_advert_bot\n\n❗️جميع الروبوتات عامة & للاستخدام الشائع",
 }
 l_language_get = {
-    'ru': "🌏 Выбери один из доступных языков",
+    'ru': "🌏 <b>Выбери</b> один из доступных языков",
     'en': "🌏 Choose language",
     'es': "🌏 Elige idioma",
     'fr': "🌏 Choisissez la langue",
     'zh': "🌏 選擇語言",
     'ar': "🌏 اختر اللغة",
 }
 l_language_set = {
@@ -278,14 +278,66 @@
     'fr': '👇🏽 Choisissez l\'orientation',
     'zh': '👇🏽 選擇方向',
     'ar': '👇🏽 اختر الاتجاه',
 }
 # endregion
 
 
+# region FereyWorkBot
+l_work_btn1 = {
+    'ru': '⛰️ Вакансии',
+    'en': '⛰️ Projects',
+    'es': '⛰️ Projects',
+    'fr': '⛰️ Projects',
+    'zh': '⛰️ 團體',
+    'ar': '⛰️ مجموعات',
+}
+l_work_btn2 = {
+    'ru': '🌬 Подписка',
+    'en': '🌬 Subcribe',
+    'es': '🌬 Sobre',
+    'fr': '🌬 À propos de',
+    'zh': '🌬 關於',
+    'ar': '🌬 حول',
+}
+l_work_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>проекта</code> <b>Ferey</b>:\n\n▪️<b>информация</b> обо всех проектах\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'en': "🌱 {0}, welcome to <i>landing-bot</i> for <code>administration</code> <b>Telegram</b>-channels:\n\n▪️<b>pretecting</b> channel from spy-joining of\n▪️store offers in <b>unique</b> space\n▪️defend offers form <b>auto</b> deleted* \n(*even it has stop-words)\n\n❗️to order chat-bot-development go to <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'es': "🌱 {0}, Bienvenida(o) a <i>lugar de aterrizaje-bot</i> por <code>creando & publicando</code> <b>Telegram</b>-Grupos:\n\n▪️️crear <b>cualquier</b> tipo de oferta (con botones)\n▪️almacenar ofertas en un espacio <b>único</b>\n▪️️defend ofrece formulario <b>auto</b> borrado* \n(*incluso tiene palabras vacías)\n\n❗️para ordenar chat-bot-desarrollo vaya a <a href='https://t.me/{1}'>Ferey</a>-estudio",
+    'fr': "🌱 {0}, bienvenue sur <i>landing-bot</i> pour la <code>création et publication</code> <b>Télégramme</b>-channeles:\n\n▪️créer <b>tout </b> type d'offre (avec boutons)\n▪️stocker les offres dans un espace <b>unique</b>\n▪️défendre les offres sous forme <b>auto</b> supprimées* \n(*même si elles ont cessé -words)\n\n❗️pour commander le développement de chat-bot, rendez-vous sur <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'zh': "🌱 {0}, 歡迎來到 <i>著陸點-bot</i> 為了 <code>創造 & 張貼</code> <b>Telegram</b>-團體:\n\n▪️️創造 <b>任何</b> 報價類型 (帶按鈕)\n▪️商店優惠在 <b>獨特的</b> 獨特的\n▪️捍衛報價表格自動刪除* \n(*捍衛自動刪除的提議)\n\n❗️訂購 Telegram-bot 去 <a href='https://t.me/{1}'>Ferey</a>-工作室",
+    'ar': "🌱 {0} ، مرحبًا بك في <i> برنامج التتبع </i> من أجل الإنشاء والنش Telegram - مجموعات: \n\n▪️ إنشاء <b> أي </b> نوع العرض (مع الأزرار) \n▪️ عروض المتجر في مساحة فريدة \n▪️ الدفاع عن نموذج عروض <b> تلقائي </b> محذوفة * \n (* حتى إذا توقفت -كلمات) \n\n لطلب تطوير chat-bot-انتقل إلى <a href='https://t.me/{1}'>Ferey</a>-studio"
+}
+l_vacancy_1 = {
+    'ru': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'en': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'es': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'fr': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'zh': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'ar': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
+}
+l_vacancy_2 = {
+    'ru': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
+    'en': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
+    'es': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
+    'fr': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
+    'zh': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
+    'ar': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
+}
+l_vacancy_3 = {
+    'ru': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'en': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'es': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'fr': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'zh':'👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'ar': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
+}
+# endregion
+
+
 # region post
 l_post_text = {
     'ru': "✏️ 1. Напиши мне <b>текст</b> для нового поста (не забудь использовать <i>форматирование</i>)\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 1. Send me <b>text</b> for new post for (don't forget to use <i>formatting</i>)\n\n(<i>or click the «➡️️/Next» to skip this step</i>)",
     'es': "✏️ 1. Envíame <b>texto</b> para una nueva publicación (no olvides usar <i>formato</i>)\n\n(<i>o haz clic en «➡️️ /Next» para omitir este paso</i>)",
     'fr': "✏️ 1. Envoyez-moi un <b>texte</b> pour un nouveau message (n'oubliez pas d'utiliser le <i>formatage</i>)\n\n(<i>ou cliquez sur le «➡️️ /Next» pour ignorer cette étape</i>)",
     'zh': "✏️ 1. 給我 <b>文本</b> 對於新職位 (不要忘記使用 <i>格式化</i>)\n\n(<i>或單擊 «➡️️/Next» 跳過這一步</i>)",
@@ -616,8 +668,8 @@
     'ru': "🕒 Укажи время в будущем",
     'en': "🕒 Specify a time in the future",
     'es': "🕒 Especificar un tiempo en el futuro",
     'fr': "🕒 Spécifiez une heure dans le futur",
     'zh': "🕒 指定未來的時間",
     'ar': "🕒 حدد وقتًا في المستقبل",
 }
-# endregion
+# endregion
```

### Comparing `yeref-0.1.35/yeref/yeref.py` & `yeref-0.1.37/yeref/yeref.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 #!/usr/bin/python3
 # region data
 import ast
 import asyncio
 import datetime
 import io
-from uuid import uuid4
-from math import radians, cos, sin, asin, sqrt
 import logging
 import mimetypes
 import os
 import random
 import re
 import shutil
 import sqlite3
 import string
 from calendar import monthrange
 from contextlib import closing
+from math import radians, cos, sin, asin, sqrt
 from random import randrange
-
+from uuid import uuid4
 import httplib2
 import moviepy.editor as mp
 from PIL import Image
 from aiogram import types
+from aiogram.enums import ParseMode
+from aiogram.exceptions import TelegramRetryAfter
 from aiogram.utils.keyboard import InlineKeyboardBuilder
 from exiftool import ExifToolHelper
 from googleapiclient.discovery import build
 from googleapiclient.http import MediaFileUpload, MediaIoBaseDownload
 from loguru import logger
-from aiogram.enums import ParseMode
 from oauth2client.service_account import ServiceAccountCredentials
+from pydub import AudioSegment
 from pyrogram import enums, Client
 from pyrogram.errors import FloodWait, UserAlreadyParticipant, UsernameInvalid, BadRequest, SlowmodeWait, \
     UserDeactivatedBan, SessionRevoked, SessionExpired, AuthKeyUnregistered, AuthKeyInvalid, AuthKeyDuplicated, \
     InviteHashExpired, InviteHashInvalid, ChatAdminRequired, UserDeactivated, UsernameNotOccupied, ChannelBanned
 from pyrogram.raw import functions
 from stegano import lsb, exifHeader
 from telegraph import Telegraph
 
+from yeref import l_post_media_toobig
+
 one_minute = 60
 one_hour = 3600
 seconds_in_day = 86400
 my_tid = 5491025132
 my_tids = [
     '5900268983',
     '6283902226',
@@ -114,14 +117,16 @@
 All projects: t.me/FereyDemoBot
 🇬🇧🇨🇳🇦🇪🇪🇸🇷🇸🇫🇷
 """
 
 markupAdmin = types.ReplyKeyboardMarkup(keyboard=[
     [types.KeyboardButton(text='⬅️ Prev'), types.KeyboardButton(text='↩️ Menu'),
      types.KeyboardButton(text='➡️️ Next')]], resize_keyboard=True, selective=True, row_width=3)
+
+
 # endregion
 
 
 # region db
 def sqlite_lower(value_):
     return value_.lower() if value_ else None
 
@@ -184,514 +189,14 @@
             retry -= 1
     return 0
 
 
 # endregion
 
 
-# region send
-async def auto_destroy_msg(bot, telegram_bot, chat_id, text, message_id, type_='text', sec=5):
-    result = None
-    try:
-        step = 1
-        by = f"<a href='https://t.me/{ferey_telegram_demo_bot}'>by</a>"
-        text = f"{text}\n\n{by} @{telegram_bot} <b>{sec}</b>sec"
-        ix_sec = text.rfind('</b>sec')
-        while text[ix_sec] != '>': ix_sec -= 1
-
-        while sec > 0:
-            try:
-                text = text.replace(f"<b>{sec}</b>sec", f"<b>{sec - 1}</b>sec")
-                sec -= step
-                if type_ == 'text':
-                    await bot.edit_message_text(text, chat_id, message_id, disable_web_page_preview=True)
-                else:
-                    await bot.edit_message_caption(chat_id=chat_id, message_id=message_id, caption=text)
-                await asyncio.sleep(1)
-            except Exception as e:
-                logger.info(log_ % str(e))
-                await asyncio.sleep(round(random.uniform(1, 2), 2))
-                break
-        await bot.delete_message(chat_id, message_id)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(e)
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
-async def send_my_text(bot, chat_id, text, reply_markup=None, disable_web_page_preview=True, typetime=None):
-    result = None
-    try:
-        # печатает
-        await bot.send_chat_action(chat_id=chat_id, action='typing')
-
-        text = await no_war_text(text)
-        text = text[0:4095]
-
-        if typetime:
-            copy_text = text
-            copy_text = re.sub(re.compile('<.*?>'), '', copy_text)
-            copy_text_clean = copy_text
-            tbp = ""
-            typing_symbol = "▒"
-            result = await bot.send_message(chat_id=chat_id, text=copy_text, reply_markup=reply_markup)
-            couple = int(len(copy_text) / 99) + 3
-
-            for i in range(0, 99):
-                try:
-                    result = await bot.edit_message_text(text=tbp + typing_symbol, chat_id=chat_id,
-                                                         message_id=result.message_id, reply_markup=reply_markup)
-                    await asyncio.sleep(0.07)
-
-                    tbp = tbp + copy_text[0:couple]
-                    copy_text = copy_text[couple:]
-
-                    result = await bot.edit_message_text(text=tbp, chat_id=chat_id, message_id=result.message_id,
-                                                         reply_markup=reply_markup)
-                    await asyncio.sleep(0.07)
-
-                    if copy_text_clean == tbp:
-                        break
-                except RetryAfter as e:
-                    logger.info(log_ % f"RetryAfter {e.retry_after}")
-                    await asyncio.sleep(e.retry_after + 1)
-                except Exception as e:
-                    logger.info(log_ % str(e))
-                    await asyncio.sleep(round(random.uniform(1, 2), 2))
-            # await asyncio.sleep(2)
-            await bot.edit_message_text(text=text, chat_id=chat_id, message_id=result.message_id,
-                                        reply_markup=reply_markup,
-                                        disable_web_page_preview=disable_web_page_preview)
-        else:
-            result = await bot.send_message(chat_id=chat_id, text=text, reply_markup=reply_markup,
-                                            disable_web_page_preview=disable_web_page_preview,
-                                            disable_notification=True)
-            text = text[0:32].replace('\n', '')
-            logger.info(
-                log_ % f"@{(await bot.get_chat(chat_id)).username} (<code>{chat_id}</code>): {text}")
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
-async def send_my_photo(bot, chat_id, photo_name, caption, CONF_P, EXTRA_D, MEDIA_D, BASE_D, reply_markup=None,
-                        re_write=True):
-    result = None
-    try:
-        # печатает
-        await bot.send_chat_action(chat_id=chat_id, action='upload_photo')  # UPLOAD_PHOTO
-
-        caption = await no_war_text(caption)
-        caption = caption[0:1023]
-        fl_photo = await get_from_media(CONF_P, EXTRA_D, MEDIA_D, BASE_D, photo_name, re_write)
-        photo = types.InputFile(fl_photo) if fl_photo and '/' in fl_photo and '://' not in fl_photo else fl_photo
-        result = await bot.send_photo(chat_id=chat_id, photo=photo, caption=caption, reply_markup=reply_markup,
-                                      disable_notification=True)
-        await save_fileid(result, photo_name, BASE_D)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
-async def send_my_video(bot, chat_id, video_name, caption, CONF_P, EXTRA_D, MEDIA_D, BASE_D, thumb_name=None,
-                        reply_markup=None, re_write=True):
-    result = None
-    try:
-        # записывает видео
-        await bot.send_chat_action(chat_id=chat_id, action='record_video')  # RECORD_VIDEO doesn't work
-
-        caption = await no_war_text(caption)
-        caption = caption[0:1023]
-
-        fl_video = await get_from_media(CONF_P, EXTRA_D, MEDIA_D, BASE_D, video_name, re_write)
-        video = types.InputFile(fl_video) if fl_video and '/' in fl_video else fl_video
-        fl_thumb = await get_from_media(CONF_P, EXTRA_D, MEDIA_D, BASE_D, thumb_name, re_write, 160)
-        thumb = types.InputFile(fl_thumb) if fl_thumb and '/' in fl_thumb else fl_thumb
-        result = await bot.send_video(chat_id=chat_id, video=video, thumb=thumb, caption=caption,
-                                      reply_markup=reply_markup, disable_notification=True)
-        await save_fileid(result, video_name, BASE_D)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
-async def send_my_video_note(bot, chat_id, videonote_name, CONF_P, EXTRA_D, MEDIA_D, BASE_D, thumb_name=None,
-                             reply_markup=None, re_write=True):
-    result = None
-    try:
-        # записывает видео # UPLOAD_VIDEO_NOTE - это печатает
-        await bot.send_chat_action(chat_id=chat_id, action='record_video')
-
-        fl_videonote = await get_from_media(CONF_P, EXTRA_D, MEDIA_D, BASE_D, videonote_name, re_write, 440)
-        videonote = types.InputFile(fl_videonote) if fl_videonote and '/' in fl_videonote else fl_videonote
-        fl_thumb = await get_from_media(CONF_P, EXTRA_D, MEDIA_D, BASE_D, thumb_name, re_write, 160)
-        thumb = types.InputFile(fl_thumb) if fl_thumb and '/' in fl_thumb else fl_thumb
-        result = await bot.send_video_note(chat_id=chat_id, video_note=videonote, thumb=thumb,
-                                           reply_markup=reply_markup, disable_notification=True)
-        await save_fileid(result, videonote_name, BASE_D)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
-async def send_my_media_group(bot, chat_id, media_names, CONF_P, EXTRA_D, MEDIA_D, BASE_D, re_write=True):
-    result = None
-    try:
-        # печатает
-        await bot.send_chat_action(chat_id=chat_id, action=ChatActions.UPLOAD_VIDEO)
-        await bot.send_chat_action(chat_id=chat_id, action=ChatActions.UPLOAD_PHOTO)
-
-        media = types.MediaGroup()
-        for media_name in media_names:
-            fl_media = await get_from_media(CONF_P, EXTRA_D, MEDIA_D, BASE_D, media_name, re_write)
-            tmp_media = types.InputFile(fl_media) if fl_media and '/' in fl_media else fl_media
-            media.attach_photo(tmp_media)
-
-        result = await bot.send_media_group(chat_id=chat_id, media=media, disable_notification=True)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
-async def send_my_doc(bot, chat_id, doc_name, CONF_P, BASE_D, MEDIA_D, EXTRA_D, caption, thumb_name=None,
-                      reply_markup=None, re_write=True):
-    # загружает документ
-    # thumb - JPEG format,  less than 200 kB in size. A thumbnail‘s width and height should not exceed 320
-    result = None
-    try:
-        await bot.send_chat_action(chat_id=chat_id, action='upload_document')
-
-        caption = await no_war_text(caption)
-        caption = caption[0:1023]
-
-        fl_doc = await get_from_media(CONF_P, EXTRA_D, MEDIA_D, BASE_D, doc_name, re_write)
-        # fl_doc = os.path.abspath(os.path.join(os.path.dirname(__file__),'config.ini'))
-        document = types.InputFile(fl_doc) if fl_doc and '/' in fl_doc else fl_doc
-        fl_thumb = await get_from_media(CONF_P, EXTRA_D, MEDIA_D, BASE_D, thumb_name, re_write, 160)
-        thumb = types.InputFile(fl_thumb) if fl_thumb and '/' in fl_thumb else fl_thumb
-        result = await bot.send_document(chat_id=chat_id, document=document, thumb=thumb, caption=caption,
-                                         disable_content_type_detection=True,
-                                         reply_markup=reply_markup, disable_notification=True)
-        await save_fileid(result, doc_name, BASE_D)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
-async def send_my_audio(bot, chat_id, audio_name, caption, CONF_P, EXTRA_D, MEDIA_D, BASE_D, thumb_name=None,
-                        reply_markup=None, re_write=True):
-    result = None
-    try:
-        # записывает голосовое сообщение    # = RECORD_AUDIO = UPLOAD_VOICE = RECORD_VOICE
-        await bot.send_chat_action(chat_id=chat_id, action='record_voice')
-
-        caption = await no_war_text(caption)
-        caption = caption[0:1023]
-
-        fl_audio = await get_from_media(CONF_P, EXTRA_D, MEDIA_D, BASE_D, audio_name, re_write)
-        audio = types.InputFile(fl_audio) if fl_audio and '/' in fl_audio else fl_audio
-        fl_thumb = await get_from_media(CONF_P, EXTRA_D, MEDIA_D, BASE_D, thumb_name, re_write, 160)
-        thumb = types.InputFile(fl_thumb) if fl_thumb and '/' in fl_thumb else fl_thumb
-        # thumb = types.InputFile(os.path.join(DEFAULT_EXTRA, 'img.png'))
-        # title='Canto Ostinato Pt1 Section14.mp3', performer='Simeon ten Holt',
-        result = await bot.send_audio(chat_id=chat_id, audio=audio, thumb=thumb, caption=caption, title='Listen',
-                                      reply_markup=reply_markup, disable_notification=True)
-        await save_fileid(result, audio_name, BASE_D)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
-async def send_my_voice(bot, chat_id, voice_name, caption, CONF_P, EXTRA_D, MEDIA_D, BASE_D, reply_markup=None,
-                        re_write=True):
-    result = None
-    try:
-        # записывает аудио  # = RECORD_AUDIO = UPLOAD_VOICE = RECORD_VOICE
-        await bot.send_chat_action(chat_id=chat_id, action='record_voice')
-
-        caption = await no_war_text(caption)
-        caption = caption[0:1023]
-
-        fl_voice = await get_from_media(CONF_P, EXTRA_D, MEDIA_D, BASE_D, voice_name, re_write)
-        voice = types.InputFile(fl_voice) if fl_voice and '/' in fl_voice else fl_voice
-        result = await bot.send_voice(chat_id=chat_id, voice=voice, caption=caption, reply_markup=reply_markup,
-                                      disable_notification=True)
-        await save_fileid(result, voice_name, BASE_D)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
-async def send_my_animation(bot, chat_id, animation_name, caption, CONF_P, EXTRA_D, MEDIA_D, BASE_D, thumb_name=None,
-                            reply_markup=None, re_write=True):
-    result = None
-    try:
-        # печатает
-        await bot.send_chat_action(chat_id=chat_id, action='upload_video')  # UPLOAD_PHOTO
-
-        caption = await no_war_text(caption)
-        caption = caption[0:1023]
-
-        fl_animation = await get_from_media(CONF_P, EXTRA_D, MEDIA_D, BASE_D, animation_name, re_write)
-        animation = types.InputFile(fl_animation) if fl_animation and '/' in fl_animation else fl_animation
-        fl_thumb = await get_from_media(CONF_P, EXTRA_D, MEDIA_D, BASE_D, thumb_name, re_write, 160)
-        thumb = types.InputFile(fl_thumb) if fl_thumb and '/' in fl_thumb else fl_thumb
-        result = await bot.send_animation(chat_id=chat_id, animation=animation, thumb=thumb, caption=caption,
-                                          reply_markup=reply_markup, disable_notification=True)
-        await save_fileid(result, animation_name, BASE_D)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
-async def send_my_sticker(bot, chat_id, sticker, reply_markup=None):
-    result = None
-    try:
-        # ищет стикер
-        await bot.send_chat_action(chat_id=chat_id, action='choose_sticker')
-
-        result = await bot.send_sticker(chat_id=chat_id, sticker=sticker, reply_markup=reply_markup,
-                                        disable_notification=True)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
-##############################
-
-
-async def send_message_my(bot, chat_id, text, reply_markup=None, action_=False, disable_preview=True,
-                          disable_notific=None, is_protect=None, typing=None):
-    result = None
-    try:
-        if action_ == '☑':
-            await bot.send_chat_action(chat_id=chat_id, action=ChatActions.TYPING)
-
-        text = text[0:4095]
-
-        if typing:
-            copy_text = text
-            copy_text = re.sub(re.compile('<.*?>'), '', copy_text)
-            copy_text_clean = copy_text
-            tbp = ""
-            typing_symbol = "▒"
-            result = await bot.send_message(chat_id=chat_id, text=copy_text, reply_markup=reply_markup)
-            couple = int(len(copy_text) / 99) + 3
-
-            for i in range(0, 99):
-                try:
-                    result = await bot.edit_message_text(text=tbp + typing_symbol, chat_id=chat_id,
-                                                         message_id=result.message_id, reply_markup=reply_markup)
-                    await asyncio.sleep(0.07)
-
-                    tbp = tbp + copy_text[0:couple]
-                    copy_text = copy_text[couple:]
-
-                    result = await bot.edit_message_text(text=tbp, chat_id=chat_id, message_id=result.message_id,
-                                                         reply_markup=reply_markup)
-                    await asyncio.sleep(0.07)
-
-                    if copy_text_clean == tbp:
-                        break
-                except RetryAfter as e:
-                    logger.info(log_ % f"RetryAfter {e.retry_after}")
-                    await asyncio.sleep(e.retry_after + 1)
-                except Exception as e:
-                    logger.info(log_ % str(e))
-                    await asyncio.sleep(round(random.uniform(1, 2), 2))
-
-            await bot.edit_message_text(text=text, chat_id=chat_id, message_id=result.message_id,
-                                        reply_markup=reply_markup,
-                                        disable_web_page_preview=disable_web_page_preview)
-        else:
-            result = await bot.send_message(chat_id=chat_id, text=text, reply_markup=reply_markup,
-                                            disable_web_page_preview=disable_web_page_preview,
-                                            disable_notification=disable_notific, protect_content=is_protect)
-
-        text = re.sub(re.compile('<.*?>'), '', text[0:32].replace('\n', ''))
-        logger.info(log_ % f"@{(await bot.get_chat(chat_id)).username} [{chat_id}]: {text}")
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
-async def send_photo_my(bot, chat_id, photo, caption, MEDIA_D, reply_markup=None, action_=False, disable_notific=None,
-                        is_protect=None):
-    result = None
-    try:
-        if action_ == '☑':  # UPLOAD_PHOTO
-            await bot.send_chat_action(chat_id=chat_id, action=ChatActions.TYPING)
-        photo_name = photo
-        caption = caption[0:1023]
-
-        BASE_BOT = os.path.join(MEDIA_D, str(BOT_TID), f"{BOT_TID}.db")
-        sql = "SELECT FILE_TID, FILE_HASH FROM FILE WHERE FILE_NAME=?"
-        data_file = await db_select(sql, (photo,), BASE_BOT)
-        if len(data_file):
-            FILE_TID, FILE_HASH = data_file[0]
-        else:
-            FILE_TID, FILE_HASH = None, None
-
-        photo = FILE_TID if FILE_TID else photo
-        photo = types.InputFile(photo) if '/' in photo and '://' not in photo else photo
-        result = await bot.send_photo(chat_id=chat_id, photo=photo, caption=caption, reply_markup=reply_markup,
-                                      disable_notification=disable_notific, protect_content=is_protect)
-
-        await save_fileid_my(result, photo_name, BASE_BOT)
-        text = re.sub(re.compile('<.*?>'), '', caption[0:32].replace('\n', ''))
-        logger.info(log_ % f"@{(await bot.get_chat(chat_id)).username} [{chat_id}]: {text}")
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
-async def save_fileid_my(message, src, BASE_BOT):
-    try:
-        if message.photo:
-            file_id = message.photo[-1].file_id
-        elif message.audio:  # m4a
-            file_id = message.audio.file_id
-        elif message.document:
-            file_id = message.document.file_id
-        elif message.video:
-            file_id = message.video.file_id
-        elif message.animation:  # giff
-            file_id = message.animation.file_id
-        elif message.voice:
-            file_id = message.voice.file_id
-        elif message.video_note:
-            file_id = message.video_note.file_id
-        elif message.sticker:
-            file_id = message.sticker.file_id
-
-        sql = "INSERT OR IGNORE INTO FILE (FILE_TID, FILE_NAME) VALUES (?, ?)"
-        await db_change(sql, (file_id, src,), BASE_BOT)
-        sql = "UPDATE FILE SET FILE_TID=? WHERE FILE_NAME=?"
-        await db_change(sql, (file_id, src,), BASE_BOT)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
-async def send_voice_my(bot, chat_id, voice, caption, MEDIA_D, EXTRA_D, restricted_, reply_markup=None, action_=False,
-                        disable_notific=None, is_protect=None):
-    result = None
-    try:
-        get_chat_ = await bot.get_chat(chat_id)
-        if get_chat_.has_restricted_voice_and_video_messages and restricted_ == '☐': return
-        if action_ == '☑':  # записывает аудио  # = RECORD_AUDIO = UPLOAD_VOICE = RECORD_VOICE
-            await bot.send_chat_action(chat_id=chat_id, action=ChatActions.UPLOAD_AUDIO)
-        caption = caption[0:1023]
-        voice_name = voice
-
-        BASE_BOT = os.path.join(MEDIA_D, str(BOT_TID), f"{BOT_TID}.db")
-        FILE_FIELD = "FILE_TID2" if restricted_ and has_restricted else "FILE_TID"
-        sql = f"SELECT {FILE_FIELD}, FILE_HASH FROM FILE WHERE FILE_NAME=?"
-        data_file = await db_select(sql, (voice,), BASE_BOT)
-        if len(data_file):
-            FILE_TID, FILE_HASH = data_file[0]
-        else:
-            FILE_TID, FILE_HASH = None, None
-
-        voice = FILE_TID if FILE_TID else voice
-        voice = types.InputFile(voice) if '/' in voice and '://' not in voice else voice
-        if restricted_:
-            performer = get_chat_.first_name
-            username = f"@{get_chat_.username}" if get_chat_.username else None
-            title = get_chat_.bio or username or 'audio voice'
-            thumb = types.InputFile(os.path.join(EXTRA_D, 'img.jpg'))
-            result = await bot.send_audio(chat_id=chat_id, voice=voice, caption=caption, reply_markup=reply_markup,
-                                          performer=performer, title=title, thumb=thumb,
-                                          disable_notification=disable_notific, protect_content=is_protect)
-        else:
-            result = await bot.send_voice(chat_id=chat_id, voice=voice, caption=caption, reply_markup=reply_markup,
-                                          disable_notification=disable_notific, protect_content=is_protect)
-
-        await save_fileid_my(result, voice_name, BASE_BOT)
-        text = re.sub(re.compile('<.*?>'), '', caption[0:32].replace('\n', ''))
-        logger.info(log_ % f"@{get_chat_.username} [{chat_id}]: {text}")
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
-# endregion
-
-
 # region menu
 async def is_ban_menu(chat_id):
     result = False
     try:
         telegraph_ = Telegraph(access_token=TGPH_TOKEN_BAN)
         pages = telegraph_.get_page_list()
 
@@ -703,16 +208,16 @@
 
                     if str(chat_id) in ban_ids:
                         return True
                     break
             except Exception as e:
                 logger.info(log_ % str(e))
                 await asyncio.sleep(round(random.uniform(0, 1), 2))
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         return result
 
@@ -741,16 +246,16 @@
                         await bot.send_message(chat_id, f"👩🏽‍💻 {modul}th added to /ban (len: {length2})")
                     else:
                         await bot.send_message(chat_id, f"👩🏽‍💻 {modul}th already in /ban (len: {length2})")
                     break
             except Exception as e:
                 logger.info(log_ % str(e))
                 await asyncio.sleep(round(random.uniform(0, 1), 2))
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def unban_handler_menu(bot, chat_id, prepare_ids):
@@ -777,16 +282,16 @@
                         await bot.send_message(chat_id, f"👩🏽‍💻 {modul}th removed from /ban (len: {length2})")
                     else:
                         await bot.send_message(chat_id, f"👩🏽‍💻 {modul}th already deleted from /ban (len: {length2})")
                     break
             except Exception as e:
                 logger.info(log_ % str(e))
                 await asyncio.sleep(round(random.uniform(0, 1), 2))
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def bots_by_inline(chat_id, message, BASE_D):
@@ -794,15 +299,15 @@
     try:
         lz = await lz_code(chat_id, message.from_user.language_code, BASE_D)
 
         data = [
             ['👩🏽‍💻 @FereyDemoBot', l_inline_demo[lz], 'https://t.me/FereyDemoBot'],
             ['👩🏽‍💻 @FereyBotBot', l_inline_bot[lz], 'https://t.me/FereyBotBot'],
             ['👩🏽‍💻 @FereyPostBot', l_inline_post[lz], 'https://t.me/FereyPostBot'],
-            ['👩🏽‍💻 @FereyMediaBot', l_inline_media[lz],  'https://t.me/FereyMediaBot'],
+            ['👩🏽‍💻 @FereyMediaBot', l_inline_media[lz], 'https://t.me/FereyMediaBot'],
             ['👩🏽‍💻 @FereyChannelBot', l_inline_channel[lz], 'https://t.me/FereyChannelBot'],
             ['👩🏽‍💻 @FereyGroupBot', l_inline_group[lz], 'https://t.me/FereyGroupBot'],
             ['👩🏽‍💻 @FereyFindBot', l_inline_find[lz], 'https://t.me/FereyFindBot'],
             ['👩🏽‍💻 @FereyAIBot', l_inline_ai[lz], 'https://t.me/FereyAIBot'],
             ['👩🏽‍💻 @FereyAdsBot', l_inline_ads[lz], 'https://t.me/FereyAdsBot'],
             ['👩🏽‍💻 @FereyVPNBot', l_inline_vpn[lz], 'https://t.me/FereyVPNBot'],
             ['👩🏽‍💻 @FereyTargetBot', l_inline_target[lz], 'https://t.me/FereyTargetBot'],
@@ -829,24 +334,27 @@
 
 async def get_buttons_main(lz, bot_username, BASE_D):
     result = []
     try:
         result = [
             types.InlineKeyboardButton(text="👩🏽‍💼Acc", url=f"tg://user?id={my_tid}"),
             types.InlineKeyboardButton(text="🙌🏽Tgph", web_app=types.WebAppInfo(url='https://telegra.ph')),
-            types.InlineKeyboardButton(text="🔗Share", url=f'https://t.me/share/url?url=https%3A%2F%2Ft.me%2F{bot_username}&text=%40{bot_username}'),
+            types.InlineKeyboardButton(text="🔗Share",
+                                       url=f'https://t.me/share/url?url=https%3A%2F%2Ft.me%2F{bot_username}&text=%40{bot_username}'),
             types.InlineKeyboardButton(text=f"{(await read_likes(BASE_D))}♥️Like", callback_data=f"like"),
             types.InlineKeyboardButton(text="🦋Chan", url=f"https://t.me/{get_tg_channel(lz)}"),
             types.InlineKeyboardButton(text="🫥Bots", switch_inline_query_current_chat=f"~"),
         ]
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         return result
+
+
 # endregion
 
 
 # region l_
 l_offer_text = {
     'ru': "✏️ 1/4. Напиши мне <b>текст</b> для нового оффера (не забудь использовать <i>форматирование</i>)\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 1/4. Send me <b>text</b> for new post for (don't forget to use <i>formatting</i>)\n\n(<i>or click the «➡️️/Next» to skip this step</i>)",
@@ -1440,14 +948,16 @@
     'ru': "вакансии/конкурсы",
     'en': "forever",
     'es': "siempre",
     'fr': "toujours",
     'zh': "永遠",
     'ar': "إلى الأبد",
 }
+
+
 # endregion
 
 
 # region admin
 async def pre_upload(bot, chat_id, media_name, media_type, EXTRA_D, BASE_D):
     result = None
     try:
@@ -1510,15 +1020,16 @@
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         return result
 
 
-async def show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, post_id=1, call=None):
+async def show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, bot_username, post_id=1,
+                            call=None):
     try:
         sql = "SELECT OFFER_ID, OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, " \
               "OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, OFFER_DT FROM OFFER"
         data_offers = await db_select(sql, (), BASE_D)
         if not data_offers:
             if call: await call.message.delete()
             await bot.send_message(chat_id, l_offer_text[lz], reply_markup=markupAdmin)
@@ -1622,29 +1133,32 @@
                                            disable_web_page_preview=True)
             else:
                 if OFFER_MEDIATYPE == 'photo' or OFFER_MEDIATYPE == 'text':
                     if call.message.video_note or call.message.voice or call.message.sticker or call.message.text:
                         await bot.send_photo(chat_id, OFFER_FILEID, caption=OFFER_TEXT,
                                              reply_markup=reply_markup.as_markup(), has_spoiler=OFFER_ISSPOILER)
                     else:
-                        media = types.InputMediaPhoto(media=OFFER_FILEID, caption=OFFER_TEXT, has_spoiler=OFFER_ISSPOILER)
+                        media = types.InputMediaPhoto(media=OFFER_FILEID, caption=OFFER_TEXT,
+                                                      has_spoiler=OFFER_ISSPOILER)
                         await call.message.edit_media(media=media, reply_markup=reply_markup.as_markup())
                 elif OFFER_MEDIATYPE == 'animation':
                     if call.message.video_note or call.message.voice or call.message.sticker or call.message.text:
                         await bot.send_animation(chat_id, OFFER_FILEID, caption=OFFER_TEXT,
                                                  reply_markup=reply_markup.as_markup(), has_spoiler=OFFER_ISSPOILER)
                     else:
-                        media = types.InputMediaAnimation(media=OFFER_FILEID, caption=OFFER_TEXT, has_spoiler=OFFER_ISSPOILER)
+                        media = types.InputMediaAnimation(media=OFFER_FILEID, caption=OFFER_TEXT,
+                                                          has_spoiler=OFFER_ISSPOILER)
                         await call.message.edit_media(media=media, reply_markup=reply_markup.as_markup())
                 elif OFFER_MEDIATYPE == 'video':
                     if call.message.video_note or call.message.voice or call.message.sticker or call.message.text:
                         await bot.send_video(chat_id, OFFER_FILEID, caption=OFFER_TEXT,
                                              reply_markup=reply_markup.as_markup(), has_spoiler=OFFER_ISSPOILER)
                     else:
-                        media = types.InputMediaVideo(media=OFFER_FILEID, caption=OFFER_TEXT, has_spoiler=OFFER_ISSPOILER)
+                        media = types.InputMediaVideo(media=OFFER_FILEID, caption=OFFER_TEXT,
+                                                      has_spoiler=OFFER_ISSPOILER)
                         await call.message.edit_media(media=media, reply_markup=reply_markup.as_markup())
                 elif OFFER_MEDIATYPE == 'audio':
                     if call.message.video_note or call.message.voice or call.message.sticker or call.message.text:
                         await bot.send_audio(chat_id, OFFER_FILEID, caption=OFFER_TEXT,
                                              reply_markup=reply_markup.as_markup())
                     else:
                         media = types.InputMediaAudio(media=OFFER_FILEID, caption=OFFER_TEXT)
@@ -1688,28 +1202,30 @@
                     OFFER_MEDIATYPE) if OFFER_MEDIATYPE and '[' in OFFER_MEDIATYPE else OFFER_MEDIATYPE
 
                 media = []
                 for i in range(0, len(OFFER_FILEID)):
                     caption = OFFER_TEXT if i == 0 else None
 
                     if OFFER_MEDIATYPE[i] == 'photo':
-                        media.append(types.InputMediaPhoto(media=OFFER_FILEID[i], caption=caption, has_spoiler=OFFER_ISSPOILER))
+                        media.append(
+                            types.InputMediaPhoto(media=OFFER_FILEID[i], caption=caption, has_spoiler=OFFER_ISSPOILER))
                     elif OFFER_MEDIATYPE[i] == 'video':
-                        media.append(types.InputMediaVideo(media=OFFER_FILEID[i], caption=caption, has_spoiler=OFFER_ISSPOILER))
+                        media.append(
+                            types.InputMediaVideo(media=OFFER_FILEID[i], caption=caption, has_spoiler=OFFER_ISSPOILER))
                     elif OFFER_MEDIATYPE[i] == 'audio':
                         media.append(types.InputMediaAudio(media=OFFER_FILEID[i], caption=caption))
                     elif OFFER_MEDIATYPE[i] == 'document':
                         media.append(types.InputMediaDocument(media=OFFER_FILEID[i], caption=caption,
                                                               disable_content_type_detection=True))
 
                 await bot.send_media_group(chat_id, media)
                 await bot.send_message(chat_id=chat_id, text=extra, reply_markup=reply_markup.as_markup())
         # endregion
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def get_current_page_number(call):
@@ -1725,15 +1241,15 @@
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         return result
 
 
-async def broadcast_send_admin(bot, chat_id, lz, offer_id, BASE_D, ids='all'):
+async def broadcast_send_admin(bot, chat_id, lz, offer_id, BASE_D, ids):
     try:
         if ids == 'me':
             user_ids = [chat_id]
         elif ids == 'all':
             sql = "SELECT USER_TID FROM USER"
             data = await db_select(sql, (), BASE_D)
             user_ids = [item[0] for item in data]
@@ -1785,32 +1301,33 @@
               "OFFER_TGPHLINK, OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, " \
               "OFFER_DT FROM OFFER WHERE OFFER_ID=?"
         data = await db_select(sql, (offer_id,), BASE_D)
         if not len(data): return
         OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_FILEIDNOTE, OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, \
             OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, OFFER_DT = data[0]
 
-        reply_markup = await create_replymarkup2(bot, offer_id, OFFER_BUTTON) if OFFER_ISBUTTON else InlineKeyboardBuilder()
+        reply_markup = await create_replymarkup2(bot, offer_id,
+                                                 OFFER_BUTTON) if OFFER_ISBUTTON else InlineKeyboardBuilder()
 
         if '[' in OFFER_MEDIATYPE:
             OFFER_FILEID = ast.literal_eval(OFFER_FILEID)
             OFFER_MEDIATYPE = ast.literal_eval(OFFER_MEDIATYPE)
             OFFER_TGPHLINK = ast.literal_eval(OFFER_TGPHLINK)
 
-            len_ = len(OFFER_FILEID)
             OFFER_FILEID = OFFER_FILEID[current - 1] if message_id else OFFER_FILEID[0]
             OFFER_MEDIATYPE = OFFER_MEDIATYPE[current - 1] if message_id else OFFER_MEDIATYPE[0]
             OFFER_TGPHLINK = OFFER_TGPHLINK[current - 1] if message_id else OFFER_TGPHLINK[0]
 
         if OFFER_ISTGPH and OFFER_TGPHLINK and '[' not in OFFER_TGPHLINK:
             OFFER_MEDIATYPE = 'text'
-            OFFER_TEXT = OFFER_TEXT if OFFER_TEXT and OFFER_TEXT!= '' else "."
+            OFFER_TEXT = OFFER_TEXT if OFFER_TEXT and OFFER_TEXT != '' else "."
             OFFER_TEXT = f"<a href='{OFFER_TGPHLINK}'>​</a>{OFFER_TEXT}"
 
             if OFFER_ISGALLERY:
+                len_ = len(OFFER_FILEID)
                 buttons = [
                     types.InlineKeyboardButton(text="←", callback_data=f'gallery_prev_{offer_id}'),
                     types.InlineKeyboardButton(text=f"{current}/{len_}", callback_data=f'gallery_current_{offer_id}'),
                     types.InlineKeyboardButton(text="→", callback_data=f'gallery_next_{offer_id}'),
                 ]
                 reply_markup.row(*buttons)
 
@@ -1906,16 +1423,16 @@
             result = await bot.send_sticker(chat_id=chat_id,
                                             sticker=OFFER_FILEID,
                                             disable_notification=OFFER_ISSILENCE,
                                             reply_markup=reply_markup.as_markup())
 
         if result and OFFER_ISPIN and not message_id:
             await bot.pin_chat_message(chat_id=chat_id, message_id=result.message_id, disable_notification=False)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         return result
 
@@ -1982,16 +1499,16 @@
                 tmp = []
 
         if is_new:
             await bot.send_message(chat_id=chat_id, text=l_offer_date[lz], reply_markup=reply_markup.as_markup())
         else:
             await bot.edit_message_text(chat_id=chat_id, text=l_offer_date[lz], message_id=message_id,
                                         reply_markup=reply_markup.as_markup())
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def callbacks_ofr_admin(bot, FsmOffer, call, state, BASE_D):
@@ -2099,16 +1616,16 @@
                 types.InlineKeyboardButton(text=l_all[lz], callback_data=f"pub_all_{offer_id}"),
                 types.InlineKeyboardButton(text=l_ids[lz], callback_data=f"pub_ids_{offer_id}"),
             ]
             reply_markup.add(*buttons).adjust(1)
 
             text = l_recipient[lz]
             await bot.send_message(chat_id, text, reply_markup=reply_markup.as_markup())
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def callbacks_pub_admin(bot, FsmIds, call, state, BASE_D):
@@ -2125,36 +1642,36 @@
             loop.create_task(broadcast_send_admin(bot, chat_id, lz, offer_id, BASE_D, 'all'))
         elif option == 'ids':
             await state.set_state(FsmIds.start)
             await state.update_data(offer_id=offer_id)
 
             text = l_enter[lz]
             await bot.send_message(chat_id, text)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def fsm_ids_start_admin(bot, FsmIds, message, state, BASE_D):
     try:
         chat_id = message.from_user.id
         lz = await lz_code(chat_id, message.from_user.language_code, BASE_D)
-        arr = re.split(r'[`\-=~!@#$%^&*()_+\[\]{};\'\\:"|<,./<>?]', message.text)
+        arr = re.split(r'[`\-=~!@#$%^&*()_+\[\]{};\'\\:"|<,./?]', message.text)
         ids = [it for it in arr if it != '']
         data = await state.get_data()
         offer_id = data.get('offer_id')
 
         loop = asyncio.get_event_loop()
         loop.create_task(broadcast_send_admin(bot, chat_id, lz, offer_id, BASE_D, ids))
         await state.clear()
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def fsm_text_admin(bot, FsmOffer, message, state, BASE_D):
@@ -2173,16 +1690,16 @@
                 text = l_offer_text_limit[lz].format(len(message.html_text))
                 await bot.send_message(chat_id, text)
                 return
 
             await state.update_data(offer_text=message.html_text)
             await bot.send_message(chat_id=chat_id, text=l_offer_media[lz])
             await state.set_state(FsmOffer.media)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def fsm_album_admin(bot, FsmOffer, message, album, state, MEDIA_D, BASE_D):
@@ -2259,23 +1776,23 @@
             if len(ast.literal_eval(str(offer_file_id))) < 2:
                 await bot.send_message(chat_id=chat_id, text=l_offer_media[lz])
                 await state.set_state(FsmOffer.media)
                 return
 
             await generate_calendar_admin(bot, state, lz, chat_id)
             await state.set_state(FsmOffer.date_)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
-async def fsm_media_admin(bot, FsmOffer, message, state, MEDIA_D, BASE_D):
+async def fsm_media_admin(bot, FsmOffer, message, state, MEDIA_D, BASE_D, EXTRA_D):
     chat_id = message.from_user.id
     lz = await lz_code(chat_id, message.from_user.language_code, BASE_D)
 
     try:
         data = await state.get_data()
         offer_text = data.get('offer_text', None)
 
@@ -2415,24 +1932,24 @@
             await state.update_data(offer_file_id=file_id, offer_file_id_note=file_id_note, offer_file_type=file_type,
                                     offer_tgph_link=offer_tgph_link, file_name_part=file_name_part)
 
             text = l_offer_button[lz].replace('XXXXX', message.chat.username) if message.chat.username else \
                 l_offer_button[lz].replace('XXXXX', '')
             await bot.send_message(chat_id, text)
             await state.set_state(FsmOffer.button)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     # except FileIsTooBig as e:
     #     logger.info(log_ % str(e))
     #     await asyncio.sleep(round(random.uniform(0, 1), 2))
     #     await bot.send_message(chat_id, l_offer_media_toobig[lz])
     except Exception as e:
         if 'too big' in str(e):
-            await bot.send_message(chat_id, l_.offer_media_toobig[lz])
+            await bot.send_message(chat_id, l_post_media_toobig[lz])
         else:
             logger.info(log_ % str(e))
             await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def fsm_button_admin(bot, FsmOffer, message, state, BASE_D):
     try:
@@ -2453,16 +1970,16 @@
                 await bot.send_message(chat_id, text)
                 await state.set_state(FsmOffer.button)
                 return
 
             await state.update_data(offer_button=message.text.strip())
             await generate_calendar_admin(bot, state, lz, chat_id)
             await state.set_state(FsmOffer.date_)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def fsm_date_cb_admin(bot, FsmOffer, call, state, BASE_D):
@@ -2492,16 +2009,16 @@
 
         datetime_plus = (dt_cur + datetime.timedelta(hours=1)).strftime("%H:%M")
         datetime_current = dt_cur.strftime("%H:%M")
 
         text = generate_calendar_time[lz].format(dt_user, datetime_plus, datetime_current, USER_TZ)
         await bot.send_message(chat_id, text)
         await state.set_state(FsmOffer.time_)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def calendar_handler_admin(bot, call, state, BASE_D):
@@ -2517,16 +2034,16 @@
         if shift == 'left':
             shift_month = 0 if shift_month == 0 else shift_month - 1
         elif shift == 'right':
             shift_month = shift_month + 1
 
         await state.update_data(shift_month=shift_month)
         await generate_calendar_admin(bot, state, lz, chat_id, message_id, False)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def fsm_date_admin(bot, FsmOffer, message, state, BASE_D):
@@ -2538,16 +2055,16 @@
             text = l_offer_button[lz].replace('XXXXX', message.chat.username) if message.chat.username else \
                 l_offer_button[lz].replace('XXXXX', '')
             await bot.send_message(chat_id, text)
             await state.set_state(FsmOffer.button)
         else:
             await bot.send_message(chat_id, l_offer_finish[lz])
             await state.set_state(FsmOffer.finish)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def fsm_time_admin(bot, FsmOffer, message, state, BASE_D):
@@ -2598,16 +2115,16 @@
                 return
 
             offer_dt = dt_user_new.strftime('%d-%m-%Y %H:%M')
             await state.update_data(offer_dt=offer_dt)
 
             await bot.send_message(chat_id, l_offer_finish[lz])
             await state.set_state(FsmOffer.finish)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def fsm_finish_admin(bot, FsmOffer, message, state, EXTRA_D, BASE_D):
@@ -2657,16 +2174,16 @@
 
             sql = "SELECT * FROM OFFER"
             data = await db_select(sql, (), BASE_D)
             items = [item[0] for item in data]
             view_post_id = items.index(offer_id) + 1 if offer_id else len(data)
             await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, view_post_id)
             await state.clear()
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 def get_keyboard_admin(data, src, post_id=1):
@@ -2690,16 +2207,16 @@
         chat_id = call.from_user.id
         src = call.data.split("_")[1]
         post_id = int(call.data.split("_")[-1])
         lz = await lz_code(chat_id, call.from_user.language_code, BASE_D)
         has_restricted = (await bot.get_chat(chat_id)).has_restricted_voice_and_video_messages
 
         await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, post_id, call)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def get_current_index(offer_id, inline_keyboard):
@@ -2712,16 +2229,16 @@
                         current = await parse_index(it.text.split('/')[0])
                         length = await parse_index(it.text.split('/')[1])
                         return
             elif item.callback_data == f"gallery_current_{offer_id}" and '/' in item.text:
                 current = await parse_index(item.text.split('/')[0])
                 length = await parse_index(item.text.split('/')[1])
                 return
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         return current, length
 
@@ -2730,16 +2247,16 @@
     result = None
     try:
         res = ''
         for item in str_num:
             if item in '0123456789':
                 res = f"{res}{item}"
         result = int(res) if res != '' else None
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         return result
 
@@ -2759,16 +2276,16 @@
         elif option == 'next':
             current, length = await get_current_index(offer_id, call.message.reply_markup.inline_keyboard)
             if current is None or length is None: await call.answer(); return
             current = 1 if current == length and option == 'next' else current + 1
             await send_user(bot, chat_id, offer_id, BASE_D, message_id, current)
         elif data[1] == 'current':
             pass
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 # endregion
@@ -3060,15 +2577,15 @@
         elif '@' in username and not username.startswith('@'):
             result = False
         else:
             for it in username:
                 if it not in string.ascii_letters + string.digits + "@_":
                     result = False
                     return
-    except RetryAfter as e:
+    except TelegramRetryAfter as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         return result
@@ -3194,15 +2711,15 @@
                 break
     except Exception as e:
         logger.info(log_ % str(e))
     finally:
         return result
 
 
-async def get_photo_file_id(BASE_D):
+async def get_photo_file_id(bot, chat_id, file_id_text, BASE_D):
     result = None
     try:
         sql = "SELECT FILE_FILEID FROM FILE WHERE FILE_FILENAME='text.jpg'"
         data2 = await db_select(sql, (), BASE_D)
         if not len(data2):
             res = await bot.send_photo(chat_id, text_jpeg)
             result = res.photo[-1].file_id
@@ -3300,61 +2817,19 @@
             result = 'ferey_group_europe'
     except Exception as e:
         logger.info(e)
     finally:
         return result
 
 
-async def is_bad(bot, chat_id, username, CONF_P, EXTRA_D, BASE_D, BASE_S, fields_1):
-    result = False
-    try:
-        if username and (username.startswith('kwpr') or username.startswith('kvpr')):
-            result = True
-            return
-
-        sql = "SELECT BAD_TID, BAD_OFFERBOT FROM BAD WHERE BAD_TID=?"
-        data = await db_select(sql, (chat_id,), BASE_S)
-        if not len(data): return
-        # BAD_TID, BAD_OFFERBOT = data[0]
-        # if not BAD_OFFERBOT:
-        if True:
-            result = True
-            sql = "SELECT USER_TID, USER_USERNAME, USER_FULLNAME FROM USER WHERE USER_TID=?"
-            data = await db_select(sql, (chat_id,), BASE_D)
-            if not len(data): return
-            USER_TID, USER_USERNAME, USER_FULLNAME = data[0]
-
-            # удаляем последнюю строку в Google-таблице
-            sql = "SELECT USER_TID FROM USER"
-            daat = await db_select(sql, (), BASE_D)
-            daat = [item[0] for item in daat]
-            d1 = [('', '', '', '', '', '', '', '', '', '', '', '')]
-            d2 = 'A' + str(len(daat) + 1)
-            d12 = (r_conf('db_file_id', CONF_P))[0]
-            await api_sync_update(d1, d12, d2, CONF_P, EXTRA_D)
-            sql = "DELETE FROM USER WHERE USER_TID=?"
-            await db_change(sql, (chat_id,), BASE_D)
-
-            sql = f"SELECT {fields_1} FROM USER"
-            value_many = await db_select(sql, (), BASE_D)
-            spreadsheet_id = (r_conf('db_file_id', CONF_P))[0]
-            await api_sync_all(value_many, spreadsheet_id, CONF_P, EXTRA_D)
-            await send_my_text(bot, my_tid, f"✅ Delete from user @{USER_USERNAME} ({USER_TID}) {USER_FULLNAME} ok")
-    except Exception as e:
-        await log(e)
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
 async def send_to_admins(bot, CONF_P, txt):
     try:
         for admin_id in r_conf('admin_id', CONF_P):
             try:
-                await send_my_text(bot=bot, chat_id=int(admin_id), text=txt)
+                await bot.send_message(chat_id=int(admin_id), text=txt)
             except Exception as e:
                 logger.info(log_ % str(e))
                 await asyncio.sleep(round(random.uniform(1, 2), 2))
         logger.info(log_ % txt)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
@@ -3450,24 +2925,14 @@
     await asyncio.sleep(part_of_hour + 200)
     while True:
         logger.info(log_ % f'start sending...{str(datetime.datetime.now())}')
         await api_update_send_folder(CONF_P, EXTRA_D, INI_D)
         await asyncio.sleep(one_hour - (datetime.datetime.now()).minute * 60 + 200)
 
 
-async def scheduled_minute(part_of_minute, bot, CONF_P, EXTRA_D, MEDIA_D, BASE_D):
-    logger.info(log_ % 'scheduled_minute ok')
-    await api_check_send_folder(bot, CONF_P, EXTRA_D, MEDIA_D, BASE_D)
-    await asyncio.sleep(part_of_minute)
-    while True:
-        # logger.info(log_ % f'start sending...{str(datetime.datetime.now())}')
-        await api_check_send_folder(bot, CONF_P, EXTRA_D, MEDIA_D, BASE_D)
-        await asyncio.sleep(one_minute - datetime.datetime.utcnow().second)
-
-
 async def read_likes(BASE_D, POST_ID=1):
     cnt = '⁰'
     try:
         sql = "SELECT USER_ID FROM LIKE WHERE POST_ID = ?"
         data = await db_select(sql, (POST_ID,), BASE_D)
         cnt = str(100 + len(data))
         cnt = cnt.replace('0', '⁰').replace('1', '¹').replace('2', '²').replace('3', '³').replace('4', '⁴') \
@@ -3538,20 +3003,19 @@
         # logger.info(log_ % str(e))
         pass
     finally:
         return result
 
 
 async def create_replymarkup(bot, owner_id, chat_id, offer_id, OFFER_BUTTON, BASE_D, COLUMN_OWNER="OFFER_CHATTID"):
-    result = None
+    result = InlineKeyboardBuilder()
     try:
         if OFFER_BUTTON is None or OFFER_BUTTON == '': return
         tmp = []
         dic_btns = await check_buttons(bot, None, OFFER_BUTTON)
-        result = types.InlineKeyboardMarkup()
         buttons = []
         offer_id = int(offer_id)
         for k, v in dic_btns.items():
             try:
                 if v[0]:
                     sql = f"SELECT * FROM OFFER WHERE {COLUMN_OWNER}=?"
                     data = await db_select(sql, (owner_id,), BASE_D)
@@ -3582,15 +3046,15 @@
                 await asyncio.sleep(round(random.uniform(1, 2), 2))
         if len(buttons) > 0:
             result.add(*buttons)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
-        return result
+        return result.as_markup()
 
 
 async def create_replymarkup2(bot, offer_id, OFFER_BUTTON):
     result = None
     try:
         if OFFER_BUTTON is None or OFFER_BUTTON == '': return
         tmp = []
@@ -3659,28 +3123,28 @@
                 else:
                     tmp = txt[start_[ix][0] + 1: finish_[ix][0]]
                     split_btn = tmp.strip().split('|')
                     if len(split_btn) > 1:
                         btn_name = split_btn[0].strip() if len(split_btn) > 1 else "🔗 Go"
                         btn_link = split_btn[-1].strip()
                         if not await is_url(btn_link):
-                            await send_my_text(bot, chat_id, f"🔗 {btn_link}: invalid")
+                            await bot.send_message(chat_id, f"🔗 {btn_link}: invalid")
                             return
                     else:
                         btn_name = split_btn[0]
                         # btn_link = cleanhtml(split_btn[0])[:20]
                         # btn_link = f"btn_{btn_link.encode('utf-8').hex()}"
                         btn_link = f"btn_"
 
                     result[ix] = [btn_name, btn_link]
             except Exception as e:
                 logger.info(log_ % str(e))
                 await asyncio.sleep(round(random.uniform(1, 2), 2))
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}", 95)
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}", 95)
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
@@ -4015,50 +3479,53 @@
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
 
 async def haversine(lon1, lat1, lon2, lat2):
+    result = None
     try:
         """
         Calculate the great circle distance in kilometers between two points
         on the earth (specified in decimal degrees)
         """
         # convert decimal degrees to radians
         lon1, lat1, lon2, lat2 = map(radians, [lon1, lat1, lon2, lat2])
 
         # haversine formula
         dlon = lon2 - lon1
         dlat = lat2 - lat1
         a = sin(dlat / 2) ** 2 + cos(lat1) * cos(lat2) * sin(dlon / 2) ** 2
         c = 2 * asin(sqrt(a))
         r = 6372
-        result =  c * r * 1000.0
+        result = c * r * 1000.0
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
+
+
 # endregion
 
 
 # region pyrogram
 async def get_session(SESSION_TID, SESSION_D, BASE_S, EXTRA_D, CONF_P, is_proxy=True):
     res = proxy = None
     try:
         sql = "SELECT SESSION_NAME, SESSION_APIID, SESSION_APIHASH, SESSION_PHONE FROM SESSION WHERE SESSION_TID = ?"
         data = await db_select(sql, (SESSION_TID,), BASE_S)
         if not len(data): return
         SESSION_NAME, SESSION_APIID, SESSION_APIHASH, SESSION_PHONE = data[0]
 
         if is_proxy:
-            proxy = await get_proxy(identifier, EXTRA_D, CONF_P)
+            proxy = await get_proxy(SESSION_TID, EXTRA_D, CONF_P)
 
-        res = Client(name=os.path.join(SESSIONS_D, SESSION_NAME), api_id=SESSION_APIID, api_hash=SESSION_APIHASH,
+        res = Client(name=os.path.join(SESSION_D, SESSION_NAME), api_id=SESSION_APIID, api_hash=SESSION_APIHASH,
                      device_model='IPhone',
                      system_version="6.12.0",
                      app_version="10 P (28)",
                      phone_number=SESSION_PHONE, proxy=proxy)
     finally:
         return res
 
@@ -4085,15 +3552,15 @@
                 async with await get_session(SESSION_TID, SESSIONS_D, EXTRA_D, CONF_P, BASE_S, False) as app:
                     r = await join_my_chat(bot, app, chat_id, link, SESSION_TID, BASE_S, BASE_E)
                     if r is None:
                         logger.info(log_ % f"{link} is None")
                         return
                     txt_ = f"👩🏽‍💻 Администратор закрытой группы не принял заявки на вступление"
                     if r == -1:
-                        await send_my_text(bot, chat_id, txt_)
+                        await bot.send_message(chat_id, txt_)
                         return
                     result = await app.get_chat(r.id)
                     if is_history:
                         try:
                             get_chat_history_count = await app.get_chat_history_count(r.id)
                         except Exception as e:
                             await log(e)
@@ -4154,22 +3621,22 @@
                     # get_chat https://t.me/+KO7_fV4aGKZkYTUy
                     if r == -1 or r is None: return
                     r = await app.get_chat(r.id)
                     logger.info(log_ % f"{SESSION_TID} get_chat {r.id}")
 
                     if not (r.type.value in ['group', 'supergroup']):
                         text = "🚶 Вставь ссылку на группу, а не канал"
-                        await send_my_text(bot, chat_id, text)
+                        await bot.send_message(chat_id, text)
                     elif hasattr(r.permissions, 'can_invite_users') and not r.permissions.can_invite_users:
                         text = "🚶 Зайди в «Разрешения» группы и включи <i>участникам группы</i> возможность: " \
                                "«Добавление участников»"
-                        await send_my_text(bot, chat_id, text)
+                        await bot.send_message(chat_id, text)
                     else:
                         text = "🚶 Начинаем проверку группы..\n#длительность 2мин"
-                        await send_my_text(bot, chat_id, text)
+                        await bot.send_message(chat_id, text)
                         # await asyncio.sleep(r_conf('AWAIT_JOIN'))
 
                         try:
                             get_chat_member = await app.get_chat_member(chat_id=r.id, user_id=int(SESSION_TID))
                             result = True if get_chat_member and get_chat_member.status.value == 'member' else False
                         except Exception as e:
                             await log(e)
@@ -4236,19 +3703,19 @@
         except Exception:
             pass
     except (InviteHashExpired, InviteHashInvalid) as e:
         await log(e)
         try:
             result = await app.join_chat(link)
         except Exception:
-            await send_my_text(bot, chat_id, f"▪️ Ссылка на чат {link} не валидна (или попробуйте еще раз)")
+            await bot.send_message(chat_id, f"▪️ Ссылка на чат {link} не валидна (или попробуйте еще раз)")
     except (UsernameInvalid, UsernameNotOccupied, ChannelBanned) as e:
         await log(e)
         await asyncio.sleep(round(random.uniform(1, 2), 2))
-        await send_my_text(bot, chat_id, f"▪️ Ссылка/username на группу {link} не валидна")
+        await bot.send_message(chat_id, f"▪️ Ссылка/username на группу {link} не валидна")
         await delete_invalid_chat(link, BASE_E)
     except BadRequest as e:
         await log(e)
         await asyncio.sleep(round(random.uniform(2, 3), 2))
 
         try:
             result = await app.join_chat(link)
@@ -4278,15 +3745,15 @@
         await asyncio.sleep(round(random.uniform(5, 10), 2))
 
 
 async def get_chat_members(bot, chat_id, link, SESSIONS_D, EXTRA_D, CONF_P, BASE_S, BASE_E):
     result = []
     try:
         text = f"🚶 Проверяем участников группы..\n#длительность 1мин"
-        await send_my_text(bot, chat_id, text)
+        await bot.send_message(chat_id, text)
         sql = "SELECT SESSION_TID,SESSION_STATUS FROM SESSION WHERE SESSION_SPAM IS NOT '*'"
         data = await db_select(sql, (), BASE_S)
         random.shuffle(data)
         for item in data:
             tmp_members = []
             SESSION_TID, SESSION_STATUS = item
             if not (await check_session_flood(SESSION_TID, BASE_S) and (
@@ -4310,15 +3777,15 @@
                         async for member in app.get_chat_members(r.id, filter=enums.ChatMembersFilter.SEARCH):
                             if member.user.username and not member.user.is_bot and not member.user.is_deleted and \
                                     not member.user.is_scam and not member.user.is_fake and not member.user.is_support \
                                     and str(member.user.id) not in data_:
                                 tmp_members.append(member.user.username)
                     except ChatAdminRequired as e:
                         await log(e)
-                        await send_my_text(bot, chat_id, f"🔺 Требуются права админа")
+                        await bot.send_message(chat_id, f"🔺 Требуются права админа")
                         return
                     except Exception as e:
                         await log(e)
 
                     # leave chat
                     await leave_my_chat(app, r, link)
 
@@ -4393,16 +3860,16 @@
 
         sql = "DELETE FROM COMPANY WHERE COMPANY_FROMUSERTID = ?"
         await db_change(sql, (SESSION_TID,), BASE_S)
 
         if os.path.exists(SESSION_NAME):
             os.remove(SESSION_NAME)
         await bot.send_message(my_tid, f"✅ deleteAccount {SESSION_TID} ok")
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         await log(e)
         await asyncio.sleep(round(random.uniform(1, 2), 2))
 
 
 async def delete_invalid_chat(chat, BASE_E):
@@ -4701,237 +4168,25 @@
     try:
         # USER_TID = 5150111687
         await bot.copy_message(chat_id=int(USER_TID), from_chat_id=result.chat.id, message_id=result.message_id,
                                reply_markup=result.reply_markup)
         cnt += 1
         logger.info(log_ % f"\t{cnt}. send to user {USER_TID}-{USER_USERNAME} ok")
         await asyncio.sleep(0.05)
-    except RetryAfter as e:
-        logger.info(log_ % f"RetryAfter {e.retry_after}")
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         await log(e)
         logger.info(log_ % f"\tsend to user {USER_TID}-{USER_USERNAME} error")
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return cnt
 
 
-async def api_check_send_folder(bot, CONF_P, EXTRA_D, MEDIA_D, BASE_D):
-    google_folder = r_conf('google_folder', CONF_P)
-    google_key = r_conf('google_key', CONF_P)
-    cnt = 0
-
-    for folder in google_folder:
-        try:
-            USER_TID = USER_USERNAME = None
-            sql = "SELECT USER_TID, USER_USERNAME FROM USER"
-            data = await db_select(sql, (), BASE_D)
-            result = None
-            fix_utc_now = datetime.datetime.utcnow()
-
-            for user in data:
-                try:
-                    USER_TID, USER_USERNAME = user
-                    user_datetime = fix_utc_now + datetime.timedelta(hours=0)
-                    user_datetime = datetime.datetime(year=user_datetime.year, month=user_datetime.month,
-                                                      day=user_datetime.day, hour=user_datetime.hour,
-                                                      minute=user_datetime.minute)
-                    # log(f"{user_datetime} and {datetime.datetime.strptime(folder, '%d-%m-%Y %H:%M')}")
-
-                    # if True:
-                    #     g_post_time_utc = '01-04-2022 09:00'
-                    if user_datetime == datetime.datetime.strptime(folder, "%d-%m-%Y %H:%M"):
-                        logger.info(log_ % f"\t! CHECK {folder}")
-                        logger.info(log_ % f"\tprepare send to {USER_TID} {USER_USERNAME}")
-                        if result:
-                            cnt = await send_my_copy(bot, cnt, USER_TID, USER_USERNAME, result)
-                            continue
-
-                        # drive service
-                        credentials = ServiceAccountCredentials.from_json_keyfile_name(
-                            os.path.join(EXTRA_D, (r_conf('credential_file', CONF_P))[0]),
-                            r_conf('scopes', CONF_P))
-                        http_auth = credentials.authorize(httplib2.Http())
-                        drive_service = build('drive', 'v3', http=http_auth, cache_discovery=False)
-
-                        # скачали
-                        k_info = post_media = ''
-                        dynamic_folder_name = google_key[google_folder.index(folder)]
-                        # dynamic_folder_name = (r_conf('dynamic_folder_id'))[0]
-                        file_list_dic = await api_get_file_list(drive_service, dynamic_folder_name, {})
-                        for k, v in file_list_dic.items():
-                            try:
-                                if v[0] == 'info':  # and v[2] == f"{g_post_time_utc}+{delta_hour}":
-                                    k_info = k
-                                # and v[2] == f"{g_post_time_utc}+{delta_hour}":
-                                elif v[1] != 'application/vnd.google-apps.folder':
-                                    post_media = await api_dl_file(drive_service, k, v[0], v[1], MEDIA_D)
-                                    logger.info(log_ % f'\tdl {v[0]} ok')
-                            except Exception as e:
-                                await log(e)
-                                await asyncio.sleep(round(random.uniform(1, 2), 2))
-
-                        # sheets service
-                        credentials = ServiceAccountCredentials.from_json_keyfile_name(
-                            os.path.join(EXTRA_D, (r_conf('credential_file', CONF_P))[0]),
-                            r_conf('scopes', CONF_P))
-                        http_auth = credentials.authorize(httplib2.Http())
-                        sheets_service = build('sheets', 'v4', http=http_auth, cache_discovery=False)
-
-                        # get meta from info
-                        values_list_values = sheets_service.spreadsheets().values()
-                        values_get = values_list_values.get(spreadsheetId=k_info, range='Sheet1', fields='values')
-                        values_list = values_get.execute().get('values', [])
-                        logger.info(log_ % f'\tdl info ok')
-                        post_txt = values_list[0][1] if len(values_list[0]) > 1 else ''
-                        post_btn = (values_list[1][1]) if len(values_list[1]) > 1 and values_list[1][1] else None
-                        post_url = (values_list[2][1]) if len(values_list[2]) > 1 and values_list[2][1] else None
-                        post_media_type = values_list[4][1] if len(values_list[4]) > 1 and values_list[4][1] else None
-                        post_pin = is_yes_not(values_list[5][1]) if len(values_list[5]) > 1 else False
-
-                        url = post_url if post_url else None
-                        text = post_btn if post_btn else "🔗 GO"
-                        inline_add = types.InlineKeyboardButton(text=text, url=url)
-                        reply_markup = types.InlineKeyboardMarkup().add(inline_add) if post_url else None
-                        # по умолчанию мы перезаписываем re_write=True, но в этом случае когда мы работаем с рассылкой,
-                        # то мы удаляем файл чуть выше, и загружаем
-
-                        logger.info(log_ % '\tbefore send')
-                        if post_media_type and post_media_type == 'photo':
-                            result = await send_my_photo(
-                                bot=bot,
-                                chat_id=int(USER_TID),
-                                photo_name=post_media,
-                                caption=post_txt,
-                                CONF_P=CONF_P,
-                                EXTRA_D=EXTRA_D,
-                                MEDIA_D=MEDIA_D,
-                                BASE_D=BASE_D,
-                                reply_markup=reply_markup,
-                                re_write=False
-                            )
-                        elif post_media_type and post_media_type == 'animation':  # gif == mp4
-                            result = await send_my_animation(
-                                bot=bot,
-                                chat_id=int(USER_TID),
-                                animation_name=post_media,
-                                caption=post_txt,
-                                CONF_P=CONF_P,
-                                EXTRA_D=EXTRA_D,
-                                MEDIA_D=MEDIA_D,
-                                BASE_D=BASE_D,
-                                reply_markup=reply_markup,
-                                re_write=False
-                            )
-                        elif post_media_type and post_media_type == 'video':
-                            result = await send_my_video(
-                                bot=bot,
-                                chat_id=int(USER_TID),
-                                video_name=post_media,
-                                caption=post_txt,
-                                CONF_P=CONF_P,
-                                EXTRA_D=EXTRA_D,
-                                MEDIA_D=MEDIA_D,
-                                BASE_D=BASE_D,
-                                reply_markup=reply_markup,
-                                re_write=False
-                            )
-                        elif post_media_type and post_media_type == 'audio':  # m4a, mp3, ogg + Listen Title
-                            result = await send_my_audio(
-                                bot=bot,
-                                chat_id=int(USER_TID),
-                                audio_name=post_media,
-                                caption=post_txt,
-                                CONF_P=CONF_P,
-                                EXTRA_D=EXTRA_D,
-                                MEDIA_D=MEDIA_D,
-                                BASE_D=BASE_D,
-                                reply_markup=reply_markup,
-                                re_write=False
-                            )
-                        elif post_media_type and post_media_type == 'voice':  # m4a, mp3, ogg
-                            result = await send_my_voice(
-                                bot=bot,
-                                chat_id=int(USER_TID),
-                                voice_name=post_media,
-                                caption=post_txt,
-                                CONF_P=CONF_P,
-                                EXTRA_D=EXTRA_D,
-                                MEDIA_D=MEDIA_D,
-                                BASE_D=BASE_D,
-                                reply_markup=reply_markup,
-                                re_write=False
-                            )
-                        elif post_media_type and post_media_type == 'video_note':  # < 1 min
-                            result = await send_my_video_note(
-                                bot=bot,
-                                chat_id=int(USER_TID),
-                                videonote_name=post_media,
-                                CONF_P=CONF_P,
-                                EXTRA_D=EXTRA_D,
-                                MEDIA_D=MEDIA_D,
-                                BASE_D=BASE_D,
-                                reply_markup=reply_markup,
-                                re_write=False
-                            )
-                        elif post_media_type and post_media_type == 'document':
-                            result = await send_my_doc(
-                                bot=bot,
-                                chat_id=int(USER_TID),
-                                doc_name=post_media,
-                                caption=post_txt,
-                                CONF_P=CONF_P,
-                                EXTRA_D=EXTRA_D,
-                                MEDIA_D=MEDIA_D,
-                                BASE_D=BASE_D,
-                                reply_markup=reply_markup,
-                                re_write=False
-                            )
-                        elif post_media_type and post_media_type == 'poll':
-                            result = await send_my_poll(
-                                bot=bot,
-                                chat_id=int(USER_TID),
-                                question=post_txt,
-                                options=post_media,
-                                reply_markup=reply_markup
-                            )
-                        elif post_txt != '':
-                            result = await send_my_text(
-                                bot=bot,
-                                chat_id=int(USER_TID),
-                                text=post_txt,
-                                reply_markup=reply_markup)
-                        elif post_txt == '' and post_url:
-                            result = await bot.send_message(
-                                chat_id=int(USER_TID),
-                                text=f"<a href='{post_url}'>🔗 Переходи по ссылке</a>",
-                                reply_markup=reply_markup
-                            )
-                        # проверить чему равно result если первый из USER_TID заблокирует бота
-
-                        if post_pin:
-                            await bot.pin_chat_message(chat_id=USER_TID, message_id=result.message_id,
-                                                       disable_notification=False)
-                        cnt += 1
-                        logger.info(log_ % f"\t{cnt}. send to user {USER_TID}-{USER_USERNAME} ok")
-                except RetryAfter as e:
-                    logger.info(log_ % f"RetryAfter {e.retry_after}")
-                    await asyncio.sleep(e.retry_after + 1)
-                except Exception as e:
-                    await log(e)
-                    logger.info(log_ % f"\tsend to user {USER_TID}-{USER_USERNAME} error")
-                    await asyncio.sleep(round(random.uniform(1, 2), 2))
-        except Exception as e:
-            await log(e)
-            await asyncio.sleep(round(random.uniform(1, 2), 2))
-    if cnt:
-        logger.info(log_ % f"-----send to users cnt = {cnt}-----")
-
-
 async def api_get_file_list(drive_service, folder_id, tmp_dic={} or None, parent_name='', is_file=False):
     if is_file:
         file = drive_service.files().get(fileId=folder_id, fields="id, name, size, modifiedTime, mimeType").execute()
         tmp_dic[file['id']] = [file['name'], file['mimeType'], parent_name, file['modifiedTime']]
         return tmp_dic
     q = "\'" + folder_id + "\'" + " in parents"
     fields = "nextPageToken, files(id, name, size, modifiedTime, mimeType)"
```

