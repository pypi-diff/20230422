# Comparing `tmp/pyrew-0.8.0.tar.gz` & `tmp/pyrew-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrew-0.8.0.tar", last modified: Sat Apr 22 07:08:14 2023, max compression
+gzip compressed data, was "pyrew-0.9.0.tar", last modified: Sat Apr 22 08:26:59 2023, max compression
```

## Comparing `pyrew-0.8.0.tar` & `pyrew-0.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 07:08:14.590971 pyrew-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 07:08:14.590971 pyrew-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-22 07:08:02.000000 pyrew-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 07:08:02.000000 pyrew-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 07:08:14.590971 pyrew-0.8.0/pyrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 07:08:14.000000 pyrew-0.8.0/pyrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-22 07:08:14.000000 pyrew-0.8.0/pyrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 07:08:14.000000 pyrew-0.8.0/pyrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 07:08:14.000000 pyrew-0.8.0/pyrew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-04-22 07:08:02.000000 pyrew-0.8.0/pyrew.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 07:08:14.590971 pyrew-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-22 07:08:02.000000 pyrew-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:26:59.589461 pyrew-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 08:26:59.589461 pyrew-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-22 08:26:49.000000 pyrew-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 08:26:49.000000 pyrew-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:26:59.589461 pyrew-0.9.0/pyrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 08:26:59.000000 pyrew-0.9.0/pyrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-22 08:26:59.000000 pyrew-0.9.0/pyrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 08:26:59.000000 pyrew-0.9.0/pyrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 08:26:59.000000 pyrew-0.9.0/pyrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-04-22 08:26:49.000000 pyrew-0.9.0/pyrew.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 08:26:59.589461 pyrew-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-22 08:26:49.000000 pyrew-0.9.0/setup.py
```

### Comparing `pyrew-0.8.0/PKG-INFO` & `pyrew-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrew
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python library for writing shorter and more efficient Python code.
 Home-page: https://github.com/AquaQuokka/pyrew
 Author: AquaQuokka
 License: BSD-3-Clause
 
 =============
 Pyrew
```

### Comparing `pyrew-0.8.0/pyrew.egg-info/PKG-INFO` & `pyrew-0.9.0/pyrew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrew
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python library for writing shorter and more efficient Python code.
 Home-page: https://github.com/AquaQuokka/pyrew
 Author: AquaQuokka
 License: BSD-3-Clause
 
 =============
 Pyrew
```

### Comparing `pyrew-0.8.0/pyrew.py` & `pyrew-0.9.0/pyrew.py`

 * *Files 27% similar despite different names*

```diff
@@ -48,41 +48,69 @@
             def append(path, content):
                 with open(os.path.join(os.getcwd(), path), 'a') as f:
                     f.write(content)
 
             @staticmethod
             def read(path):
                 with open(os.path.join(os.getcwd(), path), 'r') as f:
-                    return str(f.read(f))
+                    return str(f.read())
                 
             @staticmethod
             def write(path, content):
                 with open(os.path.join(os.getcwd(), path), 'w') as f:
                     f.write(content)
+
+        class cfd:
+
+            @staticmethod
+            def append(path, content):
+                
+                cfd = os.path.dirname(os.path.abspath(__file__))
+
+                with open(os.path.join(cfd, path), 'a') as f:
+                    f.wwrite(content)
+
+            @staticmethod
+            def read(path, content):
+                
+                cfd = os.path.dirname(os.path.abspath(__file__))
+
+                with open(os.path.join(cfd, path), 'r') as f:
+                    return str(f.read())
+                
+            @staticmethod
+            def write(path, content):
+
+                cfd = os.path.dirname(os.path.abspath(__file__))
+
+                with open(os.path.join(cfd, path), 'w') as f:
+                    f.write(content)
                 
         @staticmethod
         def append(path, content):
             with open(path, 'a') as f:
                 f.write(content)
 
         @staticmethod
         def read(path):
             with open(path, 'r') as f:
-                return str(f.read(f))
+                return str(f.read())
             
         @staticmethod
         def write(path, content):
             with open(path, 'w') as f:
                 f.write(content)
 
+    """
     @staticmethod
     @contextmanager
     def run(n):
         for i in range(n):
-            yield i
+            yield
+    """
 
     @staticmethod
     def throw(*exceptions):
         if len(exceptions) == 1:
             raise exceptions[0]
 
         raise MultiException(exceptions)
@@ -127,38 +155,60 @@
             time.sleep(timeout)
             func()
 
     class sh:
 
         @staticmethod
         def run(*cmds):
+
             for cmd in cmds:
-                confirm = input(f"You are about to do something potentially dangerous. Are you sure you want to run \"{cmd}\"? y/N: ")
+
+                confirm = input(f"You are about to do something potentially dangerous. Are you sure you want to run \"{cmd}\"? (Y/n): ")
+
                 if confirm.lower() in ["y", "yes"]:
                     os.system(cmd)
+
                 else:
                     print(f"Cancelled action \"{cmd}\"! Good call.")
 
         class cwd:
 
             @staticmethod
             def run(*cmds):
 
                 cwd = os.getcwd()
 
                 for cmd in cmds:
 
-                    confirm = input(f"You are about to do something potentially dangerous. Are you sure you want to run \"{cmd}\"? y/N: ")
+                    confirm = input(f"You are about to do something potentially dangerous. Are you sure you want to run \"{cmd}\"? (Y/n): ")
 
                     if confirm.lower() in ["y", "yes"]:
                         os.chdir(cwd)
                         os.system(cmd)
 
                     else:
                         print(f"Cancelled action \"{cmd}\" in \"{cwd}\"! Good call.")
+        
+        class cfd:
+
+            @staticmethod
+            def run(*cmds):
+                
+                cfd = os.path.dirname(os.path.abspath(__file__))
+
+                for cmd in cmds:
+
+                    confirm = input(f"You are about to do something potentially dangerous. Are you sure you want to run \"{cmd}\"? (Y/n): ")
+
+                    if confirm.lower() in ['y', 'yes']:
+                        os.chdir(cfd)
+                        os.system(cmd)
+
+                    else:
+                        print(f"Cancelled action \"{cmd}\" in \"{cfd}\"! Good call.")
 
     @staticmethod
     def spin(func):
         
         spinner = itertools.cycle(
                 [
                     f"\033[31m\u2015\033[0m",
@@ -207,19 +257,14 @@
                     else:
                         return False
                 
                 results.append(validate_email(email))
 
             return results
 
-
-
-
-
-
 builtins.print = Pyrew().write
 
 builtins.__dict__['true'] = True
 builtins.__dict__['false'] = False
 builtins.__dict__['string'] = str
 builtins.__dict__['integer'] = int
 builtins.__dict__['boolean'] = bool
```

