# Comparing `tmp/czech_workdays_holidays-0.1.1.tar.gz` & `tmp/czech_workdays_holidays-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "czech_workdays_holidays-0.1.1.tar", last modified: Fri Apr 21 23:21:09 2023, max compression
+gzip compressed data, was "czech_workdays_holidays-0.1.2.tar", last modified: Sat Apr 22 11:45:16 2023, max compression
```

## Comparing `czech_workdays_holidays-0.1.1.tar` & `czech_workdays_holidays-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 23:21:09.565541 czech_workdays_holidays-0.1.1/
--rw-rw-rw-   0        0        0     1072 2023-04-21 15:08:04.000000 czech_workdays_holidays-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     4742 2023-04-21 23:21:09.565541 czech_workdays_holidays-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4077 2023-04-21 22:21:46.000000 czech_workdays_holidays-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 23:21:09.562541 czech_workdays_holidays-0.1.1/czech_workdays_holidays.egg-info/
--rw-rw-rw-   0        0        0     4742 2023-04-21 23:21:09.000000 czech_workdays_holidays-0.1.1/czech_workdays_holidays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-21 23:21:09.000000 czech_workdays_holidays-0.1.1/czech_workdays_holidays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 23:21:09.000000 czech_workdays_holidays-0.1.1/czech_workdays_holidays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-21 23:21:09.000000 czech_workdays_holidays-0.1.1/czech_workdays_holidays.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-21 23:21:09.000000 czech_workdays_holidays-0.1.1/czech_workdays_holidays.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13766 2023-04-21 23:16:45.000000 czech_workdays_holidays-0.1.1/czech_workdays_holidays.py
--rw-rw-rw-   0        0        0      756 2023-04-21 22:25:50.000000 czech_workdays_holidays-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 23:21:09.565541 czech_workdays_holidays-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 23:21:09.564541 czech_workdays_holidays-0.1.1/test/
--rw-rw-rw-   0        0        0     5239 2023-04-21 23:20:15.000000 czech_workdays_holidays-0.1.1/test/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-22 11:45:16.879615 czech_workdays_holidays-0.1.2/
+-rw-rw-rw-   0        0        0     1072 2023-04-21 15:08:04.000000 czech_workdays_holidays-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4742 2023-04-22 11:45:16.879615 czech_workdays_holidays-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4077 2023-04-21 22:21:46.000000 czech_workdays_holidays-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 11:45:16.877614 czech_workdays_holidays-0.1.2/czech_workdays_holidays.egg-info/
+-rw-rw-rw-   0        0        0     4742 2023-04-22 11:45:16.000000 czech_workdays_holidays-0.1.2/czech_workdays_holidays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-22 11:45:16.000000 czech_workdays_holidays-0.1.2/czech_workdays_holidays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 11:45:16.000000 czech_workdays_holidays-0.1.2/czech_workdays_holidays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-22 11:45:16.000000 czech_workdays_holidays-0.1.2/czech_workdays_holidays.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-22 11:45:16.000000 czech_workdays_holidays-0.1.2/czech_workdays_holidays.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13820 2023-04-22 11:18:12.000000 czech_workdays_holidays-0.1.2/czech_workdays_holidays.py
+-rw-rw-rw-   0        0        0      756 2023-04-22 10:34:23.000000 czech_workdays_holidays-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-22 11:45:16.879615 czech_workdays_holidays-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-22 11:45:16.878615 czech_workdays_holidays-0.1.2/test/
+-rw-rw-rw-   0        0        0     9683 2023-04-22 11:22:55.000000 czech_workdays_holidays-0.1.2/test/tests.py
```

### Comparing `czech_workdays_holidays-0.1.1/LICENSE` & `czech_workdays_holidays-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.1.1/PKG-INFO` & `czech_workdays_holidays-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czech_workdays_holidays
-Version: 0.1.1
+Version: 0.1.2
 Summary: Czech Workdays, Holidays and Shopping Days
 Author-email: David Gamba <gamba.d@seznam.cz>
 Project-URL: Homepage, https://github.com/david-gamba/Czech-Working-Days
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `czech_workdays_holidays-0.1.1/README.md` & `czech_workdays_holidays-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.1.1/czech_workdays_holidays.egg-info/PKG-INFO` & `czech_workdays_holidays-0.1.2/czech_workdays_holidays.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czech-workdays-holidays
-Version: 0.1.1
+Version: 0.1.2
 Summary: Czech Workdays, Holidays and Shopping Days
 Author-email: David Gamba <gamba.d@seznam.cz>
 Project-URL: Homepage, https://github.com/david-gamba/Czech-Working-Days
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `czech_workdays_holidays-0.1.1/czech_workdays_holidays.py` & `czech_workdays_holidays-0.1.2/czech_workdays_holidays.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,16 +225,17 @@
         holidays.pop(2)
 
     if shopping_restricted:
         if year < 2016:
             raise Exception("Shopping resctriction came into effect 01/10/2016 (DD/MM/YY)")
         elif year == 2016:
             # shopping restricted holidays before legslation change is filtered out
-            holidays = list(filter(lambda x:
-                                   x["shopping_restricted"] is True and x["date"] > date(2016, 10, 1), holidays))
+            holidays = list(filter(lambda holiday:
+                                   holiday["shopping_restricted"] is True and holiday["date"] > date(2016, 10, 1),
+                                   holidays))
             warn("Shopping resctriction came into effect 01/10/2016 (DD/MM/YY) thus holidays that are usually "
                  "shopping restricted are not filtered. This applies only for year 2016")
         else:
             holidays = list(filter(lambda x: x["shopping_restricted"] is True, holidays))
 
     if dates_only:
         holiday_dates = list(set(holiday["date"] for holiday in holidays))
```

### Comparing `czech_workdays_holidays-0.1.1/pyproject.toml` & `czech_workdays_holidays-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools >= 42.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "czech_workdays_holidays"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="David Gamba", email="gamba.d@seznam.cz" },
 ]
 description = "Czech Workdays, Holidays and Shopping Days"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

