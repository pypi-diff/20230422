# Comparing `tmp/styledlogger-0.0.3.tar.gz` & `tmp/styledlogger-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "styledlogger-0.0.3.tar", last modified: Sat Apr 22 10:06:34 2023, max compression
+gzip compressed data, was "styledlogger-0.0.4.tar", last modified: Sat Apr 22 11:39:24 2023, max compression
```

## Comparing `styledlogger-0.0.3.tar` & `styledlogger-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-22 10:06:34.932707 styledlogger-0.0.3/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1338 2023-04-20 07:54:38.000000 styledlogger-0.0.3/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1547 2023-04-22 10:06:34.932707 styledlogger-0.0.3/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1045 2023-04-22 10:04:56.000000 styledlogger-0.0.3/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-22 10:06:34.932707 styledlogger-0.0.3/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      998 2023-04-22 10:06:19.000000 styledlogger-0.0.3/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-22 10:06:34.928707 styledlogger-0.0.3/styledlogger/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      104 2023-04-22 09:45:32.000000 styledlogger-0.0.3/styledlogger/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-22 10:06:34.932707 styledlogger-0.0.3/styledlogger/classes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-21 11:27:07.000000 styledlogger-0.0.3/styledlogger/classes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      821 2023-04-21 11:27:07.000000 styledlogger-0.0.3/styledlogger/classes/printcolors.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      296 2023-04-21 11:27:07.000000 styledlogger-0.0.3/styledlogger/classes/printtypes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2988 2023-04-22 09:59:27.000000 styledlogger-0.0.3/styledlogger/classes/styleconfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2182 2023-04-21 11:30:14.000000 styledlogger-0.0.3/styledlogger/logger.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-22 10:06:34.928707 styledlogger-0.0.3/styledlogger.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1547 2023-04-22 10:06:34.000000 styledlogger-0.0.3/styledlogger.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      393 2023-04-22 10:06:34.000000 styledlogger-0.0.3/styledlogger.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-22 10:06:34.000000 styledlogger-0.0.3/styledlogger.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       61 2023-04-22 10:06:34.000000 styledlogger-0.0.3/styledlogger.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-04-22 10:06:34.000000 styledlogger-0.0.3/styledlogger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:39:24.119378 styledlogger-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-22 11:39:14.000000 styledlogger-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-22 11:39:24.119378 styledlogger-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-22 11:39:14.000000 styledlogger-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 11:39:24.119378 styledlogger-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-22 11:39:14.000000 styledlogger-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:39:24.119378 styledlogger-0.0.4/styledlogger/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-22 11:39:14.000000 styledlogger-0.0.4/styledlogger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:39:24.119378 styledlogger-0.0.4/styledlogger/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:39:14.000000 styledlogger-0.0.4/styledlogger/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-22 11:39:14.000000 styledlogger-0.0.4/styledlogger/classes/printcolors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-22 11:39:14.000000 styledlogger-0.0.4/styledlogger/classes/printtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-22 11:39:14.000000 styledlogger-0.0.4/styledlogger/classes/styleconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-22 11:39:14.000000 styledlogger-0.0.4/styledlogger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:39:24.119378 styledlogger-0.0.4/styledlogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-22 11:39:24.000000 styledlogger-0.0.4/styledlogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-22 11:39:24.000000 styledlogger-0.0.4/styledlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 11:39:24.000000 styledlogger-0.0.4/styledlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-22 11:39:24.000000 styledlogger-0.0.4/styledlogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-22 11:39:24.000000 styledlogger-0.0.4/styledlogger.egg-info/top_level.txt
```

### Comparing `styledlogger-0.0.3/LICENSE` & `styledlogger-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `styledlogger-0.0.3/PKG-INFO` & `styledlogger-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: styledlogger
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple, styled logging library.
 Home-page: https://github.com/SpLayzDK/StyledLogger/
 Author: ImAlek (splayzdk)
 Author-email: alek@imalek.me
 License: BSL 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
@@ -33,13 +33,14 @@
 >>> logger.debug("This is just a test print")
 9:55:30 :: DEBU @ Main - This is just a test print
 
 >>> logger.error("Could not fetch url 'https://example.com'")
 10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
 
 >>> from styledlogger import StyleConfig
->>> logger.set_style(StyleConfig( text_format="(%time%) | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs
+>>> logger.set_style(StyleConfig( text_format="(%time%) | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
+>>> logger.warn("CPU usage exceeding 90%")
 (22/04/2023 10:01) | WARN - CPU usage exceeding 90%
 ```
 
 Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
 Contact me at mail: alek@imalek.me
```

### Comparing `styledlogger-0.0.3/README.md` & `styledlogger-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,13 +17,14 @@
 >>> logger.debug("This is just a test print")
 9:55:30 :: DEBU @ Main - This is just a test print
 
 >>> logger.error("Could not fetch url 'https://example.com'")
 10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
 
 >>> from styledlogger import StyleConfig
->>> logger.set_style(StyleConfig( text_format="(%time%) | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs
+>>> logger.set_style(StyleConfig( text_format="(%time%) | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
+>>> logger.warn("CPU usage exceeding 90%")
 (22/04/2023 10:01) | WARN - CPU usage exceeding 90%
 ```
 
 Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
 Contact me at mail: alek@imalek.me
```

### Comparing `styledlogger-0.0.3/setup.py` & `styledlogger-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     # Basics
     name='styledlogger',
-    version='0.0.3',
+    version='0.0.4',
     description='A simple, styled logging library.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     
     # Author
     author='ImAlek (splayzdk)',
     author_email='alek@imalek.me',
@@ -37,8 +37,8 @@
     extras_require={
         'dev': [
             'pytest>=7.0',
             "twine>=4.0.2"
         ]
     }
 
-)
+)
```

### Comparing `styledlogger-0.0.3/styledlogger/classes/printcolors.py` & `styledlogger-0.0.4/styledlogger/classes/printcolors.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.0.3/styledlogger/classes/styleconfig.py` & `styledlogger-0.0.4/styledlogger/classes/styleconfig.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.0.3/styledlogger/logger.py` & `styledlogger-0.0.4/styledlogger/logger.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.0.3/styledlogger.egg-info/PKG-INFO` & `styledlogger-0.0.4/styledlogger.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: styledlogger
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple, styled logging library.
 Home-page: https://github.com/SpLayzDK/StyledLogger/
 Author: ImAlek (splayzdk)
 Author-email: alek@imalek.me
 License: BSL 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
@@ -33,13 +33,14 @@
 >>> logger.debug("This is just a test print")
 9:55:30 :: DEBU @ Main - This is just a test print
 
 >>> logger.error("Could not fetch url 'https://example.com'")
 10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
 
 >>> from styledlogger import StyleConfig
->>> logger.set_style(StyleConfig( text_format="(%time%) | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs
+>>> logger.set_style(StyleConfig( text_format="(%time%) | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
+>>> logger.warn("CPU usage exceeding 90%")
 (22/04/2023 10:01) | WARN - CPU usage exceeding 90%
 ```
 
 Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
 Contact me at mail: alek@imalek.me
```

