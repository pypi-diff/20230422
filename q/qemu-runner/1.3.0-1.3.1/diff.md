# Comparing `tmp/qemu-runner-1.3.0.tar.gz` & `tmp/qemu-runner-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qemu-runner-1.3.0.tar", last modified: Sat Apr 15 08:40:20 2023, max compression
+gzip compressed data, was "qemu-runner-1.3.1.tar", last modified: Sat Apr 22 14:51:54 2023, max compression
```

## Comparing `qemu-runner-1.3.0.tar` & `qemu-runner-1.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:20.840066 qemu-runner-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-15 08:40:20.840066 qemu-runner-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 08:40:20.840066 qemu-runner-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:20.828066 qemu-runner-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:20.832066 qemu-runner-1.3.0/src/qemu_runner/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/find_qemu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/layer_locator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:20.836066 qemu-runner-1.3.0/src/qemu_runner/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/layers/virt-cortex-m.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:20.836066 qemu-runner-1.3.0/src/qemu_runner/make_runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/make_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/make_runner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/make_runner/main.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/make_runner/make.py
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/make_runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/variable_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:20.836066 qemu-runner-1.3.0/src/qemu_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-15 08:40:20.000000 qemu-runner-1.3.0/src/qemu_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-15 08:40:20.000000 qemu-runner-1.3.0/src/qemu_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:40:20.000000 qemu-runner-1.3.0/src/qemu_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-15 08:40:20.000000 qemu-runner-1.3.0/src/qemu_runner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-15 08:40:20.000000 qemu-runner-1.3.0/src/qemu_runner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:20.840066 qemu-runner-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_find_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_find_qemu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_layer_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_layer_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_layer_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_qemu_argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_qemu_argument_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_runner_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_utllities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:54.960073 qemu-runner-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-22 14:51:54.960073 qemu-runner-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 14:51:54.960073 qemu-runner-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:54.940073 qemu-runner-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:54.948073 qemu-runner-1.3.1/src/qemu_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/find_qemu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/layer_locator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:54.952073 qemu-runner-1.3.1/src/qemu_runner/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/layers/virt-cortex-m.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:54.952073 qemu-runner-1.3.1/src/qemu_runner/make_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/make_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/make_runner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/make_runner/main.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/make_runner/make.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/make_runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/src/qemu_runner/variable_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:54.952073 qemu-runner-1.3.1/src/qemu_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-22 14:51:54.000000 qemu-runner-1.3.1/src/qemu_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-22 14:51:54.000000 qemu-runner-1.3.1/src/qemu_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 14:51:54.000000 qemu-runner-1.3.1/src/qemu_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-22 14:51:54.000000 qemu-runner-1.3.1/src/qemu_runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-22 14:51:54.000000 qemu-runner-1.3.1/src/qemu_runner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:51:54.956073 qemu-runner-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_find_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_find_qemu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_layer_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_layer_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_layer_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_qemu_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_qemu_argument_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_runner_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_utllities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-22 14:51:43.000000 qemu-runner-1.3.1/tests/test_venv.py
```

### Comparing `qemu-runner-1.3.0/LICENSE.txt` & `qemu-runner-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/PKG-INFO` & `qemu-runner-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qemu-runner
-Version: 1.3.0
+Version: 1.3.1
 Summary: Create self-contained wrappers around QEMU to hide & share long command-line invocations
 Home-page: https://github.com/Novakov/qemu-runner
 Author: Maciej Nowak
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qemu-runner-1.3.0/README.md` & `qemu-runner-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/setup.py` & `qemu-runner-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open(os.path.dirname(os.path.abspath(__file__)) + '/README.md', 'r') as f:
     description = f.read()
 
 setup(
     name='qemu-runner',
-    version='1.3.0',
+    version='1.3.1',
     description='Create self-contained wrappers around QEMU to hide & share long command-line invocations',
     url='https://github.com/Novakov/qemu-runner',
     long_description=description,
     long_description_content_type='text/markdown',
     author='Maciej Nowak',
     classifiers=[
         'Development Status :: 4 - Beta',
```

### Comparing `qemu-runner-1.3.0/src/qemu_runner/argument.py` & `qemu-runner-1.3.1/src/qemu_runner/argument.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/src/qemu_runner/find_qemu.py` & `qemu-runner-1.3.1/src/qemu_runner/find_qemu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import sys
 from os.path import dirname
 from pathlib import Path
 from typing import Optional, List
 
 
 def find_qemu(
         engine: str,
```

### Comparing `qemu-runner-1.3.0/src/qemu_runner/layer.py` & `qemu-runner-1.3.1/src/qemu_runner/layer.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/src/qemu_runner/layer_locator.py` & `qemu-runner-1.3.1/src/qemu_runner/layer_locator.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/src/qemu_runner/make_runner/__main__.py` & `qemu-runner-1.3.1/src/qemu_runner/make_runner/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 def main(argv: List[str]):
     args = parse_args(argv)
     layer_contents = load_layers_from_all_search_paths(args.layers)
     make_runner(
         args.output,
         layer_contents=layer_contents,
-        additional_script_bases=[]
+        additional_script_bases=[],
+        additional_search_paths=[]
     )
 
 
 def run():
     main(sys.argv[1:])
```

### Comparing `qemu-runner-1.3.0/src/qemu_runner/make_runner/make.py` & `qemu-runner-1.3.1/src/qemu_runner/make_runner/make.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,15 +92,16 @@
         with importlib.resources.path(qemu_runner, '') as p:
             copy_directory_path(p, archive, package.__name__)
 
 
 def make_runner(output: IO[bytes],
                 *,
                 layer_contents: List[str],
-                additional_script_bases: List[str]
+                additional_script_bases: List[str],
+                additional_search_paths: List[str]
                 ) -> None:
     with zipfile.ZipFile(output, mode='w', compression=zipfile.ZIP_STORED) as archive:
         copy_package(qemu_runner, archive)
 
         with archive.open('embedded_layers/__init__.py', 'w'):
             pass
 
@@ -108,9 +109,10 @@
             with archive.open(f'embedded_layers/layers/{i}.ini', 'w') as f1:
                 f1.write(layer_content.encode('utf-8'))
 
         with archive.open('__main__.py', 'w') as f:
             main_template = pkgutil.get_data('qemu_runner.make_runner', 'main.py.in').decode('utf-8')
             f.write(main_template.format(
                 embedded_layers=[f'{i}.ini' for i in range(0, len(layer_contents))],
-                additional_script_bases=additional_script_bases
+                additional_script_bases=additional_script_bases,
+                additional_search_paths=additional_search_paths
             ).encode('utf-8'))
```

### Comparing `qemu-runner-1.3.0/src/qemu_runner/make_runner/runner.py` & `qemu-runner-1.3.1/src/qemu_runner/make_runner/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     return Layer(general=general)
 
 
 def build_qemu_command_line(
         *,
         embedded_layers: List[str],
         additional_script_bases: List[str],
+        additional_search_paths: List[str],
         args: argparse.Namespace,
         additional_qemu_args: str) -> List[str]:
     from qemu_runner.layer_locator import load_layer
     layer_contents = [load_layer(
         layer,
         packages=['embedded_layers']
     ) for layer in embedded_layers]
@@ -109,15 +110,15 @@
         if args.qemu:
             return Path(args.qemu)
 
         from qemu_runner import find_qemu
         return find_qemu(
             engine=engine,
             script_paths=[__file__] + additional_script_bases,
-            search_paths=[args.qemu_dir] if args.qemu_dir else []
+            search_paths=additional_search_paths + ([args.qemu_dir] if args.qemu_dir else [])
         )
 
     from qemu_runner.layer import build_command_line
     full_cmdline = build_command_line(combined_layer, find_qemu_func=do_find_qemu)
 
     result = list(full_cmdline)
 
@@ -132,15 +133,15 @@
     try:
         cp = subprocess.run(command_line)
         sys.exit(cp.returncode)
     except FileNotFoundError:
         raise
 
 
-def make_derived_runner(embedded_layers: List[str], args: argparse.Namespace) -> None:
+def make_derived_runner(embedded_layers: List[str], additional_search_paths: List[str], args: argparse.Namespace) -> None:
     from qemu_runner.make_runner.make import make_runner, load_layers_from_all_search_paths
     from qemu_runner.layer_locator import load_layer
     base_layers = [load_layer(
         layer,
         packages=['embedded_layers']
     ) for layer in embedded_layers]
 
@@ -148,20 +149,21 @@
 
     if args.track_qemu:
         base_script_paths: List[str] = [__file__]
     else:
         base_script_paths = []
 
     if args.qemu_dir:
-        base_script_paths.append(args.qemu_dir)
+        additional_search_paths.append(args.qemu_dir)
 
     make_runner(
         args.derive,
         layer_contents=base_layers + additional_layers,
-        additional_script_bases=base_script_paths
+        additional_script_bases=base_script_paths,
+        additional_search_paths=additional_search_paths
     )
 
 
 def make_layer_printer():
     try:
         from pygments import highlight
         from pygments.lexers.configs import IniLexer
@@ -184,15 +186,15 @@
 
     for layer_name, layer in layers:
         print(f'# Layer embedded_layers/{layer_name}:')
         print_ini(layer.strip())
         print()
 
 
-def execute_runner(embedded_layers: List[str], additional_script_bases: List[str], args: List[str]) -> None:
+def execute_runner(embedded_layers: List[str], additional_script_bases: List[str], additional_search_paths: List[str], args: List[str]) -> None:
     arg_parser = make_arg_parser()
 
     env_runner_args = os.environ.get('QEMU_RUNNER_FLAGS', '')
     if env_runner_args != '':
         splitted_args = shlex.split(env_runner_args, posix=sys.platform != 'win32')
         args = [*splitted_args, *args]
 
@@ -213,21 +215,22 @@
     if parsed_args.inspect and parsed_args.dry_run:
         arg_parser.error('--derive and --dry-run cannot be used together')
 
     if not parsed_args.inspect and not parsed_args.derive and (not parsed_args.kernel and not parsed_args.dry_run):
         arg_parser.error('Specify action to perform: kernel, --derive or --inspect')
 
     if parsed_args.derive:
-        make_derived_runner(embedded_layers, parsed_args)
+        make_derived_runner(embedded_layers, additional_search_paths, parsed_args)
     elif parsed_args.inspect:
         inspect_runner(embedded_layers)
     else:
         cmdline = build_qemu_command_line(
             embedded_layers=embedded_layers,
             additional_script_bases=additional_script_bases,
+            additional_search_paths=additional_search_paths,
             args=parsed_args,
             additional_qemu_args=os.environ.get('QEMU_FLAGS', '')
         )
 
         if parsed_args.dry_run:
             print(shlex.join(cmdline))
             sys.exit(0)
```

### Comparing `qemu-runner-1.3.0/src/qemu_runner/variable_resolution.py` & `qemu-runner-1.3.1/src/qemu_runner/variable_resolution.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/src/qemu_runner.egg-info/PKG-INFO` & `qemu-runner-1.3.1/src/qemu_runner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qemu-runner
-Version: 1.3.0
+Version: 1.3.1
 Summary: Create self-contained wrappers around QEMU to hide & share long command-line invocations
 Home-page: https://github.com/Novakov/qemu-runner
 Author: Maciej Nowak
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qemu-runner-1.3.0/src/qemu_runner.egg-info/SOURCES.txt` & `qemu-runner-1.3.1/src/qemu_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/tests/test_find_layer.py` & `qemu-runner-1.3.1/tests/test_find_layer.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/tests/test_find_qemu.py` & `qemu-runner-1.3.1/tests/test_find_qemu.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/tests/test_layer.py` & `qemu-runner-1.3.1/tests/test_layer.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/tests/test_layer_cmdline.py` & `qemu-runner-1.3.1/tests/test_layer_cmdline.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/tests/test_layer_equality.py` & `qemu-runner-1.3.1/tests/test_layer_equality.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/tests/test_layer_parsing.py` & `qemu-runner-1.3.1/tests/test_layer_parsing.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/tests/test_qemu_argument.py` & `qemu-runner-1.3.1/tests/test_qemu_argument.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/tests/test_qemu_argument_equality.py` & `qemu-runner-1.3.1/tests/test_qemu_argument_equality.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/tests/test_runner_flow.py` & `qemu-runner-1.3.1/tests/test_runner_flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -217,15 +217,15 @@
 
     cmdline = capture_runner_cmdline(tmp_path / 'dir2' / 'derived.pyz', 'abc.elf')
 
     assert cmdline[0] == engine
 
 
 def test_derive_add_qemu_dir(tmp_path: Path):
-    engine = place_echo_args(tmp_path / 'dir1' / 'qemu' / 'my-qemu')
+    engine = place_echo_args(tmp_path / 'dir1' / 'some-path' / 'my-qemu')
 
     with open(tmp_path / 'layer1.ini', 'w') as f:
         f.write("""
         [general]
         engine = my-qemu
 
         [device:d1]
@@ -234,23 +234,56 @@
 
     (tmp_path / 'dir2').mkdir()
 
     run_make_runner('-l', './layer1.ini', '-o', tmp_path / 'dir2' / 'base_runner.pyz', cwd=tmp_path)
 
     execute_runner(
         tmp_path / 'dir2' / 'base_runner.pyz',
-        ['--layers', './layer1.ini', '--derive', './dir2/derived.pyz', '--qemu-dir', tmp_path / 'dir1' / 'qemu'],
+        ['--layers', './layer1.ini', '--derive', './dir2/derived.pyz', '--qemu-dir', tmp_path / 'dir1' / 'some-path'],
         cwd=tmp_path
     )
 
     cmdline = capture_runner_cmdline(tmp_path / 'dir2' / 'derived.pyz', 'abc.elf')
 
     assert cmdline[0] == engine
 
 
+def test_preserve_additional_search_path_in_next_derived_runner(tmp_path: Path):
+    engine = place_echo_args(tmp_path / 'dir1' / 'some-path' / 'my-qemu')
+
+    with open(tmp_path / 'layer1.ini', 'w') as f:
+        f.write("""
+        [general]
+        engine = my-qemu
+
+        [device:d1]
+        @=test
+        """)
+
+    (tmp_path / 'dir2').mkdir()
+
+    run_make_runner('-l', './layer1.ini', '-o', tmp_path / 'dir2' / 'base_runner.pyz', cwd=tmp_path)
+
+    execute_runner(
+        tmp_path / 'dir2' / 'base_runner.pyz',
+        ['--layers', './layer1.ini', '--derive', './dir2/derived1.pyz', '--qemu-dir', tmp_path / 'dir1' / 'some-path'],
+        cwd=tmp_path
+    )
+
+    execute_runner(
+        tmp_path / 'dir2' / 'derived1.pyz',
+        ['--layers', './layer1.ini', '--derive', './dir2/derived2.pyz', '--qemu-dir', tmp_path / 'dir2' / 'some-path'],
+        cwd=tmp_path
+    )
+
+    cmdline = capture_runner_cmdline(tmp_path / 'dir2' / 'derived2.pyz', 'abc.elf')
+
+    assert cmdline[0] == engine
+
+
 def test_env_qemu_flags(tmp_path: Path):
     engine = place_echo_args(tmp_path / 'qemu' / 'my-qemu')
 
     with open(tmp_path / 'layer1.ini', 'w') as f:
         f.write("""
         [general]
         engine = my-qemu
```

### Comparing `qemu-runner-1.3.0/tests/test_utllities.py` & `qemu-runner-1.3.1/tests/test_utllities.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.0/tests/test_venv.py` & `qemu-runner-1.3.1/tests/test_venv.py`

 * *Files identical despite different names*

