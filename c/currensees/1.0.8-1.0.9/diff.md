# Comparing `tmp/currensees-1.0.8.tar.gz` & `tmp/currensees-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/currensees-1.0.8.tar", last modified: Thu Apr 20 00:46:30 2023, max compression
+gzip compressed data, was "dist/currensees-1.0.9.tar", last modified: Sat Apr 22 19:10:34 2023, max compression
```

## Comparing `currensees-1.0.8.tar` & `currensees-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-20 00:46:30.788519 currensees-1.0.8/
--rw-r--r--   0 finn       (501) staff       (20)     6279 2023-04-20 00:46:30.788835 currensees-1.0.8/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     3154 2023-04-20 00:45:27.000000 currensees-1.0.8/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-20 00:46:30.782690 currensees-1.0.8/currensees/
--rw-r--r--   0 finn       (501) staff       (20)      292 2023-04-20 00:30:20.000000 currensees-1.0.8/currensees/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)      908 2023-04-19 23:42:50.000000 currensees-1.0.8/currensees/auth.py
--rw-r--r--   0 finn       (501) staff       (20)      711 2023-04-19 23:51:19.000000 currensees-1.0.8/currensees/convert.py
--rw-r--r--   0 finn       (501) staff       (20)      665 2023-04-19 23:53:31.000000 currensees-1.0.8/currensees/convert_all.py
--rw-r--r--   0 finn       (501) staff       (20)     1149 2023-04-19 23:47:05.000000 currensees-1.0.8/currensees/currencies.py
--rw-r--r--   0 finn       (501) staff       (20)      493 2023-04-19 23:55:16.000000 currensees-1.0.8/currensees/daily_average.py
--rw-r--r--   0 finn       (501) staff       (20)     1261 2023-04-19 23:49:50.000000 currensees-1.0.8/currensees/historical.py
--rw-r--r--   0 finn       (501) staff       (20)     1218 2023-04-19 23:59:06.000000 currensees-1.0.8/currensees/margins_spreads.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-20 00:45:55.000000 currensees-1.0.8/currensees/version.py
--rw-r--r--   0 finn       (501) staff       (20)      530 2023-04-19 23:56:35.000000 currensees-1.0.8/currensees/weekly_average.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-20 00:46:30.787857 currensees-1.0.8/currensees.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     6279 2023-04-20 00:46:30.000000 currensees-1.0.8/currensees.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      479 2023-04-20 00:46:30.000000 currensees-1.0.8/currensees.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-20 00:46:30.000000 currensees-1.0.8/currensees.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-20 00:46:17.000000 currensees-1.0.8/currensees.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-20 00:46:30.000000 currensees-1.0.8/currensees.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       11 2023-04-20 00:46:30.000000 currensees-1.0.8/currensees.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-20 00:46:30.789793 currensees-1.0.8/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2646 2023-04-20 00:45:55.000000 currensees-1.0.8/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-22 19:10:34.497223 currensees-1.0.9/
+-rw-r--r--   0 finn       (501) staff       (20)     6299 2023-04-22 19:10:34.497521 currensees-1.0.9/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     3174 2023-04-22 19:08:57.000000 currensees-1.0.9/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-22 19:10:34.491913 currensees-1.0.9/currensees/
+-rw-r--r--   0 finn       (501) staff       (20)      292 2023-04-20 00:30:20.000000 currensees-1.0.9/currensees/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)      908 2023-04-19 23:42:50.000000 currensees-1.0.9/currensees/auth.py
+-rw-r--r--   0 finn       (501) staff       (20)      755 2023-04-22 18:24:20.000000 currensees-1.0.9/currensees/convert.py
+-rw-r--r--   0 finn       (501) staff       (20)      709 2023-04-22 18:21:27.000000 currensees-1.0.9/currensees/convert_all.py
+-rw-r--r--   0 finn       (501) staff       (20)     1149 2023-04-22 18:45:05.000000 currensees-1.0.9/currensees/currencies.py
+-rw-r--r--   0 finn       (501) staff       (20)      493 2023-04-19 23:55:16.000000 currensees-1.0.9/currensees/daily_average.py
+-rw-r--r--   0 finn       (501) staff       (20)     1261 2023-04-22 19:03:02.000000 currensees-1.0.9/currensees/historical.py
+-rw-r--r--   0 finn       (501) staff       (20)     1218 2023-04-22 18:46:05.000000 currensees-1.0.9/currensees/margins_spreads.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-22 19:09:45.000000 currensees-1.0.9/currensees/version.py
+-rw-r--r--   0 finn       (501) staff       (20)      530 2023-04-19 23:56:35.000000 currensees-1.0.9/currensees/weekly_average.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-22 19:10:34.496671 currensees-1.0.9/currensees.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     6299 2023-04-22 19:10:34.000000 currensees-1.0.9/currensees.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      479 2023-04-22 19:10:34.000000 currensees-1.0.9/currensees.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-22 19:10:34.000000 currensees-1.0.9/currensees.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-22 19:10:19.000000 currensees-1.0.9/currensees.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-22 19:10:34.000000 currensees-1.0.9/currensees.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       11 2023-04-22 19:10:34.000000 currensees-1.0.9/currensees.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-22 19:10:34.498349 currensees-1.0.9/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2646 2023-04-22 19:09:45.000000 currensees-1.0.9/setup.py
```

### Comparing `currensees-1.0.8/PKG-INFO` & `currensees-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currensees
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python library for integrating with the Currency API.
 Home-page: https://moatsystems.com/currency-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/moatsystems/currensees_sdk/issues
 Project-URL: Changes, https://github.com/moatsystems/currensees_sdk/blob/main/CHANGELOG.md
@@ -75,23 +75,23 @@
             print("Currency:", result)
         
             historical = Historical(auth.headers)
             result = historical.get_historical(username, "2023_04_19", "19", "04", "2023")
             print("Historical data:", result)
         
             uuid = "historical_uuid"
-            result = historical.get_historical_currency(uuid, username, "19", "04", "2023", "2023_04_19")
+            result = historical.get_historical_currency(uuid, username, "2023_04_19", "19", "04", "2023")
             print("Historical currency:", result)
         
             convert = Convert(auth.headers)
-            result = convert.convert_currency("2023_04_19", "GBP", "EUR", "500")
+            result = convert.convert_currency(username, "2023_04_19", "GBP", "EUR", "500")
             print("Converted amount:", result)
         
             convert_all = ConvertAll(auth.headers)
-            result = convert_all.convert_all_currencies("GBP", 120, "2023_04_19")
+            result = convert_all.convert_all_currencies(username, "GBP", 120, "2023_04_19")
             print("Converted amounts:", result)
         
             daily_average = DailyAverage(auth.headers)
             result = daily_average.get_daily_average("2023_04_19")
             print("Daily average:", result)
         
             weekly_average = WeeklyAverage(auth.headers)
```

### Comparing `currensees-1.0.8/README.md` & `currensees-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,23 @@
 print("Currency:", result)
 
 historical = Historical(auth.headers)
 result = historical.get_historical(username, "2023_04_19", "19", "04", "2023")
 print("Historical data:", result)
 
 uuid = "historical_uuid"
-result = historical.get_historical_currency(uuid, username, "19", "04", "2023", "2023_04_19")
+result = historical.get_historical_currency(uuid, username, "2023_04_19", "19", "04", "2023")
 print("Historical currency:", result)
 
 convert = Convert(auth.headers)
-result = convert.convert_currency("2023_04_19", "GBP", "EUR", "500")
+result = convert.convert_currency(username, "2023_04_19", "GBP", "EUR", "500")
 print("Converted amount:", result)
 
 convert_all = ConvertAll(auth.headers)
-result = convert_all.convert_all_currencies("GBP", 120, "2023_04_19")
+result = convert_all.convert_all_currencies(username, "GBP", 120, "2023_04_19")
 print("Converted amounts:", result)
 
 daily_average = DailyAverage(auth.headers)
 result = daily_average.get_daily_average("2023_04_19")
 print("Daily average:", result)
 
 weekly_average = WeeklyAverage(auth.headers)
```

### Comparing `currensees-1.0.8/currensees/auth.py` & `currensees-1.0.9/currensees/auth.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.8/currensees/convert.py` & `currensees-1.0.9/currensees/convert.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import json
 
 class Convert:
     def __init__(self, headers):
         self.base_url = 'https://currensees.com/v1'
         self.headers = headers
 
-    def convert_currency(self, date, base_currency, target_currency, amount):
+    def convert_currency(self, username, date, base_currency, target_currency, amount):
         url = f'{self.base_url}/convert'
         data = {
+            'username': username,
             'date': date,
             'base_currency': base_currency,
             'target_currency': target_currency,
             'amount': amount
         }
         response = requests.post(url, headers=self.headers, data=json.dumps(data))
```

### Comparing `currensees-1.0.8/currensees/convert_all.py` & `currensees-1.0.9/currensees/convert_all.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import json
 
 class ConvertAll:
     def __init__(self, headers):
         self.base_url = 'https://currensees.com/v1'
         self.headers = headers
 
-    def convert_all_currencies(self, base_currency, amount, date):
+    def convert_all_currencies(self, username, base_currency, amount, date):
         url = f'{self.base_url}/convert_all'
         data = {
+            'username': username,
             'base_currency': base_currency,
             'amount': amount,
             'date': date
         }
         response = requests.post(url, headers=self.headers, data=json.dumps(data))
         
         if response.status_code == 200:
```

### Comparing `currensees-1.0.8/currensees/currencies.py` & `currensees-1.0.9/currensees/currencies.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.8/currensees/historical.py` & `currensees-1.0.9/currensees/historical.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,22 +18,22 @@
         response = requests.get(url, headers=self.headers, params=params)
         
         if response.status_code == 200:
             return response.json()
         else:
             raise Exception(f"Failed to get historical data: {response.text}")
 
-    def get_historical_currency(self, uuid, username, day, month, year, date_string):
+    def get_historical_currency(self, uuid, username, date_string, day, month, year):
         url = f'{self.base_url}/historical/{uuid}'
         params = {
             'username': username,
+            'date_string': date_string,
             'day': day,
             'month': month,
-            'year': year,
-            'date_string': date_string
+            'year': year
         }
         response = requests.get(url, headers=self.headers, params=params)
         
         if response.status_code == 200:
             return response.json()
         else:
             raise Exception(f"Failed to get historical currency: {response.text}")
```

### Comparing `currensees-1.0.8/currensees/margins_spreads.py` & `currensees-1.0.9/currensees/margins_spreads.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.8/currensees/weekly_average.py` & `currensees-1.0.9/currensees/weekly_average.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.8/currensees.egg-info/PKG-INFO` & `currensees-1.0.9/currensees.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currensees
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python library for integrating with the Currency API.
 Home-page: https://moatsystems.com/currency-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/moatsystems/currensees_sdk/issues
 Project-URL: Changes, https://github.com/moatsystems/currensees_sdk/blob/main/CHANGELOG.md
@@ -75,23 +75,23 @@
             print("Currency:", result)
         
             historical = Historical(auth.headers)
             result = historical.get_historical(username, "2023_04_19", "19", "04", "2023")
             print("Historical data:", result)
         
             uuid = "historical_uuid"
-            result = historical.get_historical_currency(uuid, username, "19", "04", "2023", "2023_04_19")
+            result = historical.get_historical_currency(uuid, username, "2023_04_19", "19", "04", "2023")
             print("Historical currency:", result)
         
             convert = Convert(auth.headers)
-            result = convert.convert_currency("2023_04_19", "GBP", "EUR", "500")
+            result = convert.convert_currency(username, "2023_04_19", "GBP", "EUR", "500")
             print("Converted amount:", result)
         
             convert_all = ConvertAll(auth.headers)
-            result = convert_all.convert_all_currencies("GBP", 120, "2023_04_19")
+            result = convert_all.convert_all_currencies(username, "GBP", 120, "2023_04_19")
             print("Converted amounts:", result)
         
             daily_average = DailyAverage(auth.headers)
             result = daily_average.get_daily_average("2023_04_19")
             print("Daily average:", result)
         
             weekly_average = WeeklyAverage(auth.headers)
```

### Comparing `currensees-1.0.8/setup.py` & `currensees-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "currensees"
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 REQUIRES = ["requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

