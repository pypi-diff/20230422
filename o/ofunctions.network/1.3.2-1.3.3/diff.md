# Comparing `tmp/ofunctions.network-1.3.2.tar.gz` & `tmp/ofunctions.network-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofunctions.network-1.3.2.tar", last modified: Sun Nov  6 21:02:00 2022, max compression
+gzip compressed data, was "ofunctions.network-1.3.3.tar", last modified: Sat Apr 22 21:41:09 2023, max compression
```

## Comparing `ofunctions.network-1.3.2.tar` & `ofunctions.network-1.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-11-06 21:02:00.192221 ofunctions.network-1.3.2/
--rw-rw-rw-   0        0        0     1590 2021-12-22 10:52:43.000000 ofunctions.network-1.3.2/LICENSE
--rw-rw-rw-   0        0        0    12013 2022-11-06 21:02:00.192221 ofunctions.network-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    10702 2022-11-06 20:27:56.000000 ofunctions.network-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2022-11-06 21:02:00.176597 ofunctions.network-1.3.2/ofunctions/
-drwxrwxrwx   0        0        0        0 2022-11-06 21:02:00.192221 ofunctions.network-1.3.2/ofunctions/network/
--rw-rw-rw-   0        0        0    22685 2022-11-06 20:18:12.000000 ofunctions.network-1.3.2/ofunctions/network/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-06 21:02:00.192221 ofunctions.network-1.3.2/ofunctions.network.egg-info/
--rw-rw-rw-   0        0        0    12013 2022-11-06 21:02:00.000000 ofunctions.network-1.3.2/ofunctions.network.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2022-11-06 21:02:00.000000 ofunctions.network-1.3.2/ofunctions.network.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-06 21:02:00.000000 ofunctions.network-1.3.2/ofunctions.network.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-11-06 21:02:00.000000 ofunctions.network-1.3.2/ofunctions.network.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0        2 2022-07-10 12:31:30.000000 ofunctions.network-1.3.2/ofunctions.network.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      133 2022-11-06 21:02:00.000000 ofunctions.network-1.3.2/ofunctions.network.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-11-06 21:02:00.000000 ofunctions.network-1.3.2/ofunctions.network.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-06 21:02:00.192221 ofunctions.network-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     7592 2021-12-22 10:52:43.000000 ofunctions.network-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 21:41:09.277978 ofunctions.network-1.3.3/
+-rw-rw-rw-   0        0        0     1590 2023-01-22 21:50:29.000000 ofunctions.network-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0    14586 2023-04-22 21:41:09.276978 ofunctions.network-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    13275 2023-01-09 18:22:02.000000 ofunctions.network-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 21:41:09.259976 ofunctions.network-1.3.3/ofunctions/
+drwxrwxrwx   0        0        0        0 2023-04-22 21:41:09.274978 ofunctions.network-1.3.3/ofunctions/network/
+-rw-rw-rw-   0        0        0    22683 2023-04-22 21:39:53.000000 ofunctions.network-1.3.3/ofunctions/network/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 21:41:09.273978 ofunctions.network-1.3.3/ofunctions.network.egg-info/
+-rw-rw-rw-   0        0        0    14586 2023-04-22 21:41:09.000000 ofunctions.network-1.3.3/ofunctions.network.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-04-22 21:41:09.000000 ofunctions.network-1.3.3/ofunctions.network.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 21:41:09.000000 ofunctions.network-1.3.3/ofunctions.network.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-22 21:41:09.000000 ofunctions.network-1.3.3/ofunctions.network.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0        2 2022-07-10 12:31:30.000000 ofunctions.network-1.3.3/ofunctions.network.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      156 2023-04-22 21:41:09.000000 ofunctions.network-1.3.3/ofunctions.network.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-22 21:41:09.000000 ofunctions.network-1.3.3/ofunctions.network.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 21:41:09.277978 ofunctions.network-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     7592 2021-12-22 10:52:43.000000 ofunctions.network-1.3.3/setup.py
```

### Comparing `ofunctions.network-1.3.2/LICENSE` & `ofunctions.network-1.3.3/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2015-2021, netinvent, Orsiris de Jong, contact@netinvent.fr
+Copyright (c) 2015-2023, netinvent, Orsiris de Jong, contact@netinvent.fr
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `ofunctions.network-1.3.2/PKG-INFO` & `ofunctions.network-1.3.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: ofunctions.network
-Version: 1.3.2
-Summary: Network diagnostics, MTU probing, Public IP discovery, HTTP/HTTPS internet connectivty tests, ping, name resolution...
-Home-page: https://github.com/netinvent/ofunctions
-Author: NetInvent - Orsiris de Jong
-Author-email: contact@netinvent.fr
-Keywords: network,bisection,logging
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: Topic :: System
-Classifier: Topic :: System :: Operating System
-Classifier: Topic :: System :: Shells
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: POSIX :: BSD :: FreeBSD
-Classifier: Operating System :: POSIX :: BSD :: NetBSD
-Classifier: Operating System :: POSIX :: BSD :: OpenBSD
-Classifier: Operating System :: Microsoft
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ofunctions
 ## Collection of useful python functions
 
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/netinvent/ofunctions.svg)](http://isitmaintained.com/project/netinvent/ofunctions "Percentage of issues still open")
 [![Maintainability](https://api.codeclimate.com/v1/badges/d82ea82db47d8a91c5b6/maintainability)](https://codeclimate.com/github/netinvent/ofunctions/maintainability)
 [![codecov](https://codecov.io/gh/netinvent/ofunctions/branch/master/graph/badge.svg?token=WKQQHGHTO8)](https://codecov.io/gh/netinvent/ofunctions)
@@ -148,14 +119,41 @@
 my_json = {'some.name': 'some\tvalue'}
 my_santized_json = json_sanitize(my_json)
 ```
 my_santized_json will contain `{'somename': 'somevalue'}`
 
 ## logger_utils Usage
 
+ofunctions.logger_utils is an easy implementation of logger which promises to always work, regardless of encoding issues.
+Easy usage:
+```
+from ofunctions.logger_utils import logger_get_logger
+
+logger = logger_get_logger(log_file='/path/to/log/file')
+```
+
+logger_utils will automatically try to open a temp log file if given log_file is not writable.
+You can also disable console output with `console=False`, enable debug_mode with `debug=True` (or later with `logger.setLevel(logging.DEBUG)`).
+Also allows to inject more LOGGER formatter objects, eg:
+```
+logger = logger_get_logger(formatter_insert="%(processName)s")
+```
+
+logger_utils also allows to know what was the worst loglevel that has been called in your program:
+
+```
+from ofunctions.logger_utils import logger_get_logger, get_worst_logger_level
+
+logger = logger_get_logger()
+logger.error("Oh no !")
+
+print("worst log level was :", get_worst_logger_level())  # 10-50, 10 = debug, 50 = critical
+```
+
+
 ## mailer Usage
 
 ofunctions.mailer is a simple mailing class and a rfc822 email validation function.
 
 Setup:
 ```
 pip install ofunctions.mailer
@@ -197,14 +195,59 @@
 mailer = Mailer()  # Uses localhost:25
 
 # attachment can be a binary blob or a file path
 # filename is optional, and will rename a binary blob to something more meaningful
 mailer.send_email(subject='test', sender_mail='me@example.com', recipient_mails='them@example.com', body='some body just told me', attachment=attachment, filename='My Attachment File.txt')
 ```
 
+## misc Usage
+
+Misc is a collection of somehow useful functions.
+
+Example: BytesConverter
+
+BytesConverter is that little tool that you want when handling bits and byte units.
+Internally, BytesConverter always represents data an int number of bytes.
+BytesConverter will return a float or a str if human output is requested.
+
+Example (output is shown as comment):
+
+```
+from ofunctions.misc import BytesConverter
+
+print(BytesConverter("64 KB"))  # 64000.0
+print(BytesConverter("64 KiB")) # 65536.0
+print(BytesConverter("64 Kb"))  # 8000.0
+print(BytesConverter("64 KiB")) # 65536.0
+
+value = BytesConverter("20MB")
+print(value.human)              # 20.0 MB
+print(value.human_iec_bytes)    # 19.1 MiB
+print(value.human_bits)         # 160.0 Mb
+print(value.human_iec_bits)     # 152.6 Mib
+
+print(BytesConverter(1234))                 # 1234.0
+print(BytesConverter(1234).bits)            # 9872.0
+print(BytesConverter(1234).kbytes)          # 1.2
+print(BytesConverter(1234).human)           # 1.2 KB
+
+print(BytesConverter(65535).kbytes)         # 64.0
+print(BytesConverter(9000000).mbytes)       # 8.6
+print(BytesConverter("4MB"))                # 4000000.0
+print(BytesConverter("4MiB"))               # 4194304.0
+print(BytesConverter("9600 Kb").mbytes)     # 1.1
+```
+
+Arithmetics:
+BytesConverter objects can be added just as other mathematic types:
+```
+print(BytesConverter("50 MB") + BytesConverter("8192 Kb"))                          # 51024000.0
+print(BytesConverter(BytesConverter("50 MB") + BytesConverter("8192 Kb")).human)    # 51.0 MB
+```
+
 ## network Usage
 
 ofunctions.network is a collection of various tools making network diag / mapping easier.
 
 Setup:
 ```commandline
 pip install ofunctions.network
```

### Comparing `ofunctions.network-1.3.2/ofunctions/network/__init__.py` & `ofunctions.network-1.3.3/ofunctions/network/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 """
 
 __intname__ = "ofunctions.network"
 __author__ = "Orsiris de Jong"
 __copyright__ = "Copyright (C) 2014-2022 Orsiris de Jong"
 __description__ = "Network diagnostics, MTU probing, Public IP discovery, HTTP/HTTPS internet connectivty tests, ping, name resolution..."
 __licence__ = "BSD 3 Clause"
-__version__ = "1.3.2"
-__build__ = "2022110601"
+__version__ = "1.3.3"
+__build__ = "2023042201"
 __compat__ = "python2.7+"
 
 import logging
 import os
 import socket
 import warnings
 from ipaddress import IPv4Address, IPv6Address, AddressValueError
@@ -308,15 +308,14 @@
         else:
             if all_targets_must_succeed:
                 ip_success = False
                 break
 
     # Only ip servers succeed, but not fqdn servers
     if (not (fqdn_servers and fqdn_success)) and ip_success:
-
         # Don't bother with diag message when multiple fqdn_servers exist and all_targets_must_succeed is enabled
         if not all_targets_must_succeed or (
             all_targets_must_succeed and len(fqdn_servers) == 1
         ):
             diag_messages = (
                 diag_messages
                 + "\nNo FQDN server test worked, but at least one IP server test worked. "
```

### Comparing `ofunctions.network-1.3.2/ofunctions.network.egg-info/PKG-INFO` & `ofunctions.network-1.3.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofunctions.network
-Version: 1.3.2
+Version: 1.3.3
 Summary: Network diagnostics, MTU probing, Public IP discovery, HTTP/HTTPS internet connectivty tests, ping, name resolution...
 Home-page: https://github.com/netinvent/ofunctions
 Author: NetInvent - Orsiris de Jong
 Author-email: contact@netinvent.fr
 Keywords: network,bisection,logging
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -148,14 +148,41 @@
 my_json = {'some.name': 'some\tvalue'}
 my_santized_json = json_sanitize(my_json)
 ```
 my_santized_json will contain `{'somename': 'somevalue'}`
 
 ## logger_utils Usage
 
+ofunctions.logger_utils is an easy implementation of logger which promises to always work, regardless of encoding issues.
+Easy usage:
+```
+from ofunctions.logger_utils import logger_get_logger
+
+logger = logger_get_logger(log_file='/path/to/log/file')
+```
+
+logger_utils will automatically try to open a temp log file if given log_file is not writable.
+You can also disable console output with `console=False`, enable debug_mode with `debug=True` (or later with `logger.setLevel(logging.DEBUG)`).
+Also allows to inject more LOGGER formatter objects, eg:
+```
+logger = logger_get_logger(formatter_insert="%(processName)s")
+```
+
+logger_utils also allows to know what was the worst loglevel that has been called in your program:
+
+```
+from ofunctions.logger_utils import logger_get_logger, get_worst_logger_level
+
+logger = logger_get_logger()
+logger.error("Oh no !")
+
+print("worst log level was :", get_worst_logger_level())  # 10-50, 10 = debug, 50 = critical
+```
+
+
 ## mailer Usage
 
 ofunctions.mailer is a simple mailing class and a rfc822 email validation function.
 
 Setup:
 ```
 pip install ofunctions.mailer
@@ -197,14 +224,59 @@
 mailer = Mailer()  # Uses localhost:25
 
 # attachment can be a binary blob or a file path
 # filename is optional, and will rename a binary blob to something more meaningful
 mailer.send_email(subject='test', sender_mail='me@example.com', recipient_mails='them@example.com', body='some body just told me', attachment=attachment, filename='My Attachment File.txt')
 ```
 
+## misc Usage
+
+Misc is a collection of somehow useful functions.
+
+Example: BytesConverter
+
+BytesConverter is that little tool that you want when handling bits and byte units.
+Internally, BytesConverter always represents data an int number of bytes.
+BytesConverter will return a float or a str if human output is requested.
+
+Example (output is shown as comment):
+
+```
+from ofunctions.misc import BytesConverter
+
+print(BytesConverter("64 KB"))  # 64000.0
+print(BytesConverter("64 KiB")) # 65536.0
+print(BytesConverter("64 Kb"))  # 8000.0
+print(BytesConverter("64 KiB")) # 65536.0
+
+value = BytesConverter("20MB")
+print(value.human)              # 20.0 MB
+print(value.human_iec_bytes)    # 19.1 MiB
+print(value.human_bits)         # 160.0 Mb
+print(value.human_iec_bits)     # 152.6 Mib
+
+print(BytesConverter(1234))                 # 1234.0
+print(BytesConverter(1234).bits)            # 9872.0
+print(BytesConverter(1234).kbytes)          # 1.2
+print(BytesConverter(1234).human)           # 1.2 KB
+
+print(BytesConverter(65535).kbytes)         # 64.0
+print(BytesConverter(9000000).mbytes)       # 8.6
+print(BytesConverter("4MB"))                # 4000000.0
+print(BytesConverter("4MiB"))               # 4194304.0
+print(BytesConverter("9600 Kb").mbytes)     # 1.1
+```
+
+Arithmetics:
+BytesConverter objects can be added just as other mathematic types:
+```
+print(BytesConverter("50 MB") + BytesConverter("8192 Kb"))                          # 51024000.0
+print(BytesConverter(BytesConverter("50 MB") + BytesConverter("8192 Kb")).human)    # 51.0 MB
+```
+
 ## network Usage
 
 ofunctions.network is a collection of various tools making network diag / mapping easier.
 
 Setup:
 ```commandline
 pip install ofunctions.network
```

### Comparing `ofunctions.network-1.3.2/setup.py` & `ofunctions.network-1.3.3/setup.py`

 * *Files identical despite different names*

