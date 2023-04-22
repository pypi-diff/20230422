# Comparing `tmp/auto-screener-0.0.4.tar.gz` & `tmp/auto-screener-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-screener-0.0.4.tar", last modified: Sat Apr 22 09:12:33 2023, max compression
+gzip compressed data, was "auto-screener-0.0.5.tar", last modified: Sat Apr 22 09:21:56 2023, max compression
```

## Comparing `auto-screener-0.0.4.tar` & `auto-screener-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 09:12:33.496573 auto-screener-0.0.4/
--rw-rw-rw-   0        0        0      115 2023-04-22 09:12:32.000000 auto-screener-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2066 2023-04-22 09:12:33.496573 auto-screener-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 09:12:33.484466 auto-screener-0.0.4/auto_screener/
--rw-rw-rw-   0        0        0      498 2023-04-21 09:31:59.000000 auto-screener-0.0.4/auto_screener/__init__.py
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.0.4/auto_screener/base.py
--rw-rw-rw-   0        0        0     5944 2023-04-22 07:38:43.000000 auto-screener-0.0.4/auto_screener/dataset.py
--rw-rw-rw-   0        0        0      526 2023-04-21 17:13:30.000000 auto-screener-0.0.4/auto_screener/document.py
--rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.0.4/auto_screener/hints.py
--rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.0.4/auto_screener/interval.py
--rw-rw-rw-   0        0        0    10013 2023-04-21 17:11:58.000000 auto-screener-0.0.4/auto_screener/progress.py
--rw-rw-rw-   0        0        0    46749 2023-04-22 09:12:28.000000 auto-screener-0.0.4/auto_screener/screening.py
--rw-rw-rw-   0        0        0     9865 2023-04-21 17:03:15.000000 auto-screener-0.0.4/auto_screener/tickers.py
-drwxrwxrwx   0        0        0        0 2023-04-22 09:12:33.495575 auto-screener-0.0.4/auto_screener.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-04-22 09:12:33.000000 auto-screener-0.0.4/auto_screener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-22 09:12:33.000000 auto-screener-0.0.4/auto_screener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 09:12:33.000000 auto-screener-0.0.4/auto_screener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 09:12:33.000000 auto-screener-0.0.4/auto_screener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-22 09:12:33.000000 auto-screener-0.0.4/auto_screener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.0.4/build.py
--rw-rw-rw-   0        0        0      645 2023-04-22 09:12:32.000000 auto-screener-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       38 2023-04-21 17:54:19.000000 auto-screener-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 09:12:33.497573 auto-screener-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1655 2023-04-22 09:12:28.000000 auto-screener-0.0.4/setup.py
--rw-rw-rw-   0        0        0     1477 2023-04-22 08:54:08.000000 auto-screener-0.0.4/test.py
+drwxrwxrwx   0        0        0        0 2023-04-22 09:21:56.818702 auto-screener-0.0.5/
+-rw-rw-rw-   0        0        0      115 2023-04-22 09:21:55.000000 auto-screener-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2066 2023-04-22 09:21:56.818702 auto-screener-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 09:21:56.804191 auto-screener-0.0.5/auto_screener/
+-rw-rw-rw-   0        0        0      498 2023-04-21 09:31:59.000000 auto-screener-0.0.5/auto_screener/__init__.py
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.0.5/auto_screener/base.py
+-rw-rw-rw-   0        0        0     5944 2023-04-22 07:38:43.000000 auto-screener-0.0.5/auto_screener/dataset.py
+-rw-rw-rw-   0        0        0      526 2023-04-21 17:13:30.000000 auto-screener-0.0.5/auto_screener/document.py
+-rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.0.5/auto_screener/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.0.5/auto_screener/interval.py
+-rw-rw-rw-   0        0        0    10013 2023-04-21 17:11:58.000000 auto-screener-0.0.5/auto_screener/progress.py
+-rw-rw-rw-   0        0        0    46642 2023-04-22 09:21:33.000000 auto-screener-0.0.5/auto_screener/screening.py
+-rw-rw-rw-   0        0        0     9865 2023-04-21 17:03:15.000000 auto-screener-0.0.5/auto_screener/tickers.py
+drwxrwxrwx   0        0        0        0 2023-04-22 09:21:56.817702 auto-screener-0.0.5/auto_screener.egg-info/
+-rw-rw-rw-   0        0        0     2066 2023-04-22 09:21:56.000000 auto-screener-0.0.5/auto_screener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-22 09:21:56.000000 auto-screener-0.0.5/auto_screener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 09:21:56.000000 auto-screener-0.0.5/auto_screener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 09:21:56.000000 auto-screener-0.0.5/auto_screener.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-22 09:21:56.000000 auto-screener-0.0.5/auto_screener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.0.5/build.py
+-rw-rw-rw-   0        0        0      645 2023-04-22 09:21:55.000000 auto-screener-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       38 2023-04-21 17:54:19.000000 auto-screener-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 09:21:56.818702 auto-screener-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1655 2023-04-22 09:21:51.000000 auto-screener-0.0.5/setup.py
+-rw-rw-rw-   0        0        0     1477 2023-04-22 08:54:08.000000 auto-screener-0.0.5/test.py
```

### Comparing `auto-screener-0.0.4/PKG-INFO` & `auto-screener-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.0.4
+Version: 0.0.5
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.0.4/README.md` & `auto-screener-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.4/auto_screener/base.py` & `auto-screener-0.0.5/auto_screener/base.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.4/auto_screener/dataset.py` & `auto-screener-0.0.5/auto_screener/dataset.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.4/auto_screener/document.py` & `auto-screener-0.0.5/auto_screener/document.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.4/auto_screener/interval.py` & `auto-screener-0.0.5/auto_screener/interval.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.4/auto_screener/progress.py` & `auto-screener-0.0.5/auto_screener/progress.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.4/auto_screener/screening.py` & `auto-screener-0.0.5/auto_screener/screening.py`

 * *Files 0% similar despite different names*

```diff
@@ -1591,18 +1591,15 @@
     def run_loop(self) -> None:
         """Runs the process of the price screening."""
 
         self.running = True
 
         while self.running:
             for screener in self.screeners:
-                threading.Thread(
-                    target=self.save_dataset,
-                    kwargs=dict(screener=screener)
-                ).start()
+                self.save_dataset(screener=screener)
             # end for
 
             delay = self.delay
 
             if isinstance(self.delay, dt.timedelta):
                 delay = delay.total_seconds()
             # end if
```

### Comparing `auto-screener-0.0.4/auto_screener/tickers.py` & `auto-screener-0.0.5/auto_screener/tickers.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.4/auto_screener.egg-info/PKG-INFO` & `auto-screener-0.0.5/auto_screener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.0.4
+Version: 0.0.5
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.0.4/build.py` & `auto-screener-0.0.5/build.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.4/pyproject.toml` & `auto-screener-0.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'auto-screener'
-version = '0.0.4'
+version = '0.0.5'
 description = 'A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `auto-screener-0.0.4/setup.py` & `auto-screener-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         include=[
             "test.py",
             "auto_screener/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='auto-screener',
-        version='0.0.4',
+        version='0.0.5',
         description=(
             "A software for automatically screening "
             "crypto exchanges for crypto pairs "
             "trading prices and rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `auto-screener-0.0.4/test.py` & `auto-screener-0.0.5/test.py`

 * *Files identical despite different names*

