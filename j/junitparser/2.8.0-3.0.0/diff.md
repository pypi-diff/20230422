# Comparing `tmp/junitparser-2.8.0.tar.gz` & `tmp/junitparser-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junitparser-2.8.0.tar", last modified: Fri Aug 19 08:42:50 2022, max compression
+gzip compressed data, was "junitparser-3.0.0.tar", last modified: Sat Apr 22 04:09:03 2023, max compression
```

## Comparing `junitparser-2.8.0.tar` & `junitparser-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 08:42:50.121614 junitparser-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-08-19 08:42:35.000000 junitparser-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7920 2022-08-19 08:42:50.121614 junitparser-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7340 2022-08-19 08:42:35.000000 junitparser-2.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 08:42:50.121614 junitparser-2.8.0/junitparser/
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-08-19 08:42:35.000000 junitparser-2.8.0/junitparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-08-19 08:42:35.000000 junitparser-2.8.0/junitparser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3077 2022-08-19 08:42:35.000000 junitparser-2.8.0/junitparser/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    22018 2022-08-19 08:42:35.000000 junitparser-2.8.0/junitparser/junitparser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 08:42:50.121614 junitparser-2.8.0/junitparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7920 2022-08-19 08:42:50.000000 junitparser-2.8.0/junitparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-08-19 08:42:50.000000 junitparser-2.8.0/junitparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-19 08:42:50.000000 junitparser-2.8.0/junitparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-08-19 08:42:50.000000 junitparser-2.8.0/junitparser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-19 08:42:50.000000 junitparser-2.8.0/junitparser.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-19 08:42:50.000000 junitparser-2.8.0/junitparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-19 08:42:50.000000 junitparser-2.8.0/junitparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-19 08:42:35.000000 junitparser-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-08-19 08:42:50.125614 junitparser-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-08-19 08:42:35.000000 junitparser-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:09:03.271137 junitparser-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-22 04:08:55.000000 junitparser-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-04-22 04:09:03.271137 junitparser-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-04-22 04:08:55.000000 junitparser-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:09:03.271137 junitparser-3.0.0/junitparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-22 04:08:55.000000 junitparser-3.0.0/junitparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-22 04:08:55.000000 junitparser-3.0.0/junitparser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-22 04:08:55.000000 junitparser-3.0.0/junitparser/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21378 2023-04-22 04:08:55.000000 junitparser-3.0.0/junitparser/junitparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:09:03.271137 junitparser-3.0.0/junitparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-04-22 04:09:03.000000 junitparser-3.0.0/junitparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-22 04:09:03.000000 junitparser-3.0.0/junitparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:09:03.000000 junitparser-3.0.0/junitparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-22 04:09:03.000000 junitparser-3.0.0/junitparser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:09:03.000000 junitparser-3.0.0/junitparser.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-22 04:09:03.000000 junitparser-3.0.0/junitparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-22 04:09:03.000000 junitparser-3.0.0/junitparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-22 04:08:55.000000 junitparser-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-22 04:09:03.271137 junitparser-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-22 04:08:55.000000 junitparser-3.0.0/setup.py
```

### Comparing `junitparser-2.8.0/LICENSE` & `junitparser-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `junitparser-2.8.0/PKG-INFO` & `junitparser-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: junitparser
-Version: 2.8.0
+Version: 3.0.0
 Summary: Manipulates JUnit/xUnit Result XML files
 Home-page: https://github.com/weiwei/junitparser
 Author: Weiwei Wang
 Author-email: gastlygem@gmail.com
 License: Apache 2.0
 Keywords: junit xunit xml parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Text Processing
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 junitparser -- Pythonic JUnit/xUnit Result XML Parser
 ======================================================
 
 .. image:: https://github.com/weiwei/junitparser/workflows/build/badge.svg?branch=master
```

### Comparing `junitparser-2.8.0/README.rst` & `junitparser-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `junitparser-2.8.0/junitparser/cli.py` & `junitparser-3.0.0/junitparser/cli.py`

 * *Files identical despite different names*

### Comparing `junitparser-2.8.0/junitparser/junitparser.py` & `junitparser-3.0.0/junitparser/junitparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,39 +2,22 @@
 junitparser is a JUnit/xUnit Result XML Parser. Use it to parse and manipulate
 existing Result XML files, or create new JUnit/xUnit result XMLs from scratch.
 
 :copyright: (c) 2019 by Joel Wang.
 :license: Apache2, see LICENSE for more details.
 """
 
-from __future__ import with_statement
-from __future__ import absolute_import
-from __future__ import unicode_literals
-from future.utils import with_metaclass
-from builtins import object
-from io import open
 import itertools
-
-try:
-    import itertools.izip as zip
-except ImportError:
-    pass
+from copy import deepcopy
 
 try:
     from lxml import etree
 except ImportError:
     from xml.etree import ElementTree as etree
 
-from copy import deepcopy
-
-try:
-    type(unicode)
-except NameError:
-    unicode = str
-
 
 def write_xml(obj, filepath=None, pretty=False, to_console=False):
     tree = etree.ElementTree(obj._elem)
     if filepath is None:
         filepath = obj.filepath
     if filepath is None:
         raise JUnitXmlError("Missing filepath argument.")
@@ -80,55 +63,55 @@
     def __get__(self, instance, cls):
         """Gets value from attribute, return None if attribute doesn't exist."""
         return instance._elem.attrib.get(self.name)
 
     def __set__(self, instance, value):
         """Sets XML element attribute."""
         if value is not None:
-            instance._elem.attrib[self.name] = unicode(value)
+            instance._elem.attrib[self.name] = str(value)
 
 
 class IntAttr(Attr):
     """An integer attribute for an XML element.
 
     This class is used internally for counting test cases, but you could use
     it for any specific purpose.
     """
 
     def __get__(self, instance, cls):
-        result = super(IntAttr, self).__get__(instance, cls)
+        result = super().__get__(instance, cls)
         if result is None and isinstance(instance, (JUnitXml, TestSuite)):
             instance.update_statistics()
-            result = super(IntAttr, self).__get__(instance, cls)
+            result = super().__get__(instance, cls)
         return int(result) if result else None
 
     def __set__(self, instance, value):
         if not isinstance(value, int):
             raise TypeError("Expected integer value.")
-        super(IntAttr, self).__set__(instance, value)
+        super().__set__(instance, value)
 
 
 class FloatAttr(Attr):
     """A float attribute for an XML element.
 
     This class is used internally for counting test durations, but you could
     use it for any specific purpose.
     """
 
     def __get__(self, instance, cls):
-        result = super(FloatAttr, self).__get__(instance, cls)
+        result = super().__get__(instance, cls)
         if result is None and isinstance(instance, (JUnitXml, TestSuite)):
             instance.update_statistics()
-            result = super(FloatAttr, self).__get__(instance, cls)
+            result = super().__get__(instance, cls)
         return float(result.replace(",", "")) if result else None
 
     def __set__(self, instance, value):
         if not (isinstance(value, float) or isinstance(value, int)):
             raise TypeError("Expected float value.")
-        super(FloatAttr, self).__set__(instance, value)
+        super().__set__(instance, value)
 
 
 def attributed(cls):
     """Decorator to read XML element attribute name from class attribute."""
     for key, value in vars(cls).items():
         if isinstance(value, Attr):
             value.name = key
@@ -140,15 +123,15 @@
 
     def __new__(meta, name, bases, methods):
         cls = super(junitxml, meta).__new__(meta, name, bases, methods)
         cls = attributed(cls)
         return cls
 
 
-class Element(with_metaclass(junitxml, object)):
+class Element(metaclass=junitxml):
     """Base class for all Junit XML elements."""
 
     def __init__(self, name=None):
         if not name:
             name = self._tag
         self._elem = etree.Element(name)
 
@@ -239,20 +222,20 @@
     time = FloatAttr()
     tests = IntAttr()
     failures = IntAttr()
     errors = IntAttr()
     skipped = IntAttr()
 
     def __init__(self, name=None):
-        super(JUnitXml, self).__init__(self._tag)
+        super().__init__(self._tag)
         self.filepath = None
         self.name = name
 
     def __iter__(self):
-        return super(JUnitXml, self).iterchildren(TestSuite)
+        return super().iterchildren(TestSuite)
 
     def __len__(self):
         return len(list(self.__iter__()))
 
     def __add__(self, other):
         result = JUnitXml()
         for suite in self:
@@ -360,24 +343,24 @@
     timestamp = Attr()
     tests = IntAttr()
     failures = IntAttr()
     errors = IntAttr()
     skipped = IntAttr()
 
     def __init__(self, name=None):
-        super(TestSuite, self).__init__(self._tag)
+        super().__init__(self._tag)
         self.name = name
         self.filepath = None
 
     def __iter__(self):
         return itertools.chain(
-            super(TestSuite, self).iterchildren(TestCase),
+            super().iterchildren(TestCase),
             (
                 case
-                for suite in super(TestSuite, self).iterchildren(TestSuite)
+                for suite in super().iterchildren(TestSuite)
                 for case in suite
             ),
         )
 
     def __len__(self):
         return len(list(self.__iter__()))
 
@@ -429,15 +412,15 @@
         result.add_testsuite(other)
         return result
 
     def remove_testcase(self, testcase):
         """Removes a test case from the suite."""
         for case in self:
             if case == testcase:
-                super(TestSuite, self).remove(case)
+                super().remove(case)
                 self.update_statistics()
 
     def update_statistics(self):
         """Updates test count and test time."""
         tests = errors = failures = skipped = 0
         time = 0
         for case in self:
@@ -522,21 +505,21 @@
 
     See :class:`Property`
     """
 
     _tag = "properties"
 
     def __init__(self):
-        super(Properties, self).__init__(self._tag)
+        super().__init__(self._tag)
 
     def add_property(self, property_):
         self.append(property_)
 
     def __iter__(self):
-        return super(Properties, self).iterchildren(Property)
+        return super().iterchildren(Property)
 
     def __eq__(self, other):
         p1 = list(self)
         p2 = list(other)
         p1.sort()
         p2.sort()
         if len(p1) != len(p2):
@@ -558,15 +541,15 @@
     """
 
     _tag = "property"
     name = Attr()
     value = Attr()
 
     def __init__(self, name=None, value=None):
-        super(Property, self).__init__(self._tag)
+        super().__init__(self._tag)
         self.name = name
         self.value = value
 
     def __eq__(self, other):
         return self.name == other.name and self.value == other.value
 
     def __ne__(self, other):
@@ -614,33 +597,33 @@
 
 class Skipped(Result):
     """Test result when the case is skipped."""
 
     _tag = "skipped"
 
     def __eq__(self, other):
-        return super(Skipped, self).__eq__(other)
+        return super().__eq__(other)
 
 
 class Failure(Result):
     """Test result when the case failed."""
 
     _tag = "failure"
 
     def __eq__(self, other):
-        return super(Failure, self).__eq__(other)
+        return super().__eq__(other)
 
 
 class Error(Result):
     """Test result when the case has errors during execution."""
 
     _tag = "error"
 
     def __eq__(self, other):
-        return super(Error, self).__eq__(other)
+        return super().__eq__(other)
 
 
 POSSIBLE_RESULTS = {Failure, Error, Skipped}
 
 
 class TestCase(Element):
     """Object to store a testcase and its result.
@@ -658,24 +641,24 @@
 
     _tag = "testcase"
     name = Attr()
     classname = Attr()
     time = FloatAttr()
 
     def __init__(self, name=None, classname=None, time=None):
-        super(TestCase, self).__init__(self._tag)
+        super().__init__(self._tag)
         if name is not None:
             self.name = name
         if classname is not None:
             self.classname = classname
         if time is not None:
             self.time = float(time)
 
     def __hash__(self):
-        return super(TestCase, self).__hash__()
+        return super().__hash__()
 
     def __iter__(self):
         all_types = set.union(POSSIBLE_RESULTS, {SystemOut}, {SystemErr})
         for elem in self._elem.iter():
             for entry_type in all_types:
                 if elem.tag == entry_type._tag:
                     yield entry_type.fromelem(elem)
@@ -706,15 +689,15 @@
                 results.append(entry)
 
         return results
 
     @result.setter
     def result(self, value):
         # First remove all existing results
-        for entry in self:
+        for entry in self.result:
             if any(isinstance(entry, r) for r in POSSIBLE_RESULTS):
                 self.remove(entry)
         for entry in value:
             if any(isinstance(entry, r) for r in POSSIBLE_RESULTS):
                 self.append(entry)
 
     @property
@@ -758,15 +741,15 @@
     Attributes:
         text: the output message
     """
 
     _tag = ""
 
     def __init__(self, content=None):
-        super(System, self).__init__(self._tag)
+        super().__init__(self._tag)
         self.text = content
 
     @property
     def text(self):
         return self._elem.text
 
     @text.setter
```

### Comparing `junitparser-2.8.0/junitparser.egg-info/PKG-INFO` & `junitparser-3.0.0/junitparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: junitparser
-Version: 2.8.0
+Version: 3.0.0
 Summary: Manipulates JUnit/xUnit Result XML files
 Home-page: https://github.com/weiwei/junitparser
 Author: Weiwei Wang
 Author-email: gastlygem@gmail.com
 License: Apache 2.0
 Keywords: junit xunit xml parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Text Processing
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 junitparser -- Pythonic JUnit/xUnit Result XML Parser
 ======================================================
 
 .. image:: https://github.com/weiwei/junitparser/workflows/build/badge.svg?branch=master
```

### Comparing `junitparser-2.8.0/setup.py` & `junitparser-3.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     description="Manipulates JUnit/xUnit Result XML files",
     long_description=read("README.rst"),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Text Processing",
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
     ],
     url="https://github.com/weiwei/junitparser",
     author="Weiwei Wang",
     author_email="gastlygem@gmail.com",
     license="Apache 2.0",
     install_requires=["future"],
```

