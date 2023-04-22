# Comparing `tmp/pyrew-0.5.2.tar.gz` & `tmp/pyrew-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrew-0.5.2.tar", last modified: Sat Apr 22 06:04:11 2023, max compression
+gzip compressed data, was "pyrew-0.6.2.tar", last modified: Sat Apr 22 06:40:21 2023, max compression
```

## Comparing `pyrew-0.5.2.tar` & `pyrew-0.6.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 06:04:11.057977 pyrew-0.5.2/
--rw-rw-rw-   0        0        0      610 2023-04-22 06:04:11.056656 pyrew-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      386 2023-04-22 06:03:39.000000 pyrew-0.5.2/README.rst
--rw-rw-rw-   0        0        0       91 2023-04-22 04:22:49.000000 pyrew-0.5.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-22 06:04:11.053394 pyrew-0.5.2/pyrew.egg-info/
--rw-rw-rw-   0        0        0      610 2023-04-22 06:04:10.000000 pyrew-0.5.2/pyrew.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-04-22 06:04:10.000000 pyrew-0.5.2/pyrew.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 06:04:10.000000 pyrew-0.5.2/pyrew.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-22 06:04:10.000000 pyrew-0.5.2/pyrew.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6187 2023-04-22 06:04:00.000000 pyrew-0.5.2/pyrew.py
--rw-rw-rw-   0        0        0       42 2023-04-22 06:04:11.057977 pyrew-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0      497 2023-04-22 06:04:02.000000 pyrew-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:40:21.782803 pyrew-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 06:40:21.782803 pyrew-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-22 06:40:08.000000 pyrew-0.6.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 06:40:08.000000 pyrew-0.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:40:21.782803 pyrew-0.6.2/pyrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 06:40:21.000000 pyrew-0.6.2/pyrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-22 06:40:21.000000 pyrew-0.6.2/pyrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 06:40:21.000000 pyrew-0.6.2/pyrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 06:40:21.000000 pyrew-0.6.2/pyrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-04-22 06:40:08.000000 pyrew-0.6.2/pyrew.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 06:40:21.782803 pyrew-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-22 06:40:08.000000 pyrew-0.6.2/setup.py
```

### Comparing `pyrew-0.5.2/pyrew.py` & `pyrew-0.6.2/pyrew.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,229 +1,229 @@
-import sys
-import builtins
-import importlib
-import os
-from contextlib import contextmanager
-import logging
-import asyncio
-import time
-import itertools
-import threading
-import re
-
-try:
-    import colorama
-    colorama.init()
-
-except ImportError:
-    pass
-
-class MultiException(Exception):
-    def __init__(self, exceptions):
-        self.exceptions = exceptions
-        super().__init__(f"{len(exceptions)} exceptions occurred")
-
-class Pyrew:
-    @staticmethod
-    def write(*args, end='\n'):
-
-        args_list = list(args)
-
-        for i in range(len(args_list)):
-            if args_list[i] is None:
-                args_list[i] = ''
-
-        if end is None:
-            __end__ = ''
-        else:
-            __end__ = end
-        
-        output = ''.join(str(arg) for arg in args_list)
-        sys.stdout.write(f"{output}{__end__}")
-
-    class files:
-
-        class cwd:
-
-            @staticmethod
-            def append(path, content):
-                with open(os.path.join(os.getcwd(), path), 'a') as f:
-                    f.write(content)
-
-            @staticmethod
-            def read(path):
-                with open(os.path.join(os.getcwd(), path), 'r') as f:
-                    return str(f.read(f))
-                
-            @staticmethod
-            def write(path, content):
-                with open(os.path.join(os.getcwd(), path), 'w') as f:
-                    f.write(content)
-                
-        @staticmethod
-        def append(path, content):
-            with open(path, 'a') as f:
-                f.write(content)
-
-        @staticmethod
-        def read(path):
-            with open(path, 'r') as f:
-                return str(f.read(f))
-            
-        @staticmethod
-        def write(path, content):
-            with open(path, 'w') as f:
-                f.write(content)
-
-    @staticmethod
-    @contextmanager
-    def run(n):
-        for i in range(n):
-            yield i
-
-    @staticmethod
-    def throw(*exceptions):
-        if len(exceptions) == 1:
-            raise exceptions[0]
-
-        raise MultiException(exceptions)
-
-    class log:
-
-        @staticmethod
-        def warn(message):
-            logging.warning(message)
-            
-        @staticmethod
-        def error(message):
-            logging.error(message)
-
-        @staticmethod
-        def info(message):
-            logging.info(message)
-        
-        @staticmethod
-        def debug(message):
-            logging.debug(message)
-
-        @staticmethod
-        def clear():
-            os.system('cls' if os.name == 'nt' else 'clear')
-
-    @staticmethod
-    def tupmod(tup, index, val):
-        return tup[:index] + (val,) + tup[index + 1:]
-    
-    @staticmethod
-    def set_timeout(func, n=None, timeout=None):
-
-        if n is None:
-            n = 1
-
-        for i in range(n):
-
-            if timeout is None:
-                timeout = 0
-            
-            time.sleep(timeout)
-            func()
-
-    class sh:
-
-        @staticmethod
-        def run(*cmds):
-            for cmd in cmds:
-                confirm = input(f"You are about to do something potentially dangerous. Are you sure you want to run \"{cmd}\"? y/N: ")
-                if confirm.lower() in ["y", "yes"]:
-                    os.system(cmd)
-                else:
-                    print(f"Cancelled action \"{cmd}\"! Good call.")
-
-        class cwd:
-
-            @staticmethod
-            def run(*cmds):
-
-                cwd = os.getcwd()
-
-                for cmd in cmds:
-
-                    confirm = input(f"You are about to do something potentially dangerous. Are you sure you want to run \"{cmd}\"? y/N: ")
-
-                    if confirm.lower() in ["y", "yes"]:
-                        os.chdir(cwd)
-                        os.system(cmd)
-
-                    else:
-                        print(f"Cancelled action \"{cmd}\" in \"{cwd}\"! Good call.")
-
-    @staticmethod
-    def spin(func):
-        
-        spinner = itertools.cycle(
-                [
-                    f"\033[31m\u2015\033[0m",
-                    f"\033[32m/\033[0m", 
-                    f"\033[33m|\033[0m", 
-                    f"\033[34m\\\033[0m"
-                ]
-            )
-        
-        stop_spinner = threading.Event()
-
-        def animate():
-            while not stop_spinner.is_set():
-                sys.stdout.write("\rRunning... " + next(spinner))
-                sys.stdout.flush()
-                time.sleep(0.1)
-        
-        spinner_thread = threading.Thread(target=animate)
-        spinner_thread.start()
-
-        try:
-            func()
-
-        finally:
-            stop_spinner.set()
-            spinner_thread.join()
-            sys.stdout.write("\r\nDone!\n")
-            sys.stdout.flush()
-
-    class validate:
-
-        @staticmethod
-        def email(*emails):
-
-            email_re = r"(?:[a-z0-9!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*|\"(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21\x23-\x5b\x5d-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])*\")@(?:(?:[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?|\[(?:(?:(2(5[0-5]|[0-4][0-9])|1[0-9][0-9]|[1-9]?[0-9]))\.){3}(?:(2(5[0-5]|[0-4][0-9])|1[0-9][0-9]|[1-9]?[0-9])|[a-z0-9-]*[a-z0-9]:(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21-\x5a\x53-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])+)\])"
-
-            results = []
-
-            for email in emails:
-            
-                def validate_email(email=email):
-
-                    if re.match(email_re, email):
-                        return True
-                    
-                    else:
-                        return False
-                
-                results.append(validate_email(email))
-
-            return results
-
-
-
-
-
-
-builtins.print = Pyrew().write
-
-builtins.__dict__['true'] = True
-builtins.__dict__['false'] = False
-builtins.__dict__['string'] = str
-builtins.__dict__['integer'] = int
-builtins.__dict__['boolean'] = bool
-builtins.__dict__['none'] = None
-builtins.__dict__['null'] = None
-builtins.__dict__['void'] = None
-
+import sys
+import builtins
+import importlib
+import os
+from contextlib import contextmanager
+import logging
+import asyncio
+import time
+import itertools
+import threading
+import re
+
+try:
+    import colorama
+    colorama.init()
+
+except ImportError:
+    pass
+
+class MultiException(Exception):
+    def __init__(self, exceptions):
+        self.exceptions = exceptions
+        super().__init__(f"{len(exceptions)} exceptions occurred")
+
+class Pyrew:
+    @staticmethod
+    def write(*args, end='\n'):
+
+        args_list = list(args)
+
+        for i in range(len(args_list)):
+            if args_list[i] is None:
+                args_list[i] = ''
+
+        if end is None:
+            __end__ = ''
+        else:
+            __end__ = end
+        
+        output = ''.join(str(arg) for arg in args_list)
+        sys.stdout.write(f"{output}{__end__}")
+
+    class files:
+
+        class cwd:
+
+            @staticmethod
+            def append(path, content):
+                with open(os.path.join(os.getcwd(), path), 'a') as f:
+                    f.write(content)
+
+            @staticmethod
+            def read(path):
+                with open(os.path.join(os.getcwd(), path), 'r') as f:
+                    return str(f.read(f))
+                
+            @staticmethod
+            def write(path, content):
+                with open(os.path.join(os.getcwd(), path), 'w') as f:
+                    f.write(content)
+                
+        @staticmethod
+        def append(path, content):
+            with open(path, 'a') as f:
+                f.write(content)
+
+        @staticmethod
+        def read(path):
+            with open(path, 'r') as f:
+                return str(f.read(f))
+            
+        @staticmethod
+        def write(path, content):
+            with open(path, 'w') as f:
+                f.write(content)
+
+    @staticmethod
+    @contextmanager
+    def run(n):
+        for i in range(n):
+            yield i
+
+    @staticmethod
+    def throw(*exceptions):
+        if len(exceptions) == 1:
+            raise exceptions[0]
+
+        raise MultiException(exceptions)
+
+    class log:
+
+        @staticmethod
+        def warn(message):
+            logging.warning(message)
+            
+        @staticmethod
+        def error(message):
+            logging.error(message)
+
+        @staticmethod
+        def info(message):
+            logging.info(message)
+        
+        @staticmethod
+        def debug(message):
+            logging.debug(message)
+
+        @staticmethod
+        def clear():
+            os.system('cls' if os.name == 'nt' else 'clear')
+
+    @staticmethod
+    def tupmod(tup, index, val):
+        return tup[:index] + (val,) + tup[index + 1:]
+    
+    @staticmethod
+    def set_timeout(func, n=None, timeout=None):
+
+        if n is None:
+            n = 1
+
+        for i in range(n):
+
+            if timeout is None:
+                timeout = 0
+            
+            time.sleep(timeout)
+            func()
+
+    class sh:
+
+        @staticmethod
+        def run(*cmds):
+            for cmd in cmds:
+                confirm = input(f"You are about to do something potentially dangerous. Are you sure you want to run \"{cmd}\"? y/N: ")
+                if confirm.lower() in ["y", "yes"]:
+                    os.system(cmd)
+                else:
+                    print(f"Cancelled action \"{cmd}\"! Good call.")
+
+        class cwd:
+
+            @staticmethod
+            def run(*cmds):
+
+                cwd = os.getcwd()
+
+                for cmd in cmds:
+
+                    confirm = input(f"You are about to do something potentially dangerous. Are you sure you want to run \"{cmd}\"? y/N: ")
+
+                    if confirm.lower() in ["y", "yes"]:
+                        os.chdir(cwd)
+                        os.system(cmd)
+
+                    else:
+                        print(f"Cancelled action \"{cmd}\" in \"{cwd}\"! Good call.")
+
+    @staticmethod
+    def spin(func):
+        
+        spinner = itertools.cycle(
+                [
+                    f"\033[31m\u2015\033[0m",
+                    f"\033[32m/\033[0m", 
+                    f"\033[33m|\033[0m", 
+                    f"\033[34m\\\033[0m"
+                ]
+            )
+        
+        stop_spinner = threading.Event()
+
+        def animate():
+            while not stop_spinner.is_set():
+                sys.stdout.write("\rRunning... " + next(spinner))
+                sys.stdout.flush()
+                time.sleep(0.1)
+        
+        spinner_thread = threading.Thread(target=animate)
+        spinner_thread.start()
+
+        try:
+            func()
+
+        finally:
+            stop_spinner.set()
+            spinner_thread.join()
+            sys.stdout.write("\r\nDone!\n")
+            sys.stdout.flush()
+
+    class validate:
+
+        @staticmethod
+        def email(*emails):
+
+            email_re = r"(?:[a-z0-9!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*|\"(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21\x23-\x5b\x5d-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])*\")@(?:(?:[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?|\[(?:(?:(2(5[0-5]|[0-4][0-9])|1[0-9][0-9]|[1-9]?[0-9]))\.){3}(?:(2(5[0-5]|[0-4][0-9])|1[0-9][0-9]|[1-9]?[0-9])|[a-z0-9-]*[a-z0-9]:(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21-\x5a\x53-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])+)\])"
+
+            results = []
+
+            for email in emails:
+            
+                def validate_email(email=email):
+
+                    if re.match(email_re, email):
+                        return True
+                    
+                    else:
+                        return False
+                
+                results.append(validate_email(email))
+
+            return results
+
+
+
+
+
+
+builtins.print = Pyrew().write
+
+builtins.__dict__['true'] = True
+builtins.__dict__['false'] = False
+builtins.__dict__['string'] = str
+builtins.__dict__['integer'] = int
+builtins.__dict__['boolean'] = bool
+builtins.__dict__['none'] = None
+builtins.__dict__['null'] = None
+builtins.__dict__['void'] = None
+
```

