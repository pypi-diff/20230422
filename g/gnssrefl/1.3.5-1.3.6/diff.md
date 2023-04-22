# Comparing `tmp/gnssrefl-1.3.5.tar.gz` & `tmp/gnssrefl-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-1.3.5.tar", last modified: Sun Apr 16 09:36:43 2023, max compression
+gzip compressed data, was "gnssrefl-1.3.6.tar", last modified: Sat Apr 22 16:09:35 2023, max compression
```

## Comparing `gnssrefl-1.3.5.tar` & `gnssrefl-1.3.6.tar`

### file list

```diff
@@ -1,90 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:36:43.380895 gnssrefl-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-16 09:36:43.380895 gnssrefl-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:36:43.360895 gnssrefl-1.3.5/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/check_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/check_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/check_rinex_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:36:43.360895 gnssrefl-1.3.5/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/felipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/filesizes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15934 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/gnssir.py
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (123)   174542 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-16 09:36:29.000000 gnssrefl-1.3.5/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/make_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/nmea2snr_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34269 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19809 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/quickLook_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5879 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/quickPhase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19480 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/quickPhase_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49164 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/rinex3_snr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    60155 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    58741 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/vwc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:36:43.360895 gnssrefl-1.3.5/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-16 09:36:43.000000 gnssrefl-1.3.5/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-16 09:36:43.000000 gnssrefl-1.3.5/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:36:43.000000 gnssrefl-1.3.5/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-16 09:36:43.000000 gnssrefl-1.3.5/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-16 09:36:43.000000 gnssrefl-1.3.5/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 09:36:43.000000 gnssrefl-1.3.5/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 09:36:43.380895 gnssrefl-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:36:43.380895 gnssrefl-1.3.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-16 09:36:30.000000 gnssrefl-1.3.5/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:09:35.223649 gnssrefl-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-22 16:09:35.223649 gnssrefl-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:09:35.203649 gnssrefl-1.3.6/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/check_rinex_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:09:35.203649 gnssrefl-1.3.6/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/felipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/filesizes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15934 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/gnssir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (123)   174790 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/make_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/nmea2snr_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34303 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19809 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/quickLook_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5871 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/quickPhase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19480 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/quickPhase_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49164 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/rinex3_snr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/smoosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60155 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58967 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/vwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:09:35.203649 gnssrefl-1.3.6/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-22 16:09:35.000000 gnssrefl-1.3.6/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-22 16:09:35.000000 gnssrefl-1.3.6/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 16:09:35.000000 gnssrefl-1.3.6/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-22 16:09:35.000000 gnssrefl-1.3.6/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-22 16:09:35.000000 gnssrefl-1.3.6/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-22 16:09:35.000000 gnssrefl-1.3.6/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 16:09:35.223649 gnssrefl-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:09:35.223649 gnssrefl-1.3.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/test/test_rinex2snr.py
```

### Comparing `gnssrefl-1.3.5/LICENSE` & `gnssrefl-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/PKG-INFO` & `gnssrefl-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.3.5
+Version: 1.3.6
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.3.5** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.3.6** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
```

### Comparing `gnssrefl-1.3.5/README.md` & `gnssrefl-1.3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # gnssrefl
 
-**github version: 1.3.5** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.3.6** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
```

### Comparing `gnssrefl-1.3.5/gnssrefl/EGM96.py` & `gnssrefl-1.3.6/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/check_rinex2.py` & `gnssrefl-1.3.6/gnssrefl/check_rinex_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,22 +62,27 @@
                                 l2psats = l2psats + 1
 
         isat = isat + 3
 
     print('\nFound ', l2cfound, ' GPS satellites that could possibly be L2C in first epoch')
     print('Of those, your file has ', foundGPS-l2psats, ' valid L2C SNR observations')  
 
-def check_rinex_header(rinexfile):
+def check_rinex_file(rinexfile):
     """
     commandline tool to look at header information in a RINEX file
     tries to look for existence of L2C data
 
+    Example
+    -------
+
+    check_rinex_file p0311520.21o
+
     Parameters
-    --------
-    rinexfile : string
+    ----------
+    rinexfile : str
         name of the RINEX 2.11 file
 
     """
     last = rinexfile[-12:]
     year = 2000 + int(last[-3:-1])
     doy = int(last[4:7])
     # assume no coordinates in the file
@@ -171,14 +176,14 @@
 def main():
 
     parser = argparse.ArgumentParser()
     parser.add_argument("rinexfile", help="rinexfile 2.11 name", type=str)
     args = parser.parse_args()
     rinexfile = args.rinexfile
     if os.path.exists(rinexfile):
-        check_rinex_header(rinexfile)
+        check_rinex_file(rinexfile)
     else:
         print('Your input file: ', rinexfile, ' does not exist ')
 
 if __name__ == "__main__":
     main()
```

### Comparing `gnssrefl-1.3.5/gnssrefl/computemp1mp2.py` & `gnssrefl-1.3.6/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/daily_avg.py` & `gnssrefl-1.3.6/gnssrefl/daily_avg.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/daily_avg_cl.py` & `gnssrefl-1.3.6/gnssrefl/daily_avg_cl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# command line module that calls daily_avg.py
 import argparse
 import matplotlib.pyplot as matplt
 import os
 import sys
 
-# my code
 import gnssrefl.gps as g
 import gnssrefl.daily_avg as da
 
 from gnssrefl.utils import str2bool
 
 def parse_arguments():
     # must input start and end year
@@ -36,22 +34,29 @@
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
 def daily_avg(station: str , medfilter: float, ReqTracks: int, txtfile: str = None, plt: bool = True, 
         extension: str = '', year1: int = 2005, year2: int = 2030, fr: int = 0, csv: bool = False, azim1: int = 0, azim2: int = 360, test: bool = False, subdir: str=None):
     """
-    The goal is to consolidate individual RH results into a single file consisting of daily averaged RH without outliers.
+    The goal of this code is to consolidate individual RH results into a single file consisting of daily averaged RH without outliers.
 
-    Currently called as : daily_avg p041 0.25 10 
+    There are multiple optional choices as discussed below. The code also creates a file with all the subdaily RH as well.
 
-    where p041 is the station name, 0.25 is the median filter value in meters, and 10 is the number of values required to
-    trust the daily average.
+    Examples
+    -------- 
+    daily_avg p041 0.25 10 
+        consolidates results for p041 with median filter of 0.25 meters and at least 10 solutions per day
+    daily_avg p041 0.25 10  -year1 2015 -year2 2020
+        consolidates results for p041 with median filter of 0.25 meters and at least 10 solutions per day
+        and restricts it to years between 2015 and 2020
+    daily_avg p041 0.25 10  -year1 2015 -year2 2020 -azim1 0 -azim2 180
+        consolidates results for p041 with median filter of 0.25 meters and at least 10 solutions per day
+        and restricts it to years between 2015 and 2020 and azimuths between 0 and 180 degrees
 
-    There are multiple optional choices as discussed below. The code also creates a file with all the subdaily RH as well.
 
     Parameters
     ----------
     station : string
         4 ch station name 
 
     medfilter : float
```

### Comparing `gnssrefl-1.3.5/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-1.3.6/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/download_ioc.py` & `gnssrefl-1.3.6/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/download_noaa.py` & `gnssrefl-1.3.6/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/download_orbits.py` & `gnssrefl-1.3.6/gnssrefl/download_orbits.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
-"""
-downloads Orbit files from various sources
-"""
 import argparse
+import numpy as np
 import sys
+import time
 
 import gnssrefl.gps as g
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser()
     parser.add_argument("orbit", help="orbit name (gps,gnss,gps+glo, or specific e.g. jax) ", type=str)
@@ -20,15 +19,29 @@
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
 def download_orbits(orbit: str, year: int, month: int, day: int, doy_end: int = None ):
     """
-    command line interface for download_orbits
+    command line interface for download_orbits. If day is zero, then it is assumed that 
+    the month record is day or year
+
+    Examples
+    --------
+    download_orbits nav 2020 50 0
+        downloads broadcast orbits for day of year 50 in the year 2020
+    download_orbits nav 2020 1 1 
+        downloads broadcast orbits for January 1, 2020
+    download_orbits gnss 2023 1 1 
+        multi-GNSS orbits from GFZ
+    download_orbits rapid 2023 1 1 
+        rapid multi-GNSS orbits from GFZ
+    download_orbits rapid 2023 1 0 -doy_end 10
+        rapid multi-GNSS orbits from GFZ for days of year 1 thru 10 in 2023
 
     Parameters
     ----------
 
     orbit : string
         value options:
 
@@ -66,21 +79,18 @@
 
             ultra : ultra orbits directly from GFZ
 
             rapid : rapid orbits directly from GFZ
 
     year : integer
         full year
-
     month : integer
         calendar month
-
     day : integer
         day of the month
-
     doy_end : integer 
         optional, allows multiple day download
 
     """
 
 #   make sure environment variables exist.  set to current directory if not
     g.check_environ_variables()
@@ -117,16 +127,18 @@
 
     # using gfz multi-gnss for rapid
     if pCtr == 'rapid':
         pCtr = 'gfr'
 
     d1= int(doy); d2 = int(doy_end) + 1
     for d in range(d1, d2):
+        s1 = time.time()
 
         year,month,day= g.ydoy2ymd(year,d)
+        print('Looking for ', year, '/', d, ' mm/dd', month, day)
         if (pCtr == 'nav'):
             navname, navdir, foundit = g.getnavfile(year, month, day)
             if foundit:
                 print('\n SUCCESS:', navdir+'/'+navname)
         elif (pCtr == 'nav-esa'):
             navname, navdir, foundit = g.getnavfile_archive(year, month, day,'esa')
             if foundit:
@@ -157,14 +169,16 @@
                     filename, fdir, foundit = g.avoid_cddis(year, month, day)
                 else:
                     filename, fdir, foundit = g.getsp3file_mgex(year, month, day, pCtr)
             if foundit:
                 print('SUCCESS:', fdir+'/'+filename)
             else:
                 print(filename, ' not found')
+        s2 = time.time()
+        print('That download took ', np.round(s2-s1,2), ' seconds')
 
 
 def main():
     args = parse_arguments()
     download_orbits(**args)
```

### Comparing `gnssrefl-1.3.5/gnssrefl/download_psmsl.py` & `gnssrefl-1.3.6/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/download_rinex.py` & `gnssrefl-1.3.6/gnssrefl/download_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/download_teqc.py` & `gnssrefl-1.3.6/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/download_tides.py` & `gnssrefl-1.3.6/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/download_unr.py` & `gnssrefl-1.3.6/gnssrefl/download_unr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-# -*- coding: utf-8 -*-
-"""
-downloads East North Vertical nevada reno position files
-IGS2014 frame
-"""
 import argparse
 import wget
 import sys
 import os
 import gnssrefl.gps as g
 
 
@@ -17,20 +12,30 @@
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
 def download_unr(station: str):
     """
-    Command line interface for download_blewitt
+    Command line interface for downloading time series from the 
+    University of Nevada Reno website
+
+    This code is not actively maintained.
+
+    Examples
+    --------
+    download_unr p041
+
+    download_unr sc02
 
     Parameters
     ----------
     station : str
         4 character ID of the station name
+
     """
 
     if len(station) != 4:
         print('illegal station name-must be 4 characters')
         sys.exit()
     station = station.upper()
     url= 'http://geodesy.unr.edu/gps_timeseries/tenv3/IGS14/'
```

### Comparing `gnssrefl-1.3.5/gnssrefl/download_wsv.py` & `gnssrefl-1.3.6/gnssrefl/download_wsv.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/felipe.py` & `gnssrefl-1.3.6/gnssrefl/felipe.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/filesizes.py` & `gnssrefl-1.3.6/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/gnssir.py` & `gnssrefl-1.3.6/gnssrefl/gnssir.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/gnssir_cl.py` & `gnssrefl-1.3.6/gnssrefl/gnssir_cl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-# -*- coding: utf-8 -*-
-# kristine M. larson
-# command line for gnssir.py module
-# 2022 April 15 added gzip boolean input
-
 
 import argparse
 import os
 import subprocess
 import sys
 import wget
 
@@ -56,131 +51,113 @@
 
 def gnssir(station: str, year: int, doy: int, snr: int = 66, plt: bool = False, fr: int = None,
            ampl: float = None, sat: int = None, doy_end: int = None, year_end: int = None,
            azim1: int = 0, azim2: int = 360, nooverwrite: bool = False, extension: str = '',
            compress: bool = False, screenstats: bool = False, delTmax: int = None,
            e1: float = None, e2: float = None, mmdd: bool = False, gzip: bool = False, dec : int = 1):
     """
-        gnssir is the main driver for estimating Reflector Height using GNSS Interferometric Reflectometry.
+        gnssir is the main driver for estimating Reflector Heights
         The user is required to have set up an analysis strategy using "make_json_input" 
         
-        To run the gnssir code,  you need 1) a SNR file and 2) the analysis strategy.   The required inputs
-        (station, year, doy) tell the code where to find the SNR file. The station name tells the code whre
-        to find the analysis strategy file.
-
-        Sample function call:
-
-        gnssir p041 2021 15 would analyze the data for station p041, year 2021 and day of year 15.
-
-        If gnssir is not working properly - or you do not understand why it is making various choices, you 
-        are encouraged to set screenstats to True.
+        Examples
+        --------
+        gnssir p041 2021 15 
+            analyzes the data for station p041, year 2021 and day of year 15.
+        gnssir p041 2021 15  -snr 99
+            uses SNR files with a 99 suffix
+        gnssir p041 2021 15  -snr 99 -screenstats T
+            sends debugging information to the screen
+        gnssir p041 2021 15  -nooverwrite T 
+            only runs gnssir if there isn't a previous solution
+        gnssir p041 2021 15  -doy_end 20 
+            Analyzes data from day of year 15 to day of year 20
 
         Parameters
         ----------
-        station : string
-            4 character ID of the station
-            lowercase please
-
-        year : integer
-            Year
-
+        station : str
+            lowercase 4 character ID of the station
+        year : int
+            full Year
         doy : integer
             Day of year
-
-        snr : integer, optional
+        snr : int, optional
             SNR format. This tells the code what elevation angles to save data for. Will be the snr file ending.
             value options:
                 66 (default) : saves all data with elevation angles less than 30 degress
 
                 99 : saves all data with elevation angles between 5 and 30 degrees
 
                 88 : saves all data 
 
                 50 : saves all data with elevation angles less than 10 degrees
 
-        plt : boolean, optional
-            Send plots to screen or not.
-            Default is False.
-
-        fr : integer, optional
-            GNSS frequency.
-            value options:
+        plt : bool, optional
+            Send plots to screen or not. Default is False.
+        fr : int, optional
+            GNSS frequency. Value options:
                 1,2,20,5 : GPS L1, L2, L2C, L5
 
                 101,102 : GLONASS L1, L2
 
                 201, 205,206,207,208 : GALILEO E1, E5a,E6,E5b,E5
 
                 302,306,307 : BEIDOU B1, B3, B2
 
         ampl : float, optional
             minimum spectral peak amplitude.
             default is None
 
-        sat : integer, optional
+        sat : int, optional
             satellite number to only look at that single satellite.
             default is None.
 
         doy_end : int, optional
             end day of year. This is to create a range from doy to doy_end of days.
             If year_end parameter is used - then day_end will end in the day of the year_end.
             Default is None. (meaning only a single day using the doy parameter)
 
         year_end : int, optional
             end year. This is to create a range from year to year_end to get the snr files for more than one year.
             doy_end will be for year_end.
             Default is None.
 
-        azim1 : integer, optional
+        azim1 : int, optional
             lower limit azimuth.
             If the azimuth angles are changed in the json (using 'azval' key) and not here, then the json overrides these.
             If changed here, then it overrides what you requested in the json.
             default is 0.
-
-        azim2 : integer, optional
+        azim2 : int, optional
             upper limit azimuth.
             If the azimuth angles are changed in the json (using 'azval' key) and not changed here, then the json overrides these.
             If changed here, then it overrides what you requested in the json.
             default is 360.
-
-        nooverwrite : boolean, optional
+        nooverwrite : bool, optional
             Use to overwrite lomb scargle result files or not.
             Default is True (do not overwrite files).
-
         extension : string, optional
             extension for result file, useful for testing strategies.
             default is ''. (empty string)
-
         compress : boolean, optional
             xz compress SNR files after use.
             default is False.
-
-        screenstats : boolean, optional
+        screenstats : bool, optional
             whether to print stats to the screen or not.
             default is True.
-
-        delTmax : integer, optional
-            satellite arc length in minutes.
-            default is None.
-
+        delTmax : int, optional
+            maximum satellite arc length in minutes. Set in make_json_input
         e1 : float, optional
             use to override the minimum elevation angle.
-            default is None.
-
         e2 : float, optional
             use to override the maximum elevation angle.
-            default is None.
-
         mmdd : boolean, optional
             adds columns in results for month, day, hour, and minute.
             default is False.
         gzip : boolean, optional
             gzip compress SNR files after use.
             default is False.
-
         dec : int, optional
             decimate SNR file to this sampling period before the 
             periodograms are computed. 1 sec is default (i.e. no decimating)
 
     """
 
 #   make sure environment variables exist.  set to current directory if not
```

### Comparing `gnssrefl-1.3.5/gnssrefl/gnsssnr.f` & `gnssrefl-1.3.6/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/gnsssnrbigger.f` & `gnssrefl-1.3.6/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/gps.py` & `gnssrefl-1.3.6/gnssrefl/gps.py`

 * *Files 0% similar despite different names*

```diff
@@ -858,35 +858,43 @@
                 subprocess.call(['uncompress', secure_file])
                 store_orbitfile(name,year,'sp3') ; 
 
     return foundit
 
 def kgpsweek(year, month, day, hour, minute, second):
     """
+    Calculates GPS week and GPS second of the week
+    There is another version that works on character string.
+    I think (kgpsweekC)
+    
+    Examples
+    --------
+    kgpsweek(2023,1,1,0,0,0)
+        returns 2243  and  0
 
     Parameters
     ----------
-    year : string
-        4 char
-    month : string 
-        2 char
-    day : string
-        2 char
-    hour: string
-        2 char
-    minute : string
-        2 char
-
-    second : integer?
+    year : int 
+        full year
+    month : int 
+        calendar month
+    day : int 
+        calendar day
+    hour: int
+        hour of the Day (gps time)
+    minute : int 
+        minutes 
+    second : int
+        seconds
 
     Returns
-    --------
-    GPS_wk : integer
+    -------
+    GPS_wk : int
         GPS week
-    GPS_sec_wk : intger
+    GPS_sec_wk : int
         GPS second of the week
 
     """
 
     year = int(year)
     M = int(month)
     D = int(day)
@@ -4862,15 +4870,15 @@
     return littlename, fdir, foundit
 
 def rapid_gfz_orbits(year,month,day):
     """
     downloads gfz rapid orbit and stores in $ORBITS
 
     Parameters
-    --------------
+    ----------
     year : int
         full year
     month : int
         month or day of year if day is set to zero
     day : int
         day of month
 
@@ -4910,15 +4918,15 @@
 
 
 def ultra_gfz_orbits(year,month,day,hour):
     """
     downloads rapid GFZ sp3 file and stores them in $ORBITS
 
     Parameters
-    -----------
+    ----------
     year : int
         full year
 
     month : int
         month or day of year
 
     day : int
@@ -5982,15 +5990,15 @@
 
 def quickp(station,t,sealevel):
     """
     makes a quick plot of sea level 
     prints the plot to the screen - it does not save it.
 
     Parameters
-    -----------
+    ----------
     station : str
         station name
 
     t : numpy array in datetime format
         time of the sea level observations UTC
 
     sealevel : list,  float
```

### Comparing `gnssrefl-1.3.5/gnssrefl/gpssnr.f` & `gnssrefl-1.3.6/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/gpsweek.py` & `gnssrefl-1.3.6/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/gpt_1wA.pickle` & `gnssrefl-1.3.6/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/highrate.py` & `gnssrefl-1.3.6/gnssrefl/highrate.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/installexe_cl.py` & `gnssrefl-1.3.6/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/invsnr_cl.py` & `gnssrefl-1.3.6/gnssrefl/invsnr_cl.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,41 +54,44 @@
            screenstats: bool = False, tempres: int = 1, polydeg: int = 2, snrfit: bool = True, plt: bool = True,
            doy_end: int = None, lspfigs: bool = False, snrfigs: bool = False, knot_space: int = 3,
            rough_in: float = 0.1, risky: bool = False, snr_ending: int = 66, outfile_type: str = 'txt',
            outfile_name: str = '', outlier_limit: float = 0.5, no_dots: bool = False, delta_out: int = 300,
            refraction: bool = True, json_override: bool = False):
 
     """
-    Wrapper to call invsnr code.
+    Calls invsnr code.
 
-    outfile_name and outfile_type are unnecessary. Consolidate them.
+    Note: outfile_name and outfile_type are unnecessary. Consolidate them.
     
-    Example:
-
+    Examples
+    -------
     invsnr sc02 2023 15 L1+L2+L5 
+        would analyze day of year 15 and the L1, L2, and L5 signals
+    invsnr sc02 2023 15 ALL
+        would analyze day of year 15 and all signals
+    invsnr sc02 2023 15 L1+L2
+        would analyze day of year 15 and just L1 and L2
+    invsnr sc02 2023 15 L1+L2  -doy_end 18
+        would analyze day of years 15 through 18 and L1 and L2 signals
 
     Parameters
     ----------
-    station : string
+    station : str
         four character ID 
-
-    year : integer
+    year : int
         Year
-
-    doy : integer
+    doy : int
         Day of year
-
-    signal : string
+    signal : str
         signal to use.
-        value options: L1 L2 L5 L6 L7 L1+L2 L1+L2+L5 L1+L5 ALL
-
+        value options: 
+            L1  L2 L5 L6 L7 L1+L2 L1+L2+L5 L1+L5 ALL
     pktnlim: float, optional
         Peak2noise ratio limit for Quality Control.
         Default is 4
-
     constel: str, optional
         Only a single constellation.
         Default is gps, glonass, and galileo.
         value options:
                 G : GPS
 
                 E : Galileo
@@ -98,88 +101,71 @@
                 C : Beidou
 
                 withBeidou : adds Beidou to the default.
 
     screenstats: bool, optional
         Whether to print out stats to the screen.
         Default is False
-
     tempres: int, optional
         SNR file decimator (seconds)
         Default is 1 (everything)
-
-
     polydeg : integer, optional
         polynomial degree for direct signal removal
         Default is 2
-
     snrfit : bool, optional
         Whether to do the inversion or not
         Default is True
-
     plt : bool, optional
         Whether to plot to the screen or not
         Default is True
-
     doy_end : int, optional
         day of year to end analysis.
         Default is None.
-
     lspfigs : bool, optional
         Whether or not to make LSP plots
         Note: Don't turn these on unless you really need plots because it is 
         slow to make one per satellite arc.
         Default is False
-
     snrfigs : boolean, optional
         Whether or not to make SNR plots
-        Don't turn these on unless you really need plots because it is slow to make one per satellite arc.
+        Don't turn these on unless you really need plots because it is 
+        slow to make one per satellite arc.
         Default is False
-
     knot_space : float, optional
         Knot spacing in hours
         Default is 3
-
     rough_in : float, optional
         Roughness
         Default is 0.1
-
     risky : bool, optional
         Risky taker related to gaps/knot spacing
         Default is False
-
     snr_ending : int, optional
         SNR file ending. Default is 66
-
     outfile_type : string, optional
         output file type, txt or csv
         Default is txt
-
     outfile_name : string, optional
         output file name.
-        Default is ''
-
+        Default is ??
     outlier_limit : float, optional
         Outliers plotted. (meters)
         Default is 0.5
-
     no_dots : bool, optional
         To plot lombscargle or not.
         Default is False
-
     delta_out : int, optional
         Output increment, in seconds.
         Default is 300
-
     refraction : bool, optional
         Default is True
-
     json_override : bool, optional
         Override json file name
         Default is False
+
     """
 
     if len(station) != 4:
         print('Stations must be four characters long. Exiting.')
         sys.exit()
 
     if signal.upper() not in ['L1', 'L2', 'L5', 'L6', 'L7', 'L1+L2', 'L1+L2+L5', 'L1+L5', 'ALL']:
```

### Comparing `gnssrefl-1.3.5/gnssrefl/invsnr_input.py` & `gnssrefl-1.3.6/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/karnak_libraries.py` & `gnssrefl-1.3.6/gnssrefl/karnak_libraries.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/kelly.py` & `gnssrefl-1.3.6/gnssrefl/kelly.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/llh2xyz.py` & `gnssrefl-1.3.6/gnssrefl/llh2xyz.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 import gnssrefl.gps as g
 
 def main():
     """
     Command line tool that converts latitude, longitude, and 
     ellipsoidal ht to Cartesian coordinates  and prints to the screen
 
+    Example
+    -------
+    llh2xyz  39.949492042 -105.194266387  1728.856
+        returns  -1283634.1616   -4726427.8934    4074798.0432
+
     Parameters
     ----------
     lat : float
         latitude in degrees
     lon : float
         longitude in degrees
     height : float
```

### Comparing `gnssrefl-1.3.5/gnssrefl/make_json_input.py` & `gnssrefl-1.3.6/gnssrefl/make_json_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/nmea2snr.py` & `gnssrefl-1.3.6/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/nmea2snr_cl.py` & `gnssrefl-1.3.6/gnssrefl/nmea2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/phase_functions.py` & `gnssrefl-1.3.6/gnssrefl/phase_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     subdir : str
         subdirectory in Files
 
     """
     outdir = xdir + '/Files/' + subdir
     plt.figure(figsize=(10, 6))
-    plt.plot(datetime_dates, tv[:, 2], 'bo')
+    plt.plot(datetime_dates, tv[:, 2], 'b-')
     plt.ylabel('phase (degrees)')
     if fr == 1:
         plt.title(f"Daily L1 Phase Results: {station.upper()}")
     else:
         plt.title(f"Daily L2C Phase Results: {station.upper()}")
     plt.grid()
     plt.gcf().autofmt_xdate()
@@ -991,15 +991,15 @@
         amplitudes of peak LSP 
 
     results : ??
 
     """
     print('Requested frequency: ', freq)
     dataexist = False
-
+    xdir = os.environ['REFL_CODE']
     xfile = xdir + '/input/override/' + station + '_vwc' 
     found_override = False
     # not implementing this yet
     if os.path.exists(xfile):
         print('found override file but not implementing at this time')
     #    override = np.loadtxt(xfile, comments='%')
     #    found_override = True
```

### Comparing `gnssrefl-1.3.5/gnssrefl/prn2gps.py` & `gnssrefl-1.3.6/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/query_unr.py` & `gnssrefl-1.3.6/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/quickLook_cl.py` & `gnssrefl-1.3.6/gnssrefl/quickLook_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/quickLook_function.py` & `gnssrefl-1.3.6/gnssrefl/quickLook_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/quickPhase.py` & `gnssrefl-1.3.6/gnssrefl/quickPhase.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,16 @@
     """
     quickphase computes phase for the given inputs (station, years, doy, elevation angles)
     These phase results are subquently used in vwc. The command line call is phase
     (which maybe we should change).
     
     Examples
     --------
-
     phase p038 2021 4
-        analyzes data from day of year 4
+        analyzes data for year 2021 and day of year 4
 
     phase p038 2021 1 -doy_end 365 
         analyzes data for the whole year
 
 
     Parameters
     ----------
@@ -73,15 +72,15 @@
     snr : integer, optional
         SNR format. This tells the code what elevation angles are in the SNR file
         value options:
             66 (default) : data with elevation angles less than 30 degrees
 
             99 : data with elevation angles between 5 and 30 degrees
 
-            88 : data with elevation angles between 5 and 90 degrees
+            88 : data with all elevation angles 
 
             50 : data with elevation angles less than 10 degrees
 
     fr : string, optional
         GNSS frequency. Currently only supports L2C.
         Default is 20 (l2c)
```

### Comparing `gnssrefl-1.3.5/gnssrefl/quickPhase_function.py` & `gnssrefl-1.3.6/gnssrefl/quickPhase_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/quickplt.py` & `gnssrefl-1.3.6/gnssrefl/quickplt.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,38 +8,57 @@
 import sys
 
 
 def main():
     """
     quick file plotting using matplotlib
 
+    Examples
+    --------
+
+    quickplt txtfile 1 16
+        would plot column 1 on the x-axis and column 16 on the y-axis
+
+    quickplt txtfile 1 16 -xlabel Time
+        would plot column 1 on the x-axis and column 16 on the y-axis
+        and add Time on the x-axis label
+
+    quickplt txtfile 1 16 -reverse T
+        would plot column 1 on the x-axis and column 16 on the y-axis
+        it would reverse the y-axis parameter as you might want if 
+        you are ploting RH but want it to have the same sense as a tide gauge.
+
+    quickplt txtfile 1 16 -ylimits 0 2
+        would restrict y-axis to be between 0 and 2
+
+
     Parameters
     ----------
     filename : str
         name of file to be plotted 
     xcol : str
         column number in the file for the x-axis parameter
     ycol : str
         column number in the file for the y-axis parameter
     mjd : str
         T or True, code will convert MJD to datetime, optional
-    xlabel : str
-        label for x-axis, optional
+    xlabel : str, optional
+        label for x-axis 
     ylabel : str
-        label for y-axis, optional
-    symbol : str
-        prescibe the marker used in the plot, optional
-    reverse : str
-        T or True, to reverse y-axis limits, optional
-    title : str
-        optional title for plot
-    outfile : str
-        name of png file to store plot
-    ylimits: str
-        pair of yaxis limits 
+        label for y-axis 
+    symbol : str, optional
+        prescibe the marker used in the plot 
+    reverse : str, optional
+        T or True, to reverse y-axis limits
+    title : str, optional
+        title for plot 
+    outfile : str, optional
+        name of png file to store plot 
+    ylimits: float, optional
+        pair of yaxis limits  
 
     """
 
     parser = argparse.ArgumentParser()
     parser.add_argument("filename", help="filename", type=str)
     parser.add_argument("xcol", help="x-column", type=str)
     parser.add_argument("ycol",   help="y-column", type=str)
```

### Comparing `gnssrefl-1.3.5/gnssrefl/read_snr_files.py` & `gnssrefl-1.3.6/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/refl_zones.py` & `gnssrefl-1.3.6/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/refl_zones_cl.py` & `gnssrefl-1.3.6/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/refraction.py` & `gnssrefl-1.3.6/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/rh_plot.py` & `gnssrefl-1.3.6/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/rinex2snr.py` & `gnssrefl-1.3.6/gnssrefl/rinex2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/rinex2snr_cl.py` & `gnssrefl-1.3.6/gnssrefl/rinex2snr_cl.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,48 +86,44 @@
     rinex2snr mchl00aus 2022 15  -orb rapid -archive ga 
         30 sec data for mchl00aus and Geoscience Australia
 
     rinex2snr warn00deu 2023 87 -dec 5 -rate high -samplerate 1 -orb rapid -archive bkg -stream S -bkg IGS
         1 sec data for warn00deu, 1 sec decimated to 5 sec, multi-GNSS, bkg archive, streamed, in IGS folder
 
     RINEX3 30 second archives supported  
-        bev, bkg, cddis, epn, ga, gfz, nrcan, sonel, and unavco
+        bev, bkg, cddis, epn, ga, gfz, nrcan, sonel
 
     RINEX3 15 sec archives
-        bfg
+        bfg, unavco
 
     RINEX3 1 sec 
         cddis, bkg, maybe nrcan
 
     Parameters
     ----------
     station : str
-        4 or 9 character ID of the station
-
+        4 or 9 character ID of the station, preferably lowercase
     year : int
         Year
-
     doy : int
         Day of year
-
     snr : int, optional
         SNR format. This tells the code what elevation angles to save data for. Will be the snr file ending.
         value options:
 
-        66 (default) : saves all data with elevation angles less than 30 degrees
+            66 (default) : saves all data with elevation angles less than 30 degrees
 
-        99 : saves all data with elevation angles between 5 and 30 degrees
+            99 : saves all data with elevation angles between 5 and 30 degrees
 
-        88 : saves all data 
+            88 : saves all data 
         
-        50 : saves all data with elevation angles less than 10 degrees
+            50 : saves all data with elevation angles less than 10 degrees
 
     orb : str, optional
-        Which orbit files to download. 
-        Value options:
+        Which orbit files to download. Value options:
 
             gps (default) : will use GPS broadcast orbit
 
             gps+glos : will use JAXA orbits which have GPS and Glonass (usually available in 48 hours)
 
             gnss : will use GFZ orbits, which is multi-GNSS (available in 3-4 days?)
```

### Comparing `gnssrefl-1.3.5/gnssrefl/rinex3_rinex2.py` & `gnssrefl-1.3.6/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/rinex3_snr.py` & `gnssrefl-1.3.6/gnssrefl/rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/rinpy.py` & `gnssrefl-1.3.6/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-1.3.6/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/snow_functions.py` & `gnssrefl-1.3.6/gnssrefl/snow_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import sys
 
 
 import gnssrefl.gps as g
 
-def time_limits(wateryear,longer):
+def time_limits(wateryear,longer,end_doy):
     """
     pick up some time values for windowing RH/snow depth data
 
     Parameters
     ----------
     wateryear : int
         water year
     longer : bool
         whether you want a longer plot
+    end_doy : int
+        last day of the year in the water year you want snow depth calculated for 
 
     Returns
     -------
     starting : float
         start time, fractional (year + doy/365.25)
     ending : float
         end time, fractional (year + doy/365.25)
@@ -35,17 +37,23 @@
         # for plot
         left = datetime.datetime(year=year-1, month=8, day = 1)
     else:
         startdoy, cdoy, cyyyy, cyy = g.ymd2doy(year-1,10,1)
         left = datetime.datetime(year=year-1, month=10, day = 1)
 
     # xaxis limit for the plot
-    right = datetime.datetime(year=year, month=6, day = 30)
+    if end_doy is None: 
+        right = datetime.datetime(year=year, month=6, day = 30)
+        enddoy, cdoy, cyyyy, cyy = g.ymd2doy(year,6,30)
+    else:
+        # doy to mmdd and vice versa.  grrr
+        yy,mm,dd, cyyyy, cdoy, YMD = g.ydoy2useful(year,end_doy)
 
-    enddoy, cdoy, cyyyy, cyy = g.ymd2doy(year,6,30)
+        right = datetime.datetime(year=year, month=mm, day = dd)
+        enddoy, cdoy, cyyyy, cyy = g.ymd2doy(year,mm,dd)
 
     # simple minded extracting the data for given limits
     starting = year-1 + startdoy/365.25
     ending = year + enddoy/365.25
 
     return starting, ending, left, right
 
@@ -178,15 +186,15 @@
         print('Very likely this failed - and you do not have enough bare soil values')
     snow = np.asarray(snow)
     std = np.asarray(std)
 
     return gobst, snow, std
 
 
-def snow_simple(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,outputpng,outputfile,minS,maxS,barereq_days):
+def snow_simple(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,outputpng,outputfile,minS,maxS,barereq_days,end_doy):
     """
     simple snow depth algorithm
 
     Parameters
     ----------
     station : str
         4 ch station name
@@ -213,14 +221,16 @@
         name of the output snowdepth txt file
     minS : float
         minimum snowdepth for plot (m)
     maxS : float
         maximum snowdepth for plot (m)
     barereq_days: int
         min number of days to believe a bare soil average
+    end_doy : int
+        last day of year you want a snow depth value for
 
     """
     ii = (gps[:,1] >= doy1) & ((gps[:,1] <= doy2) & (gps[:,0] == bs))
 
     baresoil = gps[ii,2]
     if len(baresoil) == 0:
         print('No values in the bare soil definition. Exiting')
@@ -234,15 +244,15 @@
         print('Current settings for bare soil are year/', bs, ' for days ', doy1, doy2)
         print('Code requires: ', NB)
         sys.exit()
 
     noSnowRH = np.mean(baresoil)
     print('Bare Soil RH: ', '{0:7.3f}'.format( noSnowRH),'(m)' )
 
-    starting, ending, left, right = time_limits(year, longer)
+    starting, ending, left, right = time_limits(year, longer,end_doy)
 
     t = gps[:,0] + gps[:,1]/365.25
     ii = (t >= starting) & (t <=ending)
     usegps = gps[ii,:]
     if len(usegps) == 0:
         print('No data in this water year. Exiting')
         sys.exit()
@@ -310,15 +320,15 @@
 
     plt.savefig(outputpng, dpi=300)
     if pltit:
         plt.show()
 
     return
 
-def snow_azimuthal(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,outputpng,outputfile,minS,maxS,barereq_days):
+def snow_azimuthal(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,outputpng,outputfile,minS,maxS,barereq_days,end_doy):
     """
     azimuthal snow depth algorithm
     tries to determine the bare soil correction in 20 degree azimuth swaths
 
     Parameters
     ----------
     station : str
@@ -346,14 +356,16 @@
         name of the output snowdepth txt file
     minS : float
         minimum snowdepth for plot (m)
     maxS : float
         maximum snowdepth for plot (m)
     barereq_days : int 
         number of days required to trust a bare soil average
+    end_doy : int
+        last day of year you want to compute snow depth for
 
     """
     ii = (gps[:,1] >= doy1) & ((gps[:,1] <= doy2) & (gps[:,0] == bs))
 
     baresoilAll = gps[ii,:]
     baresoil = gps[ii,2] # 
     if len(baresoil) == 0:
@@ -365,15 +377,15 @@
     # this constraint is actually done later ...
     # could be removed
     NB = barereq_days
     if len(baresoil) < NB:
         print('Not enough values to define baresoil: ', NB)
         sys.exit()
 
-    starting, ending, left, right = time_limits(year, longer)
+    starting, ending, left, right = time_limits(year, longer,end_doy)
 
     # window current water year's data to within time limits
     t = gps[:,0] + gps[:,1]/365.25
     ii = (t >= starting) & (t <=ending)
     usegps = gps[ii,:]
     if len(usegps) == 0:
         print('No data in this water year. Exiting')
```

### Comparing `gnssrefl-1.3.5/gnssrefl/snowdepth_cl.py` & `gnssrefl-1.3.6/gnssrefl/snowdepth_cl.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     parser.add_argument("station", help="station name (4 ch only)", type=str)
     parser.add_argument("year", help="Northern Hemisphere water year", type=int)
     parser.add_argument("-minS", help="y-axis minimum snow depth (m)", type=float,default=None)
     parser.add_argument("-maxS", help="y-axis maximum snow depth (m)", type=float,default=None)
     parser.add_argument("-longer", help="plot longer series", type=str, default=None)
     parser.add_argument("-bare_date1", help="bare soil start yyyy-mm-dd", type=str, default=None)
     parser.add_argument("-bare_date2", help="bare soil end yyyy-mm-dd", type=str, default=None)
-    parser.add_argument("-plt_enddate", help="end date for the plot, yyyy-mm-dd", type=str, default=None)
+    parser.add_argument("-plt_enddate", help="end date for the plot/snow solns, yyyy-mm-dd", type=str, default=None)
     parser.add_argument("-plt", help="whether you want the plot to come to the screen", type=str, default=None)
     parser.add_argument("-simple", help="use simple algorithm (default is false)", type=str, default=None)
     parser.add_argument("-medfilter", help="median filter for daily average(m)", type=float, default=None)
     parser.add_argument("-ReqTracks", help="how many arcs needed for daily average)", type=int, default=None)
     parser.add_argument("-barereq_days", help="how many bare soil values req (default is 15)", type=int, default=None)
 
     args = parser.parse_args().__dict__
@@ -57,16 +57,15 @@
     Output is currently written to a plain text file and a plot is written to a png file.
     Both are located in the $REFL_CODE/Files/station directory
 
     If simple is set to true, the algorithms computes bare soil (and thus snow depth), using
     all values together.  The default defines bare soil values every 10 degrees in azimuth.  
 
     Examples
-    -------
-
+    --------
     snowdepth p101 2022
         would use results from a previous run of daily_avg
 
     snowdepth p101 2022 -medfilter 0.25 -ReqTracks 50
         would run daily_avg for you using 50 tracks/0.25 meter median filter
 
     Parameters
@@ -139,29 +138,33 @@
         sys.exit()
 
 
     if plt_enddate is not None:
         pyear = int(plt_enddate[0:4])
         pmonth = int(plt_enddate[5:7])
         pday = int(plt_enddate[8:10])
+        yend, end_doy = g.cdate2ydoy(plt_enddate)
 
         end_dt = datetime.datetime(year=pyear, month=pmonth, day = pday)
     else:
+        end_doy = None
         end_dt = None
 
     # this overrides other ways of doing things.
     if bare_date1 is not None:
         bs, doy1 = g.cdate2ydoy(bare_date1)
     if bare_date2 is not None:
         rrrr, doy2 = g.cdate2ydoy(bare_date2)
 
     if simple:
-        sf.snow_simple(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,outputpng,outputfile,minS,maxS,barereq_days)
+        sf.snow_simple(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,outputpng,
+                outputfile,minS,maxS,barereq_days,end_doy)
     else:
-        sf.snow_azimuthal(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,outputpng,outputfile,minS,maxS,barereq_days)
+        sf.snow_azimuthal(station,gps,year,longer, doy1,doy2,bs,plt, end_dt,
+                outputpng,outputfile,minS,maxS,barereq_days,end_doy)
 
 def main():
     args = parse_arguments()
     snowdepth(**args)
 
 
 if __name__ == "__main__":
```

### Comparing `gnssrefl-1.3.5/gnssrefl/spline_functions.py` & `gnssrefl-1.3.6/gnssrefl/spline_functions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import numpy as np
 from astropy.time import Time
 from astropy.timeseries import LombScargle
 import datetime
 import math
 import matplotlib.pyplot as plt
+import numpy as np
 import os
 import pickle
 from scipy import interpolate
 from scipy.optimize import least_squares
 import scipy.signal as spectral
 
 from matplotlib.dates import (date2num, DateFormatter)
```

### Comparing `gnssrefl-1.3.5/gnssrefl/subdaily.py` & `gnssrefl-1.3.6/gnssrefl/subdaily.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     plt.xlim((beginT, endT))
     plt.grid()
     g.save_plot(txtdir + '/' + station + '_rhdot1.png')
     plt.close()
 
 def print_badpoints(t,outliersize,txtdir,real_residuals):
     """
-    prints outliers to a file so you can look at them separately
+    prints outliers to a file.
 
     Parameters
     ----------
     t : numpy array
         lomb scargle result array of "bad points". Format given below
 
     outliersize : float
@@ -1154,14 +1154,22 @@
     outlierV : float
        outlier criterion, in meters  used in first go thru
        if None, then use 3 sigma (which is the default)
     outlierV2 : float
        outlier criterion, in meters  used in second go thru
        if None, then use 3 sigma (which is the default)
 
+    delta_out : float, optional
+        seconds for smooth output
+    txtdir : str
+        if wanting to set your own output directory
+    apply_if_corr : bool, optional
+        whether you want to apply the IF correction
+        default is true
+
     """
     # output will go to REFL_CODE/Files unless txtdir provided
     xdir = os.environ['REFL_CODE']
 
     val = kwargs.get('txtdir',[])
     if len(val) == 0:
         txtdir = xdir + '/Files/'
@@ -1707,15 +1715,15 @@
     Eval : numpy array
         number of galileo satellites at an epoch
     Cval : numpy array
         number of beidou satellites at an epoch
     txtdir : str
         where results are stored
     fs : int
-        fontsize 
+        fontsize for the plots
 
     """
 
     fig,ax=plt.subplots()
     ax.plot(tval,nval,'ko',label='Total',markersize=3)
     if (np.sum(Gval) > 0):
         ax.plot(tval,Gval,'bo',label='GPS',markersize=3)
```

### Comparing `gnssrefl-1.3.5/gnssrefl/subdaily_cl.py` & `gnssrefl-1.3.6/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/utils.py` & `gnssrefl-1.3.6/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/veg_multiyr.py` & `gnssrefl-1.3.6/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/vwc.py` & `gnssrefl-1.3.6/gnssrefl/vwc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-import matplotlib.pyplot as plt
+import matplotlib.pyplot as matplt
 import numpy as np
 import os
 import subprocess
 import sys
 
 from datetime import datetime
 from pathlib import Path
@@ -17,106 +17,109 @@
 
 def parse_arguments():
     parser = argparse.ArgumentParser()
     parser.add_argument("station", help="station", type=str)
     parser.add_argument("year", help="year", type=int)
     parser.add_argument("-year_end", default=None, help="year_end", type=int)
     parser.add_argument("-fr", help="frequency", type=int)
-    parser.add_argument("-plt2screen", default=None, type=str, help="boolean for plotting to screen")
+    parser.add_argument("-plt", default=None, type=str, help="boolean for plotting to screen")
     parser.add_argument("-screenstats", default=None, type=str, help="boolean for plotting statistics to screen")
-    parser.add_argument("-min_req_pts_track", default=None, type=int, help="minimum number of points for a track to be kept. Default is 50")
+    parser.add_argument("-min_req_pts_track", default=None, type=int, help="min number of points for a track to be kept. Default is 50")
     parser.add_argument("-polyorder", default=None, type=int, help="override on polynomial order")
-    parser.add_argument("-minvalperday", default=None, type=int, help="minimum number of satellite tracks needed each day. Default is 10")
+    parser.add_argument("-minvalperday", default=None, type=int, help="min number of satellite tracks needed each day. Default is 10")
     parser.add_argument("-snow_filter", default=None, type=str, help="boolean for attempting to remove days contaminated by snow")
     parser.add_argument("-circles", default=None, type=str, help="boolean for circles instead of lines for the final VWC plot ")
     parser.add_argument("-subdir", default=None, type=str, help="use non-default subdirectory for output files")
     parser.add_argument("-tmin", default=None, type=str, help="minimum soil texture")
     parser.add_argument("-tmax", default=None, type=str, help="maximum soil texture")
+    parser.add_argument("-warning_value", default=None, type=float, help="What threshold for bad tracks (default is 5.5 )")
+    parser.add_argument("-auto_removal", default=None, type=str, help="Whether you want to remove bad tracks automatically, default is False)")
 
     args = parser.parse_args().__dict__
 
-    boolean_args = ['plt2screen','screenstats','snow_filter','circles']
+    boolean_args = ['plt','screenstats','snow_filter','circles','auto_removal']
     args = str2bool(args, boolean_args)
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
-def vwc(station: str, year: int, year_end: int = None, fr: int = 20, plt2screen: bool = True, screenstats: bool = False, 
+def vwc(station: str, year: int, year_end: int = None, fr: int = 20, plt: bool = True, screenstats: bool = False, 
         min_req_pts_track: int = 50, polyorder: int = -99, minvalperday: int = 10, 
-        snow_filter: bool = False, circles: bool=False, subdir: str=None, tmin: str=None, tmax: str=None):
+        snow_filter: bool = False, circles: bool=False, subdir: str=None, tmin: str=None, tmax: str=None, warning_value : float=5.5, auto_removal : bool=False):
     """
     Computes VWC from GNSS-IR phase estimates. It concatenates previously computed phase results,  
     makes plots for the four geographic quadrants, computes daily average phase files before converting 
     to volumetric water content (VWC).
 
-    IMO This should be moved into a driver so that the main functions are called separately.
 
     Examples
     --------
-
-    one year for station p038 
-        vwc p038 2017
-
-    three years  for station p038 
-        vwc p038 2015 -year_end 207
+    vwc p038 2017
+        one year for station p038 
+    vwc p038 2015 -year_end 2017
+        three years  for station p038 
+    vwc p038 2015 -year_end 2017 -warning_value 6
+        warns you about tracks greater than 6 %
+    vwc p038 2015 -year_end 2017 -warning_value 6 -auto_removal
+        makes new list of tracks based on your new warning value
 
     Parameters
     ----------
     station : str
         4 character ID of the station
-
-    year : integer
-        Year
-    year_end : integer
+    year : int
+        full Year
+    year_end : int, optional
         last year for analysis
-
     fr : integer, optional
         GNSS frequency. Currently only supports l2c.
         Default is 20 (l2c)
-
-    plt2screen: bool, optional
+    plt: bool, optional
         Whether to produce plots to the screen.
         Default is True
-
     min_req_pts_track : int, optional
         how many points needed to keep a satellite track
         default is 50
-
     polyorder : int
         polynomial order used for leveling.  Usually the code picks it but this allows to users to override. 
         Default is -99 which means let the code decide
-
     minvalperday: integer
         how many phase measurements are needed for each daily measurement
         default is 10
-
     snow_filter: boolean 
         whether you want to attempt to remove points contaminated by snow
         default is False
-
     circles : boolean
         whether you want circles in the final plot (lines are default)
-
     subdir: str
         subdirectory in $REFL_CODE/Files for plots and text file outputs
     tmin: str
         minimum soil texture value, e.g. 0.05
     tmax: str
         maximum soil texture value, e.g. 0.45
+    warning_value : float
+         screen warning about bad tracks (percent VWC).
+         default is 5.5 
+    auto_removal : boolean, optional
+         whether to automatically remove tracks that hit your bad track threshold
+         default value is false
 
     Returns
     -------
 
     Daily phase results in a file at $REFL_CODE/<year>/phase/<station>_phase.txt
         with columns: Year DOY Ph Phsig NormA MM DD
 
     VWC results in a file at $$REFL_CODE/<year>/phase/<station>_vwc.txt
         with columns: FracYr Year DOY  VWC Month Day
 
     """
+
+    remove_bad_tracks = auto_removal
+
     if (len(station) != 4):
         print('station name must be four characters')
         sys.exit()
 
     if (len(str(year)) != 4):
         print('Year must be four characters')
         sys.exit()
@@ -140,27 +143,27 @@
     # default is station name
     if subdir == None:
         subdir = station 
 
     # make sure subdirectory exists
     g.set_subdir(subdir)
 
-    if not plt2screen:
+    if not plt:
         print('no plots will come to screen. Will only be saved.')
 
     # this is leftover from the old code
     writeout = True
 
     snow_file = xdir + '/Files/snowmask_' + station + '.txt'
     snowfileexists = False
     if snow_filter:
         medf = 0.2 # this is meters
         ReqTracks = 10 # have a pretty small number here
         snowfileexists = qp.make_snow_filter(station, medf, ReqTracks, year, year_end)
-        plt.close ('all')# we do not want the plots to come to the screen for the daily average
+        matplt.close ('all')# we do not want the plots to come to the screen for the daily average
 
     # azimuth list
     azlist = [270, 0, 180,90 ]
 
     # load past analysis  for QC
     avg_exist, avg_date, avg_phase = qp.load_avg_phase(station,freq)
     if not avg_exist:
@@ -196,33 +199,42 @@
     stracks = tracks[:, 2]  # satellite names
 
     # column 3 is sat, 4 is azimuth, npoints is 5, azim is 6 and 7
     k = 1
     vxyz = np.empty(shape=[0, 7]) 
 
     # try removing these
-    fig = plt.figure(figsize=(13, 10))
-    ax=plt.subplots_adjust(hspace=0.2)
-    plt.suptitle(f"Station: {station}", size=16)
+    fig = matplt.figure(figsize=(13, 10))
+    ax=matplt.subplots_adjust(hspace=0.2)
+    matplt.suptitle(f"Station: {station}", size=16)
 
     # this is the number of points for a given satellite track
     reqNumpts = min_req_pts_track
 
     # checking each geographic quadrant
+    k4 = 1
+    # list of tracks
+    newlist = station + '_tmp.txt'
+    oldlist = xdir + '/input/' + station + '_phaseRH.txt'
+    print(newlist,oldlist)
+    ftmp = open(newlist,'w+')
+    ftmp.write("{0:s} \n".format( '% station ' + station) )
+    ftmp.write("{0:s} \n".format( '% TrackN  RefH SatNu MeanAz  Nval  Azimuths'))
     for index, az in enumerate(azlist):
         b = 0
         k += 1
         amin = az
         amax = az + 90
         # make a quadrant average for plotting purposes
         vquad = np.empty(shape=[0, 4])
         # pick up the sat list from the actual list
         satlist = stracks[atracks == amin]
 
-        ax = plt.subplot(2, 2, index + 1)
+
+        ax = matplt.subplot(2, 2, index + 1)
         ax.set_title(f'Azimuth {str(amin)}-{str(amax)} deg.')
         ax.grid()
         #ax.autofmt_xdate()
 
         # this satellite list is really satellite TRACKS
         for satellite in satlist:
             if screenstats:
@@ -233,14 +245,18 @@
             t = doy[ii]
             h = hr[ii] # TODO this is never used
             y = year_sat_phase[ii]
             azd = azdata[ii]
             s = ssat[ii]
             amps = amp[ii]
             rhs = rh[ii]
+            iikk  = (atracks == amin) & (stracks == satellite) 
+            rhtrack = float(tracks[iikk,1])
+            meanaztrack = float(tracks[iikk,3])
+            nvalstrack = float(tracks[iikk,4])
 
             if len(x) > reqNumpts:
                 b += 1
                 sortY = np.sort(x)
 
                 N = len(sortY)
                 NN = int(np.round(0.20*N))
@@ -293,16 +309,25 @@
                         # figure out intersetion with "good" results
                         inter, id1, id2 = np.intersect1d(avg_date, satdate, assume_unique=True, return_indices=True)
                         aa = avg_phase[id1]
                         bb = satphase[id2]
                         if len(aa) > 0:
                             res = np.round(np.std(aa - bb), 2)
                             addit = ''
-                            if res > 5.5:
+                            keepit = True
+                            if (res > warning_value ) :
+                                # warning
                                 addit = '>>>>>  Consider Removing This Track <<<<<'
+                                if remove_bad_tracks:
+                                    addit = '>>>>>  Removing This Track - rerun to see effect <<<<<'
+                                    keepit = False
+                            if keepit:
+                                ftmp.write("{0:3.0f} {1:7.2f} {2:3.0f} {3:7.1f} {4:7.0f} {5:4.0f} {6:4.0f} \n".format(k4,rhtrack, satellite,meanaztrack,nvalstrack,amin,amax))
+                                k4 = k4 + 1
+
                             print(f"Npts {len(aa):4.0f} SatNu {satellite:2.0f} Residual {res:6.2f} Azims {amin:3.0f} {amax:3.0f} Amp {max(normAmps):4.2f} {addit:20s} ")
                         else:
                             print('No QC assessment could be made for this satellite track')
                     else:
                         print('No average , so no QC. You should iterate.')
 
 
@@ -310,23 +335,29 @@
                     vxyz = np.vstack((vxyz, newl))
                     datetime_dates = []
                     for yr, d in zip(y, t):
                         datetime_dates.append(datetime.strptime(f'{int(yr)} {int(d)}', '%Y %j'))
 
                     ax.plot(datetime_dates, new_phase, 'o', markersize=3)
                     ax.set_ylabel('Phase')
-                    #ax.set_ylimit((-20,60))
-                    plt.ylim((-20,60))
+                    matplt.ylim((-20,60))
                     # ???
-                    plt.gcf().autofmt_xdate()
+                    matplt.gcf().autofmt_xdate()
 
 
+    ftmp.close()
+    if remove_bad_tracks:
+        print('Writing out a new list of good satellite tracks to ', oldlist)
+        subprocess.call(['mv','-f', newlist, oldlist])
+    else:
+        subprocess.call(['rm','-f', newlist ])
+
     plot_path = f'{xdir}/Files/{subdir}/{station}_az_phase.png'
     print(f"Saving to {plot_path}")
-    plt.savefig(plot_path)
+    matplt.savefig(plot_path)
 
     # this is now done in a function. i believe this can be commented out
     #tv = np.empty(shape=[0, 4])
     # year, day of year, phase, satellite, azimuth, RH, and RH amplitude
     y1 = vxyz[:, 0]
     d1 = vxyz[:, 1]
     phase = vxyz[:, 2]
@@ -346,15 +377,15 @@
             sys.exit()
 
         # make datetime date array
         datetime_dates = [datetime.strptime(f'{int(yr)} {int(d)}', '%Y %j') for yr, d in zip(tv[:, 0], tv[:, 1])]
 
         qp.daily_phase_plot(station, fr,datetime_dates, tv,xdir,subdir)
 
-        qp.convert_phase(station, year, year_end, plt2screen,fr,tmin,tmax,polyorder,circles,subdir)
+        qp.convert_phase(station, year, year_end, plt,fr,tmin,tmax,polyorder,circles,subdir)
 
 
 def main():
     args = parse_arguments()
     vwc(**args)
```

### Comparing `gnssrefl-1.3.5/gnssrefl/vwc_input.py` & `gnssrefl-1.3.6/gnssrefl/vwc_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,30 +9,37 @@
 from gnssrefl.utils import read_files_in_dir, FileTypes, FileManagement
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser()
     parser.add_argument("station", help="station name", type=str)
     parser.add_argument("year", help="year", type=int)
-    parser.add_argument("-min_tracks", default=None, help="minimum number of tracks needed to keep the mean RH", type=int)
-    parser.add_argument("-fr", default=None, help="frequency", type=int)
+    parser.add_argument("-min_tracks", default=None, help="min number of tracks to keep mean RH (default is 100)", type=int)
+    parser.add_argument("-fr", default=None, help="frequency (default is L2C)", type=int)
 
     args = parser.parse_args().__dict__
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
 def vwc_input(station: str, year: int, fr: int = 20, min_tracks: int = 100 ):
     """
     Starts the analysis for volumetric water content.  
     Picks up reflector height (RH) results for a given station and year-year end range and 
     computes the RH mean values and writes them to a file. These will be used to compute a consistent
     set of phase estimates.
 
+    Examples
+    --------
+    vwc_input p038 2018
+         
+    vwc_input p038 2018 -min_tracks 10
+        allow fewer values to accept a satellite track
+
     Parameters
     ----------
     station : string
         4 character ID of the station
     year : integer
         Year
     fr : integer, optional
```

### Comparing `gnssrefl-1.3.5/gnssrefl/xyz2llh.py` & `gnssrefl-1.3.6/gnssrefl/xyz2llh.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 import gnssrefl.gps as g
 
 def main():
     """
     Converts Cartesian coordinates to latitude, longitude, ellipsoidal height.
     Prints to screen
 
+    Example
+    -------
+    xyz2llh -1283634.1615 -4726427.8931 4074798.0429
+        returns 39.949492042 -105.194266387  1728.856
+
     Parameters
     ----------
     x : float
         X coordinate (m)
     y : float
         Y coordinate (m)
     z : float
```

### Comparing `gnssrefl-1.3.5/gnssrefl/ydoy.py` & `gnssrefl-1.3.6/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl/ymd.py` & `gnssrefl-1.3.6/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-1.3.6/gnssrefl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.3.5
+Version: 1.3.6
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.3.5** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.3.6** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
```

### Comparing `gnssrefl-1.3.5/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-1.3.6/gnssrefl.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 gnssrefl/EGM96.py
 gnssrefl/__init__.py
-gnssrefl/check_rinex.py
-gnssrefl/check_rinex2.py
 gnssrefl/check_rinex_file.py
 gnssrefl/computemp1mp2.py
 gnssrefl/daily_avg.py
 gnssrefl/daily_avg_cl.py
 gnssrefl/download_ioc.py
 gnssrefl/download_noaa.py
 gnssrefl/download_orbits.py
@@ -56,14 +54,15 @@
 gnssrefl/rh_plot.py
 gnssrefl/rinex2snr.py
 gnssrefl/rinex2snr_cl.py
 gnssrefl/rinex3_rinex2.py
 gnssrefl/rinex3_snr.py
 gnssrefl/rinpy.py
 gnssrefl/rt_rinex3_snr.py
+gnssrefl/smoosh.py
 gnssrefl/snow_functions.py
 gnssrefl/snowdepth_cl.py
 gnssrefl/spline_functions.py
 gnssrefl/subdaily.py
 gnssrefl/subdaily_cl.py
 gnssrefl/utils.py
 gnssrefl/veg_multiyr.py
```

### Comparing `gnssrefl-1.3.5/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-1.3.6/gnssrefl.egg-info/entry_points.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 [console_scripts]
-check_rinex = gnssrefl.check_rinex:main
 check_rinex_file = gnssrefl.check_rinex_file:main
 daily_avg = gnssrefl.daily_avg_cl:main
 download_orbits = gnssrefl.download_orbits:main
 download_rinex = gnssrefl.download_rinex:main
 download_teqc = gnssrefl.download_teqc:main
 download_tides = gnssrefl.download_tides:main
 download_unr = gnssrefl.download_unr:main
@@ -25,14 +24,15 @@
 quickplt = gnssrefl.quickplt:main
 refl_zones = gnssrefl.refl_zones_cl:main
 rh_plot = gnssrefl.rh_plot:main
 rinex2snr = gnssrefl.rinex2snr_cl:main
 rinex3_rinex2 = gnssrefl.rinex3_rinex2:main
 rinex3_snr = gnssrefl.rinex3_snr:main
 rt_rinex3_snr = gnssrefl.rt_rinex3_snr:main
+smoosh = gnssrefl.smoosh:main
 snowdepth = gnssrefl.snowdepth_cl:main
 subdaily = gnssrefl.subdaily_cl:main
 veg_multiyr = gnssrefl.veg_multiyr:main
 vwc = gnssrefl.vwc:main
 vwc_input = gnssrefl.vwc_input:main
 xyz2llh = gnssrefl.xyz2llh:main
 ydoy = gnssrefl.ydoy:main
```

### Comparing `gnssrefl-1.3.5/pyproject.toml` & `gnssrefl-1.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.5/setup.py` & `gnssrefl-1.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["numpy","wget","scipy","matplotlib","requests","progress","astropy","simplekml","earthscope-sdk"]
 setup(
     name="gnssrefl",
-    version="1.3.5",
+    version="1.3.6",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
@@ -52,25 +52,25 @@
             'installexe= gnssrefl.installexe_cl:main',
             'download_unr = gnssrefl.download_unr:main',
             'query_unr= gnssrefl.query_unr:main',
             'mp1mp2= gnssrefl.computemp1mp2:main',
             'download_teqc = gnssrefl.download_teqc:main',
             'rinex3_rinex2= gnssrefl.rinex3_rinex2:main',
             'veg_multiyr= gnssrefl.veg_multiyr:main',
-            'check_rinex= gnssrefl.check_rinex:main',
             'check_rinex_file= gnssrefl.check_rinex_file:main',
             'rinex3_snr= gnssrefl.rinex3_snr:main',
             'rt_rinex3_snr= gnssrefl.rt_rinex3_snr:main',
             'filesizes= gnssrefl.filesizes:main',
             'invsnr= gnssrefl.invsnr_cl:main',
             'invsnr_input= gnssrefl.invsnr_input:main',
             'vwc_input= gnssrefl.vwc_input:main',
             'phase= gnssrefl.quickPhase:main',
             'refl_zones= gnssrefl.refl_zones_cl:main',
             'vwc= gnssrefl.vwc:main',
+            'smoosh= gnssrefl.smoosh:main',
             'quickplt= gnssrefl.quickplt:main',
             'snowdepth= gnssrefl.snowdepth_cl:main',
             'rh_plot= gnssrefl.rh_plot:main',
             'pickle_dilemma= gnssrefl.pickle_dilemma:main',
             ], 
         },
     install_requires=requirements,
```

### Comparing `gnssrefl-1.3.5/test/test_gps.py` & `gnssrefl-1.3.6/test/test_gps.py`

 * *Files identical despite different names*

