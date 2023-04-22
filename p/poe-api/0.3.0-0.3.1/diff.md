# Comparing `tmp/poe_api-0.3.0-py3-none-any.whl.zip` & `tmp/poe_api-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 36504 bytes, number of entries: 40
--rw-r--r--  2.0 unx    16058 b- defN 23-Apr-17 09:12 poe.py
+Zip file size: 37114 bytes, number of entries: 40
+-rw-r--r--  2.0 unx    16891 b- defN 23-Apr-22 02:50 poe.py
 -rw-r--r--  2.0 unx     1093 b- defN 23-Apr-08 20:17 poe_graphql/AddHumanMessageMutation.graphql
 -rw-r--r--  2.0 unx      373 b- defN 23-Apr-08 20:17 poe_graphql/AddMessageBreakMutation.graphql
 -rw-r--r--  2.0 unx      180 b- defN 23-Apr-08 20:17 poe_graphql/AutoSubscriptionMutation.graphql
 -rw-r--r--  2.0 unx       97 b- defN 23-Apr-08 20:17 poe_graphql/BioFragment.graphql
 -rw-r--r--  2.0 unx       73 b- defN 23-Apr-08 20:17 poe_graphql/ChatAddedSubscription.graphql
 -rw-r--r--  2.0 unx      100 b- defN 23-Apr-08 20:17 poe_graphql/ChatFragment.graphql
 -rw-r--r--  2.0 unx     6971 b- defN 23-Apr-08 20:17 poe_graphql/ChatListPaginationQuery.graphql
@@ -30,13 +30,13 @@
 -rw-r--r--  2.0 unx      147 b- defN 23-Apr-08 20:17 poe_graphql/SummarizeQuotePostQuery.graphql
 -rw-r--r--  2.0 unx      180 b- defN 23-Apr-08 20:17 poe_graphql/SummarizeSharePostQuery.graphql
 -rw-r--r--  2.0 unx      368 b- defN 23-Apr-08 20:17 poe_graphql/UserSnippetFragment.graphql
 -rw-r--r--  2.0 unx      400 b- defN 23-Apr-08 20:17 poe_graphql/ViewerInfoQuery.graphql
 -rw-r--r--  2.0 unx     1038 b- defN 23-Apr-08 20:17 poe_graphql/ViewerStateFragment.graphql
 -rw-r--r--  2.0 unx      657 b- defN 23-Apr-08 20:17 poe_graphql/ViewerStateUpdatedSubscription.graphql
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-08 20:17 poe_graphql/__init__.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Apr-17 09:19 poe_api-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    13746 b- defN 23-Apr-17 09:19 poe_api-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 09:19 poe_api-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-17 09:19 poe_api-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3759 b- defN 23-Apr-17 09:19 poe_api-0.3.0.dist-info/RECORD
-40 files, 89025 bytes uncompressed, 30306 bytes compressed:  66.0%
+-rw-r--r--  2.0 unx    35149 b- defN 23-Apr-22 02:55 poe_api-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14177 b- defN 23-Apr-22 02:55 poe_api-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 02:55 poe_api-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-22 02:55 poe_api-0.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3759 b- defN 23-Apr-22 02:55 poe_api-0.3.1.dist-info/RECORD
+40 files, 90289 bytes uncompressed, 30916 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -99,23 +99,23 @@
 
 Filename: poe_graphql/ViewerStateUpdatedSubscription.graphql
 Comment: 
 
 Filename: poe_graphql/__init__.py
 Comment: 
 
-Filename: poe_api-0.3.0.dist-info/LICENSE
+Filename: poe_api-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: poe_api-0.3.0.dist-info/METADATA
+Filename: poe_api-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: poe_api-0.3.0.dist-info/WHEEL
+Filename: poe_api-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: poe_api-0.3.0.dist-info/top_level.txt
+Filename: poe_api-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: poe_api-0.3.0.dist-info/RECORD
+Filename: poe_api-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## poe.py

```diff
@@ -1,22 +1,35 @@
 import requests, re, json, random, logging, time, queue, threading, traceback, hashlib, string, random
 import requests.adapters
 import websocket
 from pathlib import Path
 from urllib.parse import urlparse
 
-
 parent_path = Path(__file__).resolve().parent
 queries_path = parent_path / "poe_graphql"
 queries = {}
 
 logging.basicConfig()
 logger = logging.getLogger()
 
-user_agent = "Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0"
+user_agent = "This will be ignored! See the README for info on how to set custom headers."
+headers = {
+  "User-Agent": "Mozilla/5.0 (X11; CrOS x86_64 14541.0.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36",
+  "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+  "Accept-Encoding": "gzip, deflate, br",
+  "Accept-Language": "en-US,en;q=0.9,und;q=0.8,af;q=0.7",
+  "Cache-Control": "no-cache",
+  "Dnt": "1",
+  "Pragma": "no-cache",
+  "Sec-Ch-Ua": "\"Google Chrome\";v=\"111\", \"Not(A:Brand\";v=\"8\", \"Chromium\";v=\"111\"",
+  "Sec-Ch-Ua-Mobile": "?0",
+  "Sec-Ch-Ua-Platform": "\"Chrome OS\"",
+  "Sec-Gpc": "1",
+  "Upgrade-Insecure-Requests": "1"
+}
 
 def load_queries():
   for path in queries_path.iterdir():
     if path.suffix != ".graphql":
       continue
     with open(path) as f:
       queries[path.stem] = f.read()
@@ -40,15 +53,15 @@
 
 class Client:
   gql_url = "https://poe.com/api/gql_POST"
   gql_recv_url = "https://poe.com/api/receive_POST"
   home_url = "https://poe.com"
   settings_url = "https://poe.com/api/settings"
   
-  def __init__(self, token, proxy=None):
+  def __init__(self, token, proxy=None, headers=headers):
     self.proxy = proxy
     self.session = requests.Session()
     self.adapter = requests.adapters.HTTPAdapter(pool_connections=100, pool_maxsize=100)
     self.session.mount("http://", self.adapter)
     self.session.mount("https://", self.adapter)
         
     if proxy:
@@ -58,19 +71,22 @@
       }
       logger.info(f"Proxy enabled: {self.proxy}")
 
     self.active_messages = {}
     self.message_queues = {}
 
     self.session.cookies.set("p-b", token, domain="poe.com")
-    self.headers = {
-      "User-Agent": user_agent,
+    self.headers = {**headers, **{
       "Referrer": "https://poe.com/",
       "Origin": "https://poe.com",
-    }
+      "Host": "poe.com",
+      "Sec-Fetch-Dest": "empty",
+      "Sec-Fetch-Mode": "cors",
+      "Sec-Fetch-Site": "same-origin",
+    }}
     self.session.headers.update(self.headers)
 
     self.setup_connection()
     self.connect_ws()
 
   def setup_connection(self):
     self.ws_domain = f"tch{random.randint(1, 1e6)}"
@@ -176,16 +192,16 @@
   
   def get_websocket_url(self, channel=None):
     if channel is None:
       channel = self.channel
     query = f'?min_seq={channel["minSeq"]}&channel={channel["channel"]}&hash={channel["channelHash"]}'
     return f'wss://{self.ws_domain}.tch.{channel["baseHost"]}/up/{channel["boxName"]}/updates'+query
 
-  def send_query(self, query_name, variables):
-    for i in range(20):
+  def send_query(self, query_name, variables, attempts=20):
+    for i in range(attempts):
       json_data = generate_payload(query_name, variables)
       payload = json.dumps(json_data, separators=(",", ":"))
       
       base_string = payload + self.gql_headers["poe-formkey"] + "WpuLMiXEKKE98j56k"
       
       headers = {
         "content-type": "application/json",
```

## Comparing `poe_api-0.3.0.dist-info/LICENSE` & `poe_api-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `poe_api-0.3.0.dist-info/METADATA` & `poe_api-0.3.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-api
-Version: 0.3.0
+Version: 0.3.1
 Summary: A reverse engineered API wrapper for Quora's Poe
 Home-page: https://github.com/ading2210/poe-api
 Author: ading2210
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -34,15 +34,14 @@
     + [Clearing the Conversation Context](#clearing-the-conversation-context)
     + [Downloading Conversation History](#downloading-conversation-history)
     + [Deleting Messages](#deleting-messages)
     + [Purging a Conversation](#purging-a-conversation)
   * [Misc](#misc)
     + [Changing the Logging Level](#changing-the-logging-level)
     + [Setting a Custom User-Agent](#setting-a-custom-user-agent)
-    + [Bypassing The GPT-4 Quota](#)
 - [Copyright](#copyright)
   * [Copyright Notice](#copyright-notice)
 
 *Table of contents generated with [markdown-toc](http://ecotrust-canada.github.io/markdown-toc).*
 
 ## Features:
  - Log in with token
@@ -128,15 +127,15 @@
 ```
 
 #### Editing a Bot:
 You can edit a custom bot using the `client.edit_bot` function, which accepts the following arguments:
  - `bot_id` - The `botId` of the bot to edit.
  - `handle` - The handle of the bot to edit.
  - `prompt` - The prompt for the new bot.
- - `base_model = "chinchilla"` - The new model that the bot uses. This can be any of the preset models, including ones that are limited on free accounts.
+ - `base_model = "chinchilla"` - The new model that the bot uses. This must be either `"chinchilla"` (ChatGPT)  or `"a2"` (Claude). Previously, it was possible to set this to `"beaver"` (GPT-4), which would bypass the free account restrictions, but this is now patched.
  - `description = ""` - The new description for the bot.
  - `intro_message = ""` - The new intro message for the bot. If this is an empty string then the bot will not have an intro message.
  - `prompt_public = True` - Whether or not the prompt should be publicly visible. 
  - `pfp_url = None` - The URL for the bot's profile picture. Currently, there is no way to actually upload a custom image using this library.
  - `linkification = False` - Whether or not the bot should turn some text in the response into clickable links.
  - `markdown_rendering = True` - Whether or not to enable markdown rendering for the bot's responses.
  - `suggested_replies = False` - Whether or not the bot should suggest possible replies after each response.
@@ -259,34 +258,49 @@
 ```python
 import poe
 import logging
 poe.logger.setLevel(logging.INFO)
 ```
 
 #### Setting a Custom User-Agent:
-If you want to change the user-agent that is being spoofed, set `poe.user_agent` after importing the library. 
+If you want to change the headers that are spoofed, set `poe.headers` after importing the library. 
 
+To use your browser's own headers, visit [this site](https://headers.uniqueostrich18.repl.co/), and copy-paste its contents.
 ```python
 import poe
-poe.user_agent = "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36"
+poe.headers = {
+  "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0",
+  "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
+  "Accept-Encoding": "gzip, deflate, br",
+  "Accept-Language": "en-US,en;q=0.5",
+  "Te": "trailers",
+  "Upgrade-Insecure-Requests": "1"
+}
+```
+
+The following headers will be ignored and overwritten:
+```python
+{
+  "Referrer": "https://poe.com/",
+  "Origin": "https://poe.com",
+  "Host": "poe.com",
+  "Sec-Fetch-Dest": "empty",
+  "Sec-Fetch-Mode": "cors",
+  "Sec-Fetch-Site": "same-origin"
+}
 ```
 
-#### Bypassing the Free Account Quota:
-You can bypass the free account quota simply by editing a custom bot and setting the base model to one of the following options:
- - `"a2_2"` - Claude+ (normal limit: 3 messages/day)
- - `"beaver"` - GPT-4 (normal limit: 1 message/day)
-
-An example of how to do this is located at `examples/create_bot.py`.
+Previously, this was done through `poe.user_agent`, but that variable is now completely ignored.
 
 ## Copyright: 
 This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt). Most code, with the exception of the GraphQL queries, has been written by me, [ading2210](https://github.com/ading2210).
 
 Reverse engineering the `poe-tag-id` header has been done by [xtekky](https://github.com/xtekky) in [PR #39](https://github.com/ading2210/poe-api/pull/39).
 
-The `client.get_remaining_messages` was written by [Snowad14](https://github.com/Snowad14) in [PR #46](https://github.com/ading2210/poe-api/pull/46).
+The `client.get_remaining_messages` function was written by [Snowad14](https://github.com/Snowad14) in [PR #46](https://github.com/ading2210/poe-api/pull/46).
 
 Most of the GraphQL queries are taken from [muharamdani/poe](https://github.com/muharamdani/poe), which is licenced under the ISC License. 
 
 ### Copyright Notice:
 ```
 ading2210/poe-api: a reverse engineered Python API wrapepr for Quora's Poe
 Copyright (C) 2023 ading2210
```

## Comparing `poe_api-0.3.0.dist-info/RECORD` & `poe_api-0.3.1.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-poe.py,sha256=LOSiQtZYSYOROfM3HityesCI58-4yfDLCtVnQdT0h-0,16058
+poe.py,sha256=ue5A8T9gys7Lf21wlnt6yrxc8bkX8X_nG7zA9JN2Zn4,16891
 poe_graphql/AddHumanMessageMutation.graphql,sha256=Va4SoysKE2qPlJfbwoKp6mNv0vs5hnVR20g8hPvAxdY,1093
 poe_graphql/AddMessageBreakMutation.graphql,sha256=0XrqSAgAkG5vCFwBALRpoAgUDSFM9XUB5wBy5Iou9c8,373
 poe_graphql/AutoSubscriptionMutation.graphql,sha256=3i8EnqwUrjOcJ2Hxly-lKhwPBJdbpO99POiM_K6jVD4,180
 poe_graphql/BioFragment.graphql,sha256=3ZdXaPtuHK38bG10WFH6bvpebcyrTLu5fs-ddtfLjf0,97
 poe_graphql/ChatAddedSubscription.graphql,sha256=NFLZJAwi0V2WQea1oelyRUrtNrwOE58NOeX8ChzVE10,73
 poe_graphql/ChatFragment.graphql,sha256=NFVSvT3NdYlEquue3yTHPu9ezCIgx6k1OXJZo2ytIzU,100
 poe_graphql/ChatListPaginationQuery.graphql,sha256=-jtpUwcHsF8nEXQcxLe9gFycYuKRVDBjGNFiH-nPL98,6971
@@ -29,12 +29,12 @@
 poe_graphql/SummarizeQuotePostQuery.graphql,sha256=V4PQ1XkEDCsVR3z7h4SLsonZsWG7RptFd6JPwlGwOvE,147
 poe_graphql/SummarizeSharePostQuery.graphql,sha256=iCN8oiUUp2jfsiBxmsTA7k3_60E0MNwA5gnNrhnYpJc,180
 poe_graphql/UserSnippetFragment.graphql,sha256=Eg8rK7XM6-HqVJkpEBY0bJaYqF-FdDdWdg-Jj3VTnF0,368
 poe_graphql/ViewerInfoQuery.graphql,sha256=Xtn-VGGiknKgrW81s7YfIJwhmilobrSqiCObpoJdYfw,400
 poe_graphql/ViewerStateFragment.graphql,sha256=aicUJncsRpPBh_L2xqDv0aHcUIPIsDrDFPfDs3jcFoU,1038
 poe_graphql/ViewerStateUpdatedSubscription.graphql,sha256=1dPs0WuOLl4ybZXm4bUF60eVc94O10EkKOtqnQYODic,657
 poe_graphql/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-poe_api-0.3.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-poe_api-0.3.0.dist-info/METADATA,sha256=g1vRVkLWDuhHpweg784-IaSKdOg2Lk3uQUM7LkeCYkI,13746
-poe_api-0.3.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-poe_api-0.3.0.dist-info/top_level.txt,sha256=7Sk_jA5I5n3fNZ1671pcBau4TWZLe6UXCEnCD5NhGGI,16
-poe_api-0.3.0.dist-info/RECORD,,
+poe_api-0.3.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+poe_api-0.3.1.dist-info/METADATA,sha256=m657xYNo5rqJBG7s-N5qQcoqePidrcpZyb80Cc2sbeg,14177
+poe_api-0.3.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+poe_api-0.3.1.dist-info/top_level.txt,sha256=7Sk_jA5I5n3fNZ1671pcBau4TWZLe6UXCEnCD5NhGGI,16
+poe_api-0.3.1.dist-info/RECORD,,
```

