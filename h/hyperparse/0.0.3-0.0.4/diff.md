# Comparing `tmp/hyperparse-0.0.3.tar.gz` & `tmp/hyperparse-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperparse-0.0.3.tar", last modified: Sun Apr 16 17:17:27 2023, max compression
+gzip compressed data, was "hyperparse-0.0.4.tar", last modified: Sat Apr 22 17:03:00 2023, max compression
```

## Comparing `hyperparse-0.0.3.tar` & `hyperparse-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx--S---   0 zhfu     (32413) info_fil (10015)        0 2023-04-16 17:17:27.118532 hyperparse-0.0.3/
--rw-------   0 zhfu     (32413) info_fil (10015)     2016 2023-04-16 17:17:27.116532 hyperparse-0.0.3/PKG-INFO
--rw-r--r--   0 zhfu     (32413) info_fil (10015)     1725 2023-04-14 07:04:57.000000 hyperparse-0.0.3/README.md
-drwx--S---   0 zhfu     (32413) info_fil (10015)        0 2023-04-16 17:17:27.079532 hyperparse-0.0.3/hyperparse/
--rw-r--r--   0 zhfu     (32413) info_fil (10015)       78 2023-04-13 11:22:30.000000 hyperparse-0.0.3/hyperparse/__init__.py
--rw-r--r--   0 zhfu     (32413) info_fil (10015)     2570 2023-04-15 20:09:42.000000 hyperparse-0.0.3/hyperparse/hyperparse.py
--rw-r--r--   0 zhfu     (32413) info_fil (10015)       22 2023-04-16 17:17:18.000000 hyperparse-0.0.3/hyperparse/version.py
-drwx--S---   0 zhfu     (32413) info_fil (10015)        0 2023-04-16 17:17:27.104532 hyperparse-0.0.3/hyperparse.egg-info/
--rw-------   0 zhfu     (32413) info_fil (10015)     2016 2023-04-16 17:17:26.000000 hyperparse-0.0.3/hyperparse.egg-info/PKG-INFO
--rw-------   0 zhfu     (32413) info_fil (10015)      237 2023-04-16 17:17:27.000000 hyperparse-0.0.3/hyperparse.egg-info/SOURCES.txt
--rw-------   0 zhfu     (32413) info_fil (10015)        1 2023-04-16 17:17:26.000000 hyperparse-0.0.3/hyperparse.egg-info/dependency_links.txt
--rw-------   0 zhfu     (32413) info_fil (10015)       11 2023-04-16 17:17:26.000000 hyperparse-0.0.3/hyperparse.egg-info/top_level.txt
--rw-------   0 zhfu     (32413) info_fil (10015)       38 2023-04-16 17:17:27.119532 hyperparse-0.0.3/setup.cfg
--rw-r--r--   0 zhfu     (32413) info_fil (10015)      737 2023-04-13 11:26:41.000000 hyperparse-0.0.3/setup.py
-drwx--S---   0 zhfu     (32413) info_fil (10015)        0 2023-04-16 17:17:27.110532 hyperparse-0.0.3/test/
--rw-r--r--   0 zhfu     (32413) info_fil (10015)     2111 2023-04-13 19:08:23.000000 hyperparse-0.0.3/test/test.py
+drwx--S---   0 zhfu     (32413) info_fil (10015)        0 2023-04-22 17:03:00.709991 hyperparse-0.0.4/
+-rw-------   0 zhfu     (32413) info_fil (10015)     2053 2023-04-22 17:03:00.706991 hyperparse-0.0.4/PKG-INFO
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)     1725 2023-04-14 07:04:57.000000 hyperparse-0.0.4/README.md
+drwx--S---   0 zhfu     (32413) info_fil (10015)        0 2023-04-22 17:03:00.668991 hyperparse-0.0.4/hyperparse/
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)       78 2023-04-13 11:22:30.000000 hyperparse-0.0.4/hyperparse/__init__.py
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)     3179 2023-04-21 15:44:04.000000 hyperparse-0.0.4/hyperparse/hyperparse.py
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)       22 2023-04-22 17:02:46.000000 hyperparse-0.0.4/hyperparse/version.py
+drwx--S---   0 zhfu     (32413) info_fil (10015)        0 2023-04-22 17:03:00.694991 hyperparse-0.0.4/hyperparse.egg-info/
+-rw-------   0 zhfu     (32413) info_fil (10015)     2053 2023-04-22 17:02:58.000000 hyperparse-0.0.4/hyperparse.egg-info/PKG-INFO
+-rw-------   0 zhfu     (32413) info_fil (10015)      237 2023-04-22 17:03:00.000000 hyperparse-0.0.4/hyperparse.egg-info/SOURCES.txt
+-rw-------   0 zhfu     (32413) info_fil (10015)        1 2023-04-22 17:02:58.000000 hyperparse-0.0.4/hyperparse.egg-info/dependency_links.txt
+-rw-------   0 zhfu     (32413) info_fil (10015)       11 2023-04-22 17:02:59.000000 hyperparse-0.0.4/hyperparse.egg-info/top_level.txt
+-rw-------   0 zhfu     (32413) info_fil (10015)       38 2023-04-22 17:03:00.710991 hyperparse-0.0.4/setup.cfg
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)      737 2023-04-13 11:26:41.000000 hyperparse-0.0.4/setup.py
+drwx--S---   0 zhfu     (32413) info_fil (10015)        0 2023-04-22 17:03:00.701991 hyperparse-0.0.4/test/
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)     2091 2023-04-20 14:37:08.000000 hyperparse-0.0.4/test/test.py
```

### Comparing `hyperparse-0.0.3/PKG-INFO` & `hyperparse-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: hyperparse
-Version: 0.0.3
+Version: 0.0.4
 Summary: Parse shell env variables to python dict
 Home-page: https://github.com/fuzihaofzh/hyperparse
 Author: 
 Author-email: 
+License: UNKNOWN
 Keywords: Shell env
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 
 # Hyperparse : A Simple Shell Environment Variables Parser 
 
 ## Introduction
 This script provides a way to parse environment variables and use them as hyperparameters in Python scripts.
@@ -56,7 +58,9 @@
 usermode = get_hyper("usermode")
 a = 5
 f = "stk"
 set_hyper(usermode)
 print(a) # 1
 print(f) # itud
 ```# hyperparse
+
+
```

### Comparing `hyperparse-0.0.3/README.md` & `hyperparse-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hyperparse-0.0.3/hyperparse/hyperparse.py` & `hyperparse-0.0.4/hyperparse/hyperparse.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,18 +5,24 @@
 import ctypes
 import sys
 
 global var_list, str_list
 var_list = {}
 str_list = {}
 
+def convert_float(s):
+    try:
+        return float(s)
+    except:
+        return None
+
 def parse_value(value):
     if value.isdigit():
         return int(value)
-    elif "." in value and value.replace(".", "", 1).isdigit():
+    elif convert_float(value) is not None:#"." in value and value.replace(".", "", 1).isdigit():
         return float(value)
     elif value.lower() == "none":
         return None
     elif value.lower() == "true":
         return True
     elif value.lower() == "false":
         return False
@@ -49,45 +55,64 @@
 """for key, value in env_vars.items():
     result = parse_string(value)
     if key not in globals():
         globals()[key] = result
         globals()[key + "_str"] = value"""
 
 
-def get_hyper(name):
+def parse(name = ""):
+    mode = {}
     if name not in var_list:
-        if name in os.environ:
+        if type(name) is str and name in os.environ:
             parse_env(name)
         elif f"--{name}" in sys.argv:
             parse_arg(name)
+        elif len(sys.argv) > 1:
+            parse_arg(name)
         else:
-            return {}
-    return var_list[name]
+            var_list[name] = {}
+    mode = var_list[name]
+
+    if name not in str_list:
+        mode_str = ""
+    else:
+        mode_str = str_list[name]
+    return mode, mode_str
 
 def get_hyper_str(name):
     if name not in str_list:
-        get_hyper(name)
+        parse(name)
     if name not in str_list:
         return None
     else:
         return str_list[name]
 
 def parse_arg(name):
-    parser = argparse.ArgumentParser()
-    parser.add_argument(f"--{name}", type=str, default="")
-    args, unknown_args = parser.parse_known_args()
-    value = getattr(args, name)
+    if type(name) is int:
+        try:
+            value = sys.argv[name]
+        except IndexError:
+            print(f"You do not have {name} arguments")
+            value = ""
+    elif name != "":
+        parser = argparse.ArgumentParser()
+        parser.add_argument(f"--{name}", type=str, default="")
+        args, unknown_args = parser.parse_known_args()
+        value = getattr(args, name)
+        sys.argv = [sys.argv[0]] + unknown_args
+    else:
+        value = sys.argv[1]
     result = parse_string(value)
     var_list[name] = result
     str_list[name] = value
-    sys.argv = [sys.argv[0]] + unknown_args
+    
 
 def reset_hyper(hyper, pargs=None):
     if type(hyper) is str:
-        hyper = get_hyper(hyper)
+        hyper = parse(hyper)[0]
     if pargs is None:
         frame = inspect.currentframe().f_back
         pargs = frame.f_locals
     for k in hyper:
         v = hyper[k]
         if isinstance(pargs, argparse.Namespace) and hasattr(pargs, k):
             setattr(pargs, k, v)
```

### Comparing `hyperparse-0.0.3/hyperparse.egg-info/PKG-INFO` & `hyperparse-0.0.4/hyperparse.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: hyperparse
-Version: 0.0.3
+Version: 0.0.4
 Summary: Parse shell env variables to python dict
 Home-page: https://github.com/fuzihaofzh/hyperparse
 Author: 
 Author-email: 
+License: UNKNOWN
 Keywords: Shell env
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 
 # Hyperparse : A Simple Shell Environment Variables Parser 
 
 ## Introduction
 This script provides a way to parse environment variables and use them as hyperparameters in Python scripts.
@@ -56,7 +58,9 @@
 usermode = get_hyper("usermode")
 a = 5
 f = "stk"
 set_hyper(usermode)
 print(a) # 1
 print(f) # itud
 ```# hyperparse
+
+
```

### Comparing `hyperparse-0.0.3/setup.py` & `hyperparse-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `hyperparse-0.0.3/test/test.py` & `hyperparse-0.0.4/test/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 import argparse
 sys.path.append(".")
 
 class TestHyperParse(unittest.TestCase):
 
     def test_basic(self):
         os.environ["usermode"] = "a=1,b,c=[1,2,3],d=4,e=3.2,f=itud,g=False"
-        from hyperparse import get_hyper
-        self.assertDictEqual(get_hyper("usermode"), {'a': 1, 'b': None, 'c': [1, 2, 3], 'd': 4, 'e': 3.2, 'f': 'itud', 'g': False})
+        from hyperparse import parse
+        self.assertDictEqual(parse("usermode")[0], {'a': 1, 'b': None, 'c': [1, 2, 3], 'd': 4, 'e': 3.2, 'f': 'itud', 'g': False})
 
     def test_argparse(self):
         os.environ["usermode"] = "a=1,b,c=[1,2,3],d=4,e=3.2,f=itud,g=False"
-        from hyperparse import get_hyper, reset_hyper
-        get_hyper("usermode")
+        from hyperparse import parse, reset_hyper
+        parse("usermode")
         parser = argparse.ArgumentParser()
         parser.add_argument('--a', type=int, default=5)
         parser.add_argument('--f', type=str, default="hello")
         args = parser.parse_args()
-        reset_hyper(get_hyper("usermode"), args)
+        reset_hyper(parse("usermode")[0], args)
         self.assertEqual(args.a, 1)
         self.assertEqual(args.f, "itud")
 
     def test_func(self):
         os.environ["usermode"] = "a=1,b,c=[1,2,3],d=4,e=3.2,f=itud,g=False"
-        from hyperparse import get_hyper, reset_hyper
-        usermode = get_hyper("usermode")
+        from hyperparse import parse, reset_hyper
+        usermode = parse("usermode")[0]
         a = 5
         f = "stk"
         reset_hyper(usermode)
         self.assertEqual(a, 1)
         self.assertEqual(f, "itud")
 
     def test_func_strname(self):
@@ -46,14 +46,14 @@
         sys.argv += ["--usermode", "a=1,b,c=[1,2,3],d=4,e=3.2,f=itud,g=False"]
         import hyperparse 
         hyperparse.parse_arg("usermode")
         parser = argparse.ArgumentParser()
         parser.add_argument('--a', type=int, default=5)
         parser.add_argument('--f', type=str, default="hello")
         args = parser.parse_args()
-        usermode = hyperparse.get_hyper("usermode")
+        usermode = hyperparse.parse("usermode")[0]
         hyperparse.reset_hyper(usermode, args)
         self.assertEqual(args.a, 1)
         self.assertEqual(args.f, "itud")
 
 if __name__ == '__main__':
     unittest.main()
```

