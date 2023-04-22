# Comparing `tmp/markit-gateway-1.8.4.tar.gz` & `tmp/markit-gateway-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rfmarkit-gateway/rfmarkit-gateway/dist/.tmp-jffviwt6/markit-gateway-1.8.4.tar", last modified: Sat Apr 22 01:59:03 2023, max compression
+gzip compressed data, was "/home/runner/work/rfmarkit-gateway/rfmarkit-gateway/dist/.tmp-6hi54tsy/markit-gateway-2.0.1.tar", last modified: Sat Apr 22 09:11:26 2023, max compression
```

## Comparing `markit-gateway-1.8.4.tar` & `markit-gateway-2.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:59:03.000000 markit-gateway-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-22 01:59:03.000000 markit-gateway-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:59:03.000000 markit-gateway-1.8.4/markit_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:59:03.000000 markit-gateway-1.8.4/markit_gateway/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/cmd/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/cmd/easy_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/cmd/portal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:59:03.000000 markit-gateway-1.8.4/markit_gateway/common/
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/common/IMUParser.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/common/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/common/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/common/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:59:03.000000 markit-gateway-1.8.4/markit_gateway/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/functional/align.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/functional/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/functional/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/functional/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:59:03.000000 markit-gateway-1.8.4/markit_gateway/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/scripts/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:59:03.000000 markit-gateway-1.8.4/markit_gateway/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/tasks/imu_render_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/tasks/measure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:59:03.000000 markit-gateway-1.8.4/markit_gateway/tasks/obj/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/tasks/obj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/tasks/tcp_listen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/tasks/tcp_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/markit_gateway/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:59:03.000000 markit-gateway-1.8.4/markit_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-22 01:59:02.000000 markit-gateway-1.8.4/markit_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-22 01:59:03.000000 markit-gateway-1.8.4/markit_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 01:59:02.000000 markit-gateway-1.8.4/markit_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-22 01:59:02.000000 markit-gateway-1.8.4/markit_gateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-22 01:59:02.000000 markit-gateway-1.8.4/markit_gateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 01:59:03.000000 markit-gateway-1.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:59:03.000000 markit-gateway-1.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/tests/test_fit_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/tests/test_measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-22 01:58:51.000000 markit-gateway-1.8.4/tests/test_streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/markit_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/markit_gateway/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/cmd/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/cmd/easy_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/cmd/portal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/markit_gateway/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/common/IMUParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/common/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/common/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/common/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/markit_gateway/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/functional/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/functional/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/functional/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/functional/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/markit_gateway/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/scripts/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/markit_gateway/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/tasks/imu_render_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/tasks/measure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/markit_gateway/tasks/obj/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/tasks/obj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/tasks/tcp_listen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/tasks/tcp_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/markit_gateway/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/markit_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/markit_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/markit_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/markit_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/markit_gateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/markit_gateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:11:26.000000 markit-gateway-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/tests/test_fit_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/tests/test_measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-22 09:11:12.000000 markit-gateway-2.0.1/tests/test_streamlit.py
```

### Comparing `markit-gateway-1.8.4/PKG-INFO` & `markit-gateway-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markit-gateway
-Version: 1.8.4
+Version: 2.0.1
 Summary: IMU message broker
 Author: davidliyutong
 Author-email: davidliyutong@sjtu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # MARKIT Gateway
```

### Comparing `markit-gateway-1.8.4/markit_gateway/__main__.py` & `markit-gateway-2.0.1/markit_gateway/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 import argparse
 import sys
 
 from markit_gateway.scripts import cli, configure
+from markit_gateway.cmd import portal
+from .config import BrokerConfig
 
 if __name__ == '__main__':
-    if len(sys.argv) > 1 and sys.argv[1] == 'configure':
-        parser = argparse.ArgumentParser()
-        parser.add_argument("--input", "-i", type=str, default=None, help="path to input config file")
-        parser.add_argument("--output", "-o", type=str, default="imu_config.yaml", help="path to output config file")
-        args = parser.parse_args(sys.argv[2:])
-        configure(args)
+    argv = sys.argv[1:]
+    if len(argv) > 0:
+        if sys.argv[0] == 'configure':
+            parser = argparse.ArgumentParser()
+            parser.add_argument("--input", "-i", type=str, default=None, help="path to input config file")
+            parser.add_argument("--output", "-o", type=str, default="imu_config.yaml", help="path to output config file")
+            args = parser.parse_args(sys.argv[2:])
+            configure(args)
+        elif argv[0] == 'serve':
+            parser = argparse.ArgumentParser()
+            parser.add_argument('--config', type=str, default='./imu_config.yaml', help="path to config file")
+            args = parser.parse_args(argv[1:])
+            option = BrokerConfig(args.config)
+            portal(option)
+
     else:
         parser = argparse.ArgumentParser()
         parser.add_argument('-P', action="store_true", help="portal mode")
         parser.add_argument('--easy', action="store_true", help="start easy setup")
         parser.add_argument('--config', type=str, default='./imu_config.yaml', help="path to config file")
         args = parser.parse_args()
         cli(args)
```

### Comparing `markit-gateway-1.8.4/markit_gateway/cmd/control.py` & `markit-gateway-2.0.1/markit_gateway/cmd/control.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/cmd/easy_setup.py` & `markit-gateway-2.0.1/markit_gateway/cmd/easy_setup.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/cmd/portal.py` & `markit-gateway-2.0.1/markit_gateway/cmd/portal.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/common/IMUParser.py` & `markit-gateway-2.0.1/markit_gateway/common/IMUParser.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/common/render.py` & `markit-gateway-2.0.1/markit_gateway/common/render.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/common/repo.py` & `markit-gateway-2.0.1/markit_gateway/common/repo.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/common/tcp.py` & `markit-gateway-2.0.1/markit_gateway/common/tcp.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/config.py` & `markit-gateway-2.0.1/markit_gateway/config.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/functional/align.py` & `markit-gateway-2.0.1/markit_gateway/functional/align.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/functional/convert.py` & `markit-gateway-2.0.1/markit_gateway/functional/convert.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/functional/ellipse.py` & `markit-gateway-2.0.1/markit_gateway/functional/ellipse.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/functional/vector.py` & `markit-gateway-2.0.1/markit_gateway/functional/vector.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/scripts/cli.py` & `markit-gateway-2.0.1/markit_gateway/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/scripts/configure.py` & `markit-gateway-2.0.1/markit_gateway/scripts/configure.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/tasks/imu_render_ui.py` & `markit-gateway-2.0.1/markit_gateway/tasks/imu_render_ui.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/tasks/measure.py` & `markit-gateway-2.0.1/markit_gateway/tasks/measure.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/tasks/tcp_listen.py` & `markit-gateway-2.0.1/markit_gateway/tasks/tcp_listen.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/tasks/tcp_process.py` & `markit-gateway-2.0.1/markit_gateway/tasks/tcp_process.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway/utils.py` & `markit-gateway-2.0.1/markit_gateway/utils.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/markit_gateway.egg-info/PKG-INFO` & `markit-gateway-2.0.1/markit_gateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markit-gateway
-Version: 1.8.4
+Version: 2.0.1
 Summary: IMU message broker
 Author: davidliyutong
 Author-email: davidliyutong@sjtu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # MARKIT Gateway
```

### Comparing `markit-gateway-1.8.4/markit_gateway.egg-info/SOURCES.txt` & `markit-gateway-2.0.1/markit_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/setup.py` & `markit-gateway-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 requires = open("requirements.txt", "r").readlines() if os.path.exists("requirements.txt") else open("./markit_gateway.egg-info/requires.txt", "r").readlines()
 print("#-------------------    ", str(os.listdir("./")))
 setup(
     name="markit-gateway",
-    version="1.8.4",
+    version="2.0.1",
     author="davidliyutong",
     author_email="davidliyutong@sjtu.edu.cn",
     description="IMU message broker",
     packages=[
         "markit_gateway",
         "markit_gateway.cmd",
         "markit_gateway.common",
```

### Comparing `markit-gateway-1.8.4/tests/test_measure.py` & `markit-gateway-2.0.1/tests/test_measure.py`

 * *Files identical despite different names*

### Comparing `markit-gateway-1.8.4/tests/test_streamlit.py` & `markit-gateway-2.0.1/tests/test_streamlit.py`

 * *Files identical despite different names*

