# Comparing `tmp/clipcrop-2.4.2.tar.gz` & `tmp/clipcrop-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcrop-2.4.2.tar", last modified: Mon Apr 17 15:07:18 2023, max compression
+gzip compressed data, was "clipcrop-2.4.3.tar", last modified: Sat Apr 22 04:14:00 2023, max compression
```

## Comparing `clipcrop-2.4.2.tar` & `clipcrop-2.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:07:18.570051 clipcrop-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-17 15:07:08.000000 clipcrop-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-17 15:07:18.570051 clipcrop-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-17 15:07:08.000000 clipcrop-2.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:07:18.570051 clipcrop-2.4.2/clipcrop/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:07:08.000000 clipcrop-2.4.2/clipcrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-17 15:07:08.000000 clipcrop-2.4.2/clipcrop/clipcrop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:07:18.570051 clipcrop-2.4.2/clipcrop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-17 15:07:18.000000 clipcrop-2.4.2/clipcrop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 15:07:18.000000 clipcrop-2.4.2/clipcrop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:07:18.000000 clipcrop-2.4.2/clipcrop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:07:18.000000 clipcrop-2.4.2/clipcrop.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 15:07:18.000000 clipcrop-2.4.2/clipcrop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 15:07:18.000000 clipcrop-2.4.2/clipcrop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 15:07:18.570051 clipcrop-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-17 15:07:08.000000 clipcrop-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:14:00.495897 clipcrop-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-22 04:13:51.000000 clipcrop-2.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-22 04:14:00.495897 clipcrop-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-22 04:13:51.000000 clipcrop-2.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:14:00.495897 clipcrop-2.4.3/clipcrop/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:13:51.000000 clipcrop-2.4.3/clipcrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-22 04:13:51.000000 clipcrop-2.4.3/clipcrop/clipcrop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:14:00.495897 clipcrop-2.4.3/clipcrop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-22 04:14:00.000000 clipcrop-2.4.3/clipcrop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-22 04:14:00.000000 clipcrop-2.4.3/clipcrop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:14:00.000000 clipcrop-2.4.3/clipcrop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:14:00.000000 clipcrop-2.4.3/clipcrop.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-22 04:14:00.000000 clipcrop-2.4.3/clipcrop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-22 04:14:00.000000 clipcrop-2.4.3/clipcrop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-22 04:14:00.499897 clipcrop-2.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-22 04:13:51.000000 clipcrop-2.4.3/setup.py
```

### Comparing `clipcrop-2.4.2/LICENSE` & `clipcrop-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clipcrop-2.4.2/PKG-INFO` & `clipcrop-2.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 2.4.2
+Version: 2.4.3
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clipcrop-2.4.2/README.md` & `clipcrop-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `clipcrop-2.4.2/clipcrop/clipcrop.py` & `clipcrop-2.4.3/clipcrop/clipcrop.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
   def __init__(self, input_path, input_text):
     
     self.input_path = input_path
     self.input_text = input_text
 
   def load_models(self):
     
-    segmentor = pipeline("image-segmentation")
+    segmentor = pipeline("image-segmentation", model="facebook/maskformer-swin-tiny-coco")
     model = CLIPModel.from_pretrained("openai/clip-vit-base-patch32")
     processor = CLIPProcessor.from_pretrained("openai/clip-vit-base-patch32") 
 
     return segmentor, model, processor
 
   def unmask(self, img, segim):
 
@@ -187,8 +187,8 @@
       nz = np.uint8(nz * 255)
       res = np.dstack((res_cv, nz))
       respl = Image.fromarray(res)  
       seg_dict["image"] = respl
       seg_dict["score"] = scores[x]
       seg_list.append(seg_dict)
     
-    return seg_list
+    return seg_list
```

### Comparing `clipcrop-2.4.2/clipcrop.egg-info/PKG-INFO` & `clipcrop-2.4.3/clipcrop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 2.4.2
+Version: 2.4.3
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
```

