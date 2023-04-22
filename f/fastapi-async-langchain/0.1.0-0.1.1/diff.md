# Comparing `tmp/fastapi_async_langchain-0.1.0.tar.gz` & `tmp/fastapi_async_langchain-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_async_langchain-0.1.0.tar", max compression
+gzip compressed data, was "fastapi_async_langchain-0.1.1.tar", max compression
```

## Comparing `fastapi_async_langchain-0.1.0.tar` & `fastapi_async_langchain-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-04-20 09:14:06.830428 fastapi_async_langchain-0.1.0/LICENSE
--rw-r--r--   0        0        0     1574 2023-04-20 09:14:06.830428 fastapi_async_langchain-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-20 09:14:06.834428 fastapi_async_langchain-0.1.0/fastapi_async_langchain/__init__.py
--rw-r--r--   0        0        0      648 2023-04-20 09:14:06.834428 fastapi_async_langchain-0.1.0/fastapi_async_langchain/callback.py
--rw-r--r--   0        0        0     2190 2023-04-20 09:14:06.834428 fastapi_async_langchain-0.1.0/fastapi_async_langchain/response.py
--rw-r--r--   0        0        0      481 2023-04-20 09:14:06.834428 fastapi_async_langchain-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2139 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-22 07:29:58.832117 fastapi_async_langchain-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1574 2023-04-22 07:29:58.832117 fastapi_async_langchain-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 07:29:58.840117 fastapi_async_langchain-0.1.1/fastapi_async_langchain/__init__.py
+-rw-r--r--   0        0        0      648 2023-04-22 07:29:58.840117 fastapi_async_langchain-0.1.1/fastapi_async_langchain/callback.py
+-rw-r--r--   0        0        0     2457 2023-04-22 07:29:58.840117 fastapi_async_langchain-0.1.1/fastapi_async_langchain/response.py
+-rw-r--r--   0        0        0      481 2023-04-22 07:29:58.840117 fastapi_async_langchain-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2139 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.1.1/PKG-INFO
```

### Comparing `fastapi_async_langchain-0.1.0/LICENSE` & `fastapi_async_langchain-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.1.0/README.md` & `fastapi_async_langchain-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.1.0/fastapi_async_langchain/callback.py` & `fastapi_async_langchain-0.1.1/fastapi_async_langchain/callback.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.1.0/fastapi_async_langchain/response.py` & `fastapi_async_langchain-0.1.1/fastapi_async_langchain/response.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 
         def chain_wrapper_fn(chain: LLMChain, inputs: Union[Dict[str, Any], Any]):
             async def wrapper(send: Send):
                 if not isinstance(chain.llm.callback_manager, AsyncCallbackManager):
                     raise TypeError(
                         "llm.callback_manager must be an instance of AsyncCallbackManager"
                     )
+                for handler in chain.llm.callback_manager.handlers:
+                    if isinstance(handler, AsyncFastApiStreamingCallback):
+                        chain.llm.callback_manager.remove_handler(handler)
+                        break
                 chain.llm.callback_manager.add_handler(
                     AsyncFastApiStreamingCallback(send=send)
                 )
                 await chain.arun(inputs)
 
             return wrapper
 
@@ -55,9 +59,10 @@
             await send(
                 {
                     "type": "http.response.body",
                     "body": str(e).encode(self.charset),
                     "more_body": False,
                 }
             )
+            return
 
         await send({"type": "http.response.body", "body": b"", "more_body": False})
```

### Comparing `fastapi_async_langchain-0.1.0/PKG-INFO` & `fastapi_async_langchain-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-async-langchain
-Version: 0.1.0
+Version: 0.1.1
 Summary: FastAPI async components for streaming LLM chains.
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

