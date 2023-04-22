# Comparing `tmp/ezstools-2.4.tar.gz` & `tmp/ezstools-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezstools-2.4.tar", last modified: Tue Apr 11 21:30:04 2023, max compression
+gzip compressed data, was "ezstools-2.5.tar", last modified: Sat Apr 22 13:58:23 2023, max compression
```

## Comparing `ezstools-2.4.tar` & `ezstools-2.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 21:30:04.968792 ezstools-2.4/
--rw-rw-rw-   0        0        0     2546 2023-04-11 21:30:04.966797 ezstools-2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2255 2023-04-05 23:05:59.000000 ezstools-2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 21:30:04.913975 ezstools-2.4/ezstools/
--rw-rw-rw-   0        0        0      177 2023-04-11 20:47:41.000000 ezstools-2.4/ezstools/__init__.py
--rw-rw-rw-   0        0        0      714 2023-04-05 22:52:24.000000 ezstools-2.4/ezstools/console_utils.py
--rw-rw-rw-   0        0        0     1524 2021-11-16 00:24:08.000000 ezstools-2.4/ezstools/errorshelp.py
--rw-rw-rw-   0        0        0     1919 2023-04-05 22:51:37.000000 ezstools-2.4/ezstools/funcs.py
--rw-rw-rw-   0        0        0    11247 2022-07-25 16:30:19.000000 ezstools-2.4/ezstools/html_slice.py
--rw-rw-rw-   0        0        0     6230 2023-04-11 21:28:35.000000 ezstools-2.4/ezstools/iterator.py
--rw-rw-rw-   0        0        0     9064 2022-05-30 12:31:38.000000 ezstools-2.4/ezstools/json_tools.py
--rw-rw-rw-   0        0        0      330 2022-11-12 14:50:00.000000 ezstools-2.4/ezstools/module_tools.py
--rw-rw-rw-   0        0        0     1964 2022-05-30 12:28:59.000000 ezstools-2.4/ezstools/random_generator.py
--rw-rw-rw-   0        0        0     2027 2022-11-10 21:58:33.000000 ezstools-2.4/ezstools/simple_kv.py
--rw-rw-rw-   0        0        0     3565 2023-04-11 21:10:19.000000 ezstools-2.4/ezstools/string_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-11 21:30:04.952834 ezstools-2.4/ezstools.egg-info/
--rw-rw-rw-   0        0        0     2546 2023-04-11 21:30:04.000000 ezstools-2.4/ezstools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-04-11 21:30:04.000000 ezstools-2.4/ezstools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 21:30:04.000000 ezstools-2.4/ezstools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-11 21:30:04.000000 ezstools-2.4/ezstools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-11 21:30:04.000000 ezstools-2.4/ezstools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 21:30:04.969791 ezstools-2.4/setup.cfg
--rw-rw-rw-   0        0        0     1363 2023-04-11 21:25:52.000000 ezstools-2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:58:23.450237 ezstools-2.5/
+-rw-rw-rw-   0        0        0     2546 2023-04-22 13:58:23.429159 ezstools-2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2255 2023-04-05 23:05:59.000000 ezstools-2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 13:58:23.229074 ezstools-2.5/ezstools/
+-rw-rw-rw-   0        0        0      190 2023-04-22 13:06:30.000000 ezstools-2.5/ezstools/__init__.py
+-rw-rw-rw-   0        0        0      714 2023-04-05 22:52:24.000000 ezstools-2.5/ezstools/console_utils.py
+-rw-rw-rw-   0        0        0     1524 2021-11-16 00:24:08.000000 ezstools-2.5/ezstools/errorshelp.py
+-rw-rw-rw-   0        0        0     1919 2023-04-05 22:51:37.000000 ezstools-2.5/ezstools/funcs.py
+-rw-rw-rw-   0        0        0    11247 2022-07-25 16:30:19.000000 ezstools-2.5/ezstools/html_slice.py
+-rw-rw-rw-   0        0        0     6934 2023-04-21 20:23:27.000000 ezstools-2.5/ezstools/iterator.py
+-rw-rw-rw-   0        0        0     9064 2022-05-30 12:31:38.000000 ezstools-2.5/ezstools/json_tools.py
+-rw-rw-rw-   0        0        0      330 2022-11-12 14:50:00.000000 ezstools-2.5/ezstools/module_tools.py
+-rw-rw-rw-   0        0        0     1964 2022-05-30 12:28:59.000000 ezstools-2.5/ezstools/random_generator.py
+-rw-rw-rw-   0        0        0     2027 2022-11-10 21:58:33.000000 ezstools-2.5/ezstools/simple_kv.py
+-rw-rw-rw-   0        0        0     3565 2023-04-11 21:10:19.000000 ezstools-2.5/ezstools/string_tools.py
+-rw-rw-rw-   0        0        0     6104 2023-04-22 13:54:21.000000 ezstools-2.5/ezstools/traits.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:58:23.425176 ezstools-2.5/ezstools.egg-info/
+-rw-rw-rw-   0        0        0     2546 2023-04-22 13:58:21.000000 ezstools-2.5/ezstools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-04-22 13:58:21.000000 ezstools-2.5/ezstools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 13:58:21.000000 ezstools-2.5/ezstools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-22 13:58:21.000000 ezstools-2.5/ezstools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-22 13:58:21.000000 ezstools-2.5/ezstools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 13:58:23.451233 ezstools-2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1363 2023-04-11 21:25:52.000000 ezstools-2.5/setup.py
```

### Comparing `ezstools-2.4/PKG-INFO` & `ezstools-2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezstools
-Version: 2.4
+Version: 2.5
 Summary: Libreria Multi proposito, con modulos variados para ayudar con ciertos problemas
 Home-page: 
 Author: Hendrick Y. "NoVa
 Author-email: hendrickrodriguez.nova@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `ezstools-2.4/README.md` & `ezstools-2.5/README.md`

 * *Files identical despite different names*

### Comparing `ezstools-2.4/ezstools/console_utils.py` & `ezstools-2.5/ezstools/console_utils.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.4/ezstools/errorshelp.py` & `ezstools-2.5/ezstools/errorshelp.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.4/ezstools/funcs.py` & `ezstools-2.5/ezstools/funcs.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.4/ezstools/html_slice.py` & `ezstools-2.5/ezstools/html_slice.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.4/ezstools/iterator.py` & `ezstools-2.5/ezstools/iterator.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,43 @@
     i.any(lambda x: x % 2 == 0) # True
     i.all(lambda x: x % 2 == 0) # False
     ```
     """
     def __init__(self, iterable: Iterable) -> None:
         self._iterable = iterable
 
+    def convert_to(self, t: Type) -> Type:
+        """
+        #### Returns the iterator as the specified type.
+        Example:
+        ``` 
+        i = Iterator([1, 2, 3, 4, 5])
+        i.to(set)
+        ```
+        """
+        return t(self._iterable)
+
+    def to_set(self) -> set:
+        """
+        #### Returns the iterator as a set.
+        """
+        return set(self._iterable)
+
+    def to_list(self) -> list:
+        """
+        #### Returns the iterator as a list.
+        """
+        return list(self._iterable)
+    
+    def to_tuple(self) -> tuple:
+        """
+        #### Returns the iterator as a tuple.
+        """
+        return tuple(self._iterable)
+    
     def __iter__(self) -> Iterable:
         return iter(self._iterable)
     
     def __next__(self) -> object:
         return next(self._iterable)      
 
     def __getitem__(self, key: Union[int, slice]) -> object:
```

### Comparing `ezstools-2.4/ezstools/json_tools.py` & `ezstools-2.5/ezstools/json_tools.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.4/ezstools/random_generator.py` & `ezstools-2.5/ezstools/random_generator.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.4/ezstools/simple_kv.py` & `ezstools-2.5/ezstools/simple_kv.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.4/ezstools/string_tools.py` & `ezstools-2.5/ezstools/string_tools.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.4/ezstools.egg-info/PKG-INFO` & `ezstools-2.5/ezstools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezstools
-Version: 2.4
+Version: 2.5
 Summary: Libreria Multi proposito, con modulos variados para ayudar con ciertos problemas
 Home-page: 
 Author: Hendrick Y. "NoVa
 Author-email: hendrickrodriguez.nova@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `ezstools-2.4/setup.py` & `ezstools-2.5/setup.py`

 * *Files identical despite different names*

