# Comparing `tmp/jija-0.2.1.tar.gz` & `tmp/jija-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jija-0.2.1.tar", last modified: Tue Apr 18 13:42:44 2023, max compression
+gzip compressed data, was "jija-0.3.tar", last modified: Sat Apr 22 10:51:19 2023, max compression
```

## Comparing `jija-0.2.1.tar` & `jija-0.3.tar`

### file list

```diff
@@ -1,62 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:42:44.722684 jija-0.2.1/
--rw-r--r--   0 root         (0) root         (0)      181 2023-04-18 13:42:44.722684 jija-0.2.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:42:44.722684 jija-0.2.1/jija/
--rwxr-xr-x   0 root         (0) root         (0)      355 2023-01-23 14:07:37.000000 jija-0.2.1/jija/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5456 2023-04-18 12:51:51.000000 jija-0.2.1/jija/app.py
--rwxr-xr-x   0 root         (0) root         (0)     4455 2023-01-23 14:10:41.000000 jija-0.2.1/jija/apps.py
--rwxr-xr-x   0 root         (0) root         (0)      460 2023-01-22 17:43:04.000000 jija-0.2.1/jija/collector.py
--rwxr-xr-x   0 root         (0) root         (0)      456 2022-11-19 22:00:09.000000 jija-0.2.1/jija/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:42:44.722684 jija-0.2.1/jija/commands/
--rwxr-xr-x   0 root         (0) root         (0)      325 2022-11-05 14:37:03.000000 jija-0.2.1/jija/commands/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      226 2022-11-05 21:57:40.000000 jija-0.2.1/jija/commands/migrate.py
--rwxr-xr-x   0 root         (0) root         (0)     1366 2023-04-18 13:14:24.000000 jija-0.2.1/jija/commands/run.py
--rwxr-xr-x   0 root         (0) root         (0)      299 2023-02-26 05:34:17.000000 jija-0.2.1/jija/commands/runprocess.py
--rwxr-xr-x   0 root         (0) root         (0)       97 2022-11-05 14:37:03.000000 jija-0.2.1/jija/commands/test.py
--rwxr-xr-x   0 root         (0) root         (0)      223 2022-11-05 21:57:40.000000 jija-0.2.1/jija/commands/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:42:44.722684 jija-0.2.1/jija/config/
--rwxr-xr-x   0 root         (0) root         (0)      202 2023-04-18 13:15:44.000000 jija-0.2.1/jija/config/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1162 2023-01-23 14:19:45.000000 jija-0.2.1/jija/config/base.py
--rwxr-xr-x   0 root         (0) root         (0)      597 2022-11-18 11:42:58.000000 jija-0.2.1/jija/config/database.py
--rwxr-xr-x   0 root         (0) root         (0)      678 2023-04-18 13:34:45.000000 jija-0.2.1/jija/config/dev.py
--rwxr-xr-x   0 root         (0) root         (0)      382 2023-02-26 03:28:48.000000 jija-0.2.1/jija/config/docs.py
--rwxr-xr-x   0 root         (0) root         (0)      463 2022-11-18 11:42:58.000000 jija-0.2.1/jija/config/drivers.py
--rwxr-xr-x   0 root         (0) root         (0)      575 2023-01-22 17:43:04.000000 jija-0.2.1/jija/config/fields.py
--rwxr-xr-x   0 root         (0) root         (0)      262 2022-11-18 11:42:58.000000 jija-0.2.1/jija/config/network.py
--rwxr-xr-x   0 root         (0) root         (0)     1207 2022-11-18 11:42:58.000000 jija-0.2.1/jija/config/structute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:42:44.712684 jija-0.2.1/jija/contrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:42:44.722684 jija-0.2.1/jija/contrib/auth/
--rwxr-xr-x   0 root         (0) root         (0)      460 2022-11-19 22:00:09.000000 jija-0.2.1/jija/contrib/auth/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:42:44.722684 jija-0.2.1/jija/docs/
--rwxr-xr-x   0 root         (0) root         (0)       29 2023-01-22 17:43:04.000000 jija-0.2.1/jija/docs/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4563 2023-02-26 05:35:18.000000 jija-0.2.1/jija/docs/processor.py
--rwxr-xr-x   0 root         (0) root         (0)     1361 2023-02-26 03:58:21.000000 jija-0.2.1/jija/docs/setup.py
--rwxr-xr-x   0 root         (0) root         (0)      240 2023-01-22 17:43:04.000000 jija-0.2.1/jija/docs/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:42:44.722684 jija-0.2.1/jija/drivers/
--rwxr-xr-x   0 root         (0) root         (0)      105 2022-11-18 11:42:58.000000 jija-0.2.1/jija/drivers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       22 2022-11-18 11:42:58.000000 jija-0.2.1/jija/drivers/base.py
--rwxr-xr-x   0 root         (0) root         (0)     1446 2022-11-19 22:00:09.000000 jija-0.2.1/jija/drivers/database.py
--rwxr-xr-x   0 root         (0) root         (0)       72 2022-11-18 11:42:58.000000 jija-0.2.1/jija/drivers/docs.py
--rwxr-xr-x   0 root         (0) root         (0)      171 2023-01-22 17:43:04.000000 jija-0.2.1/jija/exceptions.py
--rwxr-xr-x   0 root         (0) root         (0)      270 2023-01-22 17:43:04.000000 jija-0.2.1/jija/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:42:44.722684 jija-0.2.1/jija/middlewares/
--rwxr-xr-x   0 root         (0) root         (0)       28 2022-11-05 14:37:03.000000 jija-0.2.1/jija/middlewares/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      966 2022-11-05 14:37:03.000000 jija-0.2.1/jija/middlewares/print_request.py
--rwxr-xr-x   0 root         (0) root         (0)     1785 2023-04-18 13:41:23.000000 jija-0.2.1/jija/reloader.py
--rwxr-xr-x   0 root         (0) root         (0)     1370 2023-01-22 17:43:04.000000 jija-0.2.1/jija/response.py
--rwxr-xr-x   0 root         (0) root         (0)     2079 2023-04-18 00:55:04.000000 jija-0.2.1/jija/router.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:42:44.722684 jija-0.2.1/jija/serializers/
--rwxr-xr-x   0 root         (0) root         (0)      138 2023-01-22 17:43:04.000000 jija-0.2.1/jija/serializers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      310 2023-01-22 17:43:04.000000 jija-0.2.1/jija/serializers/exceptions.py
--rwxr-xr-x   0 root         (0) root         (0)     2902 2023-01-22 17:55:13.000000 jija-0.2.1/jija/serializers/fields.py
--rwxr-xr-x   0 root         (0) root         (0)     1331 2023-01-22 17:43:04.000000 jija-0.2.1/jija/serializers/serializer.py
--rwxr-xr-x   0 root         (0) root         (0)     2640 2023-01-22 17:43:04.000000 jija-0.2.1/jija/serializers/validators.py
--rwxr-xr-x   0 root         (0) root         (0)     5937 2023-04-18 03:59:37.000000 jija-0.2.1/jija/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:42:44.722684 jija-0.2.1/jija.egg-info/
--rw-r--r--   0 root         (0) root         (0)      181 2023-04-18 13:42:44.000000 jija-0.2.1/jija.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1112 2023-04-18 13:42:44.000000 jija-0.2.1/jija.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 13:42:44.000000 jija-0.2.1/jija.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 13:42:44.000000 jija-0.2.1/jija.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       83 2023-04-18 13:42:44.000000 jija-0.2.1/jija.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-18 13:42:44.000000 jija-0.2.1/jija.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 13:42:44.722684 jija-0.2.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      564 2023-04-18 13:42:39.000000 jija-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:51:19.156313 jija-0.3/
+-rw-r--r--   0 root         (0) root         (0)      256 2023-04-22 10:51:19.156313 jija-0.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:51:19.146313 jija-0.3/jija/
+-rwxr-xr-x   0 root         (0) root         (0)      308 2023-04-20 16:55:27.000000 jija-0.3/jija/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6316 2023-04-22 10:21:56.000000 jija-0.3/jija/app.py
+-rwxr-xr-x   0 root         (0) root         (0)     4247 2023-04-20 22:18:05.000000 jija-0.3/jija/apps.py
+-rwxr-xr-x   0 root         (0) root         (0)      513 2023-04-20 22:16:18.000000 jija-0.3/jija/collector.py
+-rwxr-xr-x   0 root         (0) root         (0)      456 2022-11-19 22:00:09.000000 jija-0.3/jija/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:51:19.156313 jija-0.3/jija/config/
+-rwxr-xr-x   0 root         (0) root         (0)      136 2023-04-20 15:42:10.000000 jija-0.3/jija/config/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1162 2023-01-23 14:19:45.000000 jija-0.3/jija/config/base.py
+-rwxr-xr-x   0 root         (0) root         (0)      685 2023-04-20 10:04:29.000000 jija-0.3/jija/config/dev.py
+-rwxr-xr-x   0 root         (0) root         (0)      928 2023-04-20 15:19:31.000000 jija-0.3/jija/config/drivers.py
+-rwxr-xr-x   0 root         (0) root         (0)      290 2023-04-20 13:46:57.000000 jija-0.3/jija/config/network.py
+-rwxr-xr-x   0 root         (0) root         (0)     1280 2023-04-20 13:50:19.000000 jija-0.3/jija/config/structute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:51:19.156313 jija-0.3/jija/drivers/
+-rwxr-xr-x   0 root         (0) root         (0)       90 2023-04-20 14:55:05.000000 jija-0.3/jija/drivers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      163 2023-04-20 15:18:55.000000 jija-0.3/jija/drivers/base.py
+-rwxr-xr-x   0 root         (0) root         (0)      270 2023-04-20 15:29:36.000000 jija-0.3/jija/drivers/database.py
+-rwxr-xr-x   0 root         (0) root         (0)       72 2023-04-20 14:28:01.000000 jija-0.3/jija/drivers/docs.py
+-rwxr-xr-x   0 root         (0) root         (0)      171 2023-01-22 17:43:04.000000 jija-0.3/jija/exceptions.py
+-rwxr-xr-x   0 root         (0) root         (0)      270 2023-01-22 17:43:04.000000 jija-0.3/jija/middleware.py
+-rwxr-xr-x   0 root         (0) root         (0)     1829 2023-04-20 10:04:29.000000 jija-0.3/jija/reloader.py
+-rwxr-xr-x   0 root         (0) root         (0)     1370 2023-01-22 17:43:04.000000 jija-0.3/jija/response.py
+-rwxr-xr-x   0 root         (0) root         (0)     2281 2023-04-20 21:45:15.000000 jija-0.3/jija/router.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:51:19.156313 jija-0.3/jija/serializers/
+-rwxr-xr-x   0 root         (0) root         (0)      138 2023-01-22 17:43:04.000000 jija-0.3/jija/serializers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      310 2023-01-22 17:43:04.000000 jija-0.3/jija/serializers/exceptions.py
+-rwxr-xr-x   0 root         (0) root         (0)     3305 2023-04-20 13:50:19.000000 jija-0.3/jija/serializers/fields.py
+-rwxr-xr-x   0 root         (0) root         (0)     1283 2023-04-20 11:10:56.000000 jija-0.3/jija/serializers/serializer.py
+-rwxr-xr-x   0 root         (0) root         (0)     3220 2023-04-20 13:50:19.000000 jija-0.3/jija/serializers/validators.py
+-rwxr-xr-x   0 root         (0) root         (0)     6044 2023-04-20 14:13:13.000000 jija-0.3/jija/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:51:19.156313 jija-0.3/jija.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      256 2023-04-22 10:51:19.000000 jija-0.3/jija.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      726 2023-04-22 10:51:19.000000 jija-0.3/jija.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 10:51:19.000000 jija-0.3/jija.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 10:51:19.000000 jija-0.3/jija.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-22 10:51:19.000000 jija-0.3/jija.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-22 10:51:19.000000 jija-0.3/jija.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 10:51:19.156313 jija-0.3/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      522 2023-04-22 10:51:00.000000 jija-0.3/setup.py
```

### Comparing `jija-0.2.1/jija/apps.py` & `jija-0.3/jija/apps.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,45 @@
 from __future__ import annotations
 
-from aiohttp import web
-import asyncio
+from typing import TYPE_CHECKING, Type, Optional
+if TYPE_CHECKING:
+    from jija.config.base import Config
 
 from pathlib import Path
 import importlib
+import asyncio
 import sys
 import os
 
-from typing import List, TYPE_CHECKING
-if TYPE_CHECKING:
-    from jija.config.base import Config
-
-
 from jija.collector import collect_subclasses
-from jija import middlewares
-from jija import commands
-from jija import app
+from jija.command import Command
+import jija.base_app.app
 from jija import config
+from jija import app
 
 
 class AppGetter(type):
-    def __getattr__(self, item):
-        """
-        :type item: str
-        :rtype: App
-        """
-
+    def __getattr__(self, item: str) -> app.App:
         jija_app = Apps.apps.get(item)
         if jija_app:
             return jija_app
 
         raise AttributeError(item)
 
 
 class Apps(metaclass=AppGetter):
-    apps = {}
-    commands = {
-        'system': commands.COMMANDS
-    }
+    apps: dict[str, app.App] = {}
 
     __REQUIRED_CONFIGS = {
         config.StructureConfig,
         config.DriversConfig,
         config.NetworkConfig
     }
 
-    __INITED_CONFIGS: List[Config] = []
+    __INITED_CONFIGS: list[Config] = []
     __PREFLIGHT_TASKS = []
 
     @classmethod
     def load(cls):
         cls.__init_configs()
         Apps.apps['core'] = cls.__create_base_app()
         cls.__collect(config.StructureConfig.APPS_PATH, Apps.apps['core'])
@@ -71,36 +60,34 @@
     @classmethod
     async def __freeze_configs(cls):
         for config_class in cls.__INITED_CONFIGS:
             await config_class.freeze()
             cls.__PREFLIGHT_TASKS.append(config_class.preflight)
 
     @classmethod
-    def __create_base_app(cls):
-        """
-        :rtype: web.Application
-        """
-
-        aiohttp_app = web.Application()
-
-        aiohttp_app.middlewares.extend([
-            middlewares.print_request.PrintRequest(),
-        ])
+    def __create_base_app(cls) -> app.App:
+        base_app = jija.base_app.app.BaseApp.construct(
+            name='core',
+            path=Path(jija.base_app.app.__file__).parent,
+            parent=None,
+        )
 
         if cls.app_exists(config.StructureConfig.CORE_PATH):
-            app_class = cls.get_modify_class(config.StructureConfig.CORE_PATH)
+            core_app = cls.get_modify_class(config.StructureConfig.CORE_PATH).construct(
+                name='core',
+                path=config.StructureConfig.CORE_PATH,
+                extends=base_app
+            )
         else:
-            app_class = app.App
+            core_app = base_app
 
         for config_unit in cls.__INITED_CONFIGS:
-            aiohttp_app = config_unit.base_app_update(aiohttp_app)
+            core_app.aiohttp_app_update(config_unit.base_app_update(core_app.aiohttp_app))
 
-        jija_app = app_class(path=config.StructureConfig.CORE_PATH, aiohttp_app=aiohttp_app, name='core')
-
-        return jija_app
+        return core_app
 
     @staticmethod
     def app_exists(path: Path) -> bool:
         return path.joinpath('app.py').exists()
 
     @classmethod
     def __collect(cls, path: Path, parent: app.App):
@@ -108,49 +95,40 @@
             return
 
         for sub_app_name in os.listdir(path):
             sub_app_name: str
 
             next_path = path.joinpath(sub_app_name)
             if app.App.is_app(next_path):
-                jija_app = cls.get_modify_class(next_path)(path=next_path, parent=parent, name=sub_app_name)
-                cls.commands[sub_app_name] = jija_app.commands
+                jija_app = cls.get_modify_class(next_path).construct(path=next_path, parent=parent, name=sub_app_name)
                 cls.apps[sub_app_name] = jija_app
                 cls.__collect(path.joinpath(sub_app_name), jija_app)
 
     @staticmethod
-    def get_modify_class(path: Path) -> type:
+    def get_modify_class(path: Path) -> Type[app.App]:
         modify_class_path = path.joinpath('app')
         import_path = ".".join(modify_class_path.relative_to(config.StructureConfig.PROJECT_PATH).parts)
 
         module = importlib.import_module(import_path)
         modify_class = list(collect_subclasses(module, app.App))
         return modify_class[0] if modify_class else app.App
 
     @classmethod
     def __register_apps(cls):
         cls.apps['core'].register()
 
     @classmethod
-    def get_command(cls, module, command):
-        """
-        :type module: str
-        :type command: str
-        :rtype: type
-        """
-
-        if module is None:
-            module = 'system'
-
-        return cls.commands[module][command]
+    def get_command(cls, module: Optional[list[str]], command: str) -> Type[Command]:
+        return cls.apps[module or 'core'].commands[command]
 
     @classmethod
     def run_command(cls):
         args = sys.argv
         command = args[1].split('.')
+
         Apps.load()
         asyncio.get_event_loop().run_until_complete(cls.__preflight())
 
         if len(command) == 1:
             module = None
             command = command[0]
         else:
```

### Comparing `jija-0.2.1/jija/config/base.py` & `jija-0.3/jija/config/base.py`

 * *Files identical despite different names*

### Comparing `jija-0.2.1/jija/config/dev.py` & `jija-0.3/jija/config/dev.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from jija.config import base
 
 
 class DevConfig(base.Config):
-    RELOADER_EXCLUDED_DIRS: set
+    RELOADER_EXCLUDED_DIRS: set = None
 
     def __init__(self, *, reloader_excluded=None):
         self.__class__.__PREF = {
             'RELOADER_EXCLUDED_DIRS': reloader_excluded if reloader_excluded else set()
         }
 
         super().__init__()
```

### Comparing `jija-0.2.1/jija/config/structute.py` & `jija-0.3/jija/config/structute.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from jija.config import base, fields
+from jija.config import base
+from jija.serializers import fields
 
 from pathlib import Path as Path
 import sys
 
 
 class StructureConfig(base.Config):
-    PROJECT_PATH = None
+    PROJECT_PATH: Path = fields.InstanceField(instance_pattern=Path)
     CORE_PATH = None
     APPS_PATH = None
     PYTHON_PATH = fields.CharField(default=sys.executable)
 
     def __init__(self, *, project_path=None, core_dir='core', apps_dir='apps', python_path=None):
         super().__init__(project_path=project_path, core_dir=core_dir, apps_dir=apps_dir, python_path=python_path)
```

### Comparing `jija-0.2.1/jija/reloader.py` & `jija-0.3/jija/reloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             pre_hash = hashlib.sha1()
 
         files = os.listdir(path)
 
         for file in files:
             next_path = f'{path}/{file}'
 
-            if next_path in config.DevConfig.RELOADER_EXCLUDED_DIRS:
+            if config.DevConfig.RELOADER_EXCLUDED_DIRS and next_path in config.DevConfig.RELOADER_EXCLUDED_DIRS:
                 continue
 
             if os.path.isdir(next_path):
                 pre_hash = await self.__get_hash(next_path, pre_hash)
 
             else:
                 async with aiofile.async_open(next_path, 'rb') as buffer:
```

### Comparing `jija-0.2.1/jija/response.py` & `jija-0.3/jija/response.py`

 * *Files identical despite different names*

### Comparing `jija-0.2.1/jija/router.py` & `jija-0.3/jija/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,23 +28,29 @@
 
     def __repr__(self):
         return f'<{self.__class__.__name__}: {len(self.endpoints)} endpoints, {len(self.__routes)} routes>'
 
     def __str__(self):
         return self.__repr__()
 
+    def __add__(self, other):
+        if not isinstance(other, Router):
+            raise TypeError(f'Can not add "Router" to {type(other)}')
+
+        return Router(self.endpoints + other.endpoints)
+
 
 class AbsEndpoint:
     def generate_routes(self, prefix=''):
         raise NotImplementedError()
 
 
 class Endpoint(AbsEndpoint):
-    def __init__(self, path, view: typing.Type[views.ViewBase]):
-        if not issubclass(view, views.ViewBase):
+    def __init__(self, path, view: typing.Type[views._ViewBase]):
+        if not issubclass(view, views._ViewBase):
             raise AttributeError(f'view must be a subclass of "jija.views.ViewBase", got {view}')
 
         self.__path = path
         self.__view = view
 
     @property
     def path(self) -> str:
```

### Comparing `jija-0.2.1/jija/serializers/fields.py` & `jija-0.3/jija/serializers/fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -112,7 +112,24 @@
 
 class SelectField(Field):
     validators = (OptionsValidator,)
 
     def __init__(self, *, options, **kwargs):
         super().__init__(**kwargs)
         self.options = options
+
+
+class ClassField(Field):
+    validators = SubclassValidator,
+
+    def __init__(self, *, class_pattern, **kwargs):
+        self.class_pattern = class_pattern
+        super().__init__(**kwargs)
+
+
+class InstanceField(Field):
+    validators = (InstanceValidator,)
+
+    def __init__(self, *, instance_pattern, **kwargs):
+        self.instance_pattern = instance_pattern
+        super().__init__(**kwargs)
+
```

### Comparing `jija-0.2.1/jija/serializers/serializer.py` & `jija-0.3/jija/serializers/serializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,16 +40,13 @@
 
         self.__valid = len(self.errors) == 0
         if not self.__valid:
             print(self.errors)
 
         return self.__valid
 
-    async def out_validate(self):
-        pass
-
     @property
     def valid(self):
         return self.__valid
 
     def clean(self):
         pass
```

### Comparing `jija-0.2.1/jija/serializers/validators.py` & `jija-0.3/jija/serializers/validators.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,7 +85,25 @@
 class OptionsValidator(Validator):
     @classmethod
     async def validate(cls, value, field):
         if value not in field.options:
             raise ValidationError(f'Недопустимое значение', value)
 
         return value
+
+
+class SubclassValidator(Validator):
+    @classmethod
+    async def validate(cls, value, field):
+        if not issubclass(value, field.class_pattern):
+            raise ValidationError(f'Value must be subclass of {field.class_pattern}, not {type(value)}', value)
+
+        return value
+
+
+class InstanceValidator(Validator):
+    @classmethod
+    async def validate(cls, value, field):
+        if not isinstance(value, field.instance_pattern):
+            raise ValidationError(f'Value must be instance of {field.instance_pattern}, not {type(value)}', value)
+
+        return value
```

### Comparing `jija-0.2.1/jija/views.py` & `jija-0.3/jija/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import inspect
 import json
-from typing import Union
+from typing import Union, Type
 
 import aiohttp.http_websocket
 from aiohttp import web
 
 from jija import response, serializers, exceptions
 
 
-class ViewBase:
+class _ViewBase:
     def __init__(self, request: web.Request, path_params: web.UrlMappingMatchInfo):
         self.__request = request
         self.__path_params = path_params
 
     @property
     def request(self) -> web.Request:
         return self.__request
@@ -33,21 +33,17 @@
         except exceptions.ViewForceExit as exception:
             return exception.response
 
     async def dispatch(self):
         raise NotImplementedError()
 
 
-class View(ViewBase):
+class View(_ViewBase):
     methods = ('get', 'post', 'patch', 'put', 'delete')
 
-    serializers_in = None
-
-    # serializers_out = None TODO
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.__method = self.request.method.lower()
         self.__data: dict = {}
 
     @property
@@ -64,31 +60,25 @@
         for method in cls.methods:
             if hasattr(cls, method):
                 view_methods.append(method)
 
         return view_methods
 
     async def dispatch(self):
-        try:
-            await self.load_data()
-            handler = getattr(self, self.method)
-            return await handler() if inspect.iscoroutinefunction(handler) else handler()
-
-        except serializers.SerializeError as error:
-            return response.JsonResponse(error.serializer.errors, status=400)
+        await self.load_data()
+        handler = getattr(self, self.method)
+        return await self.run_handler(handler)
 
     async def load_data(self):
-        data = {
+        self.__data = {
             **await self.parse_body(),
             **self.parse_path(),
             **self.parse_query()
         }
 
-        self.__data = await self.in_serialize(data)
-
     async def parse_body(self) -> dict:
         if self.method != 'get':
             try:
                 return await self.request.json()
             except json.JSONDecodeError:
                 return {}
 
@@ -105,67 +95,82 @@
             if len(value) == 1:
                 value = value[0]
 
             data[key] = value
 
         return data
 
-    async def in_serialize(self, data: dict) -> dict:
-        serializer_class = await self.get_in_serializer(self.method)
-        if serializer_class:
-            serializer = serializer_class(data)
-            await serializer.in_serialize()
+    async def run_handler(self, handler):
+        if inspect.iscoroutinefunction(handler):
+            return await handler()
+        else:
+            return handler()
 
-            if not serializer.valid:
-                raise serializers.SerializeError(serializer)
 
-            return serializer.data
+class _SerializedViewMeta(type):
+    def __new__(mcs, name, bases, attrs):
+        cls = super().__new__(mcs, name, bases, attrs)
 
-        return data
+        for method in cls.get_methods():
+            handler = getattr(cls, method)
+            cls.__annotate_serializers(handler)
 
-    async def out_serialize(self, response) -> web.Response:
-        # if isinstance(response, SerializeResponse): TODO
-        #
-        #     serializer_class = await self.get_out_serializer(self.method)
-        #     if not serializer_class:
-        #         raise ValueError('Got SerializerResponse, but out serializer not set')
-        #
-        #     return await response.serialize(serializer_class)
+        return cls
 
-        return response
+    @staticmethod
+    def __annotate_serializers(handler):
+        handler_serializers = {}
+        for name, arg in inspect.signature(handler).parameters.items():
+            if name == 'self':
+                continue
 
-    @classmethod
-    async def get_in_serializer(cls, method):
-        return cls.serializers_in and cls.serializers_in[method]
+            if issubclass(arg.annotation, serializers.Serializer):
+                handler_serializers[name] = arg.annotation
+
+        handler.__serializers__ = handler_serializers
 
-    # @classmethod TODO
-    # async def get_out_serializer(cls, method):
-    #     return cls.serializers_out and cls.serializers_out[method]
-
-
-class SerializersSet:
-    def __init__(self, get=None, post=None, put=None, path=None, delete=None, **kwargs):
-        self.__serializers = {
-            'get': get,
-            'post': post,
-            'put': put,
-            'path': path,
-            'delete': delete,
-            **kwargs
-        }
 
-    def __getitem__(self, item):
-        return self.__serializers[item]
+class SerializedView(View, metaclass=_SerializedViewMeta):
+    async def dispatch(self):
+        try:
+            return await super().dispatch()
+
+        except serializers.SerializeError as error:
+            return response.JsonResponse(error.serializer.errors, status=400)
+
+    async def run_handler(self, handler):
+        data = await self.in_serialize(handler.__serializers__)
+        if inspect.iscoroutinefunction(handler):
+            return await handler(**data)
+        else:
+            return handler(**data)
+
+    async def in_serialize(
+            self,
+            handler_serializers: dict[str, Type[serializers.Serializer]]
+    ) -> dict[str, serializers.Serializer]:
+
+        data = {}
+        for name, serializer_class in handler_serializers.items():
+            serializer = serializer_class(self.data)
+            await serializer.in_serialize()
+
+            if not serializer.valid:
+                raise serializers.SerializeError(serializer)
+
+            data[name] = serializer
+
+        return data
 
 
 class DocMixin:
     pass
 
 
-class WSView(ViewBase):
+class WSView(_ViewBase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.__ws = None
 
     @classmethod
     def get_methods(cls):
         return 'get',
```

