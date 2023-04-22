# Comparing `tmp/alcf-1.4.1.post1.tar.gz` & `tmp/alcf-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alcf-1.4.1.post1.tar", last modified: Fri Apr 21 22:06:40 2023, max compression
+gzip compressed data, was "alcf-1.5.0.tar", last modified: Sat Apr 22 13:43:47 2023, max compression
```

## Comparing `alcf-1.4.1.post1.tar` & `alcf-1.5.0.tar`

### file list

```diff
@@ -1,199 +1,195 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.101308 alcf-1.4.1.post1/
--rw-r--r--   0 peter     (1000) peter     (1000)      239 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/.editorconfig
--rw-r--r--   0 peter     (1000) peter     (1000)     1144 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)      181 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/MANIFEST.in
--rw-r--r--   0 peter     (1000) peter     (1000)     1275 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)     1022 2023-04-21 22:06:40.101308 alcf-1.4.1.post1/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      764 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/README.md
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.085308 alcf-1.4.1.post1/alcf/
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.089308 alcf-1.4.1.post1/alcf/algorithms/
--rw-r--r--   0 peter     (1000) peter     (1000)       27 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.089308 alcf-1.4.1.post1/alcf/algorithms/calibration/
--rw-r--r--   0 peter     (1000) peter     (1000)       62 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/calibration/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      373 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/calibration/default.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.089308 alcf-1.4.1.post1/alcf/algorithms/cloud_base_detection/
--rw-r--r--   0 peter     (1000) peter     (1000)       71 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/cloud_base_detection/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      930 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/cloud_base_detection/default.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.089308 alcf-1.4.1.post1/alcf/algorithms/cloud_detection/
--rw-r--r--   0 peter     (1000) peter     (1000)       66 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/cloud_detection/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      798 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/cloud_detection/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2029 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/couple.py
--rw-r--r--   0 peter     (1000) peter     (1000)   259682 2023-04-21 19:26:50.000000 alcf-1.4.1.post1/alcf/algorithms/interp.c
--rw-r--r--   0 peter     (1000) peter     (1000)     1018 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/interp.pyx
--rw-r--r--   0 peter     (1000) peter     (1000)      781 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/lidar_ratio.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.089308 alcf-1.4.1.post1/alcf/algorithms/noise_removal/
--rw-r--r--   0 peter     (1000) peter     (1000)       64 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/noise_removal/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      981 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/noise_removal/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1682 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/output_sample.py
--rw-r--r--   0 peter     (1000) peter     (1000)     9415 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/stats.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1120 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/tsample.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1776 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/algorithms/zsample.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.089308 alcf-1.4.1.post1/alcf/cmds/
--rw-r--r--   0 peter     (1000) peter     (1000)      408 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/cmds/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3555 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/cmds/auto.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.089308 alcf-1.4.1.post1/alcf/cmds/auto_cmds/
--rw-r--r--   0 peter     (1000) peter     (1000)      141 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/cmds/auto_cmds/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      843 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/cmds/auto_cmds/compare.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1671 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/cmds/auto_cmds/lidar.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1086 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/cmds/auto_cmds/model.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2804 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/cmds/calibrate.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2148 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/cmds/compare.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3429 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/cmds/convert.py
--rw-r--r--   0 peter     (1000) peter     (1000)    10693 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/cmds/lidar.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1395 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/cmds/main.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6342 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/cmds/model.py
--rw-r--r--   0 peter     (1000) peter     (1000)    17038 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/cmds/plot.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6425 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/cmds/simulate.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3569 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/cmds/stats.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.089308 alcf-1.4.1.post1/alcf/fonts/
--rw-r--r--   0 peter     (1000) peter     (1000)     6709 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/fonts/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)    56032 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/fonts/PublicSans-Bold.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    60100 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/fonts/PublicSans-BoldItalic.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    60316 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/fonts/PublicSans-Italic.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    56792 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/fonts/PublicSans-Regular.otf
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.089308 alcf-1.4.1.post1/alcf/lidars/
--rw-r--r--   0 peter     (1000) peter     (1000)     1426 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/lidars/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2033 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/lidars/blview.py
--rw-r--r--   0 peter     (1000) peter     (1000)      101 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/lidars/caliop.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1632 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/lidars/chm15k.py
--rw-r--r--   0 peter     (1000) peter     (1000)      410 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/lidars/cl31.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2157 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/lidars/cl51.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1709 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/lidars/cl61.py
--rw-r--r--   0 peter     (1000) peter     (1000)      996 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/lidars/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3358 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/lidars/mpl.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1873 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/lidars/mpl2nc.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3867 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/misc.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.093308 alcf-1.4.1.post1/alcf/models/
--rw-r--r--   0 peter     (1000) peter     (1000)     2156 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/models/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2221 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/models/amps.py
--rw-r--r--   0 peter     (1000) peter     (1000)      359 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/models/cmip5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2726 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/models/era5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2570 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/models/icon.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2809 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/models/jra55.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1878 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/models/merra2.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2020 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/models/nzcsm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3099 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/models/nzesm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2421 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/alcf/models/um.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.085308 alcf-1.4.1.post1/alcf.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)     1022 2023-04-21 22:06:39.000000 alcf-1.4.1.post1/alcf.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     4516 2023-04-21 22:06:40.000000 alcf-1.4.1.post1/alcf.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-21 22:06:39.000000 alcf-1.4.1.post1/alcf.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-21 19:26:50.000000 alcf-1.4.1.post1/alcf.egg-info/not-zip-safe
--rw-r--r--   0 peter     (1000) peter     (1000)      158 2023-04-21 22:06:39.000000 alcf-1.4.1.post1/alcf.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        5 2023-04-21 22:06:39.000000 alcf-1.4.1.post1/alcf.egg-info/top_level.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.093308 alcf-1.4.1.post1/bin/
--rwxr-xr-x   0 peter     (1000) peter     (1000)      282 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/bin/alcf
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1677 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/build_doc
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.093308 alcf-1.4.1.post1/cosp/
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.093308 alcf-1.4.1.post1/cosp/MISR_simulator/
--rw-r--r--   0 peter     (1000) peter     (1000)    16546 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/MISR_simulator/MISR_simulator.f
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.093308 alcf-1.4.1.post1/cosp/MODIS_simulator/
--rw-r--r--   0 peter     (1000) peter     (1000)    64835 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/MODIS_simulator/modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     7387 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/MODIS_simulator/test_modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5167 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)     7506 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/Makefile.cmor1
--rw-r--r--   0 peter     (1000) peter     (1000)     7515 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/Makefile.ibm
--rw-r--r--   0 peter     (1000) peter     (1000)      842 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/README.md
--rw-r--r--   0 peter     (1000) peter     (1000)    48320 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/README.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      467 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/README_v1.4.1.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.093308 alcf-1.4.1.post1/cosp/actsim/
--rw-r--r--   0 peter     (1000) peter     (1000)    35248 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/actsim/lidar_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    38101 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/actsim/lmd_ipsl_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11672 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/actsim/mie_backscatter_1064.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11571 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/actsim/mie_backscatter_532.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11642 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/actsim/mie_backscatter_910.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.093308 alcf-1.4.1.post1/cosp/cfmip2/
--rw-r--r--   0 peter     (1000) peter     (1000)     2508 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     2487 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     7271 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     7400 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     3320 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     3261 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    31979 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    15220 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_constants.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     1881 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_defs.h
--rw-r--r--   0 peter     (1000) peter     (1000)     2644 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_htfrtc.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     6934 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_input_nl.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    40704 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_io.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     4292 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_isccp_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     4123 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_lidar.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     3561 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_misr_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    25019 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     3646 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_output_nl.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    26091 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_rttov.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5694 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_rttov_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     9657 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    13744 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    70107 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_types.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    13287 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/cosp_utils.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.097308 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/
--rw-r--r--   0 peter     (1000) peter     (1000)     2957 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)    59127 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/README
--rw-r--r--   0 peter     (1000) peter     (1000)      165 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/congvec.expected
--rw-r--r--   0 peter     (1000) peter     (1000)     2545 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/congvec.f
--rw-r--r--   0 peter     (1000) peter     (1000)    43978 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/icarus.f
--rw-r--r--   0 peter     (1000) peter     (1000)      869 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/input.data
--rw-r--r--   0 peter     (1000) peter     (1000)     1042 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/input.data.halved
--rw-r--r--   0 peter     (1000) peter     (1000)    13495 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f
--rw-r--r--   0 peter     (1000) peter     (1000)     1845 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/license
--rwxr-xr-x   0 peter     (1000) peter     (1000)       15 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/rcsid
--rw-r--r--   0 peter     (1000) peter     (1000)    11849 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/scops.f
--rw-r--r--   0 peter     (1000) peter     (1000)     2539 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/test_congvec.f
--rwxr-xr-x   0 peter     (1000) peter     (1000)     2660 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/test_congvec.ksh
--rw-r--r--   0 peter     (1000) peter     (1000)    13385 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f
--rwxr-xr-x   0 peter     (1000) peter     (1000)     3095 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.097308 alcf-1.4.1.post1/cosp/llnl/
--rw-r--r--   0 peter     (1000) peter     (1000)     7918 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/llnl/cosp_radar.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     6082 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/llnl/llnl_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5703 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/llnl/pf_to_mr.f
--rw-r--r--   0 peter     (1000) peter     (1000)     9585 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/llnl/prec_scops.f
--rw-r--r--   0 peter     (1000) peter     (1000)    75040 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/mac_info.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     1317 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/predict_mom07.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.097308 alcf-1.4.1.post1/cosp/quickbeam/
--rw-r--r--   0 peter     (1000) peter     (1000)     1563 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/README
--rw-r--r--   0 peter     (1000) peter     (1000)     4166 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/array_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     5500 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/atmos_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     7260 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/calc_Re.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    10671 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/dsd.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4282 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/format_input.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     7774 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/gases.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     1665 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/load_hydrometeor_classes.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     1761 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/load_mie_table.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     9299 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/math_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    17248 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/mrgrnk.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    36058 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/optics_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4211 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/predict_psd07.f
--rw-r--r--   0 peter     (1000) peter     (1000)    18284 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/radar_simulator.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4867 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/radar_simulator_init.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     2934 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/radar_simulator_types.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4039 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/scale_LUTs_io.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4852 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/quickbeam/zeff.f90
--rwxr-xr-x   0 peter     (1000) peter     (1000)      143 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/replace_tabs.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)      196 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/tests.sh
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.097308 alcf-1.4.1.post1/cosp/utils/
--rwxr-xr-x   0 peter     (1000) peter     (1000)     8682 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/utils/COSP_plots.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)     3379 2021-11-30 13:13:22.000000 alcf-1.4.1.post1/cosp/utils/append_cf3hr_files.sh
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.085308 alcf-1.4.1.post1/dist/
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.085308 alcf-1.4.1.post1/dist/alcf-1.4.1/
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.085308 alcf-1.4.1.post1/dist/alcf-1.4.1/alcf/
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.097308 alcf-1.4.1.post1/dist/alcf-1.4.1/alcf/algorithms/
--rw-r--r--   0 peter     (1000) peter     (1000)     1018 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/dist/alcf-1.4.1/alcf/algorithms/interp.pyx
--rwxr-xr-x   0 peter     (1000) peter     (1000)      326 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/download_cosp
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.097308 alcf-1.4.1.post1/man/
--rw-r--r--   0 peter     (1000) peter     (1000)     4118 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/man/alcf-auto.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2261 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/man/alcf-calibrate.1
--rw-r--r--   0 peter     (1000) peter     (1000)      792 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/man/alcf-compare.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1985 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/man/alcf-convert.1
--rw-r--r--   0 peter     (1000) peter     (1000)     5366 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/man/alcf-lidar.1
--rw-r--r--   0 peter     (1000) peter     (1000)     3035 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/man/alcf-model.1
--rw-r--r--   0 peter     (1000) peter     (1000)     5220 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/man/alcf-plot.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1962 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/man/alcf-simulate.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2965 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/man/alcf-stats.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1390 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/man/alcf.1
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-04-21 22:06:40.101308 alcf-1.4.1.post1/setup.cfg
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1977 2023-04-21 22:06:35.000000 alcf-1.4.1.post1/setup.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:06:40.101308 alcf-1.4.1.post1/src/
--rw-r--r--   0 peter     (1000) peter     (1000)    12585 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/src/cosp_run.f03
--rw-r--r--   0 peter     (1000) peter     (1000)    10920 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/src/main.f03
--rw-r--r--   0 peter     (1000) peter     (1000)     8501 2023-04-21 19:23:28.000000 alcf-1.4.1.post1/src/nc_utils.f03
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.651363 alcf-1.5.0/
+-rw-r--r--   0 peter     (1000) peter     (1000)      239 2023-04-22 13:41:56.000000 alcf-1.5.0/.editorconfig
+-rw-r--r--   0 peter     (1000) peter     (1000)     1144 2023-04-22 13:41:56.000000 alcf-1.5.0/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)      181 2023-04-22 13:41:56.000000 alcf-1.5.0/MANIFEST.in
+-rw-r--r--   0 peter     (1000) peter     (1000)     1275 2023-04-22 13:41:56.000000 alcf-1.5.0/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)     1016 2023-04-22 13:43:47.651363 alcf-1.5.0/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      764 2023-04-22 13:41:56.000000 alcf-1.5.0/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.639364 alcf-1.5.0/alcf/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.639364 alcf-1.5.0/alcf/algorithms/
+-rw-r--r--   0 peter     (1000) peter     (1000)       27 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.639364 alcf-1.5.0/alcf/algorithms/calibration/
+-rw-r--r--   0 peter     (1000) peter     (1000)       62 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/calibration/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      373 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/calibration/default.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.639364 alcf-1.5.0/alcf/algorithms/cloud_base_detection/
+-rw-r--r--   0 peter     (1000) peter     (1000)       71 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/cloud_base_detection/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      930 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/cloud_base_detection/default.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.639364 alcf-1.5.0/alcf/algorithms/cloud_detection/
+-rw-r--r--   0 peter     (1000) peter     (1000)       66 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/cloud_detection/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      798 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/cloud_detection/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2029 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/couple.py
+-rw-r--r--   0 peter     (1000) peter     (1000)   259682 2023-04-22 13:43:47.000000 alcf-1.5.0/alcf/algorithms/interp.c
+-rw-r--r--   0 peter     (1000) peter     (1000)     1018 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/interp.pyx
+-rw-r--r--   0 peter     (1000) peter     (1000)      781 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/lidar_ratio.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.639364 alcf-1.5.0/alcf/algorithms/noise_removal/
+-rw-r--r--   0 peter     (1000) peter     (1000)       64 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/noise_removal/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      981 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/noise_removal/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1682 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/output_sample.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     9415 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/stats.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1120 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/tsample.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1776 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/algorithms/zsample.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.643364 alcf-1.5.0/alcf/cmds/
+-rw-r--r--   0 peter     (1000) peter     (1000)      408 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/cmds/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3555 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/cmds/auto.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.643364 alcf-1.5.0/alcf/cmds/auto_cmds/
+-rw-r--r--   0 peter     (1000) peter     (1000)      141 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/cmds/auto_cmds/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      843 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/cmds/auto_cmds/compare.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1671 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/cmds/auto_cmds/lidar.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1086 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/cmds/auto_cmds/model.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2804 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/cmds/calibrate.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2148 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/cmds/compare.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3429 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/cmds/convert.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    10693 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/cmds/lidar.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1395 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/cmds/main.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6342 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/cmds/model.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    17038 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/cmds/plot.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6424 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/cmds/simulate.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3569 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/cmds/stats.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.643364 alcf-1.5.0/alcf/fonts/
+-rw-r--r--   0 peter     (1000) peter     (1000)     6709 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/fonts/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    56032 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/fonts/PublicSans-Bold.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    60100 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/fonts/PublicSans-BoldItalic.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    60316 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/fonts/PublicSans-Italic.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    56792 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/fonts/PublicSans-Regular.otf
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.643364 alcf-1.5.0/alcf/lidars/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1426 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/lidars/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2033 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/lidars/blview.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      101 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/lidars/caliop.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1632 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/lidars/chm15k.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      410 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/lidars/cl31.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2157 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/lidars/cl51.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1709 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/lidars/cl61.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      996 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/lidars/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3358 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/lidars/mpl.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1873 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/lidars/mpl2nc.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3900 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/misc.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.643364 alcf-1.5.0/alcf/models/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2156 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/models/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2283 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/models/amps.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      359 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/models/cmip5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2680 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/models/era5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2516 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/models/icon.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2755 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/models/jra55.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1832 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/models/merra2.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2042 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/models/nzcsm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3121 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/models/nzesm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2375 2023-04-22 13:41:56.000000 alcf-1.5.0/alcf/models/um.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.639364 alcf-1.5.0/alcf.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1016 2023-04-22 13:43:47.000000 alcf-1.5.0/alcf.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     4492 2023-04-22 13:43:47.000000 alcf-1.5.0/alcf.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-22 13:43:47.000000 alcf-1.5.0/alcf.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-22 13:43:47.000000 alcf-1.5.0/alcf.egg-info/not-zip-safe
+-rw-r--r--   0 peter     (1000) peter     (1000)      158 2023-04-22 13:43:47.000000 alcf-1.5.0/alcf.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        5 2023-04-22 13:43:47.000000 alcf-1.5.0/alcf.egg-info/top_level.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.643364 alcf-1.5.0/bin/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      282 2023-04-22 13:41:56.000000 alcf-1.5.0/bin/alcf
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1677 2023-04-22 13:41:56.000000 alcf-1.5.0/build_doc
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.647364 alcf-1.5.0/cosp/
+-rw-r--r--   0 peter     (1000) peter     (1000)      260 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/.editorconfig
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.647364 alcf-1.5.0/cosp/MISR_simulator/
+-rw-r--r--   0 peter     (1000) peter     (1000)    16546 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/MISR_simulator/MISR_simulator.f
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.647364 alcf-1.5.0/cosp/MODIS_simulator/
+-rw-r--r--   0 peter     (1000) peter     (1000)    64835 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/MODIS_simulator/modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7387 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/MODIS_simulator/test_modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5167 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)     7506 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/Makefile.cmor1
+-rw-r--r--   0 peter     (1000) peter     (1000)     7515 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/Makefile.ibm
+-rw-r--r--   0 peter     (1000) peter     (1000)      936 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/README.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    48320 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/README.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      467 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/README_v1.4.1.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.647364 alcf-1.5.0/cosp/actsim/
+-rw-r--r--   0 peter     (1000) peter     (1000)    35248 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/actsim/lidar_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    38101 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/actsim/lmd_ipsl_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11672 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/actsim/mie_backscatter_1064.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11571 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/actsim/mie_backscatter_532.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11642 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/actsim/mie_backscatter_910.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.647364 alcf-1.5.0/cosp/cfmip2/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2508 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     2487 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     7271 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     7400 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     3320 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     3261 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    31979 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    15220 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_constants.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1881 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_defs.h
+-rw-r--r--   0 peter     (1000) peter     (1000)     2644 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_htfrtc.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     6934 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_input_nl.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    40704 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_io.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4292 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_isccp_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4123 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_lidar.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     3561 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_misr_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    25019 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     3646 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_output_nl.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    26091 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_rttov.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5694 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_rttov_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     9657 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    13744 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    70109 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_types.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    13287 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/cosp_utils.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.647364 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2957 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)    59127 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/README
+-rw-r--r--   0 peter     (1000) peter     (1000)      165 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/congvec.expected
+-rw-r--r--   0 peter     (1000) peter     (1000)     2545 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/congvec.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    43978 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/icarus.f
+-rw-r--r--   0 peter     (1000) peter     (1000)      869 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/input.data
+-rw-r--r--   0 peter     (1000) peter     (1000)     1042 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/input.data.halved
+-rw-r--r--   0 peter     (1000) peter     (1000)    13495 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     1845 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/license
+-rwxr-xr-x   0 peter     (1000) peter     (1000)       15 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/rcsid
+-rw-r--r--   0 peter     (1000) peter     (1000)    11849 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/scops.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     2539 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/test_congvec.f
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     2660 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh
+-rw-r--r--   0 peter     (1000) peter     (1000)    13385 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     3095 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.651363 alcf-1.5.0/cosp/llnl/
+-rw-r--r--   0 peter     (1000) peter     (1000)     7918 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/llnl/cosp_radar.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     6082 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/llnl/llnl_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5703 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/llnl/pf_to_mr.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     9585 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/llnl/prec_scops.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    75040 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/mac_info.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     1317 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/predict_mom07.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.651363 alcf-1.5.0/cosp/quickbeam/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1563 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/README
+-rw-r--r--   0 peter     (1000) peter     (1000)     4166 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/array_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5500 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/atmos_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7260 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/calc_Re.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    10671 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/dsd.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4282 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/format_input.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7774 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/gases.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1665 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/load_hydrometeor_classes.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1761 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/load_mie_table.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     9299 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/math_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    17248 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/mrgrnk.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    36058 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/optics_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4211 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/predict_psd07.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    18284 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/radar_simulator.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4867 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/radar_simulator_init.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     2934 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/radar_simulator_types.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4039 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/scale_LUTs_io.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4852 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/quickbeam/zeff.f90
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      143 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/replace_tabs.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      196 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/tests.sh
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.651363 alcf-1.5.0/cosp/utils/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     8682 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/utils/COSP_plots.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     3379 2023-04-22 09:28:05.000000 alcf-1.5.0/cosp/utils/append_cf3hr_files.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      326 2023-04-22 13:41:56.000000 alcf-1.5.0/download_cosp
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.651363 alcf-1.5.0/man/
+-rw-r--r--   0 peter     (1000) peter     (1000)     4118 2023-04-22 13:41:56.000000 alcf-1.5.0/man/alcf-auto.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2261 2023-04-22 13:41:56.000000 alcf-1.5.0/man/alcf-calibrate.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      792 2023-04-22 13:41:56.000000 alcf-1.5.0/man/alcf-compare.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1985 2023-04-22 13:41:56.000000 alcf-1.5.0/man/alcf-convert.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     5366 2023-04-22 13:41:56.000000 alcf-1.5.0/man/alcf-lidar.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     3035 2023-04-22 13:41:56.000000 alcf-1.5.0/man/alcf-model.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     5220 2023-04-22 13:41:56.000000 alcf-1.5.0/man/alcf-plot.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1962 2023-04-22 13:41:56.000000 alcf-1.5.0/man/alcf-simulate.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2965 2023-04-22 13:41:56.000000 alcf-1.5.0/man/alcf-stats.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1390 2023-04-22 13:41:56.000000 alcf-1.5.0/man/alcf.1
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-04-22 13:43:47.651363 alcf-1.5.0/setup.cfg
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1971 2023-04-22 13:41:56.000000 alcf-1.5.0/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 13:43:47.651363 alcf-1.5.0/src/
+-rw-r--r--   0 peter     (1000) peter     (1000)    12585 2023-04-22 13:41:56.000000 alcf-1.5.0/src/cosp_run.f03
+-rw-r--r--   0 peter     (1000) peter     (1000)    11128 2023-04-22 13:41:56.000000 alcf-1.5.0/src/main.f03
+-rw-r--r--   0 peter     (1000) peter     (1000)     8501 2023-04-22 13:41:56.000000 alcf-1.5.0/src/nc_utils.f03
```

### Comparing `alcf-1.4.1.post1/LICENSE.md` & `alcf-1.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/Makefile` & `alcf-1.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/PKG-INFO` & `alcf-1.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alcf
-Version: 1.4.1.post1
+Version: 1.5.0
 Summary: Automatic Lidar and Ceilometer Framework (ALCF)
 Home-page: https://alcf.peterkuma.net
 Author: Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn
 Author-email: peter@peterkuma.net
 License: MIT
 Description: UNKNOWN
 Keywords: alc,ceilometer,lidar,atmosphere,model,simulator,nwp,gcm,cosp,actsim,vaisala,cl51,cl31,lufft,chm-15k,minimpl,amps,merra-2,um
```

### Comparing `alcf-1.4.1.post1/README.md` & `alcf-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/algorithms/cloud_base_detection/default.py` & `alcf-1.5.0/alcf/algorithms/cloud_base_detection/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/algorithms/cloud_detection/default.py` & `alcf-1.5.0/alcf/algorithms/cloud_detection/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/algorithms/couple.py` & `alcf-1.5.0/alcf/algorithms/couple.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/algorithms/interp.c` & `alcf-1.5.0/alcf/algorithms/interp.c`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/algorithms/interp.pyx` & `alcf-1.5.0/alcf/algorithms/interp.pyx`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/algorithms/lidar_ratio.py` & `alcf-1.5.0/alcf/algorithms/lidar_ratio.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/algorithms/noise_removal/default.py` & `alcf-1.5.0/alcf/algorithms/noise_removal/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/algorithms/output_sample.py` & `alcf-1.5.0/alcf/algorithms/output_sample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/algorithms/stats.py` & `alcf-1.5.0/alcf/algorithms/stats.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/algorithms/tsample.py` & `alcf-1.5.0/alcf/algorithms/tsample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/algorithms/zsample.py` & `alcf-1.5.0/alcf/algorithms/zsample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/cmds/auto.py` & `alcf-1.5.0/alcf/cmds/auto.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/cmds/auto_cmds/compare.py` & `alcf-1.5.0/alcf/cmds/auto_cmds/compare.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/cmds/auto_cmds/lidar.py` & `alcf-1.5.0/alcf/cmds/auto_cmds/lidar.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/cmds/auto_cmds/model.py` & `alcf-1.5.0/alcf/cmds/auto_cmds/model.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/cmds/calibrate.py` & `alcf-1.5.0/alcf/cmds/calibrate.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/cmds/compare.py` & `alcf-1.5.0/alcf/cmds/compare.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/cmds/convert.py` & `alcf-1.5.0/alcf/cmds/convert.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/cmds/lidar.py` & `alcf-1.5.0/alcf/cmds/lidar.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/cmds/main.py` & `alcf-1.5.0/alcf/cmds/main.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/cmds/model.py` & `alcf-1.5.0/alcf/cmds/model.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/cmds/plot.py` & `alcf-1.5.0/alcf/cmds/plot.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/cmds/simulate.py` & `alcf-1.5.0/alcf/cmds/simulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	config%RADAR_FREQ=94.0,
 	config%SURFACE_RADAR=0,
 	config%use_mie_tables=0,
 	config%use_gas_abs=1,
 	config%do_ray=0,
 	config%melt_lay=0,
 	config%k2=-1,
-	config%use_reff=.false.,
+	config%use_reff=.true.,
 	config%use_precipitation_fluxes=.false.,
 	config%Nprmts_max_hydro=12,
 	config%Naero=1,
 	config%Nprmts_max_aero=1,
 	config%lidar_ice_type=0,
 	config%lidar_wavelength=${wavelength},
 	config%lidar_max_range=${max_range},
```

### Comparing `alcf-1.4.1.post1/alcf/cmds/stats.py` & `alcf-1.5.0/alcf/cmds/stats.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/fonts/LICENSE.md` & `alcf-1.5.0/alcf/fonts/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/fonts/PublicSans-Bold.otf` & `alcf-1.5.0/alcf/fonts/PublicSans-Bold.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/fonts/PublicSans-BoldItalic.otf` & `alcf-1.5.0/alcf/fonts/PublicSans-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/fonts/PublicSans-Italic.otf` & `alcf-1.5.0/alcf/fonts/PublicSans-Italic.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/fonts/PublicSans-Regular.otf` & `alcf-1.5.0/alcf/fonts/PublicSans-Regular.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/lidars/__init__.py` & `alcf-1.5.0/alcf/lidars/__init__.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/lidars/blview.py` & `alcf-1.5.0/alcf/lidars/blview.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/lidars/chm15k.py` & `alcf-1.5.0/alcf/lidars/chm15k.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/lidars/cl51.py` & `alcf-1.5.0/alcf/lidars/cl51.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/lidars/cl61.py` & `alcf-1.5.0/alcf/lidars/cl61.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/lidars/default.py` & `alcf-1.5.0/alcf/lidars/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/lidars/mpl.py` & `alcf-1.5.0/alcf/lidars/mpl.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/lidars/mpl2nc.py` & `alcf-1.5.0/alcf/lidars/mpl2nc.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/misc.py` & `alcf-1.5.0/alcf/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,17 +90,17 @@
 	n = len(time)
 	bnds = np.full((n, 2), np.nan, time.dtype)
 	bnds[:,0] = time - step*0.5
 	bnds[:,1] = time + step*0.5
 	bnds[1:,0] = np.maximum(bnds[:-1,1], bnds[1:,0])
 	bnds[:-1,1] = np.minimum(bnds[1:,0], bnds[:-1,1])
 	if start is not None:
-		bnds[0,0] = start
+		bnds[0,0] = max(bnds[0,0], start)
 	if end is not None:
-		bnds[-1,1] = end
+		bnds[-1,1] = min(bnds[-1,1], end)
 	return bnds
 
 def sun_altitude(t, lon, lat):
 	loc = astropy.coordinates.EarthLocation(
 		lon=lon*astropy.units.deg,
 		lat=lat*astropy.units.deg
 	)
```

### Comparing `alcf-1.4.1.post1/alcf/models/__init__.py` & `alcf-1.5.0/alcf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/alcf/models/amps.py` & `alcf-1.5.0/alcf/models/amps.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,21 +19,28 @@
 	'HGT',
 	'XTIME',
 	'XLONG',
 	'XLAT',
 	'T',
 ]
 
+def index(dirname, warnings=[], recursive=False, njobs=1):
+	return ds.readdir(dirname, ['XTIME'],
+		jd=True,
+		recursive=recursive,
+		warnings=warnings,
+		parallel=(njobs > 1),
+		njobs=njobs,
+	)
+
 def read(dirname, index, track, warnings=[], step=3./24., recursive=False):
-	dd_index = ds.readdir(dirname, variables=['XTIME'], jd=True,
-		recursive=recursive)
 	start_time = track['time'][0]
 	end_time = track['time'][-1]
 	dd = []
-	for d_index in dd_index:
+	for d_index in index:
 		time = d_index['XTIME'][0]
 		time0 = d_index['.']['.']['SIMULATION_START_DATE']
 		time0 = aq.from_iso(time0.replace('_', 'T'))
 		if time < 2000000.:
 			time = time0 + time/(24.*60.)
 		filename = d_index['filename']
 		if (time >= start_time - step*0.5) & (time < end_time + step*0.5):
@@ -71,10 +78,9 @@
 				'time': np.array([time]),
 				'.': META,
 			}
 			dd.append(d_new)
 	d = ds.op.merge(dd, 'time')
 	if 'time' in d:
 		d['time_bnds'] = misc.time_bnds(d['time'], step, start_time, end_time)
-		d['time'] = np.mean(d['time_bnds'], axis=1)
 	d['.'] = META
 	return d
```

### Comparing `alcf-1.4.1.post1/alcf/models/era5.py` & `alcf-1.5.0/alcf/models/era5.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,15 +103,14 @@
 				d['ta'] = d['ta'][:,::-1]
 				d['zfull'] = d['zfull'][:,::-1]
 				d['pfull'] = d['pfull'][:,::-1]
 			dd.append(d)
 	d = ds.op.merge(dd, 'time')
 	if 'time' in d:
 		d['time_bnds'] = misc.time_bnds(d['time'], step, start_time, end_time)
-		d['time'] = np.mean(d['time_bnds'], axis=1)
 	if 'pfull' in d:
 		d['pfull'] = 1e2*d['pfull']
 	if 'zfull' in d:
 		d['zfull'] /= 9.80665
 	if 'orog' in d:
 		d['orog'] /= 9.80665
 	if 'cl' in d:
```

### Comparing `alcf-1.4.1.post1/alcf/models/icon.py` & `alcf-1.5.0/alcf/models/icon.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,11 +99,10 @@
 		ii = [t in time for t in d['time']]
 		ds.select(d, {'time': ii})
 		d_out.update(d)
 
 	d_out['cl'] = np.full(d_out['cli'].shape, 100., np.float64)
 	if 'time' in d_out:
 		d_out['time_bnds'] = misc.time_bnds(d_out['time'], step, start_time, end_time)
-		d_out['time'] = np.mean(d_out['time_bnds'], axis=1)
 	d_out['.'] = META
 
 	return d_out
```

### Comparing `alcf-1.4.1.post1/alcf/models/jra55.py` & `alcf-1.5.0/alcf/models/jra55.py`

 * *Files 7% similar despite different names*

```diff
@@ -108,10 +108,9 @@
 				and TRANS[var_aux] in ds.get_vars(d) \
 				and not np.all(d_out[TRANS[var_aux]] == d[TRANS[var_aux]]):
 				raise ValueError('%s: Field differs between input files' % TRANS[var_aux])
 		d_out.update(d)
 	d_out['pfull'] = d_out['pfull']*1e2
 	if 'time' in d_out:
 		d_out['time_bnds'] = misc.time_bnds(d_out['time'], step, start_time, end_time)
-		d_out['time'] = np.mean(d_out['time_bnds'], axis=1)
 	d_out['.'] = META
 	return d_out
```

### Comparing `alcf-1.4.1.post1/alcf/models/merra2.py` & `alcf-1.5.0/alcf/models/merra2.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,10 +69,9 @@
 				'time': np.array([t]),
 				'.': META,
 			}
 			dd.append(d_new)
 	d = ds.op.merge(dd, 'time')
 	if 'time' in d:
 		d['time_bnds'] = misc.time_bnds(d['time'], step, start_time, end_time)
-		d['time'] = np.mean(d['time_bnds'], axis=1)
 	d['.'] = META
 	return d
```

### Comparing `alcf-1.4.1.post1/alcf/models/nzcsm.py` & `alcf-1.5.0/alcf/models/nzcsm.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,9 +63,9 @@
 				'lat': np.array([lat[j,k]]),
 				'time': np.array([time[i]]),
 				'.': META,
 			}
 			dd.append(d_new)
 	d = ds.op.merge(dd, 'time')
 	if 'time' in d:
-		d['time_bnds'] = misc.time_bnds(d['time'], step)
+		d['time_bnds'] = misc.time_bnds(d['time'], step, start_time, end_time)
 	return d
```

### Comparing `alcf-1.4.1.post1/alcf/models/nzesm.py` & `alcf-1.5.0/alcf/models/nzesm.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,10 +101,10 @@
 	del d['level_height']
 	if 'orog' not in d:
 		n, m = d['zfull'].shape
 		d['orog'] = np.full(n, np.nan, dtype=np.float64)
 		for i in range(n):
 			d['orog'][i] = 2*d['zfull'][i,0] - d['zfull'][i,1]
 	if 'time' in d:
-		d['time_bnds'] = misc.time_bnds(d['time'], step)
+		d['time_bnds'] = misc.time_bnds(d['time'], step, start_time, end_time)
 	d['.'] = META
 	return d
```

### Comparing `alcf-1.4.1.post1/alcf/models/um.py` & `alcf-1.5.0/alcf/models/um.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,10 +89,9 @@
 			d['.']['orog'] = {'.dims': ['time']}
 			del d['eta']
 			dd.append(d)
 	d = ds.op.merge(dd, 'time')
 	d['cl'] *= 100.
 	if 'time' in d:
 		d['time_bnds'] = misc.time_bnds(d['time'], step, start_time, end_time)
-		d['time'] = np.mean(d['time_bnds'], axis=1)
 	d['.'] = META
 	return d
```

### Comparing `alcf-1.4.1.post1/alcf.egg-info/PKG-INFO` & `alcf-1.5.0/alcf.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alcf
-Version: 1.4.1.post1
+Version: 1.5.0
 Summary: Automatic Lidar and Ceilometer Framework (ALCF)
 Home-page: https://alcf.peterkuma.net
 Author: Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn
 Author-email: peter@peterkuma.net
 License: MIT
 Description: UNKNOWN
 Keywords: alc,ceilometer,lidar,atmosphere,model,simulator,nwp,gcm,cosp,actsim,vaisala,cl51,cl31,lufft,chm-15k,minimpl,amps,merra-2,um
```

### Comparing `alcf-1.4.1.post1/alcf.egg-info/SOURCES.txt` & `alcf-1.5.0/alcf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 alcf/models/icon.py
 alcf/models/jra55.py
 alcf/models/merra2.py
 alcf/models/nzcsm.py
 alcf/models/nzesm.py
 alcf/models/um.py
 bin/alcf
+cosp/.editorconfig
 cosp/Makefile
 cosp/Makefile.cmor1
 cosp/Makefile.ibm
 cosp/README.md
 cosp/README.txt
 cosp/README_v1.4.1.txt
 cosp/cosp.F90
@@ -148,15 +149,14 @@
 cosp/quickbeam/radar_simulator.f90
 cosp/quickbeam/radar_simulator_init.f90
 cosp/quickbeam/radar_simulator_types.f90
 cosp/quickbeam/scale_LUTs_io.f90
 cosp/quickbeam/zeff.f90
 cosp/utils/COSP_plots.py
 cosp/utils/append_cf3hr_files.sh
-dist/alcf-1.4.1/alcf/algorithms/interp.pyx
 man/alcf-auto.1
 man/alcf-calibrate.1
 man/alcf-compare.1
 man/alcf-convert.1
 man/alcf-lidar.1
 man/alcf-model.1
 man/alcf-plot.1
```

### Comparing `alcf-1.4.1.post1/build_doc` & `alcf-1.5.0/build_doc`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/MISR_simulator/MISR_simulator.f` & `alcf-1.5.0/cosp/MISR_simulator/MISR_simulator.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/MODIS_simulator/modis_simulator.F90` & `alcf-1.5.0/cosp/MODIS_simulator/modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/MODIS_simulator/test_modis_simulator.F90` & `alcf-1.5.0/cosp/MODIS_simulator/test_modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/Makefile` & `alcf-1.5.0/cosp/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/Makefile.cmor1` & `alcf-1.5.0/cosp/Makefile.cmor1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/Makefile.ibm` & `alcf-1.5.0/cosp/Makefile.ibm`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/README.md` & `alcf-1.5.0/cosp/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -19,10 +19,14 @@
 - `lidar_wavelength` – Lidar wavelength (nm)
 
 See the original [README](README.txt) for more information.
 
 Release notes
 -------------
 
+### 1.1.0 (2023-04-22)
+
+- Radar scheme information is not printed to prevent output clutter.
+
 ### 1.0.0 (2021-11-30)
 
 - CMOR dependencies removed to simplify installation.
```

### Comparing `alcf-1.4.1.post1/cosp/README.txt` & `alcf-1.5.0/cosp/README.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/actsim/lidar_simulator.F90` & `alcf-1.5.0/cosp/actsim/lidar_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/actsim/lmd_ipsl_stats.F90` & `alcf-1.5.0/cosp/actsim/lmd_ipsl_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/actsim/mie_backscatter_1064.F90` & `alcf-1.5.0/cosp/actsim/mie_backscatter_1064.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/actsim/mie_backscatter_532.F90` & `alcf-1.5.0/cosp/actsim/mie_backscatter_532.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/actsim/mie_backscatter_910.F90` & `alcf-1.5.0/cosp/actsim/mie_backscatter_910.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt` & `alcf-1.5.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt` & `alcf-1.5.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt` & `alcf-1.5.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt` & `alcf-1.5.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt` & `alcf-1.5.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt` & `alcf-1.5.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp.F90` & `alcf-1.5.0/cosp/cosp.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp_constants.F90` & `alcf-1.5.0/cosp/cosp_constants.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp_defs.h` & `alcf-1.5.0/cosp/cosp_defs.h`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp_htfrtc.F90` & `alcf-1.5.0/cosp/cosp_htfrtc.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp_input_nl.txt` & `alcf-1.5.0/cosp/cosp_input_nl.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp_io.F90` & `alcf-1.5.0/cosp/cosp_io.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp_isccp_simulator.F90` & `alcf-1.5.0/cosp/cosp_isccp_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp_lidar.F90` & `alcf-1.5.0/cosp/cosp_lidar.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp_misr_simulator.F90` & `alcf-1.5.0/cosp/cosp_misr_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp_modis_simulator.F90` & `alcf-1.5.0/cosp/cosp_modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp_output_nl.txt` & `alcf-1.5.0/cosp/cosp_output_nl.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp_rttov.F90` & `alcf-1.5.0/cosp/cosp_rttov.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp_rttov_simulator.F90` & `alcf-1.5.0/cosp/cosp_rttov_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp_simulator.F90` & `alcf-1.5.0/cosp/cosp_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp_stats.F90` & `alcf-1.5.0/cosp/cosp_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/cosp_types.F90` & `alcf-1.5.0/cosp/cosp_types.F90`

 * *Files 0% similar despite different names*

```diff
@@ -1088,16 +1088,16 @@
 
     ! NOTE: This location use to contain initialization of some radar simulator variables
     ! this initialization (including use of the variable "dist_prmts_hydro" - now obselete) 
     ! has been unified in the quickbeam v3 subroutine "radar_simulator_init".   Roj, June 2010
 
     ! --- Initialize the distributional parameters for hydrometeors in radar simulator
 
-    write(*,*) 'RADAR_SIM microphysics scheme is set to: ', &
-            trim(RADAR_SIM_MICROPHYSICS_SCHEME_NAME)
+    !write(*,*) 'RADAR_SIM microphysics scheme is set to: ', &
+    !        trim(RADAR_SIM_MICROPHYSICS_SCHEME_NAME)
 
 
     if(y%Nhydro.ne.N_HYDRO) then
 
         write(*,*) 'Number of hydrometeor input to subroutine', &
                ' CONSTRUCT_COSP_GRIDBOX does not match value', &
                ' specified in cosp_constants.f90!'
```

### Comparing `alcf-1.4.1.post1/cosp/cosp_utils.F90` & `alcf-1.5.0/cosp/cosp_utils.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/Makefile` & `alcf-1.5.0/cosp/icarus-scops-4.1-bsd/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/README` & `alcf-1.5.0/cosp/icarus-scops-4.1-bsd/README`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/congvec.f` & `alcf-1.5.0/cosp/icarus-scops-4.1-bsd/congvec.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/icarus.f` & `alcf-1.5.0/cosp/icarus-scops-4.1-bsd/icarus.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/input.data` & `alcf-1.5.0/cosp/icarus-scops-4.1-bsd/input.data`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/input.data.halved` & `alcf-1.5.0/cosp/icarus-scops-4.1-bsd/input.data.halved`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f` & `alcf-1.5.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/license` & `alcf-1.5.0/cosp/icarus-scops-4.1-bsd/license`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/scops.f` & `alcf-1.5.0/cosp/icarus-scops-4.1-bsd/scops.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/test_congvec.f` & `alcf-1.5.0/cosp/icarus-scops-4.1-bsd/test_congvec.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/test_congvec.ksh` & `alcf-1.5.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f` & `alcf-1.5.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh` & `alcf-1.5.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/llnl/cosp_radar.F90` & `alcf-1.5.0/cosp/llnl/cosp_radar.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/llnl/llnl_stats.F90` & `alcf-1.5.0/cosp/llnl/llnl_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/llnl/pf_to_mr.f` & `alcf-1.5.0/cosp/llnl/pf_to_mr.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/llnl/prec_scops.f` & `alcf-1.5.0/cosp/llnl/prec_scops.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/mac_info.txt` & `alcf-1.5.0/cosp/mac_info.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/predict_mom07.F90` & `alcf-1.5.0/cosp/predict_mom07.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/README` & `alcf-1.5.0/cosp/quickbeam/README`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/array_lib.f90` & `alcf-1.5.0/cosp/quickbeam/array_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/atmos_lib.f90` & `alcf-1.5.0/cosp/quickbeam/atmos_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/calc_Re.f90` & `alcf-1.5.0/cosp/quickbeam/calc_Re.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/dsd.f90` & `alcf-1.5.0/cosp/quickbeam/dsd.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/format_input.f90` & `alcf-1.5.0/cosp/quickbeam/format_input.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/gases.f90` & `alcf-1.5.0/cosp/quickbeam/gases.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/load_hydrometeor_classes.f90` & `alcf-1.5.0/cosp/quickbeam/load_hydrometeor_classes.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/load_mie_table.f90` & `alcf-1.5.0/cosp/quickbeam/load_mie_table.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/math_lib.f90` & `alcf-1.5.0/cosp/quickbeam/math_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/mrgrnk.f90` & `alcf-1.5.0/cosp/quickbeam/mrgrnk.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/optics_lib.f90` & `alcf-1.5.0/cosp/quickbeam/optics_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/predict_psd07.f` & `alcf-1.5.0/cosp/quickbeam/predict_psd07.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/radar_simulator.f90` & `alcf-1.5.0/cosp/quickbeam/radar_simulator.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/radar_simulator_init.f90` & `alcf-1.5.0/cosp/quickbeam/radar_simulator_init.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/radar_simulator_types.f90` & `alcf-1.5.0/cosp/quickbeam/radar_simulator_types.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/scale_LUTs_io.f90` & `alcf-1.5.0/cosp/quickbeam/scale_LUTs_io.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/quickbeam/zeff.f90` & `alcf-1.5.0/cosp/quickbeam/zeff.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/utils/COSP_plots.py` & `alcf-1.5.0/cosp/utils/COSP_plots.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/cosp/utils/append_cf3hr_files.sh` & `alcf-1.5.0/cosp/utils/append_cf3hr_files.sh`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/man/alcf-auto.1` & `alcf-1.5.0/man/alcf-auto.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/man/alcf-calibrate.1` & `alcf-1.5.0/man/alcf-calibrate.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/man/alcf-compare.1` & `alcf-1.5.0/man/alcf-compare.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/man/alcf-convert.1` & `alcf-1.5.0/man/alcf-convert.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/man/alcf-lidar.1` & `alcf-1.5.0/man/alcf-lidar.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/man/alcf-model.1` & `alcf-1.5.0/man/alcf-model.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/man/alcf-plot.1` & `alcf-1.5.0/man/alcf-plot.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/man/alcf-simulate.1` & `alcf-1.5.0/man/alcf-simulate.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/man/alcf-stats.1` & `alcf-1.5.0/man/alcf-stats.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/man/alcf.1` & `alcf-1.5.0/man/alcf.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/setup.py` & `alcf-1.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	def run(self):
 		subprocess.run('make', cwd='cosp', check=True)
 		subprocess.run('make', check=True)
 		build_py.run(self)
 
 setup(
 	name='alcf',
-	version='1.4.1.post1',
+	version='1.5.0',
 	description='Automatic Lidar and Ceilometer Framework (ALCF)',
 	author='Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn',
 	author_email='peter@peterkuma.net',
 	license='MIT',
 	scripts=['bin/alcf'],
 	packages=find_packages(),
 	ext_modules=cythonize('alcf/algorithms/interp.pyx', language_level=3),
```

### Comparing `alcf-1.4.1.post1/src/cosp_run.f03` & `alcf-1.5.0/src/cosp_run.f03`

 * *Files identical despite different names*

### Comparing `alcf-1.4.1.post1/src/main.f03` & `alcf-1.5.0/src/main.f03`

 * *Files 12% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         nhydro = N_HYDRO
 
         call allocate_cosp_input_fields(input, npoints, nlev)
 
         input%npoints = npoints
         input%nlevels = nlev
         input%emsfc_lw = 1.
+        input%Reff = 10e-6
         input%time = 1.
         input%lon = lon
         input%lat = lat
         input%orog = orog
         input%T = transpose(ta)
         input%p = transpose(pfull)
         input%tca = transpose(cl)*0.01
@@ -155,51 +156,51 @@
 
         call nc_check(nf90_create(file, 0, ncid))
         call nc_check(nf90_def_dim(ncid, 'time', npoints, time_dimid))
         call nc_check(nf90_def_dim(ncid, 'bnds', 2, bnds_dimid))
         call nc_check(nf90_def_dim(ncid, 'level', nlevels, level_dimid))
         call nc_check(nf90_def_dim(ncid, 'column', ncolumns, column_dimid))
         call nc_check(nf90_def_var(ncid, 'lon', nf90_double, time_dimid, lon_varid))
-	call nc_check(nf90_put_att(ncid, lon_varid, "long_name", "longitude"))
-	call nc_check(nf90_put_att(ncid, lon_varid, "standard_name", "longitude"))
-	call nc_check(nf90_put_att(ncid, lon_varid, "units", "degrees_east"))
+        call nc_check(nf90_put_att(ncid, lon_varid, "long_name", "longitude"))
+        call nc_check(nf90_put_att(ncid, lon_varid, "standard_name", "longitude"))
+        call nc_check(nf90_put_att(ncid, lon_varid, "units", "degrees_east"))
         call nc_check(nf90_def_var(ncid, 'lat', nf90_double, time_dimid, lat_varid))
-	call nc_check(nf90_put_att(ncid, lat_varid, "long_name", "latitude"))
-	call nc_check(nf90_put_att(ncid, lat_varid, "standard_name", "latitude"))
-	call nc_check(nf90_put_att(ncid, lat_varid, "units", "degrees_north"))
+        call nc_check(nf90_put_att(ncid, lat_varid, "long_name", "latitude"))
+        call nc_check(nf90_put_att(ncid, lat_varid, "standard_name", "latitude"))
+        call nc_check(nf90_put_att(ncid, lat_varid, "units", "degrees_north"))
         call nc_check(nf90_def_var(ncid, 'altitude', nf90_double, time_dimid, altitude_varid))
-	call nc_check(nf90_put_att(ncid, altitude_varid, "long_name", "instrument altitude"))
-	call nc_check(nf90_put_att(ncid, altitude_varid, "standard_name", "altitude"))
-	call nc_check(nf90_put_att(ncid, altitude_varid, "units", "m"))
+        call nc_check(nf90_put_att(ncid, altitude_varid, "long_name", "instrument altitude"))
+        call nc_check(nf90_put_att(ncid, altitude_varid, "standard_name", "altitude"))
+        call nc_check(nf90_put_att(ncid, altitude_varid, "units", "m"))
         call nc_check(nf90_def_var(ncid, 'zfull', nf90_double, (/level_dimid, time_dimid/), zlev_varid))
-	call nc_check(nf90_put_att(ncid, zlev_varid, "long_name", "altitude of model full-levels"))
-	call nc_check(nf90_put_att(ncid, zlev_varid, "standard_name", "height_above_reference_ellipsoid"))
-	call nc_check(nf90_put_att(ncid, zlev_varid, "units", "m"))
+        call nc_check(nf90_put_att(ncid, zlev_varid, "long_name", "altitude of model full-levels"))
+        call nc_check(nf90_put_att(ncid, zlev_varid, "standard_name", "height_above_reference_ellipsoid"))
+        call nc_check(nf90_put_att(ncid, zlev_varid, "units", "m"))
         !call nc_check(nf90_def_var(ncid, 'zhalf', nf90_double, (/level_dimid, time_dimid/), zlev_half_varid))
         call nc_check(nf90_def_var(ncid, 'pfull', nf90_double, (/level_dimid, time_dimid/), p_varid))
-	call nc_check(nf90_put_att(ncid, p_varid, "long_name", "pressure at model full-levels"))
-	call nc_check(nf90_put_att(ncid, p_varid, "standard_name", "air_pressure"))
-	call nc_check(nf90_put_att(ncid, p_varid, "units", "Pa"))
+        call nc_check(nf90_put_att(ncid, p_varid, "long_name", "pressure at model full-levels"))
+        call nc_check(nf90_put_att(ncid, p_varid, "standard_name", "air_pressure"))
+        call nc_check(nf90_put_att(ncid, p_varid, "units", "Pa"))
         !call nc_check(nf90_def_var(ncid, 'phalf', nf90_double, (/level_dimid, time_dimid/), ph_varid))
         call nc_check(nf90_def_var(ncid, 'backscatter', nf90_double, (/column_dimid, level_dimid, time_dimid/), beta_tot_varid))
-	call nc_check(nf90_put_att(ncid, beta_tot_varid, "long_name", "total attenuated volume backscattering coefficient"))
-	call nc_check(nf90_put_att(ncid, beta_tot_varid, "units", "m-1 sr-1"))
+        call nc_check(nf90_put_att(ncid, beta_tot_varid, "long_name", "total attenuated volume backscattering coefficient"))
+        call nc_check(nf90_put_att(ncid, beta_tot_varid, "units", "m-1 sr-1"))
         call nc_check(nf90_def_var(ncid, 'backscatter_mol', nf90_double, (/level_dimid, time_dimid/), beta_mol_varid))
-	call nc_check(nf90_put_att(ncid, beta_mol_varid, "long_name", "total attenuated molecular volume backscattering coefficient"))
-	call nc_check(nf90_put_att(ncid, beta_mol_varid, "units", "m-1 sr-1"))
+        call nc_check(nf90_put_att(ncid, beta_mol_varid, "long_name", "total attenuated molecular volume backscattering coefficient"))
+        call nc_check(nf90_put_att(ncid, beta_mol_varid, "units", "m-1 sr-1"))
         call nc_check(nf90_def_var(ncid, 'time', nf90_double, time_dimid, time_varid))
-	call nc_check(nf90_put_att(ncid, time_varid, "long_name", "time"))
-	call nc_check(nf90_put_att(ncid, time_varid, "standard_name", "time"))
-	call nc_check(nf90_put_att(ncid, time_varid, "units", "days since -4713-11-24 12:00 UTC"))
-	call nc_check(nf90_put_att(ncid, time_varid, "calendar", "proleptic_gregorian"))
+        call nc_check(nf90_put_att(ncid, time_varid, "long_name", "time"))
+        call nc_check(nf90_put_att(ncid, time_varid, "standard_name", "time"))
+        call nc_check(nf90_put_att(ncid, time_varid, "units", "days since -4713-11-24 12:00 UTC"))
+        call nc_check(nf90_put_att(ncid, time_varid, "calendar", "proleptic_gregorian"))
         call nc_check(nf90_def_var(ncid, 'time_bnds', nf90_double, (/bnds_dimid, time_dimid/), time_bnds_varid))
-	call nc_check(nf90_put_att(ncid, time_bnds_varid, "long_name", "time bounds"))
-	call nc_check(nf90_put_att(ncid, time_bnds_varid, "standard_name", "time"))
-	call nc_check(nf90_put_att(ncid, time_bnds_varid, "units", "days since -4713-11-24 12:00 UTC"))
-	call nc_check(nf90_put_att(ncid, time_bnds_varid, "calendar", "proleptic_gregorian"))        
+        call nc_check(nf90_put_att(ncid, time_bnds_varid, "long_name", "time bounds"))
+        call nc_check(nf90_put_att(ncid, time_bnds_varid, "standard_name", "time"))
+        call nc_check(nf90_put_att(ncid, time_bnds_varid, "units", "days since -4713-11-24 12:00 UTC"))
+        call nc_check(nf90_put_att(ncid, time_bnds_varid, "calendar", "proleptic_gregorian"))
         call nc_check(nf90_enddef(ncid))
         call nc_check(nf90_put_var(ncid, lon_varid, input%lon))
         call nc_check(nf90_put_var(ncid, lat_varid, input%lat))
         call nc_check(nf90_put_var(ncid, altitude_varid, input%orog))
         call nc_check(nf90_put_var(ncid, beta_tot_varid, reshape(output%sglidar%beta_tot, (/ncolumns, nlevels, npoints/), order=(/3,1,2/))))
         call nc_check(nf90_put_var(ncid, beta_mol_varid, reshape(output%sglidar%beta_mol, (/nlevels, npoints/), order=(/2,1/))))
         call nc_check(nf90_put_var(ncid, zlev_varid, reshape(input%zlev, (/nlevels, npoints/), order=(/2,1/))))
```

### Comparing `alcf-1.4.1.post1/src/nc_utils.f03` & `alcf-1.5.0/src/nc_utils.f03`

 * *Files identical despite different names*

