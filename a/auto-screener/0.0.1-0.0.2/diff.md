# Comparing `tmp/auto-screener-0.0.1.tar.gz` & `tmp/auto-screener-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-screener-0.0.1.tar", last modified: Fri Apr 21 17:54:54 2023, max compression
+gzip compressed data, was "auto-screener-0.0.2.tar", last modified: Sat Apr 22 08:54:27 2023, max compression
```

## Comparing `auto-screener-0.0.1.tar` & `auto-screener-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 17:54:54.974085 auto-screener-0.0.1/
--rw-rw-rw-   0        0        0      115 2023-04-21 17:54:54.000000 auto-screener-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2066 2023-04-21 17:54:54.973084 auto-screener-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 17:54:54.957548 auto-screener-0.0.1/auto_screener/
--rw-rw-rw-   0        0        0      498 2023-04-21 09:31:59.000000 auto-screener-0.0.1/auto_screener/__init__.py
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.0.1/auto_screener/base.py
--rw-rw-rw-   0        0        0     5939 2023-04-21 16:52:25.000000 auto-screener-0.0.1/auto_screener/dataset.py
--rw-rw-rw-   0        0        0      526 2023-04-21 17:13:30.000000 auto-screener-0.0.1/auto_screener/document.py
--rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.0.1/auto_screener/hints.py
--rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.0.1/auto_screener/interval.py
--rw-rw-rw-   0        0        0    10013 2023-04-21 17:11:58.000000 auto-screener-0.0.1/auto_screener/progress.py
--rw-rw-rw-   0        0        0    44904 2023-04-21 17:25:39.000000 auto-screener-0.0.1/auto_screener/screening.py
--rw-rw-rw-   0        0        0     9865 2023-04-21 17:03:15.000000 auto-screener-0.0.1/auto_screener/tickers.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:54:54.973084 auto-screener-0.0.1/auto_screener.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-04-21 17:54:54.000000 auto-screener-0.0.1/auto_screener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-21 17:54:54.000000 auto-screener-0.0.1/auto_screener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 17:54:54.000000 auto-screener-0.0.1/auto_screener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 17:54:54.000000 auto-screener-0.0.1/auto_screener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-21 17:54:54.000000 auto-screener-0.0.1/auto_screener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.0.1/build.py
--rw-rw-rw-   0        0        0      645 2023-04-21 17:54:54.000000 auto-screener-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       38 2023-04-21 17:54:19.000000 auto-screener-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 17:54:54.974085 auto-screener-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1655 2023-04-21 17:54:48.000000 auto-screener-0.0.1/setup.py
--rw-rw-rw-   0        0        0     1497 2023-04-21 17:37:38.000000 auto-screener-0.0.1/test.py
+drwxrwxrwx   0        0        0        0 2023-04-22 08:54:27.022362 auto-screener-0.0.2/
+-rw-rw-rw-   0        0        0      115 2023-04-22 08:54:26.000000 auto-screener-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2066 2023-04-22 08:54:27.022362 auto-screener-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 08:54:27.007361 auto-screener-0.0.2/auto_screener/
+-rw-rw-rw-   0        0        0      498 2023-04-21 09:31:59.000000 auto-screener-0.0.2/auto_screener/__init__.py
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.0.2/auto_screener/base.py
+-rw-rw-rw-   0        0        0     5944 2023-04-22 07:38:43.000000 auto-screener-0.0.2/auto_screener/dataset.py
+-rw-rw-rw-   0        0        0      526 2023-04-21 17:13:30.000000 auto-screener-0.0.2/auto_screener/document.py
+-rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.0.2/auto_screener/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.0.2/auto_screener/interval.py
+-rw-rw-rw-   0        0        0    10013 2023-04-21 17:11:58.000000 auto-screener-0.0.2/auto_screener/progress.py
+-rw-rw-rw-   0        0        0    46058 2023-04-22 08:52:43.000000 auto-screener-0.0.2/auto_screener/screening.py
+-rw-rw-rw-   0        0        0     9865 2023-04-21 17:03:15.000000 auto-screener-0.0.2/auto_screener/tickers.py
+drwxrwxrwx   0        0        0        0 2023-04-22 08:54:27.021392 auto-screener-0.0.2/auto_screener.egg-info/
+-rw-rw-rw-   0        0        0     2066 2023-04-22 08:54:26.000000 auto-screener-0.0.2/auto_screener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-22 08:54:26.000000 auto-screener-0.0.2/auto_screener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 08:54:26.000000 auto-screener-0.0.2/auto_screener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 08:54:26.000000 auto-screener-0.0.2/auto_screener.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-22 08:54:26.000000 auto-screener-0.0.2/auto_screener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.0.2/build.py
+-rw-rw-rw-   0        0        0      645 2023-04-22 08:54:26.000000 auto-screener-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       38 2023-04-21 17:54:19.000000 auto-screener-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 08:54:27.022362 auto-screener-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1655 2023-04-22 08:54:23.000000 auto-screener-0.0.2/setup.py
+-rw-rw-rw-   0        0        0     1477 2023-04-22 08:54:08.000000 auto-screener-0.0.2/test.py
```

### Comparing `auto-screener-0.0.1/PKG-INFO` & `auto-screener-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.0.1
+Version: 0.0.2
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.0.1/README.md` & `auto-screener-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.1/auto_screener/base.py` & `auto-screener-0.0.2/auto_screener/base.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.1/auto_screener/dataset.py` & `auto-screener-0.0.2/auto_screener/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     elif isinstance(dataset, pd.Series):
         return pd.DataFrame(
             {
                 column: [value] for column, value in
                 dict(dataset).items()
             },
-            index=[index]
+            index=[index or 0]
         )
 
     else:
         raise TypeError(
             f"Dataset must be either of type {pd.DataFrame}, "
             f"or {pd.Series}, not {type(dataset)}."
         )
```

### Comparing `auto-screener-0.0.1/auto_screener/document.py` & `auto-screener-0.0.2/auto_screener/document.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.1/auto_screener/interval.py` & `auto-screener-0.0.2/auto_screener/interval.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.1/auto_screener/progress.py` & `auto-screener-0.0.2/auto_screener/progress.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.1/auto_screener/screening.py` & `auto-screener-0.0.2/auto_screener/screening.py`

 * *Files 3% similar despite different names*

```diff
@@ -193,14 +193,18 @@
         :param timeout: The valur to add a timeout to the process.
         """
 
         self.screening_process = threading.Thread(target=self.run_loop)
 
         self.screening_process.start()
 
+        if timeout:
+            self.timeout(timeout)
+        # end if
+
         if block:
             self.block = block
 
             while self.blocking():
                 pass
             # end while
         # end if
@@ -216,20 +220,15 @@
         if isinstance(wait, bool) and wait:
             self.wait_for_initialization()
 
         elif isinstance(wait, (int, float)):
             time.sleep(wait)
         # end if
 
-        if timeout:
-            return self.timeout(timeout)
-
-        else:
-            return self.screening_process
-        # end if
+        return self.screening_process
     # end run
 
     def timeout(
             self, duration: Union[Number, dt.timedelta, dt.datetime]
     ) -> threading.Thread:
         """
         Runs a timeout for the process.
@@ -326,15 +325,15 @@
         ):
             raise ValueError(f"Cannot extract data from {source}.")
         # end if
 
         if not screener.TICKERS.setdefault(source, []):
             try:
                 screener.TICKERS[source] = list(
-                    getattr(ccxt, source)().fetch_tickers().keys()
+                    getattr(ccxt, source)().load_markets().keys()
                 )
 
             except Exception as e:
                 raise ValueError(
                     f"Cannot fetch tickers from {source}. {e}"
                 )
             # end try
@@ -605,17 +604,15 @@
         delay = self.delay
 
         if isinstance(delay, dt.timedelta):
             delay = delay.total_seconds()
         # end if
 
         while self.running:
-            if delay:
-                time.sleep(delay)
-            # end if
+            start = time.time()
 
             try:
                 data = await self.async_get_market()
 
             except Exception as e:
                 self.terminate()
 
@@ -629,14 +626,20 @@
                     [int(time.time() * 1000)], unit="ms"
                 )
             )
             new_data.index.name = DATE_TIME
 
             self.market = pd.concat([self.market, new_data])
             self.market.index.name = DATE_TIME
+
+            end = time.time()
+
+            if delay:
+                time.sleep(max([delay - (end - start), 0]))
+            # end if
         # end while
     # end async_run
 
     async def async_run(self) -> None:
         """Runs the processes of price screening."""
 
         task = self.async_run_loop()
@@ -748,15 +751,15 @@
     def __init__(
             self,
             ticker: str,
             source: str,
             interval: str,
             pro: Optional[bool] = True,
             data: Optional[pd.DataFrame] = None,
-            length: Optional[int] = None,
+            length: Optional[Union[bool, int]] = None,
             delay: Optional[Union[Number, dt.timedelta]] = None,
             screener: Optional[AutoScreener] = None,
             options: Optional[Dict[str, Any]] = None
     ) -> None:
         """
         Defines the class attributes.
 
@@ -788,18 +791,16 @@
         )
 
         if self.screener_key not in self.screeners:
             if screener is None:
                 self.built = True
 
                 screener = AutoScreener(
-                    ticker=self.ticker,
-                    source=self.source,
-                    delay=self.delay,
-                    pro=self.pro,
+                    ticker=self.ticker, source=self.source,
+                    delay=self.delay, pro=self.pro,
                     options=self.options
                 )
             # end if
 
             self.screeners[self.screener_key] = screener
         # end if
 
@@ -860,22 +861,24 @@
             raise AttributeError(
                 "Source and interval attributes must be defined "
                 "before attempting to validate the data parameter data."
             )
         # end if
 
         if (
-                (data is None) and
+            (data is None) and
+            (
+                (length is None) or
+                (length == 0) or
+                (length is False) or
                 (
-                        (length is None) or
-                        (
-                                isinstance(length, int) and
-                                (not (0 < length <= 500))
-                        )
+                    isinstance(length, int) and
+                    not (0 < length <= 500)
                 )
+            )
         ):
             data = pd.DataFrame(
                 {column: [] for column in self.COLUMNS},
                 index=[]
             )
 
         elif (data is None) and (isinstance(length, int)):
@@ -912,20 +915,26 @@
         data = ohlcv_to_dataset(data=data)
 
         if len(self.screener.market) == 0:
             asks = [np.nan] * len(data)
             bids = [np.nan] * len(data)
 
         else:
-            asks = self.screener.market[AutoScreener.ASKS][-len(data):]
-            bids = self.screener.market[AutoScreener.BIDS][-len(data):]
+            asks = (
+                self.screener.market[AutoScreener.ASKS].iloc
+                [-len(data):].values[:]
+            )
+            bids = (
+                self.screener.market[AutoScreener.BIDS].iloc
+                [-len(data):].values[:]
+            )
         # end if
 
-        data[AutoScreener.ASKS] = asks
-        data[AutoScreener.BIDS] = bids
+        data[AutoScreener.ASKS].values[:] = asks
+        data[AutoScreener.BIDS].values[:] = bids
 
         return data[list(self.COLUMNS)]
     # end data_to_dataset
 
     def run(
             self,
             wait: Optional[Union[bool, Number, dt.timedelta, dt.datetime]] = False,
@@ -948,32 +957,44 @@
     # end run
 
     def run_loop(self) -> None:
         """Runs the process of the price screening."""
 
         self.running = True
 
+        delay = interval_to_total_time(self.interval).seconds
+
         while self.running:
-            prices = row_to_dataset(
-                self.screener.market.iloc[-1]
-            )
+            start = time.time()
+
+            data = row_to_dataset(self.screener.market, index=-1)
+
+            # noinspection PyBroadException
+            try:
+                prices = self.validate_data(data=None, length=1)
+                prices[AutoScreener.BIDS].values[:] = (
+                    data[AutoScreener.BIDS].values[:]
+                )
+                prices[AutoScreener.ASKS].values[:] = (
+                    data[AutoScreener.ASKS].values[:]
+                )
+                data = prices
 
-            data = self.validate_data(data=None, length=1)
+            except Exception:
+                pass
+            # end try
 
-            data[BIDS] = prices[BIDS]
-            data[ASKS] = prices[ASKS]
+            end = time.time()
 
             self.market = pd.concat([self.market, data])
             self.market = self.market[
                 ~self.market.index.duplicated(keep='first')
             ]
 
-            time.sleep(
-                interval_to_total_time(self.interval).seconds
-            )
+            time.sleep(max([delay - (end - start), 0]))
         # end while
     # end run_loop
 
     def terminate(self) -> None:
         """Stops the trading process."""
 
         super().terminate()
@@ -1191,23 +1212,22 @@
             "timeout_process", "screeners"
         ]
     )
 
     LOCATION = "datasets"
     INTERVAL = "1m"
 
-    LENGTH = 500
     DELAY = 1
 
     def __init__(
             self,
             exchanges: Dict[str, Iterable[str]],
             delay: Optional[Union[Number, dt.timedelta]] = None,
-            interval: Optional[str] = None,
-            length: Optional[int] = None,
+            interval: Optional[Union[bool, str]] = None,
+            length: Optional[Union[int, bool]] = None,
             location: Optional[str] = None,
             pro: Optional[bool] = False,
             options: Optional[Dict[str, Any]] = None
     ) -> None:
         """
         Defines the class attributes.
 
@@ -1229,25 +1249,26 @@
 
         self.options = options or {}
 
         self.interval = interval
         self.location = location or self.LOCATION
 
         self.delay = delay or self.DELAY
-        self.length = length or self.LENGTH
+        self.length = length
 
         self.pro = pro
 
         self.exchanges = self.validate_exchanges(exchanges)
 
         self.running = False
         self.block = False
         self.saving = False
 
         self.market: Dict[str, Dict[str, Optional[AutoDataCollector]]] = {}
+        self.invalid: Dict[str, List[str]] = {}
         self.screeners: List[AutoDataCollector] = []
 
         self.saving_process = None
         self.timeout_process = None
     # end Screener
 
     @staticmethod
@@ -1337,14 +1358,16 @@
                     ticker=ticker, source=source, options=self.options,
                     pro=self.pro, delay=self.delay
                 )
             # end if
 
         except ValueError:
             container[ticker] = None
+
+            self.invalid.setdefault(source, []).append(ticker)
         # end try
     # end create_screener
 
     @staticmethod
     def configure_screener_dataset(
             screener: AutoDataCollector, path: str, length: Optional[int] = None
     ) -> None:
@@ -1362,15 +1385,17 @@
         else:
             if isinstance(screener, AutoDataset):
                 screener.market = screener.validate_data(
                     data=None, length=length
                 )
             # end if
 
-            save_dataset(dataset=screener.market, path=path)
+            if len(screener.market) > 0:
+                save_dataset(dataset=screener.market, path=path)
+            # end if
         # end if
     # end configure_screener_dataset
 
     def wait_for_initialization(
             self,
             delay: Optional[Union[Number, dt.timedelta]] = None,
             once: Optional[bool] = False,
@@ -1383,15 +1408,20 @@
         :param once: The value to get data only once.
         :param stop: The value to stop the screener objects.
 
         :returns: The total delay.
         """
 
         return wait_for_initialization(
-            *self.screeners, delay=delay, once=once, stop=stop
+            *[
+                screener.screener
+                if isinstance(screener, AutoDataset)
+                else screener
+                for screener in self.screeners
+            ], delay=delay, once=once, stop=stop
         )
     # end wait_for_initialization
 
     def wait_for_update(
             self,
             delay: Optional[Union[Number, dt.timedelta]] = None,
             once: Optional[bool] = False,
@@ -1437,17 +1467,20 @@
         ):
             time.sleep(3)
         # end while
 
         self.screeners.clear()
 
         for exchange in self.market.values():
-            for screener in exchange.values():
+            for ticker, screener in exchange.copy().items():
                 if isinstance(screener, (AutoScreener, AutoDataset)):
                     self.screeners.append(screener)
+
+                else:
+                    exchange.pop(ticker)
                 # end if
             # end for
         # end for
     # end initialize_screeners
 
     def prepare_screeners(self) -> None:
         """Initializes the screeners."""
@@ -1548,17 +1581,21 @@
             for screener in self.screeners:
                 threading.Thread(
                     target=self.save_dataset,
                     kwargs=dict(screener=screener)
                 ).start()
             # end for
 
-            time.sleep(
-                interval_to_total_time(self.interval).seconds * 0.75
-            )
+            delay = self.delay
+
+            if isinstance(self.delay, dt.timedelta):
+                delay = delay.total_seconds()
+            # end if
+
+            time.sleep(delay or 1)
         # end while
     # end run_loop
 
     def timeout(
             self, duration: Union[Number, dt.timedelta, dt.datetime]
     ) -> threading.Thread:
         """
@@ -1608,23 +1645,24 @@
             self.saving_process = threading.Thread(
                 target=self.run_loop
             )
 
             self.saving_process.start()
         # end if
 
+        if timeout:
+            self.timeout(timeout)
+        # end if
+
         if block:
             self.block = block
 
-            while self.blocking():
+            while self.blocking() and self.running:
                 pass
             # end while
         # end if
 
-        if timeout:
-            return self.timeout(timeout)
-
-        elif save:
+        if save:
             return self.saving_process
         # end if
     # end run
 # end Screener
```

### Comparing `auto-screener-0.0.1/auto_screener/tickers.py` & `auto-screener-0.0.2/auto_screener/tickers.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.1/auto_screener.egg-info/PKG-INFO` & `auto-screener-0.0.2/auto_screener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.0.1
+Version: 0.0.2
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.0.1/build.py` & `auto-screener-0.0.2/build.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.1/pyproject.toml` & `auto-screener-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'auto-screener'
-version = '0.0.1'
+version = '0.0.2'
 description = 'A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `auto-screener-0.0.1/setup.py` & `auto-screener-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         include=[
             "test.py",
             "auto_screener/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='auto-screener',
-        version='0.0.1',
+        version='0.0.2',
         description=(
             "A software for automatically screening "
             "crypto exchanges for crypto pairs "
             "trading prices and rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `auto-screener-0.0.1/test.py` & `auto-screener-0.0.2/test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 # test.py
 
 from auto_screener.screening import MultiScreener
 from auto_screener.screening import collect_exchanges
 from auto_screener.progress import Spinner
 
-WINDOW = 30
-THRESHOLD = 0.5
-PROFIT = 0.001
-
 MATCHES = [("USD", "USDT")]
 
 ASSETS = [
     "GRT", "FIL", "ETH", "BTC", "AAVE", "AVAX",
     "LTC", "EOS", "NEAR", "APE", "MATIC", "XTZ",
     "DAI", "ADA", "KSM", "DOT", "DOGE", "XLM"
 ]
@@ -21,14 +17,15 @@
     "USD": ASSETS,
     "EUR": ASSETS
 }
 
 CURRENCIES = {
     "bittrex": ["USDT", "USD", "EUR"],
     "kraken": ["USDT", "EUR"],
+    "binance": ["USDT", "EUR"],
     "kucoin": ["USDT", "EUR"]
 }
 
 EXCLUDED = {
     "bittrex": [
         "NEAR/USD", "NEAR/USDT"
     ],
@@ -38,19 +35,18 @@
         "XLM/USDT", "NEAR/USDT"
     ],
     "kucoin": [
         "DAI/USDT"
     ]
 }
 
-LENGTH = 60
+LENGTH = 0
 DELAY = 1
-PORT = 5555
 
-PRO = False
+PRO = True
 
 INTERVAL = "1m"
 LOCATION = "datasets"
 
 def main() -> None:
     """Runs the program to test the module."""
 
@@ -65,13 +61,13 @@
         pro=PRO, interval=INTERVAL
     )
 
     with Spinner(message='Initializing Screeners'):
         screener.initialize_screeners()
     # end Spinner
 
-    screener.run()
+    screener.run(block=True)
 # end main
 
 if __name__ == "__main__":
     main()
 # end if
```

