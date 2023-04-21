# Comparing `tmp/xeno-5.1.0.tar.gz` & `tmp/xeno-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeno-5.1.0.tar", last modified: Fri Apr 21 23:51:39 2023, max compression
+gzip compressed data, was "xeno-5.1.1.tar", last modified: Fri Apr 21 23:53:52 2023, max compression
```

## Comparing `xeno-5.1.0.tar` & `xeno-5.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-21 23:51:39.748570 xeno-5.1.0/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1567 2023-04-03 20:39:53.000000 xeno-5.1.0/LICENSE
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       18 2023-04-03 20:39:53.000000 xeno-5.1.0/MANIFEST.in
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-21 23:51:39.748570 xeno-5.1.0/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9195 2023-04-03 20:39:53.000000 xeno-5.1.0/README.md
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-04-21 23:51:39.748570 xeno-5.1.0/setup.cfg
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1160 2023-04-21 23:51:24.000000 xeno-5.1.0/setup.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-21 23:51:39.748570 xeno-5.1.0/xeno/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1808 2023-04-18 01:18:36.000000 xeno-5.1.0/xeno/__init__.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10174 2023-04-18 01:18:36.000000 xeno-5.1.0/xeno/abstract.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13407 2023-04-18 01:18:36.000000 xeno-5.1.0/xeno/async_injector.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7094 2023-04-18 01:18:36.000000 xeno-5.1.0/xeno/attributes.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    15648 2023-04-21 23:51:24.000000 xeno-5.1.0/xeno/build.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2956 2023-04-14 18:38:05.000000 xeno-5.1.0/xeno/color.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10080 2023-04-21 23:51:24.000000 xeno-5.1.0/xeno/cookbook.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4465 2023-04-18 01:18:36.000000 xeno-5.1.0/xeno/decorators.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2677 2023-04-14 18:38:05.000000 xeno-5.1.0/xeno/errors.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7250 2023-04-21 23:51:24.000000 xeno-5.1.0/xeno/events.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3018 2023-04-14 18:38:05.000000 xeno-5.1.0/xeno/namespaces.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1321 2023-04-14 18:38:05.000000 xeno-5.1.0/xeno/pkg_config.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    25924 2023-04-21 23:51:24.000000 xeno-5.1.0/xeno/recipe.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6738 2023-04-18 03:23:50.000000 xeno-5.1.0/xeno/shell.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1543 2023-04-18 01:18:36.000000 xeno-5.1.0/xeno/spinner.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7505 2023-04-18 01:18:36.000000 xeno-5.1.0/xeno/sync_injector.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1362 2023-04-18 01:18:36.000000 xeno-5.1.0/xeno/testing.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3258 2023-04-21 23:51:24.000000 xeno-5.1.0/xeno/utils.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-21 23:51:39.748570 xeno-5.1.0/xeno.egg-info/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-21 23:51:39.000000 xeno-5.1.0/xeno.egg-info/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      455 2023-04-21 23:51:39.000000 xeno-5.1.0/xeno.egg-info/SOURCES.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-04-21 23:51:39.000000 xeno-5.1.0/xeno.egg-info/dependency_links.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        5 2023-04-21 23:51:39.000000 xeno-5.1.0/xeno.egg-info/top_level.txt
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-21 23:53:52.465052 xeno-5.1.1/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1567 2023-04-03 20:39:53.000000 xeno-5.1.1/LICENSE
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       18 2023-04-03 20:39:53.000000 xeno-5.1.1/MANIFEST.in
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-21 23:53:52.465052 xeno-5.1.1/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9195 2023-04-03 20:39:53.000000 xeno-5.1.1/README.md
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-04-21 23:53:52.465052 xeno-5.1.1/setup.cfg
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1160 2023-04-21 23:53:33.000000 xeno-5.1.1/setup.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-21 23:53:52.465052 xeno-5.1.1/xeno/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1808 2023-04-18 01:18:36.000000 xeno-5.1.1/xeno/__init__.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10174 2023-04-18 01:18:36.000000 xeno-5.1.1/xeno/abstract.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13407 2023-04-18 01:18:36.000000 xeno-5.1.1/xeno/async_injector.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7094 2023-04-18 01:18:36.000000 xeno-5.1.1/xeno/attributes.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    15604 2023-04-21 23:53:25.000000 xeno-5.1.1/xeno/build.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2956 2023-04-14 18:38:05.000000 xeno-5.1.1/xeno/color.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10080 2023-04-21 23:51:24.000000 xeno-5.1.1/xeno/cookbook.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4465 2023-04-18 01:18:36.000000 xeno-5.1.1/xeno/decorators.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2677 2023-04-14 18:38:05.000000 xeno-5.1.1/xeno/errors.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7250 2023-04-21 23:51:24.000000 xeno-5.1.1/xeno/events.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3018 2023-04-14 18:38:05.000000 xeno-5.1.1/xeno/namespaces.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1321 2023-04-14 18:38:05.000000 xeno-5.1.1/xeno/pkg_config.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    25924 2023-04-21 23:51:24.000000 xeno-5.1.1/xeno/recipe.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6738 2023-04-18 03:23:50.000000 xeno-5.1.1/xeno/shell.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1543 2023-04-18 01:18:36.000000 xeno-5.1.1/xeno/spinner.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7505 2023-04-18 01:18:36.000000 xeno-5.1.1/xeno/sync_injector.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1362 2023-04-18 01:18:36.000000 xeno-5.1.1/xeno/testing.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3258 2023-04-21 23:51:24.000000 xeno-5.1.1/xeno/utils.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-21 23:53:52.465052 xeno-5.1.1/xeno.egg-info/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-21 23:53:52.000000 xeno-5.1.1/xeno.egg-info/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      455 2023-04-21 23:53:52.000000 xeno-5.1.1/xeno.egg-info/SOURCES.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-04-21 23:53:52.000000 xeno-5.1.1/xeno.egg-info/dependency_links.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        5 2023-04-21 23:53:52.000000 xeno-5.1.1/xeno.egg-info/top_level.txt
```

### Comparing `xeno-5.1.0/LICENSE` & `xeno-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/PKG-INFO` & `xeno-5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeno
-Version: 5.1.0
+Version: 5.1.1
 Summary: The Python dependency injector from outer space.
 Home-page: https://github.com/lainproliant/xeno
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: IOC dependency injector
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xeno-5.1.0/README.md` & `xeno-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/setup.py` & `xeno-5.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="xeno",
-    version="5.1.0",
+    version="5.1.1",
     description="The Python dependency injector from outer space.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lainproliant/xeno",
     author="Lain Musgrove (lainproliant)",
     author_email="lainproliant@gmail.com",
     license="BSD",
```

### Comparing `xeno-5.1.0/xeno/__init__.py` & `xeno-5.1.1/xeno/__init__.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/abstract.py` & `xeno-5.1.1/xeno/abstract.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/async_injector.py` & `xeno-5.1.1/xeno/async_injector.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/attributes.py` & `xeno-5.1.1/xeno/attributes.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/build.py` & `xeno-5.1.1/xeno/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,17 +270,14 @@
             if default_task is not None:
                 task_names = [default_task]
             else:
                 raise ValueError("No task specified and no default task defined.")
 
         tasks = [task_map[k] for k in task_names]
 
-        import pdb
-        pdb.set_trace()
-
         return tasks
 
     async def _make_tasks(self, config, tasks):
         self.scan.scan_params(*tasks)
         while self.scan.has_recipes():
             await self.scan.gather_all()
```

### Comparing `xeno-5.1.0/xeno/color.py` & `xeno-5.1.1/xeno/color.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/cookbook.py` & `xeno-5.1.1/xeno/cookbook.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/decorators.py` & `xeno-5.1.1/xeno/decorators.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/errors.py` & `xeno-5.1.1/xeno/errors.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/events.py` & `xeno-5.1.1/xeno/events.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/namespaces.py` & `xeno-5.1.1/xeno/namespaces.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/pkg_config.py` & `xeno-5.1.1/xeno/pkg_config.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/recipe.py` & `xeno-5.1.1/xeno/recipe.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/shell.py` & `xeno-5.1.1/xeno/shell.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/spinner.py` & `xeno-5.1.1/xeno/spinner.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/sync_injector.py` & `xeno-5.1.1/xeno/sync_injector.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/testing.py` & `xeno-5.1.1/xeno/testing.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno/utils.py` & `xeno-5.1.1/xeno/utils.py`

 * *Files identical despite different names*

### Comparing `xeno-5.1.0/xeno.egg-info/PKG-INFO` & `xeno-5.1.1/xeno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeno
-Version: 5.1.0
+Version: 5.1.1
 Summary: The Python dependency injector from outer space.
 Home-page: https://github.com/lainproliant/xeno
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: IOC dependency injector
 Classifier: Development Status :: 5 - Production/Stable
```

