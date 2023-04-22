# Comparing `tmp/naturalspeech2-pytorch-0.0.2.tar.gz` & `tmp/naturalspeech2-pytorch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naturalspeech2-pytorch-0.0.2.tar", last modified: Fri Apr 21 20:33:08 2023, max compression
+gzip compressed data, was "naturalspeech2-pytorch-0.0.3.tar", last modified: Sat Apr 22 19:10:51 2023, max compression
```

## Comparing `naturalspeech2-pytorch-0.0.2.tar` & `naturalspeech2-pytorch-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:33:08.643231 naturalspeech2-pytorch-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-21 20:32:57.000000 naturalspeech2-pytorch-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-21 20:33:08.643231 naturalspeech2-pytorch-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-21 20:32:57.000000 naturalspeech2-pytorch-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:33:08.643231 naturalspeech2-pytorch-0.0.2/naturalspeech2_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-21 20:32:57.000000 naturalspeech2-pytorch-0.0.2/naturalspeech2_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18972 2023-04-21 20:32:57.000000 naturalspeech2-pytorch-0.0.2/naturalspeech2_pytorch/naturalspeech2_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:33:08.643231 naturalspeech2-pytorch-0.0.2/naturalspeech2_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-21 20:33:08.000000 naturalspeech2-pytorch-0.0.2/naturalspeech2_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-21 20:33:08.000000 naturalspeech2-pytorch-0.0.2/naturalspeech2_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:33:08.000000 naturalspeech2-pytorch-0.0.2/naturalspeech2_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-21 20:33:08.000000 naturalspeech2-pytorch-0.0.2/naturalspeech2_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 20:33:08.000000 naturalspeech2-pytorch-0.0.2/naturalspeech2_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 20:33:08.643231 naturalspeech2-pytorch-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-21 20:32:57.000000 naturalspeech2-pytorch-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:10:51.409813 naturalspeech2-pytorch-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 19:10:35.000000 naturalspeech2-pytorch-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-22 19:10:51.409813 naturalspeech2-pytorch-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-22 19:10:35.000000 naturalspeech2-pytorch-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:10:51.409813 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-22 19:10:35.000000 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22955 2023-04-22 19:10:35.000000 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch/naturalspeech2_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:10:51.409813 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-22 19:10:51.000000 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-22 19:10:51.000000 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:10:51.000000 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-22 19:10:51.000000 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-22 19:10:51.000000 naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 19:10:51.409813 naturalspeech2-pytorch-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-22 19:10:35.000000 naturalspeech2-pytorch-0.0.3/setup.py
```

### Comparing `naturalspeech2-pytorch-0.0.2/LICENSE` & `naturalspeech2-pytorch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `naturalspeech2-pytorch-0.0.2/PKG-INFO` & `naturalspeech2-pytorch-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalspeech2-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Natural Speech 2 - Pytorch
 Home-page: https://github.com/lucidrains/naturalspeech2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,latent diffusion,speech synthesis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `naturalspeech2-pytorch-0.0.2/README.md` & `naturalspeech2-pytorch-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `naturalspeech2-pytorch-0.0.2/naturalspeech2_pytorch/naturalspeech2_pytorch.py` & `naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch/naturalspeech2_pytorch.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,28 +25,151 @@
 
 from tqdm.auto import tqdm
 
 # constants
 
 mlist = nn.ModuleList
 
+def Sequential(*mods):
+    return nn.Sequential(*filter(exists, mods))
+
 # helpers functions
 
 def exists(x):
     return x is not None
 
 def default(val, d):
     if exists(val):
         return val
     return d() if callable(d) else d
 
 def identity(t, *args, **kwargs):
     return t
 
-# model, which is ~transformer
+# model, which is wavenet + transformer
+
+class CausalConv1d(nn.Conv1d):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        kernel_size, = self.kernel_size
+        dilation, = self.dilation
+        stride, = self.stride
+
+        assert stride == 1
+        self.causal_padding = dilation * (kernel_size - 1)
+
+    def forward(self, x):
+        causal_padded_x = F.pad(x, (self.causal_padding, 0), value = 0.)
+        return super().forward(causal_padded_x)
+
+class WavenetResBlock(nn.Module):
+    def __init__(
+        self,
+        dim,
+        *,
+        dilation,
+        kernel_size = 3,
+        skip_conv = False
+    ):
+        super().__init__()
+        self.conv = CausalConv1d(dim, dim, kernel_size, dilation = dilation)
+        self.res_conv = CausalConv1d(dim, dim, 1)
+        self.skip_conv = CausalConv1d(dim, dim, 1) if skip_conv else None
+
+    def forward(self, x):
+        res = self.res_conv(x)
+
+        x = self.conv(x)
+        x = x.tanh() * x.sigmoid()
+
+        x = x + res
+
+        skip = None
+        if exists(self.skip_conv):
+            skip = self.skip_conv(x)
+
+        return x, skip
+
+
+class WavenetStack(nn.Module):
+    def __init__(
+        self,
+        dim,
+        *,
+        layers,
+        kernel_size = 3,
+        has_skip = False
+    ):
+        super().__init__()
+        dilations = 2 ** torch.arange(layers)
+
+        self.has_skip = has_skip
+        self.blocks = mlist([])
+
+        for dilation in dilations.tolist():
+            block = WavenetResBlock(
+                dim = dim,
+                kernel_size = kernel_size,
+                dilation = dilation,
+                skip_conv = has_skip
+            )
+
+            self.blocks.append(block)
+
+    def forward(self, x):
+        residuals = []
+        skips = []
+
+        if isinstance(x, torch.Tensor):
+            x = (x,) * len(self.blocks)
+
+        for block_input, block in zip(x, self.blocks):
+            residual, skip = block(block_input)
+
+            residuals.append(residual)
+            skips.append(skip)
+
+        if self.has_skip:
+            return torch.stack(skips)
+
+        return residuals
+
+class Wavenet(nn.Module):
+    def __init__(
+        self,
+        dim,
+        *,
+        init_conv_kernel = 3,
+        stacks,
+        layers
+    ):
+        super().__init__()
+        self.init_conv = CausalConv1d(dim, dim, init_conv_kernel)
+        self.stacks = mlist([])
+
+        for ind in range(stacks):
+            is_last = ind == (stacks - 1)
+
+            stack = WavenetStack(
+                dim,
+                layers = layers,
+                has_skip = is_last
+            )
+
+            self.stacks.append(stack)
+
+        self.final_conv = CausalConv1d(dim, dim, 1)
+
+    def forward(self, x):
+        x = self.init_conv(x)
+
+        for stack in self.stacks:
+            x = stack(x)
+
+        return self.final_conv(x.sum(dim = 0))
 
 class RMSNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.scale = dim ** 0.5
         self.gamma = nn.Parameter(torch.ones(dim))
 
@@ -57,24 +180,25 @@
     def __init__(
         self,
         dim,
         *,
         depth,
         dim_head = 64,
         heads = 8,
-        ff_mult = 4
+        ff_mult = 4,
+        ff_causal_conv = False
     ):
         super().__init__()
         self.dim = dim
         self.layers = mlist([])
 
         for _ in range(depth):
             self.layers.append(mlist([
                 Attention(dim = dim, dim_head = dim_head, heads = heads),
-                FeedForward(dim = dim, mult = ff_mult)
+                FeedForward(dim = dim, mult = ff_mult, causal_conv = ff_causal_conv)
             ]))
 
         self.to_pred = nn.Sequential(
             RMSNorm(dim),
             nn.Linear(dim, dim, bias = False)
         )
 
@@ -85,27 +209,73 @@
     ):
         for attn, ff in self.layers:
             x = attn(x) + x
             x = ff(x) + x
 
         return self.to_pred(x)
 
+class Model(nn.Module):
+    def __init__(
+        self,
+        dim,
+        *,
+        depth,
+        dim_head = 64,
+        heads = 8,
+        ff_mult = 4,
+        wavenet_layers = 8,
+        wavenet_stacks = 4
+    ):
+        super().__init__()
+        self.wavenet = Wavenet(
+            dim = dim,
+            stacks = wavenet_stacks,
+            layers = wavenet_layers
+        )
+
+        self.transformer = Transformer(
+            dim = dim,
+            depth = depth,
+            dim_head = dim_head,
+            heads = heads,
+            ff_mult = ff_mult,
+            ff_causal_conv = True
+        )
+
+    def forward(self, x):
+        x = rearrange(x, 'b n d -> b d n')
+        x = self.wavenet(x)
+        x = rearrange(x, 'b d n -> b n d')
+
+        x = self.transformer(x)
+        return x
+
 # feedforward
 
 class GEGLU(nn.Module):
     def forward(self, x):
         x, gate = x.chunk(2, dim = -1)
         return F.gelu(gate) * x
 
-def FeedForward(dim, mult = 4):
+def FeedForward(dim, mult = 4, causal_conv = False):
     dim_inner = int(dim * mult * 2 / 3)
-    return nn.Sequential(
+
+    conv = None
+    if causal_conv:
+        conv = nn.Sequential(
+            Rearrange('b n d -> b d n'),
+            CausalConv1d(dim_inner, dim_inner, 3),
+            Rearrange('b d n -> b n d'),
+        )
+
+    return Sequential(
         RMSNorm(dim),
         nn.Linear(dim, dim_inner * 2),
         GEGLU(),
+        conv,
         nn.Linear(dim_inner, dim)
     )
 
 # attention
 
 class Attention(nn.Module):
     def __init__(
@@ -188,15 +358,15 @@
 # gaussian diffusion
 
 class NaturalSpeech2(nn.Module):
 
     @beartype
     def __init__(
         self,
-        model: Transformer,
+        model: Model,
         codec: Optional[Union[SoundStream, EncodecWrapper]] = None,
         *,
         timesteps = 1000,
         use_ddim = True,
         noise_schedule = 'sigmoid',
         objective = 'v',
         schedule_kwargs: dict = dict(),
@@ -630,16 +800,16 @@
                     if self.step != 0 and self.step % self.save_and_sample_every == 0:
                         self.ema.ema_model.eval()
 
                         with torch.no_grad():
                             milestone = self.step // self.save_and_sample_every
                             batches = num_to_groups(self.num_samples, self.batch_size)
                             all_samples_list = list(map(lambda n: self.ema.ema_model.sample(batch_size=n), batches))
-                        #
+
                         all_samples = torch.cat(all_samples_list, dim = 0)
-                        #
+
                         torch.save(all_samples, str(self.results_folder / f'sample-{milestone}.png'))
                         self.save(milestone)
 
                 pbar.update(1)
 
         accelerator.print('training complete')
```

### Comparing `naturalspeech2-pytorch-0.0.2/naturalspeech2_pytorch.egg-info/PKG-INFO` & `naturalspeech2-pytorch-0.0.3/naturalspeech2_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalspeech2-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Natural Speech 2 - Pytorch
 Home-page: https://github.com/lucidrains/naturalspeech2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,latent diffusion,speech synthesis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `naturalspeech2-pytorch-0.0.2/setup.py` & `naturalspeech2-pytorch-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'naturalspeech2-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'Natural Speech 2 - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/naturalspeech2-pytorch',
   keywords = [
```

