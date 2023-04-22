# Comparing `tmp/nonebot_plugin_ping-1.6.5.tar.gz` & `tmp/nonebot_plugin_ping-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ping-1.6.5.tar", last modified: Fri Apr 21 00:56:32 2023, max compression
+gzip compressed data, was "nonebot_plugin_ping-1.6.6.tar", last modified: Sat Apr 22 03:20:28 2023, max compression
```

## Comparing `nonebot_plugin_ping-1.6.5.tar` & `nonebot_plugin_ping-1.6.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 00:56:32.357589 nonebot_plugin_ping-1.6.5/
--rw-rw-rw-   0        0        0     1088 2023-02-03 08:23:04.000000 nonebot_plugin_ping-1.6.5/LICENSE
--rw-rw-rw-   0        0        0     1659 2023-04-21 00:56:32.357589 nonebot_plugin_ping-1.6.5/PKG-INFO
--rw-rw-rw-   0        0        0      961 2023-02-03 08:23:04.000000 nonebot_plugin_ping-1.6.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 00:56:32.350281 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping/
--rw-rw-rw-   0        0        0     3674 2023-04-21 00:55:53.000000 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 00:56:32.354335 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping.egg-info/
--rw-rw-rw-   0        0        0     1659 2023-04-21 00:56:32.000000 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-04-21 00:56:32.000000 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 00:56:32.000000 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-21 00:56:32.000000 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-21 00:56:32.000000 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 00:56:32.357589 nonebot_plugin_ping-1.6.5/setup.cfg
--rw-rw-rw-   0        0        0     3944 2023-04-21 00:56:03.000000 nonebot_plugin_ping-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 03:20:28.530537 nonebot_plugin_ping-1.6.6/
+-rw-rw-rw-   0        0        0     1088 2023-02-03 08:23:04.000000 nonebot_plugin_ping-1.6.6/LICENSE
+-rw-rw-rw-   0        0        0     1659 2023-04-22 03:20:28.530537 nonebot_plugin_ping-1.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2023-02-03 08:23:04.000000 nonebot_plugin_ping-1.6.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 03:20:28.524021 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping/
+-rw-rw-rw-   0        0        0     3837 2023-04-22 03:18:23.000000 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 03:20:28.529137 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping.egg-info/
+-rw-rw-rw-   0        0        0     1659 2023-04-22 03:20:28.000000 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-04-22 03:20:28.000000 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 03:20:28.000000 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-22 03:20:28.000000 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-22 03:20:28.000000 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 03:20:28.530537 nonebot_plugin_ping-1.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     3944 2023-04-22 03:19:33.000000 nonebot_plugin_ping-1.6.6/setup.py
```

### Comparing `nonebot_plugin_ping-1.6.5/LICENSE` & `nonebot_plugin_ping-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ping-1.6.5/PKG-INFO` & `nonebot_plugin_ping-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_ping
-Version: 1.6.5
+Version: 1.6.6
 Summary: ping
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_ping-1.6.5/README.md` & `nonebot_plugin_ping-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ping-1.6.5/nonebot_plugin_ping/__init__.py` & `nonebot_plugin_ping-1.6.6/nonebot_plugin_ping/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,34 +16,39 @@
 """PING网址"""
 ping = on_command('ping', aliases={'Ping'}, priority=60, block=True)
 @ping.handle()
 async def _(msg: Message = CommandArg()):
     url = msg.extract_plain_text().strip()
 
     if model == 1:
-        api = f'https://v.api.aa1.cn/api/api-ping/ping.php?url={url}'
+        api = f'https://xiaoapi.cn/API/sping.php?url={url}'
         message = await api_ping(api)
     elif model == 2:
         message = await cmd_ping(url)
     else:
         message = "PING 配置项填写有误, 联系 SUPPERUSER 检查!"
 
     await ping.finish(message)
 
 
 async def api_ping(api):
     async with AsyncClient() as client:
-        res = (await client.get(api)).json()
+        # res = (await client.get(api)).json()
+        # try:
+        #     url = (res["host"])
+        #     ip = (res["ip"])
+        #     max = (res["ping_time_max"])
+        #     min = (res["ping_time_min"])
+        #     place = (res["location"])
+        #     res = f"域名: {url}\nIP: {ip}\n最大延迟: {max}\n最小延迟: {min}\n服务器归属地: {place}"
+        #     return res
+        # except Exception:
+        #     return "寄"
         try:
-            url = (res["host"])
-            ip = (res["ip"])
-            max = (res["ping_time_max"])
-            min = (res["ping_time_min"])
-            place = (res["location"])
-            res = f"域名: {url}\nIP: {ip}\n最大延迟: {max}\n最小延迟: {min}\n服务器归属地: {place}"
+            res = (await client.get(api, timeout=10)).text
             return res
         except Exception:
             return "寄"
 
 async def cmd_ping(url):
     # 获取系统信息, Windows 请求默认 4 次, Linux 请求默认不会停止.
     sys = platform.system()
```

### Comparing `nonebot_plugin_ping-1.6.5/nonebot_plugin_ping.egg-info/PKG-INFO` & `nonebot_plugin_ping-1.6.6/nonebot_plugin_ping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ping
-Version: 1.6.5
+Version: 1.6.6
 Summary: ping
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_ping-1.6.5/setup.py` & `nonebot_plugin_ping-1.6.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'nonebot_plugin_ping'
 DESCRIPTION = 'ping'
 URL = 'https://github.com/zhulinyv/nonebot_plugin_ping'
 EMAIL = 'zhulinyv2005@outlook.com'
 AUTHOR = '(๑•小丫头片子•๑)'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.6.5'
+VERSION = '1.6.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'nonebot2', 'nonebot-adapter-onebot', 'httpx',
 ]
 
 # What packages are optional?
```

