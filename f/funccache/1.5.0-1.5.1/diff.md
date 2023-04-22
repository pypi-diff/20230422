# Comparing `tmp/funccache-1.5.0.tar.gz` & `tmp/funccache-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funccache-1.5.0.tar", last modified: Sat Apr  8 02:35:44 2023, max compression
+gzip compressed data, was "funccache-1.5.1.tar", last modified: Sat Apr 22 03:34:30 2023, max compression
```

## Comparing `funccache-1.5.0.tar` & `funccache-1.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:35:44.701300 funccache-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-04-08 02:35:31.000000 funccache-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-08 02:35:44.701300 funccache-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-08 02:35:31.000000 funccache-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:35:44.701300 funccache-1.5.0/funccache/
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-08 02:35:31.000000 funccache-1.5.0/funccache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-04-08 02:35:31.000000 funccache-1.5.0/funccache/i funccache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:35:44.701300 funccache-1.5.0/funccache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-08 02:35:44.000000 funccache-1.5.0/funccache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-08 02:35:44.000000 funccache-1.5.0/funccache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 02:35:44.000000 funccache-1.5.0/funccache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-08 02:35:44.000000 funccache-1.5.0/funccache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 02:35:44.701300 funccache-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-08 02:35:31.000000 funccache-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:34:30.771948 funccache-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-04-22 03:34:19.000000 funccache-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-22 03:34:30.771948 funccache-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-22 03:34:19.000000 funccache-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:34:30.771948 funccache-1.5.1/funccache/
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-22 03:34:19.000000 funccache-1.5.1/funccache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-04-22 03:34:19.000000 funccache-1.5.1/funccache/i funccache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:34:30.771948 funccache-1.5.1/funccache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-22 03:34:30.000000 funccache-1.5.1/funccache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-22 03:34:30.000000 funccache-1.5.1/funccache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 03:34:30.000000 funccache-1.5.1/funccache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-22 03:34:30.000000 funccache-1.5.1/funccache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 03:34:30.771948 funccache-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-22 03:34:19.000000 funccache-1.5.1/setup.py
```

### Comparing `funccache-1.5.0/LICENSE` & `funccache-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `funccache-1.5.0/PKG-INFO` & `funccache-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funccache
-Version: 1.5.0
+Version: 1.5.1
 Summary: 如其名，它实现缓存功能，可缓存某个函数或某个类中定义的所有方法的返回值。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/funccache
 Classifier: Environment :: Web Environment
```

### Comparing `funccache-1.5.0/README.md` & `funccache-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `funccache-1.5.0/funccache/__init__.py` & `funccache-1.5.1/funccache/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     >>> class Alpha(metaclass=funccache):
     >>>     ...
 
     >>> @funccache
     >>> def alpha():
     >>>     ...
 
-    @version: 1.5.0
+    @version: 1.5.1
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/funccache
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -34,30 +34,29 @@
 
 def expiration_time(expires: int = -1):
     """Decorator, can select the cache duration, by the parament `expires`, less
     than or equal to 0 means immediate expiration."""
 
 
 def clear_cache_pool(func) -> None:
-    """Clears the cache pool for the specified function or object or class."""
+    """Clear the cache pool for the specified function or object or class."""
     func.__cache_pool__.clear()
 
 
 class _xe6_xad_x8c_xe7_x90_xaa_xe6_x80_xa1_xe7_x8e_xb2_xe8_x90_x8d_xe4_xba_x91:
     import sys
 
-    gpath = f'{__name__}.i {__name__}'
-    __import__(gpath)
-
+    __import__(f'{__name__}.i {__name__}')
     gcode = globals()[f'i {__name__}']
+
     FuncCache = gcode.FuncCache
 
     for gname, gvalue in globals().items():
         if gname[0] == '_' and gname != '__builtins__':
             setattr(FuncCache, gname, gvalue)
 
     FuncCache.__module__       = __package__
-    FuncCache.FuncCache        = gcode.FuncCache
+    FuncCache.FuncCache        = FuncCache
     FuncCache.expiration_time  = gcode.FunctionCallerExpirationTime
     FuncCache.clear_cache_pool = gcode.clear_cache_pool
 
     sys.modules[__name__] = FuncCache
```

### Comparing `funccache-1.5.0/funccache/i funccache.py` & `funccache-1.5.1/funccache/i funccache.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 limitations under the License.
 """
 import time
 import asyncio
 import threading
 import functools
 
-Function: type = threading.setprofile.__class__
+FunctionType: type = threading.setprofile.__class__
 
 
 class FuncCache(type):
     __shared_instance_cache__ = False
     __not_cache__ = []
 
     def __new__(mcs, __name__: str, *a, **kw):
-        if isinstance(__name__, (Function, type)):
+        if isinstance(__name__, (FunctionType, type)):
             return FunctionCaller(__name__)
         return type.__new__(mcs, __name__, *a, **kw)
 
     def __init__(cls, __name__: str, __bases__: tuple, __dict__: dict):
         __not_cache__: list = __dict__.get('__not_cache__')
 
         if __not_cache__:
@@ -188,18 +188,18 @@
     def __str__(self):
         return f'{ClassMethodCaller.__name__}' \
                f'({self.__cls.__module__}.{self.__qualname__})'
 
 
 class FunctionCaller:
 
-    def __init__(self, func: Function):
+    def __init__(self, func: FunctionType):
         self.__func__ = func
 
-        if func.__class__ is Function:
+        if func.__class__ is FunctionType:
             self.__globals__ = func.__globals__
             functools.wraps(self.__func__)(self)
 
             if asyncio.iscoroutinefunction(getattr(func, '__wrapped__', func)):
                 self.__core__ = self.__core_async__
 
         self.__exec_lock__  = threading.Lock()
@@ -240,15 +240,15 @@
 
     def __init__(self, expires: int = -1):
         self.__expires = expires
 
         self.__exec_lock__  = threading.Lock()
         self.__cache_pool__ = {}
 
-    def __call__(self, func: Function):
+    def __call__(self, func: FunctionType):
         self.__func__ = func
 
         if asyncio.iscoroutinefunction(getattr(func, '__wrapped__', func)):
             self.__core__ = self.__core_async__
 
         @functools.wraps(func, updated=('__dict__', '__globals__'))
         def inner(*a, **kw):
```

### Comparing `funccache-1.5.0/funccache.egg-info/PKG-INFO` & `funccache-1.5.1/funccache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funccache
-Version: 1.5.0
+Version: 1.5.1
 Summary: 如其名，它实现缓存功能，可缓存某个函数或某个类中定义的所有方法的返回值。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/funccache
 Classifier: Environment :: Web Environment
```

### Comparing `funccache-1.5.0/setup.py` & `funccache-1.5.1/setup.py`

 * *Files identical despite different names*

