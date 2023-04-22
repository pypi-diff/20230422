# Comparing `tmp/dcm-processor-1.0.2.tar.gz` & `tmp/dcm-processor-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcm-processor-1.0.2.tar", last modified: Mon Apr 17 10:46:55 2023, max compression
+gzip compressed data, was "dcm-processor-1.0.3.tar", last modified: Sat Apr 22 10:53:25 2023, max compression
```

## Comparing `dcm-processor-1.0.2.tar` & `dcm-processor-1.0.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:55.093347 dcm-processor-1.0.2/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1074 2021-05-11 10:55:48.000000 dcm-processor-1.0.2/LICENSE
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-04-17 10:46:55.093894 dcm-processor-1.0.2/PKG-INFO
--rwxr-xr-x   0 giles     (1000) giles     (1000)     5834 2023-04-17 10:06:58.000000 dcm-processor-1.0.2/README.md
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:54.828586 dcm-processor-1.0.2/dcm_processor/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       61 2021-10-17 14:30:50.000000 dcm-processor-1.0.2/dcm_processor/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    15407 2023-04-15 09:02:58.000000 dcm-processor-1.0.2/dcm_processor/argparser.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    33004 2023-04-14 11:38:11.000000 dcm-processor-1.0.2/dcm_processor/files.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    45679 2023-04-17 10:31:24.000000 dcm-processor-1.0.2/dcm_processor/script.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:54.778662 dcm-processor-1.0.2/dcm_processor/services/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:54.776954 dcm-processor-1.0.2/dcm_processor/services/base/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:54.875309 dcm-processor-1.0.2/dcm_processor/services/base/module/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:54.994779 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/
--rwxr-xr-x   0 giles     (1000) giles     (1000)   642195 2021-10-17 16:16:14.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)    17869 2021-10-17 16:16:15.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)      526 2023-04-06 14:13:53.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1551 2023-03-31 12:36:10.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    69564 2021-10-17 16:16:15.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:55.015758 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/config/
--rwxr-xr-x   0 giles     (1000) giles     (1000)    59497 2021-10-17 16:16:15.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script
--rwxr-xr-x   0 giles     (1000) giles     (1000)      248 2021-10-17 16:16:15.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/config/hash_table.csv
--rwxr-xr-x   0 giles     (1000) giles     (1000)       86 2021-10-17 16:16:15.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/config/psudonyms.csv
--rwxr-xr-x   0 giles     (1000) giles     (1000)    10424 2021-10-17 16:16:15.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   863881 2021-10-17 16:16:16.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)     3471 2023-03-31 12:35:15.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)  1172845 2021-10-17 16:16:18.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   391834 2021-10-17 16:16:19.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)    28241 2021-10-17 16:16:19.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   338969 2021-10-17 16:16:20.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/util.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1777 2023-03-31 20:09:03.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/utils.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)       26 2021-10-17 16:16:20.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/requirements.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       72 2021-10-17 16:16:20.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/script.sh
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:55.028789 dcm-processor-1.0.2/dcm_processor/services/base/module/storageManager/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/storageManager/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)       97 2021-10-17 16:16:20.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/storageManager/header_codes.json
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6218 2023-01-31 18:15:24.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/storageManager/lib.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    10012 2023-01-31 18:15:43.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/storageManager/main.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:55.036364 dcm-processor-1.0.2/dcm_processor/services/base/module/systemcleaner/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/systemcleaner/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     3806 2023-04-01 16:24:05.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/systemcleaner/main.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:55.040232 dcm-processor-1.0.2/dcm_processor/services/base/registry/
--rwxr-xr-x   0 giles     (1000) giles     (1000)      443 2021-10-17 16:16:20.000000 dcm-processor-1.0.2/dcm_processor/services/base/registry/__init__.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:54.793572 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:55.080412 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/module/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     4030 2023-04-14 14:47:11.000000 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/module/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)  1948128 2023-03-02 19:03:11.000000 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/module/dcm2niix
--rwxr-xr-x   0 giles     (1000) giles     (1000)      406 2023-03-24 20:50:04.000000 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/module/lib.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:55.090362 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/registry/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1013 2023-04-14 12:17:35.000000 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/registry/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)      285 2023-04-01 13:10:09.000000 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/registry/settings.json
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6601 2023-02-01 11:09:28.000000 dcm-processor-1.0.2/dcm_processor/worker.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:54.860542 dcm-processor-1.0.2/dcm_processor.egg-info/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-04-17 10:46:53.000000 dcm-processor-1.0.2/dcm_processor.egg-info/PKG-INFO
--rwxr-xr-x   0 giles     (1000) giles     (1000)     2368 2023-04-17 10:46:54.000000 dcm-processor-1.0.2/dcm_processor.egg-info/SOURCES.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)        1 2023-04-17 10:46:53.000000 dcm-processor-1.0.2/dcm_processor.egg-info/dependency_links.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       53 2023-04-17 10:46:53.000000 dcm-processor-1.0.2/dcm_processor.egg-info/entry_points.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       76 2023-04-17 10:46:53.000000 dcm-processor-1.0.2/dcm_processor.egg-info/requires.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       14 2023-04-17 10:46:53.000000 dcm-processor-1.0.2/dcm_processor.egg-info/top_level.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       89 2021-10-17 14:23:09.000000 dcm-processor-1.0.2/pyproject.toml
--rwxr-xr-x   0 giles     (1000) giles     (1000)      980 2023-04-17 10:46:55.098413 dcm-processor-1.0.2/setup.cfg
--rwxr-xr-x   0 giles     (1000) giles     (1000)      109 2021-10-17 19:37:23.000000 dcm-processor-1.0.2/setup.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.394013 dcm-processor-1.0.3/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1074 2021-05-11 10:55:48.000000 dcm-processor-1.0.3/LICENSE
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-04-22 10:53:25.394322 dcm-processor-1.0.3/PKG-INFO
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     5834 2023-04-17 10:06:58.000000 dcm-processor-1.0.3/README.md
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.132198 dcm-processor-1.0.3/dcm_processor/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       61 2021-10-17 14:30:50.000000 dcm-processor-1.0.3/dcm_processor/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    15407 2023-04-15 09:02:58.000000 dcm-processor-1.0.3/dcm_processor/argparser.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    33044 2023-04-22 10:03:38.000000 dcm-processor-1.0.3/dcm_processor/files.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    46033 2023-04-19 12:36:49.000000 dcm-processor-1.0.3/dcm_processor/script.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.085824 dcm-processor-1.0.3/dcm_processor/services/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.085127 dcm-processor-1.0.3/dcm_processor/services/base/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.165520 dcm-processor-1.0.3/dcm_processor/services/base/module/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.289840 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   642195 2021-10-17 16:16:14.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    17869 2021-10-17 16:16:15.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      526 2023-04-06 14:13:53.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1551 2023-03-31 12:36:10.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    69564 2021-10-17 16:16:15.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.309642 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/config/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    59497 2021-10-17 16:16:15.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      248 2021-10-17 16:16:15.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/config/hash_table.csv
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       86 2021-10-17 16:16:15.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/config/psudonyms.csv
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    10424 2021-10-17 16:16:15.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   863881 2021-10-17 16:16:16.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     3471 2023-03-31 12:35:15.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)  1172845 2021-10-17 16:16:18.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   391834 2021-10-17 16:16:19.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    28241 2021-10-17 16:16:19.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   338969 2021-10-17 16:16:20.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/util.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1777 2023-03-31 20:09:03.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/utils.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       26 2021-10-17 16:16:20.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/requirements.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       72 2021-10-17 16:16:20.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/script.sh
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.326522 dcm-processor-1.0.3/dcm_processor/services/base/module/storageManager/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/storageManager/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       97 2021-10-17 16:16:20.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/storageManager/header_codes.json
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6218 2023-01-31 18:15:24.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/storageManager/lib.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    10012 2023-01-31 18:15:43.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/storageManager/main.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.330046 dcm-processor-1.0.3/dcm_processor/services/base/module/systemcleaner/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/systemcleaner/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     3806 2023-04-01 16:24:05.000000 dcm-processor-1.0.3/dcm_processor/services/base/module/systemcleaner/main.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.337447 dcm-processor-1.0.3/dcm_processor/services/base/registry/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      443 2021-10-17 16:16:20.000000 dcm-processor-1.0.3/dcm_processor/services/base/registry/__init__.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.087046 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.387526 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/module/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     4030 2023-04-14 14:47:11.000000 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/module/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)  1948128 2023-03-02 19:03:11.000000 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/module/dcm2niix
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      406 2023-03-24 20:50:04.000000 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/module/lib.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.391551 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/registry/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1013 2023-04-14 12:17:35.000000 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/registry/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      288 2023-04-18 12:25:35.000000 dcm-processor-1.0.3/dcm_processor/services/dcm2nii/registry/settings.json
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6682 2023-04-21 16:23:38.000000 dcm-processor-1.0.3/dcm_processor/worker.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-22 10:53:25.157451 dcm-processor-1.0.3/dcm_processor.egg-info/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-04-22 10:53:23.000000 dcm-processor-1.0.3/dcm_processor.egg-info/PKG-INFO
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     2368 2023-04-22 10:53:24.000000 dcm-processor-1.0.3/dcm_processor.egg-info/SOURCES.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)        1 2023-04-22 10:53:23.000000 dcm-processor-1.0.3/dcm_processor.egg-info/dependency_links.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       53 2023-04-22 10:53:23.000000 dcm-processor-1.0.3/dcm_processor.egg-info/entry_points.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       76 2023-04-22 10:53:23.000000 dcm-processor-1.0.3/dcm_processor.egg-info/requires.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       14 2023-04-22 10:53:23.000000 dcm-processor-1.0.3/dcm_processor.egg-info/top_level.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       89 2021-10-17 14:23:09.000000 dcm-processor-1.0.3/pyproject.toml
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      980 2023-04-22 10:53:25.395849 dcm-processor-1.0.3/setup.cfg
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      109 2021-10-17 19:37:23.000000 dcm-processor-1.0.3/setup.py
```

### Comparing `dcm-processor-1.0.2/LICENSE` & `dcm-processor-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/PKG-INFO` & `dcm-processor-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcm-processor
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Command line tool for the dicom processor library
 Home-page: https://github.com/giesekow/dcm-processor-cli
 Author: Giles Tetteh
 Author-email: giles.tetteh@tum.de
 Keywords: orthanc,dicom,worker,processor,translation,medical
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dcm-processor-1.0.2/README.md` & `dcm-processor-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/argparser.py` & `dcm-processor-1.0.3/dcm_processor/argparser.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/files.py` & `dcm-processor-1.0.3/dcm_processor/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 DASHBOARD_AUTH = """
 { "dcm-processor": "dcm-processor" }
 """
 
 SETTINGS = """
 {
-  "headerFields": ["SeriesInstanceUID", "ImagePositionPatient", "ImageOrientationPatient", "PerformedProcedureStepDescription", "seriesId", "dcmpath", "SeriesDescription", "ContrastBolusAgent", "Modality", "ImageType", "PatientID", "SeriesNumber", "StudyDate", "ImageComments"],
+  "fullTags": true,
+  "headerFields": ["SeriesInstanceUID", "ImagePositionPatient", "ImageOrientationPatient", "PerformedProcedureStepDescription", "seriesId", "dcmpath", "SeriesDescription", "ContrastBolusAgent", "Modality", "ImageType", "PatientID", "SeriesNumber", "StudyDate", "ImageComments", "BodyPartExamined"],
   "preServices": [
     {
       "jobName": "dicomAnonymizer",
       "worker": "base.DicomAnonymizerService.worker",
       "callback": "base.dicomAnonymizer",
       "dependsOn": null,
       "channel": "default",
```

### Comparing `dcm-processor-1.0.2/dcm_processor/script.py` & `dcm-processor-1.0.3/dcm_processor/script.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,16 +283,16 @@
     file.write(FILES.DASHBOARD_AUTH)
 
 def create_worker(args):
   if not args.non_interactive:
     questions = [
       inq.Text("worker_name", message="Enter worker name"),
       inq.Path("worker_path", message="Enter workers folder", exists=True, path_type=inq.Path.DIRECTORY, normalize_to_absolute_path=True),
-      inq.Text("worker_base_image", message="Enter worker base image", default="ubuntu:18.04"),
-      inq.Text("worker_python_version", message="Enter worker python version", default="3.7"),
+      inq.Text("worker_base_image", message="Enter worker base image", default="ubuntu:20.04"),
+      inq.Text("worker_python_version", message="Enter worker python version", default="3.9"),
       inq.Text("channels", message="Enter job channels (comma separated)", default="default"),
       inq.Text("worker_description", message="Enter worker description"),
     ]
 
     answers = inq.prompt(questions)
     worker_name = answers['worker_name']
     worker_path = answers['worker_path']
@@ -312,14 +312,15 @@
 
   worker_settings = {
     "name": worker_name,
     "description": worker_description,
     "scripts": ["script.sh"],
     "entryScriptPaths": ["/scripts"],
     "baseImage": base_image,
+    "copies": [],
     "environments": [
       {
         "name": "base",
         "requirements": ["requirements.txt"],
         "entryRequirementPaths": ["/requirements"],
         "channels": [s.strip() for s in str(channels).strip().split(",")],
         "pythonVersion": python_version
@@ -867,16 +868,28 @@
   if "image" in settings:
     img = settings.get("image")
     if not img is None:
       return
 
   base_image = settings.get("baseImage", "ubuntu:18.04")
 
+  dockerfile = WORKER.DOCKERFILE.replace("BASE_IMAGE", base_image)
+
+  if "copies" in settings:
+    copies = settings.get("copies", [])
+    copy_str = ''
+    for c in copies:
+      src = c.get("source")
+      dest = c.get("destination")
+      copy_str = f"{copy_str}COPY {src} {dest}\n"
+  
+    dockerfile = dockerfile.replace("#COPIES", f"# COPY OTHER FILES HERE\n{copy_str}")
+
   initial_files = {
-    "Dockerfile": WORKER.DOCKERFILE.replace("BASE_IMAGE", base_image),
+    "Dockerfile": dockerfile,
     "entrypoint.sh": WORKER.ENTRYPOINT,
     "envs.py": WORKER.ENVS,
     "install.py": WORKER.INSTALL,
     "start.py": WORKER.START
   }
 
   ## Write initial files.
```

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar` & `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar` & `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py` & `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py` & `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar` & `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script` & `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar` & `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar` & `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py` & `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar` & `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar` & `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar` & `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/util.jar` & `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/util.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/utils.py` & `dcm-processor-1.0.3/dcm_processor/services/base/module/DicomAnonymizerService/utils.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/storageManager/lib.py` & `dcm-processor-1.0.3/dcm_processor/services/base/module/storageManager/lib.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/storageManager/main.py` & `dcm-processor-1.0.3/dcm_processor/services/base/module/storageManager/main.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/base/module/systemcleaner/main.py` & `dcm-processor-1.0.3/dcm_processor/services/base/module/systemcleaner/main.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/dcm2nii/module/__init__.py` & `dcm-processor-1.0.3/dcm_processor/services/dcm2nii/module/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/dcm2nii/module/dcm2niix` & `dcm-processor-1.0.3/dcm_processor/services/dcm2nii/module/dcm2niix`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/services/dcm2nii/registry/__init__.py` & `dcm-processor-1.0.3/dcm_processor/services/dcm2nii/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/dcm_processor/worker.py` & `dcm-processor-1.0.3/dcm_processor/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 COPY envs.py ./
 
 RUN mkdir -p /settings
 RUN mkdir -p /environments
 
 COPY ./settings/. /settings/.
 
+#COPIES
+
 # Install all required dependencies
 
 RUN apt-get update && \
     apt-get install -y software-properties-common tzdata git && \
     apt-get update -y && \
     apt-get install -y python3.9 python3-pip python3-venv python3-distutils && \
     ln -s /usr/bin/python3.9 /usr/bin/python && \
@@ -43,14 +45,20 @@
 
 WLOGS="$LOGS/worker.txt"
 
 python start.py
 
 ENVARGS=$(python envs.py)
 
+unset HTTP_PROXY
+unset http_proxy
+
+unset HTTPS_PROXY
+unset https_proxy
+
 python-mqas worker $ENVARGS --modules="$MODULES" --conn="$JOBS_CONNECTION" --dbname="$JOBS_DBNAME" --colname="$JOBS_COLNAME" --log-file="$WLOGS"
 """
 
 ENVS = """
 import json, os, subprocess
 
 DEFAULT_PYTHON_VERSION = "3.9"
```

### Comparing `dcm-processor-1.0.2/dcm_processor.egg-info/PKG-INFO` & `dcm-processor-1.0.3/dcm_processor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcm-processor
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Command line tool for the dicom processor library
 Home-page: https://github.com/giesekow/dcm-processor-cli
 Author: Giles Tetteh
 Author-email: giles.tetteh@tum.de
 Keywords: orthanc,dicom,worker,processor,translation,medical
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dcm-processor-1.0.2/dcm_processor.egg-info/SOURCES.txt` & `dcm-processor-1.0.3/dcm_processor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.2/setup.cfg` & `dcm-processor-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dcm-processor
-version = 1.0.2
+version = 1.0.3
 author = Giles Tetteh
 author_email = giles.tetteh@tum.de
 description = A Command line tool for the dicom processor library
 url = https://github.com/giesekow/dcm-processor-cli
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE
```

