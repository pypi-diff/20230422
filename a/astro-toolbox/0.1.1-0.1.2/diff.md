# Comparing `tmp/astro-toolbox-0.1.1.tar.gz` & `tmp/astro-toolbox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-toolbox-0.1.1.tar", last modified: Wed Apr 19 18:57:26 2023, max compression
+gzip compressed data, was "astro-toolbox-0.1.2.tar", last modified: Sat Apr 22 12:38:27 2023, max compression
```

## Comparing `astro-toolbox-0.1.1.tar` & `astro-toolbox-0.1.2.tar`

### file list

```diff
@@ -1,72 +1,69 @@
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.868938 astro-toolbox-0.1.1/
--rw-r--r--   0 romain     (501) staff       (20)    35160 2023-02-26 19:51:45.000000 astro-toolbox-0.1.1/LICENSE
--rw-r--r--   0 romain     (501) staff       (20)     4669 2023-04-19 18:57:26.869075 astro-toolbox-0.1.1/PKG-INFO
--rw-r--r--   0 romain     (501) staff       (20)     3847 2023-04-18 16:51:39.000000 astro-toolbox-0.1.1/README.md
--rw-r--r--   0 romain     (501) staff       (20)     1422 2023-04-19 18:57:26.869450 astro-toolbox-0.1.1/setup.cfg
--rw-r--r--   0 romain     (501) staff       (20)       68 2023-01-06 19:50:39.000000 astro-toolbox-0.1.1/setup.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.854486 astro-toolbox-0.1.1/src/
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.856502 astro-toolbox-0.1.1/src/astro_toolbox/
--rw-r--r--   0 romain     (501) staff       (20)      968 2023-04-19 18:42:22.000000 astro-toolbox-0.1.1/src/astro_toolbox/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)       88 2023-02-07 20:30:19.000000 astro-toolbox-0.1.1/src/astro_toolbox/__main__.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.858699 astro-toolbox-0.1.1/src/astro_toolbox/angle/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-0.1.1/src/astro_toolbox/angle/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     2170 2023-03-10 13:03:07.000000 astro-toolbox-0.1.1/src/astro_toolbox/angle/degrees.py
--rw-r--r--   0 romain     (501) staff       (20)     1665 2023-03-10 13:01:21.000000 astro-toolbox-0.1.1/src/astro_toolbox/angle/dms.py
--rw-r--r--   0 romain     (501) staff       (20)     1579 2023-03-10 13:04:29.000000 astro-toolbox-0.1.1/src/astro_toolbox/angle/hms.py
--rw-r--r--   0 romain     (501) staff       (20)     2230 2023-03-10 13:06:25.000000 astro-toolbox-0.1.1/src/astro_toolbox/angle/radians.py
--rw-r--r--   0 romain     (501) staff       (20)    12587 2023-04-18 18:49:19.000000 astro-toolbox-0.1.1/src/astro_toolbox/command_line.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.859502 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/__init__.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.859976 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/data/
--rw-r--r--   0 romain     (501) staff       (20)     2451 2023-02-02 19:46:48.000000 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/data/orbital_elements.json
--rw-r--r--   0 romain     (501) staff       (20)      419 2023-04-17 18:44:34.000000 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/data/sites.json
--rw-r--r--   0 romain     (501) staff       (20)     8253 2023-03-10 13:34:41.000000 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/equatorial.py
--rw-r--r--   0 romain     (501) staff       (20)     3299 2023-03-10 13:34:22.000000 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/horizontal.py
--rw-r--r--   0 romain     (501) staff       (20)     6995 2023-04-19 18:56:14.000000 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/location.py
--rw-r--r--   0 romain     (501) staff       (20)    11831 2023-03-10 13:22:52.000000 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/solar_system.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.860719 astro-toolbox-0.1.1/src/astro_toolbox/query/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-08 12:07:57.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     2415 2023-03-10 13:41:22.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/catalogs.py
--rw-r--r--   0 romain     (501) staff       (20)     3925 2023-04-17 19:20:22.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/ephemeris.py
--rw-r--r--   0 romain     (501) staff       (20)    10477 2023-04-19 18:55:51.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.867456 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/
--rw-r--r--   0 romain     (501) staff       (20)      457 2023-04-17 20:13:59.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/cloudy.png
--rw-r--r--   0 romain     (501) staff       (20)      200 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_down.png
--rw-r--r--   0 romain     (501) staff       (20)      193 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_down_left.png
--rw-r--r--   0 romain     (501) staff       (20)      220 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_down_right.png
--rw-r--r--   0 romain     (501) staff       (20)      256 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_left.png
--rw-r--r--   0 romain     (501) staff       (20)      215 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_right.png
--rw-r--r--   0 romain     (501) staff       (20)      270 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_up.png
--rw-r--r--   0 romain     (501) staff       (20)      243 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_up_left.png
--rw-r--r--   0 romain     (501) staff       (20)      228 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_up_right.png
--rw-r--r--   0 romain     (501) staff       (20)      519 2023-04-17 20:23:18.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/drizzle.png
--rw-r--r--   0 romain     (501) staff       (20)      388 2023-04-17 20:22:30.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/fog.png
--rw-r--r--   0 romain     (501) staff       (20)      470 2023-04-17 21:01:44.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/haze.png
--rw-r--r--   0 romain     (501) staff       (20)      613 2023-04-18 05:58:24.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/mainly_clear.png
--rw-r--r--   0 romain     (501) staff       (20)      329 2023-04-17 20:17:22.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/na.png
--rw-r--r--   0 romain     (501) staff       (20)      467 2023-04-17 21:07:00.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/partly_cloudy.png
--rw-r--r--   0 romain     (501) staff       (20)      555 2023-04-17 20:23:54.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/rain.png
--rw-r--r--   0 romain     (501) staff       (20)      545 2023-04-17 21:14:52.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/rain_mix.png
--rw-r--r--   0 romain     (501) staff       (20)      410 2023-04-17 20:21:39.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/sandstorm.png
--rw-r--r--   0 romain     (501) staff       (20)      525 2023-04-17 20:25:57.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/showers.png
--rw-r--r--   0 romain     (501) staff       (20)      504 2023-04-17 20:24:39.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/snow.png
--rw-r--r--   0 romain     (501) staff       (20)      504 2023-04-17 15:03:01.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/sunny.png
--rw-r--r--   0 romain     (501) staff       (20)      576 2023-04-17 21:16:48.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/thunderstorm.png
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.868183 astro-toolbox-0.1.1/src/astro_toolbox/scripts/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-17 20:03:46.000000 astro-toolbox-0.1.1/src/astro_toolbox/scripts/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     1780 2023-02-08 13:53:17.000000 astro-toolbox-0.1.1/src/astro_toolbox/scripts/planning.py
--rw-r--r--   0 romain     (501) staff       (20)    17118 2023-04-18 14:18:07.000000 astro-toolbox-0.1.1/src/astro_toolbox/scripts/plots.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.868474 astro-toolbox-0.1.1/src/astro_toolbox/time/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:53:46.000000 astro-toolbox-0.1.1/src/astro_toolbox/time/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     6330 2023-04-17 16:55:55.000000 astro-toolbox-0.1.1/src/astro_toolbox/time/core.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.868808 astro-toolbox-0.1.1/src/astro_toolbox/utils/
--rw-r--r--   0 romain     (501) staff       (20)      441 2023-02-08 13:53:35.000000 astro-toolbox-0.1.1/src/astro_toolbox/utils/python_functions.py
--rw-r--r--   0 romain     (501) staff       (20)      659 2023-04-17 16:11:48.000000 astro-toolbox-0.1.1/src/astro_toolbox/utils/strparser.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.857816 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/
--rw-r--r--   0 romain     (501) staff       (20)     4669 2023-04-19 18:57:26.000000 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 romain     (501) staff       (20)     2480 2023-04-19 18:57:26.000000 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 romain     (501) staff       (20)        1 2023-04-19 18:57:26.000000 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 romain     (501) staff       (20)       62 2023-04-19 18:57:26.000000 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 romain     (501) staff       (20)        1 2023-01-18 11:00:43.000000 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/not-zip-safe
--rw-r--r--   0 romain     (501) staff       (20)      152 2023-04-19 18:57:26.000000 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/requires.txt
--rw-r--r--   0 romain     (501) staff       (20)       14 2023-04-19 18:57:26.000000 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-22 12:38:27.915777 astro-toolbox-0.1.2/
+-rw-r--r--   0 romain     (501) staff       (20)    35160 2023-02-26 19:51:45.000000 astro-toolbox-0.1.2/LICENSE
+-rw-r--r--   0 romain     (501) staff       (20)     4754 2023-04-22 12:38:27.915861 astro-toolbox-0.1.2/PKG-INFO
+-rw-r--r--   0 romain     (501) staff       (20)     3932 2023-04-22 11:23:31.000000 astro-toolbox-0.1.2/README.md
+-rw-r--r--   0 romain     (501) staff       (20)     1422 2023-04-22 12:38:27.916190 astro-toolbox-0.1.2/setup.cfg
+-rw-r--r--   0 romain     (501) staff       (20)       68 2023-01-06 19:50:39.000000 astro-toolbox-0.1.2/setup.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-22 12:38:27.895796 astro-toolbox-0.1.2/src/
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-22 12:38:27.899059 astro-toolbox-0.1.2/src/astro_toolbox/
+-rw-r--r--   0 romain     (501) staff       (20)      968 2023-04-22 12:32:21.000000 astro-toolbox-0.1.2/src/astro_toolbox/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)       88 2023-02-07 20:30:19.000000 astro-toolbox-0.1.2/src/astro_toolbox/__main__.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-22 12:38:27.902119 astro-toolbox-0.1.2/src/astro_toolbox/angle/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-0.1.2/src/astro_toolbox/angle/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     2170 2023-03-10 13:03:07.000000 astro-toolbox-0.1.2/src/astro_toolbox/angle/degrees.py
+-rw-r--r--   0 romain     (501) staff       (20)     1665 2023-03-10 13:01:21.000000 astro-toolbox-0.1.2/src/astro_toolbox/angle/dms.py
+-rw-r--r--   0 romain     (501) staff       (20)     1579 2023-03-10 13:04:29.000000 astro-toolbox-0.1.2/src/astro_toolbox/angle/hms.py
+-rw-r--r--   0 romain     (501) staff       (20)     2230 2023-03-10 13:06:25.000000 astro-toolbox-0.1.2/src/astro_toolbox/angle/radians.py
+-rw-r--r--   0 romain     (501) staff       (20)    14631 2023-04-22 12:31:41.000000 astro-toolbox-0.1.2/src/astro_toolbox/command_line.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-22 12:38:27.903707 astro-toolbox-0.1.2/src/astro_toolbox/coordinates/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-0.1.2/src/astro_toolbox/coordinates/__init__.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-22 12:38:27.904439 astro-toolbox-0.1.2/src/astro_toolbox/coordinates/data/
+-rw-r--r--   0 romain     (501) staff       (20)     2451 2023-02-02 19:46:48.000000 astro-toolbox-0.1.2/src/astro_toolbox/coordinates/data/orbital_elements.json
+-rw-r--r--   0 romain     (501) staff       (20)      419 2023-04-17 18:44:34.000000 astro-toolbox-0.1.2/src/astro_toolbox/coordinates/data/sites.json
+-rw-r--r--   0 romain     (501) staff       (20)     8253 2023-03-10 13:34:41.000000 astro-toolbox-0.1.2/src/astro_toolbox/coordinates/equatorial.py
+-rw-r--r--   0 romain     (501) staff       (20)     3299 2023-03-10 13:34:22.000000 astro-toolbox-0.1.2/src/astro_toolbox/coordinates/horizontal.py
+-rw-r--r--   0 romain     (501) staff       (20)     6925 2023-04-22 11:14:48.000000 astro-toolbox-0.1.2/src/astro_toolbox/coordinates/location.py
+-rw-r--r--   0 romain     (501) staff       (20)    11831 2023-03-10 13:22:52.000000 astro-toolbox-0.1.2/src/astro_toolbox/coordinates/solar_system.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-22 12:38:27.905676 astro-toolbox-0.1.2/src/astro_toolbox/query/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-08 12:07:57.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     2415 2023-03-10 13:41:22.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/catalogs.py
+-rw-r--r--   0 romain     (501) staff       (20)     3925 2023-04-17 19:20:22.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/ephemeris.py
+-rw-r--r--   0 romain     (501) staff       (20)     9976 2023-04-22 11:42:30.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-22 12:38:27.912949 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/
+-rw-r--r--   0 romain     (501) staff       (20)      457 2023-04-17 20:13:59.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/cloudy.png
+-rw-r--r--   0 romain     (501) staff       (20)      200 2023-04-17 18:29:15.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/direction_down.png
+-rw-r--r--   0 romain     (501) staff       (20)      193 2023-04-17 18:29:15.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/direction_down_left.png
+-rw-r--r--   0 romain     (501) staff       (20)      220 2023-04-17 18:29:15.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/direction_down_right.png
+-rw-r--r--   0 romain     (501) staff       (20)      256 2023-04-17 18:29:15.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/direction_left.png
+-rw-r--r--   0 romain     (501) staff       (20)      215 2023-04-17 18:29:15.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/direction_right.png
+-rw-r--r--   0 romain     (501) staff       (20)      270 2023-04-17 18:29:15.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/direction_up.png
+-rw-r--r--   0 romain     (501) staff       (20)      243 2023-04-17 18:29:15.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/direction_up_left.png
+-rw-r--r--   0 romain     (501) staff       (20)      228 2023-04-17 18:29:15.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/direction_up_right.png
+-rw-r--r--   0 romain     (501) staff       (20)      519 2023-04-17 20:23:18.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/drizzle.png
+-rw-r--r--   0 romain     (501) staff       (20)      388 2023-04-17 20:22:30.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/fog.png
+-rw-r--r--   0 romain     (501) staff       (20)      613 2023-04-18 05:58:24.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/mainly_clear.png
+-rw-r--r--   0 romain     (501) staff       (20)      329 2023-04-17 20:17:22.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/na.png
+-rw-r--r--   0 romain     (501) staff       (20)      467 2023-04-17 21:07:00.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/partly_cloudy.png
+-rw-r--r--   0 romain     (501) staff       (20)      555 2023-04-17 20:23:54.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/rain.png
+-rw-r--r--   0 romain     (501) staff       (20)      525 2023-04-17 20:25:57.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/showers.png
+-rw-r--r--   0 romain     (501) staff       (20)      504 2023-04-17 20:24:39.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/snow.png
+-rw-r--r--   0 romain     (501) staff       (20)      504 2023-04-17 15:03:01.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/sunny.png
+-rw-r--r--   0 romain     (501) staff       (20)      576 2023-04-17 21:16:48.000000 astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/thunderstorm.png
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-22 12:38:27.913836 astro-toolbox-0.1.2/src/astro_toolbox/scripts/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-17 20:03:46.000000 astro-toolbox-0.1.2/src/astro_toolbox/scripts/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     1780 2023-02-08 13:53:17.000000 astro-toolbox-0.1.2/src/astro_toolbox/scripts/planning.py
+-rw-r--r--   0 romain     (501) staff       (20)    17107 2023-04-22 12:11:44.000000 astro-toolbox-0.1.2/src/astro_toolbox/scripts/plots.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-22 12:38:27.914863 astro-toolbox-0.1.2/src/astro_toolbox/time/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:53:46.000000 astro-toolbox-0.1.2/src/astro_toolbox/time/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     6330 2023-04-17 16:55:55.000000 astro-toolbox-0.1.2/src/astro_toolbox/time/core.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-22 12:38:27.915500 astro-toolbox-0.1.2/src/astro_toolbox/utils/
+-rw-r--r--   0 romain     (501) staff       (20)      441 2023-04-22 09:17:42.000000 astro-toolbox-0.1.2/src/astro_toolbox/utils/python_functions.py
+-rw-r--r--   0 romain     (501) staff       (20)      659 2023-04-17 16:11:48.000000 astro-toolbox-0.1.2/src/astro_toolbox/utils/strparser.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-22 12:38:27.900894 astro-toolbox-0.1.2/src/astro_toolbox.egg-info/
+-rw-r--r--   0 romain     (501) staff       (20)     4754 2023-04-22 12:38:27.000000 astro-toolbox-0.1.2/src/astro_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 romain     (501) staff       (20)     2330 2023-04-22 12:38:27.000000 astro-toolbox-0.1.2/src/astro_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 romain     (501) staff       (20)        1 2023-04-22 12:38:27.000000 astro-toolbox-0.1.2/src/astro_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 romain     (501) staff       (20)       62 2023-04-22 12:38:27.000000 astro-toolbox-0.1.2/src/astro_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 romain     (501) staff       (20)        1 2023-01-18 11:00:43.000000 astro-toolbox-0.1.2/src/astro_toolbox.egg-info/not-zip-safe
+-rw-r--r--   0 romain     (501) staff       (20)      152 2023-04-22 12:38:27.000000 astro-toolbox-0.1.2/src/astro_toolbox.egg-info/requires.txt
+-rw-r--r--   0 romain     (501) staff       (20)       14 2023-04-22 12:38:27.000000 astro-toolbox-0.1.2/src/astro_toolbox.egg-info/top_level.txt
```

### Comparing `astro-toolbox-0.1.1/LICENSE` & `astro-toolbox-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/PKG-INFO` & `astro-toolbox-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-toolbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: Toolbox for observationnal astronomy
 Home-page: https://github.com/rloustalet/astro_toolbox
 Author: Romain Loustalet Palengat
 Project-URL: Source, https://github.com/rloustalet/astro_toolbox
 Project-URL: Documentation, https://astro-toolbox.readthedocs.io/en/latest/
 Keywords: astro,toolbox,astro_toolbox,observationnal
 Platform: unix
@@ -139,14 +139,17 @@
 
 **-l, \--location** Option to inform a location name `-l Greenwich`,
 default is None (last location used).
 
 **-d, \--days** Counter to inform the number of days to display,
 default is 1.
 
+**-p, \--past** Counter to inform the number of past days to display,
+default is 0.
+
 ## Documentation
 
 The documentation is availale on [readthedocs.io](https://astro-toolbox.readthedocs.io/en/latest/)
 
 ## License
 
 Astropy is licensed under a GNU GPL license - see the [LICENSE](https://github.com/rloustalet/astro_toolbox/blob/main/LICENSE) file.
```

### Comparing `astro-toolbox-0.1.1/README.md` & `astro-toolbox-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -115,14 +115,17 @@
 
 **-l, \--location** Option to inform a location name `-l Greenwich`,
 default is None (last location used).
 
 **-d, \--days** Counter to inform the number of days to display,
 default is 1.
 
+**-p, \--past** Counter to inform the number of past days to display,
+default is 0.
+
 ## Documentation
 
 The documentation is availale on [readthedocs.io](https://astro-toolbox.readthedocs.io/en/latest/)
 
 ## License
 
 Astropy is licensed under a GNU GPL license - see the [LICENSE](https://github.com/rloustalet/astro_toolbox/blob/main/LICENSE) file.
```

### Comparing `astro-toolbox-0.1.1/setup.cfg` & `astro-toolbox-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/__init__.py` & `astro-toolbox-0.1.2/src/astro_toolbox/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
     "Location",
     "Ephemeris",
     "Simbad",
     "Horizons",
     "OpenMeteo",
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/angle/degrees.py` & `astro-toolbox-0.1.2/src/astro_toolbox/angle/degrees.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/angle/dms.py` & `astro-toolbox-0.1.2/src/astro_toolbox/angle/dms.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/angle/hms.py` & `astro-toolbox-0.1.2/src/astro_toolbox/angle/hms.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/angle/radians.py` & `astro-toolbox-0.1.2/src/astro_toolbox/angle/radians.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/command_line.py` & `astro-toolbox-0.1.2/src/astro_toolbox/command_line.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """This module creates the console interface.
 """
-import re
 import pathlib
 import json
 import logging
 import pkg_resources
 import click
 from matplotlib.backends.backend_pdf import PdfPages
 from rich.progress import track
+from rich.console import Console
+from rich.table import Table
 
 from astro_toolbox.angle.degrees import AngleDeg
 from astro_toolbox.angle.hms import AngleHMS
 from astro_toolbox.time.core import AstroDateTime
 from astro_toolbox.coordinates.location import Location
 from astro_toolbox.coordinates.equatorial import Equatorial
 from astro_toolbox.query.ephemeris import Horizons
@@ -24,14 +25,82 @@
 from astro_toolbox.scripts.plots import polarstar_plt_southern
 
 from astro_toolbox.query.ephemeris import DICT_OBJECTS
 
 PATH = pkg_resources.resource_filename('astro_toolbox', 'coordinates/data/')
 PATH_2 = pkg_resources.resource_filename('astro_toolbox', 'query/weather_icons/')
 
+def wmototext(code):
+    """Function to convert WMO code to text.
+
+    Parameters
+    ----------
+    code : str
+        WMO code as str.
+
+    Returns
+    -------
+    Object
+        offset_image Object.
+    """
+    if code == '00':
+        text = 'Sunny'
+    elif code == '01':
+        text = 'Mainly Clear'
+    elif code == '02':
+        text = 'Partly Cloudy'
+    elif code == '03':
+        text = 'Cloudy'
+    elif code[0] == '4':
+        text = 'Fog'
+    elif code[0] == '5':
+        text = 'Drizzle'
+    elif code[0] == '6':
+        text = 'Rain'
+    elif code[0] == '7' or code in (85, 86):
+        text = 'Snow'
+    elif code in (80, 81, 82):
+        text = 'Showers'
+    elif code[0] == ('9'):
+        text = 'Thunderstorm'
+    else:
+        text = 'N/A'
+    return text
+
+def winddirectiontotext(wind_direction):
+    """Funcion to convert wind direction to text.
+
+    Parameters
+    ----------
+    wind_direction : float
+        Wind direction
+
+    Returns
+    -------
+    Object
+        offset_image Object.
+    """
+    if 0 <= wind_direction <= 22.5 or 337.5 <= wind_direction <= 360:
+        direction = 'N'
+    elif 22.5 < wind_direction < 67.5:
+        direction = 'NE'
+    elif 67.5 < wind_direction < 112.5:
+        direction = 'E'
+    elif 112.5 < wind_direction < 157.5:
+        direction = 'SE'
+    elif 157.5 < wind_direction < 202.5:
+        direction = 'S'
+    elif 202.5 < wind_direction < 247.5:
+        direction = 'SW'
+    elif 247.5 < wind_direction < 292.5:
+        direction = 'W'
+    elif 292.5 < wind_direction < 337.5:
+        direction = 'NW'
+    return direction
+
 @click.group()
 @click.option(
     "-v",
     "--verbose",
     count=True,
     default=0,
     help="-v for DEBUG",
@@ -187,89 +256,63 @@
     add : bool
         Command to add site
     delete : bool
         Command to delete site
     update : bool
         Command to update site
     """
-    def _verify_coords(latitude, longitude, elevation):
-        """Function to verify coords
-
-        Parameters
-        ----------
-        latitude : str
-            Latitude string
-        longitude : str
-            Longitude string
-        elevation : float
-            Elevation float
-
-        Returns
-        -------
-        list
-            Coords list
-
-        Raises
-        ------
-        ValueError
-            Latitude or Longitude is not in necessary format
-        ValueError
-            Elevation is not a number
-        """
-        coords = [latitude, longitude]
-        for count, value in enumerate(coords):
-            value_flag = True
-            if ('°' and "'") in value:
-                coord_str = re.split(r"[°']",value)[:3]
-                coords[count] = tuple(float(coord_val) for coord_val in coord_str)
-                value_flag = False
-            elif '.' in value and not ('°' and "'") in value:
-                coords[count] = AngleDeg(float(value)).degtodms
-                value_flag = False
-            elif value_flag is False and (value != 'None'):
-                raise ValueError(f"{value} Latitude or longitude is not in format 0.0 or 0°0'0''")
-            if not isinstance(elevation, float):
-                raise ValueError((f"{value} Elevation value is not a number"))
-        return coords
-    if add:
+    if add and location_name != 'list':
         latitude = str(input("Enter latitude in degrees (00.00) or in dms (00°00'00\"): "))
         if '.' in latitude and ('°' and "'") not in latitude:
             latitude = AngleDeg(float(latitude)).degtodms()
         longitude = str(input("Enter longitude in degrees (00.00) or in dms (00°00'00\"): "))
         if '.' in longitude and ('°' and "'") not in longitude:
             longitude = AngleDeg(float(longitude)).degtodms()
         elevation = float(input("Enter elevation in meters: ") or 0)
-        coords = (latitude, longitude, elevation)
-        Location(location_name, coords[0], coords[1], elevation).save_site()
+        Location(location_name, latitude, longitude, elevation).save_site()
 
-    if delete:
+    if delete and location_name != 'list':
         Location(name=location_name).delete_site()
 
-    if update:
+    if update and location_name != 'list':
         click.echo('Enter only values to update')
         latitude = (str(input("Enter latitude in degrees (00.00) or in dms (00°00'00''): ")
                     or None))
         longitude = (str(input("Enter longitude in degrees (00.00) or in dms (00°00'00''): ")
                     or None))
-        elevation = (float(input("Enter elevation in meters: ")
-                    or 'nan'))
-        coords = _verify_coords(latitude=latitude, longitude=longitude, elevation=elevation)
-        Location(location_name, coords[0], coords[1], elevation).update_site()
+        elevation = (str(input("Enter elevation in meters: "))
+                    or None)
+        location = Location(location_name)
+        if latitude == "None":
+            latitude = None
+        elif '.' in latitude and ('°' and "'") not in latitude:
+            latitude = AngleDeg(float(latitude)).degtodms()
+        if longitude == "None":
+            longitude = None
+        elif '.' in longitude and ('°' and "'") not in longitude:
+            longitude = AngleDeg(float(longitude)).degtodms()
+        Location(location_name, latitude, longitude, elevation).update_site()
 
     if location_name == 'list':
         with open(PATH  + 'sites.json', encoding="utf-8") as json_file:
             dict_sites = json.load(json_file)
         name_list = list(dict_sites.keys())
         count = 1
         for name in name_list:
             click.echo(f"{count}: " + f"{name}: latitude: {dict_sites[name]['latitude']} "+
                 f"longitude: {dict_sites[name]['longitude']} "+
                 f"elevation = {dict_sites[name]['elevation']} m")
             count = count + 1
 
+    if location_name != 'list':
+        location = Location(location_name)
+        click.echo(f"{location.name}: latitude: {location.latitude} "+
+                f"longitude: {location.longitude} "+
+                f"elevation = {location.elevation} m")
+
 @cli.command('polaris')
 @click.option("-t", "--time",
             type=click.STRING,
             default=None,
             help='-t, --time the date and time default is None if None, now')
 @click.option("-l", "--location",
             type=click.STRING,
@@ -297,43 +340,64 @@
             default=None,
             help='-l --location the site name default is None if None last site used')
 @click.option(
     "-d",
     "--days",
     count=True,
     default=1)
-def weather_command(location, days):
+@click.option(
+    "-p",
+    "--past",
+    count=True,
+    default=0)
+def weather_command(location, days, past):
     """Weather forecasts displayed from Open-Meteo
 
     Parameters
     ----------
     location : str
         Saved site name.
     days : int
         Number of days displayed.
     """
     last_time = '0000-00-00T00:00:00'
     print(f'weather_forecasts @ {Location(location)}')
     weather_forecasts = OpenMeteo(Location(location))
-    for time in weather_forecasts.data['hourly']['time'][:24*days]:
+    console = Console()
+    table = Table()
+    for time in weather_forecasts.data['hourly']['time'][72 - 24 * past :72 + 24*days]:
         time += ':00'
         if int(time[8:10]) != int(last_time[8:10]):
-            print('=' * 174)
-            print(f"|{'Time (UT)':^25}|{'Temperature (°C)':^20}|" +
-                f"{'Humidity (%)':^20}|{'Precipitation (mm)':^20}|" +
-                f"{'Wind Speed (km/h)':^20}|{'Wind Direction (°)':^20}|" +
-                f"{'Cloud Coverage (%)':^20}|{'WMO':^20}|")
-            print('=' * 174)
+            console.print(table)
+            table = Table(title=f"Weather forecasts {time[:11]} " +
+                          f"@ {weather_forecasts.location.name}",
+                          show_lines=True)
+            table.add_column("Time (UT)", justify="center")
+            table.add_column("Temperature (°C)", justify="center")
+            table.add_column("Humidity (%)", justify="center")
+            table.add_column("Precipitation (mm)", justify="center")
+            table.add_column("Wind speed (km/h)", justify="center")
+            table.add_column("Wind Direction", justify="center")
+            table.add_column("Cloud Coverage (%)", justify="center")
+            table.add_column(justify="center")
+            table.add_row(f'{time:^25}',
+                        f'{weather_forecasts.get_temperature(time)}',
+                        f'{weather_forecasts.get_humidity(time)}',
+                        f'{weather_forecasts.get_precipitation(time)}',
+                        f'{weather_forecasts.get_wind_speed(time)}',
+                        f'{winddirectiontotext(weather_forecasts.get_wind_direction(time))}',
+                        f'{weather_forecasts.get_cloud(time)}',
+                        wmototext(weather_forecasts.get_wmo(time)))
         else:
-            print('-' * 174)
-        print(f'|{time:^25}|{weather_forecasts.get_temperature(time):^20}|' +
-              f'{weather_forecasts.get_humidity(time):^20}|' +
-              f'{weather_forecasts.get_precipitation(time):^20}|' +
-              f'{weather_forecasts.get_wind_speed(time):^20}|' +
-              f'{weather_forecasts.get_wind_direction(time):^20}|' +
-              f'{weather_forecasts.get_cloud(time):^20}|' +
-              f'{weather_forecasts.get_wmo(time):^20}|')
+            table.add_row(f'{time:^25}',
+                        f'{weather_forecasts.get_temperature(time)}',
+                        f'{weather_forecasts.get_humidity(time)}',
+                        f'{weather_forecasts.get_precipitation(time)}',
+                        f'{weather_forecasts.get_wind_speed(time)}',
+                        f'{winddirectiontotext(weather_forecasts.get_wind_direction(time))}',
+                        f'{weather_forecasts.get_cloud(time)}',
+                        wmototext(weather_forecasts.get_wmo(time)))
         last_time = time
-    print('-' * 174)
+    console.print(table)
 
 if __name__ == '__main__':
     cli(False)
```

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/coordinates/data/orbital_elements.json` & `astro-toolbox-0.1.2/src/astro_toolbox/coordinates/data/orbital_elements.json`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/coordinates/equatorial.py` & `astro-toolbox-0.1.2/src/astro_toolbox/coordinates/equatorial.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/coordinates/horizontal.py` & `astro-toolbox-0.1.2/src/astro_toolbox/coordinates/horizontal.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/coordinates/location.py` & `astro-toolbox-0.1.2/src/astro_toolbox/coordinates/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,16 +141,15 @@
         """
         with open(PATH  + 'sites.json', encoding="utf-8") as json_file:
             dict_sites = json.load(json_file)
         if self.name.lower() in list(key.lower() for key in dict_sites):
             keys = list(key for key in dict_sites)
             idx = [key.lower() for key in dict_sites].index(self.name.lower())
             for key in dict_sites[keys[idx]]:
-                if self.current_site[self.name][key] is not None:
-                    dict_sites[keys[idx]][key] = self.current_site[self.name][key]
+                dict_sites[keys[idx]][key] = self.current_site[self.name][key]
             with open(PATH  + 'sites.json', 'w', encoding="utf-8") as json_file:
                 json.dump(dict_sites, json_file, indent=4)
             return None
         raise ValueError("Site doesn't exist")
 
     def _get_site(self, name: str = None):
         """Method to get a site with it data.
```

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/coordinates/solar_system.py` & `astro-toolbox-0.1.2/src/astro_toolbox/coordinates/solar_system.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/query/catalogs.py` & `astro-toolbox-0.1.2/src/astro_toolbox/query/catalogs.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/query/ephemeris.py` & `astro-toolbox-0.1.2/src/astro_toolbox/query/ephemeris.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/query/weather.py` & `astro-toolbox-0.1.2/src/astro_toolbox/query/weather.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,23 +82,24 @@
         """
         link = 'https://api.open-meteo.com/v1/forecast?'
         link += (f'latitude={str(self.location.latitude.dmstodeg())}&' +
                 f'longitude={str(self.location.longitude.dmstodeg())}&' +
                 'hourly=' +
                 f'temperature_{self.pressure_level}hPa,' +
                 f'relativehumidity_{self.pressure_level}hPa,' +
+                'dewpoint_2m,' +
                 'precipitation_probability,' +
                 'precipitation,' +
                 'weathercode,' +
                 'pressure_msl,' +
                 f'cloudcover_{self.pressure_level}hPa,' +
                 f'windspeed_{self.pressure_level}hPa,' +
                 f'winddirection_{self.pressure_level}hPa')
 
-        link += f'&models={self.model}&current_weather=false&past_days=1&forecast_days=16'
+        link += f'&models={self.model}&current_weather=false&past_days=3&forecast_days=16'
         request=urllib.Request(link)
         with urllib.urlopen(request) as response:
             result = json.loads(response.read().decode('utf-8'))
         result.pop('generationtime_ms')
         return result
 
     def _get_index(self, datetime: str | tuple):
@@ -231,33 +232,14 @@
         """
         index = self._get_index(datetime)
         if math.isnan(index):
             return float('nan')
         code = self.data['hourly']['weathercode'][index]
         return f'{code:02d}'
 
-    def get_pressure(self, datetime: str | tuple = None):
-        """Get pressure method.
-
-        Parameters
-        ----------
-        datetime : str | tuple, optional
-            Date and Time as tuple (``YYYY,MM,DD,hh,mm,ss`` or ``YYYY-MM-DDThh:mm:ss``),
-            by default None.
-
-        Returns
-        -------
-        float
-            Pressure
-        """
-        index = self._get_index(datetime)
-        if math.isnan(index):
-            return float('nan')
-        return self.data['hourly']['surface_pressure'][index]
-
     def get_msl_pressure(self, datetime: str | tuple = None):
         """Get sea level pressure method.
 
         Parameters
         ----------
         datetime : str | tuple, optional
             Date and Time as tuple (``YYYY,MM,DD,hh,mm,ss`` or ``YYYY-MM-DDThh:mm:ss``),
@@ -325,14 +307,15 @@
         float
             Wind direction
         """
         index = self._get_index(datetime)
         if math.isnan(index):
             return float('nan')
         return self.data['hourly'][f'winddirection_{self.pressure_level}hPa'][index]
+
     def get_units(self):
         """Get units.
 
         Returns
         -------
         dict
             Dict containing units.
```

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/drizzle.png` & `astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/drizzle.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/mainly_clear.png` & `astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/mainly_clear.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/rain.png` & `astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/rain.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/showers.png` & `astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/showers.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/thunderstorm.png` & `astro-toolbox-0.1.2/src/astro_toolbox/query/weather_icons/thunderstorm.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/scripts/planning.py` & `astro-toolbox-0.1.2/src/astro_toolbox/scripts/planning.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/scripts/plots.py` & `astro-toolbox-0.1.2/src/astro_toolbox/scripts/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,22 +59,22 @@
     elif code == '01':
         icon = offset_image('mainly_clear', axis)
     elif code == '02':
         icon = offset_image('partly_cloudy', axis)
     elif code == '03':
         icon = offset_image('cloudy', axis)
     elif code[0] == '4':
-        icon = offset_image('rain_mix', axis)
+        icon = offset_image('fog', axis)
     elif code[0] == '5':
         icon = offset_image('drizzle', axis)
-    elif code[0] == '6' or code == 23:
+    elif code[0] == '6':
         icon = offset_image('rain', axis)
-    elif code[0] == '7' or code == '21':
+    elif code[0] == '7' or code in (85, 86):
         icon = offset_image('snow', axis)
-    elif code[0] == ('8'):
+    elif code in (80, 81, 82):
         icon = offset_image('showers', axis)
     elif code[0] == ('9'):
         icon = offset_image('thunderstorm', axis)
     else:
         icon = offset_image('na', axis)
     return icon
```

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/time/core.py` & `astro-toolbox-0.1.2/src/astro_toolbox/time/core.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox/utils/strparser.py` & `astro-toolbox-0.1.2/src/astro_toolbox/utils/strparser.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox.egg-info/PKG-INFO` & `astro-toolbox-0.1.2/src/astro_toolbox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-toolbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: Toolbox for observationnal astronomy
 Home-page: https://github.com/rloustalet/astro_toolbox
 Author: Romain Loustalet Palengat
 Project-URL: Source, https://github.com/rloustalet/astro_toolbox
 Project-URL: Documentation, https://astro-toolbox.readthedocs.io/en/latest/
 Keywords: astro,toolbox,astro_toolbox,observationnal
 Platform: unix
@@ -139,14 +139,17 @@
 
 **-l, \--location** Option to inform a location name `-l Greenwich`,
 default is None (last location used).
 
 **-d, \--days** Counter to inform the number of days to display,
 default is 1.
 
+**-p, \--past** Counter to inform the number of past days to display,
+default is 0.
+
 ## Documentation
 
 The documentation is availale on [readthedocs.io](https://astro-toolbox.readthedocs.io/en/latest/)
 
 ## License
 
 Astropy is licensed under a GNU GPL license - see the [LICENSE](https://github.com/rloustalet/astro_toolbox/blob/main/LICENSE) file.
```

### Comparing `astro-toolbox-0.1.1/src/astro_toolbox.egg-info/SOURCES.txt` & `astro-toolbox-0.1.2/src/astro_toolbox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,21 +35,18 @@
 src/astro_toolbox/query/weather_icons/direction_left.png
 src/astro_toolbox/query/weather_icons/direction_right.png
 src/astro_toolbox/query/weather_icons/direction_up.png
 src/astro_toolbox/query/weather_icons/direction_up_left.png
 src/astro_toolbox/query/weather_icons/direction_up_right.png
 src/astro_toolbox/query/weather_icons/drizzle.png
 src/astro_toolbox/query/weather_icons/fog.png
-src/astro_toolbox/query/weather_icons/haze.png
 src/astro_toolbox/query/weather_icons/mainly_clear.png
 src/astro_toolbox/query/weather_icons/na.png
 src/astro_toolbox/query/weather_icons/partly_cloudy.png
 src/astro_toolbox/query/weather_icons/rain.png
-src/astro_toolbox/query/weather_icons/rain_mix.png
-src/astro_toolbox/query/weather_icons/sandstorm.png
 src/astro_toolbox/query/weather_icons/showers.png
 src/astro_toolbox/query/weather_icons/snow.png
 src/astro_toolbox/query/weather_icons/sunny.png
 src/astro_toolbox/query/weather_icons/thunderstorm.png
 src/astro_toolbox/scripts/__init__.py
 src/astro_toolbox/scripts/planning.py
 src/astro_toolbox/scripts/plots.py
```

