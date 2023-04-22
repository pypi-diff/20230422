# Comparing `tmp/dphelper-0.0.3.tar.gz` & `tmp/dphelper-0.0.5.tar.gz`

## Comparing `dphelper-0.0.3.tar` & `dphelper-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,14 @@
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 dphelper-0.0.3/steps.txt
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 dphelper-0.0.3/src/dphelper/__init__.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 dphelper-0.0.3/src/dphelper/config.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 dphelper-0.0.3/src/dphelper/helper.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 dphelper-0.0.3/src/dphelper/package_consts.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 dphelper-0.0.3/src/dphelper/schemas.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 dphelper-0.0.3/src/dphelper/connection/__init__.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 dphelper-0.0.3/src/dphelper/connection/error.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 dphelper-0.0.3/src/dphelper/connection/fetch.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 dphelper-0.0.3/src/dphelper/connection/headers.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 dphelper-0.0.3/src/dphelper/connection/repeated_call.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 dphelper-0.0.3/src/dphelper/snapshot/__init__.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 dphelper-0.0.3/src/dphelper/snapshot/snapshot.py
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 dphelper-0.0.3/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dphelper-0.0.3/license
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 dphelper-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 dphelper-0.0.3/readme.md
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 dphelper-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 dphelper-0.0.5/steps.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dphelper-0.0.5/src/dphelper/__init__.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 dphelper-0.0.5/src/dphelper/config.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 dphelper-0.0.5/src/dphelper/helper.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 dphelper-0.0.5/src/dphelper/schemas.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 dphelper-0.0.5/src/dphelper/connection/__init__.py
+-rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 dphelper-0.0.5/src/dphelper/connection/fetch.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dphelper-0.0.5/src/dphelper/snapshot/__init__.py
+-rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 dphelper-0.0.5/src/dphelper/snapshot/snapshot.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 dphelper-0.0.5/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dphelper-0.0.5/license
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 dphelper-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 dphelper-0.0.5/readme.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 dphelper-0.0.5/PKG-INFO
```

### Comparing `dphelper-0.0.3/src/dphelper/schemas.py` & `dphelper-0.0.5/src/dphelper/schemas.py`

 * *Files identical despite different names*

### Comparing `dphelper-0.0.3/.gitignore` & `dphelper-0.0.5/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -160,8 +160,8 @@
 #.idea/
 # git ignore source file : https://github.com/github/gitignore/blob/main/Python.gitignore. license cc0
 sql_app.db
 sql_app.db-journal
 test_db.db
 test_db.db-journal
 test*.db
-debug.py
+debug*.py
```

