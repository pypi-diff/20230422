# Comparing `tmp/ws-cli-chat-0.1.0.tar.gz` & `tmp/ws_cli_chat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ws-cli-chat-0.1.0.tar", last modified: Sat Apr 22 06:20:17 2023, max compression
+gzip compressed data, was "ws_cli_chat-0.1.1.tar", max compression
```

## Comparing `ws-cli-chat-0.1.0.tar` & `ws_cli_chat-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,7 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 06:20:17.254504 ws-cli-chat-0.1.0/
--rw-rw-rw-   0        0        0     1094 2023-04-22 06:13:14.000000 ws-cli-chat-0.1.0/LICENCE
--rw-rw-rw-   0        0        0     1912 2023-04-22 06:20:17.254504 ws-cli-chat-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1553 2023-04-22 06:18:35.000000 ws-cli-chat-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 06:20:17.235358 ws-cli-chat-0.1.0/chat/
--rw-rw-rw-   0        0        0        0 2023-04-22 06:01:21.000000 ws-cli-chat-0.1.0/chat/__init__.py
--rw-rw-rw-   0        0        0       75 2023-04-22 06:01:21.000000 ws-cli-chat-0.1.0/chat/__main__.py
--rw-rw-rw-   0        0        0     1162 2023-04-22 06:01:21.000000 ws-cli-chat-0.1.0/chat/cli_chat.py
--rw-rw-rw-   0        0        0     1364 2023-04-22 06:01:21.000000 ws-cli-chat-0.1.0/chat/console.py
--rw-rw-rw-   0        0        0       42 2023-04-22 06:20:17.254504 ws-cli-chat-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-04-22 06:20:10.000000 ws-cli-chat-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 06:20:17.252504 ws-cli-chat-0.1.0/ws_cli_chat.egg-info/
--rw-rw-rw-   0        0        0     1912 2023-04-22 06:20:17.000000 ws-cli-chat-0.1.0/ws_cli_chat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-04-22 06:20:17.000000 ws-cli-chat-0.1.0/ws_cli_chat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 06:20:17.000000 ws-cli-chat-0.1.0/ws_cli_chat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-22 06:20:17.000000 ws-cli-chat-0.1.0/ws_cli_chat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-22 06:20:17.000000 ws-cli-chat-0.1.0/ws_cli_chat.egg-info/top_level.txt
+-rw-r--r--   0        0        0      516 2023-04-22 08:06:37.903046 ws_cli_chat-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1560 2023-04-22 08:02:07.727156 ws_cli_chat-0.1.1/README.md
+-rw-r--r--   0        0        0       39 2023-04-22 08:07:02.777152 ws_cli_chat-0.1.1/ws_cli_chat/__init__.py
+-rw-r--r--   0        0        0       75 2023-04-22 08:02:07.761667 ws_cli_chat-0.1.1/ws_cli_chat/__main__.py
+-rw-r--r--   0        0        0     1223 2023-04-22 08:04:21.778790 ws_cli_chat-0.1.1/ws_cli_chat/cli_chat.py
+-rw-r--r--   0        0        0     1364 2023-04-22 06:01:21.192473 ws_cli_chat-0.1.1/ws_cli_chat/console.py
+-rw-r--r--   0        0        0     2009 1970-01-01 00:00:00.000000 ws_cli_chat-0.1.1/PKG-INFO
```

### Comparing `ws-cli-chat-0.1.0/PKG-INFO` & `ws_cli_chat-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,49 @@
-Metadata-Version: 2.1
-Name: ws-cli-chat
-Version: 0.1.0
-Summary: simple cli-websocket-chat
-Home-page: https://github.com/MikalROn/WS-CLI-Chat
-Author: Daniel Coêlho
-Author-email: heromon.9010@gmail.com
-License: MIT license
-Keywords: pychat
-Platform: UNKNOWN
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-# Chat Application
-This is a command-line chat application built with Python that allows users to connect to a websocket server and chat with other users in real-time.
-
-# Requirements
-- Python 3.7+
-- websockets library
-- asyncio library
-
-# Installation
-To install the required libraries, run the following command in your terminal:
-````shell
-pip install websockets
-````
-Usage
-To start the application, run the following command in your terminal:
-
-````shell
-python chat
-````
-
-You will be prompted to choose a username. After entering your username, the application will connect to the websocket server and you will be able to chat with other users in real-time.
-
-To send a message, simply type your message and hit enter. Your message will be sent to all other users currently connected to the chat room.
-
-# Features
-- Real-time messaging: Messages are sent and received in real-time, allowing for seamless communication between users.
-- Multiple users: The chat room can accommodate multiple users at the same time, allowing for group conversations.
-- Usernames: Users can choose their own usernames, which are displayed alongside their messages in the chat room.
-- Clearing console: The console is cleared after each new message is received, making the chat experience cleaner.
-
-# Contributing
-Contributions are welcome! If you have any suggestions or feature requests, please open an issue or submit a pull request.
-
-# License
-This project is licensed under the MIT License. See the LICENSE file for more information.
-
+Metadata-Version: 2.1
+Name: ws-cli-chat
+Version: 0.1.1
+Summary: simple cli-websocket-ws-cli-chat
+Author: __coelho__
+Author-email: 109885900+MikalROn@users.noreply.github.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: websockets (>=11.0.2,<12.0.0)
+Description-Content-Type: text/markdown
+
+# Chat Application
+This is a command-line chat application built with Python that allows users to connect to a websocket server and chat with other users in real-time.
+
+# Requirements
+- Python 3.7+
+- websockets library
+- asyncio library
+
+# Installation
+To install the required libraries, run the following command in your terminal:
+````shell
+pip install websockets
+````
+Usage
+To start the application, run the following command in your terminal:
+
+````shell
+python ws_cli_chat
+````
+
+You will be prompted to choose a username. After entering your username, the application will connect to the websocket server and you will be able to chat with other users in real-time.
+
+To send a message, simply type your message and hit enter. Your message will be sent to all other users currently connected to the chat room.
+
+# Features
+- Real-time messaging: Messages are sent and received in real-time, allowing for seamless communication between users.
+- Multiple users: The chat room can accommodate multiple users at the same time, allowing for group conversations.
+- Usernames: Users can choose their own usernames, which are displayed alongside their messages in the chat room.
+- Clearing console: The console is cleared after each new message is received, making the chat experience cleaner.
+
+# Contributing
+Contributions are welcome! If you have any suggestions or feature requests, please open an issue or submit a pull request.
+
+# License
+This project is licensed under the MIT License. See the LICENSE file for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ws-cli-chat-0.1.0/README.md` & `ws_cli_chat-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ````shell
 pip install websockets
 ````
 Usage
 To start the application, run the following command in your terminal:
 
 ````shell
-python chat
+python ws_cli_chat
 ````
 
 You will be prompted to choose a username. After entering your username, the application will connect to the websocket server and you will be able to chat with other users in real-time.
 
 To send a message, simply type your message and hit enter. Your message will be sent to all other users currently connected to the chat room.
 
 # Features
```

### Comparing `ws-cli-chat-0.1.0/chat/cli_chat.py` & `ws_cli_chat-0.1.1/ws_cli_chat/cli_chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import threading
 import websockets
 import asyncio
-from console import Console
-
+import typer
+from ws_cli_chat.console import Console
 
+app = typer.Typer()
 MESSAGES: list[str] = []
 
 
 async def recive_message(socket) -> None:
     try:
         while True:
             msg: str = await socket.recv()
@@ -36,13 +37,14 @@
         async with websockets.connect(url) as socket:
             threading.Thread(target=send_message, args=(socket,)).start()
             await recive_message(socket)
     except KeyboardInterrupt:
         return None
 
 
+@app.command()
 def run_main():
     asyncio.run(main())
 
 
 if __name__ == '__main__':
     run_main()
```

### Comparing `ws-cli-chat-0.1.0/chat/console.py` & `ws_cli_chat-0.1.1/ws_cli_chat/console.py`

 * *Files identical despite different names*

