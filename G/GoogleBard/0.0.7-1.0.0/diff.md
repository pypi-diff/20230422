# Comparing `tmp/GoogleBard-0.0.7.tar.gz` & `tmp/GoogleBard-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleBard-0.0.7.tar", last modified: Fri Apr 14 12:23:00 2023, max compression
+gzip compressed data, was "GoogleBard-1.0.0.tar", last modified: Sat Apr 22 12:42:52 2023, max compression
```

## Comparing `GoogleBard-0.0.7.tar` & `GoogleBard-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:23:00.916013 GoogleBard-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-14 12:22:38.000000 GoogleBard-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-14 12:23:00.916013 GoogleBard-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-14 12:22:38.000000 GoogleBard-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:23:00.916013 GoogleBard-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 12:22:38.000000 GoogleBard-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:23:00.916013 GoogleBard-0.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-14 12:22:38.000000 GoogleBard-0.0.7/src/Bard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:23:00.916013 GoogleBard-0.0.7/src/GoogleBard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-14 12:23:00.000000 GoogleBard-0.0.7/src/GoogleBard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-14 12:23:00.000000 GoogleBard-0.0.7/src/GoogleBard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:23:00.000000 GoogleBard-0.0.7/src/GoogleBard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 12:23:00.000000 GoogleBard-0.0.7/src/GoogleBard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 12:23:00.000000 GoogleBard-0.0.7/src/GoogleBard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:42:52.382361 GoogleBard-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-22 12:42:30.000000 GoogleBard-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-22 12:42:52.382361 GoogleBard-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-22 12:42:30.000000 GoogleBard-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 12:42:52.382361 GoogleBard-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 12:42:30.000000 GoogleBard-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:42:52.382361 GoogleBard-1.0.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-22 12:42:30.000000 GoogleBard-1.0.0/src/Bard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:42:52.382361 GoogleBard-1.0.0/src/GoogleBard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-22 12:42:52.000000 GoogleBard-1.0.0/src/GoogleBard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-22 12:42:52.000000 GoogleBard-1.0.0/src/GoogleBard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 12:42:52.000000 GoogleBard-1.0.0/src/GoogleBard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-22 12:42:52.000000 GoogleBard-1.0.0/src/GoogleBard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-22 12:42:52.000000 GoogleBard-1.0.0/src/GoogleBard.egg-info/top_level.txt
```

### Comparing `GoogleBard-0.0.7/LICENSE` & `GoogleBard-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleBard-0.0.7/PKG-INFO` & `GoogleBard-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 0.0.7
+Version: 1.0.0
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
@@ -39,14 +39,33 @@
 usage: Bard.py [-h] --session SESSION
 
 options:
   -h, --help         show this help message and exit
   --session SESSION  __Secure-1PSID cookie.
 ```
 
+### Quick mode
+```
+$ export BARD_QUICK="true"
+$ export BARD_SESSION="<__Secure-1PSID>"
+$ python3 -m Bard
+```
+Environment variables can be placed in .zshrc.
+
+Example bash shortcut:
+```bash
+# USAGE1: bard QUESTION
+# USAGE2: echo "QUESTION" | bard
+bard () {
+	export BARD_QUICK=true
+	export BARD_SESSION=<REDACTED>.
+	python3 -m Bard "${@:-$(</dev/stdin)}" | tail -n+7
+}
+```
+
 ## [Developer Documentation](https://github.com/acheong08/Bard/blob/main/DOCUMENTATION.md)
 ```python
 from os import environ
 from Bard import Chatbot
 
 token = environ.get("BARD_TOKEN")
```

### Comparing `GoogleBard-0.0.7/README.md` & `GoogleBard-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,33 @@
 usage: Bard.py [-h] --session SESSION
 
 options:
   -h, --help         show this help message and exit
   --session SESSION  __Secure-1PSID cookie.
 ```
 
+### Quick mode
+```
+$ export BARD_QUICK="true"
+$ export BARD_SESSION="<__Secure-1PSID>"
+$ python3 -m Bard
+```
+Environment variables can be placed in .zshrc.
+
+Example bash shortcut:
+```bash
+# USAGE1: bard QUESTION
+# USAGE2: echo "QUESTION" | bard
+bard () {
+	export BARD_QUICK=true
+	export BARD_SESSION=<REDACTED>.
+	python3 -m Bard "${@:-$(</dev/stdin)}" | tail -n+7
+}
+```
+
 ## [Developer Documentation](https://github.com/acheong08/Bard/blob/main/DOCUMENTATION.md)
 ```python
 from os import environ
 from Bard import Chatbot
 
 token = environ.get("BARD_TOKEN")
```

### Comparing `GoogleBard-0.0.7/setup.py` & `GoogleBard-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="GoogleBard",
-    version="0.0.7",
+    version="1.0.0",
     license="MIT License",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineering of Google's Bard chatbot",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/Bard",
```

### Comparing `GoogleBard-0.0.7/src/Bard.py` & `GoogleBard-1.0.0/src/Bard.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         """
         Send a message to Google Bard and return the response.
         :param message: The message to send to Google Bard.
         :return: A dict containing the response from Google Bard.
         """
         # url params
         params = {
-            "bl": "boq_assistant-bard-web-server_20230326.21_p0",
+            "bl": "boq_assistant-bard-web-server_20230419.00_p1",
             "_reqid": str(self._reqid),
             "rt": "c",
         }
 
         # message arr -> data["f.req"]. Message is double json stringified
         message_struct = [
             [message],
```

### Comparing `GoogleBard-0.0.7/src/GoogleBard.egg-info/PKG-INFO` & `GoogleBard-1.0.0/src/GoogleBard.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 0.0.7
+Version: 1.0.0
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
@@ -39,14 +39,33 @@
 usage: Bard.py [-h] --session SESSION
 
 options:
   -h, --help         show this help message and exit
   --session SESSION  __Secure-1PSID cookie.
 ```
 
+### Quick mode
+```
+$ export BARD_QUICK="true"
+$ export BARD_SESSION="<__Secure-1PSID>"
+$ python3 -m Bard
+```
+Environment variables can be placed in .zshrc.
+
+Example bash shortcut:
+```bash
+# USAGE1: bard QUESTION
+# USAGE2: echo "QUESTION" | bard
+bard () {
+	export BARD_QUICK=true
+	export BARD_SESSION=<REDACTED>.
+	python3 -m Bard "${@:-$(</dev/stdin)}" | tail -n+7
+}
+```
+
 ## [Developer Documentation](https://github.com/acheong08/Bard/blob/main/DOCUMENTATION.md)
 ```python
 from os import environ
 from Bard import Chatbot
 
 token = environ.get("BARD_TOKEN")
```

