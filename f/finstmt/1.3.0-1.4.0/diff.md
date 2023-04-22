# Comparing `tmp/finstmt-1.3.0.tar.gz` & `tmp/finstmt-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finstmt-1.3.0.tar", max compression
+gzip compressed data, was "finstmt-1.4.0.tar", max compression
```

## Comparing `finstmt-1.3.0.tar` & `finstmt-1.4.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1082 2023-04-12 00:08:44.972746 finstmt-1.3.0/LICENSE.md
--rw-r--r--   0        0        0     2107 2023-04-12 00:08:44.972746 finstmt-1.3.0/README.md
--rw-r--r--   0        0        0     1532 2023-04-12 00:08:44.976745 finstmt-1.3.0/conf.py
--rw-r--r--   0        0        0      386 2023-04-12 00:09:23.265073 finstmt-1.3.0/finstmt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/bs/__init__.py
--rw-r--r--   0        0        0    38597 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/bs/config.py
--rw-r--r--   0        0        0      742 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/bs/main.py
--rw-r--r--   0        0        0      197 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/check.py
--rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/clean/__init__.py
--rw-r--r--   0        0        0      946 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/clean/name.py
--rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/combined/__init__.py
--rw-r--r--   0        0        0     5947 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/combined/combinator.py
--rw-r--r--   0        0        0    12737 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/combined/statements.py
--rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/config_manage/__init__.py
--rw-r--r--   0        0        0     8245 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/config_manage/base.py
--rw-r--r--   0        0        0     2189 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/config_manage/data.py
--rw-r--r--   0        0        0      872 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/config_manage/global_.py
--rw-r--r--   0        0        0     2935 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/config_manage/statement.py
--rw-r--r--   0        0        0     4483 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/config_manage/statements.py
--rw-r--r--   0        0        0      926 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/exc.py
--rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/findata/__init__.py
--rw-r--r--   0        0        0     6233 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/findata/period_data.py
--rw-r--r--   0        0        0     1505 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/findata/statement_item.py
--rw-r--r--   0        0        0    11904 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/findata/statementsbase.py
--rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/__init__.py
--rw-r--r--   0        0        0     4896 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/config.py
--rw-r--r--   0        0        0      304 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/dataframe.py
--rw-r--r--   0        0        0     6764 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/main.py
--rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/__init__.py
--rw-r--r--   0        0        0     1028 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/average.py
--rw-r--r--   0        0        0     3486 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/base.py
--rw-r--r--   0        0        0     3392 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/cagr.py
--rw-r--r--   0        0        0     1316 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/chooser.py
--rw-r--r--   0        0        0     2469 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/manual.py
--rw-r--r--   0        0        0     3007 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/prophet.py
--rw-r--r--   0        0        0      803 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/recent.py
--rw-r--r--   0        0        0     1651 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/models/trend.py
--rw-r--r--   0        0        0     1529 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/plot.py
--rw-r--r--   0        0        0     4339 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/forecast/statements.py
--rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/inc/__init__.py
--rw-r--r--   0        0        0    12013 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/inc/config.py
--rw-r--r--   0        0        0      769 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/inc/main.py
--rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/items/__init__.py
--rw-r--r--   0        0        0     2614 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/items/config.py
--rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/loaders/__init__.py
--rw-r--r--   0        0        0     1378 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/loaders/capiq.py
--rw-r--r--   0        0        0      278 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/logger.py
--rw-r--r--   0        0        0        0 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/resolver/__init__.py
--rw-r--r--   0        0        0     1140 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/resolver/base.py
--rw-r--r--   0        0        0    25053 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/resolver/forecast.py
--rw-r--r--   0        0        0     3238 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/resolver/history.py
--rw-r--r--   0        0        0     5900 2023-04-12 00:08:44.976745 finstmt-1.3.0/finstmt/resolver/solve.py
--rw-r--r--   0        0        0     1794 2023-04-12 00:09:23.161073 finstmt-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      474 2023-04-12 00:08:45.036746 finstmt-1.3.0/version.py
--rw-r--r--   0        0        0     3273 1970-01-01 00:00:00.000000 finstmt-1.3.0/setup.py
--rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 finstmt-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-22 12:11:24.546376 finstmt-1.4.0/LICENSE.md
+-rw-r--r--   0        0        0     2107 2023-04-22 12:11:24.546376 finstmt-1.4.0/README.md
+-rw-r--r--   0        0        0     1532 2023-04-22 12:11:24.546376 finstmt-1.4.0/conf.py
+-rw-r--r--   0        0        0      386 2023-04-22 12:11:57.002288 finstmt-1.4.0/finstmt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/bs/__init__.py
+-rw-r--r--   0        0        0    38597 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/bs/config.py
+-rw-r--r--   0        0        0      742 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/bs/main.py
+-rw-r--r--   0        0        0      197 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/check.py
+-rw-r--r--   0        0        0        0 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/clean/__init__.py
+-rw-r--r--   0        0        0      946 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/clean/name.py
+-rw-r--r--   0        0        0        0 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/combined/__init__.py
+-rw-r--r--   0        0        0     5947 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/combined/combinator.py
+-rw-r--r--   0        0        0    12737 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/combined/statements.py
+-rw-r--r--   0        0        0        0 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/config_manage/__init__.py
+-rw-r--r--   0        0        0     8245 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/config_manage/base.py
+-rw-r--r--   0        0        0     2189 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/config_manage/data.py
+-rw-r--r--   0        0        0      872 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/config_manage/global_.py
+-rw-r--r--   0        0        0     2935 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/config_manage/statement.py
+-rw-r--r--   0        0        0     4483 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/config_manage/statements.py
+-rw-r--r--   0        0        0      926 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/exc.py
+-rw-r--r--   0        0        0        0 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/findata/__init__.py
+-rw-r--r--   0        0        0     6233 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/findata/period_data.py
+-rw-r--r--   0        0        0     1505 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/findata/statement_item.py
+-rw-r--r--   0        0        0    11904 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/findata/statementsbase.py
+-rw-r--r--   0        0        0        0 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/forecast/__init__.py
+-rw-r--r--   0        0        0     4896 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/forecast/config.py
+-rw-r--r--   0        0        0      304 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/forecast/dataframe.py
+-rw-r--r--   0        0        0     6764 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/forecast/main.py
+-rw-r--r--   0        0        0        0 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/forecast/models/__init__.py
+-rw-r--r--   0        0        0     1028 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/forecast/models/average.py
+-rw-r--r--   0        0        0     3486 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/forecast/models/base.py
+-rw-r--r--   0        0        0     3392 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/forecast/models/cagr.py
+-rw-r--r--   0        0        0     1316 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/forecast/models/chooser.py
+-rw-r--r--   0        0        0     2469 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/forecast/models/manual.py
+-rw-r--r--   0        0        0     3007 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/forecast/models/prophet.py
+-rw-r--r--   0        0        0      803 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/forecast/models/recent.py
+-rw-r--r--   0        0        0     1651 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/forecast/models/trend.py
+-rw-r--r--   0        0        0     1529 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/forecast/plot.py
+-rw-r--r--   0        0        0     4339 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/forecast/statements.py
+-rw-r--r--   0        0        0        0 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/inc/__init__.py
+-rw-r--r--   0        0        0    12013 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/inc/config.py
+-rw-r--r--   0        0        0      769 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/inc/main.py
+-rw-r--r--   0        0        0        0 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/items/__init__.py
+-rw-r--r--   0        0        0     2614 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/items/config.py
+-rw-r--r--   0        0        0        0 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/loaders/__init__.py
+-rw-r--r--   0        0        0     1378 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/loaders/capiq.py
+-rw-r--r--   0        0        0      278 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/logger.py
+-rw-r--r--   0        0        0        0 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/resolver/__init__.py
+-rw-r--r--   0        0        0     1140 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/resolver/base.py
+-rw-r--r--   0        0        0    25053 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/resolver/forecast.py
+-rw-r--r--   0        0        0     3238 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/resolver/history.py
+-rw-r--r--   0        0        0     5900 2023-04-22 12:11:24.546376 finstmt-1.4.0/finstmt/resolver/solve.py
+-rw-r--r--   0        0        0     1794 2023-04-22 12:11:56.930288 finstmt-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-04-22 12:11:24.610376 finstmt-1.4.0/version.py
+-rw-r--r--   0        0        0     3273 1970-01-01 00:00:00.000000 finstmt-1.4.0/setup.py
+-rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 finstmt-1.4.0/PKG-INFO
```

### Comparing `finstmt-1.3.0/LICENSE.md` & `finstmt-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/README.md` & `finstmt-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/conf.py` & `finstmt-1.4.0/conf.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/bs/config.py` & `finstmt-1.4.0/finstmt/bs/config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -33,38 +33,60 @@
             "st investments",
             "shortterm invest",
             "short term invest",
             "st invest",
         ],
     ),
     ItemConfig(
+        "cash_and_st_invest",
+        "Cash and Short-Term Investments",
+        extract_names=[
+            "total cash st investments",
+            "total cash and st investments",
+            "total cash and shortterm investments",
+            "total cash and short term investments",
+            "total cash shortterm investments",
+            "total cash short term investments",
+            "total cash st invest",
+            "total cash and st invest",
+            "total cash and shortterm invest",
+            "total cash and short term invest",
+            "total cash shortterm invest",
+            "total cash short term invest",
+            "cash st investments",
+            "cash and st investments",
+            "cash and shortterm investments",
+            "cash and short term investments",
+            "cash shortterm investments",
+            "cash short term investments",
+            "cash st invest",
+            "cash and st invest",
+            "cash and shortterm invest",
+            "cash and short term invest",
+            "cash shortterm invest",
+            "cash short term invest",
+        ],
+        expr_str="cash[t] + st_invest[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+    ),
+    ItemConfig(
         "receivables",
         "Receivables",
         extract_names=["receivables", "rec", "accounts receivable", "ar"],
         forecast_config=ForecastItemConfig(pct_of="revenue"),
     ),
     ItemConfig(
         "inventory",
         "Inventory",
         extract_names=["inv", "inventory", "inventories"],
         forecast_config=ForecastItemConfig(pct_of="revenue"),
     ),
     ItemConfig(
-        "lt_invest",
-        "Long-Term Investments",
-        extract_names=[
-            "lt invest",
-            "lt investments",
-            "long term invest",
-            "long term investments",
-            "longterm invest",
-            "longterm investments",
-        ],
-    ),
-    ItemConfig(
         "def_tax_st",
         "Deferred Tax Assets, Current",
         extract_names=[
             "def tax asset curr",
             "deferred tax asset curr",
             "tax asset curr",
             "def tax assets curr",
@@ -104,14 +126,26 @@
             "other current asset",
             "other curr assets",
             "other curr asset",
             "oca",
         ],
     ),
     ItemConfig(
+        "total_current_assets",
+        "Total Current Assets",
+        extract_names=[
+            "total current assets",
+            "tca",
+        ],
+        expr_str="cash_and_st_invest[t] + receivables[t] + inventory[t] + def_tax_st[t] + other_current_assets[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+    ),
+    ItemConfig(
         "gross_ppe",
         "Gross Property, Plant & Equipment",
         extract_names=[
             "gross ppe",
             "gross property plant equipment",
             "gross property plant and equipment",
             "ppe gross",
@@ -136,14 +170,33 @@
             "acc depreciation",
             "accum depreciation",
             "acc dep",
             "accum dep",
         ],
     ),
     ItemConfig(
+        "net_ppe",
+        "Net Property, Plant & Equipment",
+        extract_names=[
+            "ppe",
+            "property plant equipment",
+            "property plant and equipment",
+            "ppe net",
+            "property plant equipment net",
+            "property plant and equipment net",
+            "net ppe",
+            "net property plant equipment",
+            "net property plant and equipment",
+        ],
+        expr_str="gross_ppe[t] - dep[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+    ),
+    ItemConfig(
         "goodwill",
         "Goodwill and Intangible Assets",
         extract_names=[
             "goodwill",
             "goodwill and intangible assets",
             "goodwill and intangibles",
             "goodwill intangible assets",
@@ -156,14 +209,26 @@
         ]
         # TODO [#50]: need to be able to extract from multiple items at once
         #
         # Morningstar financial statements have Goodwill and then Intangibles other than Goodwill,
         # both of those should be coming into the Goodwill and Intagible Assets variable.
     ),
     ItemConfig(
+        "lt_invest",
+        "Long-Term Investments",
+        extract_names=[
+            "lt invest",
+            "lt investments",
+            "long term invest",
+            "long term investments",
+            "longterm invest",
+            "longterm investments",
+        ],
+    ),
+    ItemConfig(
         "def_tax_lt",
         "Deferred Tax Assets, Long-Term",
         extract_names=[
             "def tax asset long term",
             "deferred tax asset long term",
             "tax asset long term",
             "def tax assets long term",
@@ -212,14 +277,39 @@
             "longterm assets other",
             "longterm asset other",
             "long term assets other",
             "long term asset other",
         ],
     ),
     ItemConfig(
+        "total_non_current_assets",
+        "Total Non-Current Assets",
+        extract_names=[
+            "total non current assets",
+            "total noncurrent assets",
+            "total lt assets",
+            "total longterm assets",
+            "total long term assets",
+        ],
+        expr_str="net_ppe[t] + goodwill[t] + lt_invest[t] + def_tax_lt[t] + other_lt_assets[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+    ),
+    ItemConfig(
+        "total_assets",
+        "Total Assets",
+        extract_names=["total assets", "total asset", "assets", "asset"],
+        expr_str="total_current_assets[t] + total_non_current_assets[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+            balance_with="total_liab_and_equity",
+        ),
+    ),
+    ItemConfig(
         "payables",
         "Payables",
         extract_names=[
             "payables",
             "accounts payable",
             "ap",
             "payables and accrued expenses",
@@ -238,14 +328,29 @@
             "payables and acc exp",
             "payable and acc exps",
             "payable and acc exp",
         ],
         forecast_config=ForecastItemConfig(pct_of="revenue"),
     ),
     ItemConfig(
+        "st_debt",
+        "Short-Term Debt",
+        extract_names=[
+            "st debt",
+            "short term debt",
+            "shortterm debt",
+            "st borrow",
+            "short term borrow",
+            "shortterm borrow" "st borrowings",
+            "short term borrowings",
+            "shortterm borrowings",
+        ],
+        forecast_config=ForecastItemConfig(pct_of="total_debt"),
+    ),
+    ItemConfig(
         "current_lt_debt",
         "Current Portion of Long-Term Debt",
         extract_names=[
             "curr port of lt debt",
             "curr port lt debt",
             "current port of lt debt",
             "current port lt debt",
@@ -293,158 +398,14 @@
             "curr part debt",
             "current part of debt",
             "current part debt",
         ],
         forecast_config=ForecastItemConfig(pct_of="total_debt"),
     ),
     ItemConfig(
-        "st_debt",
-        "Short-Term Debt",
-        extract_names=[
-            "st debt",
-            "short term debt",
-            "shortterm debt",
-            "st borrow",
-            "short term borrow",
-            "shortterm borrow" "st borrowings",
-            "short term borrowings",
-            "shortterm borrowings",
-        ],
-        forecast_config=ForecastItemConfig(pct_of="total_debt"),
-    ),
-    ItemConfig(
-        "lt_debt",
-        "Long-Term Debt",
-        extract_names=[
-            "lt debt",
-            "long term debt",
-            "longterm debt",
-            "lt borrow",
-            "long term borrow",
-            "longterm borrow",
-            "lt borrowings",
-            "long term borrowings",
-            "longterm borrowings",
-            "lt debt total",
-            "long term debt total",
-            "longterm debt total",
-            "lt borrow total",
-            "long term borrow total",
-            "longterm borrow total",
-            "lt borrowings total",
-            "long term borrowings total",
-            "longterm borrowings total",
-        ],
-        forecast_config=ForecastItemConfig(plug=True),
-    ),
-    ItemConfig(
-        "deferred_rev",
-        "Deferred Revenue",
-        extract_names=[
-            "deferred revenue",
-            "deferred sales",
-            "def revenue",
-            "def sales" "non current revenue",
-            "non current sales",
-            "non current revenue def",
-            "non current sales def",
-            "non current revenue deferred",
-            "non current sales deferred",
-            "revenue non current",
-            "sales non current",
-            "revenue def non current",
-            "sales def non current",
-            "revenue deferred non current",
-            "sales deferred non current",
-            "def revenue non current",
-            "def sales non current",
-            "def revenue def non current",
-            "def sales def non current",
-            "def revenue deferred non current",
-            "def sales deferred non current",
-            "deferred revenue non current",
-            "deferred sales non current",
-            "deferred revenue def non current",
-            "deferred sales def non current",
-            "deferred revenue deferred non current",
-            "deferred sales deferred non current",
-            "non curr revenue",
-            "non curr sales",
-            "non curr revenue def",
-            "non curr sales def",
-            "non curr revenue deferred",
-            "non curr sales deferred",
-            "revenue non curr",
-            "sales non curr",
-            "revenue def non curr",
-            "sales def non curr",
-            "revenue deferred non curr",
-            "sales deferred non curr",
-            "def revenue non curr",
-            "def sales non curr",
-            "def revenue def non curr",
-            "def sales def non curr",
-            "def revenue deferred non curr",
-            "def sales deferred non curr",
-            "deferred revenue non curr",
-            "deferred sales non curr",
-            "deferred revenue def non curr",
-            "deferred sales def non curr",
-            "deferred revenue deferred non curr",
-            "deferred sales deferred non curr" "noncurrent revenue",
-            "noncurrent sales",
-            "noncurrent revenue def",
-            "noncurrent sales def",
-            "noncurrent revenue deferred",
-            "noncurrent sales deferred",
-            "revenue noncurrent",
-            "sales noncurrent",
-            "revenue def noncurrent",
-            "sales def noncurrent",
-            "revenue deferred noncurrent",
-            "sales deferred noncurrent",
-            "def revenue noncurrent",
-            "def sales noncurrent",
-            "def revenue def noncurrent",
-            "def sales def noncurrent",
-            "def revenue deferred noncurrent",
-            "def sales deferred noncurrent",
-            "deferred revenue noncurrent",
-            "deferred sales noncurrent",
-            "deferred revenue def noncurrent",
-            "deferred sales def noncurrent",
-            "deferred revenue deferred noncurrent",
-            "deferred sales deferred noncurrent",
-            "noncurr revenue",
-            "noncurr sales",
-            "noncurr revenue def",
-            "noncurr sales def",
-            "noncurr revenue deferred",
-            "noncurr sales deferred",
-            "revenue noncurr",
-            "sales noncurr",
-            "revenue def noncurr",
-            "sales def noncurr",
-            "revenue deferred noncurr",
-            "sales deferred noncurr",
-            "def revenue noncurr",
-            "def sales noncurr",
-            "def revenue def noncurr",
-            "def sales def noncurr",
-            "def revenue deferred noncurr",
-            "def sales deferred noncurr",
-            "deferred revenue noncurr",
-            "deferred sales noncurr",
-            "deferred revenue def noncurr",
-            "deferred sales def noncurr",
-            "deferred revenue deferred noncurr",
-            "deferred sales deferred noncurr",
-        ],
-    ),
-    ItemConfig(
         "tax_liab_st",
         "Tax Liabilities, Short-Term",
         extract_names=[
             "tax liab shortterm",
             "tax liability shortterm",
             "tax liabilities shortterm",
             "tax liab short term",
@@ -583,14 +544,163 @@
             "other liabilities current",
             "other liab current",
             "other liabilities curr",
             "other liab curr",
         ],
     ),
     ItemConfig(
+        "total_current_liab",
+        "Total Current Liabilities",
+        extract_names=[
+            "total current liabilities",
+        ],
+        expr_str="payables[t] + st_debt[t] + tax_liab_st[t] + current_lt_debt[t] + other_current_liab[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+    ),
+    ItemConfig(
+        "lt_debt",
+        "Long-Term Debt",
+        extract_names=[
+            "lt debt",
+            "long term debt",
+            "longterm debt",
+            "lt borrow",
+            "long term borrow",
+            "longterm borrow",
+            "lt borrowings",
+            "long term borrowings",
+            "longterm borrowings",
+            "lt debt total",
+            "long term debt total",
+            "longterm debt total",
+            "lt borrow total",
+            "long term borrow total",
+            "longterm borrow total",
+            "lt borrowings total",
+            "long term borrowings total",
+            "longterm borrowings total",
+        ],
+        forecast_config=ForecastItemConfig(plug=True),
+    ),
+    ItemConfig(
+        "total_debt",
+        "Total Debt",
+        extract_names=["total debt"],
+        expr_str="st_debt[t] + lt_debt[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+    ),
+    ItemConfig(
+        "deferred_rev",
+        "Deferred Revenue",
+        extract_names=[
+            "deferred revenue",
+            "deferred sales",
+            "def revenue",
+            "def sales" "non current revenue",
+            "non current sales",
+            "non current revenue def",
+            "non current sales def",
+            "non current revenue deferred",
+            "non current sales deferred",
+            "revenue non current",
+            "sales non current",
+            "revenue def non current",
+            "sales def non current",
+            "revenue deferred non current",
+            "sales deferred non current",
+            "def revenue non current",
+            "def sales non current",
+            "def revenue def non current",
+            "def sales def non current",
+            "def revenue deferred non current",
+            "def sales deferred non current",
+            "deferred revenue non current",
+            "deferred sales non current",
+            "deferred revenue def non current",
+            "deferred sales def non current",
+            "deferred revenue deferred non current",
+            "deferred sales deferred non current",
+            "non curr revenue",
+            "non curr sales",
+            "non curr revenue def",
+            "non curr sales def",
+            "non curr revenue deferred",
+            "non curr sales deferred",
+            "revenue non curr",
+            "sales non curr",
+            "revenue def non curr",
+            "sales def non curr",
+            "revenue deferred non curr",
+            "sales deferred non curr",
+            "def revenue non curr",
+            "def sales non curr",
+            "def revenue def non curr",
+            "def sales def non curr",
+            "def revenue deferred non curr",
+            "def sales deferred non curr",
+            "deferred revenue non curr",
+            "deferred sales non curr",
+            "deferred revenue def non curr",
+            "deferred sales def non curr",
+            "deferred revenue deferred non curr",
+            "deferred sales deferred non curr" "noncurrent revenue",
+            "noncurrent sales",
+            "noncurrent revenue def",
+            "noncurrent sales def",
+            "noncurrent revenue deferred",
+            "noncurrent sales deferred",
+            "revenue noncurrent",
+            "sales noncurrent",
+            "revenue def noncurrent",
+            "sales def noncurrent",
+            "revenue deferred noncurrent",
+            "sales deferred noncurrent",
+            "def revenue noncurrent",
+            "def sales noncurrent",
+            "def revenue def noncurrent",
+            "def sales def noncurrent",
+            "def revenue deferred noncurrent",
+            "def sales deferred noncurrent",
+            "deferred revenue noncurrent",
+            "deferred sales noncurrent",
+            "deferred revenue def noncurrent",
+            "deferred sales def noncurrent",
+            "deferred revenue deferred noncurrent",
+            "deferred sales deferred noncurrent",
+            "noncurr revenue",
+            "noncurr sales",
+            "noncurr revenue def",
+            "noncurr sales def",
+            "noncurr revenue deferred",
+            "noncurr sales deferred",
+            "revenue noncurr",
+            "sales noncurr",
+            "revenue def noncurr",
+            "sales def noncurr",
+            "revenue deferred noncurr",
+            "sales deferred noncurr",
+            "def revenue noncurr",
+            "def sales noncurr",
+            "def revenue def noncurr",
+            "def sales def noncurr",
+            "def revenue deferred noncurr",
+            "def sales deferred noncurr",
+            "deferred revenue noncurr",
+            "deferred sales noncurr",
+            "deferred revenue def noncurr",
+            "deferred sales def noncurr",
+            "deferred revenue deferred noncurr",
+            "deferred sales deferred noncurr",
+        ],
+    ),
+    ItemConfig(
         "tax_liab_lt",
         "Tax Liabilities, Long-Term",
         extract_names=[
             "tax liab longterm",
             "tax liability longterm",
             "tax liabilities longterm",
             "tax liab long term",
@@ -825,14 +935,43 @@
             "liab noncurrent other",
             "liab non current other",
             "liab noncurr other",
             "liab non curr other",
         ],
     ),
     ItemConfig(
+        "total_non_current_liab",
+        "Total Non-Current Liabilities",
+        extract_names=[
+            "total non current liabilities",
+            "total noncurrent liabilities",
+            "total non current liability",
+            "total noncurrent liability",
+            "total non current liab",
+            "total noncurrent liab",
+        ],
+        expr_str="lt_debt[t] + deferred_rev[t] + tax_liab_lt[t] + deposit_liab[t] + other_lt_liab[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+    ),
+    ItemConfig(
+        "total_liab",
+        "Total Liabilities",
+        extract_names=[
+            "total liab",
+            "total liability",
+            "total liabilities",
+        ],
+        expr_str="total_non_current_liab[t] + total_current_liab[t]",
+        forecast_config=ForecastItemConfig(
+            make_forecast=False,
+        ),
+    ),
+    ItemConfig(
         "common_stock",
         "Common Stock",
         extract_names=[
             "total common stock",
             "total stock",
             "total common shares",
             "total shares",
@@ -852,24 +991,14 @@
             "total shares net",
             "common stock net",
             "stock net" "common shares net",
             "shares net",
         ],
     ),
     ItemConfig(
-        "minority_interest",
-        "Minority Interest",
-        extract_names=[
-            "minority interest",
-            "minority int",
-            "min int",
-            "min interest",
-        ],
-    ),
-    ItemConfig(
         "other_income",
         "Other Comprehensive Income",
         extract_names=[
             "other income",
             "other comprehensive income",
             "other comp income",
             "comp income",
@@ -896,151 +1025,22 @@
         ],
         force_positive=False,
         # TODO [#4]: forecast of retained earnings should be calculated
         #
         # Should be a calculation of retained_earnings[t-1] + net income[t] - dividends[t]
     ),
     ItemConfig(
-        "cash_and_st_invest",
-        "Cash and Short-Term Investments",
-        extract_names=[
-            "total cash st investments",
-            "total cash and st investments",
-            "total cash and shortterm investments",
-            "total cash and short term investments",
-            "total cash shortterm investments",
-            "total cash short term investments",
-            "total cash st invest",
-            "total cash and st invest",
-            "total cash and shortterm invest",
-            "total cash and short term invest",
-            "total cash shortterm invest",
-            "total cash short term invest",
-            "cash st investments",
-            "cash and st investments",
-            "cash and shortterm investments",
-            "cash and short term investments",
-            "cash shortterm investments",
-            "cash short term investments",
-            "cash st invest",
-            "cash and st invest",
-            "cash and shortterm invest",
-            "cash and short term invest",
-            "cash shortterm invest",
-            "cash short term invest",
-        ],
-        expr_str="cash[t] + st_invest[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
-    ),
-    ItemConfig(
-        "total_current_assets",
-        "Total Current Assets",
-        extract_names=[
-            "total current assets",
-            "tca",
-        ],
-        expr_str="cash_and_st_invest[t] + receivables[t] + inventory[t] + def_tax_st[t] + other_current_assets[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
-    ),
-    ItemConfig(
-        "net_ppe",
-        "Net Property, Plant & Equipment",
-        extract_names=[
-            "ppe",
-            "property plant equipment",
-            "property plant and equipment",
-            "ppe net",
-            "property plant equipment net",
-            "property plant and equipment net",
-            "net ppe",
-            "net property plant equipment",
-            "net property plant and equipment",
-        ],
-        expr_str="gross_ppe[t] - dep[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
-    ),
-    ItemConfig(
-        "total_non_current_assets",
-        "Total Non-Current Assets",
-        extract_names=[
-            "total non current assets",
-            "total noncurrent assets",
-            "total lt assets",
-            "total longterm assets",
-            "total long term assets",
-        ],
-        expr_str="net_ppe[t] + goodwill[t] + lt_invest[t] + def_tax_lt[t] + other_lt_assets[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
-    ),
-    ItemConfig(
-        "total_assets",
-        "Total Assets",
-        extract_names=["total assets", "total asset", "assets", "asset"],
-        expr_str="total_current_assets[t] + total_non_current_assets[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-            balance_with="total_liab_and_equity",
-        ),
-    ),
-    ItemConfig(
-        "total_current_liab",
-        "Total Current Liabilities",
-        extract_names=[
-            "total current liabilities",
-        ],
-        expr_str="payables[t] + st_debt[t] + tax_liab_st[t] + current_lt_debt[t] + other_current_liab[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
-    ),
-    ItemConfig(
-        "total_debt",
-        "Total Debt",
-        extract_names=["total debt"],
-        expr_str="st_debt[t] + lt_debt[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
-    ),
-    ItemConfig(
-        "total_non_current_liab",
-        "Total Non-Current Liabilities",
-        extract_names=[
-            "total non current liabilities",
-            "total noncurrent liabilities",
-            "total non current liability",
-            "total noncurrent liability",
-            "total non current liab",
-            "total noncurrent liab",
-        ],
-        expr_str="lt_debt[t] + deferred_rev[t] + tax_liab_lt[t] + deposit_liab[t] + other_lt_liab[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
-    ),
-    ItemConfig(
-        "total_liab",
-        "Total Liabilities",
+        "minority_interest",
+        "Minority Interest",
         extract_names=[
-            "total liab",
-            "total liability",
-            "total liabilities",
+            "minority interest",
+            "minority int",
+            "min int",
+            "min interest",
         ],
-        expr_str="total_non_current_liab[t] + total_current_liab[t]",
-        forecast_config=ForecastItemConfig(
-            make_forecast=False,
-        ),
     ),
     ItemConfig(
         "total_equity",
         "Total Stockholder's Equity",
         extract_names=[
             "total equity",
             "total shareholders equity",
```

### Comparing `finstmt-1.3.0/finstmt/bs/main.py` & `finstmt-1.4.0/finstmt/bs/main.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/clean/name.py` & `finstmt-1.4.0/finstmt/clean/name.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/combined/combinator.py` & `finstmt-1.4.0/finstmt/combined/combinator.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/combined/statements.py` & `finstmt-1.4.0/finstmt/combined/statements.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/config_manage/base.py` & `finstmt-1.4.0/finstmt/config_manage/base.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/config_manage/data.py` & `finstmt-1.4.0/finstmt/config_manage/data.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/config_manage/global_.py` & `finstmt-1.4.0/finstmt/config_manage/global_.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/config_manage/statement.py` & `finstmt-1.4.0/finstmt/config_manage/statement.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/config_manage/statements.py` & `finstmt-1.4.0/finstmt/config_manage/statements.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/exc.py` & `finstmt-1.4.0/finstmt/exc.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/findata/period_data.py` & `finstmt-1.4.0/finstmt/findata/period_data.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/findata/statement_item.py` & `finstmt-1.4.0/finstmt/findata/statement_item.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/findata/statementsbase.py` & `finstmt-1.4.0/finstmt/findata/statementsbase.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/forecast/config.py` & `finstmt-1.4.0/finstmt/forecast/config.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/forecast/main.py` & `finstmt-1.4.0/finstmt/forecast/main.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/forecast/models/average.py` & `finstmt-1.4.0/finstmt/forecast/models/average.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/forecast/models/base.py` & `finstmt-1.4.0/finstmt/forecast/models/base.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/forecast/models/cagr.py` & `finstmt-1.4.0/finstmt/forecast/models/cagr.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/forecast/models/chooser.py` & `finstmt-1.4.0/finstmt/forecast/models/chooser.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/forecast/models/manual.py` & `finstmt-1.4.0/finstmt/forecast/models/manual.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/forecast/models/prophet.py` & `finstmt-1.4.0/finstmt/forecast/models/prophet.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/forecast/models/recent.py` & `finstmt-1.4.0/finstmt/forecast/models/recent.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/forecast/models/trend.py` & `finstmt-1.4.0/finstmt/forecast/models/trend.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/forecast/plot.py` & `finstmt-1.4.0/finstmt/forecast/plot.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/forecast/statements.py` & `finstmt-1.4.0/finstmt/forecast/statements.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/inc/config.py` & `finstmt-1.4.0/finstmt/inc/config.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/inc/main.py` & `finstmt-1.4.0/finstmt/inc/main.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/items/config.py` & `finstmt-1.4.0/finstmt/items/config.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/loaders/capiq.py` & `finstmt-1.4.0/finstmt/loaders/capiq.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/resolver/base.py` & `finstmt-1.4.0/finstmt/resolver/base.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/resolver/forecast.py` & `finstmt-1.4.0/finstmt/resolver/forecast.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/resolver/history.py` & `finstmt-1.4.0/finstmt/resolver/history.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/finstmt/resolver/solve.py` & `finstmt-1.4.0/finstmt/resolver/solve.py`

 * *Files identical despite different names*

### Comparing `finstmt-1.3.0/pyproject.toml` & `finstmt-1.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 version = "1.2.2"
 
 [tool.setuptools]
 py-modules = ['finstmt']
 
 [tool.poetry]
 name = "finstmt"
-version = "1.3.0"
+version = "1.4.0"
 description = "Contains classes to work with financial statement data. Can calculate free cash flows and help project financial statements."
 authors = ["Nick DeRobertis <whoopnip@gmail.com>"]
 readme = "README.md"
 packages = [{include = "finstmt"}]
 license = "MIT"
 classifiers = [
     # How mature is this project? Common values are
```

### Comparing `finstmt-1.3.0/setup.py` & `finstmt-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'xlrd']
 
 extras_require = \
 {'forecast': ['prophet']}
 
 setup_kwargs = {
     'name': 'finstmt',
-    'version': '1.3.0',
+    'version': '1.4.0',
     'description': 'Contains classes to work with financial statement data. Can calculate free cash flows and help project financial statements.',
     'long_description': "\n\n[![](https://codecov.io/gh/nickderobertis/py-finstmt/branch/master/graph/badge.svg)](https://codecov.io/gh/nickderobertis/py-finstmt)\n[![PyPI](https://img.shields.io/pypi/v/finstmt)](https://pypi.org/project/finstmt/)\n![PyPI - License](https://img.shields.io/pypi/l/finstmt)\n[![Documentation](https://img.shields.io/badge/documentation-pass-green)](https://nickderobertis.github.io/py-finstmt/)\n![Tests Run on Ubuntu Python Versions](https://img.shields.io/badge/Tests%20Ubuntu%2FPython-3.8%20%7C%203.9%20%7C%203.10-blue)\n![Tests Run on Macos Python Versions](https://img.shields.io/badge/Tests%20Macos%2FPython-3.8%20%7C%203.9%20%7C%203.10-blue)\n![Tests Run on Windows Python Versions](https://img.shields.io/badge/Tests%20Windows%2FPython-3.8%20%7C%203.9%20%7C%203.10-blue)\n[![Github Repo](https://img.shields.io/badge/repo-github-informational)](https://github.com/nickderobertis/py-finstmt/)\n\n\n#  py-finstmt\n\n## Overview\n\nContains classes to work with financial statement data. Can calculate free cash flows and help project financial statements.\n\n## Getting Started\n\nInstall `finstmt`:\n\n```\npip install finstmt\n```\n\nA simple example:\n\n```python\nfrom finstmt import BalanceSheets, IncomeStatements, FinancialStatements\nimport pandas as pd\n\nbs_path = r'WMT Balance Sheet.xlsx'\ninc_path = r'WMT Income Statement.xlsx'\nbs_df = pd.read_excel(bs_path)\ninc_df = pd.read_excel(inc_path)\nbs_data = BalanceSheets.from_df(bs_df)\ninc_data = IncomeStatements.from_df(inc_df)\nstmts = FinancialStatements(inc_data, bs_data)\n```\n\nSee a\n[more in-depth tutorial here.](\nhttps://nickderobertis.github.io/py-finstmt/tutorial.html\n)\n\n## Links\n\nSee the\n[documentation here.](\nhttps://nickderobertis.github.io/py-finstmt/\n)\n\n## Development Status\n\nThis project is currently in early-stage development. There may be\nbreaking changes often. While the major version is 0, minor version\nupgrades will often have breaking changes.\n\n## Developing\n\nSee the [development guide](\nhttps://github.com/nickderobertis/py-finstmt/blob/master/DEVELOPING.md\n) for development details.\n\n## Author\n\nCreated by Nick DeRobertis. MIT License.\n\n",
     'author': 'Nick DeRobertis',
     'author_email': 'whoopnip@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `finstmt-1.3.0/PKG-INFO` & `finstmt-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finstmt
-Version: 1.3.0
+Version: 1.4.0
 Summary: Contains classes to work with financial statement data. Can calculate free cash flows and help project financial statements.
 License: MIT
 Author: Nick DeRobertis
 Author-email: whoopnip@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

