# Comparing `tmp/nonebot_poe_chat-0.0.5.tar.gz` & `tmp/nonebot_poe_chat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_poe_chat-0.0.5.tar", last modified: Sat Apr 22 03:54:44 2023, max compression
+gzip compressed data, was "nonebot_poe_chat-0.0.6.tar", last modified: Sat Apr 22 14:42:46 2023, max compression
```

## Comparing `nonebot_poe_chat-0.0.5.tar` & `nonebot_poe_chat-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 03:54:44.311411 nonebot_poe_chat-0.0.5/
--rw-rw-rw-   0        0        0    12533 2023-04-02 14:35:33.000000 nonebot_poe_chat-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     2950 2023-04-22 03:54:44.310411 nonebot_poe_chat-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2455 2023-04-21 15:29:49.000000 nonebot_poe_chat-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 03:54:44.299410 nonebot_poe_chat-0.0.5/nonebot_poe_chat/
--rw-rw-rw-   0        0        0    21963 2023-04-22 03:53:45.000000 nonebot_poe_chat-0.0.5/nonebot_poe_chat/__init__.py
--rw-rw-rw-   0        0        0     3026 2023-04-21 13:10:05.000000 nonebot_poe_chat-0.0.5/nonebot_poe_chat/config.py
--rw-rw-rw-   0        0        0     4341 2023-04-22 03:53:08.000000 nonebot_poe_chat-0.0.5/nonebot_poe_chat/poe_chat.py
--rw-rw-rw-   0        0        0     1440 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.5/nonebot_poe_chat/poe_clear.py
--rw-rw-rw-   0        0        0     2898 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.5/nonebot_poe_chat/poe_create.py
--rw-rw-rw-   0        0        0     2445 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.5/nonebot_poe_chat/poe_login.py
-drwxrwxrwx   0        0        0        0 2023-04-22 03:54:44.307412 nonebot_poe_chat-0.0.5/nonebot_poe_chat.egg-info/
--rw-rw-rw-   0        0        0     2950 2023-04-22 03:54:44.000000 nonebot_poe_chat-0.0.5/nonebot_poe_chat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-04-22 03:54:44.000000 nonebot_poe_chat-0.0.5/nonebot_poe_chat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 03:54:44.000000 nonebot_poe_chat-0.0.5/nonebot_poe_chat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-22 03:54:44.000000 nonebot_poe_chat-0.0.5/nonebot_poe_chat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-22 03:54:44.000000 nonebot_poe_chat-0.0.5/nonebot_poe_chat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 03:54:44.311411 nonebot_poe_chat-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1155 2023-04-22 03:53:52.000000 nonebot_poe_chat-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:42:46.197298 nonebot_poe_chat-0.0.6/
+-rw-rw-rw-   0        0        0    12533 2023-04-02 14:35:33.000000 nonebot_poe_chat-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     3044 2023-04-22 14:42:46.196298 nonebot_poe_chat-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2549 2023-04-22 14:39:54.000000 nonebot_poe_chat-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 14:42:46.191298 nonebot_poe_chat-0.0.6/nonebot_poe_chat/
+-rw-rw-rw-   0        0        0    23223 2023-04-22 14:35:13.000000 nonebot_poe_chat-0.0.6/nonebot_poe_chat/__init__.py
+-rw-rw-rw-   0        0        0     3026 2023-04-21 14:27:42.000000 nonebot_poe_chat-0.0.6/nonebot_poe_chat/config.py
+-rw-rw-rw-   0        0        0     4112 2023-04-22 14:35:57.000000 nonebot_poe_chat-0.0.6/nonebot_poe_chat/poe_chat.py
+-rw-rw-rw-   0        0        0     1440 2023-04-21 14:27:42.000000 nonebot_poe_chat-0.0.6/nonebot_poe_chat/poe_clear.py
+-rw-rw-rw-   0        0        0     2884 2023-04-21 14:53:32.000000 nonebot_poe_chat-0.0.6/nonebot_poe_chat/poe_create.py
+-rw-rw-rw-   0        0        0     1261 2023-04-22 14:26:17.000000 nonebot_poe_chat-0.0.6/nonebot_poe_chat/poe_func.py
+-rw-rw-rw-   0        0        0     2394 2023-04-22 14:36:31.000000 nonebot_poe_chat-0.0.6/nonebot_poe_chat/poe_login.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:42:46.195298 nonebot_poe_chat-0.0.6/nonebot_poe_chat.egg-info/
+-rw-rw-rw-   0        0        0     3044 2023-04-22 14:42:46.000000 nonebot_poe_chat-0.0.6/nonebot_poe_chat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-04-22 14:42:46.000000 nonebot_poe_chat-0.0.6/nonebot_poe_chat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 14:42:46.000000 nonebot_poe_chat-0.0.6/nonebot_poe_chat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-04-22 14:42:46.000000 nonebot_poe_chat-0.0.6/nonebot_poe_chat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-22 14:42:46.000000 nonebot_poe_chat-0.0.6/nonebot_poe_chat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 14:42:46.197298 nonebot_poe_chat-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1155 2023-04-22 14:41:19.000000 nonebot_poe_chat-0.0.6/setup.py
```

### Comparing `nonebot_poe_chat-0.0.5/LICENSE.txt` & `nonebot_poe_chat-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.5/PKG-INFO` & `nonebot_poe_chat-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_poe_chat
-Version: 0.0.5
+Version: 0.0.6
 Summary: nonebot_poe_chat
 Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin
 Author-email: 1969730106@qq.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -43,20 +43,26 @@
 ~切换机器人:poeswitch / 切换bot / ps  
   
 ************************  
 --以下功能仅限poe管理员可以使用  
 ~登录:poelogin / plogin / pl  
 ~添加预设:poeaddprompt / 添加预设 / pap  
 ~删除预设:poeremoveprompt / 删除预设 / prp  
-  
-## pip安装并添加到pyproject.toml的plugins列表中  
+# 安装  
+## step.1  
+### nb安装  
+```
+nb plugin install nonebot-poe-chat
+```
+### 或者pip安装并添加到pyproject.toml的plugins列表中  
 ```
 pip install nonebot-poe-chat
 ```
-##然后  
+ 
+## step.2  
 ```
 playwright install chromuim
 ```
 ## 配置（在.env中修改）  
 
 ```
 #poe_cookie,poe网站的ck，见后文截图，也可以不填，而使用/pl命令登陆
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_poe_chat Version: 0.0.5 Summary:
+Metadata-Version: 2.1 Name: nonebot_poe_chat Version: 0.0.6 Summary:
 nonebot_poe_chat Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin Author-email: 1969730106@qq.com Classifier: Programming Language
 :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE.txt
                               [nonebot_poe_chat]
@@ -20,17 +20,18 @@
 æºå¨äººçåç­ä¼ä»¥åå¤å½¢å¼åé --æä»¶å¨å­æ°æ®æ¾ç½®å¨./data/
 poe_chatä¸­ ## åè½ä½¿ç¨ --ä»¥ä¸å½ä»¤åé¢å¨é¨è¦å  / ~å¸®å©:poehelp
 / poeå¸®å© ~å¯¹è¯:poetalk / ptalk / pt ~æ¸ç©ºåå²å¯¹è¯:poedump / pdump /
 pd ~åå»ºæºå¨äºº:poecreate / åå»ºbot / pc ~å é¤æºå¨äºº:poeremove /
 å é¤bot / pr ~åæ¢æºå¨äºº:poeswitch / åæ¢bot / ps
 ************************ --ä»¥ä¸åè½ä»époeç®¡çåå¯ä»¥ä½¿ç¨ ~ç»å½:
 poelogin / plogin / pl ~æ·»å é¢è®¾:poeaddprompt / æ·»å é¢è®¾ / pap
-~å é¤é¢è®¾:poeremoveprompt / å é¤é¢è®¾ / prp ##
-pipå®è£å¹¶æ·»å å°pyproject.tomlçpluginsåè¡¨ä¸­ ``` pip install nonebot-
-poe-chat ``` ##ç¶å ``` playwright install chromuim ``` ##
+~å é¤é¢è®¾:poeremoveprompt / å é¤é¢è®¾ / prp # å®è£ ## step.1 ###
+nbå®è£ ``` nb plugin install nonebot-poe-chat ``` ###
+æèpipå®è£å¹¶æ·»å å°pyproject.tomlçpluginsåè¡¨ä¸­ ``` pip install
+nonebot-poe-chat ``` ## step.2 ``` playwright install chromuim ``` ##
 éç½®ï¼å¨.envä¸­ä¿®æ¹ï¼ ```
 #poe_cookie,poeç½ç«çckï¼è§åææªå¾ï¼ä¹å¯ä»¥ä¸å¡«ï¼èä½¿ç¨/
 plå½ä»¤ç»é poe_cookie = "f87HlVW~~%3D%3D"
 #poe_superusersï¼poeæä»¶ç®¡çåqqå· poe_superusers = ["123456","132145"]
 ``` ![ckè·å](https://github.com/canxin121/nonebot_poe_chat/blob/main/
 resource/ck.png) ## ç¤ºä¾ | Image 1 | Image 2 | |:-------:|:-------:| | ![]
 (https://github.com/canxin121/nonebot_poe_chat/blob/main/resource/demo%20
```

### Comparing `nonebot_poe_chat-0.0.5/README.md` & `nonebot_poe_chat-0.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -29,20 +29,26 @@
 ~切换机器人:poeswitch / 切换bot / ps  
   
 ************************  
 --以下功能仅限poe管理员可以使用  
 ~登录:poelogin / plogin / pl  
 ~添加预设:poeaddprompt / 添加预设 / pap  
 ~删除预设:poeremoveprompt / 删除预设 / prp  
-  
-## pip安装并添加到pyproject.toml的plugins列表中  
+# 安装  
+## step.1  
+### nb安装  
+```
+nb plugin install nonebot-poe-chat
+```
+### 或者pip安装并添加到pyproject.toml的plugins列表中  
 ```
 pip install nonebot-poe-chat
 ```
-##然后  
+ 
+## step.2  
 ```
 playwright install chromuim
 ```
 ## 配置（在.env中修改）  
 
 ```
 #poe_cookie,poe网站的ck，见后文截图，也可以不填，而使用/pl命令登陆
```

#### html2text {}

```diff
@@ -13,17 +13,18 @@
 æºå¨äººçåç­ä¼ä»¥åå¤å½¢å¼åé --æä»¶å¨å­æ°æ®æ¾ç½®å¨./data/
 poe_chatä¸­ ## åè½ä½¿ç¨ --ä»¥ä¸å½ä»¤åé¢å¨é¨è¦å  / ~å¸®å©:poehelp
 / poeå¸®å© ~å¯¹è¯:poetalk / ptalk / pt ~æ¸ç©ºåå²å¯¹è¯:poedump / pdump /
 pd ~åå»ºæºå¨äºº:poecreate / åå»ºbot / pc ~å é¤æºå¨äºº:poeremove /
 å é¤bot / pr ~åæ¢æºå¨äºº:poeswitch / åæ¢bot / ps
 ************************ --ä»¥ä¸åè½ä»époeç®¡çåå¯ä»¥ä½¿ç¨ ~ç»å½:
 poelogin / plogin / pl ~æ·»å é¢è®¾:poeaddprompt / æ·»å é¢è®¾ / pap
-~å é¤é¢è®¾:poeremoveprompt / å é¤é¢è®¾ / prp ##
-pipå®è£å¹¶æ·»å å°pyproject.tomlçpluginsåè¡¨ä¸­ ``` pip install nonebot-
-poe-chat ``` ##ç¶å ``` playwright install chromuim ``` ##
+~å é¤é¢è®¾:poeremoveprompt / å é¤é¢è®¾ / prp # å®è£ ## step.1 ###
+nbå®è£ ``` nb plugin install nonebot-poe-chat ``` ###
+æèpipå®è£å¹¶æ·»å å°pyproject.tomlçpluginsåè¡¨ä¸­ ``` pip install
+nonebot-poe-chat ``` ## step.2 ``` playwright install chromuim ``` ##
 éç½®ï¼å¨.envä¸­ä¿®æ¹ï¼ ```
 #poe_cookie,poeç½ç«çckï¼è§åææªå¾ï¼ä¹å¯ä»¥ä¸å¡«ï¼èä½¿ç¨/
 plå½ä»¤ç»é poe_cookie = "f87HlVW~~%3D%3D"
 #poe_superusersï¼poeæä»¶ç®¡çåqqå· poe_superusers = ["123456","132145"]
 ``` ![ckè·å](https://github.com/canxin121/nonebot_poe_chat/blob/main/
 resource/ck.png) ## ç¤ºä¾ | Image 1 | Image 2 | |:-------:|:-------:| | ![]
 (https://github.com/canxin121/nonebot_poe_chat/blob/main/resource/demo%20
```

### Comparing `nonebot_poe_chat-0.0.5/nonebot_poe_chat/__init__.py` & `nonebot_poe_chat-0.0.6/nonebot_poe_chat/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,123 +1,125 @@
-import re, json, uuid, asyncio,string,random
-from nonebot import require
-require("nonebot_plugin_guild_patch")
-from nonebot_plugin_guild_patch import GuildMessageEvent
+import json,asyncio
 from nonebot.plugin import on_command, on
 from nonebot.params import ArgStr, CommandArg
 from nonebot.typing import T_State
 from nonebot.matcher import Matcher
-from nonebot.adapters.onebot.v11 import Message, Event, Bot, MessageEvent,MessageSegment
+from nonebot.adapters.onebot.v11 import Message, Event, Bot, MessageEvent
 from nonebot.internal.rule import Rule
 from playwright.async_api import async_playwright
 from .poe_chat import poe_chat
 from .poe_create import poe_create
 from .poe_clear import poe_clear
 from .poe_login import submit_email, submit_code
 from .config import Config
-name = "nonebot_poe_chat"
+from .poe_func import reply_out,generate_uuid,generate_random_string,is_email
 #一些配置
 config = Config()
 user_dict = config.user_dict
 prompts_dict = config.prompts_dict
 user_path = config.user_path
 prompt_path = config.prompt_path
 cookie_path = config.cookie_path
 superusers = config.superusers
 is_cookie_exists = config.is_cookie_exists
 
-def reply_out(event: MessageEvent, content: MessageSegment | Message | str) -> Message:
-    """返回一个回复消息"""
-    if isinstance(event, GuildMessageEvent):
-        return Message(content)
-
-    return MessageSegment.reply(event.message_id) + content
 ######################################################
-#生成一个由qq号和nickname共同决定的uuid作为真名，防止重名
-def generate_uuid(s):
-    # 将字符串转换为 UUID 对象
-    uuid_object = uuid.uuid3(uuid.NAMESPACE_DNS, s)
-    # 获取 UUID 对象的 bytes 值
-    uuid_bytes = uuid_object.bytes
-    # 将 bytes 值转换为字符串
-    uuid_str = uuid_bytes.hex()[:14]
-    return uuid_str
 
+async def delete_messages(bot, user_id, dict_list):
+    if user_id in dict_list:
+        for eachmsg in dict_list[user_id]:
+            await bot.delete_msg(message_id=eachmsg['message_id'])
+        del dict_list[user_id]
+create_msgs = {}
 poe_create_ = on_command(
     "poecreate",
     aliases={
         "创建bot",
         "pc"
         },
     priority=4,
     block=False)
 @poe_create_.handle()
 async def __(matcher:Matcher,state: T_State,event: Event):
+    create_msgs[str(event.user_id)] = []
     state["user_id"] = str(event.user_id)
     if not is_cookie_exists:
         await matcher.finish(reply_out(event, "管理员还没填写可用的poe_cookie或登陆"))
     else:
         if len(prompts_dict)>0:
             str_prompts = str()
             for key, _ in prompts_dict.items():
                 str_prompts += f"{key}\n"
-            await matcher.send(reply_out(event, f"当前预设有：\n{str_prompts}"))
+            # create_msgs[str(event.user_id)].append(await matcher.send(reply_out(event, f"当前预设有：\n{str_prompts}")))
+            msg = f"当前预设有：\n{str_prompts}\n请输入\n1.机器人名称,\n2.基础模型选项，可选项为（gpt3_5输入1,claude输入2）,\n3.自定义预设（预设内容中间不要有空格） 或 \".\" + 可用本地预设名\n三个参数中间用空格隔开\n最终格式示例:\n示例一：chat 2 一个智能助理\n示例二： claude 1 .默认\n输入取消 或 算了可以终止创建"
+            create_msgs[str(event.user_id)].append(await matcher.send(reply_out(event, msg)))
         else:
-            await matcher.send(reply_out(event, "当前没有本地预设"))
+            create_msgs[str(event.user_id)].append(await matcher.send(reply_out(event, "")))
+            msg = f"当前没有可用本地预设\n\n请输入\n1.机器人名称,\n2.基础模型选项，可选项为（gpt3_5输入1,claude输入2）,\n3.自定义预设（预设内容中间不要有空格） 或 \".\" + 可用本地预设名\n三个参数中间用空格隔开\n最终格式示例:\n示例一：chat 2 一个智能助理\n示例二： claude 1 .默认\n输入取消 或 算了可以终止创建"
+            create_msgs[str(event.user_id)].append(await matcher.send(reply_out(event, msg)))
 
-@poe_create_.got('model',prompt='请输入\n1.机器人名称,\n2.基础模型选项，可选项为（gpt3_5输入1,claude输入2）,\n3.自定义预设（预设内容中间不要有空格） 或 "." + 可用本地预设名\n三个参数中间用空格隔开\n最终格式示例:\n示例一：chat 2 一个智能助理\n示例二： claude 1 .默认\n输入取消 或 算了可以终止创建')
-async def __poe_create___(matcher:Matcher,event:Event,state: T_State, infos: str = ArgStr("model")):
+@poe_create_.got('model')
+async def __poe_create___(bot: Bot,matcher: Matcher,event: Event,state: T_State, infos: str = ArgStr("model")):
     if infos in ["取消", "算了"]:
-        await matcher.finish(reply_out(event, "取消创建"))
+        create_msgs[str(event.user_id)].append(await matcher.send(reply_out(event, "取消创建")))
+        await asyncio.sleep(1)
+        await delete_messages(bot,str(event.user_id),create_msgs)
+        await poe_create_.finish()
     infos = infos.split(" ")
     if not (len(infos) == 3 and infos[1] in ['1', '2']):
-        await matcher.reject(reply_out(event, "输入信息有误，请检查后重新输入"))
+        create_msgs[str(event.user_id)].append(await matcher.send(reply_out(event, "输入信息有误，请检查后重新输入")))
+        await poe_create_.reject()
     #获取创建所需信息
     userid = str(state['user_id'])
     nickname = str(infos[0])
     truename = str(generate_uuid(str(userid + infos[0])))
     prompt = str(infos[2])
     bot_index = str(infos[1])
     if prompt.startswith("."):
         prompt_name = prompt[1:]
         if prompt_name in prompts_dict:
             prompt = prompts_dict[prompt_name]
         else:
-            await matcher.reject(reply_out(event, "输入的本地预设名不正确，请重新输入"))
+            create_msgs[str(event.user_id)].append(await matcher.send(reply_out(event, "输入的本地预设名不正确，请重新输入")))
+            await poe_create_.reject()
     
     if not userid in user_dict:
         user_dict[userid] = {}
     if 'all' not in user_dict[userid]:
         user_dict[userid]['all'] = {}
     if 'now' not in user_dict[userid]:
         user_dict[userid]['now'] = {}
     #查看对应用户下是不是有重名的bot
     if  nickname in user_dict[userid]['all']:
-        await matcher.reject(reply_out(event, "已经有同名的bot了，换一个名字重新输入吧"))
+        create_msgs[str(event.user_id)].append(await matcher.send(reply_out(event, "已经有同名的bot了，换一个名字重新输入吧")))
+        await poe_create_.reject()
     else:
         is_created = await poe_create(cookie_path,truename,int(bot_index),prompt)
         if is_created:
             # # 将更新后的字典写回到JSON文件中
             user_dict[userid]['all'][nickname] = truename
             
             if user_dict[userid]['now']:
                 user_dict[userid]['now'] = {}
             user_dict[userid]['now'][nickname] = truename
             
             with open(user_path, 'w') as f:
                 json.dump(user_dict, f)
-            await matcher.finish(reply_out(event, "创建成功并切换到新建bot"))
-        else:
-            await matcher.finish(reply_out(event, "出错了，多次出错请联系机器人管理员"))
+
+            await matcher.send(reply_out(event, "创建成功并切换到新建bot"))
+            await asyncio.sleep(1)
+            await delete_messages(bot,userid,create_msgs)
+            await poe_switch.finish()
+        else: 
+            await matcher.send(reply_out(event, "出错了，多次出错请联系机器人管理员"))
+            await asyncio.sleep(1)
+            await delete_messages(bot,userid,create_msgs)
+            await poe_switch.finish()
 
 ######################################################    
-def generate_random_string(length=8):
-    """生成指定长度的随机字符串"""
-    letters = string.ascii_letters + string.digits
-    return ''.join(random.choice(letters) for _ in range(length))
 
 #保留上一个回答的chatsuggest
 chat_lock = asyncio.Semaphore(3)
 chat_suggest = {}
 waitque = []
 poe_chat_ = on_command(
     "poetalk",
@@ -259,58 +261,69 @@
     nickname = str(list(user_dict[userid]["now"].keys())[0])
     is_cleared = await poe_clear(cookie_path,botname)
     if is_cleared:
         msg = f"成功清除了{nickname}的历史消息"
     else:
         msg = "出错了，多次错误请联系机器人主人"
     await matcher.finish(reply_out(event, msg))
-    
+switch_msgs = {}    
 ######################################################
 poe_switch = on_command(
     "poeswitch",
     aliases={
         "切换bot",
         "ps"
         },
     priority=4,
     block=False)
 @poe_switch.handle()
-async def __poe_switch__(matcher:Matcher,event: Event):
+async def __poe_switch__(bot:Bot ,matcher:Matcher,event: Event):
     if not is_cookie_exists:
         await matcher.finish(reply_out(event, "管理员还没填写可用的poe_cookie或登陆"))
     userid = str(event.user_id)
+    switch_msgs[userid] = []
     if userid not in user_dict:
         await matcher.finish(reply_out(event, "你还没创建任何bot"))
     bots = list(user_dict[userid]["all"].keys())
     bot_str = '\n'.join(str(bot) for bot in bots)
     # bot_truname = str(list(user_dict[userid]["now"].values())[0])
     nickname = str(list(user_dict[userid]["now"].keys())[0])
     if len(bots)==1:
-        await matcher.finish(reply_out(event, f"当前只有一个bot:{nickname}"))
-    msg = "你已经创建的的bot有：\n" + bot_str +f"\n当前使用的bot是{nickname}"
-    await matcher.send(reply_out(event, msg))
+        switch_msgs[userid].append(await matcher.send(reply_out(event, f"当前只有一个bot:{nickname}")))
+        await asyncio.sleep(1)
+        await delete_messages(bot,userid,switch_msgs)
+        await poe_switch.finish()
+    msg = "你已经创建的的bot有：\n" + bot_str +f"\n当前使用的bot是{nickname}\n\n请输入要切换的机器人名称"
+    switch_msgs[userid].append(await matcher.send(reply_out(event, msg)))
 
-@poe_switch.got('nickname',prompt='请输入要切换的机器人名称')
-async def __poe_switch____(matcher:Matcher,event: Event, infos: str = ArgStr("nickname")):
+@poe_switch.got('nickname')
+async def __poe_switch____(bot:Bot,matcher:Matcher,event: Event, infos: str = ArgStr("nickname")):
     userid = str(event.user_id)
     bots = list(user_dict[userid]["all"].keys())
     if infos in ["取消", "算了"]:
-        await matcher.finish(reply_out(event, "中断切换"))
+        switch_msgs[userid].append(await matcher.send(reply_out(event, "中断切换")))
+        await asyncio.sleep(1)
+        await delete_messages(bot,userid,switch_msgs)
+        await poe_switch.finish()
     infos = infos.split(" ")
     nickname = infos[0]
     if not (nickname in bots):
-        await matcher.reject(reply_out(event, "输入信息有误，请检查后重新输入"))
+        switch_msgs[userid].append(await matcher.send(reply_out(event, "输入信息有误，请检查后重新输入")))
+        await poe_switch.reject()
     to_truename = user_dict[userid]["all"][nickname]
     del user_dict[userid]["now"]
     user_dict[userid]["now"] = {}
     user_dict[userid]["now"][nickname] = to_truename
     with open(user_path, 'w') as f:
         json.dump(user_dict, f)
     msg = f"已切换为{nickname}"
-    await matcher.finish(reply_out(event, msg))
+    await matcher.send(reply_out(event, msg))
+    await asyncio.sleep(1)
+    await delete_messages(bot,userid,switch_msgs)
+    await poe_switch.finish()
     
 ######################################################
 poe_remove = on_command(
     "poeremove",
     aliases={
         "删除bot",
         "pr"
@@ -324,18 +337,18 @@
     userid = str(event.user_id)
     if userid not in user_dict:
         await matcher.finish(reply_out(event, "你还没创建任何bot"))
     bots = list(user_dict[userid]["all"].keys())
     bot_str = '\n'.join(str(bot) for bot in bots)
     # bot_truname = str(list(user_dict[userid]["now"].values())[0])
     nickname = str(list(user_dict[userid]["now"].keys())[0])
-    msg = "你已经创建的的bot有：\n" + bot_str +f"\n当前使用的bot是{nickname}"
+    msg = "你已经创建的的bot有：\n" + bot_str +f"\n当前使用的bot是{nickname}\n\n请输入要删除的机器人名称"
     await matcher.send(reply_out(event, msg))
 
-@poe_remove.got('nickname',prompt='请输入要删除的机器人名称')
+@poe_remove.got('nickname')
 async def __poe_remove____(matcher:Matcher,event: Event, infos: str = ArgStr("nickname")):
     userid = str(event.user_id)
     bots = list(user_dict[userid]["all"].keys())
     if infos in ["取消", "算了"]:
         await matcher.finish(reply_out(event, "终止切换"))
     infos = infos.split(" ")
     nickname_delete = infos[0]
@@ -347,19 +360,14 @@
     del user_dict[userid]["all"][nickname_delete]
     with open(user_path, 'w') as f:
         json.dump(user_dict, f)
     await matcher.finish(reply_out(event, f"已删除{nickname_delete}"))
     
 #####################################################
 
-def is_email(email):
-    pattern = r'^[\w\.-]+@[\w\.-]+\.[a-zA-Z]{2,}$'
-    return bool(re.match(pattern, email))
-
-
 poe_login = on_command(
     "poelogin",
     aliases={
         "poe登陆",
         "pl"
         },
     priority=4,
@@ -504,15 +512,15 @@
     aliases={
         "poe帮助",
         "ph"
         },
     priority=4,
     block=False)
 @poe_help.handle()
-async def __poe_help__(event: Event):
+async def __poe_help__(bot: Bot,event: Event):
     msg = (
     "-poe功能大全\n"
     "--注意所有功能都是用户独立的，每个用户只能操作自己的内容\n"
     "--所有分步操作都可以用 取消 或 算了来终止,并且支持错误重输\n"
     "--如果未创建机器人，对话命令将默认创建gpt3.5\n"
     "--可以直接回复机器人给你的回答来继续对话，无需命令\n"
     "--可以使用数字索引来使用建议回复\n\n"
@@ -524,8 +532,11 @@
     "~切换机器人:poeswitch / 切换bot / ps\n\n"
     "************************\n"
     "--以下功能仅限poe管理员使用\n"
     "~登录:poelogin / plogin / pl\n"
     "~添加预设:poeaddprompt / 添加预设 / pap\n"
     "~删除预设:poeremoveprompt / 删除预设 / prp"
     )
-    await poe_help.finish(msg)
+    
+    helpmsg = await poe_help.send(msg)
+    await bot.delete_msg(message_id=helpmsg['message_id'])
+    await poe_help.finish()
```

### Comparing `nonebot_poe_chat-0.0.5/nonebot_poe_chat/config.py` & `nonebot_poe_chat-0.0.6/nonebot_poe_chat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.5/nonebot_poe_chat/poe_chat.py` & `nonebot_poe_chat-0.0.6/nonebot_poe_chat/poe_chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import asyncio
 import json
 import re
-from playwright.async_api import Playwright as AsyncPlaywright
 from playwright.async_api import async_playwright
-from playwright._impl._api_types import Error as PlaywrightError
-from playwright.sync_api import TimeoutError as SyncTimeoutError
 from playwright.sync_api import Page
 
 async def send_message_async(page: Page, botname: str, input_str: str):
     # 定义重试次数和重试间隔时间
     retry_count = 5
     retry_interval = 0.5
 
@@ -89,17 +86,15 @@
         await context.add_cookies(cookies=cookies)
         is_banned = await send_message_async(page, botname, question)
         if is_banned == "banned":
             return "banned"
         result = await get_message_async(page, botname, sleep=5)
         if isinstance(result, tuple):
             answers, suggests = result
-            return answers[-1],suggests
         elif isinstance(result, str):
             is_banned = result
             return "banned"
         elif isinstance(result, bool):
             is_got = result
-            return is_got
         else:
             raise ValueError("Unexpected return type from get_message_async")
-
+        return answers[-1],suggests
```

#### html2text {}

```diff
@@ -1,24 +1,21 @@
 import asyncio import json import re from playwright.async_api import
-Playwright as AsyncPlaywright from playwright.async_api import async_playwright
-from playwright._impl._api_types import Error as PlaywrightError from
-playwright.sync_api import TimeoutError as SyncTimeoutError from
-playwright.sync_api import Page async def send_message_async(page: Page,
-botname: str, input_str: str): # å®ä¹éè¯æ¬¡æ°åéè¯é´éæ¶é´
-retry_count = 5 retry_interval = 0.5 # å®ä¹å½åéè¯æ¬¡æ°åæ¥éæ¬¡æ°
-current_retry = 0 error_count = 0 while current_retry < retry_count: try: #
-æå¼ç®æ ç½é¡µ await page.goto(f'https://poe.com/{botname}') text = "This
-bot has been deleted for violating our" content = await page.content() if text
-in content: return "banned" # æ¾å°è¾å¥æ¡åç´  input_box = await
-page.wait_for_selector('.ChatMessageInputView_textInput__Aervw') #
-å°å­ç¬¦ä¸²åéå°è¾å¥æ¡ä¸­ await input_box.fill(input_str) #
-æ¾å°åéæé®åç´ å¹¶ç¹å» await page.wait_for_selector
-('button.Button_primary__pIDjn') send_button = await page.wait_for_selector
-('button.Button_primary__pIDjn') # await asyncio.sleep(0.5) await
-send_button.click() # åéæååéåºå¾ªç¯ break except: #
+async_playwright from playwright.sync_api import Page async def
+send_message_async(page: Page, botname: str, input_str: str): #
+å®ä¹éè¯æ¬¡æ°åéè¯é´éæ¶é´ retry_count = 5 retry_interval = 0.5 #
+å®ä¹å½åéè¯æ¬¡æ°åæ¥éæ¬¡æ° current_retry = 0 error_count = 0 while
+current_retry < retry_count: try: # æå¼ç®æ ç½é¡µ await page.goto(f'https:
+//poe.com/{botname}') text = "This bot has been deleted for violating our"
+content = await page.content() if text in content: return "banned" #
+æ¾å°è¾å¥æ¡åç´  input_box = await page.wait_for_selector
+('.ChatMessageInputView_textInput__Aervw') # å°å­ç¬¦ä¸²åéå°è¾å¥æ¡ä¸­
+await input_box.fill(input_str) # æ¾å°åéæé®åç´ å¹¶ç¹å» await
+page.wait_for_selector('button.Button_primary__pIDjn') send_button = await
+page.wait_for_selector('button.Button_primary__pIDjn') # await asyncio.sleep
+(0.5) await send_button.click() # åéæååéåºå¾ªç¯ break except: #
 å¦æåºç°è¶æ¶å¼å¸¸ï¼æå°éè¯¯ä¿¡æ¯å¹¶ç¨ç­ä¸æ®µæ¶é´åéè¯
 error_count += 1 if error_count >= 1: await asyncio.sleep(retry_interval)
 current_retry += 1 continue if current_retry == retry_count: return False async
 def get_message_async(page,botname, sleep): consecutive_errors = 0 # initialize
 a counter for consecutive errors while True: await asyncio.sleep(sleep) try:
 await page.goto(f'https://poe.com/{botname}') response = await page.content()
 text = "This bot has been deleted for violating our" if text in response:
@@ -34,11 +31,11 @@
 consecutive_errors >= 10: return False else: consecutive_errors = 0 async def
 poe_chat(cookie_path,botname,question): async with async_playwright() as p:
 browser = await p.chromium.launch() context = await browser.new_context() page
 = await context.new_page() with open(cookie_path, 'r') as f: cookies =
 json.load(f) await context.add_cookies(cookies=cookies) is_banned = await
 send_message_async(page, botname, question) if is_banned == "banned": return
 "banned" result = await get_message_async(page, botname, sleep=5) if isinstance
-(result, tuple): answers, suggests = result return answers[-1],suggests elif
-isinstance(result, str): is_banned = result return "banned" elif isinstance
-(result, bool): is_got = result return is_got else: raise ValueError
-("Unexpected return type from get_message_async")
+(result, tuple): answers, suggests = result elif isinstance(result, str):
+is_banned = result return "banned" elif isinstance(result, bool): is_got =
+result else: raise ValueError("Unexpected return type from get_message_async")
+return answers[-1],suggests
```

### Comparing `nonebot_poe_chat-0.0.5/nonebot_poe_chat/poe_clear.py` & `nonebot_poe_chat-0.0.6/nonebot_poe_chat/poe_clear.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.5/nonebot_poe_chat/poe_create.py` & `nonebot_poe_chat-0.0.6/nonebot_poe_chat/poe_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
             # 定位输入框并清空原有的默认值
             name_input: ElementHandle = await page.wait_for_selector('input[name="name"]')
             await name_input.fill('')
 
             # 输入新的值
             await name_input.fill(botname)
 
-            base_select = await page.wait_for_selector('select[name="baseBot"]')
+            await page.wait_for_selector('select[name="baseBot"]')
             
             if base_bot_index == 1:
                 value = "chinchilla"
             elif base_bot_index ==2:
                 value = "a2"
             # 根据索引选择选项
             await page.select_option('.BotInfoForm_select__lFCl0', value=value)
```

### Comparing `nonebot_poe_chat-0.0.5/nonebot_poe_chat/poe_login.py` & `nonebot_poe_chat-0.0.6/nonebot_poe_chat/poe_login.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import asyncio
 import json
-from playwright.async_api import async_playwright
 async def submit_email(page,email):
     for i in range(5):
         try:
             await page.goto("https://poe.com")
             # 点击 "Use email" 按钮
             use_email_button = await page.query_selector('button:has-text("Use email")')
             await use_email_button.click()
```

### Comparing `nonebot_poe_chat-0.0.5/nonebot_poe_chat.egg-info/PKG-INFO` & `nonebot_poe_chat-0.0.6/nonebot_poe_chat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-poe-chat
-Version: 0.0.5
+Version: 0.0.6
 Summary: nonebot_poe_chat
 Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin
 Author-email: 1969730106@qq.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -43,20 +43,26 @@
 ~切换机器人:poeswitch / 切换bot / ps  
   
 ************************  
 --以下功能仅限poe管理员可以使用  
 ~登录:poelogin / plogin / pl  
 ~添加预设:poeaddprompt / 添加预设 / pap  
 ~删除预设:poeremoveprompt / 删除预设 / prp  
-  
-## pip安装并添加到pyproject.toml的plugins列表中  
+# 安装  
+## step.1  
+### nb安装  
+```
+nb plugin install nonebot-poe-chat
+```
+### 或者pip安装并添加到pyproject.toml的plugins列表中  
 ```
 pip install nonebot-poe-chat
 ```
-##然后  
+ 
+## step.2  
 ```
 playwright install chromuim
 ```
 ## 配置（在.env中修改）  
 
 ```
 #poe_cookie,poe网站的ck，见后文截图，也可以不填，而使用/pl命令登陆
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-poe-chat Version: 0.0.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-poe-chat Version: 0.0.6 Summary:
 nonebot_poe_chat Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin Author-email: 1969730106@qq.com Classifier: Programming Language
 :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE.txt
                               [nonebot_poe_chat]
@@ -20,17 +20,18 @@
 æºå¨äººçåç­ä¼ä»¥åå¤å½¢å¼åé --æä»¶å¨å­æ°æ®æ¾ç½®å¨./data/
 poe_chatä¸­ ## åè½ä½¿ç¨ --ä»¥ä¸å½ä»¤åé¢å¨é¨è¦å  / ~å¸®å©:poehelp
 / poeå¸®å© ~å¯¹è¯:poetalk / ptalk / pt ~æ¸ç©ºåå²å¯¹è¯:poedump / pdump /
 pd ~åå»ºæºå¨äºº:poecreate / åå»ºbot / pc ~å é¤æºå¨äºº:poeremove /
 å é¤bot / pr ~åæ¢æºå¨äºº:poeswitch / åæ¢bot / ps
 ************************ --ä»¥ä¸åè½ä»époeç®¡çåå¯ä»¥ä½¿ç¨ ~ç»å½:
 poelogin / plogin / pl ~æ·»å é¢è®¾:poeaddprompt / æ·»å é¢è®¾ / pap
-~å é¤é¢è®¾:poeremoveprompt / å é¤é¢è®¾ / prp ##
-pipå®è£å¹¶æ·»å å°pyproject.tomlçpluginsåè¡¨ä¸­ ``` pip install nonebot-
-poe-chat ``` ##ç¶å ``` playwright install chromuim ``` ##
+~å é¤é¢è®¾:poeremoveprompt / å é¤é¢è®¾ / prp # å®è£ ## step.1 ###
+nbå®è£ ``` nb plugin install nonebot-poe-chat ``` ###
+æèpipå®è£å¹¶æ·»å å°pyproject.tomlçpluginsåè¡¨ä¸­ ``` pip install
+nonebot-poe-chat ``` ## step.2 ``` playwright install chromuim ``` ##
 éç½®ï¼å¨.envä¸­ä¿®æ¹ï¼ ```
 #poe_cookie,poeç½ç«çckï¼è§åææªå¾ï¼ä¹å¯ä»¥ä¸å¡«ï¼èä½¿ç¨/
 plå½ä»¤ç»é poe_cookie = "f87HlVW~~%3D%3D"
 #poe_superusersï¼poeæä»¶ç®¡çåqqå· poe_superusers = ["123456","132145"]
 ``` ![ckè·å](https://github.com/canxin121/nonebot_poe_chat/blob/main/
 resource/ck.png) ## ç¤ºä¾ | Image 1 | Image 2 | |:-------:|:-------:| | ![]
 (https://github.com/canxin121/nonebot_poe_chat/blob/main/resource/demo%20
```

### Comparing `nonebot_poe_chat-0.0.5/setup.py` & `nonebot_poe_chat-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot_poe_chat",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.5",  # 程序版本
+    version="0.0.6",  # 程序版本
     author="canxin",  # 项目作者
     author_email="1969730106@qq.com",  # 作者邮件
     description="nonebot_poe_chat",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/canxin121/nonebot_poe_chat",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

