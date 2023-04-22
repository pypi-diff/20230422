# Comparing `tmp/transaction-accounts-0.0.1.tar.gz` & `tmp/transaction-accounts-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transaction-accounts-0.0.1.tar", last modified: Sat Apr 22 06:07:38 2023, max compression
+gzip compressed data, was "transaction-accounts-0.0.2.tar", last modified: Sat Apr 22 06:29:39 2023, max compression
```

## Comparing `transaction-accounts-0.0.1.tar` & `transaction-accounts-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 06:07:38.895680 transaction-accounts-0.0.1/
--rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.0.1/LICENSE.txt
--rw-r--r--   0 igormusic   (501) staff       (20)      746 2023-04-22 06:07:38.895825 transaction-accounts-0.0.1/PKG-INFO
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 06:07:38.893223 transaction-accounts-0.0.1/accounts/
--rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.0.1/accounts/__init__.py
--rw-r--r--   0 igormusic   (501) staff       (20)     8367 2023-04-22 06:04:52.000000 transaction-accounts-0.0.1/accounts/metadata.py
--rw-r--r--   0 igormusic   (501) staff       (20)    11888 2023-04-22 06:04:52.000000 transaction-accounts-0.0.1/accounts/runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-04-22 06:07:38.896294 transaction-accounts-0.0.1/setup.cfg
--rw-r--r--   0 igormusic   (501) staff       (20)      972 2023-04-22 05:59:24.000000 transaction-accounts-0.0.1/setup.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 06:07:38.895341 transaction-accounts-0.0.1/transaction_accounts.egg-info/
--rw-r--r--   0 igormusic   (501) staff       (20)      746 2023-04-22 06:07:38.000000 transaction-accounts-0.0.1/transaction_accounts.egg-info/PKG-INFO
--rw-r--r--   0 igormusic   (501) staff       (20)      311 2023-04-22 06:07:38.000000 transaction-accounts-0.0.1/transaction_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-04-22 06:07:38.000000 transaction-accounts-0.0.1/transaction_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 igormusic   (501) staff       (20)       33 2023-04-22 06:07:38.000000 transaction-accounts-0.0.1/transaction_accounts.egg-info/requires.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-04-22 06:07:38.000000 transaction-accounts-0.0.1/transaction_accounts.egg-info/top_level.txt
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 06:29:39.817572 transaction-accounts-0.0.2/
+-rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.0.2/LICENSE.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)     7001 2023-04-22 06:29:39.817723 transaction-accounts-0.0.2/PKG-INFO
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 06:29:39.814686 transaction-accounts-0.0.2/accounts/
+-rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.0.2/accounts/__init__.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     8367 2023-04-22 06:04:52.000000 transaction-accounts-0.0.2/accounts/metadata.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    11888 2023-04-22 06:04:52.000000 transaction-accounts-0.0.2/accounts/runtime.py
+-rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-04-22 06:29:39.818248 transaction-accounts-0.0.2/setup.cfg
+-rw-r--r--   0 igormusic   (501) staff       (20)     1181 2023-04-22 06:27:34.000000 transaction-accounts-0.0.2/setup.py
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 06:29:39.817229 transaction-accounts-0.0.2/transaction_accounts.egg-info/
+-rw-r--r--   0 igormusic   (501) staff       (20)     7001 2023-04-22 06:29:39.000000 transaction-accounts-0.0.2/transaction_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 igormusic   (501) staff       (20)      311 2023-04-22 06:29:39.000000 transaction-accounts-0.0.2/transaction_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-04-22 06:29:39.000000 transaction-accounts-0.0.2/transaction_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)       33 2023-04-22 06:29:39.000000 transaction-accounts-0.0.2/transaction_accounts.egg-info/requires.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-04-22 06:29:39.000000 transaction-accounts-0.0.2/transaction_accounts.egg-info/top_level.txt
```

### Comparing `transaction-accounts-0.0.1/LICENSE.txt` & `transaction-accounts-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.0.1/accounts/metadata.py` & `transaction-accounts-0.0.2/accounts/metadata.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.0.1/accounts/runtime.py` & `transaction-accounts-0.0.2/accounts/runtime.py`

 * *Files identical despite different names*

