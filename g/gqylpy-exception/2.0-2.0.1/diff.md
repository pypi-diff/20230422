# Comparing `tmp/gqylpy_exception-2.0.tar.gz` & `tmp/gqylpy_exception-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqylpy_exception-2.0.tar", last modified: Sat Apr 15 04:43:26 2023, max compression
+gzip compressed data, was "gqylpy_exception-2.0.1.tar", last modified: Sat Apr 22 03:32:08 2023, max compression
```

## Comparing `gqylpy_exception-2.0.tar` & `gqylpy_exception-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:43:26.300699 gqylpy_exception-2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-04-15 04:43:14.000000 gqylpy_exception-2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-15 04:43:26.300699 gqylpy_exception-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-15 04:43:14.000000 gqylpy_exception-2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:43:26.296699 gqylpy_exception-2.0/gqylpy_exception/
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-04-15 04:43:14.000000 gqylpy_exception-2.0/gqylpy_exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-04-15 04:43:14.000000 gqylpy_exception-2.0/gqylpy_exception/g exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:43:26.300699 gqylpy_exception-2.0/gqylpy_exception.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-15 04:43:26.000000 gqylpy_exception-2.0/gqylpy_exception.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-15 04:43:26.000000 gqylpy_exception-2.0/gqylpy_exception.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 04:43:26.000000 gqylpy_exception-2.0/gqylpy_exception.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-15 04:43:26.000000 gqylpy_exception-2.0/gqylpy_exception.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 04:43:26.300699 gqylpy_exception-2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-15 04:43:14.000000 gqylpy_exception-2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:32:08.788672 gqylpy_exception-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-04-22 03:31:57.000000 gqylpy_exception-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-22 03:32:08.788672 gqylpy_exception-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-22 03:31:57.000000 gqylpy_exception-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:32:08.788672 gqylpy_exception-2.0.1/gqylpy_exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-22 03:31:57.000000 gqylpy_exception-2.0.1/gqylpy_exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-22 03:31:57.000000 gqylpy_exception-2.0.1/gqylpy_exception/g exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:32:08.788672 gqylpy_exception-2.0.1/gqylpy_exception.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-22 03:32:08.000000 gqylpy_exception-2.0.1/gqylpy_exception.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-22 03:32:08.000000 gqylpy_exception-2.0.1/gqylpy_exception.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 03:32:08.000000 gqylpy_exception-2.0.1/gqylpy_exception.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-22 03:32:08.000000 gqylpy_exception-2.0.1/gqylpy_exception.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 03:32:08.788672 gqylpy_exception-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-22 03:31:57.000000 gqylpy_exception-2.0.1/setup.py
```

### Comparing `gqylpy_exception-2.0/LICENSE` & `gqylpy_exception-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gqylpy_exception-2.0/gqylpy_exception/__init__.py` & `gqylpy_exception-2.0.1/gqylpy_exception/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Create the exception class while executing the `raise` statement, you no longer
 need to define an exception class in advance, Convenient and Fast.
 
     >>> import gqylpy_exception as ge
     >>> raise ge.AnError(...)
 
-    @version: 2.0
+    @version: 2.0.1
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/gqylpy-exception
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -53,26 +53,26 @@
     All exception classes created with `gqylpy_exception` inherit from it, you
     can use it to handle any exception created by `gqylpy_exception`.
     """
     msg: Any
 
 
 def TryExcept(
-        etype:      Union[ExceptionTypes],
+        etype:      ExceptionTypes,
         *,
         silent_exc: Optional[bool]              = None,
         raw_exc:    Optional[bool]              = None,
         logger:     Optional[ExceptionLogger]   = None,
         ereturn:    Optional[Any]               = None,
         ecallback:  Optional[ExceptionCallback] = None,
         eexit:      Optional[bool]              = None
 ) -> Callable:
     """
-    `TryExcept` is a decorator, handles exceptions raised by the function it
-    decorates.
+    `TryExcept` is a decorator (is an additional function of `gqylpy_exception`
+    ), handles exceptions raised by the function it decorates.
 
         >>> @TryExcept(ValueError)
         >>> def func():
         >>>    int('a')
 
     @param etype:      Which exceptions to handle.
     @param silent_exc: If true, exception are processed silently without output,
@@ -100,17 +100,17 @@
         count:      Optional[int]               = None,
         cycle:      Optional[Union[int, float]] = None,
         silent_exc: Optional[bool]              = None,
         raw_exc:    Optional[bool]              = None,
         logger:     Optional[ExceptionLogger]   = None
 ) -> Callable:
     """
-    `Retry` is a decorator, retries exceptions raised by the function it
-    decorates. When an exception is raised in function decorated, try to
-    re-execute the function decorated.
+    `Retry` is a decorator (is an additional function of `gqylpy_exception`),
+    retries exceptions raised by the function it decorates. When an exception is
+    raised in function decorated, try to re-execute the function decorated.
 
         >>> @Retry(count=3, cycle=1)
         >>> def func():
         >>>     int('a')
 
         >>> @TryExcept(ValueError)
         >>> @Retry(count=3, cycle=1)
@@ -139,16 +139,17 @@
         silent_exc: Optional[bool]              = None,
         raw_exc:    Optional[bool]              = None,
         logger:     Optional[ExceptionLogger]   = None,
         ereturn:    Optional[Any]               = None,
         ecallback:  Optional[ExceptionCallback] = None,
         eexit:      Optional[bool]              = None
 ) -> Callable:
-    """`TryExceptAsync` is a decorator, handles exceptions raised by the
-    asynchronous function it decorates."""
+    """`TryExceptAsync` is a decorator (is an additional function of
+    `gqylpy_exception`), handles exceptions raised by the asynchronous function
+    it decorates."""
     warnings.warn(
         f'will be deprecated soon, replaced to {TryExcept}.', DeprecationWarning
     )
     return TryExcept(
         etype,
         silent_exc=silent_exc,
         raw_exc   =raw_exc,
@@ -164,16 +165,17 @@
         *,
         count:      Optional[int]               = None,
         cycle:      Optional[Union[int, float]] = None,
         silent_exc: Optional[bool]              = None,
         raw_exc:    Optional[bool]              = None,
         logger:     Optional[ExceptionLogger]   = None
 ) -> Callable:
-    """`RetryAsync` is a decorator, retries exceptions raised by the
-    asynchronous function it decorates."""
+    """`RetryAsync` is a decorator (is an additional function of
+    `gqylpy_exception`), retries exceptions raised by the asynchronous function
+    it decorates."""
     warnings.warn(
         f'will be deprecated soon, replaced to {Retry}.', DeprecationWarning
     )
     return Retry(
         etype,
         count     =count,
         cycle     =cycle,
```

### Comparing `gqylpy_exception-2.0/gqylpy_exception/g exception.py` & `gqylpy_exception-2.0.1/gqylpy_exception/g exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                     ename[2] != '_' and ename[-3] != '_':
                 raise AttributeError(
                     f'"{__package__}" has no attribute "{ename}".'
                 ) from None
             if ename[-5:] != 'Error':
                 warnings.warn(
                     f'strange exception class "{ename}", exception class name '
-                    'should end with "Error".', UserWarning
+                    'should end with "Error".', UserWarning, stacklevel=2
                 )
             eclass = self.__history__[ename] = type(
                 ename, (self.GqylpyError,), {'__module__': 'builtins'}
             )
             # Compatible with object serialization.
             setattr(builtins, ename, eclass)
         return eclass
```

### Comparing `gqylpy_exception-2.0/setup.py` & `gqylpy_exception-2.0.1/setup.py`

 * *Files identical despite different names*

