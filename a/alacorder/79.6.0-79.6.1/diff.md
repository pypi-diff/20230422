# Comparing `tmp/alacorder-79.6.0.tar.gz` & `tmp/alacorder-79.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-79.6.0.tar", max compression
+gzip compressed data, was "alacorder-79.6.1.tar", max compression
```

## Comparing `alacorder-79.6.0.tar` & `alacorder-79.6.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.6.0/LICENSE
--rw-r--r--   0        0        0     9558 2023-04-19 15:07:38.263494 alacorder-79.6.0/README.md
--rw-r--r--   0        0        0      679 2023-04-21 21:12:37.802217 alacorder-79.6.0/pyproject.toml
--rw-r--r--   0        0        0     9208 2023-04-21 18:06:44.921207 alacorder-79.6.0/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb
--rw-r--r--   0        0        0   138382 2023-04-21 18:24:49.412475 alacorder-79.6.0/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.6.0/src/alacorder/.python-version
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.6.0/src/alacorder/__init__.py
--rw-r--r--   0        0        0   139236 2023-04-21 21:10:27.490652 alacorder-79.6.0/src/alacorder/__main__.py
--rw-r--r--   0        0        0   139236 2023-04-21 21:10:17.909734 alacorder-79.6.0/src/alacorder/alac.py
--rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.6.0/src/alacorder/~$E 302 Portfolio.docx
--rw-r--r--   0        0        0    10448 1970-01-01 00:00:00.000000 alacorder-79.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.6.1/LICENSE
+-rw-r--r--   0        0        0     9558 2023-04-19 15:07:38.263494 alacorder-79.6.1/README.md
+-rw-r--r--   0        0        0      679 2023-04-21 22:16:00.901925 alacorder-79.6.1/pyproject.toml
+-rw-r--r--   0        0        0     9208 2023-04-21 18:06:44.921207 alacorder-79.6.1/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb
+-rw-r--r--   0        0        0   138382 2023-04-21 18:24:49.412475 alacorder-79.6.1/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.6.1/src/alacorder/.python-version
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.6.1/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   139277 2023-04-21 22:15:52.617131 alacorder-79.6.1/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   139277 2023-04-21 22:15:32.172949 alacorder-79.6.1/src/alacorder/alac.py
+-rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.6.1/src/alacorder/~$E 302 Portfolio.docx
+-rw-r--r--   0        0        0    10448 1970-01-01 00:00:00.000000 alacorder-79.6.1/PKG-INFO
```

### Comparing `alacorder-79.6.0/LICENSE` & `alacorder-79.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.0/README.md` & `alacorder-79.6.1/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.0/pyproject.toml` & `alacorder-79.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "79.6.0"
+version = "79.6.1"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-79.6.0/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb` & `alacorder-79.6.1/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.0/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-79.6.1/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.0/src/alacorder/__init__.py` & `alacorder-79.6.1/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.0/src/alacorder/__main__.py` & `alacorder-79.6.1/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     tqdm, 
     xlsxwriter, 
     xlsx2csv
 
 """
 
 name = "ALACORDER"
-version = "79.6.0"
+version = "79.6.1"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 if autoload_graphical_user_interface:
     import PySimpleGUI as sg
 
@@ -536,15 +536,15 @@
                         window=window,
                     )
                 except:
                     print("Check configuration and try again.")
                     window["TB"].update(disabled=False)
                     continue
                 window["TB"].update(disabled=True)
-                threading.Thread(target=init, args=(cf), daemon=True).start()
+                threading.Thread(target=init, args=[cf], daemon=True).start()
                 continue
             except:
                 print("Check configuration and try again.")
                 window["TB"].update(disabled=False)
                 continue
         elif event == "MA":
             if (
@@ -555,30 +555,30 @@
                 window["MA"].update(disabled=False)
                 continue
             try:
                 count = int(window["MA-COUNT"].get().strip())
             except:
                 count = 0
             try:
-                aa = set(
+                cf = set(
                     window["MA-INPUTPATH"].get(),
                     window["MA-OUTPUTPATH"].get(),
                     count=count,
                     archive=True,
                     overwrite=window["MA-OVERWRITE"].get(),
                     append=window["MA-APPEND"].get(),
                     no_prompt=True,
                     window=window,
                 )
             except:
                 sg.popup("Check configuration and try again.")
                 window["MA"].update(disabled=False)
                 continue
             window["MA"].update(disabled=True)
-            threading.Thread(target=archive, args=(aa), daemon=True).start()
+            threading.Thread(target=archive, args=[cf], daemon=True).start()
             continue
         elif event == "SQ":
             if (
                 window["SQ-INPUTPATH"].get() == ""
                 or window["SQ-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
@@ -1532,15 +1532,15 @@
     }
     dlog(out, cf=debug)
     if now:
         return init(out, window=window, debug=debug)
     return out
 
 
-def read(cf="", window=None):
+def read(cf=""):
     """
     Read `cf` input PDF directory or case text archive into memory.
     """
     if isinstance(cf, pl.dataframe.frame.DataFrame):  # df input
         df = cf
         if "AllPagesTextNoNewLine" not in df.columns and "AllPagesText" in df.columns:
             df = df.with_columns(
@@ -1551,19 +1551,19 @@
             return df
         else:
             return df
     elif isinstance(cf, list):  # [paths] input
         queue = cf
         aptxt = []
         print("Extracting text...")
-        if window:
-            window.write_event_value("PROGRESS_TOTAL", len(queue))
+        if cf['WINDOW']:
+            cf['WINDOW'].write_event_value("PROGRESS_TOTAL", len(queue))
             for i, pp in enumerate(queue):
                 aptxt += [extract_text(pp)]
-                window.write_event_value("PROGRESS", i + 1)
+                cf['WINDOW'].write_event_value("PROGRESS", i + 1)
         else:
             for pp in tqdm(queue):
                 aptxt += [extract_text(pp)]
         archive = pl.DataFrame(
             {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
         )
         archive = archive.with_columns(
@@ -1575,19 +1575,19 @@
     elif isinstance(cf, dict):  # cf input
         if cf["NEEDTEXT"] == False or "ALABAMA" in cf["QUEUE"][0]:
             return cf["QUEUE"]
         if cf["NEEDTEXT"] == True:
             queue = cf["QUEUE"]
             aptxt = []
             print("Extracting text...")
-            if window:
-                window.write_event_value("PROGRESS_TOTAL", len(queue))
+            if cf['WINDOW']:
+                cf['WINDOW'].write_event_value("PROGRESS_TOTAL", len(queue))
                 for i, pp in enumerate(queue):
                     aptxt += [extract_text(pp)]
-                    window.write_event_value("PROGRESS", i + 1)
+                    cf['WINDOW'].write_event_value("PROGRESS", i + 1)
             else:
                 for pp in tqdm(queue):
                     aptxt += [extract_text(pp)]
         archive = pl.DataFrame(
             {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
         )
         archive = archive.with_columns(
@@ -1596,19 +1596,19 @@
             .alias("AllPagesTextNoNewLine")
         )
         return archive
     elif os.path.isdir(cf):  # directory input
         queue = glob.glob(cf + "**/*.pdf", recursive=True)
         aptxt = []
         print("Extracting text...")
-        if window:
-            window.write_event_value("PROGRESS_TOTAL", len(queue))
+        if cf['WINDOW']:
+            cf['WINDOW'].write_event_value("PROGRESS_TOTAL", len(queue))
             for i, pp in enumerate(queue):
                 aptxt += [extract_text(pp)]
-                window.write_event_value("PROGRESS", i + 1)
+                cf['WINDOW'].write_event_value("PROGRESS", i + 1)
         else:
             for pp in tqdm(queue):
                 aptxt += [extract_text(pp)]
         archive = pl.DataFrame(
             {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
         )
         archive = archive.with_columns(
```

### Comparing `alacorder-79.6.0/src/alacorder/alac.py` & `alacorder-79.6.1/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     tqdm, 
     xlsxwriter, 
     xlsx2csv
 
 """
 
 name = "ALACORDER"
-version = "79.6.0"
+version = "79.6.1"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 if autoload_graphical_user_interface:
     import PySimpleGUI as sg
 
@@ -536,15 +536,15 @@
                         window=window,
                     )
                 except:
                     print("Check configuration and try again.")
                     window["TB"].update(disabled=False)
                     continue
                 window["TB"].update(disabled=True)
-                threading.Thread(target=init, args=(cf), daemon=True).start()
+                threading.Thread(target=init, args=[cf], daemon=True).start()
                 continue
             except:
                 print("Check configuration and try again.")
                 window["TB"].update(disabled=False)
                 continue
         elif event == "MA":
             if (
@@ -555,30 +555,30 @@
                 window["MA"].update(disabled=False)
                 continue
             try:
                 count = int(window["MA-COUNT"].get().strip())
             except:
                 count = 0
             try:
-                aa = set(
+                cf = set(
                     window["MA-INPUTPATH"].get(),
                     window["MA-OUTPUTPATH"].get(),
                     count=count,
                     archive=True,
                     overwrite=window["MA-OVERWRITE"].get(),
                     append=window["MA-APPEND"].get(),
                     no_prompt=True,
                     window=window,
                 )
             except:
                 sg.popup("Check configuration and try again.")
                 window["MA"].update(disabled=False)
                 continue
             window["MA"].update(disabled=True)
-            threading.Thread(target=archive, args=(aa), daemon=True).start()
+            threading.Thread(target=archive, args=[cf], daemon=True).start()
             continue
         elif event == "SQ":
             if (
                 window["SQ-INPUTPATH"].get() == ""
                 or window["SQ-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
@@ -1532,15 +1532,15 @@
     }
     dlog(out, cf=debug)
     if now:
         return init(out, window=window, debug=debug)
     return out
 
 
-def read(cf="", window=None):
+def read(cf=""):
     """
     Read `cf` input PDF directory or case text archive into memory.
     """
     if isinstance(cf, pl.dataframe.frame.DataFrame):  # df input
         df = cf
         if "AllPagesTextNoNewLine" not in df.columns and "AllPagesText" in df.columns:
             df = df.with_columns(
@@ -1551,19 +1551,19 @@
             return df
         else:
             return df
     elif isinstance(cf, list):  # [paths] input
         queue = cf
         aptxt = []
         print("Extracting text...")
-        if window:
-            window.write_event_value("PROGRESS_TOTAL", len(queue))
+        if cf['WINDOW']:
+            cf['WINDOW'].write_event_value("PROGRESS_TOTAL", len(queue))
             for i, pp in enumerate(queue):
                 aptxt += [extract_text(pp)]
-                window.write_event_value("PROGRESS", i + 1)
+                cf['WINDOW'].write_event_value("PROGRESS", i + 1)
         else:
             for pp in tqdm(queue):
                 aptxt += [extract_text(pp)]
         archive = pl.DataFrame(
             {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
         )
         archive = archive.with_columns(
@@ -1575,19 +1575,19 @@
     elif isinstance(cf, dict):  # cf input
         if cf["NEEDTEXT"] == False or "ALABAMA" in cf["QUEUE"][0]:
             return cf["QUEUE"]
         if cf["NEEDTEXT"] == True:
             queue = cf["QUEUE"]
             aptxt = []
             print("Extracting text...")
-            if window:
-                window.write_event_value("PROGRESS_TOTAL", len(queue))
+            if cf['WINDOW']:
+                cf['WINDOW'].write_event_value("PROGRESS_TOTAL", len(queue))
                 for i, pp in enumerate(queue):
                     aptxt += [extract_text(pp)]
-                    window.write_event_value("PROGRESS", i + 1)
+                    cf['WINDOW'].write_event_value("PROGRESS", i + 1)
             else:
                 for pp in tqdm(queue):
                     aptxt += [extract_text(pp)]
         archive = pl.DataFrame(
             {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
         )
         archive = archive.with_columns(
@@ -1596,19 +1596,19 @@
             .alias("AllPagesTextNoNewLine")
         )
         return archive
     elif os.path.isdir(cf):  # directory input
         queue = glob.glob(cf + "**/*.pdf", recursive=True)
         aptxt = []
         print("Extracting text...")
-        if window:
-            window.write_event_value("PROGRESS_TOTAL", len(queue))
+        if cf['WINDOW']:
+            cf['WINDOW'].write_event_value("PROGRESS_TOTAL", len(queue))
             for i, pp in enumerate(queue):
                 aptxt += [extract_text(pp)]
-                window.write_event_value("PROGRESS", i + 1)
+                cf['WINDOW'].write_event_value("PROGRESS", i + 1)
         else:
             for pp in tqdm(queue):
                 aptxt += [extract_text(pp)]
         archive = pl.DataFrame(
             {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
         )
         archive = archive.with_columns(
```

### Comparing `alacorder-79.6.0/PKG-INFO` & `alacorder-79.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 79.6.0
+Version: 79.6.1
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

