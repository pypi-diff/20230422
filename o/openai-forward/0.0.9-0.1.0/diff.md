# Comparing `tmp/openai_forward-0.0.9.tar.gz` & `tmp/openai_forward-0.1.0.tar.gz`

## Comparing `openai_forward-0.0.9.tar` & `openai_forward-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/__init__.py
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/__main__.py
--rwxr-xr-x   0        0        0     5672 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/_base.py
--rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/app.py
--rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/config.py
--rwxr-xr-x   0        0        0      729 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/openai.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/routers/__init__.py
--rwxr-xr-x   0        0        0      490 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/routers/openai_v1.py
--rwxr-xr-x   0        0        0     2316 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/routers/schemas.py
--rwxr-xr-x   0        0        0     1869 2020-02-02 00:00:00.000000 openai_forward-0.0.9/.gitignore
--rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.0.9/LICENSE
--rwxr-xr-x   0        0        0     5755 2020-02-02 00:00:00.000000 openai_forward-0.0.9/README.md
--rwxr-xr-x   0        0        0     1562 2020-02-02 00:00:00.000000 openai_forward-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     6942 2020-02-02 00:00:00.000000 openai_forward-0.0.9/PKG-INFO
+-rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/__init__.py
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/__main__.py
+-rwxr-xr-x   0        0        0     3101 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/_base.py
+-rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/app.py
+-rwxr-xr-x   0        0        0     2611 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/config.py
+-rwxr-xr-x   0        0        0      808 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/openai.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/content/__init__.py
+-rwxr-xr-x   0        0        0     3327 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/content/chat.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/content/image.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/routers/__init__.py
+-rwxr-xr-x   0        0        0      490 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/routers/openai_v1.py
+-rwxr-xr-x   0        0        0     2316 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/routers/schemas.py
+-rwxr-xr-x   0        0        0     1882 2020-02-02 00:00:00.000000 openai_forward-0.1.0/.gitignore
+-rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.0/LICENSE
+-rwxr-xr-x   0        0        0     5470 2020-02-02 00:00:00.000000 openai_forward-0.1.0/README.md
+-rwxr-xr-x   0        0        0     1635 2020-02-02 00:00:00.000000 openai_forward-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 openai_forward-0.1.0/PKG-INFO
```

### Comparing `openai_forward-0.0.9/openai_forward/app.py` & `openai_forward-0.1.0/openai_forward/app.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.0.9/openai_forward/openai.py` & `openai_forward-0.1.0/openai_forward/openai.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from ._base import OpenaiBase
 from .routers.schemas import OpenAIV1ChatCompletion
 from fastapi import Request, HTTPException, status
+from .config import setting_log
+
+setting_log(log_name="openai_forward.log")
 
 
 class Openai(OpenaiBase):
     def __init__(self):
         self.validate_host = False
 
     async def reverse_proxy(self, request: Request):
```

### Comparing `openai_forward-0.0.9/openai_forward/routers/schemas.py` & `openai_forward-0.1.0/openai_forward/routers/schemas.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.0.9/.gitignore` & `openai_forward-0.1.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .vscode/
 third-party/
 run.sh
 ssl/
 chat.yaml
 chat_*.yaml
 
+.env.example
 Log/
 dist/
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
```

### Comparing `openai_forward-0.0.9/LICENSE` & `openai_forward-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.0.9/README.md` & `openai_forward-0.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,155 +1,171 @@
-**中文** | [**English**](./README_EN.md)
+Metadata-Version: 2.1
+Name: openai_forward
+Version: 0.1.0
+Summary: 🚀 Openai api forward · OpenAI 接口转发服务 · streaming forward
+Project-URL: Homepage, https://github.com/beidongjiedeguang/openai-forward
+Project-URL: Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-forward
+Project-URL: Issues, https://github.com/beidongjiedeguang/openai-forward/issues
+Project-URL: Source, https://github.com/beidongjiedeguang/openai-forward
+Author-email: kunyuan <beidongjiedeguang@gmail.com>
+License-File: LICENSE
+Keywords: chatgpt,fastapi,forward,openai,openai-api,openai-proxy,python,streaming-api
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Requires-Dist: fastapi
+Requires-Dist: httpx
+Requires-Dist: loguru
+Requires-Dist: orjson
+Requires-Dist: python-dotenv
+Requires-Dist: sparrow-python>=0.1.1
+Requires-Dist: uvicorn
+Provides-Extra: bard
+Requires-Dist: googlebard; extra == 'bard'
+Provides-Extra: chatgpt
+Requires-Dist: revchatgpt; extra == 'chatgpt'
+Provides-Extra: edge
+Requires-Dist: edgegpt; extra == 'edge'
+Provides-Extra: ssl
+Requires-Dist: certbot; extra == 'ssl'
+Description-Content-Type: text/markdown
+
+[**中文**](./README_ZH.md) | **English**
 
 <h1 align="center">
     <br>
     OpenAI Forward
     <br>
 </h1>
 <p align="center">
     <b> OpenAI API 接口转发服务 <br/>
     The fastest way to deploy openai api forward proxy </b>
 </p>
 
-[//]: # (    <a href="https://github.com/beidongjiedeguang">)
-[//]: # (        <img alt="name" src="https://img.shields.io/badge/author-@kunyuan-orange.svg?style=flat-square&logo=appveyor">)
-[//]: # (    </a>)
-[//]: # (    <a href="https://github.com/beidongjiedeguang/openai-forward/stargazers">)
-[//]: # (        <img alt="starts" src=https://img.shields.io/github/stars/beidongjiedeguang/openai-forward?style=social>)
-[//]: # (    </a>)
-[//]: # ([![Downloads]&#40;https://static.pepy.tech/badge/openai-forward/month&#41;]&#40;https://pepy.tech/project/openai-forward&#41;)
-[//]: # (    <a href="https://codecov.io/gh/beidongjiedeguang/openai-forward">)
-[//]: # (        <img alt="codecov" src="https://codecov.io/gh/beidongjiedeguang/openai-forward/branch/dev/graph/badge.svg">)
-[//]: # (    </a>)
-
 <p align="center">
-<a href="https://badge.fury.io/py/openai-forward"><img src="https://badge.fury.io/py/openai-forward.svg" alt="PyPI version" ></a>
+    <a href="https://pypi.org/project/openai-forward/"><img src="https://img.shields.io/pypi/v/openai-forward?color=brightgreen" alt="PyPI version" ></a>
     <a href="https://github.com/beidongjiedeguang/openai-forward/blob/main/LICENSE">
         <img alt="License" src="https://img.shields.io/github/license/beidongjiedeguang/openai-forward.svg?color=blue&style=flat-square">
     </a>
     <a href="https://github.com/beidongjiedeguang/openai-forward/releases">
         <img alt="Release (latest by date)" src="https://img.shields.io/github/v/release/beidongjiedeguang/openai-forward">
     </a>
     <a href="https://github.com/beidongjiedeguang/openai-forward">
         <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/beidongjiedeguang/openai-forward">
     </a>
-    <a href="https://github.com/beidongjiedeguang/openai-forward/">
-        <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/beidongjiedeguang/openai-forward">
+    <a href="https://hub.docker.com/r/beidongjiedeguang/openai-forward">
+        <img alt="docer image size" src="https://img.shields.io/docker/image-size/beidongjiedeguang/openai-forward?style=flat&label=docker image">
     </a>
     <a href="https://github.com/beidongjiedeguang/openai-forward/actions/workflows/run_tests.yaml">
         <img alt="tests" src="https://img.shields.io/github/actions/workflow/status/beidongjiedeguang/openai-forward/run_tests.yml?label=tests">
     </a>
     <a href="https://pypi.org/project/openai_forward/">
         <img alt="pypi downloads" src="https://img.shields.io/pypi/dm/openai_forward">
     </a>
 
 </p>
+This project is designed to solve the problem of some regions being unable to directly access OpenAI. The service is deployed on a server that can access the OpenAI API, and OpenAI requests are forwarded through the service, i.e. a reverse proxy service is set up. 
 
+Test access: https://caloi.top/v1/chat/completions is equivalent to https://api.openai.com/v1/chat/completions 
 
+# Table of Contents 
 
-本项目用于解决一些地区无法直接访问OpenAI的问题，将该服务部署在可以正常访问openai api的服务器上，通过该服务转发OpenAI的请求。即搭建反向代理服务  
-测试访问：https://caloi.top/v1/chat/completions 将等价于 https://api.openai.com/v1/chat/completions
-
-# Table of Contents
+- [Features](#Features) 
+- [Usage](#Usage) 
+- [Service Deployment](#Service-Deployment) 
+- [Service Usage](#Service Usage) 
+
+# Features 
+- [x] Supports forwarding of all OpenAI interfaces 
+- [x] Supports request IP verification 
+- [x] Supports streaming forwarding 
+- [x] Supports default API key 
+- [x] pip installation and deployment 
+- [x] Docker deployment 
+- [ ] Chat content security: Chat content streaming filtering 
 
-- [Features](#Features)
-- [Usage](#Usage)
-- [服务部署](#安装部署)
-- [服务调用](#服务调用)
-
-
-# Features
-- [x] 支持转发OpenAI所有接口
-- [x] 请求IP验证
-- [x] 支持流式转发
-- [x] 支持默认api key
-- [x] pip安装
-- [x] docker部署
-- [x] 自定义转发端口
-- [ ] 自定义转发路由
-- [ ] 聊天内容安全：聊天内容流式过滤
-
-# Usage
-> 这里以个人搭建好的代理地址 https://caloi.top 为例
- 
-### [chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web)
-修改 [Docker Compose](https://github.com/Chanzhaoyu/chatgpt-web#docker-compose) 中的`OPENAI_API_BASE_URL`为我们搭建的代理服务地址:
-```bash
-OPENAI_API_BASE_URL: https://caloi.top 
-```
-
-### [ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)
-替换docker启动命令中的 `BASE_URL`为我们搭建的代理服务地址
-```bash
-docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-xxx" -e CODE="<your password>" -e BASE_URL="caloi.top" yidadaa/chatgpt-next-web
-```
+# Usage 
+> Here, the proxy address set up by the individual, https://caloi.top, is used as an example 
 
 ### Image Generation (DALL-E):
-```bash
-curl --location 'https://caloi.top/v1/images/generations' \
---header 'Authorization: Bearer sk-***[OUR_API_KEY]***' \
---header 'Content-Type: application/json' \
---data '{
-    "prompt": "A photo of a cat",
-    "n": 1,
-    "size": "512x512",
-}'
-```
-
-### 在模块中使用
-
-**Used in JS/TS**
-```typescript
-import { Configuration } from "openai";
-
-const configuration = new Configuration({
-    basePath: "https://caloi.top",
-    apiKey: "sk-******",
-    
-});
-```
-**Used in Python**  
-```python
-import openai
-openai.api_base = "https://caloi.top"
-openai.api_key = "sk-******"
-```
-
-# 服务部署
-提供两种服务部署方式,选择一种即可
-
-## 方式一:  pip
-**安装**
-```bash
-pip install openai-forward
-```
-**运行转发服务**  
-可通过`--port`指定端口号，默认为`8000`，可通过`--workers`指定工作进程数，默认为`1`
-```bash
-openai_forward run --port=9999 --workers=1
-```
-服务就搭建完成了，使用方式只需将`https://api.openai.com` 替换为服务所在端口`http://{ip}:{port}` 即可。  
-
-当然也可以将 OPENAI_API_KEY 作为环境变量传入作为默认api key， 这样客户端在请求相关路由时可以无需在Header中传入Authorization。
-带默认api key的启动方式：
-```bash
-OPENAI_API_KEY="sk-xxx" openai_forward run --port=9999 --workers=1
-```
-注: 如果既存在默认api key又在请求头中传入了api key，则以请求头中的api key会覆盖默认api key.
+```bash 
+curl --location 'https://caloi.top/v1/images/generations' \ 
+--header 'Authorization: Bearer sk-******' \ 
+--header 'Content-Type: application/json' \ 
+--data '{ 
+    "prompt": "A photo of a cat", 
+    "n": 1, 
+    "size": "512x512"
+}' 
+``` 
+
+### [chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web) 
+Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/Chanzhaoyu/chatgpt-web#docker-compose) to the address of the proxy service we set up: 
+```bash 
+OPENAI_API_BASE_URL: https://caloi.top 
+``` 
 
+### [ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web) 
+Replace `BASE_URL` in the docker startup command with the address of the proxy service we set up: 
+```bash 
+docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="<your password>" -e BASE_URL="caloi.top" yidadaa/chatgpt-next-web 
+``` 
+
+
+### Using in a module 
+
+**Used in JS/TS** 
+```typescript 
+import { Configuration } from "openai"; 
+
+const configuration = new Configuration({ 
+    basePath: "https://caloi.top", 
+    apiKey: "sk-******", 
+
+}); 
+``` 
+**Used in Python** 
+```python 
+import openai 
+openai.api_base = "https://caloi.top" 
+openai.api_key = "sk-******" 
+``` 
+
+# Service Deployment 
+Two service deployment methods are provided, choose one 
+
+## Method 1: pip 
+**Installation** 
+```bash 
+pip install openai-forward 
+``` 
+**Run forwarding service** 
+The port number can be specified through `--port`, which defaults to `8000`, and the number of worker processes can be specified through `--workers`, which defaults to `1`. 
+```bash 
+openai_forward run --port=9999 --workers=1 
+``` 
+The service is now set up, and the usage is to replace `https://api.openai.com` with the port number of the service `http://{ip}:{port}`. 
+
+Of course, OPENAI_API_KEY can also be passed in as an environment variable as the default API key, so that the client does not need to pass in the Authorization in the header when requesting the relevant route. 
+Startup command with default API key: 
+```bash 
+OPENAI_API_KEY="sk-xxx" openai_forward run --port=9999 --workers=1 
+``` 
+Note: If both the default API key and the API key passed in the request header exist, the API key in the request header will override the default API key. 
 
-## 方式二: Docker(推荐) 
-```bash
+## Method 2: Docker (recommended) 
+```bash 
 docker run --name="openai-forward" -d -p 9999:8000 beidongjiedeguang/openai-forward:latest 
-```
-将映射宿主机的9999端口，通过`http://{ip}:9999`访问服务。  
-注：同样可以在启动命令中通过-e传入环境变量OPENAI_API_KEY=sk-xxx作为默认api key
-
-# 服务调用
-替换openai的api地址为该服务的地址即可，如：
-```bash
-https://api.openai.com/v1/chat/completions
-```
-替换为
-```bash
-http://{ip}:{port}/v1/chat/completions
+``` 
+The 9999 port of the host is mapped, and the service can be accessed through `http://{ip}:9999`. 
+Note: You can also pass in the environment variable OPENAI_API_KEY=sk-xxx as the default API key in the startup command. 
+
+# Service Usage 
+Simply replace the OpenAI API address with the address of the service we set up, such as: 
+```bash 
+https://api.openai.com/v1/chat/completions 
+``` 
+Replace with 
+```bash 
+http://{ip}:{port}/v1/chat/completions 
 ```
```

### Comparing `openai_forward-0.0.9/pyproject.toml` & `openai_forward-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openai_forward"
-description = ""
+description = "🚀 Openai api forward · OpenAI 接口转发服务 · streaming forward"
 authors = [
     { name = "kunyuan", email = "beidongjiedeguang@gmail.com" },
 ]
 requires-python = ">=3.6"
 readme = "README.md"
 keywords = ["openai", "chatgpt", "openai-api", "openai-proxy", "forward", "streaming-api", "fastapi", "python"]
 classifiers = [
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

