# Comparing `tmp/crowdcores-1.0.3.tar.gz` & `tmp/crowdcores-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdcores-1.0.3.tar", last modified: Wed Apr 19 23:04:09 2023, max compression
+gzip compressed data, was "crowdcores-1.0.4.tar", last modified: Fri Apr 21 23:09:28 2023, max compression
```

## Comparing `crowdcores-1.0.3.tar` & `crowdcores-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 23:04:09.057646 crowdcores-1.0.3/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 22:40:47.000000 crowdcores-1.0.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-19 23:04:09.057646 crowdcores-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      754 2023-04-19 22:48:59.000000 crowdcores-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 23:04:09.053646 crowdcores-1.0.3/crowdcores/
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-19 23:02:37.000000 crowdcores-1.0.3/crowdcores/__init__.py
--rw-r--r--   0 root         (0) root         (0)      835 2023-04-19 22:47:45.000000 crowdcores-1.0.3/crowdcores/pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 23:04:09.053646 crowdcores-1.0.3/crowdcores.egg-info/
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-19 23:04:08.000000 crowdcores-1.0.3/crowdcores.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      245 2023-04-19 23:04:09.000000 crowdcores-1.0.3/crowdcores.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 23:04:08.000000 crowdcores-1.0.3/crowdcores.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-19 23:04:08.000000 crowdcores-1.0.3/crowdcores.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-19 23:04:08.000000 crowdcores-1.0.3/crowdcores.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 23:04:09.057646 crowdcores-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      176 2023-04-19 23:02:44.000000 crowdcores-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:09:28.667064 crowdcores-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 22:40:47.000000 crowdcores-1.0.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-21 23:09:28.667064 crowdcores-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      747 2023-04-19 23:05:28.000000 crowdcores-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:09:28.663064 crowdcores-1.0.4/crowdcores/
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-19 23:02:37.000000 crowdcores-1.0.4/crowdcores/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-04-21 22:25:15.000000 crowdcores-1.0.4/crowdcores/pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:09:28.667064 crowdcores-1.0.4/crowdcores.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-21 23:09:28.000000 crowdcores-1.0.4/crowdcores.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      245 2023-04-21 23:09:28.000000 crowdcores-1.0.4/crowdcores.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 23:09:28.000000 crowdcores-1.0.4/crowdcores.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-21 23:09:28.000000 crowdcores-1.0.4/crowdcores.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-21 23:09:28.000000 crowdcores-1.0.4/crowdcores.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 23:09:28.667064 crowdcores-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      176 2023-04-21 23:09:11.000000 crowdcores-1.0.4/setup.py
```

### Comparing `crowdcores-1.0.3/LICENSE.txt` & `crowdcores-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crowdcores-1.0.3/README.md` & `crowdcores-1.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # CrowdCores Pipeline 
 
 Learn more about [CrowdCores on the official website](https://www.crowdcores.com)
 
 To run a CrowdCores Pipeline install the package:
 
 ```
-pip3 install crowdcores
+pip install crowdcores
 ```
 
 The crowdcores_pipeline works just the same as transformers pipeline from hugging face, you simply need to import crowdcores_pipeline and replace any pipeline calls with crowdcores_pipeline. Here is an example:
 
 
 ```
 from crowdcores import crowdcores_pipeline
-#from transformers import pipeline
-...
-...
-
+#from transformers import pipeline 
 
 #note: we use crowdcore_pipeline instead of pipeline
 #generator=pipeline('text-generation', model='gpt2');
 generator=crowdcores_pipeline('text-generation', model='gpt2');
 r=generator("how are you doing ", max_length=30, num_return_sequences=4)
 print(r)
 ```
 
+
+
```

