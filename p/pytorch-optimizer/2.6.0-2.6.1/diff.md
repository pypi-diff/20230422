# Comparing `tmp/pytorch_optimizer-2.6.0.tar.gz` & `tmp/pytorch_optimizer-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_optimizer-2.6.0.tar", max compression
+gzip compressed data, was "pytorch_optimizer-2.6.1.tar", max compression
```

## Comparing `pytorch_optimizer-2.6.0.tar` & `pytorch_optimizer-2.6.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    11357 2023-04-22 07:56:58.743183 pytorch_optimizer-2.6.0/LICENSE
--rw-r--r--   0        0        0    28771 2023-04-22 07:56:58.743183 pytorch_optimizer-2.6.0/README.rst
--rw-r--r--   0        0        0     3649 2023-04-22 07:56:58.747183 pytorch_optimizer-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     6062 2023-04-22 07:56:58.747183 pytorch_optimizer-2.6.0/pytorch_optimizer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/base/__init__.py
--rw-r--r--   0        0        0     1583 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/base/exception.py
--rw-r--r--   0        0        0     4183 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/base/optimizer.py
--rw-r--r--   0        0        0     2761 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/base/scheduler.py
--rw-r--r--   0        0        0      491 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/base/types.py
--rw-r--r--   0        0        0        0 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/experimental/__init__.py
--rw-r--r--   0        0        0     1595 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py
--rw-r--r--   0        0        0      131 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/__init__.py
--rw-r--r--   0        0        0      971 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/chebyshev.py
--rw-r--r--   0        0        0     4034 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py
--rw-r--r--   0        0        0     1255 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/linear_warmup.py
--rw-r--r--   0        0        0     1400 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/proportion.py
--rw-r--r--   0        0        0        0 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/__init__.py
--rw-r--r--   0        0        0     7108 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adabelief.py
--rw-r--r--   0        0        0     5460 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adabound.py
--rw-r--r--   0        0        0     7217 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adafactor.py
--rw-r--r--   0        0        0     5941 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adai.py
--rw-r--r--   0        0        0     5223 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adamp.py
--rw-r--r--   0        0        0     5004 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adams.py
--rw-r--r--   0        0        0     5828 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adan.py
--rw-r--r--   0        0        0     5053 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adapnm.py
--rw-r--r--   0        0        0      781 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/agc.py
--rw-r--r--   0        0        0     3857 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/alig.py
--rw-r--r--   0        0        0     5428 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/apollo.py
--rw-r--r--   0        0        0    18352 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/dadapt.py
--rw-r--r--   0        0        0     4165 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/diffgrad.py
--rw-r--r--   0        0        0     5540 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/diffrgrad.py
--rw-r--r--   0        0        0    10702 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/fp16.py
--rw-r--r--   0        0        0      474 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/gc.py
--rw-r--r--   0        0        0     7601 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/gsam.py
--rw-r--r--   0        0        0     5563 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lamb.py
--rw-r--r--   0        0        0     3954 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lars.py
--rw-r--r--   0        0        0     2920 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lion.py
--rw-r--r--   0        0        0     4178 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lookahead.py
--rw-r--r--   0        0        0     6550 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/madgrad.py
--rw-r--r--   0        0        0     3639 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/nero.py
--rw-r--r--   0        0        0     4149 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/novograd.py
--rw-r--r--   0        0        0     4314 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/pcgrad.py
--rw-r--r--   0        0        0     3702 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/pnm.py
--rw-r--r--   0        0        0     5242 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/radam.py
--rw-r--r--   0        0        0     6827 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/ralamb.py
--rw-r--r--   0        0        0     6224 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/ranger.py
--rw-r--r--   0        0        0    12516 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/ranger21.py
--rw-r--r--   0        0        0     4718 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/sam.py
--rw-r--r--   0        0        0     3907 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/sgdp.py
--rw-r--r--   0        0        0    15773 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/shampoo.py
--rw-r--r--   0        0        0    20180 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/shampoo_utils.py
--rw-r--r--   0        0        0     5552 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/sm3.py
--rw-r--r--   0        0        0     7895 2023-04-22 07:56:58.751183 pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/utils.py
--rw-r--r--   0        0        0    30887 1970-01-01 00:00:00.000000 pytorch_optimizer-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-22 12:14:33.011546 pytorch_optimizer-2.6.1/LICENSE
+-rw-r--r--   0        0        0    28771 2023-04-22 12:14:33.011546 pytorch_optimizer-2.6.1/README.rst
+-rw-r--r--   0        0        0     3649 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6062 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/base/__init__.py
+-rw-r--r--   0        0        0     1583 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/base/exception.py
+-rw-r--r--   0        0        0     4183 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/base/optimizer.py
+-rw-r--r--   0        0        0     2761 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/base/scheduler.py
+-rw-r--r--   0        0        0      491 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/base/types.py
+-rw-r--r--   0        0        0        0 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/experimental/__init__.py
+-rw-r--r--   0        0        0     1595 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py
+-rw-r--r--   0        0        0      131 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0      971 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/chebyshev.py
+-rw-r--r--   0        0        0     4034 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/cosine_anealing.py
+-rw-r--r--   0        0        0     1255 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/linear_warmup.py
+-rw-r--r--   0        0        0     1400 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/proportion.py
+-rw-r--r--   0        0        0        0 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/__init__.py
+-rw-r--r--   0        0        0     7108 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adabelief.py
+-rw-r--r--   0        0        0     5460 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adabound.py
+-rw-r--r--   0        0        0     7237 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adafactor.py
+-rw-r--r--   0        0        0     5941 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adai.py
+-rw-r--r--   0        0        0     5223 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adamp.py
+-rw-r--r--   0        0        0     5004 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adams.py
+-rw-r--r--   0        0        0     5828 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adan.py
+-rw-r--r--   0        0        0     5053 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adapnm.py
+-rw-r--r--   0        0        0      781 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/agc.py
+-rw-r--r--   0        0        0     3857 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/alig.py
+-rw-r--r--   0        0        0     5428 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/apollo.py
+-rw-r--r--   0        0        0    18352 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/dadapt.py
+-rw-r--r--   0        0        0     4165 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/diffgrad.py
+-rw-r--r--   0        0        0     5540 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/diffrgrad.py
+-rw-r--r--   0        0        0    10702 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/fp16.py
+-rw-r--r--   0        0        0      474 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/gc.py
+-rw-r--r--   0        0        0     7601 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/gsam.py
+-rw-r--r--   0        0        0     5563 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lamb.py
+-rw-r--r--   0        0        0     3954 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lars.py
+-rw-r--r--   0        0        0     2920 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lion.py
+-rw-r--r--   0        0        0     4178 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lookahead.py
+-rw-r--r--   0        0        0     6550 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/madgrad.py
+-rw-r--r--   0        0        0     3639 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/nero.py
+-rw-r--r--   0        0        0     4149 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/novograd.py
+-rw-r--r--   0        0        0     4314 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/pcgrad.py
+-rw-r--r--   0        0        0     3702 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/pnm.py
+-rw-r--r--   0        0        0     5242 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/radam.py
+-rw-r--r--   0        0        0     6827 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/ralamb.py
+-rw-r--r--   0        0        0     6224 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/ranger.py
+-rw-r--r--   0        0        0    12516 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/ranger21.py
+-rw-r--r--   0        0        0     4718 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/sam.py
+-rw-r--r--   0        0        0     3907 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/sgdp.py
+-rw-r--r--   0        0        0    15773 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/shampoo.py
+-rw-r--r--   0        0        0    20180 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/shampoo_utils.py
+-rw-r--r--   0        0        0     5691 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/sm3.py
+-rw-r--r--   0        0        0     7895 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/utils.py
+-rw-r--r--   0        0        0    30887 1970-01-01 00:00:00.000000 pytorch_optimizer-2.6.1/PKG-INFO
```

### Comparing `pytorch_optimizer-2.6.0/LICENSE` & `pytorch_optimizer-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/README.rst` & `pytorch_optimizer-2.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pyproject.toml` & `pytorch_optimizer-2.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytorch_optimizer"
-version = "2.6.0"
+version = "2.6.1"
 description = "optimizer & lr scheduler implementations in PyTorch with clean-code, strict types. Also, including useful optimization ideas."
 license = "Apache-2.0"
 authors = ["kozistr <kozistr@gmail.com>"]
 maintainers = ["kozistr <kozistr@gmail.com>"]
 readme = "README.rst"
 homepage = "https://github.com/kozistr/pytorch_optimizer"
 repository = "https://github.com/kozistr/pytorch_optimizer"
```

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/__init__.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/base/exception.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/base/exception.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/base/optimizer.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/base/optimizer.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/base/scheduler.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/base/scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/chebyshev.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/chebyshev.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/cosine_anealing.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/linear_warmup.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/linear_warmup.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/lr_scheduler/proportion.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/proportion.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adabelief.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adabelief.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adabound.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adabound.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adafactor.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adafactor.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,16 +77,16 @@
                 grad_shape: Tuple[int, ...] = grad.shape
                 factored: bool = self.get_options(grad_shape)
 
                 state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
 
                 if factored:
-                    state['exp_avg_sq_row'] = torch.zeros(grad_shape[:-1], dtype=grad.dtype)
-                    state['exp_avg_sq_col'] = torch.zeros(grad_shape[:-2] + grad_shape[-1:], dtype=grad.dtype)
+                    state['exp_avg_sq_row'] = torch.zeros(grad_shape[:-1]).to(grad)
+                    state['exp_avg_sq_col'] = torch.zeros(grad_shape[:-2] + grad_shape[-1:]).to(grad)
                 else:
                     state['exp_avg_sq'] = torch.zeros_like(grad)
 
                 state['RMS'] = 0.0
 
     def get_lr(self, lr: float, step: int, rms: float) -> float:
         relative_step_size: float = lr
@@ -110,16 +110,16 @@
 
     @staticmethod
     def approximate_sq_grad(
         exp_avg_sq_row: torch.Tensor,
         exp_avg_sq_col: torch.Tensor,
         output: torch.Tensor,
     ):
-        r"""Get approximate squared gradient."""
-        r_factor: torch.Tensor = (exp_avg_sq_row / exp_avg_sq_row.mean(dim=-1)).rsqrt_().unsqueeze(-1)
+        r"""Get approximation of EMA of squared gradient."""
+        r_factor: torch.Tensor = (exp_avg_sq_row / exp_avg_sq_row.mean(dim=-1, keepdim=True)).rsqrt_().unsqueeze(-1)
         c_factor: torch.Tensor = exp_avg_sq_col.unsqueeze(-2).rsqrt()
         torch.mul(r_factor, c_factor, out=output)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
@@ -141,16 +141,18 @@
                 factored: bool = self.get_options(grad_shape)
 
                 if len(state) == 0:
                     state['step'] = 0
                     state['exp_avg'] = torch.zeros_like(p)
 
                     if factored:
-                        state['exp_avg_sq_row'] = torch.zeros(grad_shape[:-1], dtype=grad.dtype)
-                        state['exp_avg_sq_col'] = torch.zeros(grad_shape[:-2] + grad_shape[-1:], dtype=grad.dtype)
+                        state['exp_avg_sq_row'] = torch.zeros(grad_shape[:-1], dtype=grad.dtype, device=grad.device)
+                        state['exp_avg_sq_col'] = torch.zeros(
+                            grad_shape[:-2] + grad_shape[-1:], dtype=grad.dtype, device=grad.device
+                        )
                     else:
                         state['exp_avg_sq'] = torch.zeros_like(grad)
 
                     state['RMS'] = 0.0
 
                 state['step'] += 1
 
@@ -162,19 +164,17 @@
 
                 if factored:
                     exp_avg_sq_row, exp_avg_sq_col = state['exp_avg_sq_row'], state['exp_avg_sq_col']
 
                     exp_avg_sq_row.mul_(beta2_t).add_(update.mean(dim=-1), alpha=1.0 - beta2_t)
                     exp_avg_sq_col.mul_(beta2_t).add_(update.mean(dim=-2), alpha=1.0 - beta2_t)
 
-                    # Approximation of exponential moving average of square of gradient
-                    self.approximate_sq_grad(exp_avg_sq_row, exp_avg_sq_col, update)
+                    self.approximate_sq_grad(exp_avg_sq_row, exp_avg_sq_col, output=update)
                 else:
                     exp_avg_sq = state['exp_avg_sq']
-
                     exp_avg_sq.mul_(beta2_t).add_(update, alpha=1.0 - beta2_t)
                     torch.rsqrt(exp_avg_sq, out=update)
 
                 update.mul_(grad)
 
                 # TODO: implement AMSGrad
```

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adai.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adai.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adamp.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adamp.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adams.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adams.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adan.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adan.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/adapnm.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adapnm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/agc.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/agc.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/alig.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/alig.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/apollo.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/apollo.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/dadapt.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/dadapt.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/diffgrad.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/diffgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/diffrgrad.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/diffrgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/fp16.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/fp16.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/gsam.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/gsam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lamb.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lamb.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lars.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lion.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lion.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/lookahead.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lookahead.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/madgrad.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/madgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/nero.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/nero.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/novograd.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/novograd.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/pcgrad.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/pcgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/pnm.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/pnm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/radam.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/radam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/ralamb.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/ralamb.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/ranger.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/ranger.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/ranger21.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/ranger21.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/sam.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/sam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/sgdp.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/sgdp.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/shampoo.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/shampoo.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/shampoo_utils.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/shampoo_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/sm3.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/sm3.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,20 +94,22 @@
 
                 state = self.state[p]
                 if len(state) == 0:
                     state['step'] = 0
                     state['momentum_buffer'] = torch.zeros_like(p)
 
                     if grad.is_sparse:
-                        state['accumulator_0'] = torch.zeros(shape[0])
+                        state['accumulator_0'] = torch.zeros(shape[0], dtype=grad.dtype, device=grad.device)
                     elif rank == 0:
-                        state['accumulator_0'] = torch.zeros(shape)
+                        state['accumulator_0'] = torch.zeros_like(p)
                     else:
                         for i in range(rank):
-                            state[f'accumulator_{i}'] = torch.zeros([1] * i + [shape[i]] + [1] * (rank - 1 - i))
+                            state[f'accumulator_{i}'] = torch.zeros(
+                                [1] * i + [shape[i]] + [1] * (rank - 1 - i), dtype=grad.dtype, device=grad.device
+                            )
 
                 state['step'] += 1
 
                 if grad.is_sparse:
                     grad = grad.coalesce()
 
                     acc = state['accumulator_0']
```

### Comparing `pytorch_optimizer-2.6.0/pytorch_optimizer/optimizer/utils.py` & `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.0/PKG-INFO` & `pytorch_optimizer-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-optimizer
-Version: 2.6.0
+Version: 2.6.1
 Summary: optimizer & lr scheduler implementations in PyTorch with clean-code, strict types. Also, including useful optimization ideas.
 Home-page: https://github.com/kozistr/pytorch_optimizer
 License: Apache-2.0
 Keywords: pytorch,deep-learning,optimizer,lr scheduler
 Author: kozistr
 Author-email: kozistr@gmail.com
 Maintainer: kozistr
```

