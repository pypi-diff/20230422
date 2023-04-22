# Comparing `tmp/placeholders-1.1.tar.gz` & `tmp/placeholders-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/placeholders-1.1.tar", last modified: Fri Aug 26 19:41:00 2016, max compression
+gzip compressed data, was "placeholders-2.0.tar", last modified: Sat Apr 22 13:00:28 2023, max compression
```

## Comparing `placeholders-1.1.tar` & `placeholders-2.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2016-08-26 19:41:00.000000 placeholders-1.1/
--rw-r--r--   0 austinbrown   (501) staff       (20)    15453 2016-08-25 01:44:51.000000 placeholders-1.1/PDFTools.py
--rw-r--r--   0 austinbrown   (501) staff       (20)      405 2016-08-26 19:41:00.000000 placeholders-1.1/PKG-INFO
--rw-r--r--   0 austinbrown   (501) staff       (20)      675 2016-08-26 19:40:06.000000 placeholders-1.1/placeholder_tools.py
-drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2016-08-26 19:41:00.000000 placeholders-1.1/placeholders.egg-info/
--rw-r--r--   0 austinbrown   (501) staff       (20)        1 2016-08-26 19:41:00.000000 placeholders-1.1/placeholders.egg-info/dependency_links.txt
--rw-r--r--   0 austinbrown   (501) staff       (20)       69 2016-08-26 19:41:00.000000 placeholders-1.1/placeholders.egg-info/entry_points.txt
--rw-r--r--   0 austinbrown   (501) staff       (20)      405 2016-08-26 19:41:00.000000 placeholders-1.1/placeholders.egg-info/PKG-INFO
--rw-r--r--   0 austinbrown   (501) staff       (20)       27 2016-08-26 19:41:00.000000 placeholders-1.1/placeholders.egg-info/requires.txt
--rw-r--r--   0 austinbrown   (501) staff       (20)      285 2016-08-26 19:41:00.000000 placeholders-1.1/placeholders.egg-info/SOURCES.txt
--rw-r--r--   0 austinbrown   (501) staff       (20)       31 2016-08-26 19:41:00.000000 placeholders-1.1/placeholders.egg-info/top_level.txt
--rw-r--r--   0 austinbrown   (501) staff       (20)     1110 2016-08-26 19:00:16.000000 placeholders-1.1/placeholders.py
--rw-r--r--   0 austinbrown   (501) staff       (20)      100 2016-08-26 19:41:00.000000 placeholders-1.1/setup.cfg
--rw-r--r--   0 austinbrown   (501) staff       (20)      734 2016-08-26 19:40:20.000000 placeholders-1.1/setup.py
+drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:00:28.240896 placeholders-2.0/
+-rw-r--r--   0 austinbrown   (501) staff       (20)     1074 2023-04-22 12:00:08.000000 placeholders-2.0/LICENSE
+-rw-r--r--   0 austinbrown   (501) staff       (20)        0 2023-04-22 12:00:25.000000 placeholders-2.0/MANIFEST.in
+-rw-r--r--   0 austinbrown   (501) staff       (20)     1356 2023-04-22 13:00:28.240748 placeholders-2.0/PKG-INFO
+-rw-r--r--   0 austinbrown   (501) staff       (20)     1016 2023-04-22 12:59:04.000000 placeholders-2.0/README.md
+drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:00:28.239392 placeholders-2.0/placeholders/
+-rw-r--r--   0 austinbrown   (501) staff       (20)        0 2023-04-22 11:33:55.000000 placeholders-2.0/placeholders/__init__.py
+-rw-r--r--   0 austinbrown   (501) staff       (20)      833 2023-04-22 12:34:40.000000 placeholders-2.0/placeholders/controls.py
+-rw-r--r--   0 austinbrown   (501) staff       (20)     2118 2023-04-22 11:45:07.000000 placeholders-2.0/placeholders/tools.py
+drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:00:28.240320 placeholders-2.0/placeholders.egg-info/
+-rw-r--r--   0 austinbrown   (501) staff       (20)     1356 2023-04-22 13:00:28.000000 placeholders-2.0/placeholders.egg-info/PKG-INFO
+-rw-r--r--   0 austinbrown   (501) staff       (20)      310 2023-04-22 13:00:28.000000 placeholders-2.0/placeholders.egg-info/SOURCES.txt
+-rw-r--r--   0 austinbrown   (501) staff       (20)        1 2023-04-22 13:00:28.000000 placeholders-2.0/placeholders.egg-info/dependency_links.txt
+-rw-r--r--   0 austinbrown   (501) staff       (20)       14 2023-04-22 13:00:28.000000 placeholders-2.0/placeholders.egg-info/requires.txt
+-rw-r--r--   0 austinbrown   (501) staff       (20)       13 2023-04-22 13:00:28.000000 placeholders-2.0/placeholders.egg-info/top_level.txt
+drwxr-xr-x   0 austinbrown   (501) staff       (20)        0 2023-04-22 13:00:28.240532 placeholders-2.0/scripts/
+-rwxr-xr-x   0 austinbrown   (501) staff       (20)     1101 2023-04-22 13:00:19.000000 placeholders-2.0/scripts/placeholders
+-rw-r--r--   0 austinbrown   (501) staff       (20)       38 2023-04-22 13:00:28.240949 placeholders-2.0/setup.cfg
+-rw-r--r--   0 austinbrown   (501) staff       (20)      681 2023-04-22 12:20:02.000000 placeholders-2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `placeholders-1.1/placeholders.py` & `placeholders-2.0/placeholders/controls.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,47 @@
 import os
-import sys
-import click
-import placeholder_tools as pt
+import placeholders.tools as pt
 import yaml
 import warnings
+
+
 warnings.filterwarnings("ignore")
 
-@click.group()
-def ts():
-    password
-@ts.command()
-@click.argument('d')
-@click.argument('f')
-def tags(d, f):
-    def_file = open(os.path.join(d, f))
+def set_tags(f):
+    def_file = open(f)
     definitions = yaml.safe_load(def_file)
     def_file.close()
-    files = os.listdir(d)
-    for file in files:
-        if file != f:
-            pt.set_image_tag(
-                os.path.join(
-                    d, file
-                ),
-                definitions[file]
-            )
-    print "Complete!"
+    for file, tag in definitions.items():
+        pt.set_image_tag(
+            file,
+            tag
+        )    
+            
+    print("Complete!")
     return
 
-@click.group()
-def tg():
-    pass
-@tg.command()
-@click.argument('f')
-@click.argument('t')
-def tag(f, t):
+def set_tag(f, t):
     pt.set_image_tag(
         f,
         t
         )
-    print "Complete!"
+    print("Complete!")
     return
 
-@click.group()
-def gt():
-    pass
-@gt.command()
-@click.argument('f')
 def get_tag(f):
     message = pt.get_image_tag(
         f
         )
-    print message
+    print(message)
     return message
-cli = click.CommandCollection(sources=[tg, ts, gt])
-#
 
-if __name__ == "__main__":
-    cli()
-#     make_placeholders(sys.argv[1], sys.argv[2])
+def get_tags(d):
+    files = os.listdir(d)
+    for file in files:
+        full_path = os.path.join(d, file)
+        message = pt.get_image_tag(
+            full_path
+            )
+        print(file, message)
+
+    print("Complete!")
+    return
```

