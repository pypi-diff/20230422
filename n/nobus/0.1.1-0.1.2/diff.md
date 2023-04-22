# Comparing `tmp/nobus-0.1.1.tar.gz` & `tmp/nobus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobus-0.1.1.tar", max compression
+gzip compressed data, was "nobus-0.1.2.tar", max compression
```

## Comparing `nobus-0.1.1.tar` & `nobus-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-04-22 15:17:25.200487 nobus-0.1.1/LICENSE
--rw-r--r--   0        0        0       43 2023-04-22 15:17:25.200597 nobus-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-22 15:22:41.911187 nobus-0.1.1/nobus/__init__.py
--rw-r--r--   0        0        0    11318 2023-04-22 15:29:57.626477 nobus-0.1.1/nobus/safeattr.py
--rw-r--r--   0        0        0      256 2023-04-22 15:30:29.253362 nobus-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 nobus-0.1.1/setup.py
--rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 nobus-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-22 15:17:25.200487 nobus-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1081 2023-04-22 16:46:49.568611 nobus-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 15:22:41.911187 nobus-0.1.2/nobus/__init__.py
+-rw-r--r--   0        0        0    11307 2023-04-22 17:04:49.898539 nobus-0.1.2/nobus/safeattr.py
+-rw-r--r--   0        0        0      256 2023-04-22 17:05:33.468640 nobus-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1579 1970-01-01 00:00:00.000000 nobus-0.1.2/setup.py
+-rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 nobus-0.1.2/PKG-INFO
```

### Comparing `nobus-0.1.1/LICENSE` & `nobus-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nobus-0.1.1/nobus/safeattr.py` & `nobus-0.1.2/nobus/safeattr.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self._value = value
         self._type = type_
         self._optional = optional
 
     def __repr__(self):
         xs = f"{self.__class__.__name__}(value={self.value.__repr__()}"
         if self.type is not None:
-            xs += f", type_={self.type.__repr__()}"
+            xs += f", type_={self.type}"
         xs += f", optional={self.optional.__repr__()}"
         xs += ")"
         return xs
         
     @property
     def value(self):
         return self._value
```

