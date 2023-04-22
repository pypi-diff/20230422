# Comparing `tmp/telespider-0.1.1.tar.gz` & `tmp/telespider-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telespider-0.1.1.tar", max compression
+gzip compressed data, was "telespider-0.2.0.tar", max compression
```

## Comparing `telespider-0.1.1.tar` & `telespider-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2023-04-20 08:10:29.039624 telespider-0.1.1/LICENSE
--rw-r--r--   0        0        0      934 2023-04-22 08:18:34.032173 telespider-0.1.1/README.md
--rw-r--r--   0        0        0      592 2023-04-22 08:19:38.407063 telespider-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       26 2023-04-17 17:49:13.844485 telespider-0.1.1/telespider/__init__.py
--rw-r--r--   0        0        0     2392 2023-04-22 08:11:49.578255 telespider-0.1.1/telespider/__main__.py
--rw-r--r--   0        0        0      287 2023-04-17 17:57:56.434471 telespider-0.1.1/telespider/app.py
--rw-r--r--   0        0        0      538 2023-04-19 16:12:02.069745 telespider-0.1.1/telespider/config.py
--rw-r--r--   0        0        0      152 2023-04-19 17:18:45.959480 telespider-0.1.1/telespider/console.py
--rw-r--r--   0        0        0       69 2023-04-22 08:06:36.213270 telespider-0.1.1/telespider/scrapper/__init__.py
--rw-r--r--   0        0        0     2065 2023-04-22 08:01:16.056546 telespider-0.1.1/telespider/scrapper/channel.py
--rw-r--r--   0        0        0     4886 2023-04-22 08:10:51.262527 telespider-0.1.1/telespider/scrapper/scrapper.py
--rw-r--r--   0        0        0      358 2023-04-22 08:10:51.262527 telespider-0.1.1/telespider/scrapper/types.py
--rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 telespider-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-20 08:10:29.039624 telespider-0.2.0/LICENSE
+-rw-r--r--   0        0        0      934 2023-04-22 08:18:34.032173 telespider-0.2.0/README.md
+-rw-r--r--   0        0        0      592 2023-04-22 08:50:39.059492 telespider-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-04-17 17:49:13.844485 telespider-0.2.0/telespider/__init__.py
+-rw-r--r--   0        0        0     2820 2023-04-22 08:48:07.464858 telespider-0.2.0/telespider/__main__.py
+-rw-r--r--   0        0        0      305 2023-04-22 08:49:32.861777 telespider-0.2.0/telespider/app.py
+-rw-r--r--   0        0        0      538 2023-04-19 16:12:02.069745 telespider-0.2.0/telespider/config.py
+-rw-r--r--   0        0        0      152 2023-04-19 17:18:45.959480 telespider-0.2.0/telespider/console.py
+-rw-r--r--   0        0        0       69 2023-04-22 08:06:36.213270 telespider-0.2.0/telespider/scrapper/__init__.py
+-rw-r--r--   0        0        0     2095 2023-04-22 08:36:14.647055 telespider-0.2.0/telespider/scrapper/channel.py
+-rw-r--r--   0        0        0     5417 2023-04-22 08:47:54.211309 telespider-0.2.0/telespider/scrapper/scrapper.py
+-rw-r--r--   0        0        0      361 2023-04-22 08:47:20.048014 telespider-0.2.0/telespider/scrapper/types.py
+-rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 telespider-0.2.0/PKG-INFO
```

### Comparing `telespider-0.1.1/LICENSE` & `telespider-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `telespider-0.1.1/README.md` & `telespider-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `telespider-0.1.1/pyproject.toml` & `telespider-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telespider"
-version = "0.1.1"
+version = "0.2.0"
 description = "recursively parsing tg channels"
 authors = ["andrewsap <andrewsapw@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `telespider-0.1.1/telespider/__main__.py` & `telespider-0.2.0/telespider/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from typing import Optional
 import asyncio
 import uvloop
 
 import click
 
 from telespider import scrapper
-from telespider.config import settings
-from telespider.app import app
+from telespider.config import settings, ROOT_DIR
+from telespider.app import App
 from telespider.console import console
 
 uvloop.install()
 
 
 def coro(f):
     @wraps(f)
@@ -19,67 +19,83 @@
         return asyncio.get_event_loop().run_until_complete(f(*args, **kwargs))
 
     return wrapper
 
 
 @click.group()
 @click.option("--debug/--no-debug", default=False)
+@click.option(
+    "--workdir", type=click.Path(exists=True), default=ROOT_DIR.parent / "sessions"
+)
 @click.pass_context
-def cli(ctx, debug):
+def cli(ctx, debug, workdir):
+    app = App(
+        name=settings.APP_NAME,
+        api_id=settings.API_ID,
+        api_hash=settings.API_HASH,
+        workdir=workdir,
+    )
     ctx.ensure_object(dict)
     ctx.obj["DEBUG"] = debug
+    ctx.obj["APP"] = app.app
 
 
 @cli.command(name="search", help="Search word or user mentions in channels messages")
 @click.option("--explore/--no-explore", default=True, help="Auto explore new channels")
 @click.option("--silent", is_flag=True, default=False, help="Suppress all output")
 @click.option("--word", "-w", type=str, required=False)
 @click.option("--user", "-u", type=str, required=False)
 @click.option(
     "-n", type=int, default=1000, help="Number of messages to parse per channel"
 )
+@click.pass_context
 @coro
 async def search_word(
-    explore: bool, silent: bool, word: Optional[str], user: Optional[str], n: int
+    ctx, explore: bool, silent: bool, word: Optional[str], user: Optional[str], n: int
 ):
     if word is None and user is None:
         raise click.BadOptionUsage(
             option_name="word | user", message="word or user must be specified"
         )
 
+    app = ctx.obj["APP"]
+
     settings.MAX_PER_CHANNEL = n
     settings.AUTO_EXPLORE_CHANNELS = explore
     console.quiet = silent
 
     await app.start()
     try:
         if word is not None:
-            async for _ in scrapper.search_text(word):
+            async for _ in scrapper.search_text(app=app, text=word):
                 ...
         elif user is not None:
-            async for _ in scrapper.search_mentions(user):
+            async for _ in scrapper.search_mentions(app=app, mention=user):
                 ...
     finally:
         await app.stop(block=False)
 
 
 @cli.command(name="explore-channels", help="Explore channels mentions")
 @click.option("--silent", is_flag=True, default=False, help="Suppress all output")
 @click.option(
     "-n", type=int, default=1000, help="Number of messages to parse per channel"
 )
+@click.pass_context
 @coro
-async def explore_channels(silent: bool, n: int):
+async def explore_channels(ctx, silent: bool, n: int):
     settings.MAX_PER_CHANNEL = n
     console.quiet = silent
 
+    app = ctx.obj["APP"]
+
     await app.start()
     try:
-        async for i in scrapper.explore_channels():
-            source_channel = i.message.chat.username
+        async for i in scrapper.explore_channels(app=app):
+            source_channel = i.source_channel
             console.print(f"{source_channel}: {i.mentions}")
     finally:
         await app.stop(block=False)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `telespider-0.1.1/telespider/config.py` & `telespider-0.2.0/telespider/config.py`

 * *Files identical despite different names*

### Comparing `telespider-0.1.1/telespider/scrapper/channel.py` & `telespider-0.2.0/telespider/scrapper/channel.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 from pyrogram.types import Message, Chat
 from pyrogram.errors.exceptions.bad_request_400 import (
     UsernameNotOccupied,
     UsernameInvalid,
 )
 
 from pyrogram.enums import MessageEntityType
+from pyrogram.client import Client
 
 from telespider.config import settings
-from telespider.app import app
 from telespider.console import logger
 
 CHANNELS = settings.ENTRYPOINT_CHANNELS.split(",")
 
 
 async def parse_channel(
-    channel_name: str, limit: int = settings.MAX_PER_CHANNEL
+    app: Client, channel_name: str, limit: int = settings.MAX_PER_CHANNEL
 ) -> AsyncGenerator[Message, None]:
     try:
         async for message in app.get_chat_history(channel_name, limit=limit):
             yield message
     except (UsernameNotOccupied, UsernameInvalid):
         logger.error(f"Skipping {channel_name} - does not exists or invalid")
         return
 
 
 async def search_message(
-    channel_name: str, query: str
+    app: Client, channel_name: str, query: str
 ) -> AsyncGenerator[Message, None]:
     async for message in app.search_messages(channel_name, query=query):
         yield message
 
 
 def extract_channels(message: Message) -> List[str]:
     linked_channels = []
```

### Comparing `telespider-0.1.1/telespider/scrapper/scrapper.py` & `telespider-0.2.0/telespider/scrapper/scrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,97 @@
-from typing import AsyncGenerator, List
+from typing import AsyncGenerator, List, Set
 from collections import deque
 
 from pyrogram.types import Message
+from pyrogram.client import Client
 from pyrogram.enums import MessageEntityType
 from rich.panel import Panel
 
 from telespider.config import settings
 from telespider.console import console
 from .types import ExploreChannelsProgress, MessageParsingProgress
 from .channel import parse_channel, extract_channels
 
 CHANNELS = settings.ENTRYPOINT_CHANNELS.split(",")
 
 
 async def parse_messages(
+    app: Client,
     channels: List[str] = CHANNELS,
 ) -> AsyncGenerator[MessageParsingProgress, None]:
-    channels: deque = deque(set(channels))
-    parsed_channels = set()
+    channels_queue: deque = deque(set(channels))
+    parsed_channels: Set[str] = set()
 
-    while channels:
-        channel = channels.popleft()
+    while channels_queue:
+        channel = channels_queue.popleft()
 
-        async for message in parse_channel(channel_name=channel):
+        async for message in parse_channel(app=app, channel_name=channel):
             if message.text is None and message.caption is None:
                 continue
 
-            yield MessageParsingProgress(message, len(parsed_channels), len(channels))
+            yield MessageParsingProgress(
+                message, len(parsed_channels), len(channels_queue)
+            )
 
             if not settings.AUTO_EXPLORE_CHANNELS:
                 continue
 
             linked_channels = extract_channels(message)
-            linked_channels = filter(
-                lambda x: x not in parsed_channels and x not in channels,
-                linked_channels,
+            linked_channels = list(
+                filter(
+                    lambda x: x not in parsed_channels and x not in channels_queue,
+                    linked_channels,
+                )
             )
 
             for linked_channel in linked_channels:
-                channels.append(linked_channel)
+                channels_queue.append(linked_channel)
 
         parsed_channels.add(channel)
 
 
 async def explore_channels(
+    app: Client,
     channels: List[str] = CHANNELS,
 ) -> AsyncGenerator[ExploreChannelsProgress, None]:
-    channels: deque = deque(set(channels))
+    channels_queue: deque = deque(set(channels))
     parsed_channels = set()
 
-    while channels:
-        channel = channels.popleft()
-
-        async for message in parse_channel(channel_name=channel):
+    while channels_queue:
+        channel = channels_queue.popleft()
+        channel_mentions = set()
+        async for message in parse_channel(app=app, channel_name=channel):
             linked_channels = extract_channels(message)
-            linked_channels = filter(
-                lambda x: x not in parsed_channels and x not in channels,
-                linked_channels,
+            linked_channels = list(
+                filter(
+                    lambda x: x not in parsed_channels and x not in channels_queue,
+                    linked_channels,
+                )
             )
 
+            if not linked_channels:
+                continue
+
             for linked_channel in linked_channels:
-                channels.append(linked_channel)
-                yield ExploreChannelsProgress(message=message, mentions=linked_channel)
+                channels_queue.append(linked_channel)
+                channel_mentions.add(linked_channel)
+
+        yield ExploreChannelsProgress(
+            source_channel=channel, mentions=list(channel_mentions)
+        )
 
         parsed_channels.add(channel)
 
 
-async def search_text(text: str) -> AsyncGenerator[Message, None]:
+async def search_text(app: Client, text: str) -> AsyncGenerator[Message, None]:
     """Search for text in messages"""
 
     with console.status("Working...") as status:
         n_parsed = 0
-        async for p in parse_messages(channels=CHANNELS):
+        async for p in parse_messages(app=app, channels=CHANNELS):
             m = p.message
 
             if n_parsed % 100 == 0:
                 status.update(
                     f"Parsed: {p.channels_parsed} ch. {n_parsed} messages  - remaining {p.channels_remaining} ch."  # noqa: E501
                     f" | Searching for word [bold]{text}[/bold] in {m.chat.username}"
                 )
@@ -91,22 +107,22 @@
                     )
                 )
                 yield m
 
             n_parsed += 1
 
 
-async def search_mentions(mention: str) -> AsyncGenerator[Message, None]:
+async def search_mentions(app: Client, mention: str) -> AsyncGenerator[Message, None]:
     """Search for mentions in messages"""
     if mention.startswith("@"):
         mention = mention[1:]
 
     with console.status("Working...") as status:
         n_parsed = 0
-        async for p in parse_messages(channels=CHANNELS):
+        async for p in parse_messages(app=app, channels=CHANNELS):
             m = p.message
 
             if n_parsed % 100 == 0:
                 status.update(
                     f"Parsed: {p.channels_parsed} ch. {n_parsed} messages  - remaining {p.channels_remaining} ch."  # noqa: E501
                     f" | Searching for mention of [bold]{mention}[/bold] in {m.chat.username}"
                 )
```

### Comparing `telespider-0.1.1/PKG-INFO` & `telespider-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telespider
-Version: 0.1.1
+Version: 0.2.0
 Summary: recursively parsing tg channels
 License: MIT
 Author: andrewsap
 Author-email: andrewsapw@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

