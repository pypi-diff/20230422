# Comparing `tmp/telespider-0.2.0.tar.gz` & `tmp/telespider-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telespider-0.2.0.tar", max compression
+gzip compressed data, was "telespider-0.2.1.tar", max compression
```

## Comparing `telespider-0.2.0.tar` & `telespider-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2023-04-20 08:10:29.039624 telespider-0.2.0/LICENSE
--rw-r--r--   0        0        0      934 2023-04-22 08:18:34.032173 telespider-0.2.0/README.md
--rw-r--r--   0        0        0      592 2023-04-22 08:50:39.059492 telespider-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       26 2023-04-17 17:49:13.844485 telespider-0.2.0/telespider/__init__.py
--rw-r--r--   0        0        0     2820 2023-04-22 08:48:07.464858 telespider-0.2.0/telespider/__main__.py
--rw-r--r--   0        0        0      305 2023-04-22 08:49:32.861777 telespider-0.2.0/telespider/app.py
--rw-r--r--   0        0        0      538 2023-04-19 16:12:02.069745 telespider-0.2.0/telespider/config.py
--rw-r--r--   0        0        0      152 2023-04-19 17:18:45.959480 telespider-0.2.0/telespider/console.py
--rw-r--r--   0        0        0       69 2023-04-22 08:06:36.213270 telespider-0.2.0/telespider/scrapper/__init__.py
--rw-r--r--   0        0        0     2095 2023-04-22 08:36:14.647055 telespider-0.2.0/telespider/scrapper/channel.py
--rw-r--r--   0        0        0     5417 2023-04-22 08:47:54.211309 telespider-0.2.0/telespider/scrapper/scrapper.py
--rw-r--r--   0        0        0      361 2023-04-22 08:47:20.048014 telespider-0.2.0/telespider/scrapper/types.py
--rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 telespider-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-20 08:10:29.039624 telespider-0.2.1/LICENSE
+-rw-r--r--   0        0        0      934 2023-04-22 08:18:34.032173 telespider-0.2.1/README.md
+-rw-r--r--   0        0        0      592 2023-04-22 09:12:52.400575 telespider-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-22 09:11:54.244843 telespider-0.2.1/telespider/__init__.py
+-rw-r--r--   0        0        0     2558 2023-04-22 09:11:08.352689 telespider-0.2.1/telespider/__main__.py
+-rw-r--r--   0        0        0     1653 2023-04-22 09:11:08.352689 telespider-0.2.1/telespider/app.py
+-rw-r--r--   0        0        0      538 2023-04-19 16:12:02.069745 telespider-0.2.1/telespider/config.py
+-rw-r--r--   0        0        0      152 2023-04-19 17:18:45.959480 telespider-0.2.1/telespider/console.py
+-rw-r--r--   0        0        0       69 2023-04-22 08:06:36.213270 telespider-0.2.1/telespider/scrapper/__init__.py
+-rw-r--r--   0        0        0     2095 2023-04-22 08:36:14.647055 telespider-0.2.1/telespider/scrapper/channel.py
+-rw-r--r--   0        0        0     5417 2023-04-22 08:47:54.211309 telespider-0.2.1/telespider/scrapper/scrapper.py
+-rw-r--r--   0        0        0      361 2023-04-22 08:47:20.048014 telespider-0.2.1/telespider/scrapper/types.py
+-rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 telespider-0.2.1/PKG-INFO
```

### Comparing `telespider-0.2.0/LICENSE` & `telespider-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telespider-0.2.0/README.md` & `telespider-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `telespider-0.2.0/pyproject.toml` & `telespider-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telespider"
-version = "0.2.0"
+version = "0.2.1"
 description = "recursively parsing tg channels"
 authors = ["andrewsap <andrewsapw@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `telespider-0.2.0/telespider/__main__.py` & `telespider-0.2.1/telespider/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from functools import wraps
 from typing import Optional
 import asyncio
 import uvloop
 
 import click
 
-from telespider import scrapper
 from telespider.config import settings, ROOT_DIR
 from telespider.app import App
 from telespider.console import console
 
 uvloop.install()
 
 
@@ -32,15 +31,15 @@
         name=settings.APP_NAME,
         api_id=settings.API_ID,
         api_hash=settings.API_HASH,
         workdir=workdir,
     )
     ctx.ensure_object(dict)
     ctx.obj["DEBUG"] = debug
-    ctx.obj["APP"] = app.app
+    ctx.obj["APP"] = app
 
 
 @cli.command(name="search", help="Search word or user mentions in channels messages")
 @click.option("--explore/--no-explore", default=True, help="Auto explore new channels")
 @click.option("--silent", is_flag=True, default=False, help="Suppress all output")
 @click.option("--word", "-w", type=str, required=False)
 @click.option("--user", "-u", type=str, required=False)
@@ -53,49 +52,41 @@
     ctx, explore: bool, silent: bool, word: Optional[str], user: Optional[str], n: int
 ):
     if word is None and user is None:
         raise click.BadOptionUsage(
             option_name="word | user", message="word or user must be specified"
         )
 
-    app = ctx.obj["APP"]
+    app: App = ctx.obj["APP"]
 
     settings.MAX_PER_CHANNEL = n
     settings.AUTO_EXPLORE_CHANNELS = explore
     console.quiet = silent
 
-    await app.start()
-    try:
-        if word is not None:
-            async for _ in scrapper.search_text(app=app, text=word):
-                ...
-        elif user is not None:
-            async for _ in scrapper.search_mentions(app=app, mention=user):
-                ...
-    finally:
-        await app.stop(block=False)
+    if word is not None:
+        async for _ in app.search_text(text=word):
+            ...
+    elif user is not None:
+        async for _ in app.search_mentions(mention=user):
+            ...
 
 
 @cli.command(name="explore-channels", help="Explore channels mentions")
 @click.option("--silent", is_flag=True, default=False, help="Suppress all output")
 @click.option(
     "-n", type=int, default=1000, help="Number of messages to parse per channel"
 )
 @click.pass_context
 @coro
 async def explore_channels(ctx, silent: bool, n: int):
     settings.MAX_PER_CHANNEL = n
     console.quiet = silent
 
-    app = ctx.obj["APP"]
+    app: App = ctx.obj["APP"]
 
-    await app.start()
-    try:
-        async for i in scrapper.explore_channels(app=app):
-            source_channel = i.source_channel
-            console.print(f"{source_channel}: {i.mentions}")
-    finally:
-        await app.stop(block=False)
+    async for i in app.explore_channels():
+        source_channel = i.source_channel
+        console.print(f"{source_channel}: {i.mentions}")
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `telespider-0.2.0/telespider/config.py` & `telespider-0.2.1/telespider/config.py`

 * *Files identical despite different names*

### Comparing `telespider-0.2.0/telespider/scrapper/channel.py` & `telespider-0.2.1/telespider/scrapper/channel.py`

 * *Files identical despite different names*

### Comparing `telespider-0.2.0/telespider/scrapper/scrapper.py` & `telespider-0.2.1/telespider/scrapper/scrapper.py`

 * *Files identical despite different names*

### Comparing `telespider-0.2.0/PKG-INFO` & `telespider-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telespider
-Version: 0.2.0
+Version: 0.2.1
 Summary: recursively parsing tg channels
 License: MIT
 Author: andrewsap
 Author-email: andrewsapw@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

