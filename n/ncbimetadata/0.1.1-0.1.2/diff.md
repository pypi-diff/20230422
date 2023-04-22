# Comparing `tmp/ncbimetadata-0.1.1.tar.gz` & `tmp/ncbimetadata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncbimetadata-0.1.1.tar", last modified: Thu Apr 20 15:28:17 2023, max compression
+gzip compressed data, was "ncbimetadata-0.1.2.tar", last modified: Sat Apr 22 07:57:32 2023, max compression
```

## Comparing `ncbimetadata-0.1.1.tar` & `ncbimetadata-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 15:28:17.592576 ncbimetadata-0.1.1/
--rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.1.1/LICENSE
--rw-r--r--   0 taiyuan    (501) staff       (20)     3061 2023-04-20 15:28:17.592374 ncbimetadata-0.1.1/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.1.1/README.md
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 15:28:17.590797 ncbimetadata-0.1.1/ncbimetadata/
--rw-r--r--   0 taiyuan    (501) staff       (20)       81 2023-04-20 11:24:39.000000 ncbimetadata-0.1.1/ncbimetadata/__init__.py
--rw-r--r--   0 taiyuan    (501) staff       (20)    11000 2023-04-20 15:24:04.000000 ncbimetadata-0.1.1/ncbimetadata/core.py
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 15:28:17.592101 ncbimetadata-0.1.1/ncbimetadata.egg-info/
--rw-r--r--   0 taiyuan    (501) staff       (20)     3061 2023-04-20 15:28:17.000000 ncbimetadata-0.1.1/ncbimetadata.egg-info/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)      290 2023-04-20 15:28:17.000000 ncbimetadata-0.1.1/ncbimetadata.egg-info/SOURCES.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 15:28:17.000000 ncbimetadata-0.1.1/ncbimetadata.egg-info/dependency_links.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       51 2023-04-20 15:28:17.000000 ncbimetadata-0.1.1/ncbimetadata.egg-info/entry_points.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-20 15:28:17.000000 ncbimetadata-0.1.1/ncbimetadata.egg-info/requires.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-20 15:28:17.000000 ncbimetadata-0.1.1/ncbimetadata.egg-info/top_level.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-20 15:28:17.592655 ncbimetadata-0.1.1/setup.cfg
--rw-r--r--   0 taiyuan    (501) staff       (20)      807 2023-04-20 15:27:49.000000 ncbimetadata-0.1.1/setup.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-22 07:57:32.503318 ncbimetadata-0.1.2/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.1.2/LICENSE
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3061 2023-04-22 07:57:32.503192 ncbimetadata-0.1.2/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.1.2/README.md
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-22 07:57:32.502014 ncbimetadata-0.1.2/ncbimetadata/
+-rw-r--r--   0 taiyuan    (501) staff       (20)       81 2023-04-20 11:24:39.000000 ncbimetadata-0.1.2/ncbimetadata/__init__.py
+-rw-r--r--   0 taiyuan    (501) staff       (20)    12425 2023-04-22 07:56:02.000000 ncbimetadata-0.1.2/ncbimetadata/core.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-22 07:57:32.503025 ncbimetadata-0.1.2/ncbimetadata.egg-info/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3061 2023-04-22 07:57:32.000000 ncbimetadata-0.1.2/ncbimetadata.egg-info/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)      290 2023-04-22 07:57:32.000000 ncbimetadata-0.1.2/ncbimetadata.egg-info/SOURCES.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-22 07:57:32.000000 ncbimetadata-0.1.2/ncbimetadata.egg-info/dependency_links.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       51 2023-04-22 07:57:32.000000 ncbimetadata-0.1.2/ncbimetadata.egg-info/entry_points.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-22 07:57:32.000000 ncbimetadata-0.1.2/ncbimetadata.egg-info/requires.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-22 07:57:32.000000 ncbimetadata-0.1.2/ncbimetadata.egg-info/top_level.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-22 07:57:32.503362 ncbimetadata-0.1.2/setup.cfg
+-rw-r--r--   0 taiyuan    (501) staff       (20)      807 2023-04-22 07:57:09.000000 ncbimetadata-0.1.2/setup.py
```

### Comparing `ncbimetadata-0.1.1/LICENSE` & `ncbimetadata-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.1.1/PKG-INFO` & `ncbimetadata-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.1.1
+Version: 0.1.2
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
 Home-page: https://github.com/RyanYuanSun/ncbimetadata
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
```

### Comparing `ncbimetadata-0.1.1/README.md` & `ncbimetadata-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.1.1/ncbimetadata/core.py` & `ncbimetadata-0.1.2/ncbimetadata/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,27 @@
     pass
 
 
 def normalize_name(name):
     return name.capitalize().replace('_', ' ')
 
 
-def worker(accession, data, data_failed):
+def worker(accession, data, data_failed, custom_bogus, default_bogus):
     attributes = []
-    bogus_values = ['missing', 'n/a', 'not provided', 'not provided; submitted under MIGS 2.1', '', 'NA', '/', 'N/A',
-                    'missed', 'not located', 'Not Applicable', 'Missing', 'unknown', 'Unknown', 'not collected',
-                    'Not applicable', 'not applicable']
+    if default_bogus == 1:
+        bogus_values = ['missing', 'n/a', 'not provided', 'not provided; submitted under MIGS 2.1', '', 'NA', '/', 'N/A',
+                        'missed', 'not located', 'Not Applicable', 'Missing', 'unknown', 'Unknown', 'not collected',
+                        'Not applicable', 'not applicable']
+    else:
+        bogus_values = []
+    if len(custom_bogus) > 0:
+        for i in custom_bogus:
+            if i not in bogus_values:
+                bogus_values.append(i)
+
     detail_request_url = 'https://api.ncbi.nlm.nih.gov/datasets/v2alpha/genome/accession/' + accession + '/dataset_report?filters.assembly_version=all_assemblies&page_size=1000'
     try:
         result_detail = requests.get(url=detail_request_url)
     except:
         if accession not in data_failed:
             data_failed.append(accession)
             return
@@ -105,17 +113,17 @@
         if accession not in data_failed:
             data_failed.append(accession)
             return
         else:
             return
 
 
-def sub_process(job, data, data_failed):
+def sub_process(job, data, data_failed, custom_bogus, default_bogus):
     for accession in job:
-        subProcess = multiprocessing.Process(target=worker, args=(accession, data, data_failed))
+        subProcess = multiprocessing.Process(target=worker, args=(accession, data, data_failed, custom_bogus, default_bogus))
         subProcess.start()
 
 
 def collect_links(taxon_id, accession_list):
     # request_payload = '{"filters":{"has_annotation":true,"assembly_source":"refseq","exclude_paired_reports":true,"assembly_version":"current"},"page_size":1000,"page_token":null,"returned_content":"COMPLETE","taxons":["' + str(taxon_id) + '"]}'
     request_payload = '{"page_size":1000,"page_token":null,"returned_content":"COMPLETE","taxons":["' + str(taxon_id) + '"]}'
     result_page = requests.post("https://api.ncbi.nlm.nih.gov/datasets/v2alpha/genome/dataset_report", data=request_payload)
@@ -128,17 +136,17 @@
             taxon_id) + '"]}'
         result_page = requests.post("https://api.ncbi.nlm.nih.gov/datasets/v2alpha/genome/dataset_report", data=request_payload)
         for i in result_page.json()['reports']:
             accession_list.append(i['accession'])
     return accession_list
 
 
-def collect_data(job_pool, data, data_failed):
+def collect_data(job_pool, data, data_failed, custom_bogus, default_bogus):
     for i, job in enumerate(job_pool):
-        process = multiprocessing.Process(target=sub_process, args=(job, data, data_failed))
+        process = multiprocessing.Process(target=sub_process, args=(job, data, data_failed, custom_bogus, default_bogus))
         process.start()
         process.join()
 
 
 def watcher(total, list, list_2=[]):
     while True:
         time.sleep(0.2)
@@ -177,24 +185,45 @@
     except:
         return -1
 
 def run():
     parser = argparse.ArgumentParser()
     parser.add_argument("-id", "--taxon_id", type=int, help="the taxon ID", required=True)
     parser.add_argument("-t", "--thread_num", type=int, help="number of threads", default=1)
+    parser.add_argument("-bv", "--bogus_value", type=str, help="custom bogus values to be filtered out from the results, comma seperated", default="")
+    parser.add_argument("-bd", "--bogus_default", type=str, help="use or not use the default bogus values, true/false", default="true")
 
     args = parser.parse_args()
     # print(args)
 
     taxon_id = args.taxon_id
     multi_proc_num = args.thread_num
+    custom_bogus = args.bogus_value
+    use_default_bogus = args.bogus_default.strip().lower()
 
     if multi_proc_num <= 0:
         raise ValueError("Bad argument: -t")
 
+    if use_default_bogus != "true" and use_default_bogus != "false":
+        raise ValueError("Bad argument: -bd, accept: true, false")
+
+    if use_default_bogus == "true":
+        use_default_bogus = 1
+    else:
+        use_default_bogus = 0
+
+    custom_bogus_list = []
+    if custom_bogus != "":
+        custom_bogus_list_raw = (custom_bogus.strip().strip(",").strip()).split(",")
+        for i in custom_bogus_list_raw:
+            if i.strip() != "":
+                custom_bogus_list.append(i.strip())
+        if len(custom_bogus_list) > 0:
+            print("Custom bogus values:", custom_bogus_list)
+
     print("Collecting metadata...")
     total_links_count = check_taxon(taxon_id)
     if total_links_count <= 0:
         raise InvalidTaxonException("Bad taxon ID")
 
     manager = multiprocessing.Manager()
     accession_list = manager.list()
@@ -206,15 +235,15 @@
     # process_watcher.join()
 
     job_pool = allocate_jobs(accession_list, multi_proc_num)
 
     data = manager.list()
     data_failed = manager.list()
     process_watcher = multiprocessing.Process(target=watcher, args=(total_links_count, data, data_failed))
-    process_collect_data = multiprocessing.Process(target=collect_data, args=(job_pool, data, data_failed))
+    process_collect_data = multiprocessing.Process(target=collect_data, args=(job_pool, data, data_failed, custom_bogus_list, use_default_bogus))
     process_collect_data.start()
     process_watcher.start()
     process_collect_data.join()
     process_watcher.join()
 
     # retry
     while len(data_failed) > 0:
@@ -222,15 +251,15 @@
         print("Number of failed requests:", len(data_failed))
         print("Retying failed requests...")
 
         total_links_count_failed = len(data_failed)
         job_pool = allocate_jobs(data_failed, multi_proc_num)
 
         # process_watcher = multiprocessing.Process(target=watcher, args=(total_links_count_failed, data_failed))
-        process_collect_data = multiprocessing.Process(target=collect_data, args=(job_pool, data, data_failed))
+        process_collect_data = multiprocessing.Process(target=collect_data, args=(job_pool, data, data_failed, custom_bogus_list, use_default_bogus))
         process_collect_data.start()
         # process_watcher.start()
         process_collect_data.join()
         # process_watcher.join()
 
     # Sorting
     headers = []
```

### Comparing `ncbimetadata-0.1.1/ncbimetadata.egg-info/PKG-INFO` & `ncbimetadata-0.1.2/ncbimetadata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.1.1
+Version: 0.1.2
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
 Home-page: https://github.com/RyanYuanSun/ncbimetadata
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
```

### Comparing `ncbimetadata-0.1.1/setup.py` & `ncbimetadata-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readfile(filename):
     with open(filename, 'r+') as f:
         return f.read()
 
 
 setup(
     name="ncbimetadata",
-    version="0.1.1",
+    version="0.1.2",
     description="ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!",
     long_description=readfile('README.md'),
     long_description_content_type='text/markdown',
     author="Ryan Alloriadonis",
     author_email="yuantai78@gmail.com",
     url="https://github.com/RyanYuanSun/ncbimetadata",
     py_modules=['ncbimetadata'],
```

