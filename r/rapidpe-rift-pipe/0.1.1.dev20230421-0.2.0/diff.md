# Comparing `tmp/rapidpe_rift_pipe-0.1.1.dev20230421.tar.gz` & `tmp/rapidpe_rift_pipe-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.1.1.dev20230421.tar", last modified: Fri Apr 21 05:14:57 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.2.0.tar", last modified: Sat Apr 22 02:15:22 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.1.1.dev20230421.tar` & `rapidpe_rift_pipe-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.221358 rapidpe_rift_pipe-0.1.1.dev20230421/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1140 2023-04-21 05:14:57.221358 rapidpe_rift_pipe-0.1.1.dev20230421/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.215358 rapidpe_rift_pipe-0.1.1.dev20230421/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.217358 rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)     9851 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6348 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     7839 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3643 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1449 2023-04-21 05:14:57.221358 rapidpe_rift_pipe-0.1.1.dev20230421/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.215358 rapidpe_rift_pipe-0.1.1.dev20230421/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.219358 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    37438 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18220 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.220358 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.220358 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    31369 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    24280 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.221358 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-04-21 05:14:47.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:14:57.220358 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1140 2023-04-21 05:14:57.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-04-21 05:14:57.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 05:14:57.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-21 05:14:57.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-04-21 05:14:57.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-21 05:14:57.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 05:14:57.000000 rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.310191 rapidpe_rift_pipe-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-22 02:15:22.310191 rapidpe_rift_pipe-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.283192 rapidpe_rift_pipe-0.2.0/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.292192 rapidpe_rift_pipe-0.2.0/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)    10021 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     5579 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-22 02:15:22.313192 rapidpe_rift_pipe-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.285191 rapidpe_rift_pipe-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.302192 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    37420 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18297 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.307191 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.308192 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31226 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    24280 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.309192 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-04-22 02:14:53.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 02:15:22.306192 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-22 02:15:22.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-04-22 02:15:22.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 02:15:22.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-22 02:15:22.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-04-22 02:15:22.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-22 02:15:22.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 02:15:21.000000 rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/COPYING` & `rapidpe_rift_pipe-0.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/PKG-INFO` & `rapidpe_rift_pipe-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_pipe
-Version: 0.1.1.dev20230421
+Version: 0.2.0
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.2.0/bin/postscripts/compute_posterior.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 print(f"Sigma values: {sigma_str}")
 if opts.output_dir:
     output_dir = opts.output_dir
 else:
     output_dir = input_dir
 
-summary_plots_dir = os.path.join(output_dir, "summary_plots")
+summary_plots_dir = os.path.join(output_dir, "summary")
 os.system(f"mkdir -p {summary_plots_dir}")
 
 f_lower = 40
 
 # Get injection/search point
 event_info = postutils.event_info(input_dir)
 event_info_dict = event_info.load_event_info()
@@ -178,27 +178,32 @@
     grid_data_dict, grid_param_list, sigma_factor, grid_level=use_grid_level
 )
 
 
 grid_levels = np.unique(grid_data_dict["iteration_level"])
 
 if config.pastro.mode == "enabled":
+    channel_names = event_info_dict['channel_name']
+    if 'INJ' in channel_names:
+        rate_dict = config.pastro.category_rates_inj
+    else:
+        rate_dict = config.pastro.category_rates
     prior_boundary_dict = config.pastro.prior_boundary
     evidence = postutils.compute_evidence(
         grid_data_dict,
         prior_boundary_dict,
         sigma_dict,
         distance_coordinates_str=distance_coordinates_str,
     )
 
     p_astro = pastro.pastro(
         evidence_dict=evidence,
         rankstatpdf_file=config.pastro.rankstat_pdf_file,
         likelihood=event_info_dict["likelihood"],
-        rate_dict=config.pastro.category_rates,
+        rate_dict=rate_dict,
         far_threshold=config.pastro.far_threshold,
     )
 
     pastro_dict = p_astro.compute_pastro()
     pastro.plot_pastro(pastro_dict, summary_plots_dir)
     utils.save_as_json(
         pastro_dict, os.path.join(summary_plots_dir, "p_astro.json")
```

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.2.0/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.2.0/bin/postscripts/cprofile_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 input_dir = opts.input_dir
 
 if opts.output_dir:
     run_dir = opts.output_dir
 else:
     run_dir = input_dir
-summary_plot_dir = os.path.join(run_dir, "summary_plots")
+summary_plot_dir = os.path.join(run_dir, "summary")
 
 cprofile_html_file = open(os.path.join(summary_plot_dir, "cprofile.html"), "w")
 print_output(
     cprofile_html_file,
     """
 <html>
 <head>
```

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.2.0/bin/postscripts/create_summarypage.py`

 * *Files 24% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 os.makedirs(output_dir, exist_ok=True)
 write_css_file(output_dir, "stylesheet.css")
 
 if opts.output_dir:
     run_dir = opts.output_dir
 else:
     run_dir = input_dir
-summary_plot_dir = os.path.join(run_dir, "summary_plots")
+summary_plot_dir = os.path.join(run_dir, "summary")
 
 os.system(f"cp {summary_plot_dir}/* {output_dir}/")
 print(f"Summary page will be saved in {output_dir}")
 index_html_file = os.path.join(output_dir, "summarypage.html")
 
 html_file = open(index_html_file, "w")
 
@@ -171,74 +171,11 @@
     for line in config_f:
         if line[0] != "#" and len(line.strip()) > 0:
             if line[0] == "[":
                 print_output(html_file, f"<br> <b> {line} </b>")
             else:
                 print_output(html_file, f"<br> {line}")
 
-print_output(html_file, "<h1> Convergence </h1>")
-header = [
-    "filename",
-    " iteration",
-    " Neff ",
-    " sqrt(2*lnLmax)",
-    " sqrt(2*lnLmarg)",
-    " ln(Z/Lmax)",
-    "int_var",
-]
-log_file_list = np.sort(glob(input_dir + "/logs/integrate*out"))
-convergence_data = np.ones(len(log_file_list)).tolist()
-for i, log_file in enumerate(log_file_list):
-    with open(log_file, "r") as f:
-        lines = f.readlines()
-        last_line = lines[-1]
-        if "Weight" in last_line:
-            last_line = lines[-3]
-        elif "neff" in last_line:
-            last_line = lines[-3]
-        log_filename = log_file.split("/")[-1]
-        data_list = last_line.split(" ")[1:]
-        data_list[0] = log_filename
-        convergence_data[i] = data_list
-print_output(
-    html_file, tabulate(convergence_data, headers=header, tablefmt="html")
-)
-
-grep_out = sp.getoutput("ls *")
-rescue_dags = glob(run_dir + "*rescue*")
-failed_job_ids = []
-if len(rescue_dags) != 0:
-    print_output(html_file, "<h1> Failed Jobs</h1>")
-    for i, dag in enumerate(rescue_dags):
-        with open(dag, "r") as f:
-            lines = f.readlines()
-            number_of_nodes_failed = int(
-                lines[7][len("# Nodes that failed: ") :]
-            )
-            list_of_nodes_failed = lines[8][len("#   ") :].split(",")[:-1]
-        print_output(
-            html_file,
-            f"{len(list_of_nodes_failed)} jobs" f" failed in level {i} <br>",
-        )
-        failed_job_ids.extend(list_of_nodes_failed)
-    print_output(html_file, "<h2> list of failed jobs </h2>")
-
-    for j, dag_job in enumerate(failed_job_ids):
-        cmd = f'grep "DAG Node: {dag_job}" {run_dir}logs/*log'
-        grep_out = sp.getoutput(cmd)
-        outfile_path = grep_out[: grep_out.find(".log")] + ".out"
-        print_output(html_file, "<details>")
-        print_output(
-            html_file, f"<summary> {j+1}) Job ID: {dag_job} </summary>"
-        )
-        print_output(html_file, f"path: {outfile_path} <br>")
-        print_output(html_file, "<pre>")
-        with open(outfile_path, "r") as f:
-            print_output(html_file, f.read())
-        print_output(html_file, "</pre>")
-        print_output(html_file, "</details>")
-    print_output(html_file, "</details>")
-
 
 print_output(html_file, "</body></html>")
 
 html_file.close()
```

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.2.0/bin/postscripts/plot_skymap.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from argparse import ArgumentParser
 from matplotlib import rcParams
 from astropy.coordinates import SkyCoord
 from glob import glob
 from ligo.skymap import plot
 from ligo.skymap import postprocess
+from ligo.skymap.io import fits
 
 import rapidpe_rift_pipe.postscript_utils as postutils
 
 optp = ArgumentParser()
 optp.add_argument("input_dir", help="path to event run dir")
 optp.add_argument(
     "--ratio-to-include",
@@ -44,15 +45,15 @@
     output_dir = input_dir
 
 
 namestr = ratio_to_include.replace(".", "p")
 filename = glob(
     input_dir + "/ll_samples_loudest_highweight_" + namestr + ".txt"
 )[0]
-os.makedirs(os.path.join(input_dir, "summary_plots"), exist_ok=True)
+os.makedirs(os.path.join(input_dir, "summary"), exist_ok=True)
 
 (
     mass1,
     mass2,
     mchirp,
     eta,
     spin1z,
@@ -86,18 +87,15 @@
 skymap = skymap / np.sum(skymap)
 skymapring = hp.pixelfunc.reorder(skymap, inp="NESTED", out="RING")
 sigma = 0.05  # smooting parameter
 skymapring = hp.sphtfunc.smoothing(skymapring, sigma=sigma)
 skymap = hp.pixelfunc.reorder(skymapring, inp="RING", out="NESTED")
 skymap[skymap < 0] = 0
 skymap = skymap / np.sum(skymap)
-np.savetxt(
-    f"{output_dir}/summary_plots/RapidPE_skymap_{namestr}.dat",
-    skymap,
-)
+fits.write_sky_map(f"{output_dir}/summary/skymap.fits.gz", skymap)
 
 
 deg2perpix = hp.nside2pixarea(nside, degrees=True)
 probperdeg2 = skymap / deg2perpix
 ax = plt.axes(projection="astro hours mollweide")
 ax.grid()
 vmax = probperdeg2.max()
@@ -133,8 +131,12 @@
         "*",
         markerfacecolor="white",
         markeredgecolor="black",
         markersize=10,
     )
 
 
-plt.savefig(f"{output_dir}/summary_plots/skymap_{namestr}.png")
+plt.savefig(f"{output_dir}/summary/skymap_{namestr}.png")
+np.savetxt(
+    f"{output_dir}/summary/RapidPE_skymap_{namestr}.dat",
+    skymap,
+)
```

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/setup.cfg` & `rapidpe_rift_pipe-0.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -49,10 +49,10 @@
 rapidpe_rift_pipe.config_files = *.ini, *.json
 
 [options.entry_points]
 console_scripts = 
 	rapidpe-rift-pipe = rapidpe_rift_pipe.cli:main
 
 [egg_info]
-tag_build = dev.20230421
+tag_build = 
 tag_date = 0
```

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,18 +127,14 @@
             if config.event.mode == 'sid':
                 sevent = client.superevent(config.event.superevent_id).json()
                 gracedb_id = sevent['preferred_event']
             elif config.event.mode == 'gid':
                 gracedb_id = config.event.gracedb_id
             else:
                 raise RuntimeError(f'Unknown mode {config.event.mode}')
-            mdc_event_injection_file = config.event.mdc_event_injection_file
-            is_mdc = mdc_event_injection_file is not None
-            if is_mdc:
-                mdc_time_offset = int(config.event.mdc_time_offset)
             gracedb_id = get_graceid_after_superevent_check(
                 gracedb_id, client,
                 output_parent_directory,
                 email_address_for_job_complete_notice,
             )
 
             event = client.event(gracedb_id).json()
@@ -157,33 +153,15 @@
             event_info["gracedb_id"] = gracedb_id
             event_info["event_time"] = construct_event_time_string(
                 params["end_time"], params["end_time_ns"],
             )
             event_info["snr"] = coinc["snr"]
             event_info["likelihood"] = event["likelihood"]
 
-            if is_mdc:
-                mdc_xml_doc = ligolw_utils.load_filename(
-                        mdc_event_injection_file,
-                        contenthandler=ligolw.LIGOLWContentHandler,
-                        )
-                mdc_sim_inspiral_tbl = lsctables.SimInspiralTable.get_table(mdc_xml_doc)
-                list_of_keys = ["gpstime","mass1","mass2","spin1z","spin2z","distance","latitude","longitude"]
-                mdc_data_dict = {k: [] for k in list_of_keys}
-                for row in mdc_sim_inspiral_tbl:
-                    for key in list_of_keys:
-                        if key== 'gpstime':
-                           mdc_data_dict[key].append(row.geocent_end_time + 1e-9 * row.geocent_end_time_ns)
-                        else:
-                            mdc_data_dict[key].append(getattr(row,key))
-                time_diff_from_injections = np.absolute(np.array(mdc_data_dict['gpstime'])-float(event_info['event_time'])+mdc_time_offset)
-                nearest_inj_index = np.argmin(time_diff_from_injections)
-                mdc_injection_info = {k:0 for k in list_of_keys}
-                for k in list_of_keys:
-                    mdc_injection_info[k] = mdc_data_dict[k][nearest_inj_index]
+
         else:
             inj = injections[event_index]
             event_info = {}
             # TODO: double check this is still used
             if read_inj_index:
                 # Note: this is only true for the inj files I generated with
                 # generate_injections.
@@ -410,14 +388,37 @@
                 )
             # Put together cache file
             event_info["cache_file"] = data_cache_file_path
             event_info["psd_file"] = psd_file_str[:-1] + "]"
             event_info["channel_name"] = channel_str[:-1] + "]"
             event_info["coinc_xml_file"] = coinc_xml_filename
 
+            is_mdc = 'INJ' in event_info["channel_name"]
+            if is_mdc:
+                mdc_event_injection_file = config.event.mdc_event_injection_file
+                mdc_time_offset = int(config.event.mdc_time_offset)
+                mdc_xml_doc = ligolw_utils.load_filename(
+                        mdc_event_injection_file,
+                        contenthandler=ligolw.LIGOLWContentHandler,
+                        )
+                mdc_sim_inspiral_tbl = lsctables.SimInspiralTable.get_table(mdc_xml_doc)
+                list_of_keys = ["gpstime","mass1","mass2","spin1z","spin2z","distance","latitude","longitude"]
+                mdc_data_dict = {k: [] for k in list_of_keys}
+                for row in mdc_sim_inspiral_tbl:
+                    for key in list_of_keys:
+                        if key== 'gpstime':
+                           mdc_data_dict[key].append(row.geocent_end_time + 1e-9 * row.geocent_end_time_ns)
+                        else:
+                            mdc_data_dict[key].append(getattr(row,key))
+                time_diff_from_injections = np.absolute(np.array(mdc_data_dict['gpstime'])-float(event_info['event_time'])+mdc_time_offset)
+                nearest_inj_index = np.argmin(time_diff_from_injections)
+                mdc_injection_info = {k:0 for k in list_of_keys}
+                for k in list_of_keys:
+                    mdc_injection_info[k] = mdc_data_dict[k][nearest_inj_index]
+
         from . import create_submit_dag_one_event
         if config.submit_only_at_exact_signal_position:
             # Only submit one integrate job at the exact signal position
             event_info_list_strings_reformatted = {
                 key : correct_list_string_formatting_if_list_string(val)
                 for key, val in event_info.items()
             }
```

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -556,14 +556,17 @@
 
 
 _pastro_group_spec = {
     "enabled" : {
         "category_rates": {
             "parser": parse_dict,
         },
+        "category_rates_inj": {
+            "parser": parse_dict,
+        },
         "prior_boundary": {
             "parser": parse_dict,
         },
         "rankstat_pdf_file": {
             "parser": parse_str,
         },
         "far_threshold": {
```

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         os.system("mkdir -p "+output_dir)
     elif not config.overwrite_existing_event_dag:
         sys.exit("ERROR: event directory already exists")
     log_dir = os.path.join(output_dir,"logs","")
     if not os.path.isdir(log_dir):
         os.mkdir(log_dir)
         os.mkdir(os.path.join(output_dir,"results"))
-        os.mkdir(os.path.join(output_dir,"summary_plots"))
+        os.mkdir(os.path.join(output_dir,"summary"))
     if config.web_dir:
         summarypage_dir = config.web_dir
     else:
         summarypage_dir = os.path.join(os.getenv("HOME"),"public_html/RapidPE/"+output_dir[output_dir.rfind("output/")+7:])
     os.makedirs(summarypage_dir, exist_ok=True)
     os.system("cp "+cfgname+" "+os.path.join(output_dir,"Config.ini"))
     os.system('echo "\n#Original config name: '+cfgname+'" >> '+os.path.join(output_dir,'Config.ini'))
@@ -340,19 +340,18 @@
             iter_pt_filename = passthrough_filename.replace("%ITER%",str(int(indx)))
             #If it's the last command, it should launch the plotting script
             #FIXME: should this be optional?
             iter_pt_str = passthrough_str.replace("%ITER%",str(int(indx)))
             web_dir_str = ""
             if config.web_dir:
                 web_dir_str = f"--web-dir {config.web_dir}"
-            summary_plots_outfile = os.path.join(output_dir,"summary_plots/summary_plots.out")
+            summary_plots_outfile = os.path.join(output_dir,"summary/summary_plots.out")
             if indx == (config.n_iterations_per_job-1):
                 iter_pt_str = f"#!/bin/bash\necho {str(int(indx))} `date +%s` >> {output_dir}/job_timing.txt\n"
                 iter_pt_str += f"echo 'job_complete' >> {output_dir}/JOB_COMPLETE\n"
-                #iter_pt_str += "ligolw_no_ilwdchar "+output_dir+"/results/* &>> "+output_dir+"/summary_plots/summary_plots.out\n"
                 iter_pt_str += f"convert_result_to_txt.py {output_dir} --ratio-to-include 0.95  &>> {summary_plots_outfile}\n"
                 iter_pt_str += f"plot_skymap.py {output_dir} --ratio-to-include 0.95  &>> {summary_plots_outfile}\n"
                 iter_pt_str += f"compute_posterior.py {output_dir} --distance-coordinates {config.distance_coordinates } &>> {summary_plots_outfile}\n"
                 if config.cProfile:
                     iter_pt_str += f"cprofile_summary.py {output_dir} &>> {summary_plots_outfile}\n"
                 iter_pt_str += f"create_summarypage.py {output_dir} {web_dir_str}  &>> {summary_plots_outfile}\n"
                 #automatically plot the posteriors when the job is done. FIXME: change 0.99 to whatever
```

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/pastro.py` & `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/pastro.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe-rift-pipe
-Version: 0.1.1.dev20230421
+Version: 0.2.0
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.1.1.dev20230421/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.2.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

