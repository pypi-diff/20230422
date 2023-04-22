# Comparing `tmp/teelebot-1.23.1-py3-none-any.whl.zip` & `tmp/teelebot-1.24.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 50493 bytes, number of entries: 18
+Zip file size: 50570 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat     3989 b- defN 23-Apr-19 01:18 teelebot/__init__.py
 -rw-rw-rw-  2.0 fat      163 b- defN 21-Sep-11 03:28 teelebot/__main__.py
 -rw-rw-rw-  2.0 fat     7352 b- defN 21-Sep-11 03:28 teelebot/buffer.py
 -rw-rw-rw-  2.0 fat    19354 b- defN 23-Apr-19 01:22 teelebot/handler.py
 -rw-rw-rw-  2.0 fat     1808 b- defN 21-Sep-11 03:28 teelebot/logger.py
 -rw-rw-rw-  2.0 fat      619 b- defN 22-Aug-14 05:17 teelebot/polling.py
 -rw-rw-rw-  2.0 fat     4304 b- defN 23-Apr-11 13:55 teelebot/request.py
 -rw-rw-rw-  2.0 fat     3876 b- defN 21-Sep-11 03:28 teelebot/schedule.py
--rw-rw-rw-  2.0 fat   125962 b- defN 23-Apr-19 01:18 teelebot/teelebot.py
--rw-rw-rw-  2.0 fat      478 b- defN 23-Apr-19 01:17 teelebot/version.py
+-rw-rw-rw-  2.0 fat   126542 b- defN 23-Apr-22 01:35 teelebot/teelebot.py
+-rw-rw-rw-  2.0 fat      478 b- defN 23-Apr-22 01:15 teelebot/version.py
 -rw-rw-rw-  2.0 fat     2665 b- defN 22-Aug-14 10:03 teelebot/webhook.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-Apr-19 01:37 teelebot-1.23.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    14712 b- defN 23-Apr-19 01:37 teelebot-1.23.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 01:37 teelebot-1.23.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       43 b- defN 23-Apr-19 01:37 teelebot-1.23.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-19 01:37 teelebot-1.23.1.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-19 01:37 teelebot-1.23.1.dist-info/zip-safe
--rw-rw-r--  2.0 fat     1420 b- defN 23-Apr-19 01:37 teelebot-1.23.1.dist-info/RECORD
-18 files, 222671 bytes uncompressed, 48191 bytes compressed:  78.4%
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-Apr-22 01:49 teelebot-1.24.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    14991 b- defN 23-Apr-22 01:49 teelebot-1.24.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 01:49 teelebot-1.24.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 23-Apr-22 01:49 teelebot-1.24.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-22 01:49 teelebot-1.24.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-22 01:49 teelebot-1.24.0.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     1420 b- defN 23-Apr-22 01:49 teelebot-1.24.0.dist-info/RECORD
+18 files, 223530 bytes uncompressed, 48268 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -27,29 +27,29 @@
 
 Filename: teelebot/version.py
 Comment: 
 
 Filename: teelebot/webhook.py
 Comment: 
 
-Filename: teelebot-1.23.1.dist-info/LICENSE
+Filename: teelebot-1.24.0.dist-info/LICENSE
 Comment: 
 
-Filename: teelebot-1.23.1.dist-info/METADATA
+Filename: teelebot-1.24.0.dist-info/METADATA
 Comment: 
 
-Filename: teelebot-1.23.1.dist-info/WHEEL
+Filename: teelebot-1.24.0.dist-info/WHEEL
 Comment: 
 
-Filename: teelebot-1.23.1.dist-info/entry_points.txt
+Filename: teelebot-1.24.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: teelebot-1.23.1.dist-info/top_level.txt
+Filename: teelebot-1.24.0.dist-info/top_level.txt
 Comment: 
 
-Filename: teelebot-1.23.1.dist-info/zip-safe
+Filename: teelebot-1.24.0.dist-info/zip-safe
 Comment: 
 
-Filename: teelebot-1.23.1.dist-info/RECORD
+Filename: teelebot-1.24.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teelebot/teelebot.py

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 """
 @description:基于Telegram Bot Api 的机器人框架
 @creation date: 2019-08-13
-@last modification: 2023-04-19
+@last modification: 2023-04-22
 @author: Pluto (github:plutobell)
-@version: 1.23.1
+@version: 1.24.0
 """
 import inspect
 import time
 import sys
 import os
 import json
 import string
@@ -2027,14 +2027,38 @@
             addr += "&message_id=" + str(message_id)
 
         if reply_markup is not None:
             addr += "&reply_markup=" + json.dumps(reply_markup)
 
         return self.request.post(addr)
 
+    def setMyName(self, name="", language_code=None):
+        """
+        使用此方法来改变机器人的名字
+        """
+        command = inspect.stack()[0].function
+        addr = command + "?name=" + str(name)
+
+        if language_code is not None:
+            addr += "&language_code=" + str(language_code)
+
+        return self.request.post(addr)
+    
+    def getMyName(self, language_code=None):
+        """
+        使用此方法来获取给定用户语言的当前机器人名称
+        """
+        command = inspect.stack()[0].function
+        addr = command
+
+        if language_code is not None:
+            addr += "?language_code=" + str(language_code)
+
+        return self.request.post(addr)
+
     def setMyCommands(self, commands, scope=None, language_code=None):
         """
         使用此方法更改机器人的命令列表
 
         commands传入格式示例：
             commands = [
                 {"command": "start", "description": "插件列表"},
@@ -2552,15 +2576,15 @@
         addr += command + "?chat_id=" + str(chat_id)
 
         return self.request.post(addr)
 
 
     # Inline mode
     def answerInlineQuery(self, inline_query_id, results, cache_time=None,
-        is_personal=None, next_offset=None, switch_pm_text=None, switch_pm_parameter=None):
+        is_personal=None, next_offset=None, button=None):
         """
         使用此方法发送Inline mode的应答
         results format:
             results = [
                 {
                     "type": "article",
                     "id": "item_id_1",
@@ -2587,19 +2611,17 @@
 
         if cache_time is not None:
             addr += "&cache_time=" + str(cache_time)
         if is_personal is not None:
             addr += "&is_personal=" + str(is_personal)
         if next_offset is not None:
             addr += "&next_offset=" + str(next_offset)
-        if switch_pm_text is not None:
-            addr += "&switch_pm_text=" + str(switch_pm_text)
-        if switch_pm_parameter is not None:
-            addr += "&switch_pm_parameter=" + str(switch_pm_parameter)
-
+        if button is not None:
+            addr += "&button=" + json.dumps(button)
+        
         return self.request.post(addr)
 
     def answerCallbackQuery(self, callback_query_id, text=None, show_alert=False, url=None, cache_time=0):
         """
         使用此方法发送CallbackQuery的应答
         InlineKeyboardMarkup格式:
         replyKeyboard = [
```

## teelebot/version.py

```diff
@@ -1,15 +1,15 @@
 # -*- coding:utf-8 -*-
 """
 @description:基于Telegram Bot Api 的机器人框架
 @creation date: 2019-11-15
-@last modification: 2023-04-19
+@last modification: 2023-04-22
 @author: Pluto (github:plutobell)
-@version: 1.23.1
+@version: 1.24.0
 """
 
-__version__ = "1.23.1"
+__version__ = "1.24.0"
 __author__ = "Pluto"
 __email__ = "hi@ojoll.com"
 __blog__ = "https://ojoll.com"
 __github__ = "https://github.com/plutobell/teelebot"
 __description__ = "teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend."
```

## Comparing `teelebot-1.23.1.dist-info/LICENSE` & `teelebot-1.24.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `teelebot-1.23.1.dist-info/METADATA` & `teelebot-1.24.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teelebot
-Version: 1.23.1
+Version: 1.24.0
 Summary: teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend.
 Home-page: https://ojoll.com
 Author: Pluto
 Author-email: hi@ojoll.com
 License: GPLv3
 Keywords: teelebot telegram bot telegram bot api telegram
 Classifier: Programming Language :: Python :: 3
@@ -67,15 +67,17 @@
 
 * **[方法列表](./FUNCTION.md)**
 
 
 
 ## Demo ##
 
-* ~~Telegram群组： [teelebot体验群](http://t.me/teelebot_chat)（t.me/teelebot_chat）~~
+* **Telegram Group：[teelebot official](https://t.me/teelebot_official)（t.me/teelebot_official）**
+* **Bot : [teelebotBot](https://t.me/teelebotBot)（t.me/teelebotBot）**
+* ~~Telegram Group： [teelebot体验群](http://t.me/teelebot_chat)（t.me/teelebot_chat）~~
 * ~~Bot : [teelebot](http://t.me/teelebot)（t.me/teelebot）~~
 
 
 
 
 
 
@@ -544,15 +546,16 @@
 
 
 
 ## 联系我 ##
 
 * Email：hi#ojoll.com ( # == @ )
 * Blog:    [北及](https://ojoll.com)
-* ~~Telegram群组：[teelebot体验群](http://t.me/teelebot_chat)（t.me/teelebot_chat）~~
+* Telegram Group：[teelebot official](https://t.me/teelebot_official)（t.me/teelebot_official）
+* ~~Telegram Group：[teelebot体验群](http://t.me/teelebot_chat)（t.me/teelebot_chat）~~
 * 其他：本repo 的 Issue
```

## Comparing `teelebot-1.23.1.dist-info/RECORD` & `teelebot-1.24.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 teelebot/__main__.py,sha256=SRKzFAyri9IQ-2Ox_xM3h_o9KrU4Qb2SikEGl-fhun8,163
 teelebot/buffer.py,sha256=YFYDSt7wQzko4Fuzg16PdwyjpXLpvBIK_ZHenv5gD4s,7352
 teelebot/handler.py,sha256=JPF71of7h1DBxDzjHfcjqPieO3lZh4cLMZXoo1oEjjs,19354
 teelebot/logger.py,sha256=WALHg4p9zKuBTuI9ciND-8z-dZ04kVIwgdBmQx2lk0M,1808
 teelebot/polling.py,sha256=KyfGkXHUpPBkDzB2bQRZ8btJm0EOOXoTFZpRZS0b4nM,619
 teelebot/request.py,sha256=WntfQMyHqjGFtiekGx6O-YOZV9Ljqayvr0D1hsruNs8,4304
 teelebot/schedule.py,sha256=K5eecKJD-M9h_ZXqXMlgXlo3Bq8h6unqmTWt37LZhXg,3876
-teelebot/teelebot.py,sha256=pUFK0vr4AWzQzTNCrmFJPVeN_4el74KteUhlkYIFWBo,125962
-teelebot/version.py,sha256=XYjk2mOgOCX2ZjK74JQ569xQI-2m02tNpWQ96pnyUYg,478
+teelebot/teelebot.py,sha256=VlhzbOk8l7hbO_Ra-A--y3IkhGBKA0SW2wD-eaVYX94,126542
+teelebot/version.py,sha256=Wi5aXZ6aV0B5XTqAiiXlMkOWedDxozApTiOma1kxOTc,478
 teelebot/webhook.py,sha256=LQ51F722XOJW1mdErKw-rA9AhotGJnsvR8RStDotpVM,2665
-teelebot-1.23.1.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-teelebot-1.23.1.dist-info/METADATA,sha256=zEj93Q12GwnYlwJS-92GIBLjCJk_yghMr-HS6k4l8Mw,14712
-teelebot-1.23.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-teelebot-1.23.1.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
-teelebot-1.23.1.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
-teelebot-1.23.1.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-teelebot-1.23.1.dist-info/RECORD,,
+teelebot-1.24.0.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
+teelebot-1.24.0.dist-info/METADATA,sha256=8oHLUalAdHPsDBNQGSw0F534YNJJeJoo1pYWGOFI5b4,14991
+teelebot-1.24.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+teelebot-1.24.0.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
+teelebot-1.24.0.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
+teelebot-1.24.0.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+teelebot-1.24.0.dist-info/RECORD,,
```

