# Comparing `tmp/amino.api-1.0b2.tar.gz` & `tmp/amino.api-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.api-1.0b2.tar", last modified: Thu Apr 20 21:06:36 2023, max compression
+gzip compressed data, was "amino.api-1.1.tar", last modified: Fri Apr 21 11:19:33 2023, max compression
```

## Comparing `amino.api-1.0b2.tar` & `amino.api-1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 21:06:36.853437 amino.api-1.0b2/
--rw-rw-rw-   0        0        0      558 2023-04-20 21:06:36.853437 amino.api-1.0b2/PKG-INFO
--rw-rw-rw-   0        0        0       40 2023-04-18 11:48:20.000000 amino.api-1.0b2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 21:06:36.800821 amino.api-1.0b2/amino/
--rw-rw-rw-   0        0        0      860 2023-04-20 10:21:20.000000 amino.api-1.0b2/amino/__init__.py
--rw-rw-rw-   0        0        0     9436 2023-04-20 20:43:38.000000 amino.api-1.0b2/amino/client.py
--rw-rw-rw-   0        0        0    10084 2023-04-20 20:56:23.000000 amino.api-1.0b2/amino/full_client.py
--rw-rw-rw-   0        0        0     3582 2023-04-20 11:50:55.000000 amino.api-1.0b2/amino/local_client.py
--rw-rw-rw-   0        0        0    11406 2023-04-20 11:36:48.000000 amino.api-1.0b2/amino/socket.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:06:36.852437 amino.api-1.0b2/amino/utils/
--rw-rw-rw-   0        0        0        0 2023-04-18 12:11:03.000000 amino.api-1.0b2/amino/utils/__init__.py
--rw-rw-rw-   0        0        0      881 2023-04-20 08:49:05.000000 amino.api-1.0b2/amino/utils/exceptions.py
--rw-rw-rw-   0        0        0     7350 2023-04-20 16:39:36.000000 amino.api-1.0b2/amino/utils/helpers.py
--rw-rw-rw-   0        0        0     8804 2023-04-20 20:54:36.000000 amino.api-1.0b2/amino/utils/objects.py
--rw-rw-rw-   0        0        0     2117 2023-04-20 16:31:41.000000 amino.api-1.0b2/amino/utils/requester.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:06:36.825825 amino.api-1.0b2/amino.api.egg-info/
--rw-rw-rw-   0        0        0      558 2023-04-20 21:06:35.000000 amino.api-1.0b2/amino.api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-04-20 21:06:35.000000 amino.api-1.0b2/amino.api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 21:06:35.000000 amino.api-1.0b2/amino.api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 21:06:35.000000 amino.api-1.0b2/amino.api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 21:06:35.000000 amino.api-1.0b2/amino.api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 21:06:36.855430 amino.api-1.0b2/setup.cfg
--rw-rw-rw-   0        0        0     1444 2023-04-20 21:06:25.000000 amino.api-1.0b2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:19:32.995579 amino.api-1.1/
+-rw-rw-rw-   0        0        0      556 2023-04-21 11:19:32.995579 amino.api-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2023-04-18 11:48:20.000000 amino.api-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 11:19:32.938383 amino.api-1.1/amino/
+-rw-rw-rw-   0        0        0      855 2023-04-21 11:18:30.000000 amino.api-1.1/amino/__init__.py
+-rw-rw-rw-   0        0        0    18827 2023-04-21 11:17:28.000000 amino.api-1.1/amino/client.py
+-rw-rw-rw-   0        0        0    10084 2023-04-20 20:56:23.000000 amino.api-1.1/amino/full_client.py
+-rw-rw-rw-   0        0        0     3582 2023-04-20 11:50:55.000000 amino.api-1.1/amino/local_client.py
+-rw-rw-rw-   0        0        0    11406 2023-04-20 11:36:48.000000 amino.api-1.1/amino/socket.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:19:32.992585 amino.api-1.1/amino/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-18 12:11:03.000000 amino.api-1.1/amino/utils/__init__.py
+-rw-rw-rw-   0        0        0      980 2023-04-21 09:15:45.000000 amino.api-1.1/amino/utils/exceptions.py
+-rw-rw-rw-   0        0        0     7350 2023-04-20 16:39:36.000000 amino.api-1.1/amino/utils/helpers.py
+-rw-rw-rw-   0        0        0    10795 2023-04-21 10:51:11.000000 amino.api-1.1/amino/utils/objects.py
+-rw-rw-rw-   0        0        0     2117 2023-04-20 16:31:41.000000 amino.api-1.1/amino/utils/requester.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:19:32.965374 amino.api-1.1/amino.api.egg-info/
+-rw-rw-rw-   0        0        0      556 2023-04-21 11:19:31.000000 amino.api-1.1/amino.api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-04-21 11:19:31.000000 amino.api-1.1/amino.api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 11:19:31.000000 amino.api-1.1/amino.api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 11:19:31.000000 amino.api-1.1/amino.api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-21 11:19:31.000000 amino.api-1.1/amino.api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 11:19:32.998580 amino.api-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1442 2023-04-21 11:18:41.000000 amino.api-1.1/setup.py
```

### Comparing `amino.api-1.0b2/PKG-INFO` & `amino.api-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.0b2
+Version: 1.1
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino New Start</h1>
```

### Comparing `amino.api-1.0b2/amino/__init__.py` & `amino.api-1.1/amino/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 from .asynclib.local_client import AsyncLocalClient
 from .asynclib.socket import AsyncSocket
 
 from os import system as s
 from json import loads
 from requests import get
 
-__title__ = 'amino.py-api'
+__title__ = 'amino.api'
 __author__ = 'Xsarz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Xsarz'
-__version__ = '1.0b2'
+__version__ = '1.1'
 __newest__ = loads(get("https://pypi.org/pypi/amino.api/json").text)["info"]["version"]
 
 
 
 if __version__ != __newest__:
 	s('cls || clear')
 	print(f'\033[38;5;214m{__title__} made by {__author__}\nPlease update the library. Your version: {__version__}  A new version:{__newest__}\033[0m')
```

### Comparing `amino.api-1.0b2/amino/client.py` & `amino.api-1.1/amino/full_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from .socket import SocketHandler, Callbacks
 
 from time import time as timestamp
 from json import loads, dumps
 from requests import Session
 from typing import Union, BinaryIO
 from base64 import b64encode
-from json_minify import json_minify
 
-class Client(SocketHandler, Callbacks):
+
+class FullClient(SocketHandler, Callbacks):
 	def __init__(self, socket_enabled: bool = True, socket_debug: bool = False, socket_trace: bool = False,  auto_device: bool = False, deviceId: str = None, proxies: dict = None, certificatePath = None):
 		self.session = Session()
 		self.profile = objects.profile()
 		self.req = Requester(session=self.session, deviceId=deviceId, auto_device=auto_device, proxies=proxies, verify=certificatePath)
 		self.socket_enabled = socket_enabled
 
 		SocketHandler.__init__(self, self.req, socket_trace, socket_debug)
@@ -29,14 +29,23 @@
 
 	def set_device_id(self, deviceId: str):
 		self.req._set(2, deviceId)
 
 	def set_sid(self, sid: str):
 		self.req._set(1, sid)
 
+	def upload_media(self, file: BinaryIO, fileType: str):
+
+		if fileType == "audio":fileType = "audio/aac"
+		elif fileType == "image":fileType = "image/jpg"
+		else: raise exceptions.IncorrectType(fileType)
+		data = file.read()
+
+		response = self.req.make_request(method="POST", endpoint="/g/s/media/upload", body=data, type=fileType)
+		return loads(response.text)["mediaValue"]
 
 
 	def login(self, email: str, password: str = None, secret: str = None):
 		data = dumps({
 			"email": email,
 			"v": 2,
 			"secret": secret if secret else f"0 {password}",
@@ -144,25 +153,32 @@
 
 
 	def leave_community(self, comId: Union[int, str]):
 
 		response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/community/leave")
 		return response.status_code
 
-	def join_chat(self, chatId: str):
+	def join_chat(self, chatId: str, comId: Union[int, str] = None):
+		if comId:
+			response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/chat/thread/{chatId}/member/{self.profile.userId}", type="application/x-www-form-urlencoded")
+			return response.status_code		
 
 		response = self.req.make_request(method="POST", endpoint=f"/g/s/chat/thread/{chatId}/member/{self.profile.userId}", type="application/x-www-form-urlencoded")
 		return response.status_code
 
-	def leave_chat(self, chatId: str):
+	def leave_chat(self, chatId: str, comId: Union[int, str] = None):
+		if comId:
+			response = self.req.make_request(method="DELETE", endpoint=f"{self.api}/x{comId}/s/chat/thread/{chatId}/member/{self.profile.userId}")
+			return response.status_code		
 
 		response = self.req.make_request(method="DELETE", endpoint=f"/g/s/chat/thread/{chatId}/member/{self.profile.userId}")
 		return response.status_code
 
 
+
 	def send_message(self, chatId: str, comId: Union[int, str] = None, message: str = None, messageType: int = 0, file: BinaryIO = None, fileType: str = None, replyTo: str = None, mentionUserIds: list = None, stickerId: str = None, embedId: str = None, embedType: int = None, embedLink: str = None, embedTitle: str = None, embedContent: str = None, embedImage: BinaryIO = None):
 
 		if message and file is None:
 			message = message.replace("<@", "‎‏").replace("@>", "‬‭")
 		mentions = list()
 		if mentionUserIds:
 			for uid in mentionUserIds:
@@ -209,35 +225,37 @@
 				data["mediaUhqEnabled"] = True
 
 			else: raise exceptions.IncorrectType(f"fileType: {fileType}")
 
 			data["mediaUploadValue"] = b64encode(file.read()).decode()
 
 
-		response = self.req.make_request(method="POST", endpoint=f"/g/s/chat/thread/{chatId}/message", body=dumps(data))
+		response = self.req.make_request(
+				method="POST",
+				endpoint=f"/x{comId}/s/chat/thread/{chatId}/message" if comId else f"/g/s/chat/thread/{chatId}/message",
+				body=dumps(data)
+			)
 		return response.status_code
 
 
-
-	def delete_message(self, chatId: str, messageId: str, asStaff: bool = False, reason: str = None):
+	def delete_message(self, chatId: str, messageId: str, comId: Union[int, str] = None, asStaff: bool = False, reason: str = None):
 
 		if asStaff:
 			data = dumps({
 				"adminOpName": 102,
 				"adminOpNote": {"content": reason},
 				"timestamp": int(timestamp() * 1000)
 			})
 
-			response = self.req.make_request(method="POST", endpoint=f"/g/s/chat/thread/{chatId}/message/{messageId}/admin", body=data)
+			response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/chat/thread/{chatId}/message/{messageId}/admin" if comId else f"/g/s/chat/thread/{chatId}/message/{messageId}/admin", body=data)
 			return response.status_code			
 
-		response = self.req.make_request(method="DELETE", endpoint=f"/g/s/chat/thread/{chatId}/message/{messageId}")
+		response = self.req.make_request(method="DELETE", endpoint=f"/x{comId}/s/chat/thread/{chatId}/message/{messageId}" if comId else f"/g/s/chat/thread/{chatId}/message/{messageId}")
 		return response.status_code
 
-
 	def get_public_communities(self, language: str = "en", size: int = 25):
 
 		response = self.req.make_request(method="GET", endpoint=f"/g/s/topic/0/feed/community?language={language}&type=web-explore&categoryKey=recommendation&size={size}&pagingType=t")
 		return objects.communityList(loads(response.text))
 
 	def get_all_users(self, start: int = 0, size: int = 25):
 
@@ -255,14 +273,7 @@
 		return objects.coinHistoryList(loads(response.text).get("coinHistoryList", {}))
 
 
 	def watch_ad(self, userId: str = None):
 		data = dumps(self.req.gen.tapjoy_data(userId if userId else self.profile.userId))
 		response = self.req.session.request("POST", "https://ads.tapdaq.com/v4/analytics/reward", proxies=self.req.proxies, verify=self.req.verify, data=data, headers=self.req.gen.tapjoy_headers)
 		return exceptions.check_exceptions(response.text) if response.status_code != 204 else response.status_code
-
-
-	def send_active_obj(self, comId: str, tz: int = None, timers: list = None):
-		#TODO
-		data = json_minify(dumps({"userActiveTimeChunkList": timers, "timestamp": int(timestamp() * 1000), "optInAdsFlags": 2147483647, "timezone": tz if tz else self.req.gen.timezone()}))
-		response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/community/stats/user-active-time", body=data)
-		return response.status_code
```

### Comparing `amino.api-1.0b2/amino/local_client.py` & `amino.api-1.1/amino/local_client.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.0b2/amino/socket.py` & `amino.api-1.1/amino/socket.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.0b2/amino/utils/exceptions.py` & `amino.api-1.1/amino/utils/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 		Exception.__init__(*args, **kwargs)
 
 
 class IncorrectType(Exception):
 	def __init__(*args, **kwargs):
 		Exception.__init__(*args, **kwargs)
 
-
+class AgeTooLow(Exception):
+	def __init__(*args, **kwargs):
+		Exception.__init__(*args, **kwargs)
 
 errors = {
 }
 
 def check_exceptions(data):
 	try:
 		data = loads(data)
```

### Comparing `amino.api-1.0b2/amino/utils/helpers.py` & `amino.api-1.1/amino/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.0b2/amino/utils/objects.py` & `amino.api-1.1/amino/utils/objects.py`

 * *Files 9% similar despite different names*

```diff
@@ -211,8 +211,65 @@
 		self.promotionalMediaList = self.json.get("activeInfo")
 		self.icon = self.json.get("icon")
 		self.link = self.json.get("link")
 		self.updatedTime = self.json.get("updatedTime")
 		self.endpoint = self.json.get("endpoint")
 		self.name = self.json.get("name")
 		self.templateId = self.json.get("templateId")
-		self.createdTime = self.json.get("createdTime")
+		self.createdTime = self.json.get("createdTime")
+
+
+
+
+class ThreadList:
+	def __init__(self, data: dict = []):
+		self.json = data
+		self.chats = list()
+		for chat in self.json:
+			if isinstance(chat, dict):
+				self.chats.append(Thread(chat))
+
+
+class Thread:
+	def __init__(self, data: dict = []):
+		self.json = data
+		self.userAddedTopicList = self.json.get("userAddedTopicList", [])
+		self.membersQuota = self.json.get("membersQuota")
+		self.membersSummary = list()
+		self.chatId = self.json.get("threadId")
+		self.keywords = self.json.get("keywords")
+		self.membersCount = self.json.get("membersCount")
+		self.strategyInfo = self.json.get("strategyInfo")
+		self.isPinned = self.json.get("isPinned")
+		self.title = self.json.get("title")
+		self.membershipStatus = self.json.get("membershipStatus")
+		self.content = self.json.get("content")
+		self.needHidden = self.json.get("needHidden")
+		self.alertOption = self.json.get("alertOption")
+		self.lastReadTime = self.json.get("lastReadTime")
+		self.type = self.json.get("type")
+		self.status = self.json.get("status")
+		self.modifiedTime = self.json.get("modifiedTime")
+		self.lastMessageSummary = Message(self.json.get("lastMessageSummary", {}))
+		self.condition = self.json.get("condition")
+		self.icon = self.json.get("icon")
+		self.latestActivityTime = self.json.get("latestActivityTime")
+		self.author = UserProfile(self.json.get("author", {}))
+		self.extensions = self.json.get("extensions", {})
+		self.comId = self.json.get("ndcId")
+		self.createdTime = self.json.get("createdTime")
+
+		for member in self.json.get("membersSummary", []):
+			self.membersSummary.append(UserProfile(member))
+
+
+
+class MessageList:
+	def __init__(self, data: dict = []):
+		self.json = data
+		paging = self.json.get("paging", {})
+		
+		self.messages = list()
+		self.nextPageToken = paging.get("nextPageToken")
+		self.prevPageToken = paging.get("prevPageToken")
+		for message in self.json.get("messageList", []):
+			self.messages.append(Message(message))
```

### Comparing `amino.api-1.0b2/amino/utils/requester.py` & `amino.api-1.1/amino/utils/requester.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.0b2/amino.api.egg-info/PKG-INFO` & `amino.api-1.1/amino.api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.0b2
+Version: 1.1
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino New Start</h1>
```

### Comparing `amino.api-1.0b2/setup.py` & `amino.api-1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 info = {
 	"name": "amino.api",
-	"version": "1.0b2",
+	"version": "1.1",
 	"github_page": "https://github.com/xXxCLOTIxXx/amino.api",
 	"download_link": "https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip",
 	"license": "MIT",
 	"author": "Xsarz",
 	"author_email": "xsarzy@gmail.com",
 	"description": "Library for creating amino bots and scripts.",
 	"long_description": None,
```

