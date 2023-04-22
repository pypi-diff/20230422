# Comparing `tmp/nobus-0.1.0.tar.gz` & `tmp/nobus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobus-0.1.0.tar", max compression
+gzip compressed data, was "nobus-0.1.1.tar", max compression
```

## Comparing `nobus-0.1.0.tar` & `nobus-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-04-22 15:17:25.200487 nobus-0.1.0/LICENSE
--rw-r--r--   0        0        0       43 2023-04-22 15:17:25.200597 nobus-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-22 15:22:41.911187 nobus-0.1.0/nobus/__init__.py
--rw-r--r--   0        0        0    11314 2023-04-22 15:23:41.084098 nobus-0.1.0/nobus/safeattr.py
--rw-r--r--   0        0        0      256 2023-04-22 15:25:31.274603 nobus-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 nobus-0.1.0/setup.py
--rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 nobus-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-22 15:17:25.200487 nobus-0.1.1/LICENSE
+-rw-r--r--   0        0        0       43 2023-04-22 15:17:25.200597 nobus-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 15:22:41.911187 nobus-0.1.1/nobus/__init__.py
+-rw-r--r--   0        0        0    11318 2023-04-22 15:29:57.626477 nobus-0.1.1/nobus/safeattr.py
+-rw-r--r--   0        0        0      256 2023-04-22 15:30:29.253362 nobus-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 nobus-0.1.1/setup.py
+-rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 nobus-0.1.1/PKG-INFO
```

### Comparing `nobus-0.1.0/LICENSE` & `nobus-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nobus-0.1.0/nobus/safeattr.py` & `nobus-0.1.1/nobus/safeattr.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,19 +107,19 @@
 
 class SafeAttrABC(ABC):
     @staticmethod
     def typed(x, type_=None, optional=False):
         return Typed(x, type_, optional)
     
     @staticmethod
-    def immut(x, type_=None, optional=False):
+    def immutable(x, type_=None, optional=False):
         return Immutable(x, type_, optional)
 
     @staticmethod
-    def Protected(x, type_=None, optional=False):
+    def protected(x, type_=None, optional=False):
         return Protected(x, type_, optional)
     
     def _safeattr_derive(self):
         if self.is_safeattr_derived_class:
             return
         
         cls = self.__class__
```

### Comparing `nobus-0.1.0/setup.py` & `nobus-0.1.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['nobus']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'nobus',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '# nobus\n"Nobody But Us" modules for Python\n',
     'author': 'Josh Nobus',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

