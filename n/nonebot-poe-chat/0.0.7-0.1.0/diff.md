# Comparing `tmp/nonebot_poe_chat-0.0.7.tar.gz` & `tmp/nonebot_poe_chat-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_poe_chat-0.0.7.tar", last modified: Sat Apr 22 14:47:40 2023, max compression
+gzip compressed data, was "nonebot_poe_chat-0.1.0.tar", last modified: Sat Apr 22 14:50:33 2023, max compression
```

## Comparing `nonebot_poe_chat-0.0.7.tar` & `nonebot_poe_chat-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 14:47:40.298983 nonebot_poe_chat-0.0.7/
--rw-rw-rw-   0        0        0    12533 2023-04-02 14:35:33.000000 nonebot_poe_chat-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0     3044 2023-04-22 14:47:40.297994 nonebot_poe_chat-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2549 2023-04-22 14:39:54.000000 nonebot_poe_chat-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 14:47:40.290983 nonebot_poe_chat-0.0.7/nonebot_poe_chat/
--rw-rw-rw-   0        0        0    23252 2023-04-22 14:46:14.000000 nonebot_poe_chat-0.0.7/nonebot_poe_chat/__init__.py
--rw-rw-rw-   0        0        0     3026 2023-04-21 14:27:42.000000 nonebot_poe_chat-0.0.7/nonebot_poe_chat/config.py
--rw-rw-rw-   0        0        0     4112 2023-04-22 14:35:57.000000 nonebot_poe_chat-0.0.7/nonebot_poe_chat/poe_chat.py
--rw-rw-rw-   0        0        0     1440 2023-04-21 14:27:42.000000 nonebot_poe_chat-0.0.7/nonebot_poe_chat/poe_clear.py
--rw-rw-rw-   0        0        0     2884 2023-04-21 14:53:32.000000 nonebot_poe_chat-0.0.7/nonebot_poe_chat/poe_create.py
--rw-rw-rw-   0        0        0     1261 2023-04-22 14:26:17.000000 nonebot_poe_chat-0.0.7/nonebot_poe_chat/poe_func.py
--rw-rw-rw-   0        0        0     2394 2023-04-22 14:36:31.000000 nonebot_poe_chat-0.0.7/nonebot_poe_chat/poe_login.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:47:40.296992 nonebot_poe_chat-0.0.7/nonebot_poe_chat.egg-info/
--rw-rw-rw-   0        0        0     3044 2023-04-22 14:47:40.000000 nonebot_poe_chat-0.0.7/nonebot_poe_chat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-04-22 14:47:40.000000 nonebot_poe_chat-0.0.7/nonebot_poe_chat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 14:47:40.000000 nonebot_poe_chat-0.0.7/nonebot_poe_chat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-22 14:47:40.000000 nonebot_poe_chat-0.0.7/nonebot_poe_chat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-22 14:47:40.000000 nonebot_poe_chat-0.0.7/nonebot_poe_chat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 14:47:40.298983 nonebot_poe_chat-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1155 2023-04-22 14:46:22.000000 nonebot_poe_chat-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:50:33.908421 nonebot_poe_chat-0.1.0/
+-rw-rw-rw-   0        0        0    12533 2023-04-02 14:35:33.000000 nonebot_poe_chat-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3044 2023-04-22 14:50:33.907420 nonebot_poe_chat-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2549 2023-04-22 14:39:54.000000 nonebot_poe_chat-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 14:50:33.901421 nonebot_poe_chat-0.1.0/nonebot_poe_chat/
+-rw-rw-rw-   0        0        0    23252 2023-04-22 14:49:51.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat/__init__.py
+-rw-rw-rw-   0        0        0     3026 2023-04-21 14:27:42.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat/config.py
+-rw-rw-rw-   0        0        0     4112 2023-04-22 14:35:57.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_chat.py
+-rw-rw-rw-   0        0        0     1440 2023-04-21 14:27:42.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_clear.py
+-rw-rw-rw-   0        0        0     2884 2023-04-21 14:53:32.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_create.py
+-rw-rw-rw-   0        0        0     1261 2023-04-22 14:26:17.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_func.py
+-rw-rw-rw-   0        0        0     2394 2023-04-22 14:36:31.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_login.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:50:33.906421 nonebot_poe_chat-0.1.0/nonebot_poe_chat.egg-info/
+-rw-rw-rw-   0        0        0     3044 2023-04-22 14:50:33.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-04-22 14:50:33.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 14:50:33.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-04-22 14:50:33.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-22 14:50:33.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 14:50:33.908421 nonebot_poe_chat-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1155 2023-04-22 14:50:16.000000 nonebot_poe_chat-0.1.0/setup.py
```

### Comparing `nonebot_poe_chat-0.0.7/LICENSE.txt` & `nonebot_poe_chat-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.7/PKG-INFO` & `nonebot_poe_chat-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_poe_chat
-Version: 0.0.7
+Version: 0.1.0
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
-Metadata-Version: 2.1 Name: nonebot_poe_chat Version: 0.0.7 Summary:
+Metadata-Version: 2.1 Name: nonebot_poe_chat Version: 0.1.0 Summary:
 nonebot_poe_chat Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin Author-email: 1969730106@qq.com Classifier: Programming Language
 :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE.txt
                               [nonebot_poe_chat]
```

### Comparing `nonebot_poe_chat-0.0.7/README.md` & `nonebot_poe_chat-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.7/nonebot_poe_chat/__init__.py` & `nonebot_poe_chat-0.1.0/nonebot_poe_chat/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -534,10 +534,10 @@
     "--以下功能仅限poe管理员使用\n"
     "~登录:poelogin / plogin / pl\n"
     "~添加预设:poeaddprompt / 添加预设 / pap\n"
     "~删除预设:poeremoveprompt / 删除预设 / prp"
     )
     
     helpmsg = await poe_help.send(msg)
-    await bot.delete_msg(message_id=helpmsg['message_id'])
     await asyncio.sleep(30)
+    await bot.delete_msg(message_id=helpmsg['message_id'])
     await poe_help.finish()
```

### Comparing `nonebot_poe_chat-0.0.7/nonebot_poe_chat/config.py` & `nonebot_poe_chat-0.1.0/nonebot_poe_chat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.7/nonebot_poe_chat/poe_chat.py` & `nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_chat.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.7/nonebot_poe_chat/poe_clear.py` & `nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_clear.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.7/nonebot_poe_chat/poe_create.py` & `nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_create.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.7/nonebot_poe_chat/poe_func.py` & `nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.7/nonebot_poe_chat/poe_login.py` & `nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_login.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.7/nonebot_poe_chat.egg-info/PKG-INFO` & `nonebot_poe_chat-0.1.0/nonebot_poe_chat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-poe-chat
-Version: 0.0.7
+Version: 0.1.0
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
-Metadata-Version: 2.1 Name: nonebot-poe-chat Version: 0.0.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-poe-chat Version: 0.1.0 Summary:
 nonebot_poe_chat Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin Author-email: 1969730106@qq.com Classifier: Programming Language
 :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE.txt
                               [nonebot_poe_chat]
```

### Comparing `nonebot_poe_chat-0.0.7/setup.py` & `nonebot_poe_chat-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot_poe_chat",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.7",  # 程序版本
+    version="0.1.0",  # 程序版本
     author="canxin",  # 项目作者
     author_email="1969730106@qq.com",  # 作者邮件
     description="nonebot_poe_chat",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/canxin121/nonebot_poe_chat",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

