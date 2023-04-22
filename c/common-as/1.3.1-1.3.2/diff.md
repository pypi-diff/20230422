# Comparing `tmp/common_as-1.3.1.tar.gz` & `tmp/common_as-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_as-1.3.1.tar", last modified: Fri Apr 21 17:41:23 2023, max compression
+gzip compressed data, was "common_as-1.3.2.tar", last modified: Sat Apr 22 10:17:43 2023, max compression
```

## Comparing `common_as-1.3.1.tar` & `common_as-1.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 17:41:23.378647 common_as-1.3.1/
--rw-rw-rw-   0        0        0     1093 2023-01-04 12:01:22.000000 common_as-1.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0      212 2023-04-21 17:41:23.374103 common_as-1.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 17:41:23.338237 common_as-1.3.1/common_as/
--rw-rw-rw-   0        0        0      133 2023-04-21 17:24:28.000000 common_as-1.3.1/common_as/__init__.py
--rw-rw-rw-   0        0        0     1249 2023-02-01 17:58:41.000000 common_as-1.3.1/common_as/base_helper.py
--rw-rw-rw-   0        0        0    15291 2023-04-21 02:44:22.000000 common_as-1.3.1/common_as/calculate_ta.py
--rw-rw-rw-   0        0        0     1691 2023-04-21 02:44:53.000000 common_as-1.3.1/common_as/date_util.py
--rw-rw-rw-   0        0        0     2527 2023-04-21 02:38:37.000000 common_as-1.3.1/common_as/dbmysql.py
--rw-rw-rw-   0        0        0      360 2023-04-21 02:45:15.000000 common_as-1.3.1/common_as/enums.py
--rw-rw-rw-   0        0        0      385 2023-04-21 02:45:31.000000 common_as-1.3.1/common_as/file_util.py
--rw-rw-rw-   0        0        0    19434 2023-04-21 02:42:12.000000 common_as-1.3.1/common_as/helper_breeze.py
--rw-rw-rw-   0        0        0    11979 2023-04-21 02:47:15.000000 common_as-1.3.1/common_as/helper_ks.py
--rw-rw-rw-   0        0        0    16861 2023-04-21 02:45:46.000000 common_as-1.3.1/common_as/kitehelper.py
--rw-rw-rw-   0        0        0     7355 2023-04-21 02:43:37.000000 common_as-1.3.1/common_as/levels.py
--rw-rw-rw-   0        0        0     1350 2023-04-21 02:46:10.000000 common_as-1.3.1/common_as/log_util.py
--rw-rw-rw-   0        0        0     2351 2023-04-21 02:46:35.000000 common_as-1.3.1/common_as/telegram_util.py
--rw-rw-rw-   0        0        0     2237 2023-04-21 02:47:03.000000 common_as-1.3.1/common_as/util.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:41:23.374103 common_as-1.3.1/common_as.egg-info/
--rw-rw-rw-   0        0        0      212 2023-04-21 17:41:23.000000 common_as-1.3.1/common_as.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-04-21 17:41:23.000000 common_as-1.3.1/common_as.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 17:41:23.000000 common_as-1.3.1/common_as.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-21 17:41:23.000000 common_as-1.3.1/common_as.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 17:41:23.000000 common_as-1.3.1/common_as.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 17:41:23.378647 common_as-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      354 2023-04-21 17:31:14.000000 common_as-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 10:17:43.316614 common_as-1.3.2/
+-rw-rw-rw-   0        0        0     1093 2023-01-04 12:01:22.000000 common_as-1.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      212 2023-04-22 10:17:43.315614 common_as-1.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-22 10:17:43.293988 common_as-1.3.2/common_as/
+-rw-rw-rw-   0        0        0      168 2023-04-22 10:15:34.000000 common_as-1.3.2/common_as/__init__.py
+-rw-rw-rw-   0        0        0     1249 2023-02-01 17:58:41.000000 common_as-1.3.2/common_as/base_helper.py
+-rw-rw-rw-   0        0        0    15291 2023-04-21 02:44:22.000000 common_as-1.3.2/common_as/calculate_ta.py
+-rw-rw-rw-   0        0        0     1691 2023-04-21 02:44:53.000000 common_as-1.3.2/common_as/date_util.py
+-rw-rw-rw-   0        0        0     2527 2023-04-21 02:38:37.000000 common_as-1.3.2/common_as/dbmysql.py
+-rw-rw-rw-   0        0        0      360 2023-04-21 02:45:15.000000 common_as-1.3.2/common_as/enums.py
+-rw-rw-rw-   0        0        0      385 2023-04-21 02:45:31.000000 common_as-1.3.2/common_as/file_util.py
+-rw-rw-rw-   0        0        0    19434 2023-04-21 02:42:12.000000 common_as-1.3.2/common_as/helper_breeze.py
+-rw-rw-rw-   0        0        0    11979 2023-04-21 02:47:15.000000 common_as-1.3.2/common_as/helper_ks.py
+-rw-rw-rw-   0        0        0    16861 2023-04-21 02:45:46.000000 common_as-1.3.2/common_as/kitehelper.py
+-rw-rw-rw-   0        0        0     7431 2023-04-22 09:48:34.000000 common_as-1.3.2/common_as/levels.py
+-rw-rw-rw-   0        0        0     1350 2023-04-21 02:46:10.000000 common_as-1.3.2/common_as/log_util.py
+-rw-rw-rw-   0        0        0     2351 2023-04-21 02:46:35.000000 common_as-1.3.2/common_as/telegram_util.py
+-rw-rw-rw-   0        0        0     2237 2023-04-21 02:47:03.000000 common_as-1.3.2/common_as/util.py
+drwxrwxrwx   0        0        0        0 2023-04-22 10:17:43.313613 common_as-1.3.2/common_as.egg-info/
+-rw-rw-rw-   0        0        0      212 2023-04-22 10:17:43.000000 common_as-1.3.2/common_as.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-04-22 10:17:43.000000 common_as-1.3.2/common_as.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 10:17:43.000000 common_as-1.3.2/common_as.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-22 10:17:43.000000 common_as-1.3.2/common_as.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-22 10:17:43.000000 common_as-1.3.2/common_as.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 10:17:43.316614 common_as-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      344 2023-04-22 10:15:41.000000 common_as-1.3.2/setup.py
```

### Comparing `common_as-1.3.1/LICENSE.txt` & `common_as-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `common_as-1.3.1/common_as/base_helper.py` & `common_as-1.3.2/common_as/base_helper.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.1/common_as/calculate_ta.py` & `common_as-1.3.2/common_as/calculate_ta.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.1/common_as/date_util.py` & `common_as-1.3.2/common_as/date_util.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.1/common_as/dbmysql.py` & `common_as-1.3.2/common_as/dbmysql.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.1/common_as/helper_breeze.py` & `common_as-1.3.2/common_as/helper_breeze.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.1/common_as/helper_ks.py` & `common_as-1.3.2/common_as/helper_ks.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.1/common_as/kitehelper.py` & `common_as-1.3.2/common_as/kitehelper.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.1/common_as/levels.py` & `common_as-1.3.2/common_as/levels.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,19 +149,22 @@
             self.at_time=datetime.now()
         else:
             self.at_time=at_time
         self.symbol=symbol
         self.exchangeToken=exchangeToken
         self.token=exchangeToken
 
-    def __str__():
-        return f'code: {self.code}, qty: {self.qty}, price: {self.price}, b/s: {self.buysell}, token: {self.token}'
+    def __str__(self):
+        return f'Order(code: {self.code}, qty: {self.qty}, price: {self.price}, b/s: {self.buysell}, token: {self.token})'
+
+    def __repr__ (self): 
+        return self.__str__()
 
     def to_string(self):
-        return __str__()
+        return self.__str__()
 
     @classmethod
     def fromjson(self, ordjson):
         "Initialize MyData from a file"
         ord = self(ordjson['symbol'], 1,2,3,4,5,6,7)
         return ord
```

### Comparing `common_as-1.3.1/common_as/log_util.py` & `common_as-1.3.2/common_as/log_util.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.1/common_as/telegram_util.py` & `common_as-1.3.2/common_as/telegram_util.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.1/common_as/util.py` & `common_as-1.3.2/common_as/util.py`

 * *Files identical despite different names*

