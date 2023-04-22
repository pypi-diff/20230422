# Comparing `tmp/wgdi-0.6.3.tar.gz` & `tmp/wgdi-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wgdi-0.6.3.tar", last modified: Fri Mar 31 14:26:41 2023, max compression
+gzip compressed data, was "dist\wgdi-0.6.4.tar", last modified: Sat Apr 22 12:00:48 2023, max compression
```

## Comparing `wgdi-0.6.3.tar` & `wgdi-0.6.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 14:26:41.356452 wgdi-0.6.3/
--rw-rw-rw-   0        0        0     5370 2023-03-31 14:26:41.356452 wgdi-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     4014 2023-03-31 14:26:01.000000 wgdi-0.6.3/README.md
--rw-rw-rw-   0        0        0       42 2023-03-31 14:26:41.357452 wgdi-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1081 2023-03-31 14:24:14.000000 wgdi-0.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:26:41.310452 wgdi-0.6.3/wgdi/
--rw-rw-rw-   0        0        0        0 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/__init__.py
--rw-rw-rw-   0        0        0     8113 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/align_dotplot.py
--rw-rw-rw-   0        0        0     2646 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/ancestral_karyotype.py
--rw-rw-rw-   0        0        0     3385 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/ancestral_karyotype_repertoire.py
--rw-rw-rw-   0        0        0     8290 2022-12-07 13:55:37.000000 wgdi-0.6.3/wgdi/base.py
--rw-rw-rw-   0        0        0     3889 2022-11-21 05:06:20.000000 wgdi-0.6.3/wgdi/block_correspondence.py
--rw-rw-rw-   0        0        0     7791 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/block_info.py
--rw-rw-rw-   0        0        0     5023 2022-12-07 13:57:34.000000 wgdi-0.6.3/wgdi/block_ks.py
--rw-rw-rw-   0        0        0    11229 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/circos.py
--rw-rw-rw-   0        0        0     6798 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/collinearity.py
--rw-rw-rw-   0        0        0     6225 2022-12-07 14:12:47.000000 wgdi-0.6.3/wgdi/dotplot.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:26:41.354452 wgdi-0.6.3/wgdi/example/
--rw-rw-rw-   0        0        0        0 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/__init__.py
--rw-rw-rw-   0        0        0      398 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/align.conf
--rw-rw-rw-   0        0        0      540 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/alignmenttrees.conf
--rw-rw-rw-   0        0        0      341 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/ancestral_karyotype.conf
--rw-rw-rw-   0        0        0      473 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/ancestral_karyotype_repertoire.conf
--rw-rw-rw-   0        0        0      281 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/blockinfo.conf
--rw-rw-rw-   0        0        0      315 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/blockks.conf
--rw-rw-rw-   0        0        0      443 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/circos.conf
--rw-rw-rw-   0        0        0      302 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/collinearity.conf
--rw-rw-rw-   0        0        0      368 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/conf.ini
--rw-rw-rw-   0        0        0      237 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/corr.conf
--rw-rw-rw-   0        0        0      423 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/dotplot.conf
--rw-rw-rw-   0        0        0      120 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/karyotype.conf
--rw-rw-rw-   0        0        0      434 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/karyotype_mapping.conf
--rw-rw-rw-   0        0        0      183 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/ks.conf
--rw-rw-rw-   0        0        0      383 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/ks_fit_result.csv
--rw-rw-rw-   0        0        0      250 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/ksfigure.conf
--rw-rw-rw-   0        0        0      260 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/kspeaks.conf
--rw-rw-rw-   0        0        0      200 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/peaksfit.conf
--rw-rw-rw-   0        0        0      178 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/pindex.conf
--rw-rw-rw-   0        0        0      182 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/polyploidy_classification.conf
--rw-rw-rw-   0        0        0      235 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/example/retain.conf
--rw-rw-rw-   0        0        0      332 2023-03-31 14:17:47.000000 wgdi-0.6.3/wgdi/example/shared_fusion.conf
--rw-rw-rw-   0        0        0     1637 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/karyotype.py
--rw-rw-rw-   0        0        0     8509 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/karyotype_mapping.py
--rw-rw-rw-   0        0        0     6258 2023-03-31 14:23:24.000000 wgdi-0.6.3/wgdi/ks.py
--rw-rw-rw-   0        0        0     3992 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/ks_peaks.py
--rw-rw-rw-   0        0        0     3459 2022-12-07 13:59:23.000000 wgdi-0.6.3/wgdi/ksfigure.py
--rw-rw-rw-   0        0        0     3535 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/peaksfit.py
--rw-rw-rw-   0        0        0     5328 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/pindex.py
--rw-rw-rw-   0        0        0     2765 2022-12-07 14:03:46.000000 wgdi-0.6.3/wgdi/polyploidy_classification.py
--rw-rw-rw-   0        0        0     3541 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/retain.py
--rw-rw-rw-   0        0        0     7700 2023-03-31 14:24:43.000000 wgdi-0.6.3/wgdi/run.py
--rw-rw-rw-   0        0        0     5929 2022-09-16 11:35:58.000000 wgdi-0.6.3/wgdi/run_colliearity.py
--rw-rw-rw-   0        0        0     3799 2023-03-14 08:55:40.000000 wgdi-0.6.3/wgdi/shared_fusion.py
--rw-rw-rw-   0        0        0     7886 2022-10-20 11:27:44.000000 wgdi-0.6.3/wgdi/trees.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:26:41.321452 wgdi-0.6.3/wgdi.egg-info/
--rw-rw-rw-   0        0        0     5370 2023-03-31 14:26:40.000000 wgdi-0.6.3/wgdi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1361 2023-03-31 14:26:41.000000 wgdi-0.6.3/wgdi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 14:26:40.000000 wgdi-0.6.3/wgdi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-03-31 14:26:40.000000 wgdi-0.6.3/wgdi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-03-31 14:26:40.000000 wgdi-0.6.3/wgdi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-31 14:26:40.000000 wgdi-0.6.3/wgdi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-03-31 14:26:40.000000 wgdi-0.6.3/wgdi.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-22 12:00:48.321730 wgdi-0.6.4/
+-rw-rw-rw-   0        0        0     5499 2023-04-22 12:00:48.321203 wgdi-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4119 2023-04-22 11:59:58.000000 wgdi-0.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-22 12:00:48.321730 wgdi-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-04-22 11:59:58.000000 wgdi-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 12:00:48.255522 wgdi-0.6.4/wgdi/
+-rw-rw-rw-   0        0        0        0 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/__init__.py
+-rw-rw-rw-   0        0        0     8121 2023-04-22 11:59:58.000000 wgdi-0.6.4/wgdi/align_dotplot.py
+-rw-rw-rw-   0        0        0     2646 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/ancestral_karyotype.py
+-rw-rw-rw-   0        0        0     3385 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/ancestral_karyotype_repertoire.py
+-rw-rw-rw-   0        0        0     8288 2023-04-22 11:59:58.000000 wgdi-0.6.4/wgdi/base.py
+-rw-rw-rw-   0        0        0     3889 2022-11-21 05:06:20.000000 wgdi-0.6.4/wgdi/block_correspondence.py
+-rw-rw-rw-   0        0        0     7791 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/block_info.py
+-rw-rw-rw-   0        0        0     5023 2022-12-07 13:57:34.000000 wgdi-0.6.4/wgdi/block_ks.py
+-rw-rw-rw-   0        0        0    11229 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/circos.py
+-rw-rw-rw-   0        0        0     6798 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/collinearity.py
+-rw-rw-rw-   0        0        0     6225 2022-12-07 14:12:47.000000 wgdi-0.6.4/wgdi/dotplot.py
+drwxrwxrwx   0        0        0        0 2023-04-22 12:00:48.319103 wgdi-0.6.4/wgdi/example/
+-rw-rw-rw-   0        0        0        0 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/__init__.py
+-rw-rw-rw-   0        0        0      398 2023-04-04 06:33:01.000000 wgdi-0.6.4/wgdi/example/align.conf
+-rw-rw-rw-   0        0        0      540 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/alignmenttrees.conf
+-rw-rw-rw-   0        0        0      341 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/ancestral_karyotype.conf
+-rw-rw-rw-   0        0        0      473 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/ancestral_karyotype_repertoire.conf
+-rw-rw-rw-   0        0        0      281 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/blockinfo.conf
+-rw-rw-rw-   0        0        0      315 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/blockks.conf
+-rw-rw-rw-   0        0        0      443 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/circos.conf
+-rw-rw-rw-   0        0        0      302 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/collinearity.conf
+-rw-rw-rw-   0        0        0      368 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/conf.ini
+-rw-rw-rw-   0        0        0      237 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/corr.conf
+-rw-rw-rw-   0        0        0      423 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/dotplot.conf
+-rw-rw-rw-   0        0        0      120 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/karyotype.conf
+-rw-rw-rw-   0        0        0      434 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/karyotype_mapping.conf
+-rw-rw-rw-   0        0        0      183 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/ks.conf
+-rw-rw-rw-   0        0        0      383 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/ks_fit_result.csv
+-rw-rw-rw-   0        0        0      250 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/ksfigure.conf
+-rw-rw-rw-   0        0        0      260 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/kspeaks.conf
+-rw-rw-rw-   0        0        0      200 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/peaksfit.conf
+-rw-rw-rw-   0        0        0      178 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/pindex.conf
+-rw-rw-rw-   0        0        0      182 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/polyploidy_classification.conf
+-rw-rw-rw-   0        0        0      235 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/example/retain.conf
+-rw-rw-rw-   0        0        0      332 2023-03-31 14:17:47.000000 wgdi-0.6.4/wgdi/example/shared_fusion.conf
+-rw-rw-rw-   0        0        0     1637 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/karyotype.py
+-rw-rw-rw-   0        0        0     8505 2023-04-22 11:59:58.000000 wgdi-0.6.4/wgdi/karyotype_mapping.py
+-rw-rw-rw-   0        0        0     6258 2023-03-31 14:23:24.000000 wgdi-0.6.4/wgdi/ks.py
+-rw-rw-rw-   0        0        0     3992 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/ks_peaks.py
+-rw-rw-rw-   0        0        0     3459 2022-12-07 13:59:23.000000 wgdi-0.6.4/wgdi/ksfigure.py
+-rw-rw-rw-   0        0        0     3535 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/peaksfit.py
+-rw-rw-rw-   0        0        0     5326 2023-04-22 11:59:58.000000 wgdi-0.6.4/wgdi/pindex.py
+-rw-rw-rw-   0        0        0     2765 2022-12-07 14:03:46.000000 wgdi-0.6.4/wgdi/polyploidy_classification.py
+-rw-rw-rw-   0        0        0     3548 2023-04-22 11:59:58.000000 wgdi-0.6.4/wgdi/retain.py
+-rw-rw-rw-   0        0        0     7700 2023-04-22 11:59:58.000000 wgdi-0.6.4/wgdi/run.py
+-rw-rw-rw-   0        0        0     5929 2022-09-16 11:35:58.000000 wgdi-0.6.4/wgdi/run_colliearity.py
+-rw-rw-rw-   0        0        0     3799 2023-03-14 08:55:40.000000 wgdi-0.6.4/wgdi/shared_fusion.py
+-rw-rw-rw-   0        0        0     7886 2022-10-20 11:27:44.000000 wgdi-0.6.4/wgdi/trees.py
+drwxrwxrwx   0        0        0        0 2023-04-22 12:00:48.270232 wgdi-0.6.4/wgdi.egg-info/
+-rw-rw-rw-   0        0        0     5499 2023-04-22 12:00:47.000000 wgdi-0.6.4/wgdi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1361 2023-04-22 12:00:47.000000 wgdi-0.6.4/wgdi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 12:00:47.000000 wgdi-0.6.4/wgdi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-22 12:00:47.000000 wgdi-0.6.4/wgdi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-04-22 12:00:47.000000 wgdi-0.6.4/wgdi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-22 12:00:47.000000 wgdi-0.6.4/wgdi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-22 12:00:47.000000 wgdi-0.6.4/wgdi.egg-info/zip-safe
```

### Comparing `wgdi-0.6.3/PKG-INFO` & `wgdi-0.6.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wgdi
-Version: 0.6.3
+Version: 0.6.4
 Summary: Whole Genome Duplication Identification
 Home-page: https://github.com/SunPengChuan/wgdi
 Author: Pengchuan Sun
 Author-email: sunpengchuan@gmail.com
 License: BSD License
 Description: # WGDI
         
@@ -54,14 +54,17 @@
         
         If you use wgdi in your work, please cite:
         
         > Sun P., Jiao B., Yang Y., Shan L., Li T., Li X., Xi Z., Wang X., and Liu J. (2022). WGDI: A user-friendly toolkit for evolutionary analyses of whole-genome duplications and ancestral karyotypes. Mol. Plant. doi: https://doi.org/10.1016/j.molp.2022.10.018.
         
         ## News
         
+        ## 0.6.4
+        * Fixed the problem caused by the Python version, now it is compatible with version 3.11.3.
+        
         ## 0.6.3
         * Fixed some issues (-ks, -sf).
         
         ## 0.6.2
         * Added find shared fusions between species (-sf).
         
         ## 0.6.1
```

### Comparing `wgdi-0.6.3/README.md` & `wgdi-0.6.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 
 If you use wgdi in your work, please cite:
 
 > Sun P., Jiao B., Yang Y., Shan L., Li T., Li X., Xi Z., Wang X., and Liu J. (2022). WGDI: A user-friendly toolkit for evolutionary analyses of whole-genome duplications and ancestral karyotypes. Mol. Plant. doi: https://doi.org/10.1016/j.molp.2022.10.018.
 
 ## News
 
+## 0.6.4
+* Fixed the problem caused by the Python version, now it is compatible with version 3.11.3.
+
 ## 0.6.3
 * Fixed some issues (-ks, -sf).
 
 ## 0.6.2
 * Added find shared fusions between species (-sf).
 
 ## 0.6.1
```

### Comparing `wgdi-0.6.3/setup.py` & `wgdi-0.6.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 required = ['pandas>=1.1.0', 'numpy', 'biopython', 'matplotlib', 'scipy']
 
 setup(
     name="wgdi",
-    version="0.6.3",
+    version="0.6.4",
     author="Pengchuan Sun",
     author_email="sunpengchuan@gmail.com",
     description="Whole Genome Duplication Identification",
     license="BSD License",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SunPengChuan/wgdi",
```

### Comparing `wgdi-0.6.3/wgdi/align_dotplot.py` & `wgdi-0.6.4/wgdi/align_dotplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 
     def pair_positon(self, alignment, loc1, loc2, colors):
         alignment.index = alignment.index.map(loc1)
         data, i = [], 0
         for k in alignment.columns:
             df = alignment[k].map(loc2)
             df.dropna(axis=0, how='any', inplace=True)
-            for index, row in df.iteritems():
+            
+            for index, row in df.items():
                 data.append([index, row, colors[i]])
             i += 1
         df = pd.DataFrame(data, columns=['loc1', 'loc2', 'color'])
         return df
 
     def run(self):
         axis = [0, 1, 1, 0]
@@ -116,15 +117,15 @@
         sys.exit(0)
 
     def alignment(self, gff1, gff2, bkinfo):
         gff1['uid']= gff1['chr']+'g'+gff1['order'].astype(str)
         gff2['uid']= gff2['chr']+'g'+gff2['order'].astype(str)
         gff1['id'] = gff1.index
         gff2['id'] = gff2.index
-        for cl, group in bkinfo.groupby([self.classid]):
+        for cl, group in bkinfo.groupby(self.classid):
             name = 'l'+cl
             gff1[name] = np.nan
             group = group.sort_values(by=['length'], ascending=[False])
             for index, row in group.iterrows():
                 b1 = row['block1'].split('_')
                 b2 = row['block2'].split('_')
                 ks = row['ks'].split('_')
```

### Comparing `wgdi-0.6.3/wgdi/ancestral_karyotype.py` & `wgdi-0.6.4/wgdi/ancestral_karyotype.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/ancestral_karyotype_repertoire.py` & `wgdi-0.6.4/wgdi/ancestral_karyotype_repertoire.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/base.py` & `wgdi-0.6.4/wgdi/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
     gff = gff[gff['chr'].isin(lens.index)].copy()
     if len(gff)==0:
         print('Stoped! \n\nChromosomes in gff file and lens file do not correspond.')
         exit(0)
     dict_chr = dict(zip(lens.index, np.append(
         np.array([0]), lens.cumsum()[:-1].values)))
     gff.loc[:, 'loc'] = ''
-    for name, group in gff.groupby(['chr']):
+    for name, group in gff.groupby('chr'):
         gff.loc[group.index, 'loc'] = (dict_chr[name]+group[position])*step
     return gff
 
 
 def dotplot_frame(fig, ax, lens1, lens2, step1, step2, genome1_name, genome2_name, arr):
     for k in lens1.cumsum()[:-1]*step1:
         ax.axhline(y=k, alpha=0.8, color='black', lw=0.5)
```

### Comparing `wgdi-0.6.3/wgdi/block_correspondence.py` & `wgdi-0.6.4/wgdi/block_correspondence.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/block_info.py` & `wgdi-0.6.4/wgdi/block_info.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/block_ks.py` & `wgdi-0.6.4/wgdi/block_ks.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/circos.py` & `wgdi-0.6.4/wgdi/circos.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/collinearity.py` & `wgdi-0.6.4/wgdi/collinearity.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/dotplot.py` & `wgdi-0.6.4/wgdi/dotplot.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/example/alignmenttrees.conf` & `wgdi-0.6.4/wgdi/example/alignmenttrees.conf`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/karyotype.py` & `wgdi-0.6.4/wgdi/karyotype.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/karyotype_mapping.py` & `wgdi-0.6.4/wgdi/karyotype_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         gff1.loc[data.index, 'classification'] = data['classification']
         return gff1
 
     def karyotype_map(self, gff, lens):
         gff = gff[gff['chr'].isin(lens.index)]
         gff = gff[gff['color'].notnull()]
         ancestor = []
-        for chr, group in gff.groupby(['chr']):
+        for chr, group in gff.groupby('chr'):
             color, classid, arr = '', 1, []
             for index, row in group.iterrows():
                 if color == row['color'] and classid == row['classification']:
                     arr.append(row['order'])
                 else:
                     if len(arr) >= int(self.limit_length):
                         ancestor.append(
@@ -73,15 +73,15 @@
                             ancestor[-1][1], ancestor[-1][2], size=ancestor[-1][5]-1).tolist()
                         ancestor.pop()
                     arr.append(row['order'])
             if len(arr) >= int(self.limit_length):
                 ancestor.append(
                     [chr, min(arr), max(arr), color, classid, len(arr)])
         ancestor = pd.DataFrame(ancestor)
-        for chr, group in ancestor.groupby([0]):
+        for chr, group in ancestor.groupby(0):
             ancestor.loc[group.index[0], 1] = 1
             ancestor.loc[group.index[-1], 2] = lens[chr]
         ancestor[4] = ancestor[4].astype(int)
         return ancestor[[0, 1, 2, 3, 4]]
 
     def colinear_gene_pairs(self, bkinfo, gff1, gff2):
         data = []
```

### Comparing `wgdi-0.6.3/wgdi/ks.py` & `wgdi-0.6.4/wgdi/ks.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/ks_peaks.py` & `wgdi-0.6.4/wgdi/ks_peaks.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/ksfigure.py` & `wgdi-0.6.4/wgdi/ksfigure.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/peaksfit.py` & `wgdi-0.6.4/wgdi/peaksfit.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/pindex.py` & `wgdi-0.6.4/wgdi/pindex.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
     def cal_pindex(self, alignment):
         data, df = [], []
         columns = alignment.columns[:-2].tolist()
         for i in range(len(columns)-1):
             for j in range(i+1, len(columns)):
                 b = []
-                for chr, group in alignment.groupby(['chr']):
+                for chr, group in alignment.groupby('chr'):
                     sub1 = group.loc[:, columns[i]].tolist()
                     sub2 = group.loc[:, columns[j]].tolist()
                     p = self.Pindex(sub1, sub2)
                     b.append(p)
                     df.append([i, j, chr]+p)
                 sub_diver = sum([abs(k[0]+k[1]) for k in b])
                 if self.remove_delta in ['true', 'TRUE', '1']:
```

### Comparing `wgdi-0.6.3/wgdi/polyploidy_classification.py` & `wgdi-0.6.4/wgdi/polyploidy_classification.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/retain.py` & `wgdi-0.6.4/wgdi/retain.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,17 @@
         align = dict(family='Arial', verticalalignment="center",
                      horizontalalignment="center")
         plt.ylabel(self.ylabel+'\n\n\n\n', fontsize=18, **align)
         for spine in plt.gca().spines.values():
             spine.set_visible(False)
         plt.tick_params(top=False, bottom=False, left=False,
                         right=False, labelleft=False, labelbottom=False)
-        groups = self.retain.groupby(['chr'])
+        groups = self.retain.groupby('chr')
         for i in range(len(lens)):
-            group = groups.get_group(lens.index[i])
+            group = groups.get_group(lens.index.tolist()[i])
             for j in self.retain.columns[:-2]:
                 axs[i].plot(group['order'].values, group[j].values,
                             linestyle='-', color=self.colors[j-1], linewidth=1)
             axs[i].spines['right'].set_visible(False)
             axs[i].spines['top'].set_visible(False)
             axs[i].set_ylim(self.ylim)
             axs[i].tick_params(labelsize=12)
```

### Comparing `wgdi-0.6.3/wgdi/run.py` & `wgdi-0.6.4/wgdi/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 parser = argparse.ArgumentParser(
     prog='wgdi', usage='%(prog)s [options]', epilog="", formatter_class=argparse.RawDescriptionHelpFormatter,)
 parser.description = '''\
 WGDI(Whole-Genome Duplication Integrated analysis):  A user-friendly toolkit for evolutionary analyses of whole-genome duplications and ancestral karyotypes.
 
     https://wgdi.readthedocs.io/en/latest/
     -------------------------------------- '''
-parser.add_argument("-v", "--version", action='version', version='0.6.3')
+parser.add_argument("-v", "--version", action='version', version='0.6.4')
 parser.add_argument("-d", dest="dotplot",
                     help="Show homologous gene dotplot")
 parser.add_argument("-icl", dest="improvedcollinearity",
                     help="Improved version of ColinearScan ")
 parser.add_argument("-ks", dest="calks",
                     help="Calculate Ka/Ks for homologous gene pairs by YN00")
 parser.add_argument("-bk", dest="blockks",
```

### Comparing `wgdi-0.6.3/wgdi/run_colliearity.py` & `wgdi-0.6.4/wgdi/run_colliearity.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/shared_fusion.py` & `wgdi-0.6.4/wgdi/shared_fusion.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi/trees.py` & `wgdi-0.6.4/wgdi/trees.py`

 * *Files identical despite different names*

### Comparing `wgdi-0.6.3/wgdi.egg-info/PKG-INFO` & `wgdi-0.6.4/wgdi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wgdi
-Version: 0.6.3
+Version: 0.6.4
 Summary: Whole Genome Duplication Identification
 Home-page: https://github.com/SunPengChuan/wgdi
 Author: Pengchuan Sun
 Author-email: sunpengchuan@gmail.com
 License: BSD License
 Description: # WGDI
         
@@ -54,14 +54,17 @@
         
         If you use wgdi in your work, please cite:
         
         > Sun P., Jiao B., Yang Y., Shan L., Li T., Li X., Xi Z., Wang X., and Liu J. (2022). WGDI: A user-friendly toolkit for evolutionary analyses of whole-genome duplications and ancestral karyotypes. Mol. Plant. doi: https://doi.org/10.1016/j.molp.2022.10.018.
         
         ## News
         
+        ## 0.6.4
+        * Fixed the problem caused by the Python version, now it is compatible with version 3.11.3.
+        
         ## 0.6.3
         * Fixed some issues (-ks, -sf).
         
         ## 0.6.2
         * Added find shared fusions between species (-sf).
         
         ## 0.6.1
```

### Comparing `wgdi-0.6.3/wgdi.egg-info/SOURCES.txt` & `wgdi-0.6.4/wgdi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

