# Comparing `tmp/doc_transformers-1.0.tar.gz` & `tmp/doc_transformers-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doc_transformers-1.0.tar", last modified: Sat Apr 22 04:56:19 2023, max compression
+gzip compressed data, was "doc_transformers-1.0.1.tar", last modified: Sat Apr 22 10:07:08 2023, max compression
```

## Comparing `doc_transformers-1.0.tar` & `doc_transformers-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:56:19.377517 doc_transformers-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-22 04:56:05.000000 doc_transformers-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-22 04:56:19.377517 doc_transformers-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-22 04:56:05.000000 doc_transformers-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:56:19.373517 doc_transformers-1.0/doc_transformers/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:56:05.000000 doc_transformers-1.0/doc_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-22 04:56:05.000000 doc_transformers-1.0/doc_transformers/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:56:19.373517 doc_transformers-1.0/doc_transformers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-22 04:56:19.000000 doc_transformers-1.0/doc_transformers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-22 04:56:19.000000 doc_transformers-1.0/doc_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:56:19.000000 doc_transformers-1.0/doc_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:56:19.000000 doc_transformers-1.0/doc_transformers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-22 04:56:19.000000 doc_transformers-1.0/doc_transformers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-22 04:56:19.000000 doc_transformers-1.0/doc_transformers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-22 04:56:19.377517 doc_transformers-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-22 04:56:05.000000 doc_transformers-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:07:08.029289 doc_transformers-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-22 10:06:52.000000 doc_transformers-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-22 10:07:08.029289 doc_transformers-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-22 10:06:52.000000 doc_transformers-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:07:08.029289 doc_transformers-1.0.1/doc_transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 10:06:52.000000 doc_transformers-1.0.1/doc_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-22 10:06:52.000000 doc_transformers-1.0.1/doc_transformers/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:07:08.029289 doc_transformers-1.0.1/doc_transformers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-22 10:07:07.000000 doc_transformers-1.0.1/doc_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-22 10:07:08.000000 doc_transformers-1.0.1/doc_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 10:07:07.000000 doc_transformers-1.0.1/doc_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 10:07:07.000000 doc_transformers-1.0.1/doc_transformers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-22 10:07:07.000000 doc_transformers-1.0.1/doc_transformers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-22 10:07:07.000000 doc_transformers-1.0.1/doc_transformers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-22 10:07:08.029289 doc_transformers-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-22 10:06:52.000000 doc_transformers-1.0.1/setup.py
```

### Comparing `doc_transformers-1.0/LICENSE` & `doc_transformers-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `doc_transformers-1.0/PKG-INFO` & `doc_transformers-1.0.1/doc_transformers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: doc_transformers
-Version: 1.0
+Name: doc-transformers
+Version: 1.0.1
 Summary: Deep learning for document processing
 Home-page: https://github.com/Vishnunkumar/doc_transformers/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: doc_transformers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `doc_transformers-1.0/README.md` & `doc_transformers-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `doc_transformers-1.0/doc_transformers/parser.py` & `doc_transformers-1.0.1/doc_transformers/parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,96 @@
 import pandas as pd
 import numpy as np
 import pytesseract
 import torch
 from itertools import groupby
-from transformers import LayoutLMv3Processor, LayoutLMv3ForTokenClassification
+from transformers import LayoutLMv3Processor, LayoutLMv3ForTokenClassification, LayoutLMv2FeatureExtractor
 from datasets import load_dataset
 from PIL import Image, ImageDraw, ImageFont
 
-datasets = load_dataset("nielsr/funsd")
-labels = datasets['train'].features['ner_tags'].feature.names
-id2label = {v: k for v, k in enumerate(labels)}
-label2id = {k: v for v, k in enumerate(labels)}
+def load_tags():
+
+  datasets = load_dataset("nielsr/funsd")
+  labels = datasets['train'].features['ner_tags'].feature.names
+  
+  return labels
 
 def load_models():
   
+  feature_extractor = LayoutLMv2FeatureExtractor("microsoft/layoutlmv3-base", apply_ocr=True)
   processor = LayoutLMv3Processor.from_pretrained("microsoft/layoutlmv3-base")
-  model = LayoutLMv3ForTokenClassification.from_pretrained(
-      "nielsr/layoutlmv3-finetuned-funsd"
-  )
+  model = LayoutLMv3ForTokenClassification.from_pretrained("nielsr/layoutlmv3-finetuned-funsd")
   
-  return processor, model
+  return feature_extractor, processor, model
 
 def load_image(path):
   
-  image = Image.open(path)
-  image = image.convert("RGB")
-  
+  image = Image.open(path).convert("RGB")
   return image
 
 def unnormalize_box(bbox, width, height):
  
   return [
          width * (bbox[0] / 1000),
          height * (bbox[1] / 1000),
          width * (bbox[2] / 1000),
          height * (bbox[3] / 1000),
      ]
 
-def process_image(image, processor, model):
+def iob_to_label(label):
+  
+  label = label[2:]
+  if not label:
+    return 'other'
+  return label
+
+
+def process_image(image, feature_extractor, processor, model, labels):
   
+  id2label = {v: k for v, k in enumerate(labels)}
+  label2id = {k: v for v, k in enumerate(labels)}
   width, height = image.size
+
+  encods = feature_extractor(image, return_tensors="pt")
   encoding = processor(image, truncation=True, return_offsets_mapping=True, return_tensors="pt")
   offset_mapping = encoding.pop("offset_mapping")
 
   outputs = model(**encoding)
-
   predictions = outputs.logits.argmax(-1).squeeze().tolist()
   token_boxes = encoding.bbox.squeeze().tolist()
 
   is_subword = np.array(offset_mapping.squeeze().tolist())[:, 0] != 0
   true_predictions = [id2label[pred] for idx, pred in enumerate(predictions) if not is_subword[idx]]
-  true_boxes = [
-      unnormalize_box(box, width, height)
-      for idx, box in enumerate(token_boxes)
-      if not is_subword[idx]
-  ]
-  
-  true_boxes = true_boxes[1:-1]
-  true_predictions = true_predictions[1:-1]
+  true_boxes = [unnormalize_box(box, width, height) for idx, box in enumerate(token_boxes) if not is_subword[idx]]
 
-  preds = []
+  words = encods.words
+  n = len(true_predictions) - len(words[0])
+  k = int(n/2)
+  true_predictions = true_predictions[k:-k]
+  true_boxes = true_boxes[k:-k]
+  
   l_words = []
+  preds = []
   bboxes = []
+  key_pairs = []
 
-  for i,j in enumerate(true_predictions):
-
-    if j != 'O':
-      preds.append(true_predictions[i])
-      l_words.append(words[0][i])
-      bboxes.append(true_boxes[i])
-
-  return bboxes, preds, l_words, image
-
-def iob_to_label(label):
-  label = label[2:]
-  if not label:
-    return 'other'
-  return label
-
+  for i in range(0, len(words[0])):
+    json_dict = {}
+    if true_predictions[i] not in ["O"]:
+      if true_predictions[i] in ["B-HEADER", "I-HEADER"]:
+        json_dict["label"] = "TITLE"
+      elif true_predictions[i] in ["B-QUESTION", "I-QUESTION"]:
+        json_dict["label"] = "KEY"
+      else:
+        json_dict["label"] = "VALUE"
+      json_dict["value"] = words[0][i]
+      key_pairs.append(json_dict)
+  
+  return key_pairs
+  
 def visualize_image(final_bbox, final_preds, l_words, image):
 
   draw = ImageDraw.Draw(image)
   font = ImageFont.load_default()
   
   label2color = {'question':'blue', 'answer':'green', 'header':'orange', 'other':'violet'}
   l2l = {'question':'key', 'answer':'value', 'header':'title'}
```

### Comparing `doc_transformers-1.0/doc_transformers.egg-info/PKG-INFO` & `doc_transformers-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: doc-transformers
-Version: 1.0
+Name: doc_transformers
+Version: 1.0.1
 Summary: Deep learning for document processing
 Home-page: https://github.com/Vishnunkumar/doc_transformers/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: doc_transformers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `doc_transformers-1.0/setup.py` & `doc_transformers-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   'pandas',
   'numpy'
 ]
 
 
 setuptools.setup(
     name="doc_transformers",
-    version="1.0",
+    version="1.0.1",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Deep learning for document processing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/doc_transformers/',
     packages=[
```

