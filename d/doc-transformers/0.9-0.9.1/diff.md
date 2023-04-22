# Comparing `tmp/doc_transformers-0.9.tar.gz` & `tmp/doc_transformers-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doc_transformers-0.9.tar", last modified: Fri Feb  3 16:32:07 2023, max compression
+gzip compressed data, was "doc_transformers-0.9.1.tar", last modified: Sat Apr 22 04:48:42 2023, max compression
```

## Comparing `doc_transformers-0.9.tar` & `doc_transformers-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:32:07.507927 doc_transformers-0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-03 16:31:56.000000 doc_transformers-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-02-03 16:32:07.507927 doc_transformers-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-02-03 16:31:56.000000 doc_transformers-0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:32:07.507927 doc_transformers-0.9/doc_transformers/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 16:31:56.000000 doc_transformers-0.9/doc_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-02-03 16:31:56.000000 doc_transformers-0.9/doc_transformers/form_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:32:07.507927 doc_transformers-0.9/doc_transformers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-02-03 16:32:07.000000 doc_transformers-0.9/doc_transformers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-02-03 16:32:07.000000 doc_transformers-0.9/doc_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 16:32:07.000000 doc_transformers-0.9/doc_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 16:32:07.000000 doc_transformers-0.9/doc_transformers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-03 16:32:07.000000 doc_transformers-0.9/doc_transformers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-03 16:32:07.000000 doc_transformers-0.9/doc_transformers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-03 16:32:07.507927 doc_transformers-0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-02-03 16:31:56.000000 doc_transformers-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:48:42.118296 doc_transformers-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-22 04:48:31.000000 doc_transformers-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-22 04:48:42.118296 doc_transformers-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-22 04:48:31.000000 doc_transformers-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:48:42.118296 doc_transformers-0.9.1/doc_transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:48:31.000000 doc_transformers-0.9.1/doc_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-22 04:48:31.000000 doc_transformers-0.9.1/doc_transformers/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:48:42.118296 doc_transformers-0.9.1/doc_transformers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-22 04:48:42.000000 doc_transformers-0.9.1/doc_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-22 04:48:42.000000 doc_transformers-0.9.1/doc_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:48:42.000000 doc_transformers-0.9.1/doc_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:48:42.000000 doc_transformers-0.9.1/doc_transformers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-22 04:48:42.000000 doc_transformers-0.9.1/doc_transformers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-22 04:48:42.000000 doc_transformers-0.9.1/doc_transformers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-22 04:48:42.118296 doc_transformers-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-22 04:48:31.000000 doc_transformers-0.9.1/setup.py
```

### Comparing `doc_transformers-0.9/LICENSE` & `doc_transformers-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `doc_transformers-0.9/PKG-INFO` & `doc_transformers-0.9.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,51 @@
-Metadata-Version: 2.1
-Name: doc_transformers
-Version: 0.9
-Summary: Deep learning for document processing
-Home-page: https://github.com/Vishnunkumar/doc_transformers/
-Author: Vishnu Nandakumar
-Author-email: nkumarvishnu25@gmail.com
-License: MIT license
-Keywords: doc_transformers
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Doc Transformers
 Document processing using transformers. This is still in developmental phase, currently supports only extraction of form data i.e (key - value pairs)
 
-```
+```bash
 pip install -q doc-transformers
 ```
 
 ## Pre-requisites
 
 Please install the following seperately
 ```
-sudo apt install tesseract-ocr
+pip install pip --upgrade
+pip install -q git+https://github.com/huggingface/transformers.git
+
+pip install pyyaml==5.1
+
+# workaround: install old version of pytorch since detectron2 hasn't released packages for pytorch 1.9 (issue: https://github.com/facebookresearch/detectron2/issues/3158)
+pip install torch==1.8.0+cu101 torchvision==0.9.0+cu101 -f https://download.pytorch.org/whl/torch_stable.html
+
+# install detectron2 that matches pytorch 1.8
+# See https://detectron2.readthedocs.io/tutorials/install.html for instructions
 pip install -q detectron2 -f https://dl.fbaipublicfiles.com/detectron2/wheels/cu101/torch1.8/index.html
 ```
 
 ## Implementation
 
 ```python
 # loads the pretrained dataset also 
-from doc_transformers import form_parser
+from doc_transformers import parser
 
 # loads the image
-image = form_parser.load_image(input_path_image)
+image = parser.load_image(input_path_image)
+
+# loads the model
+processor, model = parser.load_models()
 
 # gets the bounding boxes, predictions, extracted words and image processed
-bbox, preds, words, image = form_parser.process_image(image)
+bbox, preds, words, image = parser.process_image(image, processor, model)
 
 # returns image and extracted key-value pairs along with title as the output
-im, df = form_parser.visualize_image(bbox, preds, words, image)
+im, df = parser.visualize_image(bbox, preds, words, image)
 
 # process and returns k-v pairs by concatenating relevant strings.
-df_main = form_parser.process_form(df)
+df_main = parser.process_form(df)
 ```
 
 ## Results
 
 **Input & Output**
 
 <p float="left">
```

### Comparing `doc_transformers-0.9/doc_transformers/form_parser.py` & `doc_transformers-0.9.1/doc_transformers/parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import pandas as pd
 import numpy as np
 import pytesseract
 import torch
 from itertools import groupby
-from datasets import load_dataset 
+from transformers import LayoutLMv3Processor, LayoutLMv3ForTokenClassification
+from datasets import load_dataset
 from PIL import Image, ImageDraw, ImageFont
-from transformers import LayoutLMv2FeatureExtractor, LayoutLMv2TokenizerFast
-from transformers import LayoutLMv2ForTokenClassification
 
 datasets = load_dataset("nielsr/funsd")
 labels = datasets['train'].features['ner_tags'].feature.names
 id2label = {v: k for v, k in enumerate(labels)}
 label2id = {k: v for v, k in enumerate(labels)}
 
+def load_models():
+  
+  processor = LayoutLMv3Processor.from_pretrained("microsoft/layoutlmv3-base")
+  model = LayoutLMv3ForTokenClassification.from_pretrained(
+      "nielsr/layoutlmv3-finetuned-funsd"
+  )
+  
+  return processor, model
+
 def load_image(path):
   
   image = Image.open(path)
   image = image.convert("RGB")
   
   return image
 
@@ -25,44 +33,33 @@
   return [
          width * (bbox[0] / 1000),
          height * (bbox[1] / 1000),
          width * (bbox[2] / 1000),
          height * (bbox[3] / 1000),
      ]
 
-def process_image(image):
+def process_image(image, processor, model):
   
-  feature_extractor = LayoutLMv2FeatureExtractor.from_pretrained("microsoft/layoutlmv2-base-uncased")
-  tokenizer = LayoutLMv2TokenizerFast.from_pretrained("microsoft/layoutlmv2-base-uncased")
-
-  encoding_feature_extractor = feature_extractor(image, return_tensors="pt")
-  words, boxes = encoding_feature_extractor.words, encoding_feature_extractor.boxes
-
-  encoding = tokenizer(words, boxes=boxes, return_offsets_mapping=True, return_tensors="pt", truncation=True)
-  offset_mapping = encoding.pop('offset_mapping')
-  encoding["image"] = encoding_feature_extractor.pixel_values
-
-  device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
-  for k,v in encoding.items():
-    encoding[k] = v.to(device)
-
-  # load the fine-tuned model from the hub
-  model = LayoutLMv2ForTokenClassification.from_pretrained("nielsr/layoutlmv2-finetuned-funsd")
-  model.to(device)
+  width, height = image.size
+  encoding = processor(image, truncation=True, return_offsets_mapping=True, return_tensors="pt")
+  offset_mapping = encoding.pop("offset_mapping")
 
-  # forward pass
   outputs = model(**encoding)
-  is_subword = np.array(offset_mapping.squeeze().tolist())[:,0] != 0
+
   predictions = outputs.logits.argmax(-1).squeeze().tolist()
   token_boxes = encoding.bbox.squeeze().tolist()
 
-  width, height = image.size
+  is_subword = np.array(offset_mapping.squeeze().tolist())[:, 0] != 0
   true_predictions = [id2label[pred] for idx, pred in enumerate(predictions) if not is_subword[idx]]
-  true_boxes = [unnormalize_box(box, width, height) for idx, box in enumerate(token_boxes) if not is_subword[idx]]
-
+  true_boxes = [
+      unnormalize_box(box, width, height)
+      for idx, box in enumerate(token_boxes)
+      if not is_subword[idx]
+  ]
+  
   true_boxes = true_boxes[1:-1]
   true_predictions = true_predictions[1:-1]
 
   preds = []
   l_words = []
   bboxes = []
```

### Comparing `doc_transformers-0.9/setup.py` & `doc_transformers-0.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = [            
   'transformers',
-  'pyyaml',
-  'torch',
-  'torchvision',
+  'pyyaml==5.1',
+  'torch==1.8.0+cu101'
+  'torchvision==0.9.0+cu101',
   'datasets',
   'pytesseract',
   'pandas',
   'numpy'
 ]
 
 
 setuptools.setup(
     name="doc_transformers",
-    version="0.9",
+    version="0.9.1",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Deep learning for document processing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/doc_transformers/',
     packages=[
```

