# Comparing `tmp/ezstools-2.5.tar.gz` & `tmp/ezstools-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezstools-2.5.tar", last modified: Sat Apr 22 13:58:23 2023, max compression
+gzip compressed data, was "ezstools-2.5.1.tar", last modified: Sat Apr 22 14:01:32 2023, max compression
```

## Comparing `ezstools-2.5.tar` & `ezstools-2.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 13:58:23.450237 ezstools-2.5/
--rw-rw-rw-   0        0        0     2546 2023-04-22 13:58:23.429159 ezstools-2.5/PKG-INFO
--rw-rw-rw-   0        0        0     2255 2023-04-05 23:05:59.000000 ezstools-2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 13:58:23.229074 ezstools-2.5/ezstools/
--rw-rw-rw-   0        0        0      190 2023-04-22 13:06:30.000000 ezstools-2.5/ezstools/__init__.py
--rw-rw-rw-   0        0        0      714 2023-04-05 22:52:24.000000 ezstools-2.5/ezstools/console_utils.py
--rw-rw-rw-   0        0        0     1524 2021-11-16 00:24:08.000000 ezstools-2.5/ezstools/errorshelp.py
--rw-rw-rw-   0        0        0     1919 2023-04-05 22:51:37.000000 ezstools-2.5/ezstools/funcs.py
--rw-rw-rw-   0        0        0    11247 2022-07-25 16:30:19.000000 ezstools-2.5/ezstools/html_slice.py
--rw-rw-rw-   0        0        0     6934 2023-04-21 20:23:27.000000 ezstools-2.5/ezstools/iterator.py
--rw-rw-rw-   0        0        0     9064 2022-05-30 12:31:38.000000 ezstools-2.5/ezstools/json_tools.py
--rw-rw-rw-   0        0        0      330 2022-11-12 14:50:00.000000 ezstools-2.5/ezstools/module_tools.py
--rw-rw-rw-   0        0        0     1964 2022-05-30 12:28:59.000000 ezstools-2.5/ezstools/random_generator.py
--rw-rw-rw-   0        0        0     2027 2022-11-10 21:58:33.000000 ezstools-2.5/ezstools/simple_kv.py
--rw-rw-rw-   0        0        0     3565 2023-04-11 21:10:19.000000 ezstools-2.5/ezstools/string_tools.py
--rw-rw-rw-   0        0        0     6104 2023-04-22 13:54:21.000000 ezstools-2.5/ezstools/traits.py
-drwxrwxrwx   0        0        0        0 2023-04-22 13:58:23.425176 ezstools-2.5/ezstools.egg-info/
--rw-rw-rw-   0        0        0     2546 2023-04-22 13:58:21.000000 ezstools-2.5/ezstools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-04-22 13:58:21.000000 ezstools-2.5/ezstools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 13:58:21.000000 ezstools-2.5/ezstools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-22 13:58:21.000000 ezstools-2.5/ezstools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-22 13:58:21.000000 ezstools-2.5/ezstools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 13:58:23.451233 ezstools-2.5/setup.cfg
--rw-rw-rw-   0        0        0     1363 2023-04-11 21:25:52.000000 ezstools-2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:01:32.845766 ezstools-2.5.1/
+-rw-rw-rw-   0        0        0     2645 2023-04-22 14:01:32.843773 ezstools-2.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2352 2023-04-22 14:01:14.000000 ezstools-2.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 14:01:32.775953 ezstools-2.5.1/ezstools/
+-rw-rw-rw-   0        0        0      190 2023-04-22 13:06:30.000000 ezstools-2.5.1/ezstools/__init__.py
+-rw-rw-rw-   0        0        0      714 2023-04-05 22:52:24.000000 ezstools-2.5.1/ezstools/console_utils.py
+-rw-rw-rw-   0        0        0     1524 2021-11-16 00:24:08.000000 ezstools-2.5.1/ezstools/errorshelp.py
+-rw-rw-rw-   0        0        0     1919 2023-04-05 22:51:37.000000 ezstools-2.5.1/ezstools/funcs.py
+-rw-rw-rw-   0        0        0    11247 2022-07-25 16:30:19.000000 ezstools-2.5.1/ezstools/html_slice.py
+-rw-rw-rw-   0        0        0     6934 2023-04-21 20:23:27.000000 ezstools-2.5.1/ezstools/iterator.py
+-rw-rw-rw-   0        0        0     9064 2022-05-30 12:31:38.000000 ezstools-2.5.1/ezstools/json_tools.py
+-rw-rw-rw-   0        0        0      330 2022-11-12 14:50:00.000000 ezstools-2.5.1/ezstools/module_tools.py
+-rw-rw-rw-   0        0        0     1964 2022-05-30 12:28:59.000000 ezstools-2.5.1/ezstools/random_generator.py
+-rw-rw-rw-   0        0        0     2027 2022-11-10 21:58:33.000000 ezstools-2.5.1/ezstools/simple_kv.py
+-rw-rw-rw-   0        0        0     3565 2023-04-11 21:10:19.000000 ezstools-2.5.1/ezstools/string_tools.py
+-rw-rw-rw-   0        0        0     6104 2023-04-22 13:54:21.000000 ezstools-2.5.1/ezstools/traits.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:01:32.839784 ezstools-2.5.1/ezstools.egg-info/
+-rw-rw-rw-   0        0        0     2645 2023-04-22 14:01:32.000000 ezstools-2.5.1/ezstools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-04-22 14:01:32.000000 ezstools-2.5.1/ezstools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 14:01:32.000000 ezstools-2.5.1/ezstools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-22 14:01:32.000000 ezstools-2.5.1/ezstools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-22 14:01:32.000000 ezstools-2.5.1/ezstools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 14:01:32.845766 ezstools-2.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1363 2023-04-11 21:25:52.000000 ezstools-2.5.1/setup.py
```

### Comparing `ezstools-2.5/PKG-INFO` & `ezstools-2.5.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: ezstools
-Version: 2.5
-Summary: Libreria Multi proposito, con modulos variados para ayudar con ciertos problemas
-Home-page: 
-Author: Hendrick Y. "NoVa
-Author-email: hendrickrodriguez.nova@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-
 # ezstools
 Ezstools is a Python library that provides a variety of tools and modules to help developers deal with common issues. Whether you need to manipulate JSON files, generate random data, or interact with the console, ezstools has you covered.
 
 *Disclaimer: This library is still in development and is not yet ready for production use.*
 
 ## Installation
 ```bash
@@ -36,18 +26,19 @@
         "Hello world",
         "ezstools",
         "hello",
         random_string(length=10)
     ]
 )) 
 ```
-
-
 ## Modules:
 
+### traits
+Provides a collection of typing hints, decorators and classes to mimic Rust's traits.
+
 ### console_utils
 contains methods to interact with the console, including methods to display links and pick menus.
 
 ### funcs
 provides a collection of general-purpose functions, such as timeit for timing code snippets and convert_num for converting a string to a number.
 
 ### json_tools
@@ -69,8 +60,8 @@
 ### simple_kv
 The simple_kv module provides tools to interact and manipulate simple key-value files (.skv), a custom file format.
 
 ### module_tools
 provides tools to create and interact with Python modules, such as methods to import and reload modules.
 
 # LICENSE
-`ezstools` is licensed under the MIT License. Please see the LICENSE file for more information.
+`ezstools` is licensed under the MIT License. Please see the LICENSE file for more information.
```

### Comparing `ezstools-2.5/README.md` & `ezstools-2.5.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: ezstools
+Version: 2.5.1
+Summary: Libreria Multi proposito, con modulos variados para ayudar con ciertos problemas
+Home-page: 
+Author: Hendrick Y. "NoVa
+Author-email: hendrickrodriguez.nova@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+
 # ezstools
 Ezstools is a Python library that provides a variety of tools and modules to help developers deal with common issues. Whether you need to manipulate JSON files, generate random data, or interact with the console, ezstools has you covered.
 
 *Disclaimer: This library is still in development and is not yet ready for production use.*
 
 ## Installation
 ```bash
@@ -26,18 +36,19 @@
         "Hello world",
         "ezstools",
         "hello",
         random_string(length=10)
     ]
 )) 
 ```
-
-
 ## Modules:
 
+### traits
+Provides a collection of typing hints, decorators and classes to mimic Rust's traits.
+
 ### console_utils
 contains methods to interact with the console, including methods to display links and pick menus.
 
 ### funcs
 provides a collection of general-purpose functions, such as timeit for timing code snippets and convert_num for converting a string to a number.
 
 ### json_tools
@@ -59,8 +70,8 @@
 ### simple_kv
 The simple_kv module provides tools to interact and manipulate simple key-value files (.skv), a custom file format.
 
 ### module_tools
 provides tools to create and interact with Python modules, such as methods to import and reload modules.
 
 # LICENSE
-`ezstools` is licensed under the MIT License. Please see the LICENSE file for more information.
+`ezstools` is licensed under the MIT License. Please see the LICENSE file for more information.
```

### Comparing `ezstools-2.5/ezstools/console_utils.py` & `ezstools-2.5.1/ezstools/console_utils.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.5/ezstools/errorshelp.py` & `ezstools-2.5.1/ezstools/errorshelp.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.5/ezstools/funcs.py` & `ezstools-2.5.1/ezstools/funcs.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.5/ezstools/html_slice.py` & `ezstools-2.5.1/ezstools/html_slice.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.5/ezstools/iterator.py` & `ezstools-2.5.1/ezstools/iterator.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.5/ezstools/json_tools.py` & `ezstools-2.5.1/ezstools/json_tools.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.5/ezstools/random_generator.py` & `ezstools-2.5.1/ezstools/random_generator.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.5/ezstools/simple_kv.py` & `ezstools-2.5.1/ezstools/simple_kv.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.5/ezstools/string_tools.py` & `ezstools-2.5.1/ezstools/string_tools.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.5/ezstools/traits.py` & `ezstools-2.5.1/ezstools/traits.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.5/ezstools.egg-info/PKG-INFO` & `ezstools-2.5.1/ezstools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezstools
-Version: 2.5
+Version: 2.5.1
 Summary: Libreria Multi proposito, con modulos variados para ayudar con ciertos problemas
 Home-page: 
 Author: Hendrick Y. "NoVa
 Author-email: hendrickrodriguez.nova@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
@@ -36,18 +36,19 @@
         "Hello world",
         "ezstools",
         "hello",
         random_string(length=10)
     ]
 )) 
 ```
-
-
 ## Modules:
 
+### traits
+Provides a collection of typing hints, decorators and classes to mimic Rust's traits.
+
 ### console_utils
 contains methods to interact with the console, including methods to display links and pick menus.
 
 ### funcs
 provides a collection of general-purpose functions, such as timeit for timing code snippets and convert_num for converting a string to a number.
 
 ### json_tools
```

### Comparing `ezstools-2.5/setup.py` & `ezstools-2.5.1/setup.py`

 * *Files identical despite different names*

