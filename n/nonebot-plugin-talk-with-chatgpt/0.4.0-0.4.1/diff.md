# Comparing `tmp/nonebot_plugin_talk_with_chatgpt-0.4.0.tar.gz` & `tmp/nonebot_plugin_talk_with_chatgpt-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.4.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.4.1.tar", max compression
```

## Comparing `nonebot_plugin_talk_with_chatgpt-0.4.0.tar` & `nonebot_plugin_talk_with_chatgpt-0.4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     8415 2023-04-21 09:12:17.992942 nonebot_plugin_talk_with_chatgpt-0.4.0/nonebot_plugin_talk_with_chatgpt/__init__.py
--rw-r--r--   0        0        0    13442 2023-04-21 07:36:53.217591 nonebot_plugin_talk_with_chatgpt-0.4.0/nonebot_plugin_talk_with_chatgpt/config.py
--rw-r--r--   0        0        0     5277 2023-04-21 09:07:58.978243 nonebot_plugin_talk_with_chatgpt-0.4.0/nonebot_plugin_talk_with_chatgpt/data_handle.py
--rw-r--r--   0        0        0      974 2023-04-21 09:15:54.048004 nonebot_plugin_talk_with_chatgpt-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4671 2023-04-21 09:16:02.318546 nonebot_plugin_talk_with_chatgpt-0.4.0/README.md
--rw-r--r--   0        0        0     5610 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     8454 2023-04-22 14:28:18.532815 nonebot_plugin_talk_with_chatgpt-0.4.1/nonebot_plugin_talk_with_chatgpt/__init__.py
+-rw-r--r--   0        0        0    13518 2023-04-22 14:27:21.436142 nonebot_plugin_talk_with_chatgpt-0.4.1/nonebot_plugin_talk_with_chatgpt/config.py
+-rw-r--r--   0        0        0     5277 2023-04-21 09:07:58.978243 nonebot_plugin_talk_with_chatgpt-0.4.1/nonebot_plugin_talk_with_chatgpt/data_handle.py
+-rw-r--r--   0        0        0      974 2023-04-22 14:28:28.184174 nonebot_plugin_talk_with_chatgpt-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4834 2023-04-22 14:30:17.504552 nonebot_plugin_talk_with_chatgpt-0.4.1/README.md
+-rw-r--r--   0        0        0     5767 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.4.1/PKG-INFO
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.0/nonebot_plugin_talk_with_chatgpt/__init__.py` & `nonebot_plugin_talk_with_chatgpt-0.4.1/nonebot_plugin_talk_with_chatgpt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 reset_cmd = pc.talk_with_chatgpt_reset_cmd
 prompt_cmd = pc.talk_with_chatgpt_prompt_cmd
 
 __plugin_meta__ = PluginMetadata(
     name="talk with chatgpt",
     description="一个简单的基于accessToken验证的ChatGPT对话插件",
     usage=f"""插件命令如下
-{talk_cmd}  # 开始对话，群里@机器人也可以
+{talk_cmd}  # 开始对话，默认群里@机器人也可以
 {reset_cmd}  # 重置对话（不会重置预设）
 {prompt_cmd}  # 设置预设（人格），设置后会重置对话
 """,
 )
 
 
 def get_id(event: MessageEvent) -> str:
@@ -52,15 +52,15 @@
     if bot != var.handle_bot:
         return False
     # 获取纯文本
     text = event.get_plaintext().strip()
 
     if isinstance(event, GroupMessageEvent):
         # 仅艾特但没发内容
-        if event.is_tome():
+        if event.is_tome() and pc.talk_with_chatgpt_talk_at:
             if text:
                 return True
             else:
                 return False
 
         return text[: len(talk_cmd)] == talk_cmd
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.0/nonebot_plugin_talk_with_chatgpt/config.py` & `nonebot_plugin_talk_with_chatgpt-0.4.1/nonebot_plugin_talk_with_chatgpt/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     # 群聊是否共享会话
     talk_with_chatgpt_group_share: bool = False
     # 只允许超级管理员修改预设
     talk_with_chatgpt_prompt_admin_only: bool = True
 
     # 触发对话的命令前缀，群聊直接艾特也可以触发
     talk_with_chatgpt_talk_cmd: str = "/talk"
+    # 群聊艾特是否响应
+    talk_with_chatgpt_talk_at: bool = True
     # 私聊沉浸式对话触发命令
     talk_with_chatgpt_talk_p_cmd: str = "/hi"
     # 重置对话，就是清空聊天记录
     talk_with_chatgpt_reset_cmd: str = "/reset"
     # 设置预设
     talk_with_chatgpt_prompt_cmd: str = "/prompt"
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.0/nonebot_plugin_talk_with_chatgpt/data_handle.py` & `nonebot_plugin_talk_with_chatgpt-0.4.1/nonebot_plugin_talk_with_chatgpt/data_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.0/pyproject.toml` & `nonebot_plugin_talk_with_chatgpt-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_talk_with_chatgpt"
-version = "0.4.0"
+version = "0.4.1"
 description = "Nonebot2 基于accessToken登录的ChatGPT聊天插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_talk_with_chatgpt"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.0/README.md` & `nonebot_plugin_talk_with_chatgpt-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   <a href="https://v2.nonebot.dev/">
     <img src="https://img.shields.io/static/v1?label=nonebot&message=v2rc1%2B&color=green" alt="nonebot2">
   </a>
   <img src="https://img.shields.io/static/v1?label=python+&message=3.8%2B&color=blue" alt="python">
 </p>
 
 # 注意！
-由于现在社区反代API用的人太多，稳定性可能不咋地，最好就自建一个，目前内置的是[https://ai.fakeopen.com/api/conversation](https://ai.fakeopen.com/api/conversation) ，截止2023/4/21是能用的。
+由于现在社区反代API用的人太多，稳定性可能不咋地，最好就自建一个，目前内置的是[https://ai.fakeopen.com/api/conversation](https://ai.fakeopen.com/api/conversation) ，截止2023/4/22是能用的，而且不需要设置代理。
 [自建反代API搭建教程](https://github.com/dqzboy/ChatGPT-Porxy)
 
 ## 简介
 发现商店里没有基于accessToken登录的chatgpt插件，也没看到喜欢的插件，就花一天时间自己写了一个。参考了[chatgpt web](https://github.com/Chanzhaoyu/chatgpt-web)这个开源项目，使用了社区上的反代，如果要使用其他反代可以参考这个项目里的。  
 <img width="100%" src="https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/nonebot_plugin_talk_with_chatgpt/readme_img/1.jpg"/>  
 
 插件功能相对其他的来说比较简单，因此也比较易用，获取accessToken并配置代理即可使用，[accessToken获取方式](https://chat.openai.com/api/auth/session)，accessToken字段的值就是了。如果有其他想法或建议欢迎提出，欢迎pr。
@@ -62,16 +62,18 @@
 talk_with_chatgpt_group_share = false
 # 只允许超级管理员修改预设
 talk_with_chatgpt_prompt_admin_only = true
 ```
 
 #### 如果要修改触发命令就填
 ```bash
-# 触发对话的命令前缀，群聊直接艾特也可以触发
+# 触发对话的命令前缀，默认群聊直接艾特也可以触发
 talk_with_chatgpt_start_cmd = /talk
+# 群聊艾特是否响应
+talk_with_chatgpt_talk_at = true
 # 私聊沉浸式对话触发命令
 talk_with_chatgpt_talk_p_cmd = /hi
 # 重置对话的命令，就是清空聊天记录
 talk_with_chatgpt_reset_cmd = /reset
 # 设置预设的命令前缀
 talk_with_chatgpt_prompt_cmd = /prompt
 ```
@@ -90,20 +92,24 @@
 # 插件数据文件名，默认./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json
 ```
 
 ## 插件命令（均可修改！） 
 | 指令 | 说明 |
 |:-----:|:----:|
-| /talk | 开始对话，群里@机器人也可以 |
+| /talk | 开始对话，默认群里@机器人也可以 |
 | /hi | 沉浸式对话（仅限私聊） |
 | /clear | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
+### 2023/4/22 \[v0.4.1]
+
+* 增加群聊at触发开关
+
 ### 2023/4/21 \[v0.4.0]
 
 * 更换了默认API，暂时能用，建议还是自己搭建API
 * 新增多预设功能，内置三个预设：猫娘、魅魔、开发者模式
 * 增加私聊沉浸式对话
 * 优化大量细节
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
                               [NoneBotPluginLogo]
                # nonebot_plugin_talk_with_chatgpt _â¨ Nonebot2
                     ä¸ä¸ªç®åæç¨çchatgptæä»¶ â¨_
                          [license] [nonebot2] [python]
 # æ³¨æï¼
 ç±äºç°å¨ç¤¾åºåä»£APIç¨çäººå¤ªå¤ï¼ç¨³å®æ§å¯è½ä¸åå°ï¼æå¥½å°±èªå»ºä¸ä¸ªï¼ç®ååç½®çæ¯
 [https://ai.fakeopen.com/api/conversation](https://ai.fakeopen.com/api/
-conversation) ï¼æªæ­¢2023/4/21æ¯è½ç¨çã [èªå»ºåä»£APIæ­å»ºæç¨]
-(https://github.com/dqzboy/ChatGPT-Porxy) ## ç®ä»
+conversation) ï¼æªæ­¢2023/4/22æ¯è½ç¨çï¼èä¸ä¸éè¦è®¾ç½®ä»£çã
+[èªå»ºåä»£APIæ­å»ºæç¨](https://github.com/dqzboy/ChatGPT-Porxy) ##
+ç®ä»
 åç°ååºéæ²¡æåºäºaccessTokenç»å½çchatgptæä»¶ï¼ä¹æ²¡çå°åæ¬¢çæä»¶ï¼å°±è±ä¸å¤©æ¶é´èªå·±åäºä¸ä¸ªãåèäº
 [chatgpt web](https://github.com/Chanzhaoyu/chatgpt-
 web)è¿ä¸ªå¼æºé¡¹ç®ï¼ä½¿ç¨äºç¤¾åºä¸çåä»£ï¼å¦æè¦ä½¿ç¨å¶ä»åä»£å¯ä»¥åèè¿ä¸ªé¡¹ç®éçã
 [https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/
 nonebot_plugin_talk_with_chatgpt/readme_img/1.jpg]
 æä»¶åè½ç¸å¯¹å¶ä»çæ¥è¯´æ¯è¾ç®åï¼å æ­¤ä¹æ¯è¾æç¨ï¼è·åaccessTokenå¹¶éç½®ä»£çå³å¯ä½¿ç¨ï¼
 [accessTokenè·åæ¹å¼](https://chat.openai.com/api/auth/
@@ -26,16 +27,17 @@
 ai.fakeopen.com/api/conversation #
 é»è®¤æ ä»£çï¼è§apiæåµçæ¯å¦éè¦æ¢¯å­ãè¿ä¸ªåç½®çåä»£ææµè¿æ¯ä¸éè¦æ¢¯å­çã
 talk_with_chatgpt_http_proxy = null # å¤çæ¶æ¯æ¶æ¯å¦æç¤º
 talk_with_chatgpt_reply_notice = true # ç¾¤èæ¯å¦å±äº«ä¼è¯
 talk_with_chatgpt_group_share = false # åªåè®¸è¶çº§ç®¡çåä¿®æ¹é¢è®¾
 talk_with_chatgpt_prompt_admin_only = true ``` ####
 å¦æè¦ä¿®æ¹è§¦åå½ä»¤å°±å¡« ```bash #
-è§¦åå¯¹è¯çå½ä»¤åç¼ï¼ç¾¤èç´æ¥è¾ç¹ä¹å¯ä»¥è§¦å
-talk_with_chatgpt_start_cmd = /talk # ç§èæ²æµ¸å¼å¯¹è¯è§¦åå½ä»¤
+è§¦åå¯¹è¯çå½ä»¤åç¼ï¼é»è®¤ç¾¤èç´æ¥è¾ç¹ä¹å¯ä»¥è§¦å
+talk_with_chatgpt_start_cmd = /talk # ç¾¤èè¾ç¹æ¯å¦ååº
+talk_with_chatgpt_talk_at = true # ç§èæ²æµ¸å¼å¯¹è¯è§¦åå½ä»¤
 talk_with_chatgpt_talk_p_cmd = /hi #
 éç½®å¯¹è¯çå½ä»¤ï¼å°±æ¯æ¸ç©ºèå¤©è®°å½ talk_with_chatgpt_reset_cmd =
 /reset # è®¾ç½®é¢è®¾çå½ä»¤åç¼ talk_with_chatgpt_prompt_cmd = /prompt ```
 #### å¤§æ¦çç¨ä¸ä¸çéå¡«é¡¹ ```bash #
 è¯·æ±è¶æ¶æ¶é´ï¼åç­çæçæ¶é´ä¹è¦ç®å¨è¿éé¢çï¼æä»¥ä¸è½å¤ªç­ï¼é»è®¤60ç§
 talk_with_chatgpt_timeout = 60 # chatgptæ¨¡åï¼é»è®¤ text-davinci-002-
 render-shaï¼æ´å¤æ¨¡åè¯·åè https://platform.openai.com/docs/models
@@ -44,16 +46,16 @@
 å¦ææå¤ä¸ªbotè¿æ¥ï¼ä¼æç§å¡«åçlistï¼å·¦è¾¹çæºå¨äººQQä¼åçº§æé«
 1234 > 5678 > 6666ï¼ä¼èªå¨åæ¢ #
 å¦æä¸å¡«è¯¥éç½®åç±ç¬¬ä¸ä¸ªè¿ä¸çbotååºï¼æä»¥åbotè¿å¯ä»¥ä¸å¡«
 talk_with_chatgpt_bot_qqnum_list = [1234, 5678, 6666] #
 æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
-| å¼å§å¯¹è¯ï¼ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
+| å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /clear |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-4/21 \[v0.4.0] *
+4/22 \[v0.4.1] * å¢å ç¾¤èatè§¦åå¼å³ ### 2023/4/21 \[v0.4.0] *
 æ´æ¢äºé»è®¤APIï¼ææ¶è½ç¨ï¼å»ºè®®è¿æ¯èªå·±æ­å»ºAPI *
 æ°å¢å¤é¢è®¾åè½ï¼åç½®ä¸ä¸ªé¢è®¾ï¼ç«å¨ãé­é­ãå¼åèæ¨¡å¼
 * å¢å ç§èæ²æµ¸å¼å¯¹è¯ * ä¼åå¤§éç»è ### 2023/4/11 \[v0.2.3] *
 åå¸ç¬¬ä¸çè¾ç®éçæä»¶ï¼å¹¶ä¿®å¤äºäºå°é®é¢ï¼ç»èå¾éè¦
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.0/PKG-INFO` & `nonebot_plugin_talk_with_chatgpt-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-talk-with-chatgpt
-Version: 0.4.0
+Version: 0.4.1
 Summary: Nonebot2 基于accessToken登录的ChatGPT聊天插件
 Home-page: https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt
 License: MIT
 Author: nikissXI
 Author-email: 1299577815@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -40,15 +40,15 @@
   <a href="https://v2.nonebot.dev/">
     <img src="https://img.shields.io/static/v1?label=nonebot&message=v2rc1%2B&color=green" alt="nonebot2">
   </a>
   <img src="https://img.shields.io/static/v1?label=python+&message=3.8%2B&color=blue" alt="python">
 </p>
 
 # 注意！
-由于现在社区反代API用的人太多，稳定性可能不咋地，最好就自建一个，目前内置的是[https://ai.fakeopen.com/api/conversation](https://ai.fakeopen.com/api/conversation) ，截止2023/4/21是能用的。
+由于现在社区反代API用的人太多，稳定性可能不咋地，最好就自建一个，目前内置的是[https://ai.fakeopen.com/api/conversation](https://ai.fakeopen.com/api/conversation) ，截止2023/4/22是能用的，而且不需要设置代理。
 [自建反代API搭建教程](https://github.com/dqzboy/ChatGPT-Porxy)
 
 ## 简介
 发现商店里没有基于accessToken登录的chatgpt插件，也没看到喜欢的插件，就花一天时间自己写了一个。参考了[chatgpt web](https://github.com/Chanzhaoyu/chatgpt-web)这个开源项目，使用了社区上的反代，如果要使用其他反代可以参考这个项目里的。  
 <img width="100%" src="https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/nonebot_plugin_talk_with_chatgpt/readme_img/1.jpg"/>  
 
 插件功能相对其他的来说比较简单，因此也比较易用，获取accessToken并配置代理即可使用，[accessToken获取方式](https://chat.openai.com/api/auth/session)，accessToken字段的值就是了。如果有其他想法或建议欢迎提出，欢迎pr。
@@ -85,16 +85,18 @@
 talk_with_chatgpt_group_share = false
 # 只允许超级管理员修改预设
 talk_with_chatgpt_prompt_admin_only = true
 ```
 
 #### 如果要修改触发命令就填
 ```bash
-# 触发对话的命令前缀，群聊直接艾特也可以触发
+# 触发对话的命令前缀，默认群聊直接艾特也可以触发
 talk_with_chatgpt_start_cmd = /talk
+# 群聊艾特是否响应
+talk_with_chatgpt_talk_at = true
 # 私聊沉浸式对话触发命令
 talk_with_chatgpt_talk_p_cmd = /hi
 # 重置对话的命令，就是清空聊天记录
 talk_with_chatgpt_reset_cmd = /reset
 # 设置预设的命令前缀
 talk_with_chatgpt_prompt_cmd = /prompt
 ```
@@ -113,20 +115,24 @@
 # 插件数据文件名，默认./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json
 ```
 
 ## 插件命令（均可修改！） 
 | 指令 | 说明 |
 |:-----:|:----:|
-| /talk | 开始对话，群里@机器人也可以 |
+| /talk | 开始对话，默认群里@机器人也可以 |
 | /hi | 沉浸式对话（仅限私聊） |
 | /clear | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
+### 2023/4/22 \[v0.4.1]
+
+* 增加群聊at触发开关
+
 ### 2023/4/21 \[v0.4.0]
 
 * 更换了默认API，暂时能用，建议还是自己搭建API
 * 新增多预设功能，内置三个预设：猫娘、魅魔、开发者模式
 * 增加私聊沉浸式对话
 * 优化大量细节
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.4.0
+Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.4.1
 Summary: Nonebot2 åºäºaccessTokenç»å½çChatGPTèå¤©æä»¶ Home-page:
 https://github.com/nikissXI/nonebot_plugins/tree/main/
 nonebot_plugin_talk_with_chatgpt License: MIT Author: nikissXI Author-email:
 1299577815@qq.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -16,16 +16,17 @@
                               [NoneBotPluginLogo]
                # nonebot_plugin_talk_with_chatgpt _â¨ Nonebot2
                     ä¸ä¸ªç®åæç¨çchatgptæä»¶ â¨_
                          [license] [nonebot2] [python]
 # æ³¨æï¼
 ç±äºç°å¨ç¤¾åºåä»£APIç¨çäººå¤ªå¤ï¼ç¨³å®æ§å¯è½ä¸åå°ï¼æå¥½å°±èªå»ºä¸ä¸ªï¼ç®ååç½®çæ¯
 [https://ai.fakeopen.com/api/conversation](https://ai.fakeopen.com/api/
-conversation) ï¼æªæ­¢2023/4/21æ¯è½ç¨çã [èªå»ºåä»£APIæ­å»ºæç¨]
-(https://github.com/dqzboy/ChatGPT-Porxy) ## ç®ä»
+conversation) ï¼æªæ­¢2023/4/22æ¯è½ç¨çï¼èä¸ä¸éè¦è®¾ç½®ä»£çã
+[èªå»ºåä»£APIæ­å»ºæç¨](https://github.com/dqzboy/ChatGPT-Porxy) ##
+ç®ä»
 åç°ååºéæ²¡æåºäºaccessTokenç»å½çchatgptæä»¶ï¼ä¹æ²¡çå°åæ¬¢çæä»¶ï¼å°±è±ä¸å¤©æ¶é´èªå·±åäºä¸ä¸ªãåèäº
 [chatgpt web](https://github.com/Chanzhaoyu/chatgpt-
 web)è¿ä¸ªå¼æºé¡¹ç®ï¼ä½¿ç¨äºç¤¾åºä¸çåä»£ï¼å¦æè¦ä½¿ç¨å¶ä»åä»£å¯ä»¥åèè¿ä¸ªé¡¹ç®éçã
 [https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/
 nonebot_plugin_talk_with_chatgpt/readme_img/1.jpg]
 æä»¶åè½ç¸å¯¹å¶ä»çæ¥è¯´æ¯è¾ç®åï¼å æ­¤ä¹æ¯è¾æç¨ï¼è·åaccessTokenå¹¶éç½®ä»£çå³å¯ä½¿ç¨ï¼
 [accessTokenè·åæ¹å¼](https://chat.openai.com/api/auth/
@@ -41,16 +42,17 @@
 ai.fakeopen.com/api/conversation #
 é»è®¤æ ä»£çï¼è§apiæåµçæ¯å¦éè¦æ¢¯å­ãè¿ä¸ªåç½®çåä»£ææµè¿æ¯ä¸éè¦æ¢¯å­çã
 talk_with_chatgpt_http_proxy = null # å¤çæ¶æ¯æ¶æ¯å¦æç¤º
 talk_with_chatgpt_reply_notice = true # ç¾¤èæ¯å¦å±äº«ä¼è¯
 talk_with_chatgpt_group_share = false # åªåè®¸è¶çº§ç®¡çåä¿®æ¹é¢è®¾
 talk_with_chatgpt_prompt_admin_only = true ``` ####
 å¦æè¦ä¿®æ¹è§¦åå½ä»¤å°±å¡« ```bash #
-è§¦åå¯¹è¯çå½ä»¤åç¼ï¼ç¾¤èç´æ¥è¾ç¹ä¹å¯ä»¥è§¦å
-talk_with_chatgpt_start_cmd = /talk # ç§èæ²æµ¸å¼å¯¹è¯è§¦åå½ä»¤
+è§¦åå¯¹è¯çå½ä»¤åç¼ï¼é»è®¤ç¾¤èç´æ¥è¾ç¹ä¹å¯ä»¥è§¦å
+talk_with_chatgpt_start_cmd = /talk # ç¾¤èè¾ç¹æ¯å¦ååº
+talk_with_chatgpt_talk_at = true # ç§èæ²æµ¸å¼å¯¹è¯è§¦åå½ä»¤
 talk_with_chatgpt_talk_p_cmd = /hi #
 éç½®å¯¹è¯çå½ä»¤ï¼å°±æ¯æ¸ç©ºèå¤©è®°å½ talk_with_chatgpt_reset_cmd =
 /reset # è®¾ç½®é¢è®¾çå½ä»¤åç¼ talk_with_chatgpt_prompt_cmd = /prompt ```
 #### å¤§æ¦çç¨ä¸ä¸çéå¡«é¡¹ ```bash #
 è¯·æ±è¶æ¶æ¶é´ï¼åç­çæçæ¶é´ä¹è¦ç®å¨è¿éé¢çï¼æä»¥ä¸è½å¤ªç­ï¼é»è®¤60ç§
 talk_with_chatgpt_timeout = 60 # chatgptæ¨¡åï¼é»è®¤ text-davinci-002-
 render-shaï¼æ´å¤æ¨¡åè¯·åè https://platform.openai.com/docs/models
@@ -59,16 +61,16 @@
 å¦ææå¤ä¸ªbotè¿æ¥ï¼ä¼æç§å¡«åçlistï¼å·¦è¾¹çæºå¨äººQQä¼åçº§æé«
 1234 > 5678 > 6666ï¼ä¼èªå¨åæ¢ #
 å¦æä¸å¡«è¯¥éç½®åç±ç¬¬ä¸ä¸ªè¿ä¸çbotååºï¼æä»¥åbotè¿å¯ä»¥ä¸å¡«
 talk_with_chatgpt_bot_qqnum_list = [1234, 5678, 6666] #
 æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
-| å¼å§å¯¹è¯ï¼ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
+| å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /clear |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-4/21 \[v0.4.0] *
+4/22 \[v0.4.1] * å¢å ç¾¤èatè§¦åå¼å³ ### 2023/4/21 \[v0.4.0] *
 æ´æ¢äºé»è®¤APIï¼ææ¶è½ç¨ï¼å»ºè®®è¿æ¯èªå·±æ­å»ºAPI *
 æ°å¢å¤é¢è®¾åè½ï¼åç½®ä¸ä¸ªé¢è®¾ï¼ç«å¨ãé­é­ãå¼åèæ¨¡å¼
 * å¢å ç§èæ²æµ¸å¼å¯¹è¯ * ä¼åå¤§éç»è ### 2023/4/11 \[v0.2.3] *
 åå¸ç¬¬ä¸çè¾ç®éçæä»¶ï¼å¹¶ä¿®å¤äºäºå°é®é¢ï¼ç»èå¾éè¦
```

