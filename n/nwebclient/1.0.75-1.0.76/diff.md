# Comparing `tmp/nwebclient-1.0.75.tar.gz` & `tmp/nwebclient-1.0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.75.tar", last modified: Thu Apr 20 19:27:27 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.76.tar", last modified: Sat Apr 22 17:18:46 2023, max compression
```

## Comparing `nwebclient-1.0.75.tar` & `nwebclient-1.0.76.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 19:27:27.083393 nwebclient-1.0.75/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.75/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-20 19:27:27.083393 nwebclient-1.0.75/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.75/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 19:27:27.083393 nwebclient-1.0.75/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.75/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.75/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3104 2023-03-29 20:50:31.000000 nwebclient-1.0.75/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)     9281 2023-04-20 18:14:27.000000 nwebclient-1.0.75/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5582 2023-03-29 09:33:58.000000 nwebclient-1.0.75/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3218 2023-03-27 16:42:32.000000 nwebclient-1.0.75/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 19:27:27.083393 nwebclient-1.0.75/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-20 19:27:26.000000 nwebclient-1.0.75/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-04-20 19:27:26.000000 nwebclient-1.0.75/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-20 19:27:26.000000 nwebclient-1.0.75/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       84 2023-04-20 19:27:26.000000 nwebclient-1.0.75/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-04-20 19:27:26.000000 nwebclient-1.0.75/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-04-20 19:27:26.000000 nwebclient-1.0.75/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-20 19:27:27.083393 nwebclient-1.0.75/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      829 2023-04-20 18:14:48.000000 nwebclient-1.0.75/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 17:18:46.889350 nwebclient-1.0.76/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.76/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-22 17:18:46.889350 nwebclient-1.0.76/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.76/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 17:18:46.889350 nwebclient-1.0.76/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.76/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.76/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3104 2023-03-29 20:50:31.000000 nwebclient-1.0.76/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     9342 2023-04-22 17:18:10.000000 nwebclient-1.0.76/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     5582 2023-03-29 09:33:58.000000 nwebclient-1.0.76/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3218 2023-03-27 16:42:32.000000 nwebclient-1.0.76/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 17:18:46.889350 nwebclient-1.0.76/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-22 17:18:46.000000 nwebclient-1.0.76/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-04-22 17:18:46.000000 nwebclient-1.0.76/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-22 17:18:46.000000 nwebclient-1.0.76/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       84 2023-04-22 17:18:46.000000 nwebclient-1.0.76/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-04-22 17:18:46.000000 nwebclient-1.0.76/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-04-22 17:18:46.000000 nwebclient-1.0.76/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-22 17:18:46.899350 nwebclient-1.0.76/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      829 2023-04-22 17:18:40.000000 nwebclient-1.0.76/setup.py
```

### Comparing `nwebclient-1.0.75/LICENSE` & `nwebclient-1.0.76/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.75/PKG-INFO` & `nwebclient-1.0.76/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.75
+Version: 1.0.76
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.75/README.md` & `nwebclient-1.0.76/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.75/nwebclient/__init__.py` & `nwebclient-1.0.76/nwebclient/__init__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.75/nwebclient/__main__.py` & `nwebclient-1.0.76/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.75/nwebclient/crypt.py` & `nwebclient-1.0.76/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.75/nwebclient/sd.py` & `nwebclient-1.0.76/nwebclient/sd.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             return
         self.scheduler = DPMSolverMultistepScheduler.from_pretrained(self.model_id, subfolder="scheduler")
         device = "cuda"
         model_revision = None
         if self.scheduler is None:
            self.pipe = StableDiffusionPipeline.from_pretrained(self.model_id, torch_dtype=torch.float16, revision=model_revision)
         else:
-           self.pipe = StableDiffusionPipeline.from_pretrained(self.model_id, scheduler=self.scheduler, custom_pipeline="lpw_stable_diffusion", torch_dtype=torch.float16, revision=model_revision)
+           self.pipe = StableDiffusionPipeline.from_pretrained(self.model_id, scheduler=self.scheduler,  torch_dtype=torch.float16, revision=model_revision) # custom_pipeline="lpw_stable_diffusion",
         self.pipe = self.pipe.to(device)
         if self.model_id=="XpucT/Deliberate" or self.model_id == "SG161222/Realistic_Vision_V1.4_Fantasy.ai":
             self.pipe.safety_checker = lambda images, clip_input: (images, False)
         self.load_model = self.model_id
     def initA1111(self):
         import webuiapi
         if self.api is None:
@@ -172,18 +172,19 @@
         jobs = data['jobs']
         i = 0
         for job in jobs:
             self.info("Job " + str(i) + "/" + str(len(jobs)) )
             self.execute(job)
             i=i+1
         result_url = data['result_url']
-        files = {'upload_file': open('data.db', 'rb')}
-        params = {'name': data['worker_name'], 'g': data['group_id']}
-        res = requests.post(result_url, params=params, files=files)
-        print(res.text)
+        if result_url.startswith('http'):
+            files = {'upload_file': open('data.db', 'rb')}
+            params = {'name': data['worker_name'], 'g': data['group_id']}
+            res = requests.post(result_url, params=params, files=files)
+            print(res.text)
         self.info("End: "+time.strftime("%Y-%m-%d, %H:%M:%S", time.localtime()))
         return i
     def executeFromUrl(self, url):
         res = requests.get(url)
         data = json.loads(res.text)
         return self.executeJobs(data)
     def info(self, message):
```

### Comparing `nwebclient-1.0.75/nwebclient/sdb.py` & `nwebclient-1.0.76/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.75/nwebclient/ticker.py` & `nwebclient-1.0.76/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.75/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.76/nwebclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.75
+Version: 1.0.76
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.75/setup.py` & `nwebclient-1.0.76/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.75",
+    version="1.0.76",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

