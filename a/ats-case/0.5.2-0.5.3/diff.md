# Comparing `tmp/ats_case-0.5.2.tar.gz` & `tmp/ats_case-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.5.2.tar", last modified: Fri Apr 21 03:49:32 2023, max compression
+gzip compressed data, was "ats_case-0.5.3.tar", last modified: Sat Apr 22 08:02:59 2023, max compression
```

## Comparing `ats_case-0.5.2.tar` & `ats_case-0.5.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 03:49:32.153328 ats_case-0.5.2/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.2/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-21 03:49:32.151336 ats_case-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 03:49:31.782241 ats_case-0.5.2/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.2/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:49:31.985736 ats_case-0.5.2/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.2/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17423 2023-04-21 02:50:28.000000 ats_case-0.5.2/ats_case/case/command.py
--rw-rw-rw-   0        0        0     9683 2023-04-20 08:35:14.000000 ats_case-0.5.2/ats_case/case/context.py
--rw-rw-rw-   0        0        0     6309 2023-04-21 03:45:03.000000 ats_case-0.5.2/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5593 2023-04-21 02:33:28.000000 ats_case-0.5.2/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:49:32.046576 ats_case-0.5.2/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.2/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.2/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.2/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:49:32.102724 ats_case-0.5.2/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.2/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.2/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.2/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:49:32.136602 ats_case-0.5.2/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.2/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.2/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-21 03:49:31.877987 ats_case-0.5.2/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-21 03:49:31.000000 ats_case-0.5.2/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-21 03:49:31.000000 ats_case-0.5.2/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 03:49:31.000000 ats_case-0.5.2/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-21 03:49:31.000000 ats_case-0.5.2/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 03:49:31.000000 ats_case-0.5.2/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 03:49:32.153328 ats_case-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-21 03:42:31.000000 ats_case-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 08:02:59.181251 ats_case-0.5.3/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-22 08:02:59.178886 ats_case-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 08:02:58.791593 ats_case-0.5.3/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.3/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 08:02:59.008314 ats_case-0.5.3/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.3/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17443 2023-04-22 08:02:29.000000 ats_case-0.5.3/ats_case/case/command.py
+-rw-rw-rw-   0        0        0     9683 2023-04-20 08:35:14.000000 ats_case-0.5.3/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     6309 2023-04-21 03:45:03.000000 ats_case-0.5.3/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5593 2023-04-21 02:33:28.000000 ats_case-0.5.3/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-22 08:02:59.073215 ats_case-0.5.3/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.3/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.3/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.3/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-22 08:02:59.134561 ats_case-0.5.3/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.3/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.3/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.3/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-22 08:02:59.168482 ats_case-0.5.3/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.3/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.3/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-22 08:02:58.883204 ats_case-0.5.3/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-22 08:02:58.000000 ats_case-0.5.3/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-22 08:02:58.000000 ats_case-0.5.3/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 08:02:58.000000 ats_case-0.5.3/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-22 08:02:58.000000 ats_case-0.5.3/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-22 08:02:58.000000 ats_case-0.5.3/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 08:02:59.181251 ats_case-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-22 08:02:46.000000 ats_case-0.5.3/setup.py
```

### Comparing `ats_case-0.5.2/PKG-INFO` & `ats_case-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.5.2
+Version: 0.5.3
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.2/README.md` & `ats_case-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.2/ats_case/case/command.py` & `ats_case-0.5.3/ats_case/case/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import time
 
 from ats_base.common import func
 from ats_base.log.logger import logger
-from ats_base.service import app, pro, em, udm
+from ats_base.service import app, pro, em, udm, build_in
 
 from ats_case.case.context import Context
 from ats_case.common.enum import *
 from ats_case.common.error import *
 
 """
     常用操作命令
@@ -142,15 +142,15 @@
     desc = param.get('desc')
 
     def decorate(callback):
         def fn(*args, **kwargs):
             client().message(desc).show(args[0])  # send(args[0], todo={'app:show': {'msg': desc}})
             r = callback(*args, **kwargs)
             return r
-        
+
         return fn
 
     return decorate
 
 
 """
     通讯协议篇
@@ -275,16 +275,16 @@
                 expect_result = context.runtime.steps[context.runtime.step - 1]
             except:
                 expect_result = None
             data = func.to_dict(result=self._parse, expect_result=expect_result, parameter=self._func_parameter)
 
             logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format(
                 self._func_module, self._func, self._func_parameter))
-            result = udm.acv(module='meter.{}'.format(self._func_module), function=self._func
-                             , data=data, url=context.acd_url)
+            result = udm.handle(module='meter.{}'.format(self._func_module), function=self._func
+                                , data=data, debug_url=context.acd_url)
             logger.info('~ @ACD<- module:{} function:{} result:{}'.format(self._func_module, self._func, result))
 
         return result
 
     def exec(self, context: Context):
         self.encode(context)
         result = send(context,
@@ -340,16 +340,16 @@
                                                                          result=self._result)})
 
     def acv(self, context: Context):
         data = func.to_dict(result=self._result)
 
         logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format(
             self._protocol.name, self._operation, self._parameter))
-        result = udm.acv(module='em.{}'.format(self._protocol.name), function=self._operation
-                         , data=data, url=context.acd_url)
+        result = udm.handle(module='em.{}'.format(self._protocol.name), function=self._operation
+                            , data=data, debug_url=context.acd_url)
         logger.info('~ @ACD<- module:{} function:{} result:{}'.format(self._protocol.name, self._operation, result))
 
         return result
 
     def exec(self, context: Context):
         self.handle(context)
         send(context, todo={'app:show': {'msg': self.acv(context)}})
@@ -399,40 +399,40 @@
         logger.info(
             '~ @BENCH-> manufacture:{} operation:{} parameter:{}'.format(self._manufacture, self._operation,
                                                                          self._parameter))
 
         if type(self._parameter) is dict:
             self._parameter = _replace_bench0(context, self._parameter)
         if self._function is not None and len(self._function) > 0:
-            self._built_in(context)
+            self._build_in(context)
 
     def decode(self, context: Context):
         logger.info('~ @BENCH<- manufacture:{} operation:{} result:{}'.format(self._manufacture,
                                                                               self._operation, self._result))
 
         self._result = self._result.get('result')
         self._flush(context)
 
-    def _built_in(self, context: Context):
+    def _build_in(self, context: Context):
         logger.info('~ @BUILTIN-> module:{} parameter:{}'.format('bench', self._parameter))
         for op, d in self._function.items():
-            v_data = udm.built_in(module='bench', function=op, data=func.to_dict(
+            v_data = build_in.handle(module='bench', function=op, data=func.to_dict(
                 param=d, iabc=context.meter.iabc, voltage=context.meter.rated_voltage,
-                current=context.meter.rated_current, index=self._exec_times), url=context.acd_url)
+                current=context.meter.rated_current, index=self._exec_times))
             self._parameter = _replace_bench1(self._parameter, v_data)
 
         logger.info('~ @BUILTIN<- module:{} parameter:{}'.format('bench', self._parameter))
 
     def acv(self, context: Context):
         data = func.to_dict(result=self._result)
 
         logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format(
             'bench', self._operation, self._result))
-        result = udm.acv(module='bench.{}'.format(self._manufacture), function=self._operation
-                         , data=data, url=context.acd_url)
+        result = udm.handle(module='bench.{}'.format(self._manufacture), function=self._operation
+                            , data=data, debug_url=context.acd_url)
         logger.info('~ @ACD<- module:{} function:{} result:{}'.format('bench', self._operation, result))
 
         return result
 
     def _flush(self, context: Context):
         context.runtime.steps.update({context.runtime.step: func.to_dict(obj='bench', op=self._operation
                                                                          , parameter=self._parameter,
```

### Comparing `ats_case-0.5.2/ats_case/case/context.py` & `ats_case-0.5.3/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.2/ats_case/case/executor.py` & `ats_case-0.5.3/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.2/ats_case/case/translator.py` & `ats_case-0.5.3/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.2/ats_case/common/error.py` & `ats_case-0.5.3/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.2/ats_case/manage/core.py` & `ats_case-0.5.3/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.2/ats_case/manage/start.py` & `ats_case-0.5.3/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.2/ats_case/template/testcase_v1.tmp` & `ats_case-0.5.3/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.2/ats_case.egg-info/PKG-INFO` & `ats_case-0.5.3/ats_case.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.5.2
+Version: 0.5.3
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.2/ats_case.egg-info/SOURCES.txt` & `ats_case-0.5.3/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.2/setup.py` & `ats_case-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.5.2",
+    version="0.5.3",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

