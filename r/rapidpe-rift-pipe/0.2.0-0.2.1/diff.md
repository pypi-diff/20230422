# Comparing `tmp/rapidpe_rift_pipe-0.2.0.tar.gz` & `tmp/rapidpe_rift_pipe-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.2.0.tar", last modified: Sat Apr 22 02:15:22 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.2.1.tar", last modified: Sat Apr 22 03:52:26 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.2.0.tar` & `rapidpe_rift_pipe-0.2.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.310191 rapidpe_rift_pipe-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-22 02:15:22.310191 rapidpe_rift_pipe-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.283192 rapidpe_rift_pipe-0.2.0/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.292192 rapidpe_rift_pipe-0.2.0/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)    10021 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6342 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     5579 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-22 02:15:22.313192 rapidpe_rift_pipe-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.285191 rapidpe_rift_pipe-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.302192 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    37420 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18297 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.307191 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.308192 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    31226 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    24280 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.309192 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.306192 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-22 02:15:22.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-04-22 02:15:22.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 02:15:22.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-22 02:15:22.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-04-22 02:15:22.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-22 02:15:22.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 02:15:21.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 03:52:26.148779 rapidpe_rift_pipe-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-22 03:52:26.149779 rapidpe_rift_pipe-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 03:52:26.144779 rapidpe_rift_pipe-0.2.1/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 03:52:26.145779 rapidpe_rift_pipe-0.2.1/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)    10021 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     5579 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-22 03:52:26.149779 rapidpe_rift_pipe-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 03:52:26.144779 rapidpe_rift_pipe-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 03:52:26.147779 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    37457 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18297 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 03:52:26.148779 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 03:52:26.148779 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31226 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    24280 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 03:52:26.148779 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-04-22 03:52:15.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 03:52:26.148779 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-22 03:52:26.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-04-22 03:52:26.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 03:52:26.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-22 03:52:26.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-04-22 03:52:26.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-22 03:52:26.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 03:52:25.000000 rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.2.0/COPYING` & `rapidpe_rift_pipe-0.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/PKG-INFO` & `rapidpe_rift_pipe-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_pipe
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.2.0/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.2.1/bin/postscripts/compute_posterior.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.2.1/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.2.1/bin/postscripts/cprofile_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.2.1/bin/postscripts/create_summarypage.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.2.1/bin/postscripts/plot_skymap.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/setup.cfg` & `rapidpe_rift_pipe-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,17 +388,17 @@
                 )
             # Put together cache file
             event_info["cache_file"] = data_cache_file_path
             event_info["psd_file"] = psd_file_str[:-1] + "]"
             event_info["channel_name"] = channel_str[:-1] + "]"
             event_info["coinc_xml_file"] = coinc_xml_filename
 
-            is_mdc = 'INJ' in event_info["channel_name"]
+            mdc_event_injection_file = config.event.mdc_event_injection_file
+            is_mdc = "INJ" in event_info["channel_name"] and mdc_event_injection_file is not None
             if is_mdc:
-                mdc_event_injection_file = config.event.mdc_event_injection_file
                 mdc_time_offset = int(config.event.mdc_time_offset)
                 mdc_xml_doc = ligolw_utils.load_filename(
                         mdc_event_injection_file,
                         contenthandler=ligolw.LIGOLWContentHandler,
                         )
                 mdc_sim_inspiral_tbl = lsctables.SimInspiralTable.get_table(mdc_xml_doc)
                 list_of_keys = ["gpstime","mass1","mass2","spin1z","spin2z","distance","latitude","longitude"]
```

### Comparing `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/pastro.py` & `rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/pastro.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe-rift-pipe
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.2.1/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

