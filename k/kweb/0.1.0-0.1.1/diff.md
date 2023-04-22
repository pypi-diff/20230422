# Comparing `tmp/kweb-0.1.0.tar.gz` & `tmp/kweb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kweb-0.1.0.tar", last modified: Sat Apr 22 14:01:28 2023, max compression
+gzip compressed data, was "kweb-0.1.1.tar", last modified: Sat Apr 22 14:12:35 2023, max compression
```

## Comparing `kweb-0.1.0.tar` & `kweb-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.666090 kweb-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-22 14:01:11.000000 kweb-0.1.0/.bumpversion.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.662090 kweb-0.1.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-22 14:01:11.000000 kweb-0.1.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-22 14:01:11.000000 kweb-0.1.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.662090 kweb-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-22 14:01:11.000000 kweb-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.662090 kweb-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-22 14:01:11.000000 kweb-0.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-22 14:01:11.000000 kweb-0.1.0/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-22 14:01:11.000000 kweb-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-22 14:01:11.000000 kweb-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-22 14:01:11.000000 kweb-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-22 14:01:11.000000 kweb-0.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-22 14:01:28.666090 kweb-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-22 14:01:11.000000 kweb-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.662090 kweb-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.658090 kweb-0.1.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.662090 kweb-0.1.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/markdown.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-22 14:01:11.000000 kweb-0.1.0/docs/rst.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-22 14:01:11.000000 kweb-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 14:01:28.666090 kweb-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.662090 kweb-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.662090 kweb-0.1.0/src/kweb/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.666090 kweb-0.1.0/src/kweb/gds_files/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/gds_files/wg.gds
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7188 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1321 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/server_jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.666090 kweb-0.1.0/src/kweb/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/static/client.css
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/static/client.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.666090 kweb-0.1.0/src/kweb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-22 14:01:11.000000 kweb-0.1.0/src/kweb/templates/client.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.666090 kweb-0.1.0/src/kweb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-22 14:01:28.000000 kweb-0.1.0/src/kweb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-22 14:01:28.000000 kweb-0.1.0/src/kweb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 14:01:28.000000 kweb-0.1.0/src/kweb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-22 14:01:28.000000 kweb-0.1.0/src/kweb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-22 14:01:28.000000 kweb-0.1.0/src/kweb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:01:28.666090 kweb-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-22 14:01:11.000000 kweb-0.1.0/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:12:35.596043 kweb-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-22 14:12:17.000000 kweb-0.1.1/.bumpversion.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:12:35.596043 kweb-0.1.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-22 14:12:17.000000 kweb-0.1.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-22 14:12:17.000000 kweb-0.1.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:12:35.596043 kweb-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-22 14:12:17.000000 kweb-0.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:12:35.596043 kweb-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-22 14:12:17.000000 kweb-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-22 14:12:17.000000 kweb-0.1.1/.github/workflows/test_code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-22 14:12:17.000000 kweb-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-22 14:12:17.000000 kweb-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-22 14:12:17.000000 kweb-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-22 14:12:17.000000 kweb-0.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-22 14:12:35.596043 kweb-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-22 14:12:17.000000 kweb-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:12:35.596043 kweb-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-22 14:12:17.000000 kweb-0.1.1/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-22 14:12:17.000000 kweb-0.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-22 14:12:17.000000 kweb-0.1.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:12:35.592043 kweb-0.1.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:12:35.596043 kweb-0.1.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-22 14:12:17.000000 kweb-0.1.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-22 14:12:17.000000 kweb-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-22 14:12:17.000000 kweb-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-22 14:12:17.000000 kweb-0.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-22 14:12:17.000000 kweb-0.1.1/docs/markdown.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-22 14:12:17.000000 kweb-0.1.1/docs/rst.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-22 14:12:17.000000 kweb-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 14:12:35.596043 kweb-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:12:35.592043 kweb-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:12:35.596043 kweb-0.1.1/src/kweb/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-22 14:12:17.000000 kweb-0.1.1/src/kweb/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 14:12:17.000000 kweb-0.1.1/src/kweb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:12:35.596043 kweb-0.1.1/src/kweb/gds_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-22 14:12:17.000000 kweb-0.1.1/src/kweb/gds_files/wg.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-22 14:12:17.000000 kweb-0.1.1/src/kweb/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7227 2023-04-22 14:12:17.000000 kweb-0.1.1/src/kweb/server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1321 2023-04-22 14:12:17.000000 kweb-0.1.1/src/kweb/server_jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:12:35.596043 kweb-0.1.1/src/kweb/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-22 14:12:17.000000 kweb-0.1.1/src/kweb/static/client.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-04-22 14:12:17.000000 kweb-0.1.1/src/kweb/static/client.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:12:35.596043 kweb-0.1.1/src/kweb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-22 14:12:17.000000 kweb-0.1.1/src/kweb/templates/client.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:12:35.596043 kweb-0.1.1/src/kweb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-22 14:12:35.000000 kweb-0.1.1/src/kweb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-22 14:12:35.000000 kweb-0.1.1/src/kweb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 14:12:35.000000 kweb-0.1.1/src/kweb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-22 14:12:35.000000 kweb-0.1.1/src/kweb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-22 14:12:35.000000 kweb-0.1.1/src/kweb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:12:35.596043 kweb-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-22 14:12:17.000000 kweb-0.1.1/tests/test_sample.py
```

### Comparing `kweb-0.1.0/.github/workflows/release.yml` & `kweb-0.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `kweb-0.1.0/.github/workflows/test_code.yml` & `kweb-0.1.1/.github/workflows/test_code.yml`

 * *Files identical despite different names*

### Comparing `kweb-0.1.0/.gitignore` & `kweb-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kweb-0.1.0/.pre-commit-config.yaml` & `kweb-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kweb-0.1.0/LICENSE` & `kweb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kweb-0.1.0/PKG-INFO` & `kweb-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kweb
-Version: 0.1.0
+Version: 0.1.1
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: ipy
 License-File: LICENSE
 
-# kweb 0.1.0
+# kweb 0.1.1
 
 KLayout Web Viewer ![demo](https://i.imgur.com/HPvePvX.png)
 
 Based on https://github.com/klayoutmatthias/canvas2canvas
 
 ## Run
```

### Comparing `kweb-0.1.0/docs/Makefile` & `kweb-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kweb-0.1.0/docs/conf.py` & `kweb-0.1.1/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project = "kweb"
-version = "0.1.0"
+version = "0.1.1"
 copyright = "2022"
 # copyright = "2020, gdsfactory"
 # author = "gdsfactory"
 
 # html_theme = "furo"
 # html_theme = "sphinx_rtd_theme"
 html_theme = "sphinx_book_theme"
```

### Comparing `kweb-0.1.0/docs/make.bat` & `kweb-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kweb-0.1.0/pyproject.toml` & `kweb-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	"Programming Language :: Python :: 3.7",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"Operating System :: OS Independent",
 ]
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 dependencies = [
   "klayout >= 0.28.3",
   "fastapi",
   "uvicorn[standard]",
@@ -71,15 +71,15 @@
   | build
   | dist
 )/
 '''
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.1.0"
+version = "0.1.1"
 version_files = [
     "pyproject.toml:version",
 ]
 
 [tool.mypy]
 python_version = "3.10"
 strict = true
```

### Comparing `kweb-0.1.0/src/kweb/main.py` & `kweb-0.1.1/src/kweb/main.py`

 * *Files identical despite different names*

### Comparing `kweb-0.1.0/src/kweb/server.py` & `kweb-0.1.1/src/kweb/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
 import asyncio
 import json
 from collections.abc import Callable
+from pathlib import Path
 from typing import Any
 
 # NOTE: import db to enable stream format readers
 import klayout.db as db
 import klayout.lay as lay
 from fastapi import WebSocket
 from starlette.endpoints import WebSocketEndpoint
@@ -44,20 +45,20 @@
 
     async def on_receive(self, websocket: WebSocket, data: str) -> None:
         await self.reader(websocket, data)
 
     async def on_disconnect(self, websocket: WebSocket, close_code: int) -> None:
         pass
 
-    async def send_image(self, websocket: WebSocket, data: str) -> None:
-        await websocket.send_text(data)
+    async def send_image(self, websocket: WebSocket, data: bytes) -> None:
+        await websocket.send_bytes(data)
 
     def image_updated(self, websocket: WebSocket) -> None:
         pixel_buffer = self.layout_view.get_screenshot_pixels()
-        asyncio.create_task(self.send_image(websocket, str(pixel_buffer.to_png_data())))
+        asyncio.create_task(self.send_image(websocket, pixel_buffer.to_png_data()))
 
     def mode_dump(self) -> list[str]:
         return self.layout_view.mode_names()
 
     def annotation_dump(self) -> list[str]:
         return [d[1] for d in self.layout_view.annotation_templates()]
 
@@ -82,15 +83,15 @@
                 }
             )
         return js
 
     async def connection(self, websocket: WebSocket, path: str | None = None) -> None:
         self.layout_view = lay.LayoutView()
         self.layout_view.load_layout(self.url)
-        if self.layer_props:
+        if Path(self.layer_props).is_file():
             self.layout_view.load_layer_props(self.layer_props)
         self.layout_view.max_hier()
 
         await websocket.send_text(
             json.dumps(
                 {
                     "msg": "loaded",
```

### Comparing `kweb-0.1.0/src/kweb/server_jupyter.py` & `kweb-0.1.1/src/kweb/server_jupyter.py`

 * *Files identical despite different names*

### Comparing `kweb-0.1.0/src/kweb/static/client.css` & `kweb-0.1.1/src/kweb/static/client.css`

 * *Files identical despite different names*

### Comparing `kweb-0.1.0/src/kweb/static/client.js` & `kweb-0.1.1/src/kweb/static/client.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -34,14 +34,15 @@
     let data = evt.data;
     if (typeof(data) === "string") {
 
         //  For debugging:
         //  message.textContent = data;
 
         //  incoming messages are JSON objects
+        console.log(data)
         js = JSON.parse(data);
         if (js.msg == "initialized") {
             initialized = true;
         } else if (js.msg == "loaded") {
             showLayers(js.layers);
             showMenu(js.modes, js.annotations);
         }
```

### Comparing `kweb-0.1.0/src/kweb/templates/client.html` & `kweb-0.1.1/src/kweb/templates/client.html`

 * *Files 17% similar despite different names*

```diff
@@ -16,19 +16,14 @@
       </div>
     </div>
     <div class="viewer-layers-cell">
       <div class="viewer-layers" id="layers"></div>
     </div>
   </div>
 </div>
-<div>
-  <p>{{ url }}</p>
-  <p>{{ gds_file }}</p>
-  <p>{{ layer_props }}</p>
-</div>
 <div id="message">
 </div>
 
 <!-- needs to go here as the simple script will access the DOM -->
 <script>var ws_url="{{ url }}"; var layer_props="{{ layer_props }}"; var gds_file="{{ gds_file }}"</script>
 <script type="text/javascript" src="{{ url_for("static", path="client.js") }}"></script>
```

#### html2text {}

```diff
@@ -1,6 +1,3 @@
 "static", path="client.css") }}>
-{{ url }}
-{{ gds_file }}
-{{ layer_props }}
 
 , path="client.js") }}">
```

### Comparing `kweb-0.1.0/src/kweb.egg-info/PKG-INFO` & `kweb-0.1.1/src/kweb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kweb
-Version: 0.1.0
+Version: 0.1.1
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: ipy
 License-File: LICENSE
 
-# kweb 0.1.0
+# kweb 0.1.1
 
 KLayout Web Viewer ![demo](https://i.imgur.com/HPvePvX.png)
 
 Based on https://github.com/klayoutmatthias/canvas2canvas
 
 ## Run
```

### Comparing `kweb-0.1.0/src/kweb.egg-info/SOURCES.txt` & `kweb-0.1.1/src/kweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

