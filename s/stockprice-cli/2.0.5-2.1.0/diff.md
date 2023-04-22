# Comparing `tmp/stockprice_cli-2.0.5-py3-none-any.whl.zip` & `tmp/stockprice_cli-2.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3192 bytes, number of entries: 8
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 16:51 stockprice/__init__.py
--rw-r--r--  2.0 unx     2404 b- defN 23-Apr-11 16:51 stockprice/calculate_price_movement.py
--rw-r--r--  2.0 unx      872 b- defN 23-Apr-11 16:51 stockprice/main.py
--rw-r--r--  2.0 unx      612 b- defN 23-Apr-11 16:51 stockprice_cli-2.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 16:51 stockprice_cli-2.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Apr-11 16:51 stockprice_cli-2.0.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-11 16:51 stockprice_cli-2.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      672 b- defN 23-Apr-11 16:51 stockprice_cli-2.0.5.dist-info/RECORD
-8 files, 4716 bytes uncompressed, 2000 bytes compressed:  57.6%
+Zip file size: 3291 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-22 16:59 stockprice/__init__.py
+-rw-r--r--  2.0 unx     2552 b- defN 23-Apr-22 16:59 stockprice/calculate_price_movement.py
+-rw-r--r--  2.0 unx      974 b- defN 23-Apr-22 16:59 stockprice/main.py
+-rw-r--r--  2.0 unx      612 b- defN 23-Apr-22 16:59 stockprice_cli-2.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 16:59 stockprice_cli-2.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Apr-22 16:59 stockprice_cli-2.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-22 16:59 stockprice_cli-2.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      672 b- defN 23-Apr-22 16:59 stockprice_cli-2.1.0.dist-info/RECORD
+8 files, 4966 bytes uncompressed, 2099 bytes compressed:  57.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: stockprice/calculate_price_movement.py
 Comment: 
 
 Filename: stockprice/main.py
 Comment: 
 
-Filename: stockprice_cli-2.0.5.dist-info/METADATA
+Filename: stockprice_cli-2.1.0.dist-info/METADATA
 Comment: 
 
-Filename: stockprice_cli-2.0.5.dist-info/WHEEL
+Filename: stockprice_cli-2.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: stockprice_cli-2.0.5.dist-info/entry_points.txt
+Filename: stockprice_cli-2.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: stockprice_cli-2.0.5.dist-info/top_level.txt
+Filename: stockprice_cli-2.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: stockprice_cli-2.0.5.dist-info/RECORD
+Filename: stockprice_cli-2.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stockprice/calculate_price_movement.py

```diff
@@ -35,18 +35,21 @@
     Returns:
         current_price (float): Current price
         currency (str): The currency of the price
         percentage_change_1day (float): Price change during last trading day
         percentage_change_7day (float): Price change since last trading day >=7days ago
         percentage_change_30day (float): Price change since last trading day >=30days ago
     """
-    response_body = requests.get(
+    response = requests.get(
         f"https://query2.finance.yahoo.com/v8/finance/chart/{ticker}?interval=1d&range=30d",
         headers={"User-Agent": "Mozilla/5.0"},
-    ).json()
+    )
+    if response.status_code == 404:
+        raise ValueError(f"The ticker symbol {ticker} is not listed on yahoo finance.")
+    response_body = response.json()
     currency = response_body["chart"]["result"][0]["meta"]["currency"]
     closing_prices = response_body["chart"]["result"][0]["indicators"]["quote"][0][
         "close"
     ]
     timestamps = response_body["chart"]["result"][0]["timestamp"]
 
     current_price = closing_prices[-1]
```

## stockprice/main.py

```diff
@@ -9,21 +9,24 @@
     for input in raw_inputs:
         input = input.upper()
         if input[-1] == ",":
             input = input[:-1]
 
         stock_tickers.extend(input.split(","))
     for ticker in stock_tickers:
-        (
-            current_price,
-            currency,
-            percentage_change_1day,
-            percentage_change_7day,
-            percentage_change_30day,
-        ) = calculate_price_movement(ticker)
-        summary = f"{ticker} -- Current price: {current_price:.2f} {currency} -- Daily change: {percentage_change_1day:.2f}%, 7-day change: {percentage_change_7day:.2f}%, 30-day change: {percentage_change_30day:.2f}%"
+        try:
+            (
+                current_price,
+                currency,
+                percentage_change_1day,
+                percentage_change_7day,
+                percentage_change_30day,
+            ) = calculate_price_movement(ticker)
+            summary = f"{ticker} -- Current price: {current_price:.2f} {currency} -- Daily change: {percentage_change_1day:.2f}%, 7-day change: {percentage_change_7day:.2f}%, 30-day change: {percentage_change_30day:.2f}%"
 
-        print(summary)
+            print(summary)
+        except ValueError as e:
+            print(e)
 
 
 if __name__ == "__main__":
     main()
```

## Comparing `stockprice_cli-2.0.5.dist-info/METADATA` & `stockprice_cli-2.1.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockprice-cli
-Version: 2.0.5
+Version: 2.1.0
 Summary: UNKNOWN
 Home-page: https://github.com/Thomas-mcinally/stockprice
 Author: Thomas Mcinally
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

## Comparing `stockprice_cli-2.0.5.dist-info/RECORD` & `stockprice_cli-2.1.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 stockprice/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-stockprice/calculate_price_movement.py,sha256=wH567ymdW6N8jVsRiN6GjpNHMvMeCzN4NQXUGpdXe3A,2404
-stockprice/main.py,sha256=FRLewUInfY40cCgXTL2UCxZss7RJ9qP4or4YWsKZDM0,872
-stockprice_cli-2.0.5.dist-info/METADATA,sha256=8Au97nk7IEyO_Q7rMr5cs2rmVi6C8ur6WzSjNPA7RzI,612
-stockprice_cli-2.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-stockprice_cli-2.0.5.dist-info/entry_points.txt,sha256=BbbvxzL6AWVnrrEHkXLFL8NaKwhZ0NsKnzHKibL587M,53
-stockprice_cli-2.0.5.dist-info/top_level.txt,sha256=KeT6ClRPQ5zQdkU0Ela_rRQ2aR7Dy7SjyOcfhcPy6kw,11
-stockprice_cli-2.0.5.dist-info/RECORD,,
+stockprice/calculate_price_movement.py,sha256=5HTpYyA7p2tfo0AzC-xq1J6QCSOJ4OmqbGSmo1F98xE,2552
+stockprice/main.py,sha256=J3LN9QYpYlPPF8YSd52uxSqBXyn1Ky1zBplg4gWISmA,974
+stockprice_cli-2.1.0.dist-info/METADATA,sha256=OiI3L6uRVjHIEXx2zyKAK9iH1TfRxtRT9gOzFSfBF2s,612
+stockprice_cli-2.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+stockprice_cli-2.1.0.dist-info/entry_points.txt,sha256=BbbvxzL6AWVnrrEHkXLFL8NaKwhZ0NsKnzHKibL587M,53
+stockprice_cli-2.1.0.dist-info/top_level.txt,sha256=KeT6ClRPQ5zQdkU0Ela_rRQ2aR7Dy7SjyOcfhcPy6kw,11
+stockprice_cli-2.1.0.dist-info/RECORD,,
```

