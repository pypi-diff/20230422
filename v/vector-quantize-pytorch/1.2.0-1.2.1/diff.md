# Comparing `tmp/vector_quantize_pytorch-1.2.0.tar.gz` & `tmp/vector_quantize_pytorch-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.2.0.tar", last modified: Sat Apr 22 00:41:00 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.2.1.tar", last modified: Sat Apr 22 17:00:46 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.2.0.tar` & `vector_quantize_pytorch-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:41:00.664843 vector_quantize_pytorch-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 00:40:49.000000 vector_quantize_pytorch-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-22 00:41:00.664843 vector_quantize_pytorch-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14067 2023-04-22 00:40:49.000000 vector_quantize_pytorch-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:41:00.664843 vector_quantize_pytorch-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-22 00:40:49.000000 vector_quantize_pytorch-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:41:00.664843 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-22 00:40:49.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-22 00:40:49.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-22 00:40:49.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    22114 2023-04-22 00:40:49.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:41:00.664843 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-22 00:41:00.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-22 00:41:00.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:41:00.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-22 00:41:00.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-22 00:41:00.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:00:46.481400 vector_quantize_pytorch-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 17:00:32.000000 vector_quantize_pytorch-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-22 17:00:46.481400 vector_quantize_pytorch-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14067 2023-04-22 17:00:32.000000 vector_quantize_pytorch-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 17:00:46.481400 vector_quantize_pytorch-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-22 17:00:32.000000 vector_quantize_pytorch-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:00:46.481400 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-22 17:00:32.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-22 17:00:32.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-22 17:00:32.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22280 2023-04-22 17:00:32.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:00:46.481400 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-22 17:00:46.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-22 17:00:46.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:00:46.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 17:00:46.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-22 17:00:46.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.2.0/LICENSE` & `vector_quantize_pytorch-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.2.0/PKG-INFO` & `vector_quantize_pytorch-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.2.0
+Version: 1.2.1
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.2.0/README.md` & `vector_quantize_pytorch-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.2.0/setup.py` & `vector_quantize_pytorch-1.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.2.0',
+  version = '1.2.1',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
     'artificial intelligence',
     'deep learning',
     'pytorch',
     'quantization'
   ],
   install_requires=[
-    'einops>=0.6',
+    'einops>=0.6.1',
     'torch'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
```

### Comparing `vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,20 @@
 
 def l2norm(t):
     return F.normalize(t, p = 2, dim = -1)
 
 def log(t, eps = 1e-20):
     return torch.log(t.clamp(min = eps))
 
+def pack_one(t, pattern):
+    return pack([t], pattern)
+
+def unpack_one(t, ps, pattern):
+    return unpack(t, ps, pattern)[0]
+
 def uniform_init(*shape):
     t = torch.empty(shape)
     nn.init.kaiming_uniform_(t)
     return t
 
 def gumbel_noise(t):
     noise = torch.zeros_like(t).uniform_(0, 1)
@@ -264,15 +270,15 @@
 
         x = x.float()
 
         if needs_codebook_dim:
             x = rearrange(x, '... -> 1 ...')
 
         shape, dtype = x.shape, x.dtype
-        flatten = rearrange(x, 'h ... d -> h (...) d')
+        flatten, ps = pack_one(x, 'h * d')
 
         self.init_embed_(flatten)
 
         embed = self.embed if not self.learnable_codebook else self.embed.detach()
 
         dist = -torch.cdist(flatten, embed, p = 2)
 
@@ -297,14 +303,16 @@
             embed_normalized = self.embed_avg / rearrange(cluster_size, '... -> ... 1')
             self.embed.data.copy_(embed_normalized)
             self.expire_codes_(x)
 
         if needs_codebook_dim:
             quantize, embed_ind = map(lambda t: rearrange(t, '1 ... -> ...'), (quantize, embed_ind))
 
+        dist = unpack_one(dist, ps, 'h * d')
+
         return quantize, embed_ind, dist
 
 class CosineSimCodebook(nn.Module):
     def __init__(
         self,
         dim,
         codebook_size,
@@ -395,15 +403,15 @@
         x = x.float()
 
         if needs_codebook_dim:
             x = rearrange(x, '... -> 1 ...')
 
         shape, dtype = x.shape, x.dtype
 
-        flatten = rearrange(x, 'h ... d -> h (...) d')
+        flatten, ps = pack_one(x, 'h * d')
         flatten = l2norm(flatten)
 
         self.init_embed_(flatten)
 
         embed = self.embed if not self.learnable_codebook else self.embed.detach()
         embed = l2norm(embed)
 
@@ -437,14 +445,15 @@
 
             self.embed.data.lerp_(embed_normalized, 1 - self.decay)
             self.expire_codes_(x)
 
         if needs_codebook_dim:
             quantize, embed_ind = map(lambda t: rearrange(t, '1 ... -> ...'), (quantize, embed_ind))
 
+        dist = unpack_one(dist, ps, 'h * d')
         return quantize, embed_ind, dist
 
 # main class
 
 class VectorQuantize(nn.Module):
     def __init__(
         self,
@@ -523,23 +532,23 @@
         codebook = self.codebook
         is_multiheaded = codebook.ndim > 2
 
         if not is_multiheaded:
             codes = codebook[indices]
             return rearrange(codes, '... h d -> ... (h d)')
 
-        indices, ps = pack([indices], 'b * h')
+        indices, ps = pack_one(indices, 'b * h')
         indices = rearrange(indices, 'b n h -> b h n')
 
         indices = repeat(indices, 'b h n -> b h n d', d = codebook.shape[-1])
         codebook = repeat(codebook, 'h n d -> b h n d', b = indices.shape[0])
 
         codes = codebook.gather(2, indices)
         codes = rearrange(codes, 'b h n d -> b n (h d)')
-        codes, = unpack(codes, ps, 'b * d')
+        codes = unpack_one(codes, ps, 'b * d')
         return codes
 
     def forward(
         self,
         x,
         indices = None,
         mask = None
@@ -569,20 +578,21 @@
         quantize, embed_ind, distances = self._codebook(x)
 
         if self.training:
             quantize = x + (quantize - x).detach()
 
         if return_loss:
             if not is_multiheaded:
-                distances = rearrange(distances, '1 (b n) l -> b l n', b = shape[0])
+                dist_einops_eq = '1 b n l -> b l n'
             elif self.separate_codebook_per_head:
-                distances = rearrange(distances, 'c (b n) l -> b l n c', b = shape[0])
+                dist_einops_eq = 'c b n l -> b l n c'
             else:
-                distances = rearrange(distances, '1 (b h n) l -> b l n h', b = shape[0], h = heads)
+                dist_einops_eq = '1 (b h) n l -> b l n h'
 
+            distances = rearrange(distances, dist_einops_eq, b = shape[0])
             return quantize, F.cross_entropy(distances, indices, ignore_index = -1)
 
         loss = torch.tensor([0.], device = device, requires_grad = self.training)
 
         if self.training:
             if self.commitment_weight > 0:
                 detached_quantize = quantize.detach()
```

### Comparing `vector_quantize_pytorch-1.2.0/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.2.1/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.2.0
+Version: 1.2.1
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

