# Comparing `tmp/fints-3.1.0.tar.gz` & `tmp/fints-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fints-3.1.0.tar", last modified: Sun Feb 20 16:59:39 2022, max compression
+gzip compressed data, was "fints-4.0.0.tar", last modified: Sat Apr 22 17:29:57 2023, max compression
```

## Comparing `fints-3.1.0.tar` & `fints-4.0.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-02-20 16:59:39.466698 fints-3.1.0/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     7651 2022-02-19 19:40:20.000000 fints-3.1.0/LICENSE.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       35 2022-02-19 19:40:20.000000 fints-3.1.0/MANIFEST.in
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2292 2022-02-20 16:59:39.466698 fints-3.1.0/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1560 2022-02-20 16:58:25.000000 fints-3.1.0/README.md
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-02-20 16:59:39.466698 fints-3.1.0/fints/
--rw-r--r--   0 raphael   (1000) raphael   (1000)       18 2022-02-20 16:58:54.000000 fints-3.1.0/fints/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    57247 2022-02-20 16:58:25.000000 fints-3.1.0/fints/client.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1345 2022-02-19 19:40:20.000000 fints-3.1.0/fints/connection.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     8834 2022-02-19 19:40:20.000000 fints-3.1.0/fints/dialog.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      645 2022-02-19 19:40:20.000000 fints-3.1.0/fints/exceptions.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     8525 2022-02-19 19:40:20.000000 fints-3.1.0/fints/fields.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    48999 2022-02-19 19:40:20.000000 fints-3.1.0/fints/formals.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-02-20 16:59:39.466698 fints-3.1.0/fints/hhd/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-02-19 19:40:20.000000 fints-3.1.0/fints/hhd/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     8197 2022-02-20 16:58:25.000000 fints-3.1.0/fints/hhd/flicker.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1511 2022-02-19 19:40:20.000000 fints-3.1.0/fints/message.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      321 2022-02-19 19:40:20.000000 fints-3.1.0/fints/models.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    16227 2022-02-20 16:58:25.000000 fints-3.1.0/fints/parser.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     6168 2022-02-19 19:40:20.000000 fints-3.1.0/fints/security.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-02-20 16:59:39.466698 fints-3.1.0/fints/segments/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-02-19 19:40:20.000000 fints-3.1.0/fints/segments/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1148 2022-02-19 19:40:20.000000 fints-3.1.0/fints/segments/accounts.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    13002 2022-02-19 19:40:20.000000 fints-3.1.0/fints/segments/auth.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     4121 2022-02-19 19:40:20.000000 fints-3.1.0/fints/segments/bank.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2650 2022-02-19 19:40:20.000000 fints-3.1.0/fints/segments/base.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    12798 2022-02-19 19:40:20.000000 fints-3.1.0/fints/segments/debit.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1946 2022-02-19 19:40:20.000000 fints-3.1.0/fints/segments/depot.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1488 2022-02-19 19:40:20.000000 fints-3.1.0/fints/segments/dialog.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2673 2022-02-19 19:40:20.000000 fints-3.1.0/fints/segments/journal.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     4263 2022-02-19 19:40:20.000000 fints-3.1.0/fints/segments/message.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     5389 2022-02-19 19:40:20.000000 fints-3.1.0/fints/segments/saldo.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     5937 2022-02-19 19:40:20.000000 fints-3.1.0/fints/segments/statement.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1575 2022-02-19 19:40:20.000000 fints-3.1.0/fints/segments/transfer.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    16804 2022-02-20 16:58:25.000000 fints-3.1.0/fints/types.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    11619 2022-02-19 19:40:20.000000 fints-3.1.0/fints/utils.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-02-20 16:59:39.466698 fints-3.1.0/fints.egg-info/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2292 2022-02-20 16:59:39.000000 fints-3.1.0/fints.egg-info/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1017 2022-02-20 16:59:39.000000 fints-3.1.0/fints.egg-info/SOURCES.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2022-02-20 16:59:39.000000 fints-3.1.0/fints.egg-info/dependency_links.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       36 2022-02-20 16:59:39.000000 fints-3.1.0/fints.egg-info/requires.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)        6 2022-02-20 16:59:39.000000 fints-3.1.0/fints.egg-info/top_level.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)      228 2022-02-20 16:59:39.466698 fints-3.1.0/setup.cfg
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1304 2022-02-19 19:40:20.000000 fints-3.1.0/setup.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-02-20 16:59:39.466698 fints-3.1.0/tests/
--rw-r--r--   0 raphael   (1000) raphael   (1000)    15384 2022-02-19 19:40:20.000000 fints-3.1.0/tests/conftest.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-02-20 16:59:39.466698 fints-3.1.0/tests/messages/
--rw-r--r--   0 raphael   (1000) raphael   (1000)    21319 2022-02-19 19:40:20.000000 fints-3.1.0/tests/messages/basic_complicated.bin
--rw-r--r--   0 raphael   (1000) raphael   (1000)      428 2022-02-19 19:40:20.000000 fints-3.1.0/tests/messages/basic_simple.bin
--rw-r--r--   0 raphael   (1000) raphael   (1000)     6575 2022-02-19 19:40:20.000000 fints-3.1.0/tests/test_client.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     7385 2022-02-19 19:40:20.000000 fints-3.1.0/tests/test_formals.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1653 2022-02-19 19:40:20.000000 fints-3.1.0/tests/test_hhd.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     4220 2022-02-19 19:40:20.000000 fints-3.1.0/tests/test_message_parser.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     7353 2022-02-19 19:40:20.000000 fints-3.1.0/tests/test_message_serializer.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    16141 2022-02-19 19:40:20.000000 fints-3.1.0/tests/test_models.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-22 17:29:57.916319 fints-4.0.0/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     7651 2018-07-23 17:53:05.000000 fints-4.0.0/LICENSE.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       55 2022-06-05 17:43:17.000000 fints-4.0.0/MANIFEST.in
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2411 2023-04-22 17:29:57.916319 fints-4.0.0/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1558 2023-04-22 17:18:37.000000 fints-4.0.0/README.md
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-22 17:29:57.736320 fints-4.0.0/fints/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       18 2023-04-22 17:27:55.000000 fints-4.0.0/fints/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    57737 2023-04-22 17:21:42.000000 fints-4.0.0/fints/client.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1345 2019-09-29 13:30:21.000000 fints-4.0.0/fints/connection.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     8834 2020-01-09 10:01:44.000000 fints-4.0.0/fints/dialog.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      645 2019-12-22 18:20:50.000000 fints-4.0.0/fints/exceptions.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     8525 2019-09-29 13:30:21.000000 fints-4.0.0/fints/fields.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    48999 2019-09-29 13:30:21.000000 fints-4.0.0/fints/formals.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-22 17:29:57.899653 fints-4.0.0/fints/hhd/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2018-07-26 20:30:22.000000 fints-4.0.0/fints/hhd/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     8344 2023-04-22 17:10:25.000000 fints-4.0.0/fints/hhd/flicker.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1511 2019-09-29 13:30:21.000000 fints-4.0.0/fints/message.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      321 2019-09-29 13:30:21.000000 fints-4.0.0/fints/models.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    16227 2022-06-05 17:36:57.000000 fints-4.0.0/fints/parser.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     6168 2019-09-29 13:30:21.000000 fints-4.0.0/fints/security.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-22 17:29:57.906319 fints-4.0.0/fints/segments/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2019-09-29 13:30:21.000000 fints-4.0.0/fints/segments/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1148 2019-09-29 13:30:21.000000 fints-4.0.0/fints/segments/accounts.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    13002 2019-09-29 13:30:21.000000 fints-4.0.0/fints/segments/auth.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     4121 2019-09-29 13:30:21.000000 fints-4.0.0/fints/segments/bank.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2650 2019-09-29 13:30:21.000000 fints-4.0.0/fints/segments/base.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    12798 2019-09-29 13:30:21.000000 fints-4.0.0/fints/segments/debit.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1946 2019-09-29 13:30:21.000000 fints-4.0.0/fints/segments/depot.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1488 2019-09-29 13:30:21.000000 fints-4.0.0/fints/segments/dialog.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2673 2019-09-29 13:30:21.000000 fints-4.0.0/fints/segments/journal.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     4263 2019-09-29 13:30:21.000000 fints-4.0.0/fints/segments/message.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5389 2019-09-29 13:30:21.000000 fints-4.0.0/fints/segments/saldo.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5937 2019-09-29 13:30:21.000000 fints-4.0.0/fints/segments/statement.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     4062 2023-04-22 17:10:26.000000 fints-4.0.0/fints/segments/transfer.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    16804 2022-06-05 17:36:57.000000 fints-4.0.0/fints/types.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    11619 2022-06-05 17:49:09.000000 fints-4.0.0/fints/utils.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-22 17:29:57.896319 fints-4.0.0/fints.egg-info/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2411 2023-04-22 17:29:57.000000 fints-4.0.0/fints.egg-info/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1017 2023-04-22 17:29:57.000000 fints-4.0.0/fints.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2023-04-22 17:29:57.000000 fints-4.0.0/fints.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       36 2023-04-22 17:29:57.000000 fints-4.0.0/fints.egg-info/requires.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        6 2023-04-22 17:29:57.000000 fints-4.0.0/fints.egg-info/top_level.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      228 2023-04-22 17:29:57.916319 fints-4.0.0/setup.cfg
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1454 2023-04-22 17:29:40.000000 fints-4.0.0/setup.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-22 17:29:57.912986 fints-4.0.0/tests/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    15384 2019-12-22 18:20:50.000000 fints-4.0.0/tests/conftest.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-22 17:29:57.916319 fints-4.0.0/tests/messages/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    21319 2019-09-29 13:30:21.000000 fints-4.0.0/tests/messages/basic_complicated.bin
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      428 2019-09-29 13:30:21.000000 fints-4.0.0/tests/messages/basic_simple.bin
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     6575 2019-12-22 18:20:50.000000 fints-4.0.0/tests/test_client.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     7385 2019-09-29 13:30:21.000000 fints-4.0.0/tests/test_formals.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1653 2019-09-29 13:30:21.000000 fints-4.0.0/tests/test_hhd.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     4220 2019-12-22 18:20:50.000000 fints-4.0.0/tests/test_message_parser.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     7353 2019-09-29 13:30:21.000000 fints-4.0.0/tests/test_message_serializer.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    16141 2019-09-29 13:30:21.000000 fints-4.0.0/tests/test_models.py
```

### Comparing `fints-3.1.0/LICENSE.txt` & `fints-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/PKG-INFO` & `fints-4.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: fints
-Version: 3.1.0
+Version: 4.0.0
 Summary: Pure-python FinTS 3.0 (formerly known as HBCI) implementation
 Home-page: https://github.com/raphaelm/python-fints
 Author: Raphael Michel
 Author-email: mail@raphaelmichel.de
 License: GNU Lesser General Public License v3 (LGPLv3)
 Keywords: hbci banking fints
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 PyFinTS
 =======
 
 This is a pure-python implementation of FinTS (formerly known as HBCI), a
 online-banking protocol commonly supported by German banks.
 
-
 [Read our documentation for more info](https://python-fints.readthedocs.io)
 
 Maintenance Status 
 ------------------
 
-This project is maintained, but with limited capacity. Working on this is takes a lot of time and testing since all banks do things differently and once you move a part here, you break an unexpected one over there. Therefore: Bugs will only be fixed by me if they occur with a bank where I have an account. New features will only be developed if I need them. PRs will be merged if they either have a very low risk of breaking things elsewhere (e.g. purely adding new commands) or if I can test them. In any case, things might take a little time until I have the bandwidth to focus on them. Sorry about that :( 
+This project is maintained, but with limited capacity. Working on this is takes a lot of time and testing since all banks do things differently and once you move a part here, you break an unexpected one over there. Therefore: Bugs will only be fixed by me if they occur with a bank where I have an account. New features will only be developed if I need them. PRs will be merged if they either have a very low risk of breaking things elsewhere (e.g. purely adding new commands) or if I can test them. In any case, things might take a little time until I have the bandwidth to focus on them. Sorry about that :(
 
 Limitations
 -----------
 
 * Only FinTS 3.0 is supported
 * Only PIN/TAN authentication is supported, no signature cards
 * Only the following operations are supported:
   * Fetching bank statements
   * Fetching balances
   * Fetching holdings
   * SEPA transfers and debits (only with required TAN and with specific TAN methods)
-* Supports Python 3.4+
+* Supports Python 3.6+
 
 Credits and License
 -------------------
 
 This library is maintained by Raphael Michel <mail@raphaelmichel.de>
 and features major contributions by Henryk Plötz.
 
 Further thanks for improving this library go out to:
 Daniel Nowak, Patrick Braune, Mathias Dalheimer, Christopher Grebs, Markus Schindler, and many more.
 
 License: LGPL
-
-
```

### Comparing `fints-3.1.0/README.md` & `fints-4.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 PyFinTS
 =======
 
 This is a pure-python implementation of FinTS (formerly known as HBCI), a
 online-banking protocol commonly supported by German banks.
 
-
 [Read our documentation for more info](https://python-fints.readthedocs.io)
 
 Maintenance Status 
 ------------------
 
-This project is maintained, but with limited capacity. Working on this is takes a lot of time and testing since all banks do things differently and once you move a part here, you break an unexpected one over there. Therefore: Bugs will only be fixed by me if they occur with a bank where I have an account. New features will only be developed if I need them. PRs will be merged if they either have a very low risk of breaking things elsewhere (e.g. purely adding new commands) or if I can test them. In any case, things might take a little time until I have the bandwidth to focus on them. Sorry about that :( 
+This project is maintained, but with limited capacity. Working on this is takes a lot of time and testing since all banks do things differently and once you move a part here, you break an unexpected one over there. Therefore: Bugs will only be fixed by me if they occur with a bank where I have an account. New features will only be developed if I need them. PRs will be merged if they either have a very low risk of breaking things elsewhere (e.g. purely adding new commands) or if I can test them. In any case, things might take a little time until I have the bandwidth to focus on them. Sorry about that :(
 
 Limitations
 -----------
 
 * Only FinTS 3.0 is supported
 * Only PIN/TAN authentication is supported, no signature cards
 * Only the following operations are supported:
   * Fetching bank statements
   * Fetching balances
   * Fetching holdings
   * SEPA transfers and debits (only with required TAN and with specific TAN methods)
-* Supports Python 3.4+
+* Supports Python 3.6+
 
 Credits and License
 -------------------
 
 This library is maintained by Raphael Michel <mail@raphaelmichel.de>
 and features major contributions by Henryk Plötz.
```

### Comparing `fints-3.1.0/fints/client.py` & `fints-4.0.0/fints/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     HKDSC1, HKDSE1, HKDSE2, DebitResponseBase,
 )
 from .segments.depot import HKWPD5, HKWPD6
 from .segments.dialog import HIRMG2, HIRMS2, HISYN4, HKSYN3
 from .segments.journal import HKPRO3, HKPRO4
 from .segments.saldo import HKSAL5, HKSAL6, HKSAL7
 from .segments.statement import DKKKU2, HKKAZ5, HKKAZ6, HKKAZ7, HKCAZ1
-from .segments.transfer import HKCCM1, HKCCS1
+from .segments.transfer import HKCCM1, HKCCS1, HKIPZ1, HKIPM1
 from .types import SegmentSequence
 from .utils import (
     MT535_Miniparser, Password, SubclassesMixin,
     compress_datablob, decompress_datablob, mt940_to_array,
 )
 
 logger = logging.getLogger(__name__)
@@ -167,16 +167,16 @@
             self.bank_identifier = bank_identifier
         elif isinstance(bank_identifier, str):
             self.bank_identifier = BankIdentifier(BankIdentifier.COUNTRY_ALPHA_TO_NUMERIC['DE'], bank_identifier)
         else:
             raise TypeError("bank_identifier must be BankIdentifier or str (BLZ)")
         self.system_id = SYSTEM_ID_UNASSIGNED
         if not product_id:
-            logger.warning('You should register your program with the ZKA and pass your own product_id as a parameter.')
-            product_id = 'DC333D745719C4BD6A6F9DB6A'
+            raise TypeError("The product_id keyword argument is mandatory starting with python-fints version 4. See "
+                            "https://python-fints.readthedocs.io/en/latest/upgrading_3_4.html for more information.")
 
         self.user_id = user_id
         self.customer_id = customer_id or user_id
         self.bpd_version = 0
         self.bpa = None
         self.bpd = SegmentSequence()
         self.upd_version = 0
@@ -740,26 +740,27 @@
             if "urn:iso:std:iso:20022:tech:xsd:{}.xsd".format(candidate) in bank_supported:
                 return candidate
 
         logger.warning("No common supported SEPA version. Defaulting to first candidate and hoping for the best: %s.", candidate_versions[0])
         return candidate_versions[0]
 
     def simple_sepa_transfer(self, account: SEPAAccount, iban: str, bic: str,
-                             recipient_name: str, amount: Decimal, account_name: str, reason: str,
+                             recipient_name: str, amount: Decimal, account_name: str, reason: str, instant_payment=False,
                              endtoend_id='NOTPROVIDED'):
         """
         Simple SEPA transfer.
 
         :param account: SEPAAccount to start the transfer from.
         :param iban: Recipient's IBAN
         :param bic: Recipient's BIC
         :param recipient_name: Recipient name
         :param amount: Amount as a ``Decimal``
         :param account_name: Sender account name
         :param reason: Transfer reason
+        :param instant_payment: Whether to use instant payment (defaults to ``False``)
         :param endtoend_id: End-to-end-Id (defaults to ``NOTPROVIDED``)
         :return: Returns either a NeedRetryResponse or TransactionResponse
         """
         config = {
             "name": account_name,
             "IBAN": account.iban,
             "BIC": account.bic,
@@ -775,49 +776,53 @@
             "amount": round(Decimal(amount) * 100),  # in cents
             "execution_date": datetime.date(1999, 1, 1),
             "description": reason,
             "endtoend_id": endtoend_id,
         }
         sepa.add_payment(payment)
         xml = sepa.export().decode()
-        return self.sepa_transfer(account, xml, pain_descriptor="urn:iso:std:iso:20022:tech:xsd:"+version)
+        return self.sepa_transfer(account, xml, pain_descriptor="urn:iso:std:iso:20022:tech:xsd:"+version, instant_payment=instant_payment)
 
     def sepa_transfer(self, account: SEPAAccount, pain_message: str, multiple=False,
                       control_sum=None, currency='EUR', book_as_single=False,
-                      pain_descriptor='urn:iso:std:iso:20022:tech:xsd:pain.001.001.03'):
+                      pain_descriptor='urn:iso:std:iso:20022:tech:xsd:pain.001.001.03', instant_payment=False):
         """
         Custom SEPA transfer.
 
         :param account: SEPAAccount to send the transfer from.
         :param pain_message: SEPA PAIN message containing the transfer details.
         :param multiple: Whether this message contains multiple transfers.
         :param control_sum: Sum of all transfers (required if there are multiple)
         :param currency: Transfer currency
         :param book_as_single: Kindly ask the bank to put multiple transactions as separate lines on the bank statement (defaults to ``False``)
         :param pain_descriptor: URN of the PAIN message schema used.
+        :param instant_payment: Whether this is an instant transfer (defaults to ``False``)
         :return: Returns either a NeedRetryResponse or TransactionResponse
         """
 
         with self._get_dialog() as dialog:
             if multiple:
-                command_class = HKCCM1
+                command_class = HKIPM1 if instant_payment else HKCCM1
             else:
-                command_class = HKCCS1
+                command_class = HKIPZ1 if instant_payment else HKCCS1
 
             hiccxs, hkccx = self._find_highest_supported_command(
                 command_class,
                 return_parameter_segment=True
             )
 
             seg = hkccx(
                 account=hkccx._fields['account'].type.from_sepa_account(account),
                 sepa_descriptor=pain_descriptor,
                 sepa_pain_message=pain_message.encode(),
             )
 
+            # if instant_payment:
+            #     seg.allow_convert_sepa_transfer = True
+
             if multiple:
                 if hiccxs.parameter.sum_amount_required and control_sum is None:
                     raise ValueError("Control sum required.")
                 if book_as_single and not hiccxs.parameter.single_booking_allowed:
                     raise FinTSUnsupportedOperation("Single booking not allowed by bank.")
 
                 if control_sum:
```

### Comparing `fints-3.1.0/fints/connection.py` & `fints-4.0.0/fints/connection.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/dialog.py` & `fints-4.0.0/fints/dialog.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/exceptions.py` & `fints-4.0.0/fints/exceptions.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/fields.py` & `fints-4.0.0/fints/fields.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/formals.py` & `fints-4.0.0/fints/formals.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/hhd/flicker.py` & `fints-4.0.0/fints/hhd/flicker.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,39 +230,44 @@
     def render_length(self):
         s = super().render_length()
         if self.version == HHD_VERSION_13 or not self.control_bytes:
             return s
         l = int(s, 16) + (1 << BIT_CONTROLBYTE)
         return h(l, 2)
 
+def code_to_bitstream(code):
+    """Convert a flicker code into a bitstream in strings."""
+    # Inspired by Andreas Schiermeier
+    # https://git.ccc-ffm.de/?p=smartkram.git;a=blob_plain;f=chiptan/flicker/flicker.sh;h
+    # =7066293b4e790c2c4c1f6cbdab703ed9976ffe1f;hb=refs/heads/master
+    code = parse(code).render()
+    data = swap_bytes(code)
+    stream = ['10000', '00000', '11111', '01111', '11111', '01111', '11111']
+    for c in data:
+        v = int(c, 16)
+        stream.append('1' + str(v & 1) + str((v & 2) >> 1) + str((v & 4) >> 2) + str((v & 8) >> 3))
+        stream.append('0' + str(v & 1) + str((v & 2) >> 1) + str((v & 4) >> 2) + str((v & 8) >> 3))
+    return stream
 
 def terminal_flicker_unix(code, field_width=3, space_width=3, height=1, clear=False, wait=0.05):
     """
     Re-encodes a flicker code and prints it on a unix terminal.
 
     :param code: Challenge value
     :param field_width: Width of fields in characters (default: 3).
     :param space_width: Width of spaces in characters (default: 3).
     :param height: Height of fields in characters (default: 1).
     :param clear: Clear terminal after every line (default: ``False``).
     :param wait: Waiting interval between lines (default: 0.05).
     """
-    # Inspired by Andreas Schiermeier
-    # https://git.ccc-ffm.de/?p=smartkram.git;a=blob_plain;f=chiptan/flicker/flicker.sh;h
-    # =7066293b4e790c2c4c1f6cbdab703ed9976ffe1f;hb=refs/heads/master
-    code = parse(code).render()
-    data = swap_bytes(code)
+    stream = code_to_bitstream(code)
+
     high = '\033[48;05;15m'
     low = '\033[48;05;0m'
     std = '\033[0m'
-    stream = ['10000', '00000', '11111', '01111', '11111', '01111', '11111']
-    for c in data:
-        v = int(c, 16)
-        stream.append('1' + str(v & 1) + str((v & 2) >> 1) + str((v & 4) >> 2) + str((v & 8) >> 3))
-        stream.append('0' + str(v & 1) + str((v & 2) >> 1) + str((v & 4) >> 2) + str((v & 8) >> 3))
 
     while True:
         for frame in stream:
             if clear:
                 print('\033c', end='')
 
             for i in range(height):
```

### Comparing `fints-3.1.0/fints/message.py` & `fints-4.0.0/fints/message.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/parser.py` & `fints-4.0.0/fints/parser.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/security.py` & `fints-4.0.0/fints/security.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/segments/accounts.py` & `fints-4.0.0/fints/segments/accounts.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/segments/auth.py` & `fints-4.0.0/fints/segments/auth.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/segments/bank.py` & `fints-4.0.0/fints/segments/bank.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/segments/base.py` & `fints-4.0.0/fints/segments/base.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/segments/debit.py` & `fints-4.0.0/fints/segments/debit.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/segments/depot.py` & `fints-4.0.0/fints/segments/depot.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/segments/dialog.py` & `fints-4.0.0/fints/segments/dialog.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/segments/journal.py` & `fints-4.0.0/fints/segments/journal.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/segments/message.py` & `fints-4.0.0/fints/segments/message.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/segments/saldo.py` & `fints-4.0.0/fints/segments/saldo.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/segments/statement.py` & `fints-4.0.0/fints/segments/statement.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/types.py` & `fints-4.0.0/fints/types.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints/utils.py` & `fints-4.0.0/fints/utils.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/fints.egg-info/PKG-INFO` & `fints-4.0.0/fints.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: fints
-Version: 3.1.0
+Version: 4.0.0
 Summary: Pure-python FinTS 3.0 (formerly known as HBCI) implementation
 Home-page: https://github.com/raphaelm/python-fints
 Author: Raphael Michel
 Author-email: mail@raphaelmichel.de
 License: GNU Lesser General Public License v3 (LGPLv3)
 Keywords: hbci banking fints
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 PyFinTS
 =======
 
 This is a pure-python implementation of FinTS (formerly known as HBCI), a
 online-banking protocol commonly supported by German banks.
 
-
 [Read our documentation for more info](https://python-fints.readthedocs.io)
 
 Maintenance Status 
 ------------------
 
-This project is maintained, but with limited capacity. Working on this is takes a lot of time and testing since all banks do things differently and once you move a part here, you break an unexpected one over there. Therefore: Bugs will only be fixed by me if they occur with a bank where I have an account. New features will only be developed if I need them. PRs will be merged if they either have a very low risk of breaking things elsewhere (e.g. purely adding new commands) or if I can test them. In any case, things might take a little time until I have the bandwidth to focus on them. Sorry about that :( 
+This project is maintained, but with limited capacity. Working on this is takes a lot of time and testing since all banks do things differently and once you move a part here, you break an unexpected one over there. Therefore: Bugs will only be fixed by me if they occur with a bank where I have an account. New features will only be developed if I need them. PRs will be merged if they either have a very low risk of breaking things elsewhere (e.g. purely adding new commands) or if I can test them. In any case, things might take a little time until I have the bandwidth to focus on them. Sorry about that :(
 
 Limitations
 -----------
 
 * Only FinTS 3.0 is supported
 * Only PIN/TAN authentication is supported, no signature cards
 * Only the following operations are supported:
   * Fetching bank statements
   * Fetching balances
   * Fetching holdings
   * SEPA transfers and debits (only with required TAN and with specific TAN methods)
-* Supports Python 3.4+
+* Supports Python 3.6+
 
 Credits and License
 -------------------
 
 This library is maintained by Raphael Michel <mail@raphaelmichel.de>
 and features major contributions by Henryk Plötz.
 
 Further thanks for improving this library go out to:
 Daniel Nowak, Patrick Braune, Mathias Dalheimer, Christopher Grebs, Markus Schindler, and many more.
 
 License: LGPL
-
-
```

### Comparing `fints-3.1.0/fints.egg-info/SOURCES.txt` & `fints-4.0.0/fints.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/setup.py` & `fints-4.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,26 +14,29 @@
     long_description = ''
 
 setup(
     name='fints',
     version=version,
     description='Pure-python FinTS 3.0 (formerly known as HBCI) implementation',
     long_description=long_description,
+    long_description_content_type='text/markdown',
     url='https://github.com/raphaelm/python-fints',
     author='Raphael Michel',
     author_email='mail@raphaelmichel.de',
     license='GNU Lesser General Public License v3 (LGPLv3)',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Other Audience',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
 
     keywords='hbci banking fints',
     install_requires=[
         'bleach',
         'mt-940',
         'requests',
```

### Comparing `fints-3.1.0/tests/conftest.py` & `fints-4.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/tests/messages/basic_complicated.bin` & `fints-4.0.0/tests/messages/basic_complicated.bin`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/tests/test_client.py` & `fints-4.0.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/tests/test_formals.py` & `fints-4.0.0/tests/test_formals.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/tests/test_hhd.py` & `fints-4.0.0/tests/test_hhd.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/tests/test_message_parser.py` & `fints-4.0.0/tests/test_message_parser.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/tests/test_message_serializer.py` & `fints-4.0.0/tests/test_message_serializer.py`

 * *Files identical despite different names*

### Comparing `fints-3.1.0/tests/test_models.py` & `fints-4.0.0/tests/test_models.py`

 * *Files identical despite different names*

