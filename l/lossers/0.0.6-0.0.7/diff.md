# Comparing `tmp/lossers-0.0.6.tar.gz` & `tmp/lossers-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lossers-0.0.6.tar", last modified: Wed Apr 19 12:19:28 2023, max compression
+gzip compressed data, was "lossers-0.0.7.tar", last modified: Sat Apr 22 00:17:05 2023, max compression
```

## Comparing `lossers-0.0.6.tar` & `lossers-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:28.827062 lossers-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-19 12:19:19.000000 lossers-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-19 12:19:28.827062 lossers-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 12:19:19.000000 lossers-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:28.823062 lossers-0.0.6/lossers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:19.000000 lossers-0.0.6/lossers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-19 12:19:19.000000 lossers-0.0.6/lossers/clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:28.827062 lossers-0.0.6/lossers/lpips/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 12:19:19.000000 lossers-0.0.6/lossers/lpips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-19 12:19:19.000000 lossers-0.0.6/lossers/lpips/lpips.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-19 12:19:19.000000 lossers-0.0.6/lossers/lpips/pretrained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-19 12:19:19.000000 lossers-0.0.6/lossers/lpips/vgg_v0.1.pth
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-19 12:19:19.000000 lossers-0.0.6/lossers/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-19 12:19:19.000000 lossers-0.0.6/lossers/ssim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:28.823062 lossers-0.0.6/lossers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-19 12:19:28.000000 lossers-0.0.6/lossers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-19 12:19:28.000000 lossers-0.0.6/lossers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:19:28.000000 lossers-0.0.6/lossers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 12:19:28.000000 lossers-0.0.6/lossers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 12:19:28.827062 lossers-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-19 12:19:19.000000 lossers-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:17:05.802178 lossers-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 00:16:50.000000 lossers-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-22 00:17:05.802178 lossers-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-22 00:16:50.000000 lossers-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:17:05.802178 lossers-0.0.7/lossers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:17:05.802178 lossers-0.0.7/lossers/lpips/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/lpips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/lpips/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/lpips/pretrained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/lpips/vgg_v0.1.pth
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-22 00:16:50.000000 lossers-0.0.7/lossers/ssim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:17:05.802178 lossers-0.0.7/lossers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-22 00:17:05.000000 lossers-0.0.7/lossers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-22 00:17:05.000000 lossers-0.0.7/lossers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:17:05.000000 lossers-0.0.7/lossers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-22 00:17:05.000000 lossers-0.0.7/lossers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:17:05.802178 lossers-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-22 00:16:50.000000 lossers-0.0.7/setup.py
```

### Comparing `lossers-0.0.6/LICENSE` & `lossers-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lossers-0.0.6/PKG-INFO` & `lossers-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lossers
-Version: 0.0.6
+Version: 0.0.7
 Summary: Deep Learning Loss Function
 Home-page: https://github.com/JiauZhang/lossers
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: MIT
 Keywords: Deep Learning,Loss Function,Artificial Intelligence
 Classifier: Intended Audience :: Developers
```

### Comparing `lossers-0.0.6/lossers/lpips/lpips.py` & `lossers-0.0.7/lossers/lpips/lpips.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,18 @@
         if(self.pnet_type in ['vgg','vgg16']):
             net_type = pn.VGG16
             self.chns = [64,128,256,512,512]
         else:
             raise RuntimeError('currently only vgg16 supported!')
         self.L = len(self.chns)
 
-        self.net = net_type(pretrained=pretrained, cache_dir=cache_dir)
+        _dir = torch.hub.get_dir()
+        if cache_dir is not None: torch.hub.set_dir(cache_dir)
+        self.net = net_type(pretrained=pretrained)
+        torch.hub.set_dir(_dir)
         self.lin0 = NetLinLayer(self.chns[0], use_dropout=use_dropout)
         self.lin1 = NetLinLayer(self.chns[1], use_dropout=use_dropout)
         self.lin2 = NetLinLayer(self.chns[2], use_dropout=use_dropout)
         self.lin3 = NetLinLayer(self.chns[3], use_dropout=use_dropout)
         self.lin4 = NetLinLayer(self.chns[4], use_dropout=use_dropout)
         self.lins = [self.lin0,self.lin1,self.lin2,self.lin3,self.lin4]
         if(self.pnet_type=='squeeze'): # 7 layers for squeezenet
```

### Comparing `lossers-0.0.6/lossers/lpips/pretrained_model.py` & `lossers-0.0.7/lossers/lpips/pretrained_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from collections import namedtuple
 import torch
 from torchvision import models as tv
 
 class VGG16(torch.nn.Module):
-    def __init__(self, requires_grad=False, pretrained=True, cache_dir=None):
+    def __init__(self, requires_grad=False, pretrained=True):
         super(VGG16, self).__init__()
-        _dir = torch.hub.get_dir()
-        torch.hub.set_dir(cache_dir)
         vgg_pretrained_features = tv.vgg16(pretrained=pretrained).features
-        torch.hub.set_dir(_dir)
         self.slice1 = torch.nn.Sequential()
         self.slice2 = torch.nn.Sequential()
         self.slice3 = torch.nn.Sequential()
         self.slice4 = torch.nn.Sequential()
         self.slice5 = torch.nn.Sequential()
         self.N_slices = 5
         for x in range(4):
```

### Comparing `lossers-0.0.6/lossers/lpips/vgg_v0.1.pth` & `lossers-0.0.7/lossers/lpips/vgg_v0.1.pth`

 * *Files identical despite different names*

### Comparing `lossers-0.0.6/lossers/ssim.py` & `lossers-0.0.7/lossers/ssim.py`

 * *Files identical despite different names*

### Comparing `lossers-0.0.6/lossers.egg-info/PKG-INFO` & `lossers-0.0.7/lossers.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lossers
-Version: 0.0.6
+Version: 0.0.7
 Summary: Deep Learning Loss Function
 Home-page: https://github.com/JiauZhang/lossers
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: MIT
 Keywords: Deep Learning,Loss Function,Artificial Intelligence
 Classifier: Intended Audience :: Developers
```

### Comparing `lossers-0.0.6/setup.py` & `lossers-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'lossers',
     packages = find_packages(exclude=['examples']),
     package_data={'': ['*/vgg_v0.1.pth']},
-    version = '0.0.6',
+    version = '0.0.7',
     license='MIT',
     description = 'Deep Learning Loss Function',
     author = 'JiauZhang',
     author_email = 'jiauzhang@163.com',
     url = 'https://github.com/JiauZhang/lossers',
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
```

