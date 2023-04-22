# Comparing `tmp/vector_quantize_pytorch-1.1.6.tar.gz` & `tmp/vector_quantize_pytorch-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.1.6.tar", last modified: Tue Apr 18 14:58:19 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.2.0.tar", last modified: Sat Apr 22 00:41:00 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.1.6.tar` & `vector_quantize_pytorch-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:19.156818 vector_quantize_pytorch-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-18 14:58:08.000000 vector_quantize_pytorch-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-18 14:58:19.156818 vector_quantize_pytorch-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-04-18 14:58:08.000000 vector_quantize_pytorch-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:58:19.156818 vector_quantize_pytorch-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-18 14:58:08.000000 vector_quantize_pytorch-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:19.156818 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-18 14:58:08.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-18 14:58:08.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-18 14:58:08.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    21552 2023-04-18 14:58:08.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:19.156818 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-18 14:58:19.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-18 14:58:19.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:58:19.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 14:58:19.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 14:58:19.000000 vector_quantize_pytorch-1.1.6/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:41:00.664843 vector_quantize_pytorch-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 00:40:49.000000 vector_quantize_pytorch-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-22 00:41:00.664843 vector_quantize_pytorch-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14067 2023-04-22 00:40:49.000000 vector_quantize_pytorch-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:41:00.664843 vector_quantize_pytorch-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-22 00:40:49.000000 vector_quantize_pytorch-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:41:00.664843 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-22 00:40:49.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-22 00:40:49.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-22 00:40:49.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22114 2023-04-22 00:40:49.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:41:00.664843 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-22 00:41:00.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-22 00:41:00.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:41:00.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-22 00:41:00.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-22 00:41:00.000000 vector_quantize_pytorch-1.2.0/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.1.6/LICENSE` & `vector_quantize_pytorch-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.1.6/PKG-INFO` & `vector_quantize_pytorch-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.1.6
+Version: 1.2.0
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.1.6/README.md` & `vector_quantize_pytorch-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -363,7 +363,15 @@
 ```bibtex
 @inproceedings{Zhang2023GoogleUS,
     title   = {Google USM: Scaling Automatic Speech Recognition Beyond 100 Languages},
     author  = {Yu Zhang and Wei Han and James Qin and Yongqiang Wang and Ankur Bapna and Zhehuai Chen and Nanxin Chen and Bo Li and Vera Axelrod and Gary Wang and Zhong Meng and Ke Hu and Andrew Rosenberg and Rohit Prabhavalkar and Daniel S. Park and Parisa Haghani and Jason Riesa and Ginger Perng and Hagen Soltau and Trevor Strohman and Bhuvana Ramabhadran and Tara N. Sainath and Pedro J. Moreno and Chung-Cheng Chiu and Johan Schalkwyk and Franccoise Beaufays and Yonghui Wu},
     year    = {2023}
 }
 ```
+
+```bibtex
+@inproceedings{Shen2023NaturalSpeech2L,
+    title   = {NaturalSpeech 2: Latent Diffusion Models are Natural and Zero-Shot Speech and Singing Synthesizers},
+    author  = {Kai Shen and Zeqian Ju and Xu Tan and Yanqing Liu and Yichong Leng and Lei He and Tao Qin and Sheng Zhao and Jiang Bian},
+    year    = {2023}
+}
+```
```

#### html2text {}

```diff
@@ -159,7 +159,12 @@
 Recognition Beyond 100 Languages}, author = {Yu Zhang and Wei Han and James Qin
 and Yongqiang Wang and Ankur Bapna and Zhehuai Chen and Nanxin Chen and Bo Li
 and Vera Axelrod and Gary Wang and Zhong Meng and Ke Hu and Andrew Rosenberg
 and Rohit Prabhavalkar and Daniel S. Park and Parisa Haghani and Jason Riesa
 and Ginger Perng and Hagen Soltau and Trevor Strohman and Bhuvana Ramabhadran
 and Tara N. Sainath and Pedro J. Moreno and Chung-Cheng Chiu and Johan
 Schalkwyk and Franccoise Beaufays and Yonghui Wu}, year = {2023} } ```
+```bibtex @inproceedings{Shen2023NaturalSpeech2L, title = {NaturalSpeech 2:
+Latent Diffusion Models are Natural and Zero-Shot Speech and Singing
+Synthesizers}, author = {Kai Shen and Zeqian Ju and Xu Tan and Yanqing Liu and
+Yichong Leng and Lei He and Tao Qin and Sheng Zhao and Jiang Bian}, year =
+{2023} } ```
```

### Comparing `vector_quantize_pytorch-1.1.6/setup.py` & `vector_quantize_pytorch-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.1.6',
+  version = '1.2.0',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import torch
 from torch import nn, einsum
 import torch.nn.functional as F
 from vector_quantize_pytorch.vector_quantize_pytorch import VectorQuantize
 
 from einops import rearrange, repeat, pack, unpack
 
+def exists(val):
+    return val is not None
+
 class RandomProjectionQuantizer(nn.Module):
     """ https://arxiv.org/abs/2202.01855 """
 
     def __init__(
         self,
         *,
         dim,
@@ -36,19 +39,28 @@
             heads = num_codebooks,
             codebook_size = codebook_size,
             use_cosine_sim = True,
             separate_codebook_per_head = True,
             **kwargs
         )
 
-    @torch.no_grad()
-    def forward(self, x):
+    def forward(
+        self,
+        x,
+        indices = None
+    ):
+        return_loss = exists(indices)
 
         x = self.norm(x)
 
         x = einsum('b n d, h d e -> b n h e', x, self.rand_projs)
         x, ps = pack([x], 'b n *')
 
         self.vq.eval()
-        _, indices, _ = self.vq(x)
+        out = self.vq(x, indices = indices)
+
+        if return_loss:
+            _, ce_loss = out
+            return ce_loss
 
+        _, indices, _ = out
         return indices
```

### Comparing `vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/residual_vq.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 import torch
 from torch import nn
 import torch.nn.functional as F
 from vector_quantize_pytorch.vector_quantize_pytorch import VectorQuantize
 
 from einops import rearrange, repeat, pack, unpack
 
+# helper functions
+
+def exists(val):
+    return val is not None
+
 def round_up_multiple(num, mult):
     return ceil(num / mult) * mult
 
 # main class
 
 class ResidualVQ(nn.Module):
     """ Follows Algorithm 1. in https://arxiv.org/pdf/2107.03312.pdf """
@@ -95,24 +100,29 @@
         all_codes, = unpack(all_codes, ps, 'q b * d')
 
         return all_codes
 
     def forward(
         self,
         x,
+        indices = None,
         return_all_codes = False
     ):
-        num_quant, quant_dropout_multiple_of, device = self.num_quantizers, self.quantize_dropout_multiple_of, x.device
+        num_quant, quant_dropout_multiple_of, return_loss, device = self.num_quantizers, self.quantize_dropout_multiple_of, exists(indices), x.device
+
+        assert not (self.accept_image_fmap and exists(indices))
+
         quantized_out = 0.
         residual = x
 
         all_losses = []
         all_indices = []
+        ce_losses = []   # for cross entropy losses across quantizers, if indices are passed in
 
-        should_quantize_dropout = self.training and self.quantize_dropout
+        should_quantize_dropout = self.training and self.quantize_dropout and not return_loss
 
         # sample a layer index at which to dropout further residual quantization
         # also prepare null indices and loss
 
         if should_quantize_dropout:
             rand_quantize_dropout_index = randrange(self.quantize_dropout_cutoff_index, num_quant)
 
@@ -128,21 +138,40 @@
         for quantizer_index, layer in enumerate(self.layers):
 
             if should_quantize_dropout and quantizer_index > rand_quantize_dropout_index:
                 all_indices.append(null_indices)
                 all_losses.append(null_loss)
                 continue
 
-            quantized, indices, loss = layer(residual)
+            layer_indices = None
+            if return_loss:
+                layer_indices = indices[..., quantizer_index]
+
+            quantized, *rest = layer(residual, indices = layer_indices)
+
             residual = residual - quantized.detach()
             quantized_out = quantized_out + quantized
 
-            all_indices.append(indices)
+            if return_loss:
+                ce_loss = rest[0]
+                ce_losses.append(ce_loss)
+                continue
+
+            embed_indices, loss = rest
+
+            all_indices.append(embed_indices)
             all_losses.append(loss)
 
+        # whether to early return the cross entropy loss
+
+        if return_loss:
+            return quantized_out, sum(ce_losses)
+
+        # stack all losses and indices
+
         all_losses, all_indices = map(partial(torch.stack, dim = -1), (all_losses, all_indices))
 
         ret = (quantized_out, all_indices, all_losses)
 
         if return_all_codes:
             # whether to return all codes from all codebooks across layers
             all_codes = self.get_codes_from_indices(all_indices)
```

### Comparing `vector_quantize_pytorch-1.1.6/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.2.0/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -297,15 +297,15 @@
             embed_normalized = self.embed_avg / rearrange(cluster_size, '... -> ... 1')
             self.embed.data.copy_(embed_normalized)
             self.expire_codes_(x)
 
         if needs_codebook_dim:
             quantize, embed_ind = map(lambda t: rearrange(t, '1 ... -> ...'), (quantize, embed_ind))
 
-        return quantize, embed_ind
+        return quantize, embed_ind, dist
 
 class CosineSimCodebook(nn.Module):
     def __init__(
         self,
         dim,
         codebook_size,
         num_codebooks = 1,
@@ -437,15 +437,15 @@
 
             self.embed.data.lerp_(embed_normalized, 1 - self.decay)
             self.expire_codes_(x)
 
         if needs_codebook_dim:
             quantize, embed_ind = map(lambda t: rearrange(t, '1 ... -> ...'), (quantize, embed_ind))
 
-        return quantize, embed_ind
+        return quantize, embed_ind, dist
 
 # main class
 
 class VectorQuantize(nn.Module):
     def __init__(
         self,
         dim,
@@ -537,22 +537,23 @@
         codes = rearrange(codes, 'b h n d -> b n (h d)')
         codes, = unpack(codes, ps, 'b * d')
         return codes
 
     def forward(
         self,
         x,
+        indices = None,
         mask = None
     ):
         only_one = x.ndim == 2
 
         if only_one:
             x = rearrange(x, 'b d -> b 1 d')
 
-        shape, device, heads, is_multiheaded, codebook_size = x.shape, x.device, self.heads, self.heads > 1, self.codebook_size
+        shape, device, heads, is_multiheaded, codebook_size, return_loss = x.shape, x.device, self.heads, self.heads > 1, self.codebook_size, exists(indices)
 
         need_transpose = not self.channel_last and not self.accept_image_fmap
 
         if self.accept_image_fmap:
             height, width = x.shape[-2:]
             x = rearrange(x, 'b c h w -> b (h w) c')
 
@@ -561,19 +562,29 @@
 
         x = self.project_in(x)
 
         if is_multiheaded:
             ein_rhs_eq = 'h b n d' if self.separate_codebook_per_head else '1 (b h) n d'
             x = rearrange(x, f'b n (h d) -> {ein_rhs_eq}', h = heads)
 
-        quantize, embed_ind = self._codebook(x)
+        quantize, embed_ind, distances = self._codebook(x)
 
         if self.training:
             quantize = x + (quantize - x).detach()
 
+        if return_loss:
+            if not is_multiheaded:
+                distances = rearrange(distances, '1 (b n) l -> b l n', b = shape[0])
+            elif self.separate_codebook_per_head:
+                distances = rearrange(distances, 'c (b n) l -> b l n c', b = shape[0])
+            else:
+                distances = rearrange(distances, '1 (b h n) l -> b l n h', b = shape[0], h = heads)
+
+            return quantize, F.cross_entropy(distances, indices, ignore_index = -1)
+
         loss = torch.tensor([0.], device = device, requires_grad = self.training)
 
         if self.training:
             if self.commitment_weight > 0:
                 detached_quantize = quantize.detach()
 
                 if exists(mask):
```

### Comparing `vector_quantize_pytorch-1.1.6/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.2.0/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.1.6
+Version: 1.2.0
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

