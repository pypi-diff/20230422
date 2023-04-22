# Comparing `tmp/nonebot_plugin_genshinuid-4.0.4.tar.gz` & `tmp/nonebot_plugin_genshinuid-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_genshinuid-4.0.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_genshinuid-4.0.5.tar", max compression
```

## Comparing `nonebot_plugin_genshinuid-4.0.4.tar` & `nonebot_plugin_genshinuid-4.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    15002 2023-04-17 18:41:54.366553 nonebot_plugin_genshinuid-4.0.4/GenshinUID/__init__.py
--rw-r--r--   0        0        0     1227 2023-04-17 18:40:04.757027 nonebot_plugin_genshinuid-4.0.4/GenshinUID/auto_install.py
--rw-r--r--   0        0        0    23514 2023-04-17 18:42:03.040685 nonebot_plugin_genshinuid-4.0.4/GenshinUID/client.py
--rw-r--r--   0        0        0     1004 2023-04-14 17:44:32.923572 nonebot_plugin_genshinuid-4.0.4/GenshinUID/models.py
--rw-r--r--   0        0        0      336 2023-04-17 18:40:04.758052 nonebot_plugin_genshinuid-4.0.4/GenshinUID/path.py
--rw-r--r--   0        0        0    35823 2023-03-31 16:54:56.436943 nonebot_plugin_genshinuid-4.0.4/LICENSE
--rw-r--r--   0        0        0     1652 2023-04-17 18:42:29.621770 nonebot_plugin_genshinuid-4.0.4/pyproject.toml
--rw-r--r--   0        0        0     3318 2023-04-17 18:40:04.759072 nonebot_plugin_genshinuid-4.0.4/README.md
--rw-r--r--   0        0        0     4482 1970-01-01 00:00:00.000000 nonebot_plugin_genshinuid-4.0.4/PKG-INFO
+-rw-r--r--   0        0        0    15002 2023-04-18 16:20:25.532575 nonebot_plugin_genshinuid-4.0.5/GenshinUID/__init__.py
+-rw-r--r--   0        0        0     1227 2023-04-18 16:20:25.533580 nonebot_plugin_genshinuid-4.0.5/GenshinUID/auto_install.py
+-rw-r--r--   0        0        0    23544 2023-04-22 04:43:39.377571 nonebot_plugin_genshinuid-4.0.5/GenshinUID/client.py
+-rw-r--r--   0        0        0     1004 2023-04-14 17:44:32.923572 nonebot_plugin_genshinuid-4.0.5/GenshinUID/models.py
+-rw-r--r--   0        0        0      336 2023-04-18 16:20:25.609922 nonebot_plugin_genshinuid-4.0.5/GenshinUID/path.py
+-rw-r--r--   0        0        0    35823 2023-03-31 16:54:56.436943 nonebot_plugin_genshinuid-4.0.5/LICENSE
+-rw-r--r--   0        0        0     1652 2023-04-22 04:44:38.967953 nonebot_plugin_genshinuid-4.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3318 2023-04-18 16:20:25.696204 nonebot_plugin_genshinuid-4.0.5/README.md
+-rw-r--r--   0        0        0     4482 1970-01-01 00:00:00.000000 nonebot_plugin_genshinuid-4.0.5/PKG-INFO
```

### Comparing `nonebot_plugin_genshinuid-4.0.4/GenshinUID/__init__.py` & `nonebot_plugin_genshinuid-4.0.5/GenshinUID/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.4/GenshinUID/auto_install.py` & `nonebot_plugin_genshinuid-4.0.5/GenshinUID/auto_install.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.4/GenshinUID/client.py` & `nonebot_plugin_genshinuid-4.0.5/GenshinUID/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,28 +35,38 @@
     PORT = '8765'
 
 
 def _get_bot(bot_id: str) -> Bot:
     if 'v12' in bot_id:
         bot_id = 'onebotv12'
     # bots: Dict[str, str] 以适配器名称为键、bot_self_id为值的字典
+    _refresh_bots()
     if bot_id not in bots:
         for _bot_id in bots.keys():
             if bot_id in _bot_id:
                 bot_id = _bot_id
                 break
         else:
             logger.warning('未获取到正确的Bot实例,将使用默认Bot...')
             logger.warning(f'当前bot_id: {bot_id}, bots: {bots}')
             return get_bot()
     bot_real_id = bots[bot_id]
     bot = get_bot(bot_real_id)
     return bot
 
 
+def _refresh_bots():
+    global bots
+    _bots = get_bots()
+    for bot_real_id in _bots:
+        bot = _bots[bot_real_id]
+        bot_id = bot.type.lower().replace(' ', '')
+        bots[bot_id] = bot_real_id
+
+
 class GsClient:
     _instance = None
 
     @classmethod
     async def async_connect(cls, IP: str = HOST, PORT: Union[str, int] = PORT):
         self = GsClient()
         cls.is_alive = True
@@ -74,21 +84,16 @@
         # 判断sv是否已经被初始化
         if cls._instance is None:
             cls._instance = super(GsClient, cls).__new__(cls, *args, **kwargs)
         return cls._instance
 
     async def recv_msg(self):
         try:
-            global bots
             await asyncio.sleep(5)
-            _bots = get_bots()
-            for bot_real_id in _bots:
-                bot = _bots[bot_real_id]
-                bot_id = bot.type.lower().replace(' ', '')
-                bots[bot_id] = bot_real_id
+            _refresh_bots()
             async for message in self.ws:
                 try:
                     _bots = get_bots()
                     msg = msgjson.decode(message, type=MessageSend)
                     logger.info(
                         f'【接收】[gsuid-core]: '
                         f'{msg.bot_id} - {msg.target_type} - {msg.target_id}'
@@ -659,19 +664,19 @@
                 data=img_bytes,
                 name=f"{file_name}",
             )
             file_id = up_data['file_id']
             await send_file_message(params, "image", file_id)
         elif file:
             file_name, file_content = file.split('|')
-            file_content = base64.b64decode(file)
+            file_data = base64.b64decode(file_content)
             up_data = await bot.call_api(
                 'upload_file',
                 type="data",
-                data=file_content,
+                data=file_data,
                 name=f"{file_name}",
             )
             file_id = up_data['file_id']
             await send_file_message(params, "file", file_id)
 
     if node:
         for _msg in node:
```

### Comparing `nonebot_plugin_genshinuid-4.0.4/GenshinUID/models.py` & `nonebot_plugin_genshinuid-4.0.5/GenshinUID/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.4/LICENSE` & `nonebot_plugin_genshinuid-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.4/pyproject.toml` & `nonebot_plugin_genshinuid-4.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nonebot-plugin-genshinuid"
-version = "4.0.4"
+version = "4.0.5"
 description = "支持OneBot(QQ)、OneBotV12、QQ频道、微信、KOOK（开黑啦）、Telegram（电报）、FeiShu（飞书）的全功能NoneBot2原神插件"
 authors = ["KimigaiiWuyi <444835641@qq.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2"
 repository = "https://github.com/KimigaiiWuyi/GenshinUID"
 documentation = "https://docs.gsuid.gbots.work/#/"
```

### Comparing `nonebot_plugin_genshinuid-4.0.4/README.md` & `nonebot_plugin_genshinuid-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.4/PKG-INFO` & `nonebot_plugin_genshinuid-4.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-genshinuid
-Version: 4.0.4
+Version: 4.0.5
 Summary: 支持OneBot(QQ)、OneBotV12、QQ频道、微信、KOOK（开黑啦）、Telegram（电报）、FeiShu（飞书）的全功能NoneBot2原神插件
 Home-page: https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2
 License: GPL-3.0-or-later
 Author: KimigaiiWuyi
 Author-email: 444835641@qq.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-genshinuid Version: 4.0.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-genshinuid Version: 4.0.5 Summary:
 æ¯æOneBot
 (QQ)ãOneBotV12ãQQé¢éãå¾®ä¿¡ãKOOKï¼å¼é»å¦ï¼ãTelegramï¼çµæ¥ï¼ãFeiShuï¼é£ä¹¦ï¼çå¨åè½NoneBot2åç¥æä»¶
 Home-page: https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2
 License: GPL-3.0-or-later Author: KimigaiiWuyi Author-email: 444835641@qq.com
 Requires-Python: >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: GNU
 General Public License v3 or later (GPLv3+) Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

