# Comparing `tmp/custom_chat_gpt-0.2.1.tar.gz` & `tmp/custom_chat_gpt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_chat_gpt-0.2.1.tar", max compression
+gzip compressed data, was "custom_chat_gpt-0.2.2.tar", max compression
```

## Comparing `custom_chat_gpt-0.2.1.tar` & `custom_chat_gpt-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      221 2023-04-22 14:51:31.930390 custom_chat_gpt-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-04-22 16:59:59.393190 custom_chat_gpt-0.2.1/chat_gpt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 16:59:59.393439 custom_chat_gpt-0.2.1/chat_gpt/commands/__init__.py
--rw-r--r--   0        0        0     1320 2023-04-22 16:59:59.393747 custom_chat_gpt-0.2.1/chat_gpt/commands/chat.py
--rw-r--r--   0        0        0     3487 2023-04-22 16:59:59.394031 custom_chat_gpt-0.2.1/chat_gpt/commands/youtube.py
--rw-r--r--   0        0        0     1385 2023-04-22 16:59:59.394326 custom_chat_gpt-0.2.1/chat_gpt/main.py
--rw-r--r--   0        0        0        0 2023-04-22 16:59:59.394382 custom_chat_gpt-0.2.1/chat_gpt/utils/__init__.py
--rw-r--r--   0        0        0      709 2023-04-22 16:59:59.394662 custom_chat_gpt-0.2.1/chat_gpt/utils/callbacks.py
--rw-r--r--   0        0        0      635 2023-04-22 16:59:59.398993 custom_chat_gpt-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 custom_chat_gpt-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      221 2023-04-22 14:51:31.930390 custom_chat_gpt-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 16:59:59.393190 custom_chat_gpt-0.2.2/chat_gpt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 16:59:59.393439 custom_chat_gpt-0.2.2/chat_gpt/commands/__init__.py
+-rw-r--r--   0        0        0     1320 2023-04-22 17:06:55.759659 custom_chat_gpt-0.2.2/chat_gpt/commands/chat.py
+-rw-r--r--   0        0        0     3267 2023-04-22 17:06:55.759966 custom_chat_gpt-0.2.2/chat_gpt/commands/youtube.py
+-rw-r--r--   0        0        0     1385 2023-04-22 16:59:59.394326 custom_chat_gpt-0.2.2/chat_gpt/main.py
+-rw-r--r--   0        0        0        0 2023-04-22 16:59:59.394382 custom_chat_gpt-0.2.2/chat_gpt/utils/__init__.py
+-rw-r--r--   0        0        0      709 2023-04-22 16:59:59.394662 custom_chat_gpt-0.2.2/chat_gpt/utils/callbacks.py
+-rw-r--r--   0        0        0      635 2023-04-22 17:07:24.914852 custom_chat_gpt-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 custom_chat_gpt-0.2.2/PKG-INFO
```

### Comparing `custom_chat_gpt-0.2.1/chat_gpt/commands/chat.py` & `custom_chat_gpt-0.2.2/chat_gpt/commands/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,17 @@
     console = Console()
 
     messages: list[BaseMessage] = [
         SystemMessage(content="You’re a helpful programming assistant. Answers the questions as a professional programmer."),
     ]
 
     console.print("Starting a chat ...")
-
+    console.print()
+    
     while True:
-        console.print()
         content = Prompt.ask("[red][b]User [b/]")
         console.print()
         messages.append(HumanMessage(content=content))
 
         stream_manager = CallbackManager(
             [StreamingTerminalCallbackHandler(output_callback= lambda x: rich_streaming_display(x, live_chat))]
         )
```

### Comparing `custom_chat_gpt-0.2.1/chat_gpt/commands/youtube.py` & `custom_chat_gpt-0.2.2/chat_gpt/commands/youtube.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,22 @@
-import sys
+
 from langchain.document_loaders import YoutubeLoader
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.vectorstores import FAISS
 from langchain.chat_models import ChatOpenAI
 from langchain import PromptTemplate
 from langchain.chains import LLMChain
 from rich.console import Console
-from rich.markdown import Markdown
 from rich.live import Live
-from langchain.schema import (
-    HumanMessage,
-    SystemMessage,
-    BaseMessage
-)
 from rich.prompt import Prompt
 
 from typing import Any
 from rich.live import Live
 from langchain.callbacks import CallbackManager
-from langchain.schema import (
-    HumanMessage,
-    SystemMessage,
-    BaseMessage
-)
 from chat_gpt.utils.callbacks import StreamingTerminalCallbackHandler, rich_streaming_display
 
 
 
 def create_db_from_youtube_video_url(url: str, language: str, console: Console) -> FAISS:
     embeddings = OpenAIEmbeddings()
 
@@ -93,12 +82,12 @@
 
     #video_url = "https://www.youtube.com/watch?v=NYSWn1ipbgg" "https://www.youtube.com/watch?v=L_Guz73e6fw"
     db = create_db_from_youtube_video_url(url, language, console)
 
     console.print("[green]You can now ask questions about the video's transcript.\n")
 
     while True:
-        content = Prompt.ask("[red][b]User [b/]: ")
+        content = Prompt.ask("[red][b]User[b/]")
         console.print()
 
         response, docs = get_response_from_query(db, content, k=5, console=console)
         console.print()
```

### Comparing `custom_chat_gpt-0.2.1/chat_gpt/main.py` & `custom_chat_gpt-0.2.2/chat_gpt/main.py`

 * *Files identical despite different names*

### Comparing `custom_chat_gpt-0.2.1/chat_gpt/utils/callbacks.py` & `custom_chat_gpt-0.2.2/chat_gpt/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `custom_chat_gpt-0.2.1/pyproject.toml` & `custom_chat_gpt-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "custom-chat-gpt"
-version = "0.2.1"
+version = "0.2.2"
 description = "Use chapgpt from your terminal"
 authors = ["RomainEconomics <jouhameau.romain@gmail.com>"]
 readme = "README.md"
 packages = [{include = "chat_gpt"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `custom_chat_gpt-0.2.1/PKG-INFO` & `custom_chat_gpt-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-chat-gpt
-Version: 0.2.1
+Version: 0.2.2
 Summary: Use chapgpt from your terminal
 Author: RomainEconomics
 Author-email: jouhameau.romain@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

