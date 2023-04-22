# Comparing `tmp/astronomica-0.0.8.tar.gz` & `tmp/astronomica-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomica-0.0.8.tar", last modified: Wed Apr 12 17:34:17 2023, max compression
+gzip compressed data, was "astronomica-0.0.9.tar", last modified: Sat Apr 22 04:32:51 2023, max compression
```

## Comparing `astronomica-0.0.8.tar` & `astronomica-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:17.757548 astronomica-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-12 17:34:03.000000 astronomica-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-12 17:34:17.757548 astronomica-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-12 17:34:03.000000 astronomica-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:17.757548 astronomica-0.0.8/astronomica/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-12 17:34:03.000000 astronomica-0.0.8/astronomica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20333 2023-04-12 17:34:03.000000 astronomica-0.0.8/astronomica/astronomica.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-12 17:34:03.000000 astronomica-0.0.8/astronomica/libconversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-12 17:34:03.000000 astronomica-0.0.8/astronomica/suntiming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:17.757548 astronomica-0.0.8/astronomica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-12 17:34:17.000000 astronomica-0.0.8/astronomica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-12 17:34:17.000000 astronomica-0.0.8/astronomica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:34:17.000000 astronomica-0.0.8/astronomica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 17:34:17.000000 astronomica-0.0.8/astronomica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 17:34:17.000000 astronomica-0.0.8/astronomica.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:34:17.757548 astronomica-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-12 17:34:03.000000 astronomica-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:32:51.993679 astronomica-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-22 04:32:41.000000 astronomica-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-04-22 04:32:51.993679 astronomica-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-22 04:32:41.000000 astronomica-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:32:51.989679 astronomica-0.0.9/astronomica/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-22 04:32:41.000000 astronomica-0.0.9/astronomica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20333 2023-04-22 04:32:41.000000 astronomica-0.0.9/astronomica/astronomica.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20111 2023-04-22 04:32:41.000000 astronomica-0.0.9/astronomica/libconversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-22 04:32:41.000000 astronomica-0.0.9/astronomica/suntiming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:32:51.993679 astronomica-0.0.9/astronomica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-04-22 04:32:51.000000 astronomica-0.0.9/astronomica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-22 04:32:51.000000 astronomica-0.0.9/astronomica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:32:51.000000 astronomica-0.0.9/astronomica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-22 04:32:51.000000 astronomica-0.0.9/astronomica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-22 04:32:51.000000 astronomica-0.0.9/astronomica.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 04:32:51.993679 astronomica-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-22 04:32:41.000000 astronomica-0.0.9/setup.py
```

### Comparing `astronomica-0.0.8/LICENSE` & `astronomica-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.8/PKG-INFO` & `astronomica-0.0.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,13 @@
-Metadata-Version: 2.1
-Name: astronomica
-Version: 0.0.8
-Summary: A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates
-Home-page: https://github.com/PyndyalaCoder/astronomica
-Author: Siddhu Pendyala
-Author-email: elcientifico.pendyala@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/PyndyalaCoder/astronomica/issues
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # astronomica
 
+<img src='astronomica.png'></img>
+<h6>logo created with kittl.com</h6>
+
+[![ForTheBadge built-with-love](https://forthebadge.com//images/badges/built-with-love.svg)](https://github.com/PyndyalaCoder/)
 ## Introduction and Purpose
 The purpose of astronomica is to provide a set of tools for analyzing, generating, searching and visualizing astronomical data. This library aims to make it easy for astronomers, researchers, and students to explore and understand the universe using Python. By providing a comprehensive set of tools and a user-friendly interface, this library aims to empower astronomers and researchers to gain new insights into the universe and advance our understanding of the cosmos.
 
 ### Note of Usage:
 <b>Astronomica is 100% free</b>!! It is also <b>driven by the <i>community</i></b>, so we welcome tips, bug fixes, and more methods added by users and the general python & astronomy community. You can also join our reddit community at https://www.reddit.com/r/pythonlibraries/ 
 
 
@@ -28,17 +20,53 @@
 
 ```python
 from astronomica import *  # import all the tools offered by astronomica
 xmars, ymars, zmars = planet_heliocentric_coordinates('mars')  # get the coordinates of mars right now
 print(f"The Heliocentric Coordinates of Mars right now are: ({xmars}, {ymars}, {zmars}).")
 ```
 
+Here is another usage example: 
+
+- Astronomers need to know when astronomical night is so they can see the stars the best:
+
+```python
+# Import datetime module
+import datetime
+from astronomica import *
+
+def get_astronomical_night():
+    # Get the local sunset time as a datetime object
+    sun = Sun(47.6, -122.2)
+    sunset_time = sun.get_local_sunset_time(datetime.datetime.now())
+    print(f"The local sunset time is {sunset_time}")
+
+    # Calculate duration of the day in hours and minutes
+    day_duration = datetime.timedelta(hours=24) - datetime.timedelta(hours=sunset_time.hour, minutes=sunset_time.minute)
+    day_duration_hours, day_duration_minutes = divmod(day_duration.seconds // 60, 60)
+
+    # Calculate the duration of astronomical twilight as a timedelta object
+    twilight_duration = datetime.timedelta(minutes=day_duration.total_seconds() * 0.2666 / 60)
+
+    # Calculate the duration of astronomical night as a timedelta object
+    night_duration = day_duration - twilight_duration
+
+    # Calculate the time of astronomical night as a datetime object
+    night_time = sunset_time + night_duration
+
+    # Format the time of astronomical night as a string in the format "HH:MM"
+    night_time_str = night_time.strftime("%H:%M")
+
+    print(f"The time of astronomical night is {night_time_str}")
+
+get_astronomical_night()
+```
+
 ## Utilities: 
 astronomica provides a <b>wide</b> range of functions and tools that extend not only into astronomy, but physics and mathematics as well. Here are some of the things astronomica offers:
-- ## Trigonometry:
+- ## Mathematics:
   - astronomica provides a wide range of trigonometry functions such as sine, cosine, tangent, arcsine, arccosine, arctangent, and more. It can also calculate a nth root of a number or raise a number to the nth power.
 - ## Visualization:
   - astronomica provides visualization tools for a growing amount of astronomical data. As of Wednesday April 12th, Astronomica provides visualization for the mean anomaly of all nine planets, and more tools for plotting your own lists.
 - ## Time:
   - astronomica provides two accurate functions for getting the current date and time as an str. They can be used in advanced calculations, as they are accurate to the second. Astronomica also has functions for getting the current julian date, local sidereal time, and conversions between gregorian and julian calendars.
 - ## Astronomy:
   - astronomica provides a strong set of methods developed to make astronomy observations easier. It includes a host of general sun calculations, sunrise and set times, heliocentric coordinates (see the example), geocentric coordinates, geocentric latitude and longitude, star calculations (including the ability to map star names to their type), scraping astronomical databases for equatorial coordinates of stars, lunar phase calculation, lunar age and percent of age calculation, and finally, a method for getting the definition of a hard astronomy word.
```

### Comparing `astronomica-0.0.8/astronomica/astronomica.py` & `astronomica-0.0.9/astronomica/astronomica.py`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.8/astronomica/suntiming.py` & `astronomica-0.0.9/astronomica/suntiming.py`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.8/setup.py` & `astronomica-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='astronomica',
-    version='0.0.8',
+    version='0.0.9',
     author='Siddhu Pendyala',
     author_email='elcientifico.pendyala@gmail.com',
     description='A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates',
     long_description = long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/PyndyalaCoder/astronomica',
     project_urls = {
```

