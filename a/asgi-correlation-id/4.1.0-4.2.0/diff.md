# Comparing `tmp/asgi_correlation_id-4.1.0.tar.gz` & `tmp/asgi_correlation_id-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgi_correlation_id-4.1.0.tar", max compression
+gzip compressed data, was "asgi_correlation_id-4.2.0.tar", max compression
```

## Comparing `asgi_correlation_id-4.1.0.tar` & `asgi_correlation_id-4.2.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1672 2023-02-24 16:09:42.665838 asgi_correlation_id-4.1.0/LICENSE
--rw-r--r--   0        0        0    22788 2023-02-24 16:09:42.665838 asgi_correlation_id-4.1.0/README.md
--rw-r--r--   0        0        0      421 2023-02-24 16:09:42.665838 asgi_correlation_id-4.1.0/asgi_correlation_id/__init__.py
--rw-r--r--   0        0        0      362 2023-02-24 16:09:42.665838 asgi_correlation_id-4.1.0/asgi_correlation_id/context.py
--rw-r--r--   0        0        0        0 2023-02-24 16:09:42.665838 asgi_correlation_id-4.1.0/asgi_correlation_id/extensions/__init__.py
--rw-r--r--   0        0        0     3705 2023-02-24 16:09:42.665838 asgi_correlation_id-4.1.0/asgi_correlation_id/extensions/celery.py
--rw-r--r--   0        0        0      829 2023-02-24 16:09:42.665838 asgi_correlation_id-4.1.0/asgi_correlation_id/extensions/sentry.py
--rw-r--r--   0        0        0     2258 2023-02-24 16:09:42.665838 asgi_correlation_id-4.1.0/asgi_correlation_id/log_filters.py
--rw-r--r--   0        0        0     3618 2023-02-24 16:09:42.665838 asgi_correlation_id-4.1.0/asgi_correlation_id/middleware.py
--rw-r--r--   0        0        0        0 2023-02-24 16:09:42.665838 asgi_correlation_id-4.1.0/asgi_correlation_id/py.typed
--rw-r--r--   0        0        0     2368 2023-02-24 16:09:42.665838 asgi_correlation_id-4.1.0/pyproject.toml
--rw-r--r--   0        0        0    24700 1970-01-01 00:00:00.000000 asgi_correlation_id-4.1.0/setup.py
--rw-r--r--   0        0        0    24743 1970-01-01 00:00:00.000000 asgi_correlation_id-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1672 2023-04-22 19:37:46.859424 asgi_correlation_id-4.2.0/LICENSE
+-rw-r--r--   0        0        0    22788 2023-04-22 19:37:46.859424 asgi_correlation_id-4.2.0/README.md
+-rw-r--r--   0        0        0      421 2023-04-22 19:37:46.859424 asgi_correlation_id-4.2.0/asgi_correlation_id/__init__.py
+-rw-r--r--   0        0        0      362 2023-04-22 19:37:46.859424 asgi_correlation_id-4.2.0/asgi_correlation_id/context.py
+-rw-r--r--   0        0        0        0 2023-04-22 19:37:46.859424 asgi_correlation_id-4.2.0/asgi_correlation_id/extensions/__init__.py
+-rw-r--r--   0        0        0     3705 2023-04-22 19:37:46.859424 asgi_correlation_id-4.2.0/asgi_correlation_id/extensions/celery.py
+-rw-r--r--   0        0        0      829 2023-04-22 19:37:46.859424 asgi_correlation_id-4.2.0/asgi_correlation_id/extensions/sentry.py
+-rw-r--r--   0        0        0     2258 2023-04-22 19:37:46.859424 asgi_correlation_id-4.2.0/asgi_correlation_id/log_filters.py
+-rw-r--r--   0        0        0     3637 2023-04-22 19:37:46.859424 asgi_correlation_id-4.2.0/asgi_correlation_id/middleware.py
+-rw-r--r--   0        0        0        0 2023-04-22 19:37:46.859424 asgi_correlation_id-4.2.0/asgi_correlation_id/py.typed
+-rw-r--r--   0        0        0     2368 2023-04-22 19:37:46.859424 asgi_correlation_id-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0    24743 1970-01-01 00:00:00.000000 asgi_correlation_id-4.2.0/PKG-INFO
```

### Comparing `asgi_correlation_id-4.1.0/LICENSE` & `asgi_correlation_id-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asgi_correlation_id-4.1.0/README.md` & `asgi_correlation_id-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `asgi_correlation_id-4.1.0/asgi_correlation_id/extensions/celery.py` & `asgi_correlation_id-4.2.0/asgi_correlation_id/extensions/celery.py`

 * *Files identical despite different names*

### Comparing `asgi_correlation_id-4.1.0/asgi_correlation_id/extensions/sentry.py` & `asgi_correlation_id-4.2.0/asgi_correlation_id/extensions/sentry.py`

 * *Files identical despite different names*

### Comparing `asgi_correlation_id-4.1.0/asgi_correlation_id/log_filters.py` & `asgi_correlation_id-4.2.0/asgi_correlation_id/log_filters.py`

 * *Files identical despite different names*

### Comparing `asgi_correlation_id-4.1.0/asgi_correlation_id/middleware.py` & `asgi_correlation_id-4.2.0/asgi_correlation_id/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     # ID transformer - can be used to clean/mutate IDs
     transformer: Optional[Callable[[str], str]] = field(default=lambda a: a)
 
     async def __call__(self, scope: 'Scope', receive: 'Receive', send: 'Send') -> None:
         """
         Load request ID from headers if present. Generate one otherwise.
         """
-        if scope['type'] != 'http':
+        if scope['type'] not in ('http', 'websocket'):
             await self.app(scope, receive, send)
             return
 
         # Try to load request ID from the request headers
         headers = MutableHeaders(scope=scope)
         header_value = headers.get(self.header_name.lower())
```

### Comparing `asgi_correlation_id-4.1.0/pyproject.toml` & `asgi_correlation_id-4.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asgi-correlation-id"
-version = "4.1.0"
+version = "4.2.0"
 description = "Middleware correlating project logs to individual requests"
 authors = ["Sondre Lillebø Gundersen <sondrelg@live.no>"]
 maintainers = ["Jonas Krüger Svensson <jonas-ks@hotmail.com>"]
 license = "BSD-4-Clause"
 readme = "README.md"
 homepage = "https://github.com/snok/asgi-correlation-id"
 repository = "https://github.com/snok/asgi-correlation-id"
```

### Comparing `asgi_correlation_id-4.1.0/setup.py` & `asgi_correlation_id-4.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,707 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: asgi-correlation-id
+Version: 4.2.0
+Summary: Middleware correlating project logs to individual requests
+Home-page: https://github.com/snok/asgi-correlation-id
+License: BSD-4-Clause
+Keywords: asgi,fastapi,starlette,async,correlation,correlation-id,request-id,x-request-id,tracing,logging,middleware,sentry,celery
+Author: Sondre Lillebø Gundersen
+Author-email: sondrelg@live.no
+Maintainer: Jonas Krüger Svensson
+Maintainer-email: jonas-ks@hotmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: celery
+Requires-Dist: celery ; extra == "celery"
+Requires-Dist: starlette (>=0.18)
+Project-URL: Repository, https://github.com/snok/asgi-correlation-id
+Description-Content-Type: text/markdown
 
-packages = \
-['asgi_correlation_id', 'asgi_correlation_id.extensions']
+[![pypi](https://img.shields.io/pypi/v/asgi-correlation-id)](https://pypi.org/project/asgi-correlation-id/)
+[![test](https://github.com/snok/asgi-correlation-id/actions/workflows/test.yml/badge.svg)](https://github.com/snok/asgi-correlation-id/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/snok/asgi-correlation-id/branch/main/graph/badge.svg?token=1aXlWPm2gb)](https://codecov.io/gh/snok/asgi-correlation-id)
 
-package_data = \
-{'': ['*']}
+# ASGI Correlation ID middleware
 
-install_requires = \
-['starlette>=0.18']
-
-extras_require = \
-{'celery': ['celery']}
-
-setup_kwargs = {
-    'name': 'asgi-correlation-id',
-    'version': '4.1.0',
-    'description': 'Middleware correlating project logs to individual requests',
-    'long_description': '[![pypi](https://img.shields.io/pypi/v/asgi-correlation-id)](https://pypi.org/project/asgi-correlation-id/)\n[![test](https://github.com/snok/asgi-correlation-id/actions/workflows/test.yml/badge.svg)](https://github.com/snok/asgi-correlation-id/actions/workflows/test.yml)\n[![codecov](https://codecov.io/gh/snok/asgi-correlation-id/branch/main/graph/badge.svg?token=1aXlWPm2gb)](https://codecov.io/gh/snok/asgi-correlation-id)\n\n# ASGI Correlation ID middleware\n\nMiddleware for reading or generating correlation IDs for each incoming request. Correlation IDs can then be added to your\nlogs, making it simple to retrieve all logs generated from a single HTTP request.\n\nWhen the middleware detects a correlation ID HTTP header in an incoming request, the ID is stored. If no header is\nfound, a correlation ID is generated for the request instead.\n\nThe middleware checks for the `X-Request-ID` header by default, but can be set to any key.\n`X-Correlation-ID` is also pretty commonly used.\n\n## Example\n\nOnce logging is configured, your output will go from this:\n\n```\nINFO    ... project.views  This is an info log\nWARNING ... project.models This is a warning log\nINFO    ... project.views  This is an info log\nINFO    ... project.views  This is an info log\nWARNING ... project.models This is a warning log\nWARNING ... project.models This is a warning log\n```\n\nto this:\n\n```docker\nINFO    ... [773fa6885] project.views  This is an info log\nWARNING ... [773fa6885] project.models This is a warning log\nINFO    ... [0d1c3919e] project.views  This is an info log\nINFO    ... [99d44111e] project.views  This is an info log\nWARNING ... [0d1c3919e] project.models This is a warning log\nWARNING ... [99d44111e] project.models This is a warning log\n```\n\nNow we\'re actually able to see which logs are related.\n\n# Installation\n\n```\npip install asgi-correlation-id\n```\n\n# Setup\n\nTo set up the package, you need to add the middleware and configure logging.\n\n## Adding the middleware\n\nThe middleware can be added like this:\n\n```python\nfrom fastapi import FastAPI\n\nfrom asgi_correlation_id import CorrelationIdMiddleware\n\napp = FastAPI()\napp.add_middleware(CorrelationIdMiddleware)\n```\n\nor any other way your framework allows.\n\nFor [Starlette](https://github.com/encode/starlette) apps, just substitute `FastAPI` with `Starlette` in all examples.\n\n## Configure logging\n\nThis section assumes you have already started configuring logging in your project. If this is not the case, check out\nthe section on [setting up logging from scratch](#setting-up-logging-from-scratch) instead.\n\nTo set up logging of the correlation ID, you simply have to add the log-filter the package provides.\n\nIf your current log-config looked like this:\n\n```python\nLOGGING = {\n    \'version\': 1,\n    \'disable_existing_loggers\': False,\n    \'formatters\': {\n        \'web\': {\n            \'class\': \'logging.Formatter\',\n            \'datefmt\': \'%H:%M:%S\',\n            \'format\': \'%(levelname)s ... %(name)s %(message)s\',\n        },\n    },\n    \'handlers\': {\n        \'web\': {\n            \'class\': \'logging.StreamHandler\',\n            \'formatter\': \'web\',\n        },\n    },\n    \'loggers\': {\n        \'my_project\': {\n            \'handlers\': [\'web\'],\n            \'level\': \'DEBUG\',\n            \'propagate\': True,\n        },\n    },\n}\n```\n\nYou simply have to add the filter, like this:\n\n```diff\nLOGGING = {\n    \'version\': 1,\n    \'disable_existing_loggers\': False,\n+   \'filters\': {\n+       \'correlation_id\': {\n+           \'()\': \'asgi_correlation_id.CorrelationIdFilter\',\n+           \'uuid_length\': 32,\n+           \'default_value\': \'-\',\n+       },\n+   },\n    \'formatters\': {\n        \'web\': {\n            \'class\': \'logging.Formatter\',\n            \'datefmt\': \'%H:%M:%S\',\n+           \'format\': \'%(levelname)s ... [%(correlation_id)s] %(name)s %(message)s\',\n        },\n    },\n    \'handlers\': {\n        \'web\': {\n            \'class\': \'logging.StreamHandler\',\n+           \'filters\': [\'correlation_id\'],\n            \'formatter\': \'web\',\n        },\n    },\n    \'loggers\': {\n        \'my_project\': {\n            \'handlers\': [\'web\'],\n            \'level\': \'DEBUG\',\n            \'propagate\': True,\n        },\n    },\n}\n```\n\nIf you\'re using a json log-formatter, just add `correlation-id: %(correlation_id)s` to your list of properties.\n\n## Middleware configuration\n\nThe middleware can be configured in a few ways, but there are no required arguments.\n\n```python\napp.add_middleware(\n    CorrelationIdMiddleware,\n    header_name=\'X-Request-ID\',\n    update_request_header=True,\n    generator=lambda: uuid4().hex,\n    validator=is_valid_uuid4,\n    transformer=lambda a: a,\n)\n```\n\nConfigurable middleware arguments include:\n\n**header_name**\n\n- Type: `str`\n- Default: `X-Request-ID`\n- Description: The header name decides which HTTP header value to read correlation IDs from. `X-Request-ID` and\n  `X-Correlation-ID` are common choices.\n\n**update_request_header**\n\n- Type: `bool`\n- Default: `True`\n- Description: Whether to update incoming request\'s header value with the generated correlation ID. This is to support\n  use cases where it\'s relied on the presence of the request header (like various tracing middlewares).\n\n**generator**\n\n- Type: `Callable[[], str]`\n- Default: `lambda: uuid4().hex`\n- Description: The generator function is responsible for generating new correlation IDs when no ID is received from an\n  incoming request\'s headers. We use UUIDs by default, but if you prefer, you could use libraries\n  like [nanoid](https://github.com/puyuan/py-nanoid) or your own custom function.\n\n**validator**\n\n- Type: `Callable[[str], bool]`\n- Default: `is_valid_uuid4` (\n  found [here](https://github.com/snok/asgi-correlation-id/blob/main/asgi_correlation_id/middleware.py#L17))\n- Description: The validator function is used when reading incoming HTTP header values. By default, we discard non-UUID\n  formatted header values, to enforce correlation ID uniqueness. If you prefer to allow any header value, you can set\n  this setting to `None`, or pass your own validator.\n\n**transformer**\n\n- Type: `Callable[[str], str]`\n- Default: `lambda a: a`\n- Description: Most users won\'t need a transformer, and by default we do nothing.\n  The argument was added for cases where users might want to alter incoming or generated ID values in some way. It\n  provides a mechanism for transforming an incoming ID in a way you see fit. See the middleware code for more context.\n\n## CORS\n\nIf you are using cross-origin resource sharing ([CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)), e.g.\nyou are making requests to an API from a frontend JavaScript code served from a different origin, you have to ensure\ntwo things:\n\n- permit correlation ID header in the incoming requests\' HTTP headers so the value can be reused by the middleware,\n- add the correlation ID header to the allowlist in responses\' HTTP headers so it can be accessed by the browser.\n\nThis can be best accomplished by using a dedicated middleware for your framework of choice. Here are some examples.\n\n### Starlette\n\nDocs: https://www.starlette.io/middleware/#corsmiddleware\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.middleware import Middleware\nfrom starlette.middleware.cors import CORSMiddleware\n\n\nmiddleware = [\n    Middleware(\n        CORSMiddleware,\n        allow_origins=[\'*\'],\n        allow_methods=[\'*\'],\n        allow_headers=[\'X-Requested-With\', \'X-Request-ID\'],\n        expose_headers=[\'X-Request-ID\']\n    )\n]\n\napp = Starlette(..., middleware=middleware)\n```\n\n### FastAPI\n\nDocs: https://fastapi.tiangolo.com/tutorial/cors/\n\n```python\nfrom app.main import app\nfrom fastapi.middleware.cors import CORSMiddleware\n\n\napp.add_middleware(\n    CORSMiddleware,\n    allow_origins=[\'*\'],\n    allow_methods=[\'*\'],\n    allow_headers=[\'X-Requested-With\', \'X-Request-ID\'],\n    expose_headers=[\'X-Request-ID\']\n)\n```\n\nFor more details on the topic, refer to the [CORS protocol](https://fetch.spec.whatwg.org/#http-cors-protocol).\n\n## Exception handling\n\nBy default, the `X-Request-ID` response header will be included in all responses from the server, *except* in the case\nof unhandled server errors. If you wish to include request IDs in the case of a `500` error you can add a custom\nexception handler.\n\nHere are some simple examples to help you get started. See each framework\'s documentation for more info.\n\n### Starlette\n\nDocs: https://www.starlette.io/exceptions/\n\n```python\nfrom starlette.requests import Request\nfrom starlette.responses import PlainTextResponse\nfrom starlette.applications import Starlette\n\nfrom asgi_correlation_id import correlation_id\n\n\nasync def custom_exception_handler(request: Request, exc: Exception) -> PlainTextResponse:\n    return PlainTextResponse(\n        "Internal Server Error",\n        status_code=500,\n        headers={\'X-Request-ID\': correlation_id.get() or ""}\n    )\n\n\napp = Starlette(\n    ...,\n    exception_handlers={500: custom_exception_handler}\n)\n```\n\n### FastAPI\n\nDocs: https://fastapi.tiangolo.com/tutorial/handling-errors/\n\n```python\nfrom app.main import app\nfrom fastapi import HTTPException, Request\nfrom fastapi.exception_handlers import http_exception_handler\nfrom fastapi.responses import JSONResponse\n\nfrom asgi_correlation_id import correlation_id\n\n\n@app.exception_handler(Exception)\nasync def unhandled_exception_handler(request: Request, exc: Exception) -> JSONResponse:\n    return await http_exception_handler(\n        request,\n        HTTPException(\n            500,\n            \'Internal server error\',\n            headers={\'X-Request-ID\': correlation_id.get() or ""}\n        ))\n```\n\nIf you are using CORS, you also have to include the `Access-Control-Allow-Origin` and `Access-Control-Expose-Headers`\nheaders in the error response. For more details, see the [CORS section](#cors) above.\n\n# Setting up logging from scratch\n\nIf your project does not have logging configured, this section will explain how to get started. If you want even more\ndetails, take a look\nat [this blogpost](https://medium.com/@sondrelg_12432/setting-up-request-id-logging-for-your-fastapi-application-4dc190aac0ea)\n.\n\nThe Python [docs](https://docs.python.org/3/library/logging.config.html) explain there are a few configuration functions\nyou may use for simpler setup. For this example we will use `dictConfig`, because that\'s what, e.g., Django users should\nfind most familiar, but the different configuration methods are interchangable, so if you want to use another method,\njust browse the python docs and change the configuration method as you please.\n\nThe benefit of `dictConfig` is that it lets you specify your entire logging configuration in a single data structure,\nand it lets you add conditional logic to it. The following example shows how to set up both console and JSON logging:\n\n```python\nfrom logging.config import dictConfig\n\nfrom app.core.config import settings\n\n\ndef configure_logging() -> None:\n    dictConfig(\n        {\n            \'version\': 1,\n            \'disable_existing_loggers\': False,\n            \'filters\': {  # correlation ID filter must be added here to make the %(correlation_id)s formatter work\n                \'correlation_id\': {\n                    \'()\': \'asgi_correlation_id.CorrelationIdFilter\',\n                    \'uuid_length\': 8 if not settings.ENVIRONMENT == \'local\' else 32,\n                    \'default_value\': \'-\',\n                },\n            },\n            \'formatters\': {\n                \'console\': {\n                    \'class\': \'logging.Formatter\',\n                    \'datefmt\': \'%H:%M:%S\',\n                    # formatter decides how our console logs look, and what info is included.\n                    # adding %(correlation_id)s to this format is what make correlation IDs appear in our logs\n                    \'format\': \'%(levelname)s:\\t\\b%(asctime)s %(name)s:%(lineno)d [%(correlation_id)s] %(message)s\',\n                },\n            },\n            \'handlers\': {\n                \'console\': {\n                    \'class\': \'logging.StreamHandler\',\n                    # Filter must be declared in the handler, otherwise it won\'t be included\n                    \'filters\': [\'correlation_id\'],\n                    \'formatter\': \'console\',\n                },\n            },\n            # Loggers can be specified to set the log-level to log, and which handlers to use\n            \'loggers\': {\n                # project logger\n                \'app\': {\'handlers\': [\'console\'], \'level\': \'DEBUG\', \'propagate\': True},\n                # third-party package loggers\n                \'databases\': {\'handlers\': [\'console\'], \'level\': \'WARNING\'},\n                \'httpx\': {\'handlers\': [\'console\'], \'level\': \'INFO\'},\n                \'asgi_correlation_id\': {\'handlers\': [\'console\'], \'level\': \'WARNING\'},\n            },\n        }\n    )\n```\n\nWith the logging configuration defined within a function like this, all you have to do is make sure to run the function\non startup somehow, and logging should work for you. You can do this any way you\'d like, but passing it to\nthe `FastAPI.on_startup` list of callables is a good starting point.\n\n# Integration with structlog\n\n[structlog](https://www.structlog.org/) is a Python library that enables structured logging.\n\nIt is trivial to configure with `asgi_correlation_id`:\n\n```python\nimport logging\nfrom typing import Any\n\nimport structlog\nfrom asgi_correlation_id import correlation_id\n\n\ndef add_correlation(\n    logger: logging.Logger, method_name: str, event_dict: dict[str, Any]\n) -> dict[str, Any]:\n    """Add request id to log message."""\n    if request_id := correlation_id.get():\n        event_dict["request_id"] = request_id\n    return event_dict\n\n\nstructlog.configure(\n    processors=[\n        add_correlation,\n        structlog.stdlib.filter_by_level,\n        structlog.stdlib.add_logger_name,\n        structlog.stdlib.add_log_level,\n        structlog.processors.TimeStamper(fmt="%Y-%m-%d %H:%M.%S"),\n        structlog.processors.StackInfoRenderer(),\n        structlog.processors.format_exc_info,\n        structlog.processors.JSONRenderer(),\n    ],\n    wrapper_class=structlog.stdlib.BoundLogger,\n    logger_factory=structlog.stdlib.LoggerFactory(),\n    cache_logger_on_first_use=True,\n)\n```\n\n# Integration with [SAQ](https://github.com/tobymao/saq)\n\nIf you\'re using [saq](https://github.com/tobymao/saq/), you\ncan easily transfer request IDs from the web server to your\nworkers by using the event hooks provided by the library:\n\n```python\nfrom uuid import uuid4\n\nfrom asgi_correlation_id import correlation_id\nfrom saq import Job, Queue\n\n\nCID_TRANSFER_KEY = \'correlation_id\'\n\n\nasync def before_enqueue(job: Job) -> None:\n    """\n    Transfer the correlation ID from the current context to the worker.\n\n    This might be called from a web server or a worker process.\n    """\n    job.meta[CID_TRANSFER_KEY] = correlation_id.get() or uuid4()\n\n\nasync def before_process(ctx: dict) -> None:\n    """\n    Load correlation ID from the enqueueing process to this one.\n    """\n    correlation_id.set(ctx[\'job\'].meta.get(CID_TRANSFER_KEY, uuid4()))\n\n\nasync def after_process(ctx: dict) -> None:\n    """\n    Reset correlation ID for this process.\n    """\n    correlation_id.set(None)\n\nqueue = Queue(...)\nqueue.register_before_enqueue(before_enqueue)\n\npriority_settings = {\n    ...,\n    \'queue\': queue,\n    \'before_process\': before_process,\n    \'after_process\': after_process,\n}\n```\n\n# Extensions\n\nIn addition to the middleware, we\'ve added a couple of extensions for third-party packages.\n\n## Sentry\n\nIf your project has [sentry-sdk](https://pypi.org/project/sentry-sdk/)\ninstalled, correlation IDs will automatically be added to Sentry events as a `transaction_id`.\n\nSee\nthis [blogpost](https://blog.sentry.io/2019/04/04/trace-errors-through-stack-using-unique-identifiers-in-sentry#1-generate-a-unique-identifier-and-set-as-a-sentry-tag-on-issuing-service)\nfor a little bit of detail. The transaction ID is displayed in the event detail view in Sentry and is just an easy way\nto connect logs to a Sentry event.\n\n## Celery\n\n> Note: If you\'re using the celery integration, install the package with `pip install asgi-correlation-id[celery]`\n\nFor Celery user\'s there\'s one primary issue: workers run as completely separate processes, so correlation IDs are lost\nwhen spawning background tasks from requests.\n\nHowever, with some Celery signal magic, we can actually transfer correlation IDs to worker processes, like this:\n\n```python\n@before_task_publish.connect()\ndef transfer_correlation_id(headers) -> None:\n    # This is called before task.delay() finishes\n    # Here we\'re able to transfer the correlation ID via the headers kept in our backend\n    headers[header_key] = correlation_id.get()\n\n\n@task_prerun.connect()\ndef load_correlation_id(task) -> None:\n    # This is called when the worker picks up the task\n    # Here we\'re able to load the correlation ID from the headers\n    id_value = task.request.get(header_key)\n    correlation_id.set(id_value)\n```\n\nTo configure correlation ID transfer, simply import and run the setup function the package provides:\n\n```python\nfrom asgi_correlation_id.extensions.celery import load_correlation_ids\n\nload_correlation_ids()\n```\n\n### Taking it one step further - Adding Celery tracing IDs\n\nIn addition to transferring request IDs to Celery workers, we\'ve added one more log filter for improving tracing in\ncelery processes. This is completely separate from correlation ID functionality, but is something we use ourselves, so\nkeep in the package with the rest of the signals.\n\nThe log filter adds an ID, `celery_current_id` for each worker process, and an ID, `celery_parent_id` for the process\nthat spawned it.\n\nHere\'s a quick summary of outputs from different scenarios:\n\n| Scenario                                           | Correlation ID     | Celery Current ID | Celery Parent ID |\n|------------------------------------------          |--------------------|-------------------|------------------|\n| Request                                            | ✅                |                   |                  |\n| Request -> Worker                                  | ✅                | ✅               |                  |\n| Request -> Worker -> Another worker                | ✅                | ✅               | ✅              |\n| Beat -> Worker     | ✅*               | ✅                |                   |                  |\n| Beat -> Worker -> Worker     | ✅*     | ✅                | ✅               | ✅              |\n\n*When we\'re in a process spawned separately from an HTTP request, a correlation ID is still spawned for the first\nprocess in the chain, and passed down. You can think of the correlation ID as an origin ID, while the combination of\ncurrent and parent-ids as a way of linking the chain.\n\nTo add the current and parent IDs, just alter your `celery.py` to this:\n\n```diff\n+ from asgi_correlation_id.extensions.celery import load_correlation_ids, load_celery_current_and_parent_ids\n\nload_correlation_ids()\n+ load_celery_current_and_parent_ids()\n```\n\nIf you wish to correlate celery task IDs through the IDs found in your broker (i.e., the celery `task_id`), use the `use_internal_celery_task_id` argument on `load_celery_current_and_parent_ids`\n```diff\nfrom asgi_correlation_id.extensions.celery import load_correlation_ids, load_celery_current_and_parent_ids\n\nload_correlation_ids()\n+ load_celery_current_and_parent_ids(use_internal_celery_task_id=True)\n```\nNote: `load_celery_current_and_parent_ids` will ignore the `generator` argument when `use_internal_celery_task_id` is set to `True`\n\nTo set up the additional log filters, update your log config like this:\n\n```diff\nLOGGING = {\n    \'version\': 1,\n    \'disable_existing_loggers\': False,\n    \'filters\': {\n        \'correlation_id\': {\n+           \'()\': \'asgi_correlation_id.CorrelationIdFilter\',\n+           \'uuid_length\': 32,\n+           \'default_value\': \'-\',\n+       },\n+       \'celery_tracing\': {\n+            \'()\': \'asgi_correlation_id.CeleryTracingIdsFilter\',\n+            \'uuid_length\': 32,\n+            \'default_value\': \'-\',\n+       },\n    },\n    \'formatters\': {\n        \'web\': {\n            \'class\': \'logging.Formatter\',\n            \'datefmt\': \'%H:%M:%S\',\n            \'format\': \'%(levelname)s ... [%(correlation_id)s] %(name)s %(message)s\',\n        },\n+       \'celery\': {\n+           \'class\': \'logging.Formatter\',\n+           \'datefmt\': \'%H:%M:%S\',\n+           \'format\': \'%(levelname)s ... [%(correlation_id)s] [%(celery_parent_id)s-%(celery_current_id)s] %(name)s %(message)s\',\n+       },\n    },\n    \'handlers\': {\n        \'web\': {\n            \'class\': \'logging.StreamHandler\',\n            \'filters\': [\'correlation_id\'],\n            \'formatter\': \'web\',\n        },\n+       \'celery\': {\n+           \'class\': \'logging.StreamHandler\',\n+           \'filters\': [\'correlation_id\', \'celery_tracing\'],\n+           \'formatter\': \'celery\',\n+       },\n    },\n    \'loggers\': {\n        \'my_project\': {\n+           \'handlers\': [\'celery\' if any(\'celery\' in i for i in sys.argv) else \'web\'],\n            \'level\': \'DEBUG\',\n            \'propagate\': True,\n        },\n    },\n}\n```\n\nWith these IDs configured you should be able to:\n\n1. correlate all logs from a single origin, and\n2. piece together the order each log was run, and which process spawned which\n\n#### Example\n\nWith everything configured, assuming you have a set of tasks like this:\n\n```python\n@celery.task()\ndef debug_task() -> None:\n    logger.info(\'Debug task 1\')\n    second_debug_task.delay()\n    second_debug_task.delay()\n\n\n@celery.task()\ndef second_debug_task() -> None:\n    logger.info(\'Debug task 2\')\n    third_debug_task.delay()\n    fourth_debug_task.delay()\n\n\n@celery.task()\ndef third_debug_task() -> None:\n    logger.info(\'Debug task 3\')\n    fourth_debug_task.delay()\n    fourth_debug_task.delay()\n\n\n@celery.task()\ndef fourth_debug_task() -> None:\n    logger.info(\'Debug task 4\')\n```\n\nyour logs could look something like this:\n\n```\n   correlation-id               current-id\n          |        parent-id        |\n          |            |            |\nINFO [3b162382e1] [    -     ] [93ddf3639c] project.tasks - Debug task 1\nINFO [3b162382e1] [93ddf3639c] [24046ab022] project.tasks - Debug task 2\nINFO [3b162382e1] [93ddf3639c] [cb5595a417] project.tasks - Debug task 2\nINFO [3b162382e1] [24046ab022] [08f5428a66] project.tasks - Debug task 3\nINFO [3b162382e1] [24046ab022] [32f40041c6] project.tasks - Debug task 4\nINFO [3b162382e1] [cb5595a417] [1c75a4ed2c] project.tasks - Debug task 3\nINFO [3b162382e1] [08f5428a66] [578ad2d141] project.tasks - Debug task 4\nINFO [3b162382e1] [cb5595a417] [21b2ef77ae] project.tasks - Debug task 4\nINFO [3b162382e1] [08f5428a66] [8cad7fc4d7] project.tasks - Debug task 4\nINFO [3b162382e1] [1c75a4ed2c] [72a43319f0] project.tasks - Debug task 4\nINFO [3b162382e1] [1c75a4ed2c] [ec3cf4113e] project.tasks - Debug task 4\n```\n',
-    'author': 'Sondre Lillebø Gundersen',
-    'author_email': 'sondrelg@live.no',
-    'maintainer': 'Jonas Krüger Svensson',
-    'maintainer_email': 'jonas-ks@hotmail.com',
-    'url': 'https://github.com/snok/asgi-correlation-id',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
+Middleware for reading or generating correlation IDs for each incoming request. Correlation IDs can then be added to your
+logs, making it simple to retrieve all logs generated from a single HTTP request.
+
+When the middleware detects a correlation ID HTTP header in an incoming request, the ID is stored. If no header is
+found, a correlation ID is generated for the request instead.
+
+The middleware checks for the `X-Request-ID` header by default, but can be set to any key.
+`X-Correlation-ID` is also pretty commonly used.
+
+## Example
+
+Once logging is configured, your output will go from this:
+
+```
+INFO    ... project.views  This is an info log
+WARNING ... project.models This is a warning log
+INFO    ... project.views  This is an info log
+INFO    ... project.views  This is an info log
+WARNING ... project.models This is a warning log
+WARNING ... project.models This is a warning log
+```
+
+to this:
+
+```docker
+INFO    ... [773fa6885] project.views  This is an info log
+WARNING ... [773fa6885] project.models This is a warning log
+INFO    ... [0d1c3919e] project.views  This is an info log
+INFO    ... [99d44111e] project.views  This is an info log
+WARNING ... [0d1c3919e] project.models This is a warning log
+WARNING ... [99d44111e] project.models This is a warning log
+```
+
+Now we're actually able to see which logs are related.
+
+# Installation
+
+```
+pip install asgi-correlation-id
+```
+
+# Setup
+
+To set up the package, you need to add the middleware and configure logging.
+
+## Adding the middleware
+
+The middleware can be added like this:
+
+```python
+from fastapi import FastAPI
+
+from asgi_correlation_id import CorrelationIdMiddleware
+
+app = FastAPI()
+app.add_middleware(CorrelationIdMiddleware)
+```
+
+or any other way your framework allows.
+
+For [Starlette](https://github.com/encode/starlette) apps, just substitute `FastAPI` with `Starlette` in all examples.
+
+## Configure logging
+
+This section assumes you have already started configuring logging in your project. If this is not the case, check out
+the section on [setting up logging from scratch](#setting-up-logging-from-scratch) instead.
+
+To set up logging of the correlation ID, you simply have to add the log-filter the package provides.
+
+If your current log-config looked like this:
+
+```python
+LOGGING = {
+    'version': 1,
+    'disable_existing_loggers': False,
+    'formatters': {
+        'web': {
+            'class': 'logging.Formatter',
+            'datefmt': '%H:%M:%S',
+            'format': '%(levelname)s ... %(name)s %(message)s',
+        },
+    },
+    'handlers': {
+        'web': {
+            'class': 'logging.StreamHandler',
+            'formatter': 'web',
+        },
+    },
+    'loggers': {
+        'my_project': {
+            'handlers': ['web'],
+            'level': 'DEBUG',
+            'propagate': True,
+        },
+    },
 }
+```
+
+You simply have to add the filter, like this:
+
+```diff
+LOGGING = {
+    'version': 1,
+    'disable_existing_loggers': False,
++   'filters': {
++       'correlation_id': {
++           '()': 'asgi_correlation_id.CorrelationIdFilter',
++           'uuid_length': 32,
++           'default_value': '-',
++       },
++   },
+    'formatters': {
+        'web': {
+            'class': 'logging.Formatter',
+            'datefmt': '%H:%M:%S',
++           'format': '%(levelname)s ... [%(correlation_id)s] %(name)s %(message)s',
+        },
+    },
+    'handlers': {
+        'web': {
+            'class': 'logging.StreamHandler',
++           'filters': ['correlation_id'],
+            'formatter': 'web',
+        },
+    },
+    'loggers': {
+        'my_project': {
+            'handlers': ['web'],
+            'level': 'DEBUG',
+            'propagate': True,
+        },
+    },
+}
+```
+
+If you're using a json log-formatter, just add `correlation-id: %(correlation_id)s` to your list of properties.
+
+## Middleware configuration
+
+The middleware can be configured in a few ways, but there are no required arguments.
+
+```python
+app.add_middleware(
+    CorrelationIdMiddleware,
+    header_name='X-Request-ID',
+    update_request_header=True,
+    generator=lambda: uuid4().hex,
+    validator=is_valid_uuid4,
+    transformer=lambda a: a,
+)
+```
+
+Configurable middleware arguments include:
+
+**header_name**
+
+- Type: `str`
+- Default: `X-Request-ID`
+- Description: The header name decides which HTTP header value to read correlation IDs from. `X-Request-ID` and
+  `X-Correlation-ID` are common choices.
+
+**update_request_header**
+
+- Type: `bool`
+- Default: `True`
+- Description: Whether to update incoming request's header value with the generated correlation ID. This is to support
+  use cases where it's relied on the presence of the request header (like various tracing middlewares).
+
+**generator**
+
+- Type: `Callable[[], str]`
+- Default: `lambda: uuid4().hex`
+- Description: The generator function is responsible for generating new correlation IDs when no ID is received from an
+  incoming request's headers. We use UUIDs by default, but if you prefer, you could use libraries
+  like [nanoid](https://github.com/puyuan/py-nanoid) or your own custom function.
+
+**validator**
+
+- Type: `Callable[[str], bool]`
+- Default: `is_valid_uuid4` (
+  found [here](https://github.com/snok/asgi-correlation-id/blob/main/asgi_correlation_id/middleware.py#L17))
+- Description: The validator function is used when reading incoming HTTP header values. By default, we discard non-UUID
+  formatted header values, to enforce correlation ID uniqueness. If you prefer to allow any header value, you can set
+  this setting to `None`, or pass your own validator.
+
+**transformer**
+
+- Type: `Callable[[str], str]`
+- Default: `lambda a: a`
+- Description: Most users won't need a transformer, and by default we do nothing.
+  The argument was added for cases where users might want to alter incoming or generated ID values in some way. It
+  provides a mechanism for transforming an incoming ID in a way you see fit. See the middleware code for more context.
+
+## CORS
+
+If you are using cross-origin resource sharing ([CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)), e.g.
+you are making requests to an API from a frontend JavaScript code served from a different origin, you have to ensure
+two things:
+
+- permit correlation ID header in the incoming requests' HTTP headers so the value can be reused by the middleware,
+- add the correlation ID header to the allowlist in responses' HTTP headers so it can be accessed by the browser.
+
+This can be best accomplished by using a dedicated middleware for your framework of choice. Here are some examples.
+
+### Starlette
+
+Docs: https://www.starlette.io/middleware/#corsmiddleware
+
+```python
+from starlette.applications import Starlette
+from starlette.middleware import Middleware
+from starlette.middleware.cors import CORSMiddleware
+
+
+middleware = [
+    Middleware(
+        CORSMiddleware,
+        allow_origins=['*'],
+        allow_methods=['*'],
+        allow_headers=['X-Requested-With', 'X-Request-ID'],
+        expose_headers=['X-Request-ID']
+    )
+]
+
+app = Starlette(..., middleware=middleware)
+```
+
+### FastAPI
+
+Docs: https://fastapi.tiangolo.com/tutorial/cors/
+
+```python
+from app.main import app
+from fastapi.middleware.cors import CORSMiddleware
+
+
+app.add_middleware(
+    CORSMiddleware,
+    allow_origins=['*'],
+    allow_methods=['*'],
+    allow_headers=['X-Requested-With', 'X-Request-ID'],
+    expose_headers=['X-Request-ID']
+)
+```
+
+For more details on the topic, refer to the [CORS protocol](https://fetch.spec.whatwg.org/#http-cors-protocol).
+
+## Exception handling
+
+By default, the `X-Request-ID` response header will be included in all responses from the server, *except* in the case
+of unhandled server errors. If you wish to include request IDs in the case of a `500` error you can add a custom
+exception handler.
+
+Here are some simple examples to help you get started. See each framework's documentation for more info.
+
+### Starlette
+
+Docs: https://www.starlette.io/exceptions/
+
+```python
+from starlette.requests import Request
+from starlette.responses import PlainTextResponse
+from starlette.applications import Starlette
+
+from asgi_correlation_id import correlation_id
+
+
+async def custom_exception_handler(request: Request, exc: Exception) -> PlainTextResponse:
+    return PlainTextResponse(
+        "Internal Server Error",
+        status_code=500,
+        headers={'X-Request-ID': correlation_id.get() or ""}
+    )
+
+
+app = Starlette(
+    ...,
+    exception_handlers={500: custom_exception_handler}
+)
+```
+
+### FastAPI
+
+Docs: https://fastapi.tiangolo.com/tutorial/handling-errors/
+
+```python
+from app.main import app
+from fastapi import HTTPException, Request
+from fastapi.exception_handlers import http_exception_handler
+from fastapi.responses import JSONResponse
+
+from asgi_correlation_id import correlation_id
+
+
+@app.exception_handler(Exception)
+async def unhandled_exception_handler(request: Request, exc: Exception) -> JSONResponse:
+    return await http_exception_handler(
+        request,
+        HTTPException(
+            500,
+            'Internal server error',
+            headers={'X-Request-ID': correlation_id.get() or ""}
+        ))
+```
+
+If you are using CORS, you also have to include the `Access-Control-Allow-Origin` and `Access-Control-Expose-Headers`
+headers in the error response. For more details, see the [CORS section](#cors) above.
+
+# Setting up logging from scratch
+
+If your project does not have logging configured, this section will explain how to get started. If you want even more
+details, take a look
+at [this blogpost](https://medium.com/@sondrelg_12432/setting-up-request-id-logging-for-your-fastapi-application-4dc190aac0ea)
+.
+
+The Python [docs](https://docs.python.org/3/library/logging.config.html) explain there are a few configuration functions
+you may use for simpler setup. For this example we will use `dictConfig`, because that's what, e.g., Django users should
+find most familiar, but the different configuration methods are interchangable, so if you want to use another method,
+just browse the python docs and change the configuration method as you please.
+
+The benefit of `dictConfig` is that it lets you specify your entire logging configuration in a single data structure,
+and it lets you add conditional logic to it. The following example shows how to set up both console and JSON logging:
+
+```python
+from logging.config import dictConfig
+
+from app.core.config import settings
+
+
+def configure_logging() -> None:
+    dictConfig(
+        {
+            'version': 1,
+            'disable_existing_loggers': False,
+            'filters': {  # correlation ID filter must be added here to make the %(correlation_id)s formatter work
+                'correlation_id': {
+                    '()': 'asgi_correlation_id.CorrelationIdFilter',
+                    'uuid_length': 8 if not settings.ENVIRONMENT == 'local' else 32,
+                    'default_value': '-',
+                },
+            },
+            'formatters': {
+                'console': {
+                    'class': 'logging.Formatter',
+                    'datefmt': '%H:%M:%S',
+                    # formatter decides how our console logs look, and what info is included.
+                    # adding %(correlation_id)s to this format is what make correlation IDs appear in our logs
+                    'format': '%(levelname)s:\t\b%(asctime)s %(name)s:%(lineno)d [%(correlation_id)s] %(message)s',
+                },
+            },
+            'handlers': {
+                'console': {
+                    'class': 'logging.StreamHandler',
+                    # Filter must be declared in the handler, otherwise it won't be included
+                    'filters': ['correlation_id'],
+                    'formatter': 'console',
+                },
+            },
+            # Loggers can be specified to set the log-level to log, and which handlers to use
+            'loggers': {
+                # project logger
+                'app': {'handlers': ['console'], 'level': 'DEBUG', 'propagate': True},
+                # third-party package loggers
+                'databases': {'handlers': ['console'], 'level': 'WARNING'},
+                'httpx': {'handlers': ['console'], 'level': 'INFO'},
+                'asgi_correlation_id': {'handlers': ['console'], 'level': 'WARNING'},
+            },
+        }
+    )
+```
+
+With the logging configuration defined within a function like this, all you have to do is make sure to run the function
+on startup somehow, and logging should work for you. You can do this any way you'd like, but passing it to
+the `FastAPI.on_startup` list of callables is a good starting point.
+
+# Integration with structlog
+
+[structlog](https://www.structlog.org/) is a Python library that enables structured logging.
+
+It is trivial to configure with `asgi_correlation_id`:
+
+```python
+import logging
+from typing import Any
+
+import structlog
+from asgi_correlation_id import correlation_id
+
+
+def add_correlation(
+    logger: logging.Logger, method_name: str, event_dict: dict[str, Any]
+) -> dict[str, Any]:
+    """Add request id to log message."""
+    if request_id := correlation_id.get():
+        event_dict["request_id"] = request_id
+    return event_dict
+
+
+structlog.configure(
+    processors=[
+        add_correlation,
+        structlog.stdlib.filter_by_level,
+        structlog.stdlib.add_logger_name,
+        structlog.stdlib.add_log_level,
+        structlog.processors.TimeStamper(fmt="%Y-%m-%d %H:%M.%S"),
+        structlog.processors.StackInfoRenderer(),
+        structlog.processors.format_exc_info,
+        structlog.processors.JSONRenderer(),
+    ],
+    wrapper_class=structlog.stdlib.BoundLogger,
+    logger_factory=structlog.stdlib.LoggerFactory(),
+    cache_logger_on_first_use=True,
+)
+```
+
+# Integration with [SAQ](https://github.com/tobymao/saq)
+
+If you're using [saq](https://github.com/tobymao/saq/), you
+can easily transfer request IDs from the web server to your
+workers by using the event hooks provided by the library:
+
+```python
+from uuid import uuid4
+
+from asgi_correlation_id import correlation_id
+from saq import Job, Queue
+
+
+CID_TRANSFER_KEY = 'correlation_id'
+
+
+async def before_enqueue(job: Job) -> None:
+    """
+    Transfer the correlation ID from the current context to the worker.
+
+    This might be called from a web server or a worker process.
+    """
+    job.meta[CID_TRANSFER_KEY] = correlation_id.get() or uuid4()
+
+
+async def before_process(ctx: dict) -> None:
+    """
+    Load correlation ID from the enqueueing process to this one.
+    """
+    correlation_id.set(ctx['job'].meta.get(CID_TRANSFER_KEY, uuid4()))
+
+
+async def after_process(ctx: dict) -> None:
+    """
+    Reset correlation ID for this process.
+    """
+    correlation_id.set(None)
+
+queue = Queue(...)
+queue.register_before_enqueue(before_enqueue)
+
+priority_settings = {
+    ...,
+    'queue': queue,
+    'before_process': before_process,
+    'after_process': after_process,
+}
+```
+
+# Extensions
+
+In addition to the middleware, we've added a couple of extensions for third-party packages.
+
+## Sentry
+
+If your project has [sentry-sdk](https://pypi.org/project/sentry-sdk/)
+installed, correlation IDs will automatically be added to Sentry events as a `transaction_id`.
+
+See
+this [blogpost](https://blog.sentry.io/2019/04/04/trace-errors-through-stack-using-unique-identifiers-in-sentry#1-generate-a-unique-identifier-and-set-as-a-sentry-tag-on-issuing-service)
+for a little bit of detail. The transaction ID is displayed in the event detail view in Sentry and is just an easy way
+to connect logs to a Sentry event.
+
+## Celery
+
+> Note: If you're using the celery integration, install the package with `pip install asgi-correlation-id[celery]`
+
+For Celery user's there's one primary issue: workers run as completely separate processes, so correlation IDs are lost
+when spawning background tasks from requests.
+
+However, with some Celery signal magic, we can actually transfer correlation IDs to worker processes, like this:
+
+```python
+@before_task_publish.connect()
+def transfer_correlation_id(headers) -> None:
+    # This is called before task.delay() finishes
+    # Here we're able to transfer the correlation ID via the headers kept in our backend
+    headers[header_key] = correlation_id.get()
+
+
+@task_prerun.connect()
+def load_correlation_id(task) -> None:
+    # This is called when the worker picks up the task
+    # Here we're able to load the correlation ID from the headers
+    id_value = task.request.get(header_key)
+    correlation_id.set(id_value)
+```
+
+To configure correlation ID transfer, simply import and run the setup function the package provides:
+
+```python
+from asgi_correlation_id.extensions.celery import load_correlation_ids
+
+load_correlation_ids()
+```
+
+### Taking it one step further - Adding Celery tracing IDs
+
+In addition to transferring request IDs to Celery workers, we've added one more log filter for improving tracing in
+celery processes. This is completely separate from correlation ID functionality, but is something we use ourselves, so
+keep in the package with the rest of the signals.
+
+The log filter adds an ID, `celery_current_id` for each worker process, and an ID, `celery_parent_id` for the process
+that spawned it.
+
+Here's a quick summary of outputs from different scenarios:
+
+| Scenario                                           | Correlation ID     | Celery Current ID | Celery Parent ID |
+|------------------------------------------          |--------------------|-------------------|------------------|
+| Request                                            | ✅                |                   |                  |
+| Request -> Worker                                  | ✅                | ✅               |                  |
+| Request -> Worker -> Another worker                | ✅                | ✅               | ✅              |
+| Beat -> Worker     | ✅*               | ✅                |                   |                  |
+| Beat -> Worker -> Worker     | ✅*     | ✅                | ✅               | ✅              |
+
+*When we're in a process spawned separately from an HTTP request, a correlation ID is still spawned for the first
+process in the chain, and passed down. You can think of the correlation ID as an origin ID, while the combination of
+current and parent-ids as a way of linking the chain.
+
+To add the current and parent IDs, just alter your `celery.py` to this:
+
+```diff
++ from asgi_correlation_id.extensions.celery import load_correlation_ids, load_celery_current_and_parent_ids
+
+load_correlation_ids()
++ load_celery_current_and_parent_ids()
+```
+
+If you wish to correlate celery task IDs through the IDs found in your broker (i.e., the celery `task_id`), use the `use_internal_celery_task_id` argument on `load_celery_current_and_parent_ids`
+```diff
+from asgi_correlation_id.extensions.celery import load_correlation_ids, load_celery_current_and_parent_ids
+
+load_correlation_ids()
++ load_celery_current_and_parent_ids(use_internal_celery_task_id=True)
+```
+Note: `load_celery_current_and_parent_ids` will ignore the `generator` argument when `use_internal_celery_task_id` is set to `True`
+
+To set up the additional log filters, update your log config like this:
+
+```diff
+LOGGING = {
+    'version': 1,
+    'disable_existing_loggers': False,
+    'filters': {
+        'correlation_id': {
++           '()': 'asgi_correlation_id.CorrelationIdFilter',
++           'uuid_length': 32,
++           'default_value': '-',
++       },
++       'celery_tracing': {
++            '()': 'asgi_correlation_id.CeleryTracingIdsFilter',
++            'uuid_length': 32,
++            'default_value': '-',
++       },
+    },
+    'formatters': {
+        'web': {
+            'class': 'logging.Formatter',
+            'datefmt': '%H:%M:%S',
+            'format': '%(levelname)s ... [%(correlation_id)s] %(name)s %(message)s',
+        },
++       'celery': {
++           'class': 'logging.Formatter',
++           'datefmt': '%H:%M:%S',
++           'format': '%(levelname)s ... [%(correlation_id)s] [%(celery_parent_id)s-%(celery_current_id)s] %(name)s %(message)s',
++       },
+    },
+    'handlers': {
+        'web': {
+            'class': 'logging.StreamHandler',
+            'filters': ['correlation_id'],
+            'formatter': 'web',
+        },
++       'celery': {
++           'class': 'logging.StreamHandler',
++           'filters': ['correlation_id', 'celery_tracing'],
++           'formatter': 'celery',
++       },
+    },
+    'loggers': {
+        'my_project': {
++           'handlers': ['celery' if any('celery' in i for i in sys.argv) else 'web'],
+            'level': 'DEBUG',
+            'propagate': True,
+        },
+    },
+}
+```
+
+With these IDs configured you should be able to:
+
+1. correlate all logs from a single origin, and
+2. piece together the order each log was run, and which process spawned which
+
+#### Example
+
+With everything configured, assuming you have a set of tasks like this:
+
+```python
+@celery.task()
+def debug_task() -> None:
+    logger.info('Debug task 1')
+    second_debug_task.delay()
+    second_debug_task.delay()
+
+
+@celery.task()
+def second_debug_task() -> None:
+    logger.info('Debug task 2')
+    third_debug_task.delay()
+    fourth_debug_task.delay()
+
+
+@celery.task()
+def third_debug_task() -> None:
+    logger.info('Debug task 3')
+    fourth_debug_task.delay()
+    fourth_debug_task.delay()
+
+
+@celery.task()
+def fourth_debug_task() -> None:
+    logger.info('Debug task 4')
+```
+
+your logs could look something like this:
 
+```
+   correlation-id               current-id
+          |        parent-id        |
+          |            |            |
+INFO [3b162382e1] [    -     ] [93ddf3639c] project.tasks - Debug task 1
+INFO [3b162382e1] [93ddf3639c] [24046ab022] project.tasks - Debug task 2
+INFO [3b162382e1] [93ddf3639c] [cb5595a417] project.tasks - Debug task 2
+INFO [3b162382e1] [24046ab022] [08f5428a66] project.tasks - Debug task 3
+INFO [3b162382e1] [24046ab022] [32f40041c6] project.tasks - Debug task 4
+INFO [3b162382e1] [cb5595a417] [1c75a4ed2c] project.tasks - Debug task 3
+INFO [3b162382e1] [08f5428a66] [578ad2d141] project.tasks - Debug task 4
+INFO [3b162382e1] [cb5595a417] [21b2ef77ae] project.tasks - Debug task 4
+INFO [3b162382e1] [08f5428a66] [8cad7fc4d7] project.tasks - Debug task 4
+INFO [3b162382e1] [1c75a4ed2c] [72a43319f0] project.tasks - Debug task 4
+INFO [3b162382e1] [1c75a4ed2c] [ec3cf4113e] project.tasks - Debug task 4
+```
 
-setup(**setup_kwargs)
```

