# Comparing `tmp/telespider-0.2.3.tar.gz` & `tmp/telespider-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telespider-0.2.3.tar", max compression
+gzip compressed data, was "telespider-0.2.4.tar", max compression
```

## Comparing `telespider-0.2.3.tar` & `telespider-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2023-04-20 08:10:29.039624 telespider-0.2.3/LICENSE
--rw-r--r--   0        0        0      934 2023-04-22 08:18:34.032173 telespider-0.2.3/README.md
--rw-r--r--   0        0        0      592 2023-04-22 09:28:37.068328 telespider-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-22 09:11:54.244843 telespider-0.2.3/telespider/__init__.py
--rw-r--r--   0        0        0     2662 2023-04-22 09:20:41.573975 telespider-0.2.3/telespider/__main__.py
--rw-r--r--   0        0        0     1701 2023-04-22 09:20:55.313815 telespider-0.2.3/telespider/app.py
--rw-r--r--   0        0        0      605 2023-04-22 09:28:07.946481 telespider-0.2.3/telespider/config.py
--rw-r--r--   0        0        0      201 2023-04-22 09:27:51.193158 telespider-0.2.3/telespider/console.py
--rw-r--r--   0        0        0       69 2023-04-22 08:06:36.213270 telespider-0.2.3/telespider/scrapper/__init__.py
--rw-r--r--   0        0        0     2095 2023-04-22 08:36:14.647055 telespider-0.2.3/telespider/scrapper/channel.py
--rw-r--r--   0        0        0     5475 2023-04-22 09:20:55.193817 telespider-0.2.3/telespider/scrapper/scrapper.py
--rw-r--r--   0        0        0      361 2023-04-22 08:47:20.048014 telespider-0.2.3/telespider/scrapper/types.py
--rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 telespider-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-20 08:10:29.039624 telespider-0.2.4/LICENSE
+-rw-r--r--   0        0        0      934 2023-04-22 08:18:34.032173 telespider-0.2.4/README.md
+-rw-r--r--   0        0        0      592 2023-04-22 10:02:05.279521 telespider-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-22 09:11:54.244843 telespider-0.2.4/telespider/__init__.py
+-rw-r--r--   0        0        0     3743 2023-04-22 10:01:36.656824 telespider-0.2.4/telespider/__main__.py
+-rw-r--r--   0        0        0     1771 2023-04-22 10:01:36.656824 telespider-0.2.4/telespider/app.py
+-rw-r--r--   0        0        0      605 2023-04-22 09:28:07.946481 telespider-0.2.4/telespider/config.py
+-rw-r--r--   0        0        0      150 2023-04-22 10:01:36.656824 telespider-0.2.4/telespider/console.py
+-rw-r--r--   0        0        0       69 2023-04-22 08:06:36.213270 telespider-0.2.4/telespider/scrapper/__init__.py
+-rw-r--r--   0        0        0     2095 2023-04-22 08:36:14.647055 telespider-0.2.4/telespider/scrapper/channel.py
+-rw-r--r--   0        0        0     3893 2023-04-22 10:01:36.656824 telespider-0.2.4/telespider/scrapper/scrapper.py
+-rw-r--r--   0        0        0      361 2023-04-22 08:47:20.048014 telespider-0.2.4/telespider/scrapper/types.py
+-rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 telespider-0.2.4/PKG-INFO
```

### Comparing `telespider-0.2.3/LICENSE` & `telespider-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `telespider-0.2.3/README.md` & `telespider-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `telespider-0.2.3/pyproject.toml` & `telespider-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telespider"
-version = "0.2.3"
+version = "0.2.4"
 description = "recursively parsing tg channels"
 authors = ["andrewsap <andrewsapw@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `telespider-0.2.3/telespider/config.py` & `telespider-0.2.4/telespider/config.py`

 * *Files identical despite different names*

### Comparing `telespider-0.2.3/telespider/scrapper/channel.py` & `telespider-0.2.4/telespider/scrapper/channel.py`

 * *Files identical despite different names*

### Comparing `telespider-0.2.3/telespider/scrapper/scrapper.py` & `telespider-0.2.4/telespider/scrapper/scrapper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from typing import AsyncGenerator, List, Set
 from collections import deque
 
-from pyrogram.types import Message
 from pyrogram.client import Client
 from pyrogram.enums import MessageEntityType
-from rich.panel import Panel
 
 from telespider.config import settings
-from telespider.console import console
 from .types import ExploreChannelsProgress, MessageParsingProgress
 from .channel import parse_channel, extract_channels
 
 CHANNELS = settings.ENTRYPOINT_CHANNELS.split(",")
 
 
 async def parse_messages(
@@ -80,80 +77,47 @@
         )
 
         parsed_channels.add(channel)
 
 
 async def search_text(
     app: Client, text: str, channels: List[str]
-) -> AsyncGenerator[Message, None]:
+) -> AsyncGenerator[MessageParsingProgress, None]:
     """Search for text in messages"""
 
-    with console.status("Working...") as status:
-        n_parsed = 0
-        async for p in parse_messages(app=app, channels=channels):
-            m = p.message
-
-            if n_parsed % 100 == 0:
-                status.update(
-                    f"Parsed: {p.channels_parsed} ch. {n_parsed} messages  - remaining {p.channels_remaining} ch."  # noqa: E501
-                    f" | Searching for word [bold]{text}[/bold] in {m.chat.username}"
-                )
-
-            # update task description
-            message_text = m.text or m.caption
-            if text in message_text.lower():
-                # console.print(f"[bold]{m.chat.username}[/bold] - {message_text}")
-                console.print(
-                    Panel(
-                        message_text,
-                        title=f"{m.chat.username} ({m.date.strftime('%Y-%m-%d')})",
-                    )
-                )
-                yield m
+    async for p in parse_messages(app=app, channels=channels):
+        m = p.message
 
-            n_parsed += 1
+        # update task description
+        message_text = m.text or m.caption
+        if text in message_text.lower():
+            yield p
 
 
 async def search_mentions(
     app: Client, mention: str, channels: List[str]
-) -> AsyncGenerator[Message, None]:
+) -> AsyncGenerator[MessageParsingProgress, None]:
     """Search for mentions in messages"""
     if mention.startswith("@"):
         mention = mention[1:]
 
-    with console.status("Working...") as status:
-        n_parsed = 0
-        async for p in parse_messages(app=app, channels=channels):
-            m = p.message
-
-            if n_parsed % 100 == 0:
-                status.update(
-                    f"Parsed: {p.channels_parsed} ch. {n_parsed} messages  - remaining {p.channels_remaining} ch."  # noqa: E501
-                    f" | Searching for mention of [bold]{mention}[/bold] in {m.chat.username}"
-                )
-
-            # update task description
-            message_text = m.text or m.caption
-            if m.entities is None:
-                continue
+    async for p in parse_messages(app=app, channels=channels):
+        m = p.message
 
-            for message_mention in m.entities:
-                if message_mention.type in (
-                    MessageEntityType.MENTION,
-                    MessageEntityType.TEXT_MENTION,
-                ):
-                    mentioned = message_text[
-                        message_mention.offset
-                        + 1 : message_mention.offset
-                        + message_mention.length
-                    ]
-
-                    if mentioned == mention:
-                        console.print(
-                            Panel(
-                                message_text,
-                                title=f"{m.chat.username} ({m.date.strftime('%Y-%m-%d')})",
-                            )
-                        )
-                        yield m
+        # update task description
+        message_text = m.text or m.caption
+        if m.entities is None:
+            continue
+
+        for message_mention in m.entities:
+            if message_mention.type in (
+                MessageEntityType.MENTION,
+                MessageEntityType.TEXT_MENTION,
+            ):
+                mentioned = message_text[
+                    message_mention.offset
+                    + 1 : message_mention.offset
+                    + message_mention.length
+                ]
 
-            n_parsed += 1
+                if mentioned == mention:
+                    yield p
```

### Comparing `telespider-0.2.3/PKG-INFO` & `telespider-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telespider
-Version: 0.2.3
+Version: 0.2.4
 Summary: recursively parsing tg channels
 License: MIT
 Author: andrewsap
 Author-email: andrewsapw@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

