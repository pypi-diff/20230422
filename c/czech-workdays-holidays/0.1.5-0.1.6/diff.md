# Comparing `tmp/czech_workdays_holidays-0.1.5.tar.gz` & `tmp/czech_workdays_holidays-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "czech_workdays_holidays-0.1.5.tar", last modified: Sat Apr 22 15:18:52 2023, max compression
+gzip compressed data, was "czech_workdays_holidays-0.1.6.tar", last modified: Sat Apr 22 15:27:50 2023, max compression
```

## Comparing `czech_workdays_holidays-0.1.5.tar` & `czech_workdays_holidays-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 15:18:52.442033 czech_workdays_holidays-0.1.5/
--rw-rw-rw-   0        0        0     1072 2023-04-22 12:08:29.000000 czech_workdays_holidays-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     4808 2023-04-22 15:18:52.442033 czech_workdays_holidays-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4140 2023-04-22 15:16:10.000000 czech_workdays_holidays-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 15:18:52.441033 czech_workdays_holidays-0.1.5/czech_workdays_holidays.egg-info/
--rw-rw-rw-   0        0        0     4808 2023-04-22 15:18:52.000000 czech_workdays_holidays-0.1.5/czech_workdays_holidays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-22 15:18:52.000000 czech_workdays_holidays-0.1.5/czech_workdays_holidays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 15:18:52.000000 czech_workdays_holidays-0.1.5/czech_workdays_holidays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-22 15:18:52.000000 czech_workdays_holidays-0.1.5/czech_workdays_holidays.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-22 15:18:52.000000 czech_workdays_holidays-0.1.5/czech_workdays_holidays.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13714 2023-04-22 13:56:56.000000 czech_workdays_holidays-0.1.5/czech_workdays_holidays.py
--rw-rw-rw-   0        0        0      756 2023-04-22 15:18:15.000000 czech_workdays_holidays-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-22 15:18:52.443536 czech_workdays_holidays-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-22 15:18:52.442033 czech_workdays_holidays-0.1.5/test/
--rw-rw-rw-   0        0        0     9683 2023-04-22 11:22:55.000000 czech_workdays_holidays-0.1.5/test/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-22 15:27:50.248507 czech_workdays_holidays-0.1.6/
+-rw-rw-rw-   0        0        0     1072 2023-04-22 12:08:29.000000 czech_workdays_holidays-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     4808 2023-04-22 15:27:50.248507 czech_workdays_holidays-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4140 2023-04-22 15:16:10.000000 czech_workdays_holidays-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 15:27:50.246507 czech_workdays_holidays-0.1.6/czech_workdays_holidays.egg-info/
+-rw-rw-rw-   0        0        0     4808 2023-04-22 15:27:50.000000 czech_workdays_holidays-0.1.6/czech_workdays_holidays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-22 15:27:50.000000 czech_workdays_holidays-0.1.6/czech_workdays_holidays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 15:27:50.000000 czech_workdays_holidays-0.1.6/czech_workdays_holidays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-22 15:27:50.000000 czech_workdays_holidays-0.1.6/czech_workdays_holidays.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-22 15:27:50.000000 czech_workdays_holidays-0.1.6/czech_workdays_holidays.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13730 2023-04-22 15:27:26.000000 czech_workdays_holidays-0.1.6/czech_workdays_holidays.py
+-rw-rw-rw-   0        0        0      756 2023-04-22 15:27:44.000000 czech_workdays_holidays-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-22 15:27:50.248507 czech_workdays_holidays-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-22 15:27:50.247508 czech_workdays_holidays-0.1.6/test/
+-rw-rw-rw-   0        0        0     9683 2023-04-22 11:22:55.000000 czech_workdays_holidays-0.1.6/test/tests.py
```

### Comparing `czech_workdays_holidays-0.1.5/LICENSE` & `czech_workdays_holidays-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.1.5/PKG-INFO` & `czech_workdays_holidays-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czech_workdays_holidays
-Version: 0.1.5
+Version: 0.1.6
 Summary: Czech Workdays, Holidays and Shopping Days
 Author-email: David Gamba <gamba.d@seznam.cz>
 Project-URL: Homepage, https://github.com/david-gamba/Czech-Working-Days
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `czech_workdays_holidays-0.1.5/README.md` & `czech_workdays_holidays-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.1.5/czech_workdays_holidays.egg-info/PKG-INFO` & `czech_workdays_holidays-0.1.6/czech_workdays_holidays.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czech-workdays-holidays
-Version: 0.1.5
+Version: 0.1.6
 Summary: Czech Workdays, Holidays and Shopping Days
 Author-email: David Gamba <gamba.d@seznam.cz>
 Project-URL: Homepage, https://github.com/david-gamba/Czech-Working-Days
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `czech_workdays_holidays-0.1.5/czech_workdays_holidays.py` & `czech_workdays_holidays-0.1.6/czech_workdays_holidays.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
             raise Exception("Shopping resctriction came into effect 01/10/2016 (DD/MM/YY)")
         elif year == 2016:
             # shopping restricted holidays before legslation change is filtered out
             holidays = list(filter(lambda holiday:
                                    holiday["shopping_restricted"] is True and holiday["date"] > date(2016, 10, 1),
                                    holidays))
             warn("Shopping resctriction came into effect 01/10/2016 (DD/MM/YY) thus holidays that are usually "
-                 "shopping restricted are not filtered. This applies only for year 2016")
+                 "shopping restricted are not filtered before this day. This applies only for year 2016")
         else:
             holidays = list(filter(lambda holiday: holiday["shopping_restricted"] is True, holidays))
 
     if dates_only:
         holiday_dates = list(set(holiday["date"] for holiday in holidays))
         return holiday_dates
```

### Comparing `czech_workdays_holidays-0.1.5/pyproject.toml` & `czech_workdays_holidays-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools >= 42.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "czech_workdays_holidays"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="David Gamba", email="gamba.d@seznam.cz" },
 ]
 description = "Czech Workdays, Holidays and Shopping Days"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `czech_workdays_holidays-0.1.5/test/tests.py` & `czech_workdays_holidays-0.1.6/test/tests.py`

 * *Files identical despite different names*

