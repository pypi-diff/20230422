# Comparing `tmp/search_hound_ai-0.1.1.tar.gz` & `tmp/search_hound_ai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "search_hound_ai-0.1.1.tar", max compression
+gzip compressed data, was "search_hound_ai-0.1.4.tar", max compression
```

## Comparing `search_hound_ai-0.1.1.tar` & `search_hound_ai-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-04-21 15:10:20.825839 search_hound_ai-0.1.1/LICENSE
--rw-r--r--   0        0        0     1434 2023-04-21 15:10:20.825839 search_hound_ai-0.1.1/README.md
--rw-r--r--   0        0        0      431 2023-04-21 15:10:20.825839 search_hound_ai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1120 2023-04-21 15:10:20.825839 search_hound_ai-0.1.1/search_hound_ai/openai_lib.py
--rw-r--r--   0        0        0      424 2023-04-21 15:10:20.825839 search_hound_ai-0.1.1/search_hound_ai/search_hound_lib.py
--rw-r--r--   0        0        0     1937 1970-01-01 00:00:00.000000 search_hound_ai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-22 00:47:36.079460 search_hound_ai-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1434 2023-04-22 00:47:36.079460 search_hound_ai-0.1.4/README.md
+-rw-r--r--   0        0        0      541 2023-04-22 00:47:36.083461 search_hound_ai-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      504 2023-04-22 00:47:36.083461 search_hound_ai-0.1.4/search_hound_ai/__init__.py
+-rwxr-xr-x   0        0        0      530 2023-04-22 00:47:36.083461 search_hound_ai-0.1.4/search_hound_ai/app.py
+-rw-r--r--   0        0        0      369 2023-04-22 00:47:36.083461 search_hound_ai-0.1.4/search_hound_ai/app_test.py
+-rw-r--r--   0        0        0      392 2023-04-22 00:47:36.083461 search_hound_ai-0.1.4/search_hound_ai/hound_client_commands.py
+-rw-r--r--   0        0        0     1146 2023-04-22 00:47:36.083461 search_hound_ai-0.1.4/search_hound_ai/openai_lib.py
+-rw-r--r--   0        0        0      465 2023-04-22 00:47:36.083461 search_hound_ai-0.1.4/search_hound_ai/search_hound_lib.py
+-rw-r--r--   0        0        0     1902 1970-01-01 00:00:00.000000 search_hound_ai-0.1.4/PKG-INFO
```

### Comparing `search_hound_ai-0.1.1/LICENSE` & `search_hound_ai-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `search_hound_ai-0.1.1/README.md` & `search_hound_ai-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `search_hound_ai-0.1.1/search_hound_ai/openai_lib.py` & `search_hound_ai-0.1.4/search_hound_ai/openai_lib.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import typer
 from langchain.prompts import PromptTemplate
 from langchain.llms import OpenAI
 from langchain import LLMChain
 
+
 """
 This function takes in a question as input and uses OpenAI's language model to generate a response.
 
 Parameters:
 - question (str): The question to be searched.
 
 Returns:
@@ -17,15 +19,15 @@
 3. Create a prompt template using the input question and the template string.
 4. Initialize an LLMChain object with the language model and prompt template.
 5. Run the LLMChain object with the input question.
 6. Print the response generated by the LLMChain object.
 7. Return the response generated by the LLMChain object.
 """
 
-def OpenAISearch(question):
+def OpenAISearch(question: str) -> str:
     template = """Search: {question} """
     llm = OpenAI(temperature=0)
 
     prompt = PromptTemplate(
         input_variables=['question'],
         template=template,
     )
```

### Comparing `search_hound_ai-0.1.1/PKG-INFO` & `search_hound_ai-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: search-hound-ai
-Version: 0.1.1
+Version: 0.1.4
 Summary: 
-Author: thisguymartin
-Author-email: mpatino117@gmail.com
+Author: Martin Patino
+Author-email: martin@sibipro.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fire (>=0.5.0,<0.6.0)
-Requires-Dist: langchain (>=0.0.145,<0.0.146)
-Requires-Dist: logging (>=0.4.9.6,<0.5.0.0)
+Requires-Dist: langchain (>=0.0.146,<0.0.147)
+Requires-Dist: load-dotenv (>=0.1.0,<0.2.0)
 Requires-Dist: openai (>=0.27.4,<0.28.0)
-Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # SearchHoundAI
 
 
 This project aims to create an AI CLI tool that can execute AI-based commands via a command-line interface. The tool is designed to work on IOS, LINUX, and WINDOWS in .NET and can accept user inputs in the form of text, voice, or images. The tool is optimized for speed and performance and is easy to install and use with clear and concise documentation. The tool is also secure and regularly updated to address any security vulnerabilities.
```

