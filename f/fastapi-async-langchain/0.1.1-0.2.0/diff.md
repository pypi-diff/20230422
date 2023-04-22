# Comparing `tmp/fastapi_async_langchain-0.1.1.tar.gz` & `tmp/fastapi_async_langchain-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_async_langchain-0.1.1.tar", max compression
+gzip compressed data, was "fastapi_async_langchain-0.2.0.tar", max compression
```

## Comparing `fastapi_async_langchain-0.1.1.tar` & `fastapi_async_langchain-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-04-22 07:29:58.832117 fastapi_async_langchain-0.1.1/LICENSE
--rw-r--r--   0        0        0     1574 2023-04-22 07:29:58.832117 fastapi_async_langchain-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-22 07:29:58.840117 fastapi_async_langchain-0.1.1/fastapi_async_langchain/__init__.py
--rw-r--r--   0        0        0      648 2023-04-22 07:29:58.840117 fastapi_async_langchain-0.1.1/fastapi_async_langchain/callback.py
--rw-r--r--   0        0        0     2457 2023-04-22 07:29:58.840117 fastapi_async_langchain-0.1.1/fastapi_async_langchain/response.py
--rw-r--r--   0        0        0      481 2023-04-22 07:29:58.840117 fastapi_async_langchain-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2139 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-22 19:56:23.738974 fastapi_async_langchain-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1574 2023-04-22 19:56:23.738974 fastapi_async_langchain-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 19:56:23.742974 fastapi_async_langchain-0.2.0/fastapi_async_langchain/__init__.py
+-rw-r--r--   0        0        0      648 2023-04-22 19:56:23.742974 fastapi_async_langchain-0.2.0/fastapi_async_langchain/callback.py
+-rw-r--r--   0        0        0     2511 2023-04-22 19:56:23.742974 fastapi_async_langchain-0.2.0/fastapi_async_langchain/response.py
+-rw-r--r--   0        0        0      481 2023-04-22 19:56:23.742974 fastapi_async_langchain-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2139 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.2.0/PKG-INFO
```

### Comparing `fastapi_async_langchain-0.1.1/LICENSE` & `fastapi_async_langchain-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.1.1/README.md` & `fastapi_async_langchain-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.1.1/fastapi_async_langchain/callback.py` & `fastapi_async_langchain-0.2.0/fastapi_async_langchain/callback.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.1.1/fastapi_async_langchain/response.py` & `fastapi_async_langchain-0.2.0/fastapi_async_langchain/response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from functools import partial
 from typing import Any, Dict, Union
 
 from fastapi.responses import StreamingResponse
 from langchain import LLMChain
 from langchain.callbacks import AsyncCallbackManager
 from starlette.types import Send
 
@@ -28,15 +29,15 @@
                 for handler in chain.llm.callback_manager.handlers:
                     if isinstance(handler, AsyncFastApiStreamingCallback):
                         chain.llm.callback_manager.remove_handler(handler)
                         break
                 chain.llm.callback_manager.add_handler(
                     AsyncFastApiStreamingCallback(send=send)
                 )
-                await chain.arun(inputs)
+                return await chain.arun(inputs)
 
             return wrapper
 
         self.chain_wrapper_fn = chain_wrapper_fn(chain, inputs)
 
     async def stream_response(self, send: Send) -> None:
         await send(
@@ -48,17 +49,18 @@
         )
 
         async def send_token(token: Union[str, bytes]):
             if not isinstance(token, bytes):
                 token = token.encode(self.charset)
             await send({"type": "http.response.body", "body": token, "more_body": True})
 
-        # suggested in https://github.com/hwchase17/langchain/discussions/1706#discussioncomment-5576099
         try:
-            await self.chain_wrapper_fn(send_token)
+            outputs = await self.chain_wrapper_fn(send_token)
+            if self.background is not None:
+                self.background = partial(self.background, outputs)
         except Exception as e:
             await send(
                 {
                     "type": "http.response.body",
                     "body": str(e).encode(self.charset),
                     "more_body": False,
                 }
```

### Comparing `fastapi_async_langchain-0.1.1/PKG-INFO` & `fastapi_async_langchain-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-async-langchain
-Version: 0.1.1
+Version: 0.2.0
 Summary: FastAPI async components for streaming LLM chains.
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

