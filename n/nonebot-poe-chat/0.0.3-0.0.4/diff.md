# Comparing `tmp/nonebot_poe_chat-0.0.3.tar.gz` & `tmp/nonebot_poe_chat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_poe_chat-0.0.3.tar", last modified: Fri Apr 21 14:57:51 2023, max compression
+gzip compressed data, was "nonebot_poe_chat-0.0.4.tar", last modified: Fri Apr 21 15:28:24 2023, max compression
```

## Comparing `nonebot_poe_chat-0.0.3.tar` & `nonebot_poe_chat-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:57:51.253945 nonebot_poe_chat-0.0.3/
--rw-rw-rw-   0        0        0    12533 2023-04-02 14:35:33.000000 nonebot_poe_chat-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2942 2023-04-21 14:57:51.253945 nonebot_poe_chat-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2447 2023-04-21 14:42:40.000000 nonebot_poe_chat-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 14:57:51.247945 nonebot_poe_chat-0.0.3/nonebot_poe_chat/
--rw-rw-rw-   0        0        0    21868 2023-04-21 14:42:29.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat/__init__.py
--rw-rw-rw-   0        0        0     3026 2023-04-21 13:10:05.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat/config.py
--rw-rw-rw-   0        0        0     4308 2023-04-21 14:52:49.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_chat.py
--rw-rw-rw-   0        0        0     1440 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_clear.py
--rw-rw-rw-   0        0        0     2898 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_create.py
--rw-rw-rw-   0        0        0     2445 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_login.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:57:51.252945 nonebot_poe_chat-0.0.3/nonebot_poe_chat.egg-info/
--rw-rw-rw-   0        0        0     2942 2023-04-21 14:57:51.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-04-21 14:57:51.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:57:51.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-21 14:57:51.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-21 14:57:51.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 14:57:51.253945 nonebot_poe_chat-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1155 2023-04-21 14:57:12.000000 nonebot_poe_chat-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:28:24.549144 nonebot_poe_chat-0.0.4/
+-rw-rw-rw-   0        0        0    12533 2023-04-02 14:35:33.000000 nonebot_poe_chat-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2942 2023-04-21 15:28:24.549144 nonebot_poe_chat-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2447 2023-04-21 14:42:40.000000 nonebot_poe_chat-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 15:28:24.541400 nonebot_poe_chat-0.0.4/nonebot_poe_chat/
+-rw-rw-rw-   0        0        0    21963 2023-04-21 15:26:53.000000 nonebot_poe_chat-0.0.4/nonebot_poe_chat/__init__.py
+-rw-rw-rw-   0        0        0     3026 2023-04-21 13:10:05.000000 nonebot_poe_chat-0.0.4/nonebot_poe_chat/config.py
+-rw-rw-rw-   0        0        0     4308 2023-04-21 14:52:49.000000 nonebot_poe_chat-0.0.4/nonebot_poe_chat/poe_chat.py
+-rw-rw-rw-   0        0        0     1440 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.4/nonebot_poe_chat/poe_clear.py
+-rw-rw-rw-   0        0        0     2898 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.4/nonebot_poe_chat/poe_create.py
+-rw-rw-rw-   0        0        0     2445 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.4/nonebot_poe_chat/poe_login.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:28:24.548146 nonebot_poe_chat-0.0.4/nonebot_poe_chat.egg-info/
+-rw-rw-rw-   0        0        0     2942 2023-04-21 15:28:24.000000 nonebot_poe_chat-0.0.4/nonebot_poe_chat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-04-21 15:28:24.000000 nonebot_poe_chat-0.0.4/nonebot_poe_chat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 15:28:24.000000 nonebot_poe_chat-0.0.4/nonebot_poe_chat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-04-21 15:28:24.000000 nonebot_poe_chat-0.0.4/nonebot_poe_chat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-21 15:28:24.000000 nonebot_poe_chat-0.0.4/nonebot_poe_chat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 15:28:24.549144 nonebot_poe_chat-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1155 2023-04-21 15:28:13.000000 nonebot_poe_chat-0.0.4/setup.py
```

### Comparing `nonebot_poe_chat-0.0.3/LICENSE.txt` & `nonebot_poe_chat-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.3/PKG-INFO` & `nonebot_poe_chat-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_poe_chat
-Version: 0.0.3
+Version: 0.0.4
 Summary: nonebot_poe_chat
 Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin
 Author-email: 1969730106@qq.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_poe_chat Version: 0.0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot_poe_chat Version: 0.0.4 Summary:
 nonebot_poe_chat Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin Author-email: 1969730106@qq.com Classifier: Programming Language
 :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE.txt
                               [nonebot_poe_chat]
```

### Comparing `nonebot_poe_chat-0.0.3/README.md` & `nonebot_poe_chat-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.3/nonebot_poe_chat/__init__.py` & `nonebot_poe_chat-0.0.4/nonebot_poe_chat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import re, json, uuid, asyncio,string,random
+from nonebot import require
+require("nonebot_plugin_guild_patch")
 from nonebot_plugin_guild_patch import GuildMessageEvent
 from nonebot.plugin import on_command, on
 from nonebot.params import ArgStr, CommandArg
 from nonebot.typing import T_State
 from nonebot.matcher import Matcher
 from nonebot.adapters.onebot.v11 import Message, Event, Bot, MessageEvent,MessageSegment
 from nonebot.internal.rule import Rule
 from playwright.async_api import async_playwright
 from .poe_chat import poe_chat
 from .poe_create import poe_create
 from .poe_clear import poe_clear
 from .poe_login import submit_email, submit_code
 from .config import Config
+name = "nonebot_poe_chat"
 #一些配置
 config = Config()
 user_dict = config.user_dict
 prompts_dict = config.prompts_dict
 user_path = config.user_path
 prompt_path = config.prompt_path
 cookie_path = config.cookie_path
```

### Comparing `nonebot_poe_chat-0.0.3/nonebot_poe_chat/config.py` & `nonebot_poe_chat-0.0.4/nonebot_poe_chat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_chat.py` & `nonebot_poe_chat-0.0.4/nonebot_poe_chat/poe_chat.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_clear.py` & `nonebot_poe_chat-0.0.4/nonebot_poe_chat/poe_clear.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_create.py` & `nonebot_poe_chat-0.0.4/nonebot_poe_chat/poe_create.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_login.py` & `nonebot_poe_chat-0.0.4/nonebot_poe_chat/poe_login.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.3/nonebot_poe_chat.egg-info/PKG-INFO` & `nonebot_poe_chat-0.0.4/nonebot_poe_chat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-poe-chat
-Version: 0.0.3
+Version: 0.0.4
 Summary: nonebot_poe_chat
 Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin
 Author-email: 1969730106@qq.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-poe-chat Version: 0.0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-poe-chat Version: 0.0.4 Summary:
 nonebot_poe_chat Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin Author-email: 1969730106@qq.com Classifier: Programming Language
 :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE.txt
                               [nonebot_poe_chat]
```

### Comparing `nonebot_poe_chat-0.0.3/setup.py` & `nonebot_poe_chat-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot_poe_chat",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.3",  # 程序版本
+    version="0.0.4",  # 程序版本
     author="canxin",  # 项目作者
     author_email="1969730106@qq.com",  # 作者邮件
     description="nonebot_poe_chat",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/canxin121/nonebot_poe_chat",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

