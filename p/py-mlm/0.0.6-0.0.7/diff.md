# Comparing `tmp/py-mlm-0.0.6.tar.gz` & `tmp/py-mlm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-mlm-0.0.6.tar", last modified: Fri Apr 14 00:46:25 2023, max compression
+gzip compressed data, was "py-mlm-0.0.7.tar", last modified: Sat Apr 22 05:58:01 2023, max compression
```

## Comparing `py-mlm-0.0.6.tar` & `py-mlm-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:46:25.582291 py-mlm-0.0.6/
--rw-r--r--   0 anon      (1000) wheel      (998)    35049 2022-11-14 05:29:48.000000 py-mlm-0.0.6/LICENSE
--rw-r--r--   0 anon      (1000) wheel      (998)      484 2023-04-14 00:46:25.582291 py-mlm-0.0.6/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      150 2023-03-23 05:11:28.000000 py-mlm-0.0.6/README.md
--rw-r--r--   0 anon      (1000) wheel      (998)      565 2023-04-14 00:45:35.000000 py-mlm-0.0.6/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-14 00:46:25.582291 py-mlm-0.0.6/setup.cfg
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:46:25.578957 py-mlm-0.0.6/src/
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:46:25.582291 py-mlm-0.0.6/src/mlm/
--rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 py-mlm-0.0.6/src/mlm/__init__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2335 2023-04-10 21:07:50.000000 py-mlm-0.0.6/src/mlm/__main__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     5287 2023-03-26 05:31:33.000000 py-mlm-0.0.6/src/mlm/build.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2216 2023-03-23 03:17:40.000000 py-mlm-0.0.6/src/mlm/config.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     4113 2023-03-23 03:57:31.000000 py-mlm-0.0.6/src/mlm/g_dl.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 py-mlm-0.0.6/src/mlm/initial_setup.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     3526 2023-03-26 06:19:39.000000 py-mlm-0.0.6/src/mlm/media.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     6582 2023-04-10 20:40:11.000000 py-mlm-0.0.6/src/mlm/options.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1651 2023-04-14 00:27:42.000000 py-mlm-0.0.6/src/mlm/prompts.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1968 2023-03-26 06:41:39.000000 py-mlm-0.0.6/src/mlm/search.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     5963 2023-04-10 21:06:52.000000 py-mlm-0.0.6/src/mlm/system.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     4224 2023-03-26 06:30:48.000000 py-mlm-0.0.6/src/mlm/utils.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:46:25.582291 py-mlm-0.0.6/src/py_mlm.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)      484 2023-04-14 00:46:25.000000 py-mlm-0.0.6/src/py_mlm.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      462 2023-04-14 00:46:25.000000 py-mlm-0.0.6/src/py_mlm.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-14 00:46:25.000000 py-mlm-0.0.6/src/py_mlm.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       42 2023-04-14 00:46:25.000000 py-mlm-0.0.6/src/py_mlm.egg-info/entry_points.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       37 2023-04-14 00:46:25.000000 py-mlm-0.0.6/src/py_mlm.egg-info/requires.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        4 2023-04-14 00:46:25.000000 py-mlm-0.0.6/src/py_mlm.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-22 05:58:01.406968 py-mlm-0.0.7/
+-rw-r--r--   0 anon      (1000) wheel      (998)    35049 2022-11-14 05:29:48.000000 py-mlm-0.0.7/LICENSE
+-rw-r--r--   0 anon      (1000) wheel      (998)      484 2023-04-22 05:58:01.406968 py-mlm-0.0.7/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      150 2023-03-23 05:11:28.000000 py-mlm-0.0.7/README.md
+-rw-r--r--   0 anon      (1000) wheel      (998)      565 2023-04-22 05:49:39.000000 py-mlm-0.0.7/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-22 05:58:01.406968 py-mlm-0.0.7/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-22 05:58:01.406968 py-mlm-0.0.7/src/
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-22 05:58:01.406968 py-mlm-0.0.7/src/mlm/
+-rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 py-mlm-0.0.7/src/mlm/__init__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2427 2023-04-22 05:43:35.000000 py-mlm-0.0.7/src/mlm/__main__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     5287 2023-03-26 05:31:33.000000 py-mlm-0.0.7/src/mlm/build.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2299 2023-04-22 05:23:33.000000 py-mlm-0.0.7/src/mlm/config.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     4113 2023-03-23 03:57:31.000000 py-mlm-0.0.7/src/mlm/g_dl.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 py-mlm-0.0.7/src/mlm/initial_setup.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     3953 2023-04-22 05:53:04.000000 py-mlm-0.0.7/src/mlm/media.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     6582 2023-04-10 20:40:11.000000 py-mlm-0.0.7/src/mlm/options.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1705 2023-04-22 05:50:58.000000 py-mlm-0.0.7/src/mlm/prompts.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1968 2023-03-26 06:41:39.000000 py-mlm-0.0.7/src/mlm/search.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     5963 2023-04-10 21:06:52.000000 py-mlm-0.0.7/src/mlm/system.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     4708 2023-04-22 05:48:48.000000 py-mlm-0.0.7/src/mlm/utils.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-22 05:58:01.406968 py-mlm-0.0.7/src/py_mlm.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)      484 2023-04-22 05:58:01.000000 py-mlm-0.0.7/src/py_mlm.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      462 2023-04-22 05:58:01.000000 py-mlm-0.0.7/src/py_mlm.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-22 05:58:01.000000 py-mlm-0.0.7/src/py_mlm.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       42 2023-04-22 05:58:01.000000 py-mlm-0.0.7/src/py_mlm.egg-info/entry_points.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       37 2023-04-22 05:58:01.000000 py-mlm-0.0.7/src/py_mlm.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        4 2023-04-22 05:58:01.000000 py-mlm-0.0.7/src/py_mlm.egg-info/top_level.txt
```

### Comparing `py-mlm-0.0.6/LICENSE` & `py-mlm-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.6/pyproject.toml` & `py-mlm-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-mlm"
-version = "0.0.6"
+version = "0.0.7"
 description = "mlm - Manga Library Manager. Local, and simple method for reading and tracking manga."
 readme = "README.md"
 license = { text = "GNU General Public License v3 (GPLv3)" }
 keywords = [ "zathura" ]
 dependencies = [
     "python-magic",
     "loadconf",
```

### Comparing `py-mlm-0.0.6/src/mlm/__main__.py` & `py-mlm-0.0.7/src/mlm/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .build import build_main, update_library
 from .config import NoBaseDir, NoBaseDirExists, get_user_settings
 from .g_dl import bulk_new, bulk_latest
 from .media import read_manga
 from .options import get_opts
 from .search import main_search
 from .system import browse_base, open_process, re_zip
-from .utils import add_url, cprint
+from .utils import add_url, cprint, format_string
 
 
 __license__ = "GPL-v3.0"
 __program__ = "mlm"
 
 
 def process_opts(user, args):
@@ -28,15 +28,16 @@
         return browse_base(user)
     elif args.open is not None:
         cprint("green", "Opening the given file")
     elif args.search is not None:
         return main_search(user, chapter=args.search)
     elif args.track is not None:
         main_search(user, chapter=args.track, track=True)
-        cmd = shlex.split(f"znp -e 'quit' -g '{args.page}' '{args.track}'")
+        cmd = shlex.split(format_string(user.settings["track_cmd"], args))
+        # cmd = shlex.split(f"znp -e 'quit' -g '{args.page}' '{args.track}'")
         return open_process(opener=cmd)
     elif args.update:
         cprint("green", "Updating library")
         return update_library(user, args)
     elif args.read or args.latest:
         return read_manga(user, latest=args.latest, new=args.new)
     elif args.url is not None and args.dir is not None:
```

### Comparing `py-mlm-0.0.6/src/mlm/build.py` & `py-mlm-0.0.7/src/mlm/build.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.6/src/mlm/config.py` & `py-mlm-0.0.7/src/mlm/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,21 +31,23 @@
 def get_user_settings(program, args):
     # Create user object to read files and get settings
     user = Config(program=program)
     # Define some basic settings, files, etc.
     user_settings = {
         "base_dir": None,
         "debug": False,
+        "extra_conf": False,
         "file_manager": None,
+        "language": "",
         "max_history": 20,
         "not_found": False,
+        "opener": "zathura",
         "prompt_cmd": "fzf",
         "prompt_args": "",
-        "zathura_conf": False,
-        "language": "",
+        "track_cmd": "znp -e 'quit' -g {page} {track}",
         "zip_util": "tar",
     }
     config_files = {
         "conf_file": "mlm.conf",
         "log_file": "log.json",
         "filters_file": "filters.conf",
         "library_file": "library.json",
```

### Comparing `py-mlm-0.0.6/src/mlm/g_dl.py` & `py-mlm-0.0.7/src/mlm/g_dl.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.6/src/mlm/media.py` & `py-mlm-0.0.7/src/mlm/media.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,60 +3,27 @@
 import os
 import sys
 from .utils import cprint, sort_updated_dirs, key_value_list, join
 from .prompts import user_choice, InvalidCmdPrompt, InputError
 from .system import open_process
 
 
-def zathura_cmd(item, user, path=None):
+def opener_cmd(item, user, path=None):
     """
     Return a command list to feed to system.open_process
     if a path to the item is given the two will be joined
     """
 
-    z_list = ["zathura"]
-    if user.settings["zathura_conf"]:
-        z_list.extend(["-c", user.config_dir])
+    opener_list = [user.settings["opener"]]
+    if user.settings["extra_conf"]:
+        opener_list.extend(["-c", user.config_dir])
     if path is not None:
         item = os.path.join(path, item)
-    z_list.append(item)
-    return z_list
-
-
-def update_log(log_file, library_file):
-    """
-    Update user log before displaying
-    """
-
-    # Compare log file and library modification
-    # times. Only update log if library has been
-    # modified more recently than log
-    log_time = os.path.getmtime(log_file)
-    lib_time = os.path.getmtime(library_file)
-    if lib_time < log_time:
-        return None
-
-    # Open log and library and load to objects
-    with open(log_file, "r") as data:
-        log = json.load(data)
-    with open(library_file, "r") as data:
-        library = json.load(data)
-
-    # Create blank log
-    lib_keys = list(library.keys())
-    log_keys = list(log.keys())
-
-    # Loop over log file and check if show is
-    # still in library
-    for dir in log_keys:
-        if not dir in lib_keys:
-            log.pop(dir)
-
-    with open(log_file, "w+") as data:
-        json.dump(log, data, indent=4)
+    opener_list.append(item)
+    return opener_list
 
 
 def read_manga(user, latest=False, new=False):
     """
     Watch a show from the user's library
     """
 
@@ -98,23 +65,71 @@
     choice = ask_user(options=ask_dirs, user=user, prompt="Read: ")
     if not choice:
         return 1
 
     index = dirs.index(choice)
     path = join(user.settings["base_dir"], dirs[index])
 
-    # If show is does not have a recently watched episode ask user which episode
-    # to watch
+    # If manga is does not have a recently read chapter ask user which chapter
+    # to read
     if reading[index] is None:
         opts = chapters[index]
         chapter = ask_user(options=opts, user=user, prompt="Read")
         if not chapter:
             return 1
     else:
         chapter = reading[index]
 
-    # Get the mpv command and open start watching the show
-    cmd = zathura_cmd(item=chapter, path=path, user=user)
+    # Get the opener command and open manga
+    cmd = opener_cmd(item=chapter, path=path, user=user)
 
     open_process(opener=cmd)
 
     return 0
+
+
+def update_log(log_file, library_file):
+    """
+    Update user log before displaying
+    """
+
+    # Compare log file and library modification
+    # times. Only update log if library has been
+    # modified more recently than log
+    log_time = os.path.getmtime(log_file)
+    lib_time = os.path.getmtime(library_file)
+    if lib_time < log_time:
+        return None
+
+    # Open log and library and load to objects
+    with open(log_file, "r") as data:
+        log = json.load(data)
+    with open(library_file, "r") as data:
+        library = json.load(data)
+
+    # Create blank log
+    lib_keys = list(library.keys())
+    log_keys = list(log.keys())
+
+    # Loop over log file and check if show is
+    # still in library
+    for dir in log_keys:
+        if not dir in lib_keys:
+            log.pop(dir)
+
+    with open(log_file, "w+") as data:
+        json.dump(log, data, indent=4)
+
+
+# def zathura_cmd(item, user, path=None):
+#     """
+#     Return a command list to feed to system.open_process
+#     if a path to the item is given the two will be joined
+#     """
+
+#     z_list = ["zathura"]
+#     if user.settings["zathura_conf"]:
+#         z_list.extend(["-c", user.config_dir])
+#     if path is not None:
+#         item = os.path.join(path, item)
+#     z_list.append(item)
+#     return z_list
```

### Comparing `py-mlm-0.0.6/src/mlm/options.py` & `py-mlm-0.0.7/src/mlm/options.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.6/src/mlm/prompts.py` & `py-mlm-0.0.7/src/mlm/prompts.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,8 +61,11 @@
 
     choice = p.ask(
         options=options,
         prompt=prompt,
         additional_args=cmd_args,
     )
 
-    return choice[0]
+    try:
+        return choice[0]
+    except IndexError:
+        return []
```

### Comparing `py-mlm-0.0.6/src/mlm/search.py` & `py-mlm-0.0.7/src/mlm/search.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.6/src/mlm/system.py` & `py-mlm-0.0.7/src/mlm/system.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.6/src/mlm/utils.py` & `py-mlm-0.0.7/src/mlm/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,21 +68,34 @@
         format = "\033[36m"
     else:
         print(string, file=out_file)
         return
     print(format + string + end, file=out_file)
 
 
-def sort_updated_dirs(library):
-    update_dict = {}
-    for k in library.keys():
-        update_dict[library[k]["update_time"]] = k
-    update_list = list(update_dict.keys())
-    update_list.sort(reverse=True)
-    return [update_dict[i] for i in update_list]
+def format_string(
+    raw_string: str,
+    args,
+) -> str:
+    format_dict = {
+        "page": args.page,
+        "track": args.track,
+    }
+    ret_str = raw_string
+    format_keys = re.findall("{([^}]+)}", ret_str)
+    for format_key in format_keys:
+        # Check if item_key is a known key
+        if format_key in format_dict.keys():
+            replace_str = format_dict[format_key]
+            ret_str = ret_str.replace(f"{{{format_key}}}", replace_str)
+    return ret_str
+
+
+def join(a, b):
+    return os_join(a, b)
 
 
 def key_value_list(dic, search_key=None):
     """
     Take a dicionary and return two lists one for keys and one for values
     """
     # While it is easiest if dic is a true dict
@@ -109,18 +122,14 @@
         true_dic()
     else:
         psuedo_dic()
 
     return keys, values
 
 
-def join(a, b):
-    return os_join(a, b)
-
-
 def merge_libraries(old_dict, new_dict):
     """Takes two dictionaries and merges them"""
     merged_dict = {}
     pop_key = None
     for new_key, new_val in new_dict.items():
         match = False
         for old_key, old_val in old_dict.items():
@@ -151,7 +160,16 @@
     with open(lib_file, "r") as data:
         library = json.load(data)
     for k, v in library.items():
         if v["url"] is None:
             continue
         ret.append((v["url"], k, float(v["chapters"][-1].split(".")[0])))
     return ret
+
+
+def sort_updated_dirs(library):
+    update_dict = {}
+    for k in library.keys():
+        update_dict[library[k]["update_time"]] = k
+    update_list = list(update_dict.keys())
+    update_list.sort(reverse=True)
+    return [update_dict[i] for i in update_list]
```

