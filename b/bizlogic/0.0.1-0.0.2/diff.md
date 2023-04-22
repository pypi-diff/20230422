# Comparing `tmp/bizlogic-0.0.1.tar.gz` & `tmp/bizlogic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bizlogic-0.0.1.tar", max compression
+gzip compressed data, was "bizlogic-0.0.2.tar", max compression
```

## Comparing `bizlogic-0.0.1.tar` & `bizlogic-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.0.1/LICENSE
--rw-r--r--   0        0        0     1991 2023-04-20 22:21:31.358991 bizlogic-0.0.1/README.md
--rw-r--r--   0        0        0       58 2023-04-20 22:57:52.970782 bizlogic-0.0.1/bizlogic/__init__.py
--rw-r--r--   0        0        0     2204 2023-04-21 19:07:41.827682 bizlogic-0.0.1/bizlogic/application.py
--rw-r--r--   0        0        0     6704 2023-04-21 19:08:22.662727 bizlogic-0.0.1/bizlogic/loan.py
--rw-r--r--   0        0        0     1781 2023-04-21 19:05:52.691719 bizlogic-0.0.1/bizlogic/vouch.py
--rw-r--r--   0        0        0      452 2023-04-21 00:55:40.931522 bizlogic-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2531 1970-01-01 00:00:00.000000 bizlogic-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1991 2023-04-20 22:21:31.358991 bizlogic-0.0.2/README.md
+-rw-r--r--   0        0        0       58 2023-04-22 18:31:37.985161 bizlogic-0.0.2/bizlogic/__init__.py
+-rw-r--r--   0        0        0     2492 2023-04-22 16:52:44.739841 bizlogic-0.0.2/bizlogic/application.py
+-rw-r--r--   0        0        0       16 2023-04-22 17:58:44.167371 bizlogic-0.0.2/bizlogic/loan/__init__.py
+-rw-r--r--   0        0        0     2089 2023-04-22 18:15:32.612007 bizlogic-0.0.2/bizlogic/loan/reader.py
+-rw-r--r--   0        0        0     1587 2023-04-22 18:45:00.284766 bizlogic-0.0.2/bizlogic/loan/repayment.py
+-rw-r--r--   0        0        0     1061 2023-04-22 18:21:43.913408 bizlogic-0.0.2/bizlogic/loan/status.py
+-rw-r--r--   0        0        0     3222 2023-04-22 18:21:59.201132 bizlogic-0.0.2/bizlogic/loan/writer.py
+-rw-r--r--   0        0        0     2071 2023-04-22 16:57:44.718847 bizlogic-0.0.2/bizlogic/vouch.py
+-rw-r--r--   0        0        0      451 2023-04-22 18:31:16.788313 bizlogic-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2524 1970-01-01 00:00:00.000000 bizlogic-0.0.2/PKG-INFO
```

### Comparing `bizlogic-0.0.1/LICENSE` & `bizlogic-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.1/README.md` & `bizlogic-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.1/bizlogic/application.py` & `bizlogic-0.0.2/bizlogic/application.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import time
 from typing import List, Self
 
 from ipfskvs.store import Store  # noqa: I201
-from ipfsclient.ipfs import Ipfs  # noqa: I201
 from ipfskvs.index import Index  # noqa: I201
+from ipfsclient.ipfs import Ipfs  # noqa: I201
 
 from protoc.loan_application_pb2 import LoanApplication
 
-PREFIX="application"
+PREFIX = "application"
 
 # ipfs filename:
 #   application/borrower_<id>/created_<timestamp>
 
 class LoanApplicationWriter():
+    """Loan Application Writer
+    
+    Create a request to ask for funds. Other users will then run a credit check on you
+    and send you loan offers. When the user accepts a loan offer, they can close their
+    loan application to tell others they are no longer interested in additional borrowing.
+    """
     borrower: str
     amount_asking: int
     ipfsclient: Ipfs
     data: LoanApplication
 
     def __init__(self: Self, ipfsclient: Ipfs, borrower: str, amount_asking: int):
         """Constructor"""
@@ -24,18 +30,17 @@
         self.ipfsclient = ipfsclient
         self.amount_asking = amount_asking
         self.data = LoanApplication(
             amount_asking=self.amount_asking,
             closed=False
         )
         self._generate_index()
-        self._write()
 
     
-    def _write(self):
+    def write(self):
 
         store = Store(
             index=self.index,
             ipfs=self.ipfsclient,
             writer=self.data
         )
```

### Comparing `bizlogic-0.0.1/PKG-INFO` & `bizlogic-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: bizlogic
-Version: 0.0.1
+Version: 0.0.2
 Summary: web3 lending platform business logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: ipfsclient (>=0.0.7,<0.0.8)
+Requires-Dist: ipfsclient (==0.0.7)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: protobuf (>=4.22.3,<5.0.0)
 Requires-Dist: py-multicodec (>=0.2.1,<0.3.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # BizLogic
```

