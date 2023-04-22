# Comparing `tmp/v2conf-0.1.0.tar.gz` & `tmp/v2conf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v2conf-0.1.0.tar", max compression
+gzip compressed data, was "v2conf-0.1.1.tar", max compression
```

## Comparing `v2conf-0.1.0.tar` & `v2conf-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-04-07 15:17:18.364133 v2conf-0.1.0/LICENSE
--rw-r--r--   0        0        0     4809 2023-04-08 12:17:20.508888 v2conf-0.1.0/README.md
--rw-r--r--   0        0        0      827 2023-04-08 12:17:20.508888 v2conf-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      118 2023-04-07 15:17:18.364133 v2conf-0.1.0/v2conf/__init__.py
--rw-r--r--   0        0        0     9908 2023-04-08 12:17:20.508888 v2conf-0.1.0/v2conf/__main__.py
--rw-r--r--   0        0        0     8402 2023-04-07 15:17:18.364133 v2conf-0.1.0/v2conf/configs.py
--rw-r--r--   0        0        0     1470 2023-04-07 15:17:18.364133 v2conf-0.1.0/v2conf/exclude.py
--rw-r--r--   0        0        0     6646 2023-04-08 12:17:20.508888 v2conf-0.1.0/v2conf/health.py
--rw-r--r--   0        0        0     5693 1970-01-01 00:00:00.000000 v2conf-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-07 15:17:18.364133 v2conf-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4922 2023-04-22 13:18:36.905010 v2conf-0.1.1/README.md
+-rw-r--r--   0        0        0      847 2023-04-22 13:17:12.864109 v2conf-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-04-07 15:17:18.364133 v2conf-0.1.1/v2conf/__init__.py
+-rw-r--r--   0        0        0     9908 2023-04-22 13:17:12.844108 v2conf-0.1.1/v2conf/__main__.py
+-rw-r--r--   0        0        0     8654 2023-04-22 13:11:40.808579 v2conf-0.1.1/v2conf/configs.py
+-rw-r--r--   0        0        0     1470 2023-04-07 15:17:18.364133 v2conf-0.1.1/v2conf/exclude.py
+-rw-r--r--   0        0        0     6646 2023-04-08 12:17:20.508888 v2conf-0.1.1/v2conf/health.py
+-rw-r--r--   0        0        0     5847 1970-01-01 00:00:00.000000 v2conf-0.1.1/PKG-INFO
```

### Comparing `v2conf-0.1.0/LICENSE` & `v2conf-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `v2conf-0.1.0/README.md` & `v2conf-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 sudo $(which v2conf) /home/ubuntu/confs -n 10 --no-geoip --country-code 'IR' --jalali --log-file /home/ubuntu/v2conf.log 
 ```
 
 ## Recommended Usage
 ```bash
 sudo $(which v2conf) /home/ubuntu/confs -n 10 -s 900 --timeout-penalty 15 --ema 8,2 --no-geoip --country-code 'IR' --log-level error --jalali -w "https://dl-cdn.alpinelinux.org/alpine/v3.17/releases/x86/alpine-minirootfs-3.17.1-x86.tar.gz" --log-file /home/ubuntu/v2conf.log 
 ```
-With these flags and settings, V2Conf will download the selected file every 15 minutes (900 / 60 = 15) 10 times for every outbound.\
+With these flags and settings, V2Conf will download the selected file every 15 minutes (900 / 60 = 15) 10 times for each outbound.\
 V2Conf will print logs in Jalali date times in `/home/ubuntu/v2conf.log` and `stdout` simultaneously and it will exclude IPs for Iran. (useful for domestic Iranian VPSs) \
 `--timeout-penalty 15` makes the program to consider a failed test as a test with 15 seconds latency and based on exponential moving average of last `8` evaluations (past 2 hours) and weighting more importance on recent evaluations (`2` times for every new evaluation) choose the best outbound and route all data within that.\
 `--log-level error` indicates that **V2Ray** log level will be `error`.
 
 ## Details
 
 V2Conf expects a directory with this structure from you:
@@ -42,14 +42,15 @@
   "port": 6060,
   "protocol": "trojan",
   "settings": {
     "clients":
     ...
 ```
 and **all configs must have a tag!**
+P.S.: Thanks to [Tushar](https://github.com/Mahyar24/V2Conf/pull/2) V2Conf now supports JSON5 format for configs.
 
 
 ## Usage
 ```
 $ v2conf --help
 usage: v2conf [-h] [-c CONFIG_FILE] [--country-code COUNTRY_CODE] [--no-geoip] [-t TIMEOUT] [-w WEBSITE] [-n NUM_OF_TRIES] [--timeout-penalty TIMEOUT_PENALTY] [--ema EMA] [-s SLEEP_TIME]
                    [-l {debug,info,warning,error,none}] [-q | --log-file LOG_FILE] [--jalali] [-v]
```

### Comparing `v2conf-0.1.0/pyproject.toml` & `v2conf-0.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "v2conf"
-version = "0.1.0"
+version = "0.1.1"
 description = "V2Conf helps you build V2Ray Config file automatically and evaluate and change config rules based on outbounds performances."
 authors = ["Mahyar Mahdavi <Mahyar@Mahyar24.com>"]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/mahyar24/V2Conf/"
 repository = "https://github.com/Mahyar24/V2Conf/"
 readme = "README.md"
 keywords = [
@@ -14,14 +14,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.28.1"
 aiohttp = "^3.8.3"
 jdatetime = "^4.1.0"
+json5kit = "^0.3.2"
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.990"
 black = "^22.10.0"
 isort = "^5.10.1"
 pylint = "^2.15.5"
 types-requests = "^2.28.11"
```

### Comparing `v2conf-0.1.0/v2conf/__main__.py` & `v2conf-0.1.1/v2conf/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from time import struct_time
 from typing import Optional
 from zoneinfo import ZoneInfo
 
 from .configs import make_conf, write_conf
 from .health import rank_outbounds
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __author__ = "Mahyar Mahdavi"
 __email__ = "Mahyar@Mahyar24.com"
 __license__ = "GPLv3"
 __url__ = "https://GitHub.com/Mahyar24/V2Conf"
 __pypi__ = "https://PyPI.org/project/V2Conf"
```

### Comparing `v2conf-0.1.0/v2conf/configs.py` & `v2conf-0.1.1/v2conf/configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,38 @@
 
 GitHub: https://github.com/Mahyar24/V2Conf
 Mahyar@Mahyar24.com, Sun Nov 13 2022
 """
 
 
 import argparse
+import io
 import json
 import logging
 import random
 import secrets
 import socket
 from contextlib import closing
 from pathlib import Path
 from typing import Optional, Union
 
+import json5kit
+
 from .exclude import make_ip_rule
 
 
+def read_json5_file(file: io.TextIOWrapper) -> dict:
+    """
+    Reading JSON5 files.
+    """
+    source = file.read()
+    json_source = json5kit.parse(source).to_json()
+    return json.loads(json_source)
+
+
 def find_n_unused_port(num: int) -> list[int]:
     """
     Find n unique unused port and return them as a list.
     """
     ports: set[int] = set()
     while len(ports) < num:
         with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as sock:
@@ -72,15 +84,15 @@
     if not inbounds_path.is_dir():
         raise ValueError("Inbounds directory not found!")
 
     inbounds = {}
     tags = []
     for config in inbounds_path.glob("*.json"):
         with open(config, "r", encoding="utf-8") as file:
-            data = json.load(file)
+            data = read_json5_file(file)
         try:
             inbounds[data["tag"]] = data
         except KeyError as err:
             raise KeyError(f"Tag not found in {config.name!r}") from err
         else:
             if data["tag"].startswith("inbound-http-test-"):
                 raise ValueError(
@@ -110,15 +122,15 @@
         raise ValueError("Outbounds directory not found!")
 
     outbounds = {}
     tags = []
     check_freedom = False
     for config in outbounds_path.glob("*.json"):
         with open(config, "r", encoding="utf-8") as file:
-            data = json.load(file)
+            data = read_json5_file(file)
         try:
             outbounds[data["tag"]] = data
         except KeyError as err:
             raise KeyError(f"Tag not found in {config.name!r}") from err
         else:
             if (tag := data["tag"]) in tags:
                 raise ValueError(
@@ -144,15 +156,15 @@
     if not rules_path.is_dir():
         raise ValueError("Rules directory not found!")
 
     rules = {}
     tags = []
     for config in rules_path.glob("*.json"):
         with open(config, "r", encoding="utf-8") as file:
-            data = json.load(file)
+            data = read_json5_file(file)
         try:
             rules[data["tag"]] = data
         except KeyError as err:
             raise KeyError(f"Tag not found in {config.name!r}") from err
         else:
             if (tag := data["tag"]) in tags:
                 raise ValueError(
```

### Comparing `v2conf-0.1.0/v2conf/exclude.py` & `v2conf-0.1.1/v2conf/exclude.py`

 * *Files identical despite different names*

### Comparing `v2conf-0.1.0/v2conf/health.py` & `v2conf-0.1.1/v2conf/health.py`

 * *Files identical despite different names*

### Comparing `v2conf-0.1.0/PKG-INFO` & `v2conf-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: v2conf
-Version: 0.1.0
+Version: 0.1.1
 Summary: V2Conf helps you build V2Ray Config file automatically and evaluate and change config rules based on outbounds performances.
 Home-page: https://github.com/mahyar24/V2Conf/
 License: GPL-3.0-or-later
 Keywords: V2Ray,V2Fly,X2Ray
 Author: Mahyar Mahdavi
 Author-email: Mahyar@Mahyar24.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: jdatetime (>=4.1.0,<5.0.0)
+Requires-Dist: json5kit (>=0.3.2,<0.4.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://github.com/Mahyar24/V2Conf/
 Description-Content-Type: text/markdown
 
 # V2Conf
 
 V2Conf helps you build V2Ray Config file automatically and evaluate and change config rules based on outbounds performances.
@@ -29,15 +30,15 @@
 sudo $(which v2conf) /home/ubuntu/confs -n 10 --no-geoip --country-code 'IR' --jalali --log-file /home/ubuntu/v2conf.log 
 ```
 
 ## Recommended Usage
 ```bash
 sudo $(which v2conf) /home/ubuntu/confs -n 10 -s 900 --timeout-penalty 15 --ema 8,2 --no-geoip --country-code 'IR' --log-level error --jalali -w "https://dl-cdn.alpinelinux.org/alpine/v3.17/releases/x86/alpine-minirootfs-3.17.1-x86.tar.gz" --log-file /home/ubuntu/v2conf.log 
 ```
-With these flags and settings, V2Conf will download the selected file every 15 minutes (900 / 60 = 15) 10 times for every outbound.\
+With these flags and settings, V2Conf will download the selected file every 15 minutes (900 / 60 = 15) 10 times for each outbound.\
 V2Conf will print logs in Jalali date times in `/home/ubuntu/v2conf.log` and `stdout` simultaneously and it will exclude IPs for Iran. (useful for domestic Iranian VPSs) \
 `--timeout-penalty 15` makes the program to consider a failed test as a test with 15 seconds latency and based on exponential moving average of last `8` evaluations (past 2 hours) and weighting more importance on recent evaluations (`2` times for every new evaluation) choose the best outbound and route all data within that.\
 `--log-level error` indicates that **V2Ray** log level will be `error`.
 
 ## Details
 
 V2Conf expects a directory with this structure from you:
@@ -63,14 +64,15 @@
   "port": 6060,
   "protocol": "trojan",
   "settings": {
     "clients":
     ...
 ```
 and **all configs must have a tag!**
+P.S.: Thanks to [Tushar](https://github.com/Mahyar24/V2Conf/pull/2) V2Conf now supports JSON5 format for configs.
 
 
 ## Usage
 ```
 $ v2conf --help
 usage: v2conf [-h] [-c CONFIG_FILE] [--country-code COUNTRY_CODE] [--no-geoip] [-t TIMEOUT] [-w WEBSITE] [-n NUM_OF_TRIES] [--timeout-penalty TIMEOUT_PENALTY] [--ema EMA] [-s SLEEP_TIME]
                    [-l {debug,info,warning,error,none}] [-q | --log-file LOG_FILE] [--jalali] [-v]
```

