# Comparing `tmp/nonebot_plugin_today_waifu-0.1.1.tar.gz` & `tmp/nonebot_plugin_today_waifu-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_today_waifu-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_today_waifu-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_today_waifu-0.1.1.tar` & `nonebot_plugin_today_waifu-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1091 2023-04-01 09:24:29.297752 nonebot_plugin_today_waifu-0.1.1/LICENSE
--rw-r--r--   0        0        0     9347 2023-04-05 10:44:56.994049 nonebot_plugin_today_waifu-0.1.1/nonebot_plugin_today_waifu/__init__.py
--rw-r--r--   0        0        0     1053 2023-04-01 10:49:28.758563 nonebot_plugin_today_waifu-0.1.1/nonebot_plugin_today_waifu/config.py
--rw-r--r--   0        0        0     5072 2023-04-01 07:20:39.639921 nonebot_plugin_today_waifu-0.1.1/nonebot_plugin_today_waifu/record.py
--rw-r--r--   0        0        0      639 2023-04-05 10:36:19.789847 nonebot_plugin_today_waifu-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5748 2023-04-05 10:50:05.976266 nonebot_plugin_today_waifu-0.1.1/README.md
--rw-r--r--   0        0        0     6478 1970-01-01 00:00:00.000000 nonebot_plugin_today_waifu-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-01 09:24:29.297752 nonebot_plugin_today_waifu-0.1.2/LICENSE
+-rw-r--r--   0        0        0     9712 2023-04-22 09:58:32.530323 nonebot_plugin_today_waifu-0.1.2/nonebot_plugin_today_waifu/__init__.py
+-rw-r--r--   0        0        0     1053 2023-04-01 10:49:28.758563 nonebot_plugin_today_waifu-0.1.2/nonebot_plugin_today_waifu/config.py
+-rw-r--r--   0        0        0     5072 2023-04-01 07:20:39.639921 nonebot_plugin_today_waifu-0.1.2/nonebot_plugin_today_waifu/record.py
+-rw-r--r--   0        0        0      639 2023-04-22 09:58:32.538447 nonebot_plugin_today_waifu-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5806 2023-04-22 09:58:32.548328 nonebot_plugin_today_waifu-0.1.2/README.md
+-rw-r--r--   0        0        0     6535 1970-01-01 00:00:00.000000 nonebot_plugin_today_waifu-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_today_waifu-0.1.1/LICENSE` & `nonebot_plugin_today_waifu-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_today_waifu-0.1.1/nonebot_plugin_today_waifu/__init__.py` & `nonebot_plugin_today_waifu-0.1.2/nonebot_plugin_today_waifu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from nonebot.adapters.onebot.v11 import GROUP, GroupMessageEvent, ActionFailed, Message
 
 from .config import Config
 from .record import get_group_record, save_group_record, construct_waifu_msg, clear_group_record, \
     construct_change_waifu_msg
 
 __plugin_name__ = '今日老婆'
+__plugin_version__ = '0.1.2'
 __plugin_meta__ = PluginMetadata(
     __plugin_name__,
     "随机抽取群友作为老婆吧！",
     (
         "指令表：\n"
         "▶ 今日老婆\n"
         "  ▷ 范围：群聊\n"
@@ -42,15 +43,15 @@
         "  ▷ 参数：\n"
         "    ▷ N：指定整数次数"
     ),
     Config,
     {
         "License": "MIT",
         "Author": "glamorgan9826",
-        "version": "0.1.1",
+        "version": __plugin_version__,
     },
 )
 
 global_config = nonebot.get_driver().config
 waifu_config: Config = Config.parse_obj(global_config.dict())
 
 plugin_aliases: List[str] = waifu_config.today_waifu_aliases
@@ -177,21 +178,25 @@
 
 
 @today_waifu.handle()
 async def _(bot: Bot, event: GroupMessageEvent):
     gid = str(event.group_id)
     uid = str(event.user_id)
     today = str(datetime.date.today())
-    group_record: Dict[str, Dict[str, Dict[str, int]]] = get_group_record(gid)  # 获取本群记录字典
+    group_record: Dict[str, Union[int, bool, Dict[str, Dict[str, int]]]] = get_group_record(gid)  # 获取本群记录字典
+    limit_times: int = group_record.setdefault('limit_times', default_limit_times)
+    allow_change_waifu: bool = group_record.setdefault('allow_change_waifu', default_allow_change_waifu)
     save = False  # 保存标记，是否将记录写入到本地文件
     is_first: bool  # 是否已经存在老婆标记
     waifu_id: int  # 老婆id
     if today not in group_record.keys():
         # 如果不存在今天的记录，清空本群记录字典，并添加今天的记录，保存标记置为真
         group_record.clear()
+        group_record['limit_times'] = limit_times
+        group_record['allow_change_waifu'] = allow_change_waifu
         group_record[today] = {}
         save = True
     group_today_record: Dict[str, Dict[str, int]] = group_record[today]  # 获取本群今日字典
     if uid in group_today_record.keys():
         # 如果用户在今天已经有老婆记录，记录已经存在老婆 同时 记录老婆id
         waifu_id: int = group_today_record[uid].get('waifu_id', 1234567)
         is_first = False
```

### Comparing `nonebot_plugin_today_waifu-0.1.1/nonebot_plugin_today_waifu/config.py` & `nonebot_plugin_today_waifu-0.1.2/nonebot_plugin_today_waifu/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_today_waifu-0.1.1/nonebot_plugin_today_waifu/record.py` & `nonebot_plugin_today_waifu-0.1.2/nonebot_plugin_today_waifu/record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_today_waifu-0.1.1/pyproject.toml` & `nonebot_plugin_today_waifu-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_today_waifu"
-version = "0.1.1"
+version = "0.1.2"
 description = "Nonebot2插件 可以随机抽取群友作为老婆"
 authors = ["glamorgan9826 <glamorgan9826@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/glamorgan9826/nonebot-plugin-today-waifu"
 repository = "https://github.com/glamorgan9826/nonebot-plugin-today-waifu"
```

### Comparing `nonebot_plugin_today_waifu-0.1.1/README.md` & `nonebot_plugin_today_waifu-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -137,8 +137,9 @@
 
 - [Nonebot](https://github.com/nonebot/nonebot2): 本项目的基础，非常好用的聊天机器人框架。
 - [dailywife](https://github.com/SonderXiaoming/dailywife): 本项目的灵感及思路来源。
 - [petpet](https://github.com/noneplugin/nonebot-plugin-petpet): 本项目获取群友头像的功能代码来源。
 
 ## 📋版本历史
 - 0.1.0 初始版本
-- 0.1.1 更新metadata及修复一些bug
+- 0.1.1 更新metadata及修复一些bug
+- 0.1.2 修复每次关闭换老婆状态无法保存bug
```

#### html2text {}

```diff
@@ -51,7 +51,8 @@
 | å¦ | ç¾¤è | è®¾ç½®æ¬ç¾¤æ¢èå©æå¤§æ¬¡æ°ï¼nä¸ºæ´æ° | ### ææå¾
 ææ  ## â¨å¶ä» - [Nonebot](https://github.com/nonebot/nonebot2):
 æ¬é¡¹ç®çåºç¡ï¼éå¸¸å¥½ç¨çèå¤©æºå¨äººæ¡æ¶ã - [dailywife]
 (https://github.com/SonderXiaoming/dailywife):
 æ¬é¡¹ç®ççµæåæè·¯æ¥æºã - [petpet](https://github.com/noneplugin/
 nonebot-plugin-petpet): æ¬é¡¹ç®è·åç¾¤åå¤´åçåè½ä»£ç æ¥æºã ##
 ðçæ¬åå² - 0.1.0 åå§çæ¬ - 0.1.1 æ´æ°metadataåä¿®å¤ä¸äºbug
+- 0.1.2 ä¿®å¤æ¯æ¬¡å³é­æ¢èå©ç¶ææ æ³ä¿å­bug
```

### Comparing `nonebot_plugin_today_waifu-0.1.1/PKG-INFO` & `nonebot_plugin_today_waifu-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-today-waifu
-Version: 0.1.1
+Version: 0.1.2
 Summary: Nonebot2插件 可以随机抽取群友作为老婆
 Home-page: https://github.com/glamorgan9826/nonebot-plugin-today-waifu
 License: MIT
 Author: glamorgan9826
 Author-email: glamorgan9826@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -159,7 +159,8 @@
 - [Nonebot](https://github.com/nonebot/nonebot2): 本项目的基础，非常好用的聊天机器人框架。
 - [dailywife](https://github.com/SonderXiaoming/dailywife): 本项目的灵感及思路来源。
 - [petpet](https://github.com/noneplugin/nonebot-plugin-petpet): 本项目获取群友头像的功能代码来源。
 
 ## 📋版本历史
 - 0.1.0 初始版本
 - 0.1.1 更新metadata及修复一些bug
+- 0.1.2 修复每次关闭换老婆状态无法保存bug
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-today-waifu Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-today-waifu Version: 0.1.2 Summary:
 Nonebot2æä»¶ å¯ä»¥éæºæ½åç¾¤åä½ä¸ºèå© Home-page: https://
 github.com/glamorgan9826/nonebot-plugin-today-waifu License: MIT Author:
 glamorgan9826 Author-email: glamorgan9826@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -63,7 +63,8 @@
 | å¦ | ç¾¤è | è®¾ç½®æ¬ç¾¤æ¢èå©æå¤§æ¬¡æ°ï¼nä¸ºæ´æ° | ### ææå¾
 ææ  ## â¨å¶ä» - [Nonebot](https://github.com/nonebot/nonebot2):
 æ¬é¡¹ç®çåºç¡ï¼éå¸¸å¥½ç¨çèå¤©æºå¨äººæ¡æ¶ã - [dailywife]
 (https://github.com/SonderXiaoming/dailywife):
 æ¬é¡¹ç®ççµæåæè·¯æ¥æºã - [petpet](https://github.com/noneplugin/
 nonebot-plugin-petpet): æ¬é¡¹ç®è·åç¾¤åå¤´åçåè½ä»£ç æ¥æºã ##
 ðçæ¬åå² - 0.1.0 åå§çæ¬ - 0.1.1 æ´æ°metadataåä¿®å¤ä¸äºbug
+- 0.1.2 ä¿®å¤æ¯æ¬¡å³é­æ¢èå©ç¶ææ æ³ä¿å­bug
```

