# Comparing `tmp/czech_workdays_holidays-0.1.2.tar.gz` & `tmp/czech_workdays_holidays-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "czech_workdays_holidays-0.1.2.tar", last modified: Sat Apr 22 11:45:16 2023, max compression
+gzip compressed data, was "czech_workdays_holidays-0.1.3.tar", last modified: Sat Apr 22 12:13:51 2023, max compression
```

## Comparing `czech_workdays_holidays-0.1.2.tar` & `czech_workdays_holidays-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 11:45:16.879615 czech_workdays_holidays-0.1.2/
--rw-rw-rw-   0        0        0     1072 2023-04-21 15:08:04.000000 czech_workdays_holidays-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4742 2023-04-22 11:45:16.879615 czech_workdays_holidays-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4077 2023-04-21 22:21:46.000000 czech_workdays_holidays-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 11:45:16.877614 czech_workdays_holidays-0.1.2/czech_workdays_holidays.egg-info/
--rw-rw-rw-   0        0        0     4742 2023-04-22 11:45:16.000000 czech_workdays_holidays-0.1.2/czech_workdays_holidays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-22 11:45:16.000000 czech_workdays_holidays-0.1.2/czech_workdays_holidays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 11:45:16.000000 czech_workdays_holidays-0.1.2/czech_workdays_holidays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-22 11:45:16.000000 czech_workdays_holidays-0.1.2/czech_workdays_holidays.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-22 11:45:16.000000 czech_workdays_holidays-0.1.2/czech_workdays_holidays.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13820 2023-04-22 11:18:12.000000 czech_workdays_holidays-0.1.2/czech_workdays_holidays.py
--rw-rw-rw-   0        0        0      756 2023-04-22 10:34:23.000000 czech_workdays_holidays-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-22 11:45:16.879615 czech_workdays_holidays-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-22 11:45:16.878615 czech_workdays_holidays-0.1.2/test/
--rw-rw-rw-   0        0        0     9683 2023-04-22 11:22:55.000000 czech_workdays_holidays-0.1.2/test/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-22 12:13:51.387716 czech_workdays_holidays-0.1.3/
+-rw-rw-rw-   0        0        0     1072 2023-04-22 12:08:29.000000 czech_workdays_holidays-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     4709 2023-04-22 12:13:51.387716 czech_workdays_holidays-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4044 2023-04-22 12:11:42.000000 czech_workdays_holidays-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 12:13:51.384715 czech_workdays_holidays-0.1.3/czech_workdays_holidays.egg-info/
+-rw-rw-rw-   0        0        0     4709 2023-04-22 12:13:51.000000 czech_workdays_holidays-0.1.3/czech_workdays_holidays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-22 12:13:51.000000 czech_workdays_holidays-0.1.3/czech_workdays_holidays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 12:13:51.000000 czech_workdays_holidays-0.1.3/czech_workdays_holidays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-22 12:13:51.000000 czech_workdays_holidays-0.1.3/czech_workdays_holidays.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-22 12:13:51.000000 czech_workdays_holidays-0.1.3/czech_workdays_holidays.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13820 2023-04-22 11:18:12.000000 czech_workdays_holidays-0.1.3/czech_workdays_holidays.py
+-rw-rw-rw-   0        0        0      756 2023-04-22 12:13:42.000000 czech_workdays_holidays-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-22 12:13:51.387716 czech_workdays_holidays-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-22 12:13:51.386716 czech_workdays_holidays-0.1.3/test/
+-rw-rw-rw-   0        0        0     9683 2023-04-22 11:22:55.000000 czech_workdays_holidays-0.1.3/test/tests.py
```

### Comparing `czech_workdays_holidays-0.1.2/LICENSE` & `czech_workdays_holidays-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.1.2/PKG-INFO` & `czech_workdays_holidays-0.1.3/czech_workdays_holidays.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: czech_workdays_holidays
-Version: 0.1.2
+Name: czech-workdays-holidays
+Version: 0.1.3
 Summary: Czech Workdays, Holidays and Shopping Days
 Author-email: David Gamba <gamba.d@seznam.cz>
 Project-URL: Homepage, https://github.com/david-gamba/Czech-Working-Days
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
 
 Data are valid since 2001. If selected year before 2001, exception is raised.
 
 #### Informational sources
 [Czech holidays in English](https://en.wikipedia.org/wiki/Public_holidays_in_the_Czech_Republic)  
 [Czech holidys in Czech](https://cs.wikipedia.org/wiki/%C4%8Cesk%C3%BD_st%C3%A1tn%C3%AD_sv%C3%A1tek)
 
-#### Legislation sources
+#### Legal sources
 [Czech Holidays](https://www.zakonyprolidi.cz/cs/2000-245?text=245%2F2000)  
 [Restricted shopping days](https://www.zakonyprolidi.cz/cs/2016-223)
 
 ## Installation
 `pip install czech-workdays-holidays`
 
 ## Import
@@ -104,9 +104,9 @@
 
 #### Example
 
 ```Python
 >>> from czech_workdays_holidays import get_holidays_during_weekend
 >>> get_holidays_during_weekend(2023)
 
-[datetime.date(2023, 1, 1), datetime.date(2023, 1, 1), datetime.date(2023, 10, 28), datetime.date(2023, 12, 24)]
+[datetime.date(2023, 1, 1), datetime.date(2023, 10, 28), datetime.date(2023, 12, 24)]
 ```
```

### Comparing `czech_workdays_holidays-0.1.2/README.md` & `czech_workdays_holidays-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Data are valid since 2001. If selected year before 2001, exception is raised.
 
 #### Informational sources
 [Czech holidays in English](https://en.wikipedia.org/wiki/Public_holidays_in_the_Czech_Republic)  
 [Czech holidys in Czech](https://cs.wikipedia.org/wiki/%C4%8Cesk%C3%BD_st%C3%A1tn%C3%AD_sv%C3%A1tek)
 
-#### Legislation sources
+#### Legal sources
 [Czech Holidays](https://www.zakonyprolidi.cz/cs/2000-245?text=245%2F2000)  
 [Restricted shopping days](https://www.zakonyprolidi.cz/cs/2016-223)
 
 ## Installation
 `pip install czech-workdays-holidays`
 
 ## Import
@@ -90,9 +90,9 @@
 
 #### Example
 
 ```Python
 >>> from czech_workdays_holidays import get_holidays_during_weekend
 >>> get_holidays_during_weekend(2023)
 
-[datetime.date(2023, 1, 1), datetime.date(2023, 1, 1), datetime.date(2023, 10, 28), datetime.date(2023, 12, 24)]
+[datetime.date(2023, 1, 1), datetime.date(2023, 10, 28), datetime.date(2023, 12, 24)]
 ```
```

### Comparing `czech_workdays_holidays-0.1.2/czech_workdays_holidays.egg-info/PKG-INFO` & `czech_workdays_holidays-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: czech-workdays-holidays
-Version: 0.1.2
+Name: czech_workdays_holidays
+Version: 0.1.3
 Summary: Czech Workdays, Holidays and Shopping Days
 Author-email: David Gamba <gamba.d@seznam.cz>
 Project-URL: Homepage, https://github.com/david-gamba/Czech-Working-Days
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
 
 Data are valid since 2001. If selected year before 2001, exception is raised.
 
 #### Informational sources
 [Czech holidays in English](https://en.wikipedia.org/wiki/Public_holidays_in_the_Czech_Republic)  
 [Czech holidys in Czech](https://cs.wikipedia.org/wiki/%C4%8Cesk%C3%BD_st%C3%A1tn%C3%AD_sv%C3%A1tek)
 
-#### Legislation sources
+#### Legal sources
 [Czech Holidays](https://www.zakonyprolidi.cz/cs/2000-245?text=245%2F2000)  
 [Restricted shopping days](https://www.zakonyprolidi.cz/cs/2016-223)
 
 ## Installation
 `pip install czech-workdays-holidays`
 
 ## Import
@@ -104,9 +104,9 @@
 
 #### Example
 
 ```Python
 >>> from czech_workdays_holidays import get_holidays_during_weekend
 >>> get_holidays_during_weekend(2023)
 
-[datetime.date(2023, 1, 1), datetime.date(2023, 1, 1), datetime.date(2023, 10, 28), datetime.date(2023, 12, 24)]
+[datetime.date(2023, 1, 1), datetime.date(2023, 10, 28), datetime.date(2023, 12, 24)]
 ```
```

### Comparing `czech_workdays_holidays-0.1.2/czech_workdays_holidays.py` & `czech_workdays_holidays-0.1.3/czech_workdays_holidays.py`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.1.2/pyproject.toml` & `czech_workdays_holidays-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools >= 42.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "czech_workdays_holidays"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="David Gamba", email="gamba.d@seznam.cz" },
 ]
 description = "Czech Workdays, Holidays and Shopping Days"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `czech_workdays_holidays-0.1.2/test/tests.py` & `czech_workdays_holidays-0.1.3/test/tests.py`

 * *Files identical despite different names*

