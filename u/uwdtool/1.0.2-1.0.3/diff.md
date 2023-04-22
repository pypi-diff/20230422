# Comparing `tmp/uwdtool-1.0.2.tar.gz` & `tmp/uwdtool-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwdtool-1.0.2.tar", max compression
+gzip compressed data, was "uwdtool-1.0.3.tar", max compression
```

## Comparing `uwdtool-1.0.2.tar` & `uwdtool-1.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2344 2023-04-22 03:58:10.208688 uwdtool-1.0.2/README.md
--rw-r--r--   0        0        0      342 2023-04-22 03:47:15.348573 uwdtool-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     7459 2023-04-22 03:47:24.772598 uwdtool-1.0.2/uwdtool/UWDTool.py
--rw-r--r--   0        0        0        0 2023-04-22 03:25:18.701618 uwdtool-1.0.2/uwdtool/__init__.py
--rw-r--r--   0        0        0     2839 1970-01-01 00:00:00.000000 uwdtool-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2678 2023-04-22 04:09:15.499847 uwdtool-1.0.3/README.md
+-rw-r--r--   0        0        0      342 2023-04-22 04:08:23.555632 uwdtool-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7459 2023-04-22 04:08:30.747662 uwdtool-1.0.3/uwdtool/UWDTool.py
+-rw-r--r--   0        0        0        0 2023-04-22 03:25:18.701618 uwdtool-1.0.3/uwdtool/__init__.py
+-rw-r--r--   0        0        0     3173 1970-01-01 00:00:00.000000 uwdtool-1.0.3/PKG-INFO
```

### Comparing `uwdtool-1.0.2/uwdtool/UWDTool.py` & `uwdtool-1.0.3/uwdtool/UWDTool.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import struct
 import os
 import hashlib
 from glob import glob
 from pathlib import Path
 
 
-UWDT_VERSION = "1.0.2"
+UWDT_VERSION = "1.0.3"
 HELP_STR = f"""UWDTool v{UWDT_VERSION}"""
 
 
 class UWDTException(Exception):
     def __init__(self, msg):
         self.msg = msg
 
@@ -210,15 +210,15 @@
             print("")
 
         data.close()
 
 
 def main():
     parser = argparse.ArgumentParser(
-                    prog="UWDTool",
+                    prog="uwdtool",
                     description=HELP_STR,
                     formatter_class=argparse.RawTextHelpFormatter)
     g = parser.add_mutually_exclusive_group()
 
     g.add_argument("-p", "--pack", action="store_true", help="packing files in input-path directory")
     g.add_argument("-u", "--unpack", action="store_true", help="unpacking input-path file to output-path directory")
     g.add_argument("-isp", "--inspect", action="store_true", help="show file information list of input-path file")
```

### Comparing `uwdtool-1.0.2/PKG-INFO` & `uwdtool-1.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: uwdtool
-Version: 1.0.2
+Version: 1.0.3
 Summary: The tool to pack and unpack UnityWebData files
 Author: yuria0309
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
-* [한국어](README-kr.md)
+* [한국어](https://github.com/yuria0309/uwdtool/blob/master/README-kr.md)
 * English
 
 The tool for packing or unpacking UnityWebData files.
 You can also simply check the file information that it contains.
 
 ## What Is UnityWebData
 A UnityWebData file is a file that is loaded and used in conjunction with a WebAssembly file in a WebGL game, primarily a file that combines all of the asset, resource, and metadata files.
@@ -46,18 +46,35 @@
 If you want to read a file, you can take its offset in the header and read it from that location to the size of the file in the header.
 
 ## File Struct Image
 ![img_format](https://raw.githubusercontent.com/yuria0309/uwdtool/master/img/unitywebdata_format.png)
 
 ## Usage
 ```
+pip install uwdtool
+```
+
+### CLI
+```
 python UWDTool.py <Control Option> [-i input_path] [-o output_path]
 ```
 
-### Control Option
+#### Control Option
 * -p --pack: Make the files in the input path into a UnityWebData file and save them to the output path.
 The input path is the path of the folder containing the files to be packed.
 * -u --unpack: Unpack the UnityWebData file in the input path and save it to the output path.
 The input path is the path of the file to be unpacked, and the output path is the path of the folder where the files will be stored.
 * -isp --inspect: Print information about the files that the UnityWebData file in the input path contains.
 It shows the name and size of the file. No output path is required in this case.
 * -h --help: Print help message and information from the program.
+
+### Python
+```
+from uwdtool import UWDTool
+
+
+UWDTool.Packer().pack(args.ARG_INPUT, args.ARG_OUTPUT)  # packing
+
+UWDTool.UnPacker().unpack(args.ARG_INPUT, args.ARG_OUTPUT)  # unpacking
+
+UWDTool.Inspector().inspect(args.ARG_INPUT)  # inspector
+```
```

