# Comparing `tmp/noizu_ops-0.1.0.tar.gz` & `tmp/noizu_ops-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noizu_ops-0.1.0.tar", last modified: Fri Apr 21 22:48:47 2023, max compression
+gzip compressed data, was "noizu_ops-0.1.1.tar", last modified: Fri Apr 21 23:14:58 2023, max compression
```

## Comparing `noizu_ops-0.1.0.tar` & `noizu_ops-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2023-04-21 22:48:47.793383 noizu_ops-0.1.0/
--rw-r--r--   0 keith     (1000) keith     (1000)     1070 2023-04-04 18:12:20.000000 noizu_ops-0.1.0/LICENSE
--rw-rw-r--   0 keith     (1000) keith     (1000)      480 2023-04-21 22:48:47.793383 noizu_ops-0.1.0/PKG-INFO
--rw-r--r--   0 keith     (1000) keith     (1000)      570 2023-04-21 21:55:57.000000 noizu_ops-0.1.0/README.md
-drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2023-04-21 22:48:47.793383 noizu_ops-0.1.0/noizu_ops/
--rw-r--r--   0 keith     (1000) keith     (1000)        0 2023-04-21 21:42:29.000000 noizu_ops-0.1.0/noizu_ops/__init__.py
-drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2023-04-21 22:48:47.793383 noizu_ops-0.1.0/noizu_ops/bin/
--rw-r--r--   0 keith     (1000) keith     (1000)        0 2023-04-21 21:40:51.000000 noizu_ops-0.1.0/noizu_ops/bin/__init__.py
--rwxr-xr-x   0 keith     (1000) keith     (1000)    77239 2023-04-21 21:40:51.000000 noizu_ops-0.1.0/noizu_ops/bin/noizu_ops.py
-drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2023-04-21 22:48:47.793383 noizu_ops-0.1.0/noizu_ops/config/
--rw-r--r--   0 keith     (1000) keith     (1000)      845 2023-04-21 21:40:51.000000 noizu_ops-0.1.0/noizu_ops/config/system_config.fallback.yml
-drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2023-04-21 22:48:47.793383 noizu_ops-0.1.0/noizu_ops/setup/
--rw-r--r--   0 keith     (1000) keith     (1000)        0 2023-04-21 21:40:51.000000 noizu_ops-0.1.0/noizu_ops/setup/__init__.py
--rwxr-xr-x   0 keith     (1000) keith     (1000)     8199 2023-04-21 21:40:51.000000 noizu_ops-0.1.0/noizu_ops/setup/noizu_help_init.py
-drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2023-04-21 22:48:47.793383 noizu_ops-0.1.0/noizu_ops.egg-info/
--rw-r--r--   0 keith     (1000) keith     (1000)      480 2023-04-21 22:48:47.000000 noizu_ops-0.1.0/noizu_ops.egg-info/PKG-INFO
--rw-r--r--   0 keith     (1000) keith     (1000)      408 2023-04-21 22:48:47.000000 noizu_ops-0.1.0/noizu_ops.egg-info/SOURCES.txt
--rw-r--r--   0 keith     (1000) keith     (1000)        1 2023-04-21 22:48:47.000000 noizu_ops-0.1.0/noizu_ops.egg-info/dependency_links.txt
--rw-r--r--   0 keith     (1000) keith     (1000)      126 2023-04-21 22:48:47.000000 noizu_ops-0.1.0/noizu_ops.egg-info/entry_points.txt
--rw-r--r--   0 keith     (1000) keith     (1000)       64 2023-04-21 22:48:47.000000 noizu_ops-0.1.0/noizu_ops.egg-info/requires.txt
--rw-r--r--   0 keith     (1000) keith     (1000)       10 2023-04-21 22:48:47.000000 noizu_ops-0.1.0/noizu_ops.egg-info/top_level.txt
--rw-rw-r--   0 keith     (1000) keith     (1000)       38 2023-04-21 22:48:47.793383 noizu_ops-0.1.0/setup.cfg
--rw-r--r--   0 keith     (1000) keith     (1000)     1540 2023-04-21 22:48:37.000000 noizu_ops-0.1.0/setup.py
+drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2023-04-21 23:14:58.522311 noizu_ops-0.1.1/
+-rw-r--r--   0 keith     (1000) keith     (1000)     1070 2023-04-04 18:12:20.000000 noizu_ops-0.1.1/LICENSE
+-rw-rw-r--   0 keith     (1000) keith     (1000)      538 2023-04-21 23:14:58.512311 noizu_ops-0.1.1/PKG-INFO
+-rw-r--r--   0 keith     (1000) keith     (1000)     1194 2023-04-21 23:14:18.000000 noizu_ops-0.1.1/README.md
+drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2023-04-21 23:14:58.512311 noizu_ops-0.1.1/noizu_ops/
+-rw-r--r--   0 keith     (1000) keith     (1000)        0 2023-04-21 21:42:29.000000 noizu_ops-0.1.1/noizu_ops/__init__.py
+drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2023-04-21 23:14:58.512311 noizu_ops-0.1.1/noizu_ops/bin/
+-rw-r--r--   0 keith     (1000) keith     (1000)        0 2023-04-21 21:40:51.000000 noizu_ops-0.1.1/noizu_ops/bin/__init__.py
+-rwxr-xr-x   0 keith     (1000) keith     (1000)    77239 2023-04-21 21:40:51.000000 noizu_ops-0.1.1/noizu_ops/bin/noizu_ops.py
+drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2023-04-21 23:14:58.512311 noizu_ops-0.1.1/noizu_ops/config/
+-rw-r--r--   0 keith     (1000) keith     (1000)      845 2023-04-21 21:40:51.000000 noizu_ops-0.1.1/noizu_ops/config/system_config.fallback.yml
+drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2023-04-21 23:14:58.512311 noizu_ops-0.1.1/noizu_ops/setup/
+-rw-r--r--   0 keith     (1000) keith     (1000)        0 2023-04-21 21:40:51.000000 noizu_ops-0.1.1/noizu_ops/setup/__init__.py
+-rwxr-xr-x   0 keith     (1000) keith     (1000)     8592 2023-04-21 23:08:26.000000 noizu_ops-0.1.1/noizu_ops/setup/noizu_help_init.py
+drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2023-04-21 23:14:58.512311 noizu_ops-0.1.1/noizu_ops.egg-info/
+-rw-r--r--   0 keith     (1000) keith     (1000)      538 2023-04-21 23:14:58.000000 noizu_ops-0.1.1/noizu_ops.egg-info/PKG-INFO
+-rw-r--r--   0 keith     (1000) keith     (1000)      408 2023-04-21 23:14:58.000000 noizu_ops-0.1.1/noizu_ops.egg-info/SOURCES.txt
+-rw-r--r--   0 keith     (1000) keith     (1000)        1 2023-04-21 23:14:58.000000 noizu_ops-0.1.1/noizu_ops.egg-info/dependency_links.txt
+-rw-r--r--   0 keith     (1000) keith     (1000)      126 2023-04-21 23:14:58.000000 noizu_ops-0.1.1/noizu_ops.egg-info/entry_points.txt
+-rw-r--r--   0 keith     (1000) keith     (1000)       64 2023-04-21 23:14:58.000000 noizu_ops-0.1.1/noizu_ops.egg-info/requires.txt
+-rw-r--r--   0 keith     (1000) keith     (1000)       10 2023-04-21 23:14:58.000000 noizu_ops-0.1.1/noizu_ops.egg-info/top_level.txt
+-rw-rw-r--   0 keith     (1000) keith     (1000)       38 2023-04-21 23:14:58.522311 noizu_ops-0.1.1/setup.cfg
+-rw-r--r--   0 keith     (1000) keith     (1000)     1598 2023-04-21 23:10:01.000000 noizu_ops-0.1.1/setup.py
```

### Comparing `noizu_ops-0.1.0/LICENSE` & `noizu_ops-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `noizu_ops-0.1.0/noizu_ops/bin/noizu_ops.py` & `noizu_ops-0.1.1/noizu_ops/bin/noizu_ops.py`

 * *Files identical despite different names*

### Comparing `noizu_ops-0.1.0/noizu_ops/config/system_config.fallback.yml` & `noizu_ops-0.1.1/noizu_ops/config/system_config.fallback.yml`

 * *Files identical despite different names*

### Comparing `noizu_ops-0.1.0/noizu_ops/setup/noizu_help_init.py` & `noizu_ops-0.1.1/noizu_ops/setup/noizu_help_init.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,14 +90,32 @@
             value = value.strip()
             version_dict[key] = value
         return version_dict
     except (subprocess.CalledProcessError, FileNotFoundError):
         pass
     return None
 
+def cpu_info__count():
+    try:
+        psutil.cpu_count(logical=True)
+    except:
+        None
+def cpu_info__freq():
+    try:
+        psutil.cpu_freq().current
+    except:
+        None
+
+def cpu_info__percent():
+    try:
+        psutil.cpu_percent()
+    except:
+        None
+
+
 def system_info():
     rich.print("""
     [bold yellow]:information_desk_person: Hello this is Noizu-OPs, lets setup your system.[/bold yellow]   
     ---------------------------------------------------
     In order to tailor my responses to your devops experience level and 
     operating system we will scan your system to determine your OS, ram, 
     and other basic details. 
@@ -124,34 +142,40 @@
     elif platform.system() == 'Windows':
         system_info["win_info"] = get_windows_version()
     elif platform.system() in ['FreeBSD', 'NetBSD', 'OpenBSD']:
         system_info["bsd_info"] = get_bsd_version()
 
     # Get CPU information
     cpu_info = {
-        "cpu_count": psutil.cpu_count(logical=True),
-        "cpu_freq": psutil.cpu_freq().current,
-        "cpu_percent": psutil.cpu_percent()
+        "cpu_count": cpu_info__count(),
+        "cpu_freq": cpu_info__freq(),
+        "cpu_percent": cpu_info__percent()
     }
 
     # Get RAM information
-    ram_info = {
-        "total_memory": round(psutil.virtual_memory().total / (1024.0 ** 3), 2),
-        "available_memory": round(psutil.virtual_memory().available / (1024.0 ** 3), 2),
-        "used_memory": round(psutil.virtual_memory().used / (1024.0 ** 3), 2),
-        "memory_percent": psutil.virtual_memory().percent
-    }
+    try:
+        ram_info = {
+            "total_memory": round(psutil.virtual_memory().total / (1024.0 ** 3), 2),
+            "available_memory": round(psutil.virtual_memory().available / (1024.0 ** 3), 2),
+            "used_memory": round(psutil.virtual_memory().used / (1024.0 ** 3), 2),
+            "memory_percent": psutil.virtual_memory().percent
+        }
+    except:
+        ram_info = None
 
     # Get disk information
-    disk_info = {
-        "total_disk_space": round(psutil.disk_usage('/').total / (1024.0 ** 3), 2),
-        "used_disk_space": round(psutil.disk_usage('/').used / (1024.0 ** 3), 2),
-        "free_disk_space": round(psutil.disk_usage('/').free / (1024.0 ** 3), 2),
-        "disk_percent": psutil.disk_usage('/').percent
-    }
+    try:
+        disk_info = {
+            "total_disk_space": round(psutil.disk_usage('/').total / (1024.0 ** 3), 2),
+            "used_disk_space": round(psutil.disk_usage('/').used / (1024.0 ** 3), 2),
+            "free_disk_space": round(psutil.disk_usage('/').free / (1024.0 ** 3), 2),
+            "disk_percent": psutil.disk_usage('/').percent
+        }
+    except:
+        disk_info = None
 
     # Get current user and groups
     current_user = getpass.getuser()
     name = input("Enter your name: ")
     if name == '':
         name = current_user
     email = input("Enter your email address: ")
```

### Comparing `noizu_ops-0.1.0/setup.py` & `noizu_ops-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def run(self):
         from setup import noizu_help_init
         si = noizu_help_init.system_info()
         noizu_help_init.update_config(si)
 
 setup(
     name="noizu_ops",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     package_data={
         'noizu_ops': ['config/*.yml']
     },
     cmdclass={
      'run_system_info': RunSystemInfo,
     },
@@ -42,15 +42,15 @@
         ],
         'argcomplete.completers': [
             'noizu-ops = noizu_ops.bin.noizu_ops:main'
         ]
     },
     author="Keith Brings",
     author_email="keith.brings@noizu.com",
-    description="Interactive terminal assistant, log sessions, generate todo / step instructions, apply steps , query system status for troubleshooting., etc. (wip)",
+    description="Command line LLM interface. Generate how to/answer system queries. Command passing in your system info to better target response, GPT self reflection used to improve final results. (but it's slow as heck.)",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
     ],
 )
```

