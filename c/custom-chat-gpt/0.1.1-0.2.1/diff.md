# Comparing `tmp/custom_chat_gpt-0.1.1.tar.gz` & `tmp/custom_chat_gpt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_chat_gpt-0.1.1.tar", max compression
+gzip compressed data, was "custom_chat_gpt-0.2.1.tar", max compression
```

## Comparing `custom_chat_gpt-0.1.1.tar` & `custom_chat_gpt-0.2.1.tar`

### file list

```diff
@@ -1,4 +1,10 @@
--rw-r--r--   0        0        0      221 2023-03-06 13:20:03.030511 custom_chat_gpt-0.1.1/README.md
--rw-r--r--   0        0        0     1681 2023-03-06 13:20:03.030511 custom_chat_gpt-0.1.1/chat_gpt/main.py
--rw-r--r--   0        0        0      454 2023-03-06 13:31:32.182205 custom_chat_gpt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 custom_chat_gpt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      221 2023-04-22 14:51:31.930390 custom_chat_gpt-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 16:59:59.393190 custom_chat_gpt-0.2.1/chat_gpt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 16:59:59.393439 custom_chat_gpt-0.2.1/chat_gpt/commands/__init__.py
+-rw-r--r--   0        0        0     1320 2023-04-22 16:59:59.393747 custom_chat_gpt-0.2.1/chat_gpt/commands/chat.py
+-rw-r--r--   0        0        0     3487 2023-04-22 16:59:59.394031 custom_chat_gpt-0.2.1/chat_gpt/commands/youtube.py
+-rw-r--r--   0        0        0     1385 2023-04-22 16:59:59.394326 custom_chat_gpt-0.2.1/chat_gpt/main.py
+-rw-r--r--   0        0        0        0 2023-04-22 16:59:59.394382 custom_chat_gpt-0.2.1/chat_gpt/utils/__init__.py
+-rw-r--r--   0        0        0      709 2023-04-22 16:59:59.394662 custom_chat_gpt-0.2.1/chat_gpt/utils/callbacks.py
+-rw-r--r--   0        0        0      635 2023-04-22 16:59:59.398993 custom_chat_gpt-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 custom_chat_gpt-0.2.1/PKG-INFO
```

### Comparing `custom_chat_gpt-0.1.1/PKG-INFO` & `custom_chat_gpt-0.2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: custom-chat-gpt
-Version: 0.1.1
+Version: 0.2.1
 Summary: Use chapgpt from your terminal
 Author: RomainEconomics
 Author-email: jouhameau.romain@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: chromadb (>=0.3.21,<0.4.0)
+Requires-Dist: faiss-cpu (>=1.7.3,<2.0.0)
+Requires-Dist: langchain (>=0.0.146,<0.0.147)
 Requires-Dist: openai (>=0.27.0,<0.28.0)
 Requires-Dist: rich (>=13.3,<14.0)
+Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: youtube-transcript-api (>=0.6.0,<0.7.0)
 Description-Content-Type: text/markdown
 
 # To install chat-gpt inside your terminal 
 
 ```
 pip install custom-chat-gpt
 ```
```

